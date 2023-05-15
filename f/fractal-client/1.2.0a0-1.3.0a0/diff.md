# Comparing `tmp/fractal_client-1.2.0a0.tar.gz` & `tmp/fractal_client-1.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-1.2.0a0.tar", max compression
+gzip compressed data, was "fractal_client-1.3.0a0.tar", max compression
```

## Comparing `fractal_client-1.2.0a0.tar` & `fractal_client-1.3.0a0.tar`

### file list

```diff
@@ -1,84 +1,93 @@
--rw-r--r--   0        0        0     1576 2023-01-24 13:38:35.992771 fractal_client-1.2.0a0/LICENSE
--rw-r--r--   0        0        0     2619 2023-02-21 11:48:17.528833 fractal_client-1.2.0a0/README.md
--rw-r--r--   0        0        0       24 2023-04-06 13:06:33.921838 fractal_client-1.2.0a0/fractal/__init__.py
--rw-r--r--   0        0        0      124 2023-01-24 13:38:35.992771 fractal_client-1.2.0a0/fractal/__main__.py
--rw-r--r--   0        0        0     3308 2023-03-07 10:20:25.689818 fractal_client-1.2.0a0/fractal/authclient.py
--rw-r--r--   0        0        0     3607 2023-02-21 10:48:25.467156 fractal_client-1.2.0a0/fractal/client.py
--rw-r--r--   0        0        0     7295 2023-03-15 14:37:28.093556 fractal_client-1.2.0a0/fractal/cmd/__init__.py
--rw-r--r--   0        0        0     4750 2023-03-15 12:00:23.815956 fractal_client-1.2.0a0/fractal/cmd/_dataset.py
--rw-r--r--   0        0        0     4633 2023-02-24 10:01:10.056439 fractal_client-1.2.0a0/fractal/cmd/_job.py
--rw-r--r--   0        0        0     5091 2023-04-06 13:06:04.654184 fractal_client-1.2.0a0/fractal/cmd/_project.py
--rw-r--r--   0        0        0     5377 2023-03-07 10:20:30.985750 fractal_client-1.2.0a0/fractal/cmd/_task.py
--rw-r--r--   0        0        0     4463 2023-04-06 13:06:04.654184 fractal_client-1.2.0a0/fractal/cmd/_user.py
--rw-r--r--   0        0        0     8392 2023-03-07 10:20:30.985750 fractal_client-1.2.0a0/fractal/cmd/_workflow.py
--rw-r--r--   0        0        0     2413 2023-02-20 15:10:43.839845 fractal_client-1.2.0a0/fractal/cmd/utils.py
--rw-r--r--   0        0        0       42 2023-02-21 08:49:25.750218 fractal_client-1.2.0a0/fractal/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:20.997699 fractal_client-1.2.0a0/fractal/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-21 08:49:27.594201 fractal_client-1.2.0a0/fractal/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:21.001699 fractal_client-1.2.0a0/fractal/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-21 08:49:27.594201 fractal_client-1.2.0a0/fractal/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:21.001699 fractal_client-1.2.0a0/fractal/common/README.md
--rw-r--r--   0        0        0        0 2023-02-21 08:49:27.594201 fractal_client-1.2.0a0/fractal/common/__init__.py
--rw-r--r--   0        0        0      149 2023-02-21 10:13:04.505672 fractal_client-1.2.0a0/fractal/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      147 2023-03-16 09:04:47.705157 fractal_client-1.2.0a0/fractal/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       48 2023-03-06 13:52:21.001699 fractal_client-1.2.0a0/fractal/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-21 08:49:27.594201 fractal_client-1.2.0a0/fractal/common/schemas/__init__.py
--rw-r--r--   0        0        0      374 2023-02-21 10:13:04.505672 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      372 2023-03-16 09:04:47.705157 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      490 2023-03-03 14:13:42.839064 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1253 2023-03-06 14:43:01.309210 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1251 2023-03-16 09:04:47.793156 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc
--rw-r--r--   0        0        0     2035 2023-03-06 13:52:30.237594 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2027 2023-03-16 09:04:47.705157 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc
--rw-r--r--   0        0        0     3527 2023-02-21 10:13:04.645671 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-03-16 09:04:47.797156 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc
--rw-r--r--   0        0        0     3701 2023-03-15 12:01:05.691490 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     3711 2023-03-16 09:04:47.797156 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0     1191 2023-03-06 14:07:54.286234 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1185 2023-03-16 09:04:47.801156 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/state.cpython-39.pyc
--rw-r--r--   0        0        0     4998 2023-03-06 13:52:30.321592 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     4994 2023-03-16 09:04:47.805156 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/task.cpython-39.pyc
--rw-r--r--   0        0        0     1002 2023-03-06 13:52:30.325592 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1024 2023-03-16 09:04:47.809156 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     3513 2023-03-06 14:38:40.632474 fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 11:30:39.096144 fractal_client-1.2.0a0/fractal/common/schemas/_validators.py
--rw-r--r--   0        0        0     1716 2023-03-06 13:52:21.001699 fractal_client-1.2.0a0/fractal/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-21 08:49:27.594201 fractal_client-1.2.0a0/fractal/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-04-06 11:30:39.096144 fractal_client-1.2.0a0/fractal/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-03-06 14:07:44.150418 fractal_client-1.2.0a0/fractal/common/schemas/state.py
--rw-r--r--   0        0        0     4484 2023-03-06 13:52:21.001699 fractal_client-1.2.0a0/fractal/common/schemas/task.py
--rw-r--r--   0        0        0      998 2023-04-06 11:30:39.096144 fractal_client-1.2.0a0/fractal/common/schemas/user.py
--rw-r--r--   0        0        0     2709 2023-04-06 11:30:39.096144 fractal_client-1.2.0a0/fractal/common/schemas/workflow.py
--rw-r--r--   0        0        0      415 2023-03-06 13:52:30.189594 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      415 2023-03-07 09:47:31.002846 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1578 2023-03-06 13:52:30.221594 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1578 2023-03-07 09:47:31.038845 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3382 2023-03-15 10:53:32.644401 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      859 2023-03-06 13:52:30.469591 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      859 2023-03-07 09:47:31.354842 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-03-06 13:52:30.469591 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1258 2023-03-15 10:53:32.648401 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1763 2023-03-06 14:08:06.438014 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1763 2023-03-07 09:47:31.358842 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2222 2023-03-06 13:52:30.473591 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2222 2023-03-07 09:47:31.358842 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1317 2023-03-06 13:52:30.473591 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1317 2023-03-07 09:47:31.358842 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2579 2023-03-06 14:43:41.164713 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2579 2023-03-07 09:47:31.362842 fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      139 2023-03-06 13:52:21.001699 fractal_client-1.2.0a0/fractal/common/tests/conftest.py
--rw-r--r--   0        0        0     1065 2023-03-06 13:52:21.001699 fractal_client-1.2.0a0/fractal/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-14 13:42:31.592919 fractal_client-1.2.0a0/fractal/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-03-06 13:52:21.001699 fractal_client-1.2.0a0/fractal/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 11:30:39.096144 fractal_client-1.2.0a0/fractal/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 14:07:44.150418 fractal_client-1.2.0a0/fractal/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-03-06 13:52:21.001699 fractal_client-1.2.0a0/fractal/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-04-06 11:30:39.096144 fractal_client-1.2.0a0/fractal/common/tests/test_user.py
--rw-r--r--   0        0        0     2838 2023-04-06 11:30:39.096144 fractal_client-1.2.0a0/fractal/common/tests/test_workflow.py
--rw-r--r--   0        0        0     1285 2023-02-13 07:58:20.733904 fractal_client-1.2.0a0/fractal/config.py
--rw-r--r--   0        0        0     1609 2023-01-24 13:38:35.996771 fractal_client-1.2.0a0/fractal/interface.py
--rw-r--r--   0        0        0    20730 2023-04-06 13:06:04.654184 fractal_client-1.2.0a0/fractal/parser.py
--rw-r--r--   0        0        0     1265 2023-02-03 10:03:12.204782 fractal_client-1.2.0a0/fractal/response.py
--rw-r--r--   0        0        0     1824 2023-04-06 13:06:33.917838 fractal_client-1.2.0a0/pyproject.toml
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 fractal_client-1.2.0a0/setup.py
--rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 fractal_client-1.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-05-09 19:58:57.312677 fractal_client-1.3.0a0/LICENSE
+-rw-r--r--   0        0        0     2619 2023-05-09 19:58:57.312677 fractal_client-1.3.0a0/README.md
+-rw-r--r--   0        0        0       24 2023-05-15 12:57:11.406870 fractal_client-1.3.0a0/fractal/__init__.py
+-rw-r--r--   0        0        0      124 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/__main__.py
+-rw-r--r--   0        0        0     3448 2023-05-12 13:35:21.647646 fractal_client-1.3.0a0/fractal/authclient.py
+-rw-r--r--   0        0        0     3607 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/client.py
+-rw-r--r--   0        0        0     7424 2023-05-15 12:45:04.215004 fractal_client-1.3.0a0/fractal/cmd/__init__.py
+-rw-r--r--   0        0        0     5846 2023-05-12 13:17:45.698886 fractal_client-1.3.0a0/fractal/cmd/_dataset.py
+-rw-r--r--   0        0        0     5169 2023-05-15 12:45:04.215004 fractal_client-1.3.0a0/fractal/cmd/_job.py
+-rw-r--r--   0        0        0     4116 2023-05-12 13:17:45.698886 fractal_client-1.3.0a0/fractal/cmd/_project.py
+-rw-r--r--   0        0        0     5393 2023-05-12 13:17:45.698886 fractal_client-1.3.0a0/fractal/cmd/_task.py
+-rw-r--r--   0        0        0     4463 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/cmd/_user.py
+-rw-r--r--   0        0        0     8885 2023-05-12 13:18:41.370093 fractal_client-1.3.0a0/fractal/cmd/_workflow.py
+-rw-r--r--   0        0        0     2413 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/cmd/utils.py
+-rw-r--r--   0        0        0       42 2023-02-21 08:49:25.750218 fractal_client-1.3.0a0/fractal/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:20.997699 fractal_client-1.3.0a0/fractal/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/__init__.py
+-rw-r--r--   0        0        0      149 2023-02-21 10:13:04.505672 fractal_client-1.3.0a0/fractal/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      147 2023-03-16 09:04:47.705157 fractal_client-1.3.0a0/fractal/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       48 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/schemas/__init__.py
+-rw-r--r--   0        0        0      374 2023-02-21 10:13:04.505672 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      372 2023-03-16 09:04:47.705157 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      490 2023-03-03 14:13:42.839064 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1753 2023-04-20 07:56:22.895496 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1251 2023-03-16 09:04:47.793156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc
+-rw-r--r--   0        0        0     1589 2023-05-11 16:08:00.511429 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2027 2023-03-16 09:04:47.705157 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc
+-rw-r--r--   0        0        0     3527 2023-02-21 10:13:04.645671 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-03-16 09:04:47.797156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc
+-rw-r--r--   0        0        0     3598 2023-04-20 07:56:22.903496 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     3711 2023-03-16 09:04:47.797156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0     1191 2023-03-06 14:07:54.286234 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1185 2023-03-16 09:04:47.801156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/state.cpython-39.pyc
+-rw-r--r--   0        0        0     4929 2023-05-09 20:00:39.843482 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     4994 2023-03-16 09:04:47.805156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/task.cpython-39.pyc
+-rw-r--r--   0        0        0     1121 2023-05-11 16:08:00.523429 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1024 2023-03-16 09:04:47.809156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     3943 2023-05-11 16:08:00.527429 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 11:30:39.096144 fractal_client-1.3.0a0/fractal/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1044 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-04-06 11:30:39.096144 fractal_client-1.3.0a0/fractal/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-03-06 14:07:44.150418 fractal_client-1.3.0a0/fractal/common/schemas/state.py
+-rw-r--r--   0        0        0     4323 2023-05-09 20:00:26.031645 fractal_client-1.3.0a0/fractal/common/schemas/task.py
+-rw-r--r--   0        0        0      980 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/schemas/user.py
+-rw-r--r--   0        0        0     2502 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/schemas/workflow.py
+-rw-r--r--   0        0        0      415 2023-03-06 13:52:30.189594 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      415 2023-03-07 09:47:31.002846 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      415 2023-04-20 07:57:03.191274 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1578 2023-03-06 13:52:30.221594 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1578 2023-03-07 09:47:31.038845 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      606 2023-05-15 11:49:28.546463 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3382 2023-03-15 10:53:32.644401 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3382 2023-04-20 07:57:03.471272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      859 2023-03-06 13:52:30.469591 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      859 2023-03-07 09:47:31.354842 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      859 2023-04-20 07:57:03.471272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-06 13:52:30.469591 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1164 2023-04-20 07:56:23.111495 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1164 2023-04-20 07:57:03.471272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1763 2023-03-06 14:08:06.438014 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1763 2023-03-07 09:47:31.358842 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1763 2023-04-20 07:57:03.471272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2222 2023-03-06 13:52:30.473591 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2222 2023-03-07 09:47:31.358842 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2222 2023-04-20 07:57:03.475272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1317 2023-03-06 13:52:30.473591 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2213 2023-04-20 07:56:23.115495 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2213 2023-04-20 07:57:03.479272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2579 2023-03-06 14:43:41.164713 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3032 2023-04-20 07:56:23.115495 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2911 2023-05-15 11:49:28.882460 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-14 13:42:31.592919 fractal_client-1.3.0a0/fractal/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 11:30:39.096144 fractal_client-1.3.0a0/fractal/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 14:07:44.150418 fractal_client-1.3.0a0/fractal/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-04-06 11:30:39.096144 fractal_client-1.3.0a0/fractal/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/tests/test_workflow.py
+-rw-r--r--   0        0        0     1285 2023-05-12 13:33:57.004876 fractal_client-1.3.0a0/fractal/config.py
+-rw-r--r--   0        0        0     1609 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/interface.py
+-rw-r--r--   0        0        0    21649 2023-05-15 12:45:04.215004 fractal_client-1.3.0a0/fractal/parser.py
+-rw-r--r--   0        0        0     1265 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/response.py
+-rw-r--r--   0        0        0     1824 2023-05-15 12:57:11.406870 fractal_client-1.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 fractal_client-1.3.0a0/setup.py
+-rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 fractal_client-1.3.0a0/PKG-INFO
```

### Comparing `fractal_client-1.2.0a0/LICENSE` & `fractal_client-1.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/README.md` & `fractal_client-1.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/authclient.py` & `fractal_client-1.3.0a0/fractal/authclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from json import JSONDecodeError
 from pathlib import Path
 
 import jwt
 from httpx import AsyncClient
 from jwt.exceptions import ExpiredSignatureError
 
 from .config import settings
@@ -33,17 +34,21 @@
             username=self.username,
             password=self.password,
         )
         res = await self.client.post(
             f"{settings.FRACTAL_SERVER}/auth/token/login", data=data
         )
         if res.status_code != 200:
+            try:
+                data = res.json()
+            except JSONDecodeError:
+                data = ""
             raise AuthenticationError(
                 "Error: could not obtain token. Is the user registered?\n"
-                f"{res.json()}\n"
+                f"{data}\n"
             )
         raw_token = res.json()
         self.token = raw_token["access_token"]
 
         # Create cache folder, if needed
         cache_dir = Path(f"{settings.FRACTAL_CACHE_PATH}").expanduser()
         cache_dir.mkdir(parents=True, exist_ok=True)
```

### Comparing `fractal_client-1.2.0a0/fractal/client.py` & `fractal_client-1.3.0a0/fractal/client.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/cmd/__init__.py` & `fractal_client-1.3.0a0/fractal/cmd/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,163 +1,165 @@
 from httpx import AsyncClient
 
 from ..authclient import AuthClient
 from ..config import __VERSION__
 from ..config import settings
 from ..interface import BaseInterface
 from ..interface import PrintInterface
-from ._dataset import dataset_add_resource
-from ._dataset import dataset_delete
-from ._dataset import dataset_delete_resource
-from ._dataset import dataset_edit
-from ._dataset import dataset_show
-from ._job import job_download_logs
-from ._job import job_list
-from ._job import job_show
-from ._project import project_add_dataset
-from ._project import project_create
-from ._project import project_delete
-from ._project import project_edit
-from ._project import project_list
-from ._project import project_show
+from ._dataset import delete_dataset
+from ._dataset import delete_resource
+from ._dataset import get_dataset
+from ._dataset import patch_dataset
+from ._dataset import post_dataset
+from ._dataset import post_resource
+from ._job import get_job
+from ._job import get_job_list
+from ._job import get_job_logs
+from ._job import stop_job
+from ._project import delete_project
+from ._project import get_project
+from ._project import get_project_list
+from ._project import patch_project
+from ._project import post_project
+from ._task import delete_task
+from ._task import get_task_list
+from ._task import patch_task
+from ._task import post_task
 from ._task import task_collect_pip
 from ._task import task_collection_check
-from ._task import task_delete
-from ._task import task_edit
-from ._task import task_list
-from ._task import task_new
 from ._user import user_delete
 from ._user import user_edit
 from ._user import user_list
 from ._user import user_register
 from ._user import user_show
 from ._user import user_whoami
-from ._workflow import workflow_add_task
+from ._workflow import delete_workflow
+from ._workflow import delete_workflowtask
+from ._workflow import get_workflow
+from ._workflow import get_workflow_list
+from ._workflow import patch_workflow
+from ._workflow import patch_workflowtask
+from ._workflow import post_workflow
+from ._workflow import post_workflowtask
 from ._workflow import workflow_apply
-from ._workflow import workflow_delete
-from ._workflow import workflow_edit
-from ._workflow import workflow_edit_task
 from ._workflow import workflow_export
 from ._workflow import workflow_import
-from ._workflow import workflow_list
-from ._workflow import workflow_new
-from ._workflow import workflow_remove_task
-from ._workflow import workflow_show
 
 
 class NoCommandError(ValueError):
     pass
 
 
 async def project(
     client: AuthClient, subcmd: str, batch: bool = False, **kwargs
 ) -> BaseInterface:
     if subcmd == "new":
-        iface = await project_create(client, batch=batch, **kwargs)
+        iface = await post_project(client, batch=batch, **kwargs)
     elif subcmd == "show":
-        iface = await project_show(client, **kwargs)
+        iface = await get_project(client, **kwargs)
     elif subcmd == "list":
-        iface = await project_list(client, **kwargs)
+        iface = await get_project_list(client, **kwargs)
     elif subcmd == "edit":
-        iface = await project_edit(client, **kwargs)
+        iface = await patch_project(client, **kwargs)
     elif subcmd == "add-dataset":
-        iface = await project_add_dataset(
+        iface = await post_dataset(
             client,
             batch=batch,
             project_id=kwargs.pop("project_id"),
             dataset_name=kwargs.pop("dataset_name"),
             metadata_filename=kwargs.pop("metadata"),
+            type=kwargs.pop("type"),
             **kwargs,
         )
     elif subcmd == "delete":
-        iface = await project_delete(client, **kwargs)
+        iface = await delete_project(client, **kwargs)
     else:
         raise NoCommandError(f"Command project {subcmd} not found")
 
     return iface
 
 
 async def dataset(
     client: AuthClient, subcmd: str, batch: bool = False, **kwargs
 ) -> BaseInterface:
     if subcmd == "show":
-        iface = await dataset_show(client, **kwargs)
+        iface = await get_dataset(client, **kwargs)
     elif subcmd == "add-resource":
-        iface = await dataset_add_resource(
+        iface = await post_resource(
             client,
             batch=batch,
             project_id=kwargs.pop("project_id"),
             dataset_id=kwargs.pop("dataset_id"),
             path=kwargs.pop("path"),
             **kwargs,
         )
     elif subcmd == "rm-resource":
-        iface = await dataset_delete_resource(
+        iface = await delete_resource(
             client,
             batch=batch,
             project_id=kwargs.pop("project_id"),
             dataset_id=kwargs.pop("dataset_id"),
             resource_id=kwargs.pop("resource_id"),
             **kwargs,
         )
     elif subcmd == "edit":
         project_id = int(kwargs.pop("project_id"))
         dataset_id = int(kwargs.pop("dataset_id"))
-        iface = await dataset_edit(
+        iface = await patch_dataset(
             client,
             project_id=project_id,
             dataset_id=dataset_id,
             **kwargs,
         )
     elif subcmd == "delete":
-        iface = await dataset_delete(client, **kwargs)
+        iface = await delete_dataset(client, **kwargs)
     else:
         raise NoCommandError(f"Command dataset {subcmd} not found")
     return iface
 
 
 async def task(
     client: AuthClient, subcmd: str, batch: bool = False, **kwargs
 ) -> BaseInterface:
     if subcmd == "list":
-        iface = await task_list(client, **kwargs)
+        iface = await get_task_list(client, **kwargs)
     elif subcmd == "collect":
         iface = await task_collect_pip(client, batch=batch, **kwargs)
     elif subcmd == "check-collection":
         iface = await task_collection_check(client, **kwargs)
     elif subcmd == "new":
-        iface = await task_new(client, batch=batch, **kwargs)
+        iface = await post_task(client, batch=batch, **kwargs)
     elif subcmd == "edit":
-        iface = await task_edit(client, **kwargs)
+        iface = await patch_task(client, **kwargs)
     elif subcmd == "delete":
-        iface = await task_delete(client, **kwargs)
+        iface = await delete_task(client, **kwargs)
     else:
         raise NoCommandError(f"Command task {subcmd} not found")
     return iface
 
 
 async def workflow(
     client: AuthClient, subcmd: str, batch: bool = False, **kwargs
 ) -> BaseInterface:
     if subcmd == "show":
-        iface = await workflow_show(client, **kwargs)
+        iface = await get_workflow(client, **kwargs)
     elif subcmd == "new":
-        iface = await workflow_new(client, batch=batch, **kwargs)
+        iface = await post_workflow(client, batch=batch, **kwargs)
     elif subcmd == "list":
-        iface = await workflow_list(client, batch=batch, **kwargs)
+        iface = await get_workflow_list(client, batch=batch, **kwargs)
     elif subcmd == "edit":
-        iface = await workflow_edit(client, **kwargs)
+        iface = await patch_workflow(client, **kwargs)
     elif subcmd == "delete":
-        iface = await workflow_delete(client, **kwargs)
+        iface = await delete_workflow(client, **kwargs)
     elif subcmd == "add-task":
-        iface = await workflow_add_task(client, batch=batch, **kwargs)
+        iface = await post_workflowtask(client, batch=batch, **kwargs)
     elif subcmd == "edit-task":
-        iface = await workflow_edit_task(client, **kwargs)
+        iface = await patch_workflowtask(client, **kwargs)
     elif subcmd == "rm-task":
-        iface = await workflow_remove_task(client, **kwargs)
+        iface = await delete_workflowtask(client, **kwargs)
     elif subcmd == "apply":
         iface = await workflow_apply(client, **kwargs)
     elif subcmd == "import":
         iface = await workflow_import(client, batch=batch, **kwargs)
     elif subcmd == "export":
         iface = await workflow_export(client, **kwargs)
     else:
@@ -165,19 +167,21 @@
     return iface
 
 
 async def job(
     client: AuthClient, subcmd: str, batch: bool = False, **kwargs
 ) -> BaseInterface:
     if subcmd == "list":
-        iface = await job_list(client, batch=batch, **kwargs)
+        iface = await get_job_list(client, batch=batch, **kwargs)
     elif subcmd == "show":
-        iface = await job_show(client, batch=batch, **kwargs)
+        iface = await get_job(client, batch=batch, **kwargs)
     elif subcmd == "download-logs":
-        iface = await job_download_logs(client, **kwargs)
+        iface = await get_job_logs(client, **kwargs)
+    elif subcmd == "stop":
+        iface = await stop_job(client, batch=batch, **kwargs)
     else:
         raise NoCommandError(f"Command job {subcmd} not found")
     return iface
 
 
 async def version(client: AsyncClient, **kwargs) -> PrintInterface:
     res = await client.get(f"{settings.FRACTAL_SERVER}/api/alive/")
```

### Comparing `fractal_client-1.2.0a0/fractal/cmd/_dataset.py` & `fractal_client-1.3.0a0/fractal/cmd/_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,62 @@
 import json
 import os
 from typing import Optional
 
 from rich.table import Table
 
 from ..authclient import AuthClient
+from ..common.schemas import DatasetCreate
 from ..common.schemas import DatasetRead
 from ..common.schemas import DatasetUpdate
 from ..common.schemas import ResourceCreate
 from ..common.schemas import ResourceRead
 from ..config import settings
 from ..interface import BaseInterface
 from ..interface import PrintInterface
 from ..interface import RichConsoleInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
 
 
-async def dataset_add_resource(
+async def post_dataset(
+    client: AuthClient,
+    project_id: int,
+    dataset_name: str,
+    metadata_filename: Optional[str] = None,
+    type: Optional[str] = None,
+    batch: bool = False,
+    **kwargs,
+) -> RichJsonInterface:
+
+    if metadata_filename is None:
+        meta = {}
+    else:
+        with open(metadata_filename, "r") as f:
+            meta = json.load(f)
+
+    dataset_dict = dict(name=dataset_name, meta=meta)
+    if type:
+        dataset_dict["type"] = type
+    dataset = DatasetCreate(**dataset_dict)
+
+    res = await client.post(
+        f"{settings.BASE_URL}/project/{project_id}/dataset/",
+        json=dataset.dict(exclude_unset=True),
+    )
+    new_dataset = check_response(
+        res, expected_status_code=201, coerce=DatasetRead
+    )
+    if batch:
+        return PrintInterface(retcode=0, data=new_dataset.id)
+    else:
+        return RichJsonInterface(retcode=0, data=new_dataset.dict())
+
+
+async def post_resource(
     client: AuthClient,
     *,
     batch: bool = False,
     project_id: int,
     dataset_id: int,
     path: str,
     **kwargs,
@@ -32,42 +67,48 @@
     if not os.path.isabs(path):
         msg = f"{path=} is not an absolute path"
         raise ValueError(msg)
 
     resource = ResourceCreate(path=path)
 
     res = await client.post(
-        f"{settings.BASE_URL}/project/{project_id}/{dataset_id}",
+        (
+            f"{settings.BASE_URL}/project/{project_id}/"
+            f"dataset/{dataset_id}/resource/"
+        ),
         json=resource.dict(),
     )
     new_resource = check_response(
         res, expected_status_code=201, coerce=ResourceRead
     )
     if batch:
         return PrintInterface(retcode=0, data=new_resource.id)
     else:
         return RichJsonInterface(retcode=0, data=new_resource.dict())
 
 
-async def dataset_delete_resource(
+async def delete_resource(
     client: AuthClient,
     *,
     project_id: int,
     dataset_id: int,
     resource_id: int,
     **kwargs,
 ) -> BaseInterface:
     res = await client.delete(
-        f"{settings.BASE_URL}/project/{project_id}/{dataset_id}/{resource_id}"
+        (
+            f"{settings.BASE_URL}/project/{project_id}/"
+            f"dataset/{dataset_id}/resource/{resource_id}"
+        )
     )
     check_response(res, expected_status_code=204)
     return PrintInterface(retcode=0, data="")
 
 
-async def dataset_edit(
+async def patch_dataset(
     client: AuthClient,
     *,
     project_id: int,
     dataset_id: int,
     new_name: Optional[str] = None,
     new_type: Optional[str] = None,
     meta_file: Optional[str] = None,
@@ -93,28 +134,28 @@
     dataset_update = DatasetUpdate(**dataset_update_dict)
     payload = dataset_update.dict(exclude_unset=True)
 
     if not payload:
         return PrintInterface(retcode=1, data="Nothing to update")
 
     res = await client.patch(
-        f"{settings.BASE_URL}/project/{project_id}/{dataset_id}",
+        (f"{settings.BASE_URL}/project/{project_id}/" f"dataset/{dataset_id}"),
         json=payload,
     )
     new_dataset = check_response(
         res, expected_status_code=200, coerce=DatasetRead
     )
     return RichJsonInterface(retcode=0, data=new_dataset.dict())
 
 
-async def dataset_show(
+async def get_dataset(
     client: AuthClient, *, project_id: int, dataset_id: int, **kwargs
 ) -> BaseInterface:
     res = await client.get(
-        f"{settings.BASE_URL}/project/{project_id}/{dataset_id}"
+        f"{settings.BASE_URL}/project/{project_id}/dataset/{dataset_id}"
     )
     from rich.console import Group
 
     dataset = check_response(res, expected_status_code=200, coerce=DatasetRead)
 
     if kwargs.get("json", False):
         return RichJsonInterface(retcode=0, data=dataset.dict())
@@ -139,16 +180,16 @@
         table_res.add_column("Dataset ID", justify="center", style="yellow")
         for r in dataset.resource_list:
             table_res.add_row(r.path, str(r.id), str(r.dataset_id))
         group = Group(table, table_res)
         return RichConsoleInterface(retcode=0, data=group)
 
 
-async def dataset_delete(
+async def delete_dataset(
     client: AuthClient, project_id: int, dataset_id: int, **kwargs
 ) -> PrintInterface:
 
     res = await client.delete(
-        f"{settings.BASE_URL}/project/{project_id}/{dataset_id}"
+        f"{settings.BASE_URL}/project/{project_id}/dataset/{dataset_id}"
     )
     check_response(res, expected_status_code=204)
     return PrintInterface(retcode=0, data="")
```

### Comparing `fractal_client-1.2.0a0/fractal/cmd/_job.py` & `fractal_client-1.3.0a0/fractal/cmd/_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 from ..interface import BaseInterface
 from ..interface import PrintInterface
 from ..interface import RichConsoleInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
 
 
-async def job_show(
+async def get_job(
     client: AuthClient,
+    project_id: int,
     job_id: int,
     batch: bool = False,
     do_not_separate_logs: bool = False,
     **kwargs,
 ) -> BaseInterface:
     """
     Query the status of a workflow-execution job
     """
 
-    res = await client.get(f"{settings.BASE_URL}/job/{job_id}")
+    res = await client.get(
+        f"{settings.BASE_URL}/project/{project_id}/job/{job_id}"
+    )
     job = check_response(
         res, expected_status_code=200, coerce=ApplyWorkflowRead
     )
     if batch:
         return PrintInterface(retcode=0, data=job.status)
     else:
         data = job.sanitised_dict()
@@ -40,22 +43,22 @@
             log = data.pop("log")
             extra_lines = ["\nThis is the job log:\n", log]
             return RichJsonInterface(
                 retcode=0, data=data, extra_lines=extra_lines
             )
 
 
-async def job_list(
+async def get_job_list(
     client: AuthClient,
     project_id: int,
     batch: bool = False,
     **kwargs,
 ) -> BaseInterface:
 
-    res = await client.get(f"{settings.BASE_URL}/project/{project_id}/jobs/")
+    res = await client.get(f"{settings.BASE_URL}/project/{project_id}/job/")
     jobs = check_response(res, expected_status_code=200)
 
     # Coerce to a list of ApplyWorkflowRead objects
     jobs = [ApplyWorkflowRead(**job) for job in jobs]
 
     if batch:
         job_ids = " ".join(str(job.id) for job in jobs)
@@ -77,29 +80,32 @@
                 j.status,
                 str(j.workflow_id),
                 j.working_dir,
             )
         return RichConsoleInterface(retcode=0, data=table)
 
 
-async def job_download_logs(
+async def get_job_logs(
     client: AuthClient,
+    project_id: int,
     job_id: int,
     output_folder: str,
     **kwargs,
 ) -> BaseInterface:
 
     # Check that output_folder does not already exist
     if Path(output_folder).exists():
         return PrintInterface(
             retcode=1, data=f"ERROR: {output_folder=} already exists"
         )
 
     # Send request to server
-    res = await client.get(f"{settings.BASE_URL}/job/download/{job_id}")
+    res = await client.get(
+        f"{settings.BASE_URL}/project/{project_id}/job/{job_id}/download/"
+    )
 
     # NOTE: We cannot use our default check_response here, because res._content
     # is binary. Therefore we check the status code by hand
     if res.status_code != 200:
         logging.error(f"Server returned {res.status_code}")
         logging.error(
             f"Original request: {res._request.method} {res._request.url}"
@@ -140,7 +146,26 @@
 
     # Remove zipped temporary file
     os.unlink(zipped_archive_path)
 
     return PrintInterface(
         retcode=0, data=f"Logs downloaded to {output_folder=}"
     )
+
+
+async def stop_job(
+    client: AuthClient,
+    project_id: int,
+    job_id: int,
+    **kwargs,
+) -> BaseInterface:
+    """
+    Stop a workflow-execution job
+    """
+
+    res = await client.get(
+        f"{settings.BASE_URL}/project/{project_id}/job/{job_id}/stop/"
+    )
+    check_response(res, expected_status_code=200)
+    return PrintInterface(
+        retcode=0, data="Correctly called the job-stopping endpoint"
+    )
```

### Comparing `fractal_client-1.2.0a0/fractal/cmd/_project.py` & `fractal_client-1.3.0a0/fractal/cmd/_project.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-import json
 import logging
 from typing import Optional
 from typing import Union
 
 from rich.table import Table
 
 from ..authclient import AuthClient
-from ..common.schemas import DatasetCreate
-from ..common.schemas import DatasetRead
 from ..common.schemas import ProjectCreate
 from ..common.schemas import ProjectRead
 from ..common.schemas import ProjectUpdate
 from ..config import settings
 from ..interface import BaseInterface
 from ..interface import PrintInterface
 from ..interface import RichConsoleInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
 
 
-async def project_create(
+async def post_project(
     client: AuthClient,
     name: str,
     dataset: Optional[str] = None,
     batch: bool = False,
     **kwargs,
 ) -> BaseInterface:
     # Prepare a ProjectCreate request body
@@ -47,15 +44,17 @@
             raise ValueError(msg)
         dataset_id = project.dataset_list[0].id
         return PrintInterface(retcode=0, data=f"{project.id} {dataset_id}")
     else:
         return RichJsonInterface(retcode=0, data=project.dict())
 
 
-async def project_list(client: AuthClient, **kwargs) -> RichConsoleInterface:
+async def get_project_list(
+    client: AuthClient, **kwargs
+) -> RichConsoleInterface:
 
     res = await client.get(f"{settings.BASE_URL}/project/")
     res = check_response(res, expected_status_code=200)
 
     projects = [ProjectRead(**item) for item in res]
 
     table = Table(title="Project List")
@@ -80,69 +79,36 @@
             str(p_dataset_list),
             read_only_icon,
         )
 
     return RichConsoleInterface(retcode=0, data=table)
 
 
-async def project_show(
+async def get_project(
     client: AuthClient, project_id: int, **kwargs
 ) -> RichJsonInterface:
     res = await client.get(
         f"{settings.BASE_URL}/project/{project_id}",
     )
     project = check_response(res, expected_status_code=200, coerce=ProjectRead)
     return RichJsonInterface(retcode=0, data=project.dict())
 
 
-async def project_add_dataset(
-    client: AuthClient,
-    project_id: int,
-    dataset_name: str,
-    metadata_filename: Optional[str] = None,
-    type: Optional[str] = None,
-    batch: bool = False,
-    **kwargs,
-) -> RichJsonInterface:
-
-    if metadata_filename is None:
-        meta = {}
-    else:
-        meta = json.loads(metadata_filename)
-
-    dataset_dict = dict(name=dataset_name, meta=meta)
-    if type:
-        dataset_dict["type"] = type
-    dataset = DatasetCreate(**dataset_dict)
-
-    res = await client.post(
-        f"{settings.BASE_URL}/project/{project_id}/",
-        json=dataset.dict(exclude_unset=True),
-    )
-    new_dataset = check_response(
-        res, expected_status_code=201, coerce=DatasetRead
-    )
-    if batch:
-        return PrintInterface(retcode=0, data=new_dataset.id)
-    else:
-        return RichJsonInterface(retcode=0, data=new_dataset.dict())
-
-
-async def project_delete(
+async def delete_project(
     client: AuthClient, project_id: int, **kwargs
 ) -> PrintInterface:
 
     res = await client.delete(
         f"{settings.BASE_URL}/project/{project_id}",
     )
     check_response(res, expected_status_code=204)
     return PrintInterface(retcode=0, data="")
 
 
-async def project_edit(
+async def patch_project(
     client: AuthClient,
     project_id: int,
     new_name: Optional[str] = None,
     make_read_only: bool = False,
     remove_read_only: bool = False,
     **kwargs,
 ) -> Union[RichJsonInterface, PrintInterface]:
```

### Comparing `fractal_client-1.2.0a0/fractal/cmd/_task.py` & `fractal_client-1.3.0a0/fractal/cmd/_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..interface import PrintInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
 from .utils import get_cached_task_by_name
 from .utils import refresh_task_cache
 
 
-async def task_list(client: AuthClient, **kwargs) -> RichJsonInterface:
+async def get_task_list(client: AuthClient, **kwargs) -> RichJsonInterface:
     task_list = await refresh_task_cache(client=client, **kwargs)
     return RichJsonInterface(retcode=0, data=task_list)
 
 
 async def task_collect_pip(
     client: AuthClient,
     *,
@@ -81,15 +81,15 @@
         log = state_dict["data"].pop("log")
         extra_lines = ["\nThis is the task-collection log:\n", log]
         return RichJsonInterface(
             retcode=0, data=state_dict, extra_lines=extra_lines
         )
 
 
-async def task_new(
+async def post_task(
     client: AuthClient,
     *,
     name: str,
     command: str,
     source: str,
     batch: bool = False,
     input_type: Optional[str] = "Any",
@@ -118,15 +118,15 @@
 
     if batch:
         return PrintInterface(retcode=0, data=str(new_task.id))
     else:
         return RichJsonInterface(retcode=0, data=new_task.dict())
 
 
-async def task_edit(
+async def patch_task(
     client: AuthClient,
     *,
     task_id_or_name: str,
     name: Optional[str] = None,
     command: Optional[str] = None,
     input_type: Optional[str] = None,
     output_type: Optional[str] = None,
@@ -165,16 +165,16 @@
     res = await client.patch(
         f"{settings.BASE_URL}/task/{task_id}", json=payload
     )
     new_task = check_response(res, expected_status_code=200, coerce=TaskRead)
     return RichJsonInterface(retcode=0, data=new_task.dict())
 
 
-async def task_delete(
-    client: AuthClient, task_id: int, **kwargs
+async def delete_task(
+    client: AuthClient, *, task_id: int = None, **kwargs
 ) -> PrintInterface:
 
     raise NotImplementedError("task_delete")
 
     # res = await client.delete(
     #    f"{settings.BASE_URL}/xxxx"
     # )
```

### Comparing `fractal_client-1.2.0a0/fractal/cmd/_user.py` & `fractal_client-1.3.0a0/fractal/cmd/_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/cmd/_workflow.py` & `fractal_client-1.3.0a0/fractal/cmd/_workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,80 +18,87 @@
 from ..interface import BaseInterface
 from ..interface import PrintInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
 from .utils import get_cached_task_by_name
 
 
-async def workflow_new(
+async def post_workflow(
     client: AuthClient,
     name: str,
     project_id: int,
     batch: bool = False,
     **kwargs,
 ) -> BaseInterface:
     workflow = WorkflowCreate(
         name=name,
         project_id=project_id,
     )
     logging.info(workflow)
     res = await client.post(
-        f"{settings.BASE_URL}/workflow/",
+        f"{settings.BASE_URL}/project/{project_id}/workflow/",
         json=workflow.dict(),
     )
     workflow = check_response(
         res, expected_status_code=201, coerce=WorkflowRead
     )
     if batch:
         return PrintInterface(retcode=0, data=workflow.id)
     else:
         return RichJsonInterface(retcode=0, data=workflow.dict())
 
 
-async def workflow_list(
+async def get_workflow_list(
     client: AuthClient,
     project_id: int,
     batch: bool = False,
     **kwargs,
 ) -> RichJsonInterface:
 
     res = await client.get(
-        f"{settings.BASE_URL}/project/{project_id}/workflows/"
+        f"{settings.BASE_URL}/project/{project_id}/workflow/"
     )
     workflow_list = check_response(res, expected_status_code=200)
     return RichJsonInterface(retcode=0, data=workflow_list)
 
 
-async def workflow_delete(
+async def delete_workflow(
     client: AuthClient,
     *,
+    project_id: int,
     workflow_id: int,
     **kwargs,
 ) -> BaseInterface:
-    res = await client.delete(f"{settings.BASE_URL}/workflow/{workflow_id}")
+    res = await client.delete(
+        f"{settings.BASE_URL}/project/{project_id}/workflow/{workflow_id}"
+    )
     check_response(res, expected_status_code=204)
     return PrintInterface(retcode=0, data="")
 
 
-async def workflow_show(
+async def get_workflow(
     client: AuthClient,
     *,
+    project_id: int,
     workflow_id: int,
     **kwargs,
 ) -> RichJsonInterface:
-    res = await client.get(f"{settings.BASE_URL}/workflow/{workflow_id}")
+    res = await client.get(
+        f"{settings.BASE_URL}/project/{project_id}/workflow/{workflow_id}"
+    )
     workflow = check_response(
         res, expected_status_code=200, coerce=WorkflowRead
     )
     return RichJsonInterface(retcode=0, data=workflow.dict())
 
 
-async def workflow_add_task(
+async def post_workflowtask(
     client: AuthClient,
     *,
+    project_id: int,
     workflow_id: int,
     batch: bool = False,
     task_id_or_name: str,
     order: Optional[int] = None,
     args_file: Optional[str] = None,
     meta_file: Optional[str] = None,
     **kwargs,
@@ -99,43 +106,48 @@
 
     try:
         task_id = int(task_id_or_name)
     except ValueError:
         task_id = await get_cached_task_by_name(task_id_or_name, client)
 
     if order is None:
-        workflow_task = WorkflowTaskCreate(task_id=task_id)
+        workflow_task = WorkflowTaskCreate()
     else:
-        workflow_task = WorkflowTaskCreate(task_id=task_id, order=order)
+        workflow_task = WorkflowTaskCreate(order=order)
     if args_file:
         with Path(args_file).open("r") as f:
             args = json.load(f)
             workflow_task.args = args
     if meta_file:
         with Path(meta_file).open("r") as f:
             meta = json.load(f)
             workflow_task.meta = meta
 
     res = await client.post(
-        f"{settings.BASE_URL}/workflow/{workflow_id}/add-task/",
+        (
+            f"{settings.BASE_URL}/project/{project_id}/"
+            f"workflow/{workflow_id}/wftask/"
+            f"?{task_id=}"
+        ),
         json=workflow_task.dict(exclude_unset=True),
     )
     workflow_task = check_response(
         res, expected_status_code=201, coerce=WorkflowTaskRead
     )
 
     if batch:
         return PrintInterface(retcode=0, data=str(workflow_task.id))
     else:
         return RichJsonInterface(retcode=0, data=workflow_task.dict())
 
 
-async def workflow_edit_task(
+async def patch_workflowtask(
     client: AuthClient,
     *,
+    project_id: int,
     workflow_id: int,
     workflow_task_id: int,
     args_file: Optional[str] = None,
     meta_file: Optional[str] = None,
     **kwargs,
 ) -> RichJsonInterface:
 
@@ -156,88 +168,97 @@
     if meta_file:
         with Path(meta_file).open("r") as f:
             meta = json.load(f)
             payload["meta"] = meta
 
     payload_update = WorkflowTaskUpdate(**payload)
     res = await client.patch(
-        f"{settings.BASE_URL}/"
-        f"workflow/{workflow_id}/edit-task/{workflow_task_id}",
+        (
+            f"{settings.BASE_URL}/project/{project_id}/"
+            f"workflow/{workflow_id}/wftask/{workflow_task_id}"
+        ),
         json=payload_update.dict(exclude_unset=True),
     )
     workflow_task = check_response(
         res, expected_status_code=200, coerce=WorkflowTaskRead
     )
 
     return RichJsonInterface(retcode=0, data=workflow_task.dict())
 
 
-async def workflow_remove_task(
+async def delete_workflowtask(
     client: AuthClient,
     *,
+    project_id: int,
     workflow_id: int,
     workflow_task_id: int,
     **kwargs,
 ) -> BaseInterface:
 
     res = await client.delete(
-        f"{settings.BASE_URL}/"
-        f"workflow/{workflow_id}/rm-task/{workflow_task_id}"
+        f"{settings.BASE_URL}/project/{project_id}/"
+        f"workflow/{workflow_id}/wftask/{workflow_task_id}"
     )
     check_response(res, expected_status_code=204)
     return PrintInterface(retcode=0, data="")
 
 
-async def workflow_edit(
+async def patch_workflow(
     client: AuthClient,
     *,
+    project_id: int,
     workflow_id: int,
     **workflow_update_dict,
 ) -> BaseInterface:
     workflow_update = WorkflowUpdate(**workflow_update_dict)
     payload = workflow_update.dict(exclude_unset=True)
     if not payload:
         return PrintInterface(retcode=1, data="Nothing to update")
 
     res = await client.patch(
-        f"{settings.BASE_URL}/workflow/{workflow_id}", json=payload
+        f"{settings.BASE_URL}/project/{project_id}/workflow/{workflow_id}",
+        json=payload,
     )
     new_workflow = check_response(
         res, expected_status_code=200, coerce=WorkflowRead
     )
     return RichJsonInterface(retcode=0, data=new_workflow.dict())
 
 
 async def workflow_apply(
     client: AuthClient,
     *,
+    project_id: int,
     workflow_id: int,
     input_dataset_id: int,
     output_dataset_id: int,
-    # output_dataset_id: Optional[int] = None,
-    overwrite_input: bool = False,
-    project_id: Optional[int] = None,
     worker_init: Optional[str] = None,
     **kwargs,
 ) -> BaseInterface:
     apply_wf_create_dict = dict(
         workflow_id=workflow_id,
         input_dataset_id=input_dataset_id,
         output_dataset_id=output_dataset_id,
-        overwrite_input=overwrite_input,
     )
     # Prepare ApplyWorkflowCreate object, without None attributes
-    if project_id:
-        apply_wf_create_dict["project_id"] = project_id
     if worker_init:
         apply_wf_create_dict["worker_init"] = worker_init
     apply_wf_create = ApplyWorkflowCreate(**apply_wf_create_dict)
 
+    # Prepare query parameters
+    query_parameters = (
+        f"input_dataset_id={input_dataset_id}"
+        f"&output_dataset_id={output_dataset_id}"
+    )
+
     res = await client.post(
-        f"{settings.BASE_URL}/project/apply/",
+        (
+            f"{settings.BASE_URL}/project/{project_id}/workflow/{workflow_id}/"
+            f"apply/?{query_parameters}"
+        ),
         json=apply_wf_create.dict(exclude_unset=True),
     )
     apply_wf_read = check_response(
         res, expected_status_code=202, coerce=ApplyWorkflowRead
     )
     return RichJsonInterface(retcode=0, data=apply_wf_read.sanitised_dict())
 
@@ -250,15 +271,15 @@
     batch: bool = False,
     **kwargs,
 ) -> BaseInterface:
     with Path(json_file).open("r") as f:
         workflow = json.load(f)
     workflow = WorkflowImport(**workflow)
     res = await client.post(
-        f"{settings.BASE_URL}/project/{project_id}/import-workflow/",
+        f"{settings.BASE_URL}/project/{project_id}/workflow/import/",
         json=workflow.dict(exclude_unset=True),
     )
     wf_read = check_response(
         res, expected_status_code=201, coerce=WorkflowRead
     )
     if batch:
         datastr = f"{wf_read.id}"
@@ -268,20 +289,24 @@
     else:
         return RichJsonInterface(retcode=0, data=wf_read.dict())
 
 
 async def workflow_export(
     client: AuthClient,
     *,
+    project_id: int,
     workflow_id: int,
     json_file: str,
     **kwargs,
 ) -> BaseInterface:
     res = await client.get(
-        f"{settings.BASE_URL}/workflow/{workflow_id}/export/"
+        (
+            f"{settings.BASE_URL}/project/{project_id}/"
+            f"workflow/{workflow_id}/export/"
+        ),
     )
     workflow = check_response(
         res, expected_status_code=200, coerce=WorkflowExport
     )
     with Path(json_file).open("w") as f:
         json.dump(workflow.dict(), f, indent=2)
     return PrintInterface(
```

### Comparing `fractal_client-1.2.0a0/fractal/cmd/utils.py` & `fractal_client-1.3.0a0/fractal/cmd/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/.github/workflows/ci.yml` & `fractal_client-1.3.0a0/fractal/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/.pre-commit-config.yaml` & `fractal_client-1.3.0a0/fractal/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/README.md` & `fractal_client-1.3.0a0/fractal/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__init__.py` & `fractal_client-1.3.0a0/fractal/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 14:42:57 2023 UTC, .py size: 1015 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-00000000: 6f0d 0d0a 0000 0000 f1fb 0564 f703 0000  o..........d....
+00000000: 610d 0d0a 0000 0000 f1fb 0564 f703 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
-00000030: 6500 6602 6401 6402 8404 5a01 6408 6400  e.f.d.d...Z.d.d.
-00000040: 6500 6404 6502 6604 6405 6406 8405 5a03  e.d.e.f.d.d...Z.
-00000050: 6407 5300 2909 da09 6174 7472 6962 7574  d.S.)...attribut
+00000020: 0004 0000 0040 0000 0073 2400 0000 6500  .....@...s$...e.
+00000030: 6400 9c01 6401 6402 8404 5a01 6408 6500  d...d.d...Z.d.e.
+00000040: 6502 6404 9c02 6405 6406 8405 5a03 6407  e.d...d.d...Z.d.
+00000050: 5300 2909 a901 da09 6174 7472 6962 7574  S.).....attribut
 00000060: 6563 0100 0000 0000 0000 0000 0000 0200  ec..............
-00000070: 0000 0400 0000 0300 0000 7316 0000 0064  ..........s....d
-00000080: 0174 0066 0287 0066 0164 0264 0384 0c7d  .t.f...f.d.d...}
+00000070: 0000 0400 0000 0300 0000 7316 0000 0074  ..........s....t
+00000080: 0064 019c 0187 0066 0164 0264 0384 0c7d  .d.....f.d.d...}
 00000090: 017c 0153 0029 047a 7e0a 2020 2020 4368  .|.S.).z~.    Ch
 000000a0: 6563 6b20 7468 6174 2061 2073 7472 696e  eck that a strin
 000000b0: 6720 6174 7472 6962 7574 6520 6973 206e  g attribute is n
 000000c0: 6f74 2061 6e20 656d 7074 7920 7374 7269  ot an empty stri
 000000d0: 6e67 2c20 616e 6420 7265 6d6f 7665 2074  ng, and remove t
 000000e0: 6865 0a20 2020 206c 6561 6469 6e67 2061  he.    leading a
 000000f0: 6e64 2074 7261 696c 696e 6720 7768 6974  nd trailing whit
 00000100: 6573 7061 6365 2063 6861 7261 6374 6572  espace character
-00000110: 732e 0a20 2020 20da 0673 7472 696e 6763  s..    ..stringc
-00000120: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000130: 0400 0000 1300 0000 7338 0000 007c 0064  ........s8...|.d
-00000140: 0075 0072 0c74 0064 0188 009b 0064 029d  .u.r.t.d.....d..
-00000150: 0383 0182 017c 00a0 01a1 007d 017c 0173  .....|.....}.|.s
-00000160: 1a74 0064 0188 009b 0064 039d 0383 0182  .t.d.....d......
-00000170: 017c 0153 0029 044e 7a12 5374 7269 6e67  .|.S.).Nz.String
-00000180: 2061 7474 7269 6275 7465 2027 fa10 2720   attribute '..' 
-00000190: 6361 6e6e 6f74 2062 6520 4e6f 6e65 7a11  cannot be Nonez.
-000001a0: 2720 6361 6e6e 6f74 2062 6520 656d 7074  ' cannot be empt
-000001b0: 7929 02da 0a56 616c 7565 4572 726f 72da  y)...ValueError.
-000001c0: 0573 7472 6970 2902 7202 0000 00da 0173  .strip).r......s
-000001d0: a901 7201 0000 00a9 00fa 432f 686f 6d65  ..r.......C/home
+00000110: 732e 0a20 2020 2029 01da 0673 7472 696e  s..    )...strin
+00000120: 6763 0100 0000 0000 0000 0000 0000 0200  gc..............
+00000130: 0000 0400 0000 1300 0000 7338 0000 007c  ..........s8...|
+00000140: 0064 0075 0072 1874 0064 0188 009b 0064  .d.u.r.t.d.....d
+00000150: 029d 0383 0182 017c 00a0 01a1 007d 017c  .......|.....}.|
+00000160: 0173 3474 0064 0188 009b 0064 039d 0383  .s4t.d.....d....
+00000170: 0182 017c 0153 0029 044e 7a12 5374 7269  ...|.S.).Nz.Stri
+00000180: 6e67 2061 7474 7269 6275 7465 2027 fa10  ng attribute '..
+00000190: 2720 6361 6e6e 6f74 2062 6520 4e6f 6e65  ' cannot be None
+000001a0: 7a11 2720 6361 6e6e 6f74 2062 6520 656d  z.' cannot be em
+000001b0: 7074 7929 02da 0a56 616c 7565 4572 726f  pty)...ValueErro
+000001c0: 72da 0573 7472 6970 2902 7203 0000 00da  r..strip).r.....
+000001d0: 0173 7201 0000 00a9 00fa 432f 686f 6d65  .sr.......C/home
 000001e0: 2f74 6f6d 6d61 736f 2f46 7261 6374 616c  /tommaso/Fractal
 000001f0: 2f66 7261 6374 616c 2f66 7261 6374 616c  /fractal/fractal
 00000200: 2f63 6f6d 6d6f 6e2f 7363 6865 6d61 732f  /common/schemas/
 00000210: 5f76 616c 6964 6174 6f72 732e 7079 da03  _validators.py..
-00000220: 7661 6c07 0000 0073 0c00 0000 0801 1001  val....s........
-00000230: 0801 0401 1001 0401 7a13 7661 6c73 7472  ........z.valstr
+00000220: 7661 6c07 0000 0073 0c00 0000 0001 0801  val....s........
+00000230: 1001 0801 0401 1001 7a13 7661 6c73 7472  ........z.valstr
 00000240: 2e3c 6c6f 6361 6c73 3e2e 7661 6c29 01da  .<locals>.val)..
-00000250: 0373 7472 2902 7201 0000 0072 0a00 0000  .str).r....r....
-00000260: 7208 0000 0072 0700 0000 7209 0000 00da  r....r....r.....
+00000250: 0373 7472 2902 7202 0000 0072 0a00 0000  .str).r....r....
+00000260: 7208 0000 0072 0100 0000 7209 0000 00da  r....r....r.....
 00000270: 0676 616c 7374 7201 0000 0073 0400 0000  .valstr....s....
-00000280: 1206 0408 720c 0000 00e9 0100 0000 da07  ....r...........
-00000290: 6d69 6e5f 7661 6c63 0200 0000 0000 0000  min_valc........
-000002a0: 0000 0000 0300 0000 0400 0000 0300 0000  ................
-000002b0: 7318 0000 0064 0174 0066 0287 0087 0166  s....d.t.f.....f
-000002c0: 0264 0264 0384 0c7d 027c 0253 0029 047a  .d.d...}.|.S.).z
-000002d0: 840a 2020 2020 4368 6563 6b20 7468 6174  ..    Check that
-000002e0: 2061 6e20 696e 7465 6765 7220 6174 7472   an integer attr
-000002f0: 6962 7574 6520 2865 2e67 2e20 6966 2069  ibute (e.g. if i
-00000300: 7420 6973 206d 6561 6e74 2074 6f20 6265  t is meant to be
-00000310: 2074 6865 2049 4420 6f66 2061 0a20 2020   the ID of a.   
-00000320: 2064 6174 6162 6173 6520 656e 7472 7929   database entry)
-00000330: 2069 7320 6772 6561 7465 7220 6f72 2065   is greater or e
-00000340: 7175 616c 2074 6f20 6d69 6e5f 7661 6c2e  qual to min_val.
-00000350: 0a20 2020 20da 0769 6e74 6567 6572 6301  .    ..integerc.
-00000360: 0000 0000 0000 0000 0000 0001 0000 0008  ................
-00000370: 0000 0013 0000 0073 4000 0000 7c00 6400  .......s@...|.d.
-00000380: 7500 720c 7400 6401 8800 9b00 6402 9d03  u.r.t.d.....d...
-00000390: 8301 8201 7c00 8801 6b00 721e 7400 6401  ....|...k.r.t.d.
-000003a0: 8800 9b00 6403 8801 9b00 6404 7c00 9b00  ....d.....d.|...
-000003b0: 6405 9d07 8301 8201 7c00 5300 2906 4e7a  d.......|.S.).Nz
-000003c0: 1349 6e74 6567 6572 2061 7474 7269 6275  .Integer attribu
-000003d0: 7465 2027 7203 0000 007a 1627 2063 616e  te 'r....z.' can
-000003e0: 6e6f 7420 6265 206c 6573 7320 7468 616e  not be less than
-000003f0: 207a 0820 2867 6976 656e 20fa 0129 2901   z. (given ..)).
-00000400: 7204 0000 0029 0172 0f00 0000 a902 7201  r....).r......r.
+00000280: 0006 1208 720c 0000 00e9 0100 0000 a902  ....r...........
+00000290: 7202 0000 00da 076d 696e 5f76 616c 6302  r......min_valc.
+000002a0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+000002b0: 0000 0003 0000 0073 1800 0000 7400 6401  .......s....t.d.
+000002c0: 9c01 8700 8701 6602 6402 6403 840c 7d02  ......f.d.d...}.
+000002d0: 7c02 5300 2904 7a84 0a20 2020 2043 6865  |.S.).z..    Che
+000002e0: 636b 2074 6861 7420 616e 2069 6e74 6567  ck that an integ
+000002f0: 6572 2061 7474 7269 6275 7465 2028 652e  er attribute (e.
+00000300: 672e 2069 6620 6974 2069 7320 6d65 616e  g. if it is mean
+00000310: 7420 746f 2062 6520 7468 6520 4944 206f  t to be the ID o
+00000320: 6620 610a 2020 2020 6461 7461 6261 7365  f a.    database
+00000330: 2065 6e74 7279 2920 6973 2067 7265 6174   entry) is great
+00000340: 6572 206f 7220 6571 7561 6c20 746f 206d  er or equal to m
+00000350: 696e 5f76 616c 2e0a 2020 2020 a901 da07  in_val..    ....
+00000360: 696e 7465 6765 7263 0100 0000 0000 0000  integerc........
+00000370: 0000 0000 0100 0000 0800 0000 1300 0000  ................
+00000380: 7340 0000 007c 0064 0075 0072 1874 0064  s@...|.d.u.r.t.d
+00000390: 0188 009b 0064 029d 0383 0182 017c 0088  .....d.......|..
+000003a0: 016b 0072 3c74 0064 0188 009b 0064 0388  .k.r<t.d.....d..
+000003b0: 019b 0064 047c 009b 0064 059d 0783 0182  ...d.|...d......
+000003c0: 017c 0053 0029 064e 7a13 496e 7465 6765  .|.S.).Nz.Intege
+000003d0: 7220 6174 7472 6962 7574 6520 2772 0400  r attribute 'r..
+000003e0: 0000 7a16 2720 6361 6e6e 6f74 2062 6520  ..z.' cannot be 
+000003f0: 6c65 7373 2074 6861 6e20 7a08 2028 6769  less than z. (gi
+00000400: 7665 6e20 fa01 2929 0172 0500 0000 7210  ven ..)).r....r.
 00000410: 0000 0072 0e00 0000 7208 0000 0072 0900  ...r....r....r..
 00000420: 0000 720a 0000 0018 0000 0073 1600 0000  ..r........s....
-00000430: 0801 1001 0801 0201 0801 0201 04ff 0201  ................
-00000440: 06ff 04ff 0404 7a13 7661 6c69 6e74 2e3c  ......z.valint.<
+00000430: 0001 0801 1001 0801 0201 0801 02ff 0401  ................
+00000440: 02ff 06ff 0404 7a13 7661 6c69 6e74 2e3c  ......z.valint.<
 00000450: 6c6f 6361 6c73 3e2e 7661 6c29 01da 0369  locals>.val)...i
-00000460: 6e74 2903 7201 0000 0072 0e00 0000 720a  nt).r....r....r.
-00000470: 0000 0072 0800 0000 7211 0000 0072 0900  ...r....r....r..
+00000460: 6e74 2903 7202 0000 0072 0f00 0000 720a  nt).r....r....r.
+00000470: 0000 0072 0800 0000 720e 0000 0072 0900  ...r....r....r..
 00000480: 0000 da06 7661 6c69 6e74 1200 0000 7304  ....valint....s.
-00000490: 0000 0014 0604 0a72 1300 0000 4e29 0172  .......r....N).r
+00000490: 0000 0000 0614 0a72 1400 0000 4e29 0172  .......r....N).r
 000004a0: 0d00 0000 2904 720b 0000 0072 0c00 0000  ....).r....r....
-000004b0: 7212 0000 0072 1300 0000 7208 0000 0072  r....r....r....r
+000004b0: 7213 0000 0072 1400 0000 7208 0000 0072  r....r....r....r
 000004c0: 0800 0000 7208 0000 0072 0900 0000 da08  ....r....r......
-000004d0: 3c6d 6f64 756c 653e 0100 0000 7304 0000  <module>....s...
-000004e0: 000e 0018 11                             .....
+000004d0: 3c6d 6f64 756c 653e 0100 0000 7302 0000  <module>....s...
+000004e0: 000e 11                                  ...
```

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 13:52:21 2023 UTC, .py size: 1716 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 15f0 0564 b406 0000  o..........d....
+00000000: 610d 0d0a 0000 0000 15f0 0564 b406 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c01 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c06 6d07 5a07 0100 6406 6407 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6406 6408 6c08 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -55,74 +55,73 @@
 00000360: 5f5f 7204 0000 0072 1100 0000 da04 626f  __r....r......bo
 00000370: 6f6c da03 7374 72a9 0072 1b00 0000 721b  ol..str..r....r.
 00000380: 0000 00fa 452f 686f 6d65 2f74 6f6d 6d61  ....E/home/tomma
 00000390: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
 000003a0: 616c 2f66 7261 6374 616c 2f63 6f6d 6d6f  al/fractal/commo
 000003b0: 6e2f 7363 6865 6d61 732f 6170 706c 7977  n/schemas/applyw
 000003c0: 6f72 6b66 6c6f 772e 7079 720a 0000 0012  orkflow.pyr.....
-000003d0: 0000 0073 1000 0000 0a00 0401 080d 0801  ...s............
-000003e0: 0c01 0801 0c01 1001 720a 0000 0063 0000  ........r....c..
-000003f0: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000400: 0000 4000 0000 7370 0000 0065 005a 0164  ..@...sp...e.Z.d
-00000410: 005a 0265 0364 0164 0264 038d 0265 0464  .Z.e.d.d.d...e.d
-00000420: 0183 0183 015a 0565 0364 0464 0264 038d  .....Z.e.d.d.d..
-00000430: 0265 0464 0483 0183 015a 0665 0364 0564  .e.d.....Z.e.d.d
-00000440: 0264 038d 0265 0464 0583 0183 015a 0765  .d...e.d.....Z.e
-00000450: 0364 0664 0264 038d 0265 0464 0683 0183  .d.d.d...e.d....
-00000460: 015a 0865 0364 0764 0264 038d 0265 0964  .Z.e.d.d.d...e.d
-00000470: 0783 0183 015a 0a64 0853 0029 0972 0b00  .....Z.d.S.).r..
-00000480: 0000 720d 0000 0054 2901 da0b 616c 6c6f  ..r....T)...allo
-00000490: 775f 7265 7573 6572 0e00 0000 720f 0000  w_reuser....r...
-000004a0: 0072 1000 0000 7212 0000 004e 290b 7213  .r....r....N).r.
-000004b0: 0000 0072 1400 0000 7215 0000 0072 0500  ...r....r....r..
-000004c0: 0000 7208 0000 00da 0b5f 7072 6f6a 6563  ..r......_projec
-000004d0: 745f 6964 da11 5f69 6e70 7574 5f64 6174  t_id.._input_dat
-000004e0: 6173 6574 5f69 64da 125f 6f75 7470 7574  aset_id.._output
-000004f0: 5f64 6174 6173 6574 5f69 64da 0c5f 776f  _dataset_id.._wo
-00000500: 726b 666c 6f77 5f69 6472 0900 0000 da0c  rkflow_idr......
-00000510: 5f77 6f72 6b65 725f 696e 6974 721b 0000  _worker_initr...
-00000520: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000530: 720b 0000 0028 0000 0073 2000 0000 0800  r....(...s .....
-00000540: 0a03 0601 04ff 0a03 0601 04ff 0a03 0601  ................
-00000550: 04ff 0a03 0601 04ff 0a03 0601 08ff 720b  ..............r.
-00000560: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000570: 0000 0000 0300 0000 4000 0000 7362 0000  ........@...sb..
-00000580: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
-00000590: 013c 0065 0565 0464 023c 0065 0665 0464  .<.e.e.d.<.e.e.d
-000005a0: 033c 0065 0765 0619 0065 0464 043c 0065  .<.e.e...e.d.<.e
-000005b0: 0765 0865 0619 0019 0065 0464 053c 0065  .e.e.....e.d.<.e
-000005c0: 0765 0619 0065 0464 063c 0065 0765 0619  .e...e.d.<.e.e..
-000005d0: 0065 0464 073c 0064 0864 0984 005a 0964  .e.d.<.d.d...Z.d
-000005e0: 0a53 0029 0b72 0c00 0000 da02 6964 da0f  .S.).r......id..
-000005f0: 7374 6172 745f 7469 6d65 7374 616d 70da  start_timestamp.
-00000600: 0673 7461 7475 73da 036c 6f67 da07 6869  .status..log..hi
-00000610: 7374 6f72 79da 0b77 6f72 6b69 6e67 5f64  story..working_d
-00000620: 6972 da10 776f 726b 696e 675f 6469 725f  ir..working_dir_
-00000630: 7573 6572 6301 0000 0000 0000 0000 0000  userc...........
-00000640: 0002 0000 0003 0000 0043 0000 0073 1a00  .........C...s..
-00000650: 0000 7c00 a000 a100 7d01 7401 7c00 6a02  ..|.....}.t.|.j.
-00000660: 8301 7c01 6401 3c00 7c01 5300 2902 4e72  ..|.d.<.|.S.).Nr
-00000670: 2400 0000 2903 da04 6469 6374 721a 0000  $...)...dictr...
-00000680: 0072 2400 0000 2902 da04 7365 6c66 da01  .r$...)...self..
-00000690: 6472 1b00 0000 721b 0000 0072 1c00 0000  dr....r....r....
-000006a0: da0e 7361 6e69 7469 7365 645f 6469 6374  ..sanitised_dict
-000006b0: 4500 0000 7306 0000 0008 010e 0104 017a  E...s..........z
-000006c0: 2041 7070 6c79 576f 726b 666c 6f77 5265   ApplyWorkflowRe
-000006d0: 6164 2e73 616e 6974 6973 6564 5f64 6963  ad.sanitised_dic
-000006e0: 744e 290a 7213 0000 0072 1400 0000 7215  tN).r....r....r.
-000006f0: 0000 0072 1700 0000 7218 0000 0072 0200  ...r....r....r..
-00000700: 0000 721a 0000 0072 0400 0000 7203 0000  ..r....r....r...
-00000710: 0072 2d00 0000 721b 0000 0072 1b00 0000  .r-...r....r....
-00000720: 721b 0000 0072 1c00 0000 720c 0000 003c  r....r....r....<
-00000730: 0000 0073 1200 0000 0a00 0801 0801 0801  ...s............
-00000740: 0c01 1001 0c01 0c01 0c02 720c 0000 004e  ..........r....N
-00000750: 290f 7202 0000 00da 0674 7970 696e 6772  ).r......typingr
-00000760: 0300 0000 7204 0000 00da 0870 7964 616e  ....r......pydan
-00000770: 7469 6372 0500 0000 da08 7371 6c6d 6f64  ticr......sqlmod
-00000780: 656c 7206 0000 00da 0b5f 7661 6c69 6461  elr......_valida
-00000790: 746f 7273 7208 0000 0072 0900 0000 da07  torsr....r......
-000007a0: 5f5f 616c 6c5f 5f72 0a00 0000 720b 0000  __all__r....r...
-000007b0: 0072 0c00 0000 721b 0000 0072 1b00 0000  .r....r....r....
-000007c0: 721b 0000 0072 1c00 0000 da08 3c6d 6f64  r....r......<mod
-000007d0: 756c 653e 0100 0000 7316 0000 000c 000c  ule>....s.......
-000007e0: 010c 010c 020c 010c 020c 0104 0210 0710  ................
-000007f0: 1614 14                                  ...
+000003d0: 0000 0073 0e00 0000 0a01 040d 0801 0801  ...s............
+000003e0: 0c01 0801 0c01 720a 0000 0063 0000 0000  ......r....c....
+000003f0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000400: 4000 0000 7370 0000 0065 005a 0164 005a  @...sp...e.Z.d.Z
+00000410: 0265 0364 0164 0264 038d 0265 0464 0183  .e.d.d.d...e.d..
+00000420: 0183 015a 0565 0364 0464 0264 038d 0265  ...Z.e.d.d.d...e
+00000430: 0464 0483 0183 015a 0665 0364 0564 0264  .d.....Z.e.d.d.d
+00000440: 038d 0265 0464 0583 0183 015a 0765 0364  ...e.d.....Z.e.d
+00000450: 0664 0264 038d 0265 0464 0683 0183 015a  .d.d...e.d.....Z
+00000460: 0865 0364 0764 0264 038d 0265 0964 0783  .e.d.d.d...e.d..
+00000470: 0183 015a 0a64 0853 0029 0972 0b00 0000  ...Z.d.S.).r....
+00000480: 720d 0000 0054 2901 da0b 616c 6c6f 775f  r....T)...allow_
+00000490: 7265 7573 6572 0e00 0000 720f 0000 0072  reuser....r....r
+000004a0: 1000 0000 7212 0000 004e 290b 7213 0000  ....r....N).r...
+000004b0: 0072 1400 0000 7215 0000 0072 0500 0000  .r....r....r....
+000004c0: 7208 0000 005a 0b5f 7072 6f6a 6563 745f  r....Z._project_
+000004d0: 6964 5a11 5f69 6e70 7574 5f64 6174 6173  idZ._input_datas
+000004e0: 6574 5f69 645a 125f 6f75 7470 7574 5f64  et_idZ._output_d
+000004f0: 6174 6173 6574 5f69 645a 0c5f 776f 726b  ataset_idZ._work
+00000500: 666c 6f77 5f69 6472 0900 0000 5a0c 5f77  flow_idr....Z._w
+00000510: 6f72 6b65 725f 696e 6974 721b 0000 0072  orker_initr....r
+00000520: 1b00 0000 721b 0000 0072 1c00 0000 720b  ....r....r....r.
+00000530: 0000 0028 0000 0073 1e00 0000 0803 0a01  ...(...s........
+00000540: 06ff 0403 0a01 06ff 0403 0a01 06ff 0403  ................
+00000550: 0a01 06ff 0403 0a01 06ff 720b 0000 0063  ..........r....c
+00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000570: 0300 0000 4000 0000 7362 0000 0065 005a  ....@...sb...e.Z
+00000580: 0164 005a 0255 0065 0365 0464 013c 0065  .d.Z.U.e.e.d.<.e
+00000590: 0565 0464 023c 0065 0665 0464 033c 0065  .e.d.<.e.e.d.<.e
+000005a0: 0765 0619 0065 0464 043c 0065 0765 0865  .e...e.d.<.e.e.e
+000005b0: 0619 0019 0065 0464 053c 0065 0765 0619  .....e.d.<.e.e..
+000005c0: 0065 0464 063c 0065 0765 0619 0065 0464  .e.d.<.e.e...e.d
+000005d0: 073c 0064 0864 0984 005a 0964 0a53 0029  .<.d.d...Z.d.S.)
+000005e0: 0b72 0c00 0000 da02 6964 da0f 7374 6172  .r......id..star
+000005f0: 745f 7469 6d65 7374 616d 70da 0673 7461  t_timestamp..sta
+00000600: 7475 73da 036c 6f67 da07 6869 7374 6f72  tus..log..histor
+00000610: 795a 0b77 6f72 6b69 6e67 5f64 6972 5a10  yZ.working_dirZ.
+00000620: 776f 726b 696e 675f 6469 725f 7573 6572  working_dir_user
+00000630: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000640: 0003 0000 0043 0000 0073 1a00 0000 7c00  .....C...s....|.
+00000650: a000 a100 7d01 7401 7c00 6a02 8301 7c01  ....}.t.|.j...|.
+00000660: 6401 3c00 7c01 5300 2902 4e72 1f00 0000  d.<.|.S.).Nr....
+00000670: 2903 da04 6469 6374 721a 0000 0072 1f00  )...dictr....r..
+00000680: 0000 2902 da04 7365 6c66 da01 6472 1b00  ..)...self..dr..
+00000690: 0000 721b 0000 0072 1c00 0000 da0e 7361  ..r....r......sa
+000006a0: 6e69 7469 7365 645f 6469 6374 4500 0000  nitised_dictE...
+000006b0: 7306 0000 0000 0108 010e 017a 2041 7070  s..........z App
+000006c0: 6c79 576f 726b 666c 6f77 5265 6164 2e73  lyWorkflowRead.s
+000006d0: 616e 6974 6973 6564 5f64 6963 744e 290a  anitised_dictN).
+000006e0: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+000006f0: 1700 0000 7218 0000 0072 0200 0000 721a  ....r....r....r.
+00000700: 0000 0072 0400 0000 7203 0000 0072 2600  ...r....r....r&.
+00000710: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00000720: 0072 1c00 0000 720c 0000 003c 0000 0073  .r....r....<...s
+00000730: 1000 0000 0a01 0801 0801 0801 0c01 1001  ................
+00000740: 0c01 0c02 720c 0000 004e 290f 7202 0000  ....r....N).r...
+00000750: 00da 0674 7970 696e 6772 0300 0000 7204  ...typingr....r.
+00000760: 0000 00da 0870 7964 616e 7469 6372 0500  .....pydanticr..
+00000770: 0000 5a08 7371 6c6d 6f64 656c 7206 0000  ..Z.sqlmodelr...
+00000780: 005a 0b5f 7661 6c69 6461 746f 7273 7208  .Z._validatorsr.
+00000790: 0000 0072 0900 0000 da07 5f5f 616c 6c5f  ...r......__all_
+000007a0: 5f72 0a00 0000 720b 0000 0072 0c00 0000  _r....r....r....
+000007b0: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+000007c0: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000007d0: 0000 7314 0000 000c 010c 010c 020c 010c  ..s.............
+000007e0: 020c 010c 0204 0710 1610 14              ...........
```

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/project.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 15 12:00:37 2023 UTC, .py size: 2737 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 65b3 1164 b10a 0000  o.......e..d....
+00000000: 610d 0d0a 0000 0000 65b3 1164 b10a 0000  a.......e..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d06 5a06 0100 6400 6406 6c05  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
@@ -46,187 +46,187 @@
 000002d0: da07 5f5f 646f 635f 5fda 0373 7472 da0f  ..__doc__..str..
 000002e0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fa9  __annotations__.
 000002f0: 0072 1c00 0000 721c 0000 00fa 3f2f 686f  .r....r.....?/ho
 00000300: 6d65 2f74 6f6d 6d61 736f 2f46 7261 6374  me/tommaso/Fract
 00000310: 616c 2f66 7261 6374 616c 2f66 7261 6374  al/fractal/fract
 00000320: 616c 2f63 6f6d 6d6f 6e2f 7363 6865 6d61  al/common/schema
 00000330: 732f 7072 6f6a 6563 742e 7079 7214 0000  s/project.pyr...
-00000340: 001d 0000 0073 0600 0000 0a00 0401 0c04  .....s..........
-00000350: 7214 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000360: 0000 0000 0000 0400 0000 4000 0000 f320  ..........@.... 
-00000370: 0000 0065 005a 0164 005a 0265 0364 0164  ...e.Z.d.Z.e.d.d
-00000380: 0264 038d 0265 0464 0183 0183 015a 0564  .d...e.d.....Z.d
-00000390: 0453 0029 0572 1100 0000 7215 0000 0054  .S.).r....r....T
-000003a0: a901 da0b 616c 6c6f 775f 7265 7573 654e  ....allow_reuseN
-000003b0: a906 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-000003c0: 0072 0700 0000 720a 0000 00da 055f 7061  .r....r......_pa
-000003d0: 7468 721c 0000 0072 1c00 0000 721c 0000  thr....r....r...
-000003e0: 0072 1d00 0000 7211 0000 0025 0000 00f3  .r....r....%....
-000003f0: 0400 0000 0800 1802 7211 0000 0063 0000  ........r....c..
-00000400: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000410: 0000 4000 0000 721e 0000 0029 0572 1300  ..@...r....).r..
-00000420: 0000 7215 0000 0054 721f 0000 004e 7221  ..r....Tr....Nr!
-00000430: 0000 0072 1c00 0000 721c 0000 0072 1c00  ...r....r....r..
-00000440: 0000 721d 0000 0072 1300 0000 2a00 0000  ..r....r....*...
-00000450: 7223 0000 0072 1300 0000 6300 0000 0000  r#...r....c.....
-00000460: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000470: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000480: 5500 6503 6504 6401 3c00 6503 6504 6402  U.e.e.d.<.e.e.d.
-00000490: 3c00 6403 5300 2904 7212 0000 00da 0269  <.d.S.).r......i
-000004a0: 64da 0a64 6174 6173 6574 5f69 644e 2905  d..dataset_idN).
-000004b0: 7216 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
-000004c0: 0369 6e74 721b 0000 0072 1c00 0000 721c  .intr....r....r.
-000004d0: 0000 0072 1c00 0000 721d 0000 0072 1200  ...r....r....r..
-000004e0: 0000 2f00 0000 7306 0000 000a 0008 010c  ../...s.........
-000004f0: 0172 1200 0000 6300 0000 0000 0000 0000  .r....c.........
-00000500: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-00000510: 4c00 0000 6500 5a01 6400 5a02 5500 6401  L...e.Z.d.Z.U.d.
-00000520: 5a03 6504 6505 6402 3c00 6506 6504 1900  Z.e.e.d.<.e.e...
-00000530: 6505 6403 3c00 6507 6900 6404 8d01 5a08  e.d.<.e.i.d...Z.
-00000540: 6509 6504 650a 6602 1900 6505 6405 3c00  e.e.e.f...e.d.<.
-00000550: 6406 5a0b 650c 6505 6407 3c00 6408 5300  d.Z.e.e.d.<.d.S.
-00000560: 2909 da0c 5f44 6174 6173 6574 4261 7365  )..._DatasetBase
-00000570: 7a7e 0a20 2020 2042 6173 6520 636c 6173  z~.    Base clas
-00000580: 7320 666f 7220 4461 7461 7365 740a 0a20  s for Dataset.. 
-00000590: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
-000005a0: 2020 2020 2020 206e 616d 653a 2054 4244         name: TBD
-000005b0: 0a20 2020 2020 2020 2074 7970 653a 2054  .        type: T
-000005c0: 4244 0a20 2020 2020 2020 206d 6574 613a  BD.        meta:
-000005d0: 2054 4244 0a20 2020 2020 2020 2072 6561   TBD.        rea
-000005e0: 645f 6f6e 6c79 3a20 5442 440a 2020 2020  d_only: TBD.    
-000005f0: da04 6e61 6d65 da04 7479 7065 2901 da07  ..name..type)...
-00000600: 6465 6661 756c 74da 046d 6574 6146 da09  default..metaF..
-00000610: 7265 6164 5f6f 6e6c 794e 290d 7216 0000  read_onlyN).r...
-00000620: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000630: 721a 0000 0072 1b00 0000 7205 0000 0072  r....r....r....r
-00000640: 0600 0000 722b 0000 0072 0300 0000 7202  ....r+...r....r.
-00000650: 0000 0072 2c00 0000 da04 626f 6f6c 721c  ...r,.....boolr.
-00000660: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000670: 0000 7227 0000 0037 0000 0073 0c00 0000  ..r'...7...s....
-00000680: 0a00 0401 080a 0c01 1a01 1001 7227 0000  ............r'..
-00000690: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000006a0: 0000 0400 0000 4000 0000 7366 0000 0065  ......@...sf...e
-000006b0: 005a 0164 005a 0255 0065 0365 0419 0065  .Z.d.Z.U.e.e...e
-000006c0: 0564 013c 0064 025a 0665 0365 0765 0465  .d.<.d.Z.e.e.e.e
-000006d0: 0866 0219 0019 0065 0564 033c 0065 0365  .f.....e.d.<.e.e
-000006e0: 0919 0065 0564 043c 0065 0a64 0164 0564  ...e.d.<.e.d.d.d
-000006f0: 068d 0265 0b64 0183 0183 015a 0c65 0a64  ...e.d.....Z.e.d
-00000700: 0764 0564 068d 0265 0b64 0783 0183 015a  .d.d...e.d.....Z
-00000710: 0d64 0253 0029 0872 0e00 0000 7228 0000  .d.S.).r....r(..
-00000720: 004e 722b 0000 0072 2c00 0000 5472 1f00  .Nr+...r,...Tr..
-00000730: 0000 7229 0000 0029 0e72 1600 0000 7217  ..r)...).r....r.
-00000740: 0000 0072 1800 0000 7205 0000 0072 1a00  ...r....r....r..
-00000750: 0000 721b 0000 0072 2b00 0000 7203 0000  ..r....r+...r...
-00000760: 0072 0200 0000 722d 0000 0072 0700 0000  .r....r-...r....
-00000770: 720a 0000 00da 055f 6e61 6d65 da05 5f74  r......_name.._t
-00000780: 7970 6572 1c00 0000 721c 0000 0072 1c00  yper....r....r..
-00000790: 0000 721d 0000 0072 0e00 0000 4800 0000  ..r....r....H...
-000007a0: 730c 0000 000a 000c 0118 010c 0114 0318  s...............
-000007b0: 0172 0e00 0000 6300 0000 0000 0000 0000  .r....c.........
-000007c0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-000007d0: 3400 0000 6500 5a01 6400 5a02 6503 6401  4...e.Z.d.Z.e.d.
-000007e0: 6402 6403 8d02 6504 6401 8301 8301 5a05  d.d...e.d.....Z.
-000007f0: 6503 6404 6402 6403 8d02 6504 6404 8301  e.d.d.d...e.d...
-00000800: 8301 5a06 6405 5300 2906 720f 0000 0072  ..Z.d.S.).r....r
-00000810: 2800 0000 5472 1f00 0000 7229 0000 004e  (...Tr....r)...N
-00000820: 2907 7216 0000 0072 1700 0000 7218 0000  ).r....r....r...
-00000830: 0072 0700 0000 720a 0000 0072 2e00 0000  .r....r....r....
-00000840: 722f 0000 0072 1c00 0000 721c 0000 0072  r/...r....r....r
-00000850: 1c00 0000 721d 0000 0072 0f00 0000 5200  ....r....r....R.
-00000860: 0000 7306 0000 0008 0014 0218 0172 0f00  ..s..........r..
-00000870: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000880: 0000 0003 0000 0040 0000 0073 3200 0000  .......@...s2...
-00000890: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
-000008a0: 3c00 6505 6506 1900 6504 6402 3c00 6503  <.e.e...e.d.<.e.
-000008b0: 6504 6403 3c00 6507 6504 6404 3c00 6405  e.d.<.e.e.d.<.d.
-000008c0: 5300 2906 7210 0000 0072 2400 0000 da0d  S.).r....r$.....
-000008d0: 7265 736f 7572 6365 5f6c 6973 74da 0a70  resource_list..p
-000008e0: 726f 6a65 6374 5f69 6472 2c00 0000 4e29  roject_idr,...N)
-000008f0: 0872 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000900: 7226 0000 0072 1b00 0000 7204 0000 0072  r&...r....r....r
-00000910: 1200 0000 722d 0000 0072 1c00 0000 721c  ....r-...r....r.
-00000920: 0000 0072 1c00 0000 721d 0000 0072 1000  ...r....r....r..
-00000930: 0000 5800 0000 730a 0000 000a 0008 010c  ..X...s.........
-00000940: 0108 010c 0172 1000 0000 6300 0000 0000  .....r....c.....
-00000950: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000960: 0000 0073 2e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000970: 5500 6401 5a03 6504 6505 6402 3c00 6504  U.d.Z.e.e.d.<.e.
-00000980: 6505 6403 3c00 6404 5a06 6507 6505 6405  e.d.<.d.Z.e.e.d.
-00000990: 3c00 6406 5300 2907 da0c 5f50 726f 6a65  <.d.S.)..._Proje
-000009a0: 6374 4261 7365 7a73 0a20 2020 2042 6173  ctBasezs.    Bas
-000009b0: 6520 636c 6173 7320 666f 7220 5072 6f6a  e class for Proj
-000009c0: 6563 740a 0a20 2020 2041 7474 7269 6275  ect..    Attribu
-000009d0: 7465 733a 0a20 2020 2020 2020 206e 616d  tes:.        nam
-000009e0: 653a 2054 4244 0a20 2020 2020 2020 2070  e: TBD.        p
-000009f0: 726f 6a65 6374 5f64 6972 3a20 5442 440a  roject_dir: TBD.
-00000a00: 2020 2020 2020 2020 7265 6164 5f6f 6e6c          read_onl
-00000a10: 793a 2054 4244 0a20 2020 2072 2800 0000  y: TBD.    r(...
-00000a20: da0b 7072 6f6a 6563 745f 6469 7246 722c  ..project_dirFr,
-00000a30: 0000 004e 2908 7216 0000 0072 1700 0000  ...N).r....r....
-00000a40: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000a50: 1b00 0000 722c 0000 0072 2d00 0000 721c  ....r,...r-...r.
-00000a60: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000a70: 0000 7232 0000 0062 0000 0073 0a00 0000  ..r2...b...s....
-00000a80: 0a00 0401 0809 0801 1001 7232 0000 0063  ..........r2...c
-00000a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000aa0: 0400 0000 4000 0000 735a 0000 0065 005a  ....@...sZ...e.Z
-00000ab0: 0164 005a 0255 0064 015a 0365 0465 0519  .d.Z.U.d.Z.e.e..
-00000ac0: 0065 0664 023c 0065 0764 0364 0464 058d  .e.d.<.e.d.d.d..
-00000ad0: 0265 0864 0383 0183 015a 0965 0764 0664  .e.d.....Z.e.d.d
-00000ae0: 0464 058d 0265 0864 0683 0183 015a 0a65  .d...e.d.....Z.e
-00000af0: 0764 0264 0464 058d 0265 0864 0283 0183  .d.d.d...e.d....
-00000b00: 015a 0b64 0753 0029 0872 0b00 0000 722a  .Z.d.S.).r....r*
-00000b10: 0000 00da 1464 6566 6175 6c74 5f64 6174  .....default_dat
-00000b20: 6173 6574 5f6e 616d 6572 2800 0000 5472  aset_namer(...Tr
-00000b30: 1f00 0000 7233 0000 004e 290c 7216 0000  ....r3...N).r...
-00000b40: 0072 1700 0000 7218 0000 0072 3400 0000  .r....r....r4...
-00000b50: 7205 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00000b60: 0700 0000 720a 0000 0072 2e00 0000 da0c  ....r....r......
-00000b70: 5f70 726f 6a65 6374 5f64 6972 da15 5f64  _project_dir.._d
-00000b80: 6566 6175 6c74 5f64 6174 6173 6574 5f6e  efault_dataset_n
-00000b90: 616d 6572 1c00 0000 721c 0000 0072 1c00  amer....r....r..
-00000ba0: 0000 721d 0000 0072 0b00 0000 7100 0000  ..r....r....q...
-00000bb0: 7316 0000 000a 0010 0114 030a 0106 0104  s...............
-00000bc0: ff02 0304 0104 ff06 0208 fe72 0b00 0000  ...........r....
-00000bd0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000be0: 0003 0000 0040 0000 0073 2600 0000 6500  .....@...s&...e.
-00000bf0: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
-00000c00: 6700 5a05 6506 6507 1900 6504 6402 3c00  g.Z.e.e...e.d.<.
-00000c10: 6403 5300 2904 720c 0000 0072 2400 0000  d.S.).r....r$...
-00000c20: da0c 6461 7461 7365 745f 6c69 7374 4e29  ..dataset_listN)
-00000c30: 0872 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000c40: 7226 0000 0072 1b00 0000 7237 0000 0072  r&...r....r7...r
-00000c50: 0400 0000 7210 0000 0072 1c00 0000 721c  ....r....r....r.
-00000c60: 0000 0072 1c00 0000 721d 0000 0072 0c00  ...r....r....r..
-00000c70: 0000 7e00 0000 7306 0000 000a 0008 0114  ..~...s.........
-00000c80: 0172 0c00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000c90: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-00000ca0: 5a00 0000 6500 5a01 6400 5a02 5500 6503  Z...e.Z.d.Z.U.e.
-00000cb0: 6504 1900 6505 6401 3c00 6503 6504 1900  e...e.d.<.e.e...
-00000cc0: 6505 6402 3c00 6503 6506 1900 6505 6403  e.d.<.e.e...e.d.
-00000cd0: 3c00 6507 6401 6404 6405 8d02 6508 6401  <.e.d.d.d...e.d.
-00000ce0: 8301 8301 5a09 6507 6402 6404 6405 8d02  ....Z.e.d.d.d...
-00000cf0: 6508 6402 8301 8301 5a0a 6406 5300 2907  e.d.....Z.d.S.).
-00000d00: 720d 0000 0072 2800 0000 7233 0000 0072  r....r(...r3...r
-00000d10: 2c00 0000 5472 1f00 0000 4e29 0b72 1600  ,...Tr....N).r..
-00000d20: 0000 7217 0000 0072 1800 0000 7205 0000  ..r....r....r...
-00000d30: 0072 1a00 0000 721b 0000 0072 2d00 0000  .r....r....r-...
-00000d40: 7207 0000 0072 0a00 0000 722e 0000 0072  r....r....r....r
-00000d50: 3500 0000 721c 0000 0072 1c00 0000 721c  5...r....r....r.
-00000d60: 0000 0072 1d00 0000 720d 0000 0083 0000  ...r....r.......
-00000d70: 0073 1000 0000 0a00 0c01 0c01 0c01 1403  .s..............
-00000d80: 0a01 0601 08ff 720d 0000 004e 2919 da06  ......r....N)...
-00000d90: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00000da0: 7204 0000 0072 0500 0000 da08 7079 6461  r....r......pyda
-00000db0: 6e74 6963 7206 0000 0072 0700 0000 da08  nticr....r......
-00000dc0: 7371 6c6d 6f64 656c 7208 0000 00da 0b5f  sqlmodelr......_
-00000dd0: 7661 6c69 6461 746f 7273 720a 0000 00da  validatorsr.....
-00000de0: 075f 5f61 6c6c 5f5f 7214 0000 0072 1100  .__all__r....r..
-00000df0: 0000 7213 0000 0072 1200 0000 7227 0000  ..r....r....r'..
-00000e00: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00000e10: 7232 0000 0072 0b00 0000 720c 0000 0072  r2...r....r....r
-00000e20: 0d00 0000 721c 0000 0072 1c00 0000 721c  ....r....r....r.
-00000e30: 0000 0072 1d00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000e40: 653e 0100 0000 732a 0000 000c 000c 010c  e>....s*........
-00000e50: 010c 010c 020c 010c 010c 0204 0310 1010  ................
-00000e60: 0810 0510 0510 0810 1110 0a10 0610 0a10  ................
-00000e70: 0f10 0d14 05                             .....
+00000340: 001d 0000 0073 0400 0000 0a01 0404 7214  .....s........r.
+00000350: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000360: 0000 0000 0400 0000 4000 0000 7320 0000  ........@...s ..
+00000370: 0065 005a 0164 005a 0265 0364 0164 0264  .e.Z.d.Z.e.d.d.d
+00000380: 038d 0265 0464 0183 0183 015a 0564 0453  ...e.d.....Z.d.S
+00000390: 0029 0572 1100 0000 7215 0000 0054 a901  .).r....r....T..
+000003a0: da0b 616c 6c6f 775f 7265 7573 654e a906  ..allow_reuseN..
+000003b0: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+000003c0: 0700 0000 720a 0000 00da 055f 7061 7468  ....r......_path
+000003d0: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
+000003e0: 1d00 0000 7211 0000 0025 0000 0073 0200  ....r....%...s..
+000003f0: 0000 0802 7211 0000 0063 0000 0000 0000  ....r....c......
+00000400: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000410: 0000 7320 0000 0065 005a 0164 005a 0265  ..s ...e.Z.d.Z.e
+00000420: 0364 0164 0264 038d 0265 0464 0183 0183  .d.d.d...e.d....
+00000430: 015a 0564 0453 0029 0572 1300 0000 7215  .Z.d.S.).r....r.
+00000440: 0000 0054 721e 0000 004e 7220 0000 0072  ...Tr....Nr ...r
+00000450: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
+00000460: 0000 0072 1300 0000 2a00 0000 7302 0000  ...r....*...s...
+00000470: 0008 0272 1300 0000 6300 0000 0000 0000  ...r....c.......
+00000480: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000490: 0073 1e00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+000004a0: 6503 6504 6401 3c00 6503 6504 6402 3c00  e.e.d.<.e.e.d.<.
+000004b0: 6403 5300 2904 7212 0000 00da 0269 64da  d.S.).r......id.
+000004c0: 0a64 6174 6173 6574 5f69 644e 2905 7216  .dataset_idN).r.
+000004d0: 0000 0072 1700 0000 7218 0000 00da 0369  ...r....r......i
+000004e0: 6e74 721b 0000 0072 1c00 0000 721c 0000  ntr....r....r...
+000004f0: 0072 1c00 0000 721d 0000 0072 1200 0000  .r....r....r....
+00000500: 2f00 0000 7304 0000 000a 0108 0172 1200  /...s........r..
+00000510: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000520: 0000 0003 0000 0040 0000 0073 4c00 0000  .......@...sL...
+00000530: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
+00000540: 6505 6402 3c00 6506 6504 1900 6505 6403  e.d.<.e.e...e.d.
+00000550: 3c00 6507 6900 6404 8d01 5a08 6509 6504  <.e.i.d...Z.e.e.
+00000560: 650a 6602 1900 6505 6405 3c00 6406 5a0b  e.f...e.d.<.d.Z.
+00000570: 650c 6505 6407 3c00 6408 5300 2909 da0c  e.e.d.<.d.S.)...
+00000580: 5f44 6174 6173 6574 4261 7365 7a7e 0a20  _DatasetBasez~. 
+00000590: 2020 2042 6173 6520 636c 6173 7320 666f     Base class fo
+000005a0: 7220 4461 7461 7365 740a 0a20 2020 2041  r Dataset..    A
+000005b0: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
+000005c0: 2020 206e 616d 653a 2054 4244 0a20 2020     name: TBD.   
+000005d0: 2020 2020 2074 7970 653a 2054 4244 0a20       type: TBD. 
+000005e0: 2020 2020 2020 206d 6574 613a 2054 4244         meta: TBD
+000005f0: 0a20 2020 2020 2020 2072 6561 645f 6f6e  .        read_on
+00000600: 6c79 3a20 5442 440a 2020 2020 da04 6e61  ly: TBD.    ..na
+00000610: 6d65 da04 7479 7065 2901 da07 6465 6661  me..type)...defa
+00000620: 756c 74da 046d 6574 6146 da09 7265 6164  ult..metaF..read
+00000630: 5f6f 6e6c 794e 290d 7216 0000 0072 1700  _onlyN).r....r..
+00000640: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00000650: 0072 1b00 0000 7205 0000 0072 0600 0000  .r....r....r....
+00000660: 7229 0000 0072 0300 0000 7202 0000 0072  r)...r....r....r
+00000670: 2a00 0000 da04 626f 6f6c 721c 0000 0072  *.....boolr....r
+00000680: 1c00 0000 721c 0000 0072 1d00 0000 7225  ....r....r....r%
+00000690: 0000 0037 0000 0073 0a00 0000 0a01 040a  ...7...s........
+000006a0: 0801 0c01 1a01 7225 0000 0063 0000 0000  ......r%...c....
+000006b0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+000006c0: 4000 0000 7366 0000 0065 005a 0164 005a  @...sf...e.Z.d.Z
+000006d0: 0255 0065 0365 0419 0065 0564 013c 0064  .U.e.e...e.d.<.d
+000006e0: 025a 0665 0365 0765 0465 0866 0219 0019  .Z.e.e.e.e.f....
+000006f0: 0065 0564 033c 0065 0365 0919 0065 0564  .e.d.<.e.e...e.d
+00000700: 043c 0065 0a64 0164 0564 068d 0265 0b64  .<.e.d.d.d...e.d
+00000710: 0183 0183 015a 0c65 0a64 0764 0564 068d  .....Z.e.d.d.d..
+00000720: 0265 0b64 0783 0183 015a 0d64 0253 0029  .e.d.....Z.d.S.)
+00000730: 0872 0e00 0000 7226 0000 004e 7229 0000  .r....r&...Nr)..
+00000740: 0072 2a00 0000 5472 1e00 0000 7227 0000  .r*...Tr....r'..
+00000750: 0029 0e72 1600 0000 7217 0000 0072 1800  .).r....r....r..
+00000760: 0000 7205 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000770: 0072 2900 0000 7203 0000 0072 0200 0000  .r)...r....r....
+00000780: 722b 0000 0072 0700 0000 720a 0000 00da  r+...r....r.....
+00000790: 055f 6e61 6d65 da05 5f74 7970 6572 1c00  ._name.._typer..
+000007a0: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+000007b0: 0072 0e00 0000 4800 0000 730a 0000 000a  .r....H...s.....
+000007c0: 010c 0118 010c 0314 0172 0e00 0000 6300  .........r....c.
+000007d0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+000007e0: 0000 0040 0000 0073 3400 0000 6500 5a01  ...@...s4...e.Z.
+000007f0: 6400 5a02 6503 6401 6402 6403 8d02 6504  d.Z.e.d.d.d...e.
+00000800: 6401 8301 8301 5a05 6503 6404 6402 6403  d.....Z.e.d.d.d.
+00000810: 8d02 6504 6404 8301 8301 5a06 6405 5300  ..e.d.....Z.d.S.
+00000820: 2906 720f 0000 0072 2600 0000 5472 1e00  ).r....r&...Tr..
+00000830: 0000 7227 0000 004e 2907 7216 0000 0072  ..r'...N).r....r
+00000840: 1700 0000 7218 0000 0072 0700 0000 720a  ....r....r....r.
+00000850: 0000 0072 2c00 0000 722d 0000 0072 1c00  ...r,...r-...r..
+00000860: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000870: 0072 0f00 0000 5200 0000 7304 0000 0008  .r....R...s.....
+00000880: 0214 0172 0f00 0000 6300 0000 0000 0000  ...r....c.......
+00000890: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000008a0: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
+000008b0: 6503 6504 6401 3c00 6505 6506 1900 6504  e.e.d.<.e.e...e.
+000008c0: 6402 3c00 6503 6504 6403 3c00 6507 6504  d.<.e.e.d.<.e.e.
+000008d0: 6404 3c00 6405 5300 2906 7210 0000 0072  d.<.d.S.).r....r
+000008e0: 2200 0000 da0d 7265 736f 7572 6365 5f6c  ".....resource_l
+000008f0: 6973 74da 0a70 726f 6a65 6374 5f69 6472  ist..project_idr
+00000900: 2a00 0000 4e29 0872 1600 0000 7217 0000  *...N).r....r...
+00000910: 0072 1800 0000 7224 0000 0072 1b00 0000  .r....r$...r....
+00000920: 7204 0000 0072 1200 0000 722b 0000 0072  r....r....r+...r
+00000930: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
+00000940: 0000 0072 1000 0000 5800 0000 7308 0000  ...r....X...s...
+00000950: 000a 0108 010c 0108 0172 1000 0000 6300  .........r....c.
+00000960: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000970: 0000 0040 0000 0073 2e00 0000 6500 5a01  ...@...s....e.Z.
+00000980: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
+00000990: 3c00 6504 6505 6403 3c00 6404 5a06 6507  <.e.e.d.<.d.Z.e.
+000009a0: 6505 6405 3c00 6406 5300 2907 da0c 5f50  e.d.<.d.S.)..._P
+000009b0: 726f 6a65 6374 4261 7365 7a73 0a20 2020  rojectBasezs.   
+000009c0: 2042 6173 6520 636c 6173 7320 666f 7220   Base class for 
+000009d0: 5072 6f6a 6563 740a 0a20 2020 2041 7474  Project..    Att
+000009e0: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
+000009f0: 206e 616d 653a 2054 4244 0a20 2020 2020   name: TBD.     
+00000a00: 2020 2070 726f 6a65 6374 5f64 6972 3a20     project_dir: 
+00000a10: 5442 440a 2020 2020 2020 2020 7265 6164  TBD.        read
+00000a20: 5f6f 6e6c 793a 2054 4244 0a20 2020 2072  _only: TBD.    r
+00000a30: 2600 0000 da0b 7072 6f6a 6563 745f 6469  &.....project_di
+00000a40: 7246 722a 0000 004e 2908 7216 0000 0072  rFr*...N).r....r
+00000a50: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
+00000a60: 0000 0072 1b00 0000 722a 0000 0072 2b00  ...r....r*...r+.
+00000a70: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
+00000a80: 0072 1d00 0000 7230 0000 0062 0000 0073  .r....r0...b...s
+00000a90: 0800 0000 0a01 0409 0801 0801 7230 0000  ............r0..
+00000aa0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000ab0: 0000 0400 0000 4000 0000 735a 0000 0065  ......@...sZ...e
+00000ac0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
+00000ad0: 0519 0065 0664 023c 0065 0764 0364 0464  ...e.d.<.e.d.d.d
+00000ae0: 058d 0265 0864 0383 0183 015a 0965 0764  ...e.d.....Z.e.d
+00000af0: 0664 0464 058d 0265 0864 0683 0183 015a  .d.d...e.d.....Z
+00000b00: 0a65 0764 0264 0464 058d 0265 0864 0283  .e.d.d.d...e.d..
+00000b10: 0183 015a 0b64 0753 0029 0872 0b00 0000  ...Z.d.S.).r....
+00000b20: 7228 0000 00da 1464 6566 6175 6c74 5f64  r(.....default_d
+00000b30: 6174 6173 6574 5f6e 616d 6572 2600 0000  ataset_namer&...
+00000b40: 5472 1e00 0000 7231 0000 004e 290c 7216  Tr....r1...N).r.
+00000b50: 0000 0072 1700 0000 7218 0000 0072 3200  ...r....r....r2.
+00000b60: 0000 7205 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000b70: 0072 0700 0000 720a 0000 0072 2c00 0000  .r....r....r,...
+00000b80: da0c 5f70 726f 6a65 6374 5f64 6972 5a15  .._project_dirZ.
+00000b90: 5f64 6566 6175 6c74 5f64 6174 6173 6574  _default_dataset
+00000ba0: 5f6e 616d 6572 1c00 0000 721c 0000 0072  _namer....r....r
+00000bb0: 1c00 0000 721d 0000 0072 0b00 0000 7100  ....r....r....q.
+00000bc0: 0000 7314 0000 000a 0110 0314 010a 0106  ..s.............
+00000bd0: ff04 0302 0104 ff04 0206 fe72 0b00 0000  ...........r....
+00000be0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000bf0: 0003 0000 0040 0000 0073 2600 0000 6500  .....@...s&...e.
+00000c00: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+00000c10: 6700 5a05 6506 6507 1900 6504 6402 3c00  g.Z.e.e...e.d.<.
+00000c20: 6403 5300 2904 720c 0000 0072 2200 0000  d.S.).r....r"...
+00000c30: da0c 6461 7461 7365 745f 6c69 7374 4e29  ..dataset_listN)
+00000c40: 0872 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000c50: 7224 0000 0072 1b00 0000 7234 0000 0072  r$...r....r4...r
+00000c60: 0400 0000 7210 0000 0072 1c00 0000 721c  ....r....r....r.
+00000c70: 0000 0072 1c00 0000 721d 0000 0072 0c00  ...r....r....r..
+00000c80: 0000 7e00 0000 7304 0000 000a 0108 0172  ..~...s........r
+00000c90: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000ca0: 0000 0000 0004 0000 0040 0000 0073 5a00  .........@...sZ.
+00000cb0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000cc0: 1900 6505 6401 3c00 6503 6504 1900 6505  ..e.d.<.e.e...e.
+00000cd0: 6402 3c00 6503 6506 1900 6505 6403 3c00  d.<.e.e...e.d.<.
+00000ce0: 6507 6401 6404 6405 8d02 6508 6401 8301  e.d.d.d...e.d...
+00000cf0: 8301 5a09 6507 6402 6404 6405 8d02 6508  ..Z.e.d.d.d...e.
+00000d00: 6402 8301 8301 5a0a 6406 5300 2907 720d  d.....Z.d.S.).r.
+00000d10: 0000 0072 2600 0000 7231 0000 0072 2a00  ...r&...r1...r*.
+00000d20: 0000 5472 1e00 0000 4e29 0b72 1600 0000  ..Tr....N).r....
+00000d30: 7217 0000 0072 1800 0000 7205 0000 0072  r....r....r....r
+00000d40: 1a00 0000 721b 0000 0072 2b00 0000 7207  ....r....r+...r.
+00000d50: 0000 0072 0a00 0000 722c 0000 0072 3300  ...r....r,...r3.
+00000d60: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
+00000d70: 0072 1d00 0000 720d 0000 0083 0000 0073  .r....r........s
+00000d80: 0e00 0000 0a01 0c01 0c01 0c03 1401 0a01  ................
+00000d90: 06ff 720d 0000 004e 2919 da06 7479 7069  ..r....N)...typi
+00000da0: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
+00000db0: 0072 0500 0000 da08 7079 6461 6e74 6963  .r......pydantic
+00000dc0: 7206 0000 0072 0700 0000 da08 7371 6c6d  r....r......sqlm
+00000dd0: 6f64 656c 7208 0000 00da 0b5f 7661 6c69  odelr......_vali
+00000de0: 6461 746f 7273 720a 0000 00da 075f 5f61  datorsr......__a
+00000df0: 6c6c 5f5f 7214 0000 0072 1100 0000 7213  ll__r....r....r.
+00000e00: 0000 0072 1200 0000 7225 0000 0072 0e00  ...r....r%...r..
+00000e10: 0000 720f 0000 0072 1000 0000 7230 0000  ..r....r....r0..
+00000e20: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000e30: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
+00000e40: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000e50: 0000 7328 0000 000c 010c 010c 010c 020c  ..s(............
+00000e60: 010c 010c 020c 0304 1010 0810 0510 0510  ................
+00000e70: 0810 1110 0a10 0610 0a10 0f10 0d10 05    ...............
```

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/project.cpython-39.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Mar 15 12:00:37 2023 UTC, .py size: 2737 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,232 +1,225 @@
-00000000: 610d 0d0a 0000 0000 65b3 1164 b10a 0000  a.......e..d....
+00000000: 6f0d 0d0a 0000 0000 5fad 2e64 df09 0000  o......._..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
+00000020: 0004 0000 0040 0000 0073 3401 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d06 5a06 0100 6400 6406 6c05  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000080: 0100 6408 6409 6c0a 6d0b 5a0b 0100 640a  ..d.d.l.m.Z...d.
-00000090: 5a0c 4700 640b 640c 8400 640c 6509 8303  Z.G.d.d...d.e...
-000000a0: 5a0d 4700 640d 640e 8400 640e 650d 8303  Z.G.d.d...d.e...
-000000b0: 5a0e 4700 640f 6410 8400 6410 650d 8303  Z.G.d.d...d.e...
-000000c0: 5a0f 4700 6411 6412 8400 6412 650d 8303  Z.G.d.d...d.e...
-000000d0: 5a10 4700 6413 6414 8400 6414 6509 8303  Z.G.d.d...d.e...
-000000e0: 5a11 4700 6415 6416 8400 6416 6511 8303  Z.G.d.d...d.e...
-000000f0: 5a12 4700 6417 6418 8400 6418 6511 8303  Z.G.d.d...d.e...
-00000100: 5a13 4700 6419 641a 8400 641a 6511 8303  Z.G.d.d...d.e...
-00000110: 5a14 4700 641b 641c 8400 641c 6509 8303  Z.G.d.d...d.e...
-00000120: 5a15 4700 641d 641e 8400 641e 6515 8303  Z.G.d.d...d.e...
-00000130: 5a16 4700 641f 6420 8400 6420 6515 8303  Z.G.d.d ..d e...
-00000140: 5a17 4700 6421 6422 8400 6422 6515 8303  Z.G.d!d"..d"e...
-00000150: 5a18 6423 5300 2924 e900 0000 0029 01da  Z.d#S.)$.....)..
-00000160: 0341 6e79 2901 da04 4469 6374 2901 da04  .Any)...Dict)...
-00000170: 4c69 7374 2901 da08 4f70 7469 6f6e 616c  List)...Optional
-00000180: 2901 da05 4669 656c 6429 01da 0976 616c  )...Field)...val
-00000190: 6964 6174 6f72 2901 da08 5351 4c4d 6f64  idator)...SQLMod
-000001a0: 656c e901 0000 0029 01da 0676 616c 7374  el.....)...valst
-000001b0: 7229 09da 0d50 726f 6a65 6374 4372 6561  r)...ProjectCrea
-000001c0: 7465 da0b 5072 6f6a 6563 7452 6561 64da  te..ProjectRead.
-000001d0: 0d50 726f 6a65 6374 5570 6461 7465 da0d  .ProjectUpdate..
-000001e0: 4461 7461 7365 7455 7064 6174 65da 0d44  DatasetUpdate..D
-000001f0: 6174 6173 6574 4372 6561 7465 da0b 4461  atasetCreate..Da
-00000200: 7461 7365 7452 6561 64da 0e52 6573 6f75  tasetRead..Resou
-00000210: 7263 6543 7265 6174 65da 0c52 6573 6f75  rceCreate..Resou
-00000220: 7263 6552 6561 64da 0e52 6573 6f75 7263  rceRead..Resourc
-00000230: 6555 7064 6174 6563 0000 0000 0000 0000  eUpdatec........
-00000240: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000250: 731a 0000 0065 005a 0164 005a 0255 0064  s....e.Z.d.Z.U.d
-00000260: 015a 0365 0465 0564 023c 0064 0353 0029  .Z.e.e.d.<.d.S.)
-00000270: 04da 0d5f 5265 736f 7572 6365 4261 7365  ..._ResourceBase
-00000280: 7a21 0a20 2020 2042 6173 6520 636c 6173  z!.    Base clas
-00000290: 7320 666f 7220 5265 736f 7572 6365 0a20  s for Resource. 
-000002a0: 2020 20da 0470 6174 684e 2906 da08 5f5f     ..pathN)...__
-000002b0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000002c0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000002d0: da07 5f5f 646f 635f 5fda 0373 7472 da0f  ..__doc__..str..
-000002e0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fa9  __annotations__.
-000002f0: 0072 1c00 0000 721c 0000 00fa 3f2f 686f  .r....r.....?/ho
-00000300: 6d65 2f74 6f6d 6d61 736f 2f46 7261 6374  me/tommaso/Fract
-00000310: 616c 2f66 7261 6374 616c 2f66 7261 6374  al/fractal/fract
-00000320: 616c 2f63 6f6d 6d6f 6e2f 7363 6865 6d61  al/common/schema
-00000330: 732f 7072 6f6a 6563 742e 7079 7214 0000  s/project.pyr...
-00000340: 001d 0000 0073 0400 0000 0a01 0404 7214  .....s........r.
-00000350: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000360: 0000 0000 0400 0000 4000 0000 7320 0000  ........@...s ..
-00000370: 0065 005a 0164 005a 0265 0364 0164 0264  .e.Z.d.Z.e.d.d.d
-00000380: 038d 0265 0464 0183 0183 015a 0564 0453  ...e.d.....Z.d.S
-00000390: 0029 0572 1100 0000 7215 0000 0054 a901  .).r....r....T..
-000003a0: da0b 616c 6c6f 775f 7265 7573 654e a906  ..allow_reuseN..
-000003b0: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-000003c0: 0700 0000 720a 0000 00da 055f 7061 7468  ....r......_path
-000003d0: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-000003e0: 1d00 0000 7211 0000 0025 0000 0073 0200  ....r....%...s..
-000003f0: 0000 0802 7211 0000 0063 0000 0000 0000  ....r....c......
-00000400: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-00000410: 0000 7320 0000 0065 005a 0164 005a 0265  ..s ...e.Z.d.Z.e
-00000420: 0364 0164 0264 038d 0265 0464 0183 0183  .d.d.d...e.d....
-00000430: 015a 0564 0453 0029 0572 1300 0000 7215  .Z.d.S.).r....r.
-00000440: 0000 0054 721e 0000 004e 7220 0000 0072  ...Tr....Nr ...r
-00000450: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
-00000460: 0000 0072 1300 0000 2a00 0000 7302 0000  ...r....*...s...
-00000470: 0008 0272 1300 0000 6300 0000 0000 0000  ...r....c.......
-00000480: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000490: 0073 1e00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-000004a0: 6503 6504 6401 3c00 6503 6504 6402 3c00  e.e.d.<.e.e.d.<.
-000004b0: 6403 5300 2904 7212 0000 00da 0269 64da  d.S.).r......id.
-000004c0: 0a64 6174 6173 6574 5f69 644e 2905 7216  .dataset_idN).r.
-000004d0: 0000 0072 1700 0000 7218 0000 00da 0369  ...r....r......i
-000004e0: 6e74 721b 0000 0072 1c00 0000 721c 0000  ntr....r....r...
-000004f0: 0072 1c00 0000 721d 0000 0072 1200 0000  .r....r....r....
-00000500: 2f00 0000 7304 0000 000a 0108 0172 1200  /...s........r..
-00000510: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000520: 0000 0003 0000 0040 0000 0073 4c00 0000  .......@...sL...
-00000530: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
-00000540: 6505 6402 3c00 6506 6504 1900 6505 6403  e.d.<.e.e...e.d.
-00000550: 3c00 6507 6900 6404 8d01 5a08 6509 6504  <.e.i.d...Z.e.e.
-00000560: 650a 6602 1900 6505 6405 3c00 6406 5a0b  e.f...e.d.<.d.Z.
-00000570: 650c 6505 6407 3c00 6408 5300 2909 da0c  e.e.d.<.d.S.)...
-00000580: 5f44 6174 6173 6574 4261 7365 7a7e 0a20  _DatasetBasez~. 
-00000590: 2020 2042 6173 6520 636c 6173 7320 666f     Base class fo
-000005a0: 7220 4461 7461 7365 740a 0a20 2020 2041  r Dataset..    A
-000005b0: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-000005c0: 2020 206e 616d 653a 2054 4244 0a20 2020     name: TBD.   
-000005d0: 2020 2020 2074 7970 653a 2054 4244 0a20       type: TBD. 
-000005e0: 2020 2020 2020 206d 6574 613a 2054 4244         meta: TBD
-000005f0: 0a20 2020 2020 2020 2072 6561 645f 6f6e  .        read_on
-00000600: 6c79 3a20 5442 440a 2020 2020 da04 6e61  ly: TBD.    ..na
-00000610: 6d65 da04 7479 7065 2901 da07 6465 6661  me..type)...defa
-00000620: 756c 74da 046d 6574 6146 da09 7265 6164  ult..metaF..read
-00000630: 5f6f 6e6c 794e 290d 7216 0000 0072 1700  _onlyN).r....r..
+00000080: 0100 6408 6409 6c0a 6d0b 5a0b 0100 6408  ..d.d.l.m.Z...d.
+00000090: 640a 6c0a 6d0c 5a0c 0100 640b 5a0d 4700  d.l.m.Z...d.Z.G.
+000000a0: 640c 640d 8400 640d 6509 8303 5a0e 4700  d.d...d.e...Z.G.
+000000b0: 640e 640f 8400 640f 650e 8303 5a0f 4700  d.d...d.e...Z.G.
+000000c0: 6410 6411 8400 6411 650e 8303 5a10 4700  d.d...d.e...Z.G.
+000000d0: 6412 6413 8400 6413 650e 8303 5a11 4700  d.d...d.e...Z.G.
+000000e0: 6414 6415 8400 6415 6509 8303 5a12 4700  d.d...d.e...Z.G.
+000000f0: 6416 6417 8400 6417 6512 8303 5a13 4700  d.d...d.e...Z.G.
+00000100: 6418 6419 8400 6419 6512 8303 5a14 4700  d.d...d.e...Z.G.
+00000110: 641a 641b 8400 641b 6512 8303 5a15 4700  d.d...d.e...Z.G.
+00000120: 641c 641d 8400 641d 6509 8303 5a16 4700  d.d...d.e...Z.G.
+00000130: 641e 641f 8400 641f 6516 8303 5a17 4700  d.d...d.e...Z.G.
+00000140: 6420 6421 8400 6421 6516 8303 5a18 4700  d d!..d!e...Z.G.
+00000150: 6422 6423 8400 6423 6516 8303 5a19 6424  d"d#..d#e...Z.d$
+00000160: 5300 2925 e900 0000 0029 01da 0341 6e79  S.)%.....)...Any
+00000170: 2901 da04 4469 6374 2901 da04 4c69 7374  )...Dict)...List
+00000180: 2901 da08 4f70 7469 6f6e 616c 2901 da05  )...Optional)...
+00000190: 4669 656c 6429 01da 0976 616c 6964 6174  Field)...validat
+000001a0: 6f72 2901 da08 5351 4c4d 6f64 656c e901  or)...SQLModel..
+000001b0: 0000 0029 01da 1176 616c 5f61 6273 6f6c  ...)...val_absol
+000001c0: 7574 655f 7061 7468 2901 da06 7661 6c73  ute_path)...vals
+000001d0: 7472 2909 da0d 5072 6f6a 6563 7443 7265  tr)...ProjectCre
+000001e0: 6174 65da 0b50 726f 6a65 6374 5265 6164  ate..ProjectRead
+000001f0: da0d 5072 6f6a 6563 7455 7064 6174 65da  ..ProjectUpdate.
+00000200: 0d44 6174 6173 6574 5570 6461 7465 da0d  .DatasetUpdate..
+00000210: 4461 7461 7365 7443 7265 6174 65da 0b44  DatasetCreate..D
+00000220: 6174 6173 6574 5265 6164 da0e 5265 736f  atasetRead..Reso
+00000230: 7572 6365 4372 6561 7465 da0c 5265 736f  urceCreate..Reso
+00000240: 7572 6365 5265 6164 da0e 5265 736f 7572  urceRead..Resour
+00000250: 6365 5570 6461 7465 6300 0000 0000 0000  ceUpdatec.......
+00000260: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000270: 0073 1a00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000280: 6401 5a03 6504 6505 6402 3c00 6403 5300  d.Z.e.e.d.<.d.S.
+00000290: 2904 da0d 5f52 6573 6f75 7263 6542 6173  )..._ResourceBas
+000002a0: 657a 210a 2020 2020 4261 7365 2063 6c61  ez!.    Base cla
+000002b0: 7373 2066 6f72 2052 6573 6f75 7263 650a  ss for Resource.
+000002c0: 2020 2020 da04 7061 7468 4e29 06da 085f      ..pathN)..._
+000002d0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000002e0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000002f0: 5fda 075f 5f64 6f63 5f5f da03 7374 72da  _..__doc__..str.
+00000300: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+00000310: a900 721d 0000 0072 1d00 0000 fa3f 2f68  ..r....r.....?/h
+00000320: 6f6d 652f 746f 6d6d 6173 6f2f 4672 6163  ome/tommaso/Frac
+00000330: 7461 6c2f 6672 6163 7461 6c2f 6672 6163  tal/fractal/frac
+00000340: 7461 6c2f 636f 6d6d 6f6e 2f73 6368 656d  tal/common/schem
+00000350: 6173 2f70 726f 6a65 6374 2e70 7972 1500  as/project.pyr..
+00000360: 0000 1e00 0000 7306 0000 000a 0004 010c  ......s.........
+00000370: 0472 1500 0000 6300 0000 0000 0000 0000  .r....c.........
+00000380: 0000 0000 0000 0004 0000 0040 0000 00f3  ...........@....
+00000390: 2000 0000 6500 5a01 6400 5a02 6503 6401   ...e.Z.d.Z.e.d.
+000003a0: 6402 6403 8d02 6504 6401 8301 8301 5a05  d.d...e.d.....Z.
+000003b0: 6404 5300 2905 7212 0000 0072 1600 0000  d.S.).r....r....
+000003c0: 54a9 01da 0b61 6c6c 6f77 5f72 6575 7365  T....allow_reuse
+000003d0: 4ea9 0672 1700 0000 7218 0000 0072 1900  N..r....r....r..
+000003e0: 0000 7207 0000 0072 0a00 0000 da05 5f70  ..r....r......_p
+000003f0: 6174 6872 1d00 0000 721d 0000 0072 1d00  athr....r....r..
+00000400: 0000 721e 0000 0072 1200 0000 2600 0000  ..r....r....&...
+00000410: f304 0000 0008 0018 0272 1200 0000 6300  .........r....c.
+00000420: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000430: 0000 0040 0000 0072 1f00 0000 2905 7214  ...@...r....).r.
+00000440: 0000 0072 1600 0000 5472 2000 0000 4e72  ...r....Tr ...Nr
+00000450: 2200 0000 721d 0000 0072 1d00 0000 721d  "...r....r....r.
+00000460: 0000 0072 1e00 0000 7214 0000 002b 0000  ...r....r....+..
+00000470: 0072 2400 0000 7214 0000 0063 0000 0000  .r$...r....c....
+00000480: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000490: 4000 0000 731e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+000004a0: 0255 0065 0365 0464 013c 0065 0365 0464  .U.e.e.d.<.e.e.d
+000004b0: 023c 0064 0353 0029 0472 1300 0000 da02  .<.d.S.).r......
+000004c0: 6964 da0a 6461 7461 7365 745f 6964 4e29  id..dataset_idN)
+000004d0: 0572 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
+000004e0: da03 696e 7472 1c00 0000 721d 0000 0072  ..intr....r....r
+000004f0: 1d00 0000 721d 0000 0072 1e00 0000 7213  ....r....r....r.
+00000500: 0000 0030 0000 0073 0600 0000 0a00 0801  ...0...s........
+00000510: 0c01 7213 0000 0063 0000 0000 0000 0000  ..r....c........
+00000520: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000530: 734c 0000 0065 005a 0164 005a 0255 0064  sL...e.Z.d.Z.U.d
+00000540: 015a 0365 0465 0564 023c 0065 0665 0419  .Z.e.e.d.<.e.e..
+00000550: 0065 0564 033c 0065 0769 0064 048d 015a  .e.d.<.e.i.d...Z
+00000560: 0865 0965 0465 0a66 0219 0065 0564 053c  .e.e.e.f...e.d.<
+00000570: 0064 065a 0b65 0c65 0564 073c 0064 0853  .d.Z.e.e.d.<.d.S
+00000580: 0029 09da 0c5f 4461 7461 7365 7442 6173  .)..._DatasetBas
+00000590: 657a 7e0a 2020 2020 4261 7365 2063 6c61  ez~.    Base cla
+000005a0: 7373 2066 6f72 2044 6174 6173 6574 0a0a  ss for Dataset..
+000005b0: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
+000005c0: 2020 2020 2020 2020 6e61 6d65 3a20 5442          name: TB
+000005d0: 440a 2020 2020 2020 2020 7479 7065 3a20  D.        type: 
+000005e0: 5442 440a 2020 2020 2020 2020 6d65 7461  TBD.        meta
+000005f0: 3a20 5442 440a 2020 2020 2020 2020 7265  : TBD.        re
+00000600: 6164 5f6f 6e6c 793a 2054 4244 0a20 2020  ad_only: TBD.   
+00000610: 20da 046e 616d 65da 0474 7970 6529 01da   ..name..type)..
+00000620: 0764 6566 6175 6c74 da04 6d65 7461 46da  .default..metaF.
+00000630: 0972 6561 645f 6f6e 6c79 4e29 0d72 1700  .read_onlyN).r..
 00000640: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000650: 0072 1b00 0000 7205 0000 0072 0600 0000  .r....r....r....
-00000660: 7229 0000 0072 0300 0000 7202 0000 0072  r)...r....r....r
-00000670: 2a00 0000 da04 626f 6f6c 721c 0000 0072  *.....boolr....r
-00000680: 1c00 0000 721c 0000 0072 1d00 0000 7225  ....r....r....r%
-00000690: 0000 0037 0000 0073 0a00 0000 0a01 040a  ...7...s........
-000006a0: 0801 0c01 1a01 7225 0000 0063 0000 0000  ......r%...c....
-000006b0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-000006c0: 4000 0000 7366 0000 0065 005a 0164 005a  @...sf...e.Z.d.Z
-000006d0: 0255 0065 0365 0419 0065 0564 013c 0064  .U.e.e...e.d.<.d
-000006e0: 025a 0665 0365 0765 0465 0866 0219 0019  .Z.e.e.e.e.f....
-000006f0: 0065 0564 033c 0065 0365 0919 0065 0564  .e.d.<.e.e...e.d
-00000700: 043c 0065 0a64 0164 0564 068d 0265 0b64  .<.e.d.d.d...e.d
-00000710: 0183 0183 015a 0c65 0a64 0764 0564 068d  .....Z.e.d.d.d..
-00000720: 0265 0b64 0783 0183 015a 0d64 0253 0029  .e.d.....Z.d.S.)
-00000730: 0872 0e00 0000 7226 0000 004e 7229 0000  .r....r&...Nr)..
-00000740: 0072 2a00 0000 5472 1e00 0000 7227 0000  .r*...Tr....r'..
-00000750: 0029 0e72 1600 0000 7217 0000 0072 1800  .).r....r....r..
-00000760: 0000 7205 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000770: 0072 2900 0000 7203 0000 0072 0200 0000  .r)...r....r....
-00000780: 722b 0000 0072 0700 0000 720a 0000 00da  r+...r....r.....
-00000790: 055f 6e61 6d65 da05 5f74 7970 6572 1c00  ._name.._typer..
-000007a0: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-000007b0: 0072 0e00 0000 4800 0000 730a 0000 000a  .r....H...s.....
-000007c0: 010c 0118 010c 0314 0172 0e00 0000 6300  .........r....c.
-000007d0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-000007e0: 0000 0040 0000 0073 3400 0000 6500 5a01  ...@...s4...e.Z.
-000007f0: 6400 5a02 6503 6401 6402 6403 8d02 6504  d.Z.e.d.d.d...e.
-00000800: 6401 8301 8301 5a05 6503 6404 6402 6403  d.....Z.e.d.d.d.
-00000810: 8d02 6504 6404 8301 8301 5a06 6405 5300  ..e.d.....Z.d.S.
-00000820: 2906 720f 0000 0072 2600 0000 5472 1e00  ).r....r&...Tr..
-00000830: 0000 7227 0000 004e 2907 7216 0000 0072  ..r'...N).r....r
-00000840: 1700 0000 7218 0000 0072 0700 0000 720a  ....r....r....r.
-00000850: 0000 0072 2c00 0000 722d 0000 0072 1c00  ...r,...r-...r..
-00000860: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000870: 0072 0f00 0000 5200 0000 7304 0000 0008  .r....R...s.....
-00000880: 0214 0172 0f00 0000 6300 0000 0000 0000  ...r....c.......
-00000890: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000008a0: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
-000008b0: 6503 6504 6401 3c00 6505 6506 1900 6504  e.e.d.<.e.e...e.
-000008c0: 6402 3c00 6503 6504 6403 3c00 6507 6504  d.<.e.e.d.<.e.e.
-000008d0: 6404 3c00 6405 5300 2906 7210 0000 0072  d.<.d.S.).r....r
-000008e0: 2200 0000 da0d 7265 736f 7572 6365 5f6c  ".....resource_l
-000008f0: 6973 74da 0a70 726f 6a65 6374 5f69 6472  ist..project_idr
-00000900: 2a00 0000 4e29 0872 1600 0000 7217 0000  *...N).r....r...
-00000910: 0072 1800 0000 7224 0000 0072 1b00 0000  .r....r$...r....
-00000920: 7204 0000 0072 1200 0000 722b 0000 0072  r....r....r+...r
-00000930: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
-00000940: 0000 0072 1000 0000 5800 0000 7308 0000  ...r....X...s...
-00000950: 000a 0108 010c 0108 0172 1000 0000 6300  .........r....c.
-00000960: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000970: 0000 0040 0000 0073 2e00 0000 6500 5a01  ...@...s....e.Z.
-00000980: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
-00000990: 3c00 6504 6505 6403 3c00 6404 5a06 6507  <.e.e.d.<.d.Z.e.
-000009a0: 6505 6405 3c00 6406 5300 2907 da0c 5f50  e.d.<.d.S.)..._P
-000009b0: 726f 6a65 6374 4261 7365 7a73 0a20 2020  rojectBasezs.   
-000009c0: 2042 6173 6520 636c 6173 7320 666f 7220   Base class for 
-000009d0: 5072 6f6a 6563 740a 0a20 2020 2041 7474  Project..    Att
-000009e0: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
-000009f0: 206e 616d 653a 2054 4244 0a20 2020 2020   name: TBD.     
-00000a00: 2020 2070 726f 6a65 6374 5f64 6972 3a20     project_dir: 
-00000a10: 5442 440a 2020 2020 2020 2020 7265 6164  TBD.        read
-00000a20: 5f6f 6e6c 793a 2054 4244 0a20 2020 2072  _only: TBD.    r
-00000a30: 2600 0000 da0b 7072 6f6a 6563 745f 6469  &.....project_di
-00000a40: 7246 722a 0000 004e 2908 7216 0000 0072  rFr*...N).r....r
-00000a50: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00000a60: 0000 0072 1b00 0000 722a 0000 0072 2b00  ...r....r*...r+.
-00000a70: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-00000a80: 0072 1d00 0000 7230 0000 0062 0000 0073  .r....r0...b...s
-00000a90: 0800 0000 0a01 0409 0801 0801 7230 0000  ............r0..
-00000aa0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000ab0: 0000 0400 0000 4000 0000 735a 0000 0065  ......@...sZ...e
-00000ac0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
-00000ad0: 0519 0065 0664 023c 0065 0764 0364 0464  ...e.d.<.e.d.d.d
-00000ae0: 058d 0265 0864 0383 0183 015a 0965 0764  ...e.d.....Z.e.d
-00000af0: 0664 0464 058d 0265 0864 0683 0183 015a  .d.d...e.d.....Z
-00000b00: 0a65 0764 0264 0464 058d 0265 0864 0283  .e.d.d.d...e.d..
-00000b10: 0183 015a 0b64 0753 0029 0872 0b00 0000  ...Z.d.S.).r....
-00000b20: 7228 0000 00da 1464 6566 6175 6c74 5f64  r(.....default_d
-00000b30: 6174 6173 6574 5f6e 616d 6572 2600 0000  ataset_namer&...
-00000b40: 5472 1e00 0000 7231 0000 004e 290c 7216  Tr....r1...N).r.
-00000b50: 0000 0072 1700 0000 7218 0000 0072 3200  ...r....r....r2.
-00000b60: 0000 7205 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000b70: 0072 0700 0000 720a 0000 0072 2c00 0000  .r....r....r,...
-00000b80: da0c 5f70 726f 6a65 6374 5f64 6972 5a15  .._project_dirZ.
-00000b90: 5f64 6566 6175 6c74 5f64 6174 6173 6574  _default_dataset
-00000ba0: 5f6e 616d 6572 1c00 0000 721c 0000 0072  _namer....r....r
-00000bb0: 1c00 0000 721d 0000 0072 0b00 0000 7100  ....r....r....q.
-00000bc0: 0000 7314 0000 000a 0110 0314 010a 0106  ..s.............
-00000bd0: ff04 0302 0104 ff04 0206 fe72 0b00 0000  ...........r....
-00000be0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000bf0: 0003 0000 0040 0000 0073 2600 0000 6500  .....@...s&...e.
-00000c00: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
-00000c10: 6700 5a05 6506 6507 1900 6504 6402 3c00  g.Z.e.e...e.d.<.
-00000c20: 6403 5300 2904 720c 0000 0072 2200 0000  d.S.).r....r"...
-00000c30: da0c 6461 7461 7365 745f 6c69 7374 4e29  ..dataset_listN)
-00000c40: 0872 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000c50: 7224 0000 0072 1b00 0000 7234 0000 0072  r$...r....r4...r
-00000c60: 0400 0000 7210 0000 0072 1c00 0000 721c  ....r....r....r.
-00000c70: 0000 0072 1c00 0000 721d 0000 0072 0c00  ...r....r....r..
-00000c80: 0000 7e00 0000 7304 0000 000a 0108 0172  ..~...s........r
-00000c90: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000ca0: 0000 0000 0004 0000 0040 0000 0073 5a00  .........@...sZ.
-00000cb0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000cc0: 1900 6505 6401 3c00 6503 6504 1900 6505  ..e.d.<.e.e...e.
-00000cd0: 6402 3c00 6503 6506 1900 6505 6403 3c00  d.<.e.e...e.d.<.
-00000ce0: 6507 6401 6404 6405 8d02 6508 6401 8301  e.d.d.d...e.d...
-00000cf0: 8301 5a09 6507 6402 6404 6405 8d02 6508  ..Z.e.d.d.d...e.
-00000d00: 6402 8301 8301 5a0a 6406 5300 2907 720d  d.....Z.d.S.).r.
-00000d10: 0000 0072 2600 0000 7231 0000 0072 2a00  ...r&...r1...r*.
-00000d20: 0000 5472 1e00 0000 4e29 0b72 1600 0000  ..Tr....N).r....
-00000d30: 7217 0000 0072 1800 0000 7205 0000 0072  r....r....r....r
-00000d40: 1a00 0000 721b 0000 0072 2b00 0000 7207  ....r....r+...r.
-00000d50: 0000 0072 0a00 0000 722c 0000 0072 3300  ...r....r,...r3.
-00000d60: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-00000d70: 0072 1d00 0000 720d 0000 0083 0000 0073  .r....r........s
-00000d80: 0e00 0000 0a01 0c01 0c01 0c03 1401 0a01  ................
-00000d90: 06ff 720d 0000 004e 2919 da06 7479 7069  ..r....N)...typi
-00000da0: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
-00000db0: 0072 0500 0000 da08 7079 6461 6e74 6963  .r......pydantic
-00000dc0: 7206 0000 0072 0700 0000 da08 7371 6c6d  r....r......sqlm
-00000dd0: 6f64 656c 7208 0000 00da 0b5f 7661 6c69  odelr......_vali
-00000de0: 6461 746f 7273 720a 0000 00da 075f 5f61  datorsr......__a
-00000df0: 6c6c 5f5f 7214 0000 0072 1100 0000 7213  ll__r....r....r.
-00000e00: 0000 0072 1200 0000 7225 0000 0072 0e00  ...r....r%...r..
-00000e10: 0000 720f 0000 0072 1000 0000 7230 0000  ..r....r....r0..
-00000e20: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000e30: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-00000e40: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000e50: 0000 7328 0000 000c 010c 010c 010c 020c  ..s(............
-00000e60: 010c 010c 020c 0304 1010 0810 0510 0510  ................
-00000e70: 0810 1110 0a10 0610 0a10 0f10 0d10 05    ...............
+00000650: 0072 1b00 0000 721c 0000 0072 0500 0000  .r....r....r....
+00000660: 7206 0000 0072 2c00 0000 7203 0000 0072  r....r,...r....r
+00000670: 0200 0000 722d 0000 00da 0462 6f6f 6c72  ....r-.....boolr
+00000680: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
+00000690: 0000 0072 2800 0000 3800 0000 730c 0000  ...r(...8...s...
+000006a0: 000a 0004 0108 0a0c 011a 0110 0172 2800  .............r(.
+000006b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000006c0: 0000 0004 0000 0040 0000 0073 6600 0000  .......@...sf...
+000006d0: 6500 5a01 6400 5a02 5500 6503 6504 1900  e.Z.d.Z.U.e.e...
+000006e0: 6505 6401 3c00 6402 5a06 6503 6507 6504  e.d.<.d.Z.e.e.e.
+000006f0: 6508 6602 1900 1900 6505 6403 3c00 6503  e.f.....e.d.<.e.
+00000700: 6509 1900 6505 6404 3c00 650a 6401 6405  e...e.d.<.e.d.d.
+00000710: 6406 8d02 650b 6401 8301 8301 5a0c 650a  d...e.d.....Z.e.
+00000720: 6407 6405 6406 8d02 650b 6407 8301 8301  d.d.d...e.d.....
+00000730: 5a0d 6402 5300 2908 720f 0000 0072 2900  Z.d.S.).r....r).
+00000740: 0000 4e72 2c00 0000 722d 0000 0054 7220  ..Nr,...r-...Tr 
+00000750: 0000 0072 2a00 0000 290e 7217 0000 0072  ...r*...).r....r
+00000760: 1800 0000 7219 0000 0072 0500 0000 721b  ....r....r....r.
+00000770: 0000 0072 1c00 0000 722c 0000 0072 0300  ...r....r,...r..
+00000780: 0000 7202 0000 0072 2e00 0000 7207 0000  ..r....r....r...
+00000790: 0072 0b00 0000 da05 5f6e 616d 65da 055f  .r......_name.._
+000007a0: 7479 7065 721d 0000 0072 1d00 0000 721d  typer....r....r.
+000007b0: 0000 0072 1e00 0000 720f 0000 0049 0000  ...r....r....I..
+000007c0: 0073 0c00 0000 0a00 0c01 1801 0c01 1403  .s..............
+000007d0: 1801 720f 0000 0063 0000 0000 0000 0000  ..r....c........
+000007e0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
+000007f0: 7334 0000 0065 005a 0164 005a 0265 0364  s4...e.Z.d.Z.e.d
+00000800: 0164 0264 038d 0265 0464 0183 0183 015a  .d.d...e.d.....Z
+00000810: 0565 0364 0464 0264 038d 0265 0464 0483  .e.d.d.d...e.d..
+00000820: 0183 015a 0664 0553 0029 0672 1000 0000  ...Z.d.S.).r....
+00000830: 7229 0000 0054 7220 0000 0072 2a00 0000  r)...Tr ...r*...
+00000840: 4e29 0772 1700 0000 7218 0000 0072 1900  N).r....r....r..
+00000850: 0000 7207 0000 0072 0b00 0000 722f 0000  ..r....r....r/..
+00000860: 0072 3000 0000 721d 0000 0072 1d00 0000  .r0...r....r....
+00000870: 721d 0000 0072 1e00 0000 7210 0000 0053  r....r....r....S
+00000880: 0000 0073 0600 0000 0800 1402 1801 7210  ...s..........r.
+00000890: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000008a0: 0000 0000 0300 0000 4000 0000 7332 0000  ........@...s2..
+000008b0: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
+000008c0: 013c 0065 0565 0619 0065 0464 023c 0065  .<.e.e...e.d.<.e
+000008d0: 0365 0464 033c 0065 0765 0464 043c 0064  .e.d.<.e.e.d.<.d
+000008e0: 0553 0029 0672 1100 0000 7225 0000 00da  .S.).r....r%....
+000008f0: 0d72 6573 6f75 7263 655f 6c69 7374 da0a  .resource_list..
+00000900: 7072 6f6a 6563 745f 6964 722d 0000 004e  project_idr-...N
+00000910: 2908 7217 0000 0072 1800 0000 7219 0000  ).r....r....r...
+00000920: 0072 2700 0000 721c 0000 0072 0400 0000  .r'...r....r....
+00000930: 7213 0000 0072 2e00 0000 721d 0000 0072  r....r....r....r
+00000940: 1d00 0000 721d 0000 0072 1e00 0000 7211  ....r....r....r.
+00000950: 0000 0059 0000 0073 0a00 0000 0a00 0801  ...Y...s........
+00000960: 0c01 0801 0c01 7211 0000 0063 0000 0000  ......r....c....
+00000970: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000980: 4000 0000 7326 0000 0065 005a 0164 005a  @...s&...e.Z.d.Z
+00000990: 0255 0064 015a 0365 0465 0564 023c 0064  .U.d.Z.e.e.d.<.d
+000009a0: 035a 0665 0765 0564 043c 0064 0553 0029  .Z.e.e.d.<.d.S.)
+000009b0: 06da 0c5f 5072 6f6a 6563 7442 6173 657a  ..._ProjectBasez
+000009c0: 5a0a 2020 2020 4261 7365 2063 6c61 7373  Z.    Base class
+000009d0: 2066 6f72 2050 726f 6a65 6374 0a0a 2020   for Project..  
+000009e0: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
+000009f0: 2020 2020 2020 6e61 6d65 3a20 5442 440a        name: TBD.
+00000a00: 2020 2020 2020 2020 7265 6164 5f6f 6e6c          read_onl
+00000a10: 793a 2054 4244 0a20 2020 2072 2900 0000  y: TBD.    r)...
+00000a20: 4672 2d00 0000 4e29 0872 1700 0000 7218  Fr-...N).r....r.
+00000a30: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+00000a40: 0000 721c 0000 0072 2d00 0000 722e 0000  ..r....r-...r...
+00000a50: 0072 1d00 0000 721d 0000 0072 1d00 0000  .r....r....r....
+00000a60: 721e 0000 0072 3300 0000 6300 0000 7308  r....r3...c...s.
+00000a70: 0000 000a 0004 0108 0810 0172 3300 0000  ...........r3...
+00000a80: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000a90: 0004 0000 0040 0000 0073 4600 0000 6500  .....@...sF...e.
+00000aa0: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
+00000ab0: 1900 6506 6402 3c00 6507 6403 6404 6405  ..e.d.<.e.d.d.d.
+00000ac0: 8d02 6508 6403 8301 8301 5a09 6507 6402  ..e.d.....Z.e.d.
+00000ad0: 6404 6405 8d02 6508 6402 8301 8301 5a0a  d.d...e.d.....Z.
+00000ae0: 6406 5300 2907 720c 0000 0072 2b00 0000  d.S.).r....r+...
+00000af0: da14 6465 6661 756c 745f 6461 7461 7365  ..default_datase
+00000b00: 745f 6e61 6d65 7229 0000 0054 7220 0000  t_namer)...Tr ..
+00000b10: 004e 290b 7217 0000 0072 1800 0000 7219  .N).r....r....r.
+00000b20: 0000 0072 3400 0000 7205 0000 0072 1b00  ...r4...r....r..
+00000b30: 0000 721c 0000 0072 0700 0000 720b 0000  ..r....r....r...
+00000b40: 0072 2f00 0000 da15 5f64 6566 6175 6c74  .r/....._default
+00000b50: 5f64 6174 6173 6574 5f6e 616d 6572 1d00  _dataset_namer..
+00000b60: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000b70: 0072 0c00 0000 7000 0000 7310 0000 000a  .r....p...s.....
+00000b80: 0010 0114 0302 0104 0104 ff06 0208 fe72  ...............r
+00000b90: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000ba0: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
+00000bb0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000bc0: 6401 3c00 6700 5a05 6506 6507 1900 6504  d.<.g.Z.e.e...e.
+00000bd0: 6402 3c00 6403 5300 2904 720d 0000 0072  d.<.d.S.).r....r
+00000be0: 2500 0000 da0c 6461 7461 7365 745f 6c69  %.....dataset_li
+00000bf0: 7374 4e29 0872 1700 0000 7218 0000 0072  stN).r....r....r
+00000c00: 1900 0000 7227 0000 0072 1c00 0000 7236  ....r'...r....r6
+00000c10: 0000 0072 0400 0000 7211 0000 0072 1d00  ...r....r....r..
+00000c20: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000c30: 0072 0d00 0000 7a00 0000 7306 0000 000a  .r....z...s.....
+00000c40: 0008 0114 0172 0d00 0000 6300 0000 0000  .....r....c.....
+00000c50: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
+00000c60: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
+00000c70: 5500 6503 6504 1900 6505 6401 3c00 6503  U.e.e...e.d.<.e.
+00000c80: 6506 1900 6505 6402 3c00 6507 6401 6403  e...e.d.<.e.d.d.
+00000c90: 6404 8d02 6508 6401 8301 8301 5a09 6405  d...e.d.....Z.d.
+00000ca0: 5300 2906 720e 0000 0072 2900 0000 722d  S.).r....r)...r-
+00000cb0: 0000 0054 7220 0000 004e 290a 7217 0000  ...Tr ...N).r...
+00000cc0: 0072 1800 0000 7219 0000 0072 0500 0000  .r....r....r....
+00000cd0: 721b 0000 0072 1c00 0000 722e 0000 0072  r....r....r....r
+00000ce0: 0700 0000 720b 0000 0072 2f00 0000 721d  ....r....r/...r.
+00000cf0: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
+00000d00: 0000 720e 0000 007f 0000 0073 0800 0000  ..r........s....
+00000d10: 0a00 0c01 0c01 1803 720e 0000 004e 291a  ........r....N).
+00000d20: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
+00000d30: 0000 7204 0000 0072 0500 0000 da08 7079  ..r....r......py
+00000d40: 6461 6e74 6963 7206 0000 0072 0700 0000  danticr....r....
+00000d50: da08 7371 6c6d 6f64 656c 7208 0000 00da  ..sqlmodelr.....
+00000d60: 0b5f 7661 6c69 6461 746f 7273 720a 0000  ._validatorsr...
+00000d70: 0072 0b00 0000 da07 5f5f 616c 6c5f 5f72  .r......__all__r
+00000d80: 1500 0000 7212 0000 0072 1400 0000 7213  ....r....r....r.
+00000d90: 0000 0072 2800 0000 720f 0000 0072 1000  ...r(...r....r..
+00000da0: 0000 7211 0000 0072 3300 0000 720c 0000  ..r....r3...r...
+00000db0: 0072 0d00 0000 720e 0000 0072 1d00 0000  .r....r....r....
+00000dc0: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
+00000dd0: 083c 6d6f 6475 6c65 3e01 0000 0073 2c00  .<module>....s,.
+00000de0: 0000 0c00 0c01 0c01 0c01 0c02 0c01 0c01  ................
+00000df0: 0c02 0c01 0403 1010 1008 1005 1005 1008  ................
+00000e00: 1011 100a 1006 100a 100d 100a 1405       ..............
```

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/state.cpython-39.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 13:52:21 2023 UTC, .py size: 4484 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 15f0 0564 8411 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 5aa6 5a64 e310 0000  o.......Z.Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c02 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c02 6d06 5a06 0100 6400 6406 6c02  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
@@ -215,99 +215,95 @@
 00000d60: 3a20 5442 440a 2020 2020 2020 2020 7061  : TBD.        pa
 00000d70: 636b 6167 655f 6578 7472 6173 3a20 5442  ckage_extras: TB
 00000d80: 440a 2020 2020 da07 7061 636b 6167 65da  D.    ..package.
 00000d90: 0776 6572 7369 6f6e 4eda 0e70 7974 686f  .versionN..pytho
 00000da0: 6e5f 7665 7273 696f 6eda 0e70 6163 6b61  n_version..packa
 00000db0: 6765 5f65 7874 7261 7363 0200 0000 0000  ge_extrasc......
 00000dc0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00000dd0: 0000 7340 0000 0064 017c 0176 0072 1e74  ..s@...d.|.v.r.t
+00000dd0: 0000 732a 0000 0064 017c 0176 0072 1374  ..s*...d.|.v.r.t
 00000de0: 007c 0183 017d 027c 02a0 01a1 0073 1374  .|...}.|.....s.t
-00000df0: 0264 027c 029b 009d 0283 0182 017c 02a0  .d.|.........|..
-00000e00: 03a1 0073 1e74 0264 037c 029b 009d 0283  ...s.t.d.|......
-00000e10: 0182 017c 0153 0029 044e fa01 2f7a 1f50  ...|.S.).N../z.P
-00000e20: 6163 6b61 6765 2070 6174 6820 6d75 7374  ackage path must
-00000e30: 2062 6520 6162 736f 6c75 7465 3a20 7a1d   be absolute: z.
-00000e40: 5061 636b 6167 6520 6669 6c65 2064 6f65  Package file doe
-00000e50: 7320 6e6f 7420 6578 6973 743a 2029 0472  s not exist: ).r
-00000e60: 0200 0000 da0b 6973 5f61 6273 6f6c 7574  ......is_absolut
-00000e70: 65da 0a56 616c 7565 4572 726f 72da 0665  e..ValueError..e
-00000e80: 7869 7374 7329 03da 0363 6c73 da05 7661  xists)...cls..va
-00000e90: 6c75 65da 0c70 6163 6b61 6765 5f70 6174  lue..package_pat
-00000ea0: 6872 1e00 0000 721e 0000 0072 1f00 0000  hr....r....r....
-00000eb0: da15 7061 636b 6167 655f 7061 7468 5f61  ..package_path_a
-00000ec0: 6273 6f6c 7574 6584 0000 0073 1600 0000  bsolute....s....
-00000ed0: 0802 0801 0801 0201 0801 04ff 0803 0201  ................
-00000ee0: 0801 04ff 0403 7a24 5461 736b 436f 6c6c  ......z$TaskColl
-00000ef0: 6563 7450 6970 2e70 6163 6b61 6765 5f70  ectPip.package_p
-00000f00: 6174 685f 6162 736f 6c75 7465 290a 7218  ath_absolute).r.
-00000f10: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00000f20: 0000 721c 0000 0072 1d00 0000 7207 0000  ..r....r....r...
-00000f30: 0072 3600 0000 7209 0000 0072 3f00 0000  .r6...r....r?...
-00000f40: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-00000f50: 1f00 0000 7213 0000 0074 0000 0073 1000  ....r....t...s..
-00000f60: 0000 0a00 0401 080a 0c01 1001 0c01 0602  ................
-00000f70: 0e01 7213 0000 0063 0000 0000 0000 0000  ..r....c........
-00000f80: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000f90: 7368 0000 0065 005a 0164 005a 0255 0064  sh...e.Z.d.Z.U.d
-00000fa0: 015a 0365 0464 0219 0065 0564 033c 0065  .Z.e.d...e.d.<.e
-00000fb0: 0665 0564 043c 0065 0765 0564 053c 0065  .e.d.<.e.e.d.<.e
-00000fc0: 0867 0064 068d 015a 0965 0a65 0b65 0c19  .g.d...Z.e.e.e..
-00000fd0: 0019 0065 0564 073c 0065 0a65 0619 0065  ...e.d.<.e.e...e
-00000fe0: 0564 083c 0065 0a65 0619 0065 0564 093c  .d.<.e.e...e.d.<
-00000ff0: 0064 0a64 0b84 005a 0d64 0c53 0029 0d72  .d.d...Z.d.S.).r
-00001000: 1400 0000 7aac 0a20 2020 2054 6173 6b43  ....z..    TaskC
-00001010: 6f6c 6c65 6374 5374 6174 7573 2063 6c61  ollectStatus cla
-00001020: 7373 0a0a 2020 2020 4174 7472 6962 7574  ss..    Attribut
-00001030: 6573 3a0a 2020 2020 2020 2020 7374 6174  es:.        stat
-00001040: 7573 3a20 5442 440a 2020 2020 2020 2020  us: TBD.        
-00001050: 7061 636b 6167 653a 2054 4244 0a20 2020  package: TBD.   
-00001060: 2020 2020 2076 656e 765f 7061 7468 3a20       venv_path: 
-00001070: 5442 440a 2020 2020 2020 2020 7461 736b  TBD.        task
-00001080: 5f6c 6973 743a 2054 4244 0a20 2020 2020  _list: TBD.     
-00001090: 2020 206c 6f67 3a20 5442 440a 2020 2020     log: TBD.    
-000010a0: 2020 2020 696e 666f 3a20 5442 440a 2020      info: TBD.  
-000010b0: 2020 2905 da07 7065 6e64 696e 67da 0a69    )...pending..i
-000010c0: 6e73 7461 6c6c 696e 67da 0a63 6f6c 6c65  nstalling..colle
-000010d0: 6374 696e 67da 0466 6169 6cda 024f 4bda  cting..fail..OK.
-000010e0: 0673 7461 7475 7372 3400 0000 da09 7665  .statusr4.....ve
-000010f0: 6e76 5f70 6174 6872 3000 0000 da09 7461  nv_pathr0.....ta
-00001100: 736b 5f6c 6973 74da 036c 6f67 da04 696e  sk_list..log..in
-00001110: 666f 6301 0000 0000 0000 0000 0000 0002  foc.............
-00001120: 0000 0003 0000 0043 0000 0073 1a00 0000  .......C...s....
-00001130: 7c00 a000 a100 7d01 7401 7c00 6a02 8301  |.....}.t.|.j...
-00001140: 7c01 6401 3c00 7c01 5300 2902 7a51 0a20  |.d.<.|.S.).zQ. 
-00001150: 2020 2020 2020 2052 6574 7572 6e20 6073         Return `s
-00001160: 656c 662e 6469 6374 2829 6020 6166 7465  elf.dict()` afte
-00001170: 7220 6361 7374 696e 6720 6073 656c 662e  r casting `self.
-00001180: 7665 6e76 5f70 6174 6860 2074 6f20 6120  venv_path` to a 
-00001190: 7374 7269 6e67 0a20 2020 2020 2020 2072  string.        r
-000011a0: 4600 0000 2903 da04 6469 6374 721c 0000  F...)...dictr...
-000011b0: 0072 4600 0000 2902 da04 7365 6c66 da01  .rF...)...self..
-000011c0: 6472 1e00 0000 721e 0000 0072 1f00 0000  dr....r....r....
-000011d0: da0e 7361 6e69 7469 7365 645f 6469 6374  ..sanitised_dict
-000011e0: a700 0000 7306 0000 0008 040e 0104 017a  ....s..........z
-000011f0: 2054 6173 6b43 6f6c 6c65 6374 5374 6174   TaskCollectStat
-00001200: 7573 2e73 616e 6974 6973 6564 5f64 6963  us.sanitised_dic
-00001210: 744e 290e 7218 0000 0072 1900 0000 721a  tN).r....r....r.
-00001220: 0000 0072 1b00 0000 7206 0000 0072 1d00  ...r....r....r..
-00001230: 0000 721c 0000 0072 0200 0000 720a 0000  ..r....r....r...
-00001240: 0072 4700 0000 7207 0000 0072 0500 0000  .rG...r....r....
-00001250: 7210 0000 0072 4d00 0000 721e 0000 0072  r....rM...r....r
-00001260: 1e00 0000 721e 0000 0072 1f00 0000 7214  ....r....r....r.
-00001270: 0000 0093 0000 0073 1200 0000 0a00 0401  .......s........
-00001280: 0c0c 0801 0801 1a01 0c01 0c01 0c02 7214  ..............r.
-00001290: 0000 004e 291a da07 7061 7468 6c69 6272  ...N)...pathlibr
-000012a0: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
-000012b0: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
-000012c0: 7207 0000 00da 0870 7964 616e 7469 6372  r......pydanticr
-000012d0: 0800 0000 7209 0000 00da 0873 716c 6d6f  ....r......sqlmo
-000012e0: 6465 6c72 0a00 0000 720b 0000 00da 0b5f  delr....r......_
-000012f0: 7661 6c69 6461 746f 7273 720d 0000 00da  validatorsr.....
-00001300: 075f 5f61 6c6c 5f5f 7215 0000 0072 0f00  .__all__r....r..
-00001310: 0000 7211 0000 0072 1200 0000 7210 0000  ..r....r....r...
-00001320: 0072 0e00 0000 7233 0000 0072 1300 0000  .r....r3...r....
-00001330: 7214 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-00001340: 1e00 0000 721f 0000 00da 083c 6d6f 6475  ....r......<modu
-00001350: 6c65 3e01 0000 0073 2a00 0000 0c00 0c01  le>....s*.......
-00001360: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
-00001370: 0c02 0402 100b 101c 1015 1005 1004 1009  ................
-00001380: 1013 1004 141f                           ......
+00000df0: 0264 027c 029b 009d 0283 0182 017c 0153  .d.|.........|.S
+00000e00: 0029 034e fa01 2f7a 1f50 6163 6b61 6765  .).N../z.Package
+00000e10: 2070 6174 6820 6d75 7374 2062 6520 6162   path must be ab
+00000e20: 736f 6c75 7465 3a20 2903 7202 0000 00da  solute: ).r.....
+00000e30: 0b69 735f 6162 736f 6c75 7465 da0a 5661  .is_absolute..Va
+00000e40: 6c75 6545 7272 6f72 2903 da03 636c 73da  lueError)...cls.
+00000e50: 0576 616c 7565 da0c 7061 636b 6167 655f  .value..package_
+00000e60: 7061 7468 721e 0000 0072 1e00 0000 721f  pathr....r....r.
+00000e70: 0000 00da 1570 6163 6b61 6765 5f70 6174  .....package_pat
+00000e80: 685f 6162 736f 6c75 7465 8400 0000 730e  h_absolute....s.
+00000e90: 0000 0008 0208 0108 0102 0108 0104 ff04  ................
+00000ea0: 037a 2454 6173 6b43 6f6c 6c65 6374 5069  .z$TaskCollectPi
+00000eb0: 702e 7061 636b 6167 655f 7061 7468 5f61  p.package_path_a
+00000ec0: 6273 6f6c 7574 6529 0a72 1800 0000 7219  bsolute).r....r.
+00000ed0: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000ee0: 0000 721d 0000 0072 0700 0000 7236 0000  ..r....r....r6..
+00000ef0: 0072 0900 0000 723e 0000 0072 1e00 0000  .r....r>...r....
+00000f00: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000f10: 1300 0000 7400 0000 7310 0000 000a 0004  ....t...s.......
+00000f20: 0108 0a0c 0110 010c 0106 020e 0172 1300  .............r..
+00000f30: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000f40: 0000 0003 0000 0040 0000 0073 6800 0000  .......@...sh...
+00000f50: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
+00000f60: 6402 1900 6505 6403 3c00 6506 6505 6404  d...e.d.<.e.e.d.
+00000f70: 3c00 6507 6505 6405 3c00 6508 6700 6406  <.e.e.d.<.e.g.d.
+00000f80: 8d01 5a09 650a 650b 650c 1900 1900 6505  ..Z.e.e.e.....e.
+00000f90: 6407 3c00 650a 6506 1900 6505 6408 3c00  d.<.e.e...e.d.<.
+00000fa0: 650a 6506 1900 6505 6409 3c00 640a 640b  e.e...e.d.<.d.d.
+00000fb0: 8400 5a0d 640c 5300 290d 7214 0000 007a  ..Z.d.S.).r....z
+00000fc0: ac0a 2020 2020 5461 736b 436f 6c6c 6563  ..    TaskCollec
+00000fd0: 7453 7461 7475 7320 636c 6173 730a 0a20  tStatus class.. 
+00000fe0: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
+00000ff0: 2020 2020 2020 2073 7461 7475 733a 2054         status: T
+00001000: 4244 0a20 2020 2020 2020 2070 6163 6b61  BD.        packa
+00001010: 6765 3a20 5442 440a 2020 2020 2020 2020  ge: TBD.        
+00001020: 7665 6e76 5f70 6174 683a 2054 4244 0a20  venv_path: TBD. 
+00001030: 2020 2020 2020 2074 6173 6b5f 6c69 7374         task_list
+00001040: 3a20 5442 440a 2020 2020 2020 2020 6c6f  : TBD.        lo
+00001050: 673a 2054 4244 0a20 2020 2020 2020 2069  g: TBD.        i
+00001060: 6e66 6f3a 2054 4244 0a20 2020 2029 05da  nfo: TBD.    )..
+00001070: 0770 656e 6469 6e67 da0a 696e 7374 616c  .pending..instal
+00001080: 6c69 6e67 da0a 636f 6c6c 6563 7469 6e67  ling..collecting
+00001090: da04 6661 696c da02 4f4b da06 7374 6174  ..fail..OK..stat
+000010a0: 7573 7234 0000 00da 0976 656e 765f 7061  usr4.....venv_pa
+000010b0: 7468 7230 0000 00da 0974 6173 6b5f 6c69  thr0.....task_li
+000010c0: 7374 da03 6c6f 67da 0469 6e66 6f63 0100  st..log..infoc..
+000010d0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000010e0: 0000 4300 0000 731a 0000 007c 00a0 00a1  ..C...s....|....
+000010f0: 007d 0174 017c 006a 0283 017c 0164 013c  .}.t.|.j...|.d.<
+00001100: 007c 0153 0029 027a 510a 2020 2020 2020  .|.S.).zQ.      
+00001110: 2020 5265 7475 726e 2060 7365 6c66 2e64    Return `self.d
+00001120: 6963 7428 2960 2061 6674 6572 2063 6173  ict()` after cas
+00001130: 7469 6e67 2060 7365 6c66 2e76 656e 765f  ting `self.venv_
+00001140: 7061 7468 6020 746f 2061 2073 7472 696e  path` to a strin
+00001150: 670a 2020 2020 2020 2020 7245 0000 0029  g.        rE...)
+00001160: 03da 0464 6963 7472 1c00 0000 7245 0000  ...dictr....rE..
+00001170: 0029 02da 0473 656c 66da 0164 721e 0000  .)...self..dr...
+00001180: 0072 1e00 0000 721f 0000 00da 0e73 616e  .r....r......san
+00001190: 6974 6973 6564 5f64 6963 74a3 0000 0073  itised_dict....s
+000011a0: 0600 0000 0804 0e01 0401 7a20 5461 736b  ..........z Task
+000011b0: 436f 6c6c 6563 7453 7461 7475 732e 7361  CollectStatus.sa
+000011c0: 6e69 7469 7365 645f 6469 6374 4e29 0e72  nitised_dictN).r
+000011d0: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
+000011e0: 0000 0072 0600 0000 721d 0000 0072 1c00  ...r....r....r..
+000011f0: 0000 7202 0000 0072 0a00 0000 7246 0000  ..r....r....rF..
+00001200: 0072 0700 0000 7205 0000 0072 1000 0000  .r....r....r....
+00001210: 724c 0000 0072 1e00 0000 721e 0000 0072  rL...r....r....r
+00001220: 1e00 0000 721f 0000 0072 1400 0000 8f00  ....r....r......
+00001230: 0000 7312 0000 000a 0004 010c 0c08 0108  ..s.............
+00001240: 011a 010c 010c 010c 0272 1400 0000 4e29  .........r....N)
+00001250: 1ada 0770 6174 686c 6962 7202 0000 00da  ...pathlibr.....
+00001260: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
+00001270: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
+00001280: da08 7079 6461 6e74 6963 7208 0000 0072  ..pydanticr....r
+00001290: 0900 0000 da08 7371 6c6d 6f64 656c 720a  ......sqlmodelr.
+000012a0: 0000 0072 0b00 0000 da0b 5f76 616c 6964  ...r......_valid
+000012b0: 6174 6f72 7372 0d00 0000 da07 5f5f 616c  atorsr......__al
+000012c0: 6c5f 5f72 1500 0000 720f 0000 0072 1100  l__r....r....r..
+000012d0: 0000 7212 0000 0072 1000 0000 720e 0000  ..r....r....r...
+000012e0: 0072 3300 0000 7213 0000 0072 1400 0000  .r3...r....r....
+000012f0: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
+00001300: 1f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00001310: 0000 732a 0000 000c 000c 010c 010c 010c  ..s*............
+00001320: 010c 010c 020c 010c 010c 010c 0204 0210  ................
+00001330: 0b10 1c10 1510 0510 0410 0910 1310 0414  ................
+00001340: 1b                                       .
```

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/task.cpython-39.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/task.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/user.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 13:52:21 2023 UTC, .py size: 546 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 15f0 0564 2202 0000  o..........d"...
+00000000: 610d 0d0a 0000 0000 15f0 0564 2202 0000  a..........d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6407 5a09 4700 6408 6409  m.Z...d.Z.G.d.d.
 00000070: 8400 6409 6504 6a0a 6500 6a0b 1900 8303  ..d.e.j.e.j.....
@@ -12,52 +12,53 @@
 000000b0: 004e 2901 da08 4f70 7469 6f6e 616c 2901  .N)...Optional).
 000000c0: da07 7363 6865 6d61 7329 01da 0976 616c  ..schemas)...val
 000000d0: 6964 6174 6f72 e901 0000 0029 01da 0676  idator.....)...v
 000000e0: 616c 7374 7229 03da 0855 7365 7252 6561  alstr)...UserRea
 000000f0: 64da 0a55 7365 7255 7064 6174 65da 0a55  d..UserUpdate..U
 00000100: 7365 7243 7265 6174 6563 0000 0000 0000  serCreatec......
 00000110: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000120: 0000 f31a 0000 0065 005a 0164 005a 0255  .......e.Z.d.Z.U
+00000120: 0000 731a 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
 00000130: 0065 0365 0419 0065 0564 013c 0064 0253  .e.e...e.d.<.d.S
 00000140: 0029 0372 0700 0000 da0a 736c 7572 6d5f  .).r......slurm_
 00000150: 7573 6572 4ea9 06da 085f 5f6e 616d 655f  userN....__name_
 00000160: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000170: 5f71 7561 6c6e 616d 655f 5f72 0200 0000  _qualname__r....
 00000180: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
-00000190: 696f 6e73 5f5f a900 7212 0000 0072 1200  ions__..r....r..
+00000190: 696f 6e73 5f5f a900 7211 0000 0072 1100  ions__..r....r..
 000001a0: 0000 fa3c 2f68 6f6d 652f 746f 6d6d 6173  ...</home/tommas
 000001b0: 6f2f 4672 6163 7461 6c2f 6672 6163 7461  o/Fractal/fracta
 000001c0: 6c2f 6672 6163 7461 6c2f 636f 6d6d 6f6e  l/fractal/common
 000001d0: 2f73 6368 656d 6173 2f75 7365 722e 7079  /schemas/user.py
-000001e0: 7207 0000 0011 0000 00f3 0400 0000 0a00  r...............
-000001f0: 1001 7207 0000 0063 0000 0000 0000 0000  ..r....c........
-00000200: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000210: 720a 0000 0029 0372 0800 0000 720b 0000  r....).r....r...
-00000220: 004e 720c 0000 0072 1200 0000 7212 0000  .Nr....r....r...
-00000230: 0072 1200 0000 7213 0000 0072 0800 0000  .r....r....r....
-00000240: 1500 0000 7214 0000 0072 0800 0000 6300  ....r....r....c.
-00000250: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000260: 0000 0040 0000 0073 2e00 0000 6500 5a01  ...@...s....e.Z.
-00000270: 6400 5a02 5500 6503 6504 1900 6505 6401  d.Z.U.e.e...e.d.
-00000280: 3c00 6506 6401 6402 6403 8d02 6507 6401  <.e.d.d.d...e.d.
-00000290: 8301 8301 5a08 6404 5300 2905 7209 0000  ....Z.d.S.).r...
-000002a0: 0072 0b00 0000 5429 01da 0b61 6c6c 6f77  .r....T)...allow
-000002b0: 5f72 6575 7365 4e29 0972 0d00 0000 720e  _reuseN).r....r.
-000002c0: 0000 0072 0f00 0000 7202 0000 0072 1000  ...r....r....r..
-000002d0: 0000 7211 0000 0072 0400 0000 7206 0000  ..r....r....r...
-000002e0: 00da 0b5f 736c 7572 6d5f 7573 6572 7212  ..._slurm_userr.
-000002f0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00000300: 0000 7209 0000 0019 0000 0073 0a00 0000  ..r........s....
-00000310: 0a00 0c01 0a03 0601 08ff 7209 0000 0029  ..........r....)
-00000320: 11da 0475 7569 64da 0674 7970 696e 6772  ...uuid..typingr
-00000330: 0200 0000 da0d 6661 7374 6170 695f 7573  ......fastapi_us
-00000340: 6572 7372 0300 0000 da08 7079 6461 6e74  ersr......pydant
-00000350: 6963 7204 0000 00da 0b5f 7661 6c69 6461  icr......_valida
-00000360: 746f 7273 7206 0000 00da 075f 5f61 6c6c  torsr......__all
-00000370: 5f5f da08 4261 7365 5573 6572 da04 5555  __..BaseUser..UU
-00000380: 4944 7207 0000 00da 0e42 6173 6555 7365  IDr......BaseUse
-00000390: 7255 7064 6174 6572 0800 0000 da0e 4261  rUpdater......Ba
-000003a0: 7365 5573 6572 4372 6561 7465 7209 0000  seUserCreater...
-000003b0: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-000003c0: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000003d0: 0000 0073 1200 0000 0800 0c01 0c02 0c01  ...s............
-000003e0: 0c02 0403 1807 1204 1604                 ..........
+000001e0: 7207 0000 0011 0000 0073 0200 0000 0a01  r........s......
+000001f0: 7207 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000200: 0000 0000 0000 0300 0000 4000 0000 731a  ..........@...s.
+00000210: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
+00000220: 0419 0065 0564 013c 0064 0253 0029 0372  ...e.d.<.d.S.).r
+00000230: 0800 0000 720a 0000 004e 720b 0000 0072  ....r....Nr....r
+00000240: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00000250: 0000 0072 0800 0000 1500 0000 7302 0000  ...r........s...
+00000260: 000a 0172 0800 0000 6300 0000 0000 0000  ...r....c.......
+00000270: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000280: 0073 2e00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000290: 6503 6504 1900 6505 6401 3c00 6506 6401  e.e...e.d.<.e.d.
+000002a0: 6402 6403 8d02 6507 6401 8301 8301 5a08  d.d...e.d.....Z.
+000002b0: 6404 5300 2905 7209 0000 0072 0a00 0000  d.S.).r....r....
+000002c0: 5429 01da 0b61 6c6c 6f77 5f72 6575 7365  T)...allow_reuse
+000002d0: 4e29 0972 0c00 0000 720d 0000 0072 0e00  N).r....r....r..
+000002e0: 0000 7202 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000002f0: 0072 0400 0000 7206 0000 005a 0b5f 736c  .r....r....Z._sl
+00000300: 7572 6d5f 7573 6572 7211 0000 0072 1100  urm_userr....r..
+00000310: 0000 7211 0000 0072 1200 0000 7209 0000  ..r....r....r...
+00000320: 0019 0000 0073 0800 0000 0a01 0c03 0a01  .....s..........
+00000330: 06ff 7209 0000 0029 11da 0475 7569 64da  ..r....)...uuid.
+00000340: 0674 7970 696e 6772 0200 0000 5a0d 6661  .typingr....Z.fa
+00000350: 7374 6170 695f 7573 6572 7372 0300 0000  stapi_usersr....
+00000360: da08 7079 6461 6e74 6963 7204 0000 00da  ..pydanticr.....
+00000370: 0b5f 7661 6c69 6461 746f 7273 7206 0000  ._validatorsr...
+00000380: 00da 075f 5f61 6c6c 5f5f 5a08 4261 7365  ...__all__Z.Base
+00000390: 5573 6572 da04 5555 4944 7207 0000 005a  User..UUIDr....Z
+000003a0: 0e42 6173 6555 7365 7255 7064 6174 6572  .BaseUserUpdater
+000003b0: 0800 0000 5a0e 4261 7365 5573 6572 4372  ....Z.BaseUserCr
+000003c0: 6561 7465 7209 0000 0072 1100 0000 7211  eater....r....r.
+000003d0: 0000 0072 1100 0000 7212 0000 00da 083c  ...r....r......<
+000003e0: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
+000003f0: 0801 0c02 0c01 0c02 0c03 0407 1804 1204  ................
```

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/_validators.py` & `fractal_client-1.3.0a0/fractal/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/manifest.py` & `fractal_client-1.3.0a0/fractal/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/project.py` & `fractal_client-1.3.0a0/fractal/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/state.py` & `fractal_client-1.3.0a0/fractal/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/task.py` & `fractal_client-1.3.0a0/fractal/common/schemas/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -133,18 +133,14 @@
     def package_path_absolute(cls, value):
         if "/" in value:
             package_path = Path(value)
             if not package_path.is_absolute():
                 raise ValueError(
                     f"Package path must be absolute: {package_path}"
                 )
-            if not package_path.exists():
-                raise ValueError(
-                    f"Package file does not exist: {package_path}"
-                )
         return value
 
 
 class TaskCollectStatus(_TaskCollectBase):
     """
     TaskCollectStatus class
```

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/user.py` & `fractal_client-1.3.0a0/fractal/common/schemas/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import uuid
 from typing import Optional
 
 from fastapi_users import schemas
 from pydantic import validator
 
 from ._validators import val_absolute_path
 from ._validators import valstr
@@ -11,15 +10,15 @@
 __all__ = (
     "UserRead",
     "UserUpdate",
     "UserCreate",
 )
 
 
-class UserRead(schemas.BaseUser[uuid.UUID]):
+class UserRead(schemas.BaseUser[int]):
     slurm_user: Optional[str]
     cache_dir: Optional[str]
 
 
 class UserUpdate(schemas.BaseUserUpdate):
     slurm_user: Optional[str]
     cache_dir: Optional[str]
```

### Comparing `fractal_client-1.2.0a0/fractal/common/schemas/workflow.py` & `fractal_client-1.3.0a0/fractal/common/schemas/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,16 @@
 
     meta: Optional[Dict[str, Any]] = None
     args: Optional[Dict[str, Any]] = None
 
 
 class WorkflowTaskCreate(_WorkflowTaskBase):
     order: Optional[int]
-    task_id: int
     # Validators
     _order = validator("order", allow_reuse=True)(valint("order", min_val=0))
-    _task_id = validator("task_id", allow_reuse=True)(valint("task_id"))
 
 
 class WorkflowTaskRead(_WorkflowTaskBase):
     id: int
     order: Optional[int]
     workflow_id: int
     task_id: int
@@ -75,21 +73,16 @@
 class WorkflowRead(_WorkflowBase):
     id: int
     project_id: int
     task_list: List[WorkflowTaskRead]
 
 
 class WorkflowCreate(_WorkflowBase):
-    project_id: int
-
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
-    _project_id = validator("project_id", allow_reuse=True)(
-        valint("project_id")
-    )
 
 
 class WorkflowUpdate(_WorkflowBase):
     name: Optional[str]
     reordered_workflowtask_ids: Optional[List[int]]
 
     # Validators
```

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 14 13:42:31 2023 UTC, .py size: 704 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,73 @@
-00000000: 6f0d 0d0a 0000 0000 c779 1064 c002 0000  o........y.d....
+00000000: 6f0d 0d0a 0000 0000 5fad 2e64 0d02 0000  o......._..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
 00000080: 2907 e900 0000 004e 2901 da05 6465 6275  )......N)...debu
 00000090: 6729 01da 0f56 616c 6964 6174 696f 6e45  g)...ValidationE
 000000a0: 7272 6f72 2901 da0d 5072 6f6a 6563 7443  rror)...ProjectC
 000000b0: 7265 6174 6563 0000 0000 0000 0000 0000  reatec..........
-000000c0: 0000 0600 0000 0800 0000 4300 0000 7342  ..........C...sB
-000000d0: 0100 0074 0064 0164 0264 038d 027d 0074  ...t.d.d.d...}.t
-000000e0: 017c 0083 0101 0064 047d 0174 0064 057c  .|.....d.}.t.d.|
-000000f0: 019b 0064 059d 0364 0264 038d 027d 0074  ...d...d.d...}.t
-00000100: 017c 0083 0101 007c 006a 027d 027c 027c  .|.....|.j.}.|.|
-00000110: 016b 027d 037c 0373 6474 03a0 0464 067c  .k.}.|.sdt...d.|
-00000120: 0366 0164 077c 027c 0166 02a1 0464 0874  .f.d.|.|.f...d.t
-00000130: 05a0 06a1 0076 0073 3874 03a0 077c 00a1  .....v.s8t...|..
-00000140: 0172 3d74 03a0 087c 00a1 016e 0164 0874  .r=t...|...n.d.t
-00000150: 03a0 087c 02a1 0164 0974 05a0 06a1 0076  ...|...d.t.....v
-00000160: 0073 4d74 03a0 077c 01a1 0172 5274 03a0  .sMt...|...rRt..
-00000170: 087c 01a1 016e 0164 0964 0a9c 0316 007d  .|...n.d.d.....}
-00000180: 0464 0b64 0c7c 0469 0116 007d 0574 0974  .d.d.|.i...}.t.t
-00000190: 03a0 0a7c 05a1 0183 0182 0164 0004 007d  ...|.......d...}
-000001a0: 027d 0374 0ba0 0c74 0da1 018f 0e01 0074  .}.t...t.......t
-000001b0: 0064 0564 0264 038d 0201 0057 0064 0004  .d.d.d.....W.d..
-000001c0: 0004 0083 0301 006e 0831 0073 7e77 0101  .......n.1.s~w..
-000001d0: 0001 0001 0059 0001 0074 0ba0 0c74 0da1  .....Y...t...t..
-000001e0: 018f 0f01 0074 0064 0164 0d64 038d 0201  .....t.d.d.d....
-000001f0: 0057 0064 0004 0004 0083 0301 0064 0053  .W.d.........d.S
-00000200: 0031 0073 9a77 0101 0001 0001 0059 0001  .1.s.w.......Y..
-00000210: 0064 0053 0029 0e4e 7a0a 6d79 2070 726f  .d.S.).Nz.my pro
-00000220: 6a65 6374 7a0a 2f73 6f6d 6577 6865 7265  jectz./somewhere
-00000230: 2902 da04 6e61 6d65 da0b 7072 6f6a 6563  )...name..projec
-00000240: 745f 6469 727a 1173 6f6d 6520 7072 6f6a  t_dirz.some proj
-00000250: 6563 7420 6e61 6d65 7a02 2020 2901 fa02  ect namez.  )...
-00000260: 3d3d 2901 7a2c 2528 7079 3229 730a 7b25  ==).z,%(py2)s.{%
-00000270: 2870 7932 2973 203d 2025 2870 7930 2973  (py2)s = %(py0)s
-00000280: 2e6e 616d 650a 7d20 3d3d 2025 2870 7934  .name.} == %(py4
-00000290: 2973 da01 70da 044e 414d 4529 03da 0370  )s..p..NAME)...p
-000002a0: 7930 da03 7079 32da 0370 7934 7a0e 6173  y0..py2..py4z.as
-000002b0: 7365 7274 2025 2870 7936 2973 da03 7079  sert %(py6)s..py
-000002c0: 36da 0120 290e 7204 0000 0072 0200 0000  6.. ).r....r....
-000002d0: 7205 0000 00da 0a40 7079 7465 7374 5f61  r......@pytest_a
-000002e0: 72da 115f 6361 6c6c 5f72 6570 7263 6f6d  r.._call_reprcom
-000002f0: 7061 7265 da0c 4070 795f 6275 696c 7469  pare..@py_builti
-00000300: 6e73 da06 6c6f 6361 6c73 da18 5f73 686f  ns..locals.._sho
-00000310: 756c 645f 7265 7072 5f67 6c6f 6261 6c5f  uld_repr_global_
-00000320: 6e61 6d65 da09 5f73 6166 6572 6570 72da  name.._saferepr.
-00000330: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
-00000340: 135f 666f 726d 6174 5f65 7870 6c61 6e61  ._format_explana
-00000350: 7469 6f6e da06 7079 7465 7374 da06 7261  tion..pytest..ra
-00000360: 6973 6573 7203 0000 0029 0672 0800 0000  isesr....).r....
-00000370: 7209 0000 00da 0b40 7079 5f61 7373 6572  r......@py_asser
-00000380: 7431 da0b 4070 795f 6173 7365 7274 33da  t1..@py_assert3.
-00000390: 0b40 7079 5f66 6f72 6d61 7435 da0b 4070  .@py_format5..@p
-000003a0: 795f 666f 726d 6174 37a9 0072 1d00 0000  y_format7..r....
-000003b0: fa42 2f68 6f6d 652f 746f 6d6d 6173 6f2f  .B/home/tommaso/
-000003c0: 4672 6163 7461 6c2f 6672 6163 7461 6c2f  Fractal/fractal/
-000003d0: 6672 6163 7461 6c2f 636f 6d6d 6f6e 2f74  fractal/common/t
-000003e0: 6573 7473 2f74 6573 745f 7072 6f6a 6563  ests/test_projec
-000003f0: 742e 7079 da13 7465 7374 5f70 726f 6a65  t.py..test_proje
-00000400: 6374 5f63 7265 6174 6508 0000 0073 1800  ct_create....s..
-00000410: 0000 0c02 0801 0402 1401 0801 9c01 0c02  ................
-00000420: 0e01 1cff 0c03 0e01 22ff 721f 0000 0029  ........".r....)
-00000430: 0eda 0862 7569 6c74 696e 7372 1100 0000  ...builtinsr....
-00000440: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
-00000450: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
-00000460: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
-00000470: 0f00 0000 7217 0000 00da 0864 6576 746f  ....r......devto
-00000480: 6f6c 7372 0200 0000 da17 7079 6461 6e74  olsr......pydant
-00000490: 6963 2e65 7272 6f72 5f77 7261 7070 6572  ic.error_wrapper
-000004a0: 7372 0300 0000 da07 7363 6865 6d61 7372  sr......schemasr
-000004b0: 0400 0000 721f 0000 0072 1d00 0000 721d  ....r....r....r.
-000004c0: 0000 0072 1d00 0000 721e 0000 00da 083c  ...r....r......<
-000004d0: 6d6f 6475 6c65 3e01 0000 0073 0a00 0000  module>....s....
-000004e0: 2200 0c01 0c01 0c02 0c03                 ".........
+000000c0: 0000 0600 0000 0800 0000 4300 0000 7306  ..........C...s.
+000000d0: 0100 0074 0064 0164 028d 017d 0074 017c  ...t.d.d...}.t.|
+000000e0: 0083 0101 0064 037d 0174 0064 047c 019b  .....d.}.t.d.|..
+000000f0: 0064 049d 0364 028d 017d 0074 017c 0083  .d...d...}.t.|..
+00000100: 0101 007c 006a 027d 027c 027c 016b 027d  ...|.j.}.|.|.k.}
+00000110: 037c 0373 6274 03a0 0464 057c 0366 0164  .|.sbt...d.|.f.d
+00000120: 067c 027c 0166 02a1 0464 0774 05a0 06a1  .|.|.f...d.t....
+00000130: 0076 0073 3674 03a0 077c 00a1 0172 3b74  .v.s6t...|...r;t
+00000140: 03a0 087c 00a1 016e 0164 0774 03a0 087c  ...|...n.d.t...|
+00000150: 02a1 0164 0874 05a0 06a1 0076 0073 4b74  ...d.t.....v.sKt
+00000160: 03a0 077c 01a1 0172 5074 03a0 087c 01a1  ...|...rPt...|..
+00000170: 016e 0164 0864 099c 0316 007d 0464 0a64  .n.d.d.....}.d.d
+00000180: 0b7c 0469 0116 007d 0574 0974 03a0 0a7c  .|.i...}.t.t...|
+00000190: 05a1 0183 0182 0164 0004 007d 027d 0374  .......d...}.}.t
+000001a0: 0ba0 0c74 0da1 018f 0e01 0074 0064 0464  ...t.......t.d.d
+000001b0: 028d 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+000001c0: 0064 0053 0031 0073 7c77 0101 0001 0001  .d.S.1.s|w......
+000001d0: 0059 0001 0064 0053 0029 0c4e 7a0a 6d79  .Y...d.S.).Nz.my
+000001e0: 2070 726f 6a65 6374 2901 da04 6e61 6d65   project)...name
+000001f0: 7a11 736f 6d65 2070 726f 6a65 6374 206e  z.some project n
+00000200: 616d 657a 0220 2029 01fa 023d 3d29 017a  amez.  )...==).z
+00000210: 2c25 2870 7932 2973 0a7b 2528 7079 3229  ,%(py2)s.{%(py2)
+00000220: 7320 3d20 2528 7079 3029 732e 6e61 6d65  s = %(py0)s.name
+00000230: 0a7d 203d 3d20 2528 7079 3429 73da 0170  .} == %(py4)s..p
+00000240: da04 4e41 4d45 2903 da03 7079 30da 0370  ..NAME)...py0..p
+00000250: 7932 da03 7079 347a 0e61 7373 6572 7420  y2..py4z.assert 
+00000260: 2528 7079 3629 73da 0370 7936 290e 7204  %(py6)s..py6).r.
+00000270: 0000 0072 0200 0000 7205 0000 00da 0a40  ...r....r......@
+00000280: 7079 7465 7374 5f61 72da 115f 6361 6c6c  pytest_ar.._call
+00000290: 5f72 6570 7263 6f6d 7061 7265 da0c 4070  _reprcompare..@p
+000002a0: 795f 6275 696c 7469 6e73 da06 6c6f 6361  y_builtins..loca
+000002b0: 6c73 da18 5f73 686f 756c 645f 7265 7072  ls.._should_repr
+000002c0: 5f67 6c6f 6261 6c5f 6e61 6d65 da09 5f73  _global_name.._s
+000002d0: 6166 6572 6570 72da 0e41 7373 6572 7469  aferepr..Asserti
+000002e0: 6f6e 4572 726f 72da 135f 666f 726d 6174  onError.._format
+000002f0: 5f65 7870 6c61 6e61 7469 6f6e da06 7079  _explanation..py
+00000300: 7465 7374 da06 7261 6973 6573 7203 0000  test..raisesr...
+00000310: 0029 0672 0700 0000 7208 0000 00da 0b40  .).r....r......@
+00000320: 7079 5f61 7373 6572 7431 da0b 4070 795f  py_assert1..@py_
+00000330: 6173 7365 7274 33da 0b40 7079 5f66 6f72  assert3..@py_for
+00000340: 6d61 7435 da0b 4070 795f 666f 726d 6174  mat5..@py_format
+00000350: 37a9 0072 1b00 0000 fa42 2f68 6f6d 652f  7..r.....B/home/
+00000360: 746f 6d6d 6173 6f2f 4672 6163 7461 6c2f  tommaso/Fractal/
+00000370: 6672 6163 7461 6c2f 6672 6163 7461 6c2f  fractal/fractal/
+00000380: 636f 6d6d 6f6e 2f74 6573 7473 2f74 6573  common/tests/tes
+00000390: 745f 7072 6f6a 6563 742e 7079 da13 7465  t_project.py..te
+000003a0: 7374 5f70 726f 6a65 6374 5f63 7265 6174  st_project_creat
+000003b0: 6508 0000 0073 1200 0000 0a02 0801 0402  e....s..........
+000003c0: 1201 0801 9c01 0c02 0c01 22ff 721d 0000  ..........".r...
+000003d0: 0029 0eda 0862 7569 6c74 696e 7372 0f00  .)...builtinsr..
+000003e0: 0000 da19 5f70 7974 6573 742e 6173 7365  ...._pytest.asse
+000003f0: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
+00000400: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
+00000410: 6572 0d00 0000 7215 0000 00da 0864 6576  er....r......dev
+00000420: 746f 6f6c 7372 0200 0000 da17 7079 6461  toolsr......pyda
+00000430: 6e74 6963 2e65 7272 6f72 5f77 7261 7070  ntic.error_wrapp
+00000440: 6572 7372 0300 0000 da07 7363 6865 6d61  ersr......schema
+00000450: 7372 0400 0000 721d 0000 0072 1b00 0000  sr....r....r....
+00000460: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00000470: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
+00000480: 0000 2200 0c01 0c01 0c02 0c03            ..".........
```

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 13:52:21 2023 UTC, .py size: 583 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-00000000: 6f0d 0d0a 0000 0000 15f0 0564 4702 0000  o..........dG...
+00000000: 6f0d 0d0a 0000 0000 5fad 2e64 c804 0000  o......._..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
 00000080: 2907 e900 0000 004e 2901 da05 6465 6275  )......N)...debu
 00000090: 6729 01da 0f56 616c 6964 6174 696f 6e45  g)...ValidationE
 000000a0: 7272 6f72 2901 da0a 5573 6572 4372 6561  rror)...UserCrea
-000000b0: 7465 6300 0000 0000 0000 0000 0000 0007  tec.............
-000000c0: 0000 0008 0000 0043 0000 0073 4201 0000  .......C...sB...
+000000b0: 7465 6300 0000 0000 0000 0000 0000 000d  tec.............
+000000c0: 0000 0008 0000 0043 0000 0073 6803 0000  .......C...sh...
 000000d0: 7400 6401 6402 6403 8d02 7d00 7401 7c00  t.d.d.d...}.t.|.
 000000e0: 8301 0100 7c00 6a02 7d01 6400 7d02 7c01  ....|.j.}.d.}.|.
 000000f0: 7c02 7500 7d03 7c03 7349 7403 a004 6404  |.u.}.|.sIt...d.
 00000100: 7c03 6601 6405 7c01 7c02 6602 a104 6406  |.f.d.|.|.f...d.
 00000110: 7405 a006 a100 7600 732a 7403 a007 7c00  t.....v.s*t...|.
 00000120: a101 722f 7403 a008 7c00 a101 6e01 6406  ..r/t...|...n.d.
 00000130: 7403 a008 7c01 a101 7403 a008 7c02 a101  t...|...t...|...
@@ -23,61 +23,117 @@
 00000160: 8201 6400 0400 7d01 0400 7d03 7d02 7400  ..d...}...}.}.t.
 00000170: 6401 6402 640a 640b 8d03 7d00 7401 7c00  d.d.d.d...}.t.|.
 00000180: 8301 0100 7c00 6a02 7d01 7c01 7380 640c  ....|.j.}.|.s.d.
 00000190: 6406 7405 a006 a100 7600 736b 7403 a007  d.t.....v.skt...
 000001a0: 7c00 a101 7270 7403 a008 7c00 a101 6e01  |...rpt...|...n.
 000001b0: 6406 7403 a008 7c01 a101 640d 9c02 1600  d.t...|...d.....
 000001c0: 7d06 7409 7403 a00a 7c06 a101 8301 8201  }.t.t...|.......
-000001d0: 6400 7d01 740b a00c 740d a101 8f10 0100  d.}.t...t.......
+000001d0: 6400 7d01 740b a00c 740d a101 8f0f 0100  d.}.t...t.......
 000001e0: 7400 6401 6402 640e 640b 8d03 7d00 5700  t.d.d.d.d...}.W.
-000001f0: 6400 0400 0400 8303 0100 6400 5300 3100  d.........d.S.1.
-00000200: 739a 7701 0100 0100 0100 5900 0100 6400  s.w.......Y...d.
-00000210: 5300 290f 4e7a 0561 4062 2e63 da03 6173  S.).Nz.a@b.c..as
-00000220: 6429 02da 0565 6d61 696c da08 7061 7373  d)...email..pass
-00000230: 776f 7264 2901 da02 6973 2901 7a32 2528  word)...is).z2%(
-00000240: 7079 3229 730a 7b25 2870 7932 2973 203d  py2)s.{%(py2)s =
-00000250: 2025 2870 7930 2973 2e73 6c75 726d 5f75   %(py0)s.slurm_u
-00000260: 7365 720a 7d20 6973 2025 2870 7935 2973  ser.} is %(py5)s
-00000270: da01 7529 03da 0370 7930 da03 7079 32da  ..u)...py0..py2.
-00000280: 0370 7935 7a0e 6173 7365 7274 2025 2870  .py5z.assert %(p
-00000290: 7937 2973 da03 7079 37da 0a73 6c75 726d  y7)s..py7..slurm
-000002a0: 5f75 7365 7229 0372 0600 0000 7207 0000  _user).r....r...
-000002b0: 0072 0e00 0000 7a2e 6173 7365 7274 2025  .r....z.assert %
-000002c0: 2870 7932 2973 0a7b 2528 7079 3229 7320  (py2)s.{%(py2)s 
-000002d0: 3d20 2528 7079 3029 732e 736c 7572 6d5f  = %(py0)s.slurm_
-000002e0: 7573 6572 0a7d 2902 720a 0000 0072 0b00  user.}).r....r..
-000002f0: 0000 7a02 2020 290e 7204 0000 0072 0200  ..z.  ).r....r..
-00000300: 0000 720e 0000 00da 0a40 7079 7465 7374  ..r......@pytest
-00000310: 5f61 72da 115f 6361 6c6c 5f72 6570 7263  _ar.._call_reprc
-00000320: 6f6d 7061 7265 da0c 4070 795f 6275 696c  ompare..@py_buil
-00000330: 7469 6e73 da06 6c6f 6361 6c73 da18 5f73  tins..locals.._s
-00000340: 686f 756c 645f 7265 7072 5f67 6c6f 6261  hould_repr_globa
-00000350: 6c5f 6e61 6d65 da09 5f73 6166 6572 6570  l_name.._saferep
-00000360: 72da 0e41 7373 6572 7469 6f6e 4572 726f  r..AssertionErro
-00000370: 72da 135f 666f 726d 6174 5f65 7870 6c61  r.._format_expla
-00000380: 6e61 7469 6f6e da06 7079 7465 7374 da06  nation..pytest..
-00000390: 7261 6973 6573 7203 0000 0029 0772 0900  raisesr....).r..
-000003a0: 0000 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
-000003b0: 0b40 7079 5f61 7373 6572 7434 da0b 4070  .@py_assert4..@p
-000003c0: 795f 6173 7365 7274 33da 0b40 7079 5f66  y_assert3..@py_f
-000003d0: 6f72 6d61 7436 da0b 4070 795f 666f 726d  ormat6..@py_form
-000003e0: 6174 38da 0b40 7079 5f66 6f72 6d61 7433  at8..@py_format3
-000003f0: a900 721f 0000 00fa 3f2f 686f 6d65 2f74  ..r.....?/home/t
-00000400: 6f6d 6d61 736f 2f46 7261 6374 616c 2f66  ommaso/Fractal/f
-00000410: 7261 6374 616c 2f66 7261 6374 616c 2f63  ractal/fractal/c
-00000420: 6f6d 6d6f 6e2f 7465 7374 732f 7465 7374  ommon/tests/test
-00000430: 5f75 7365 722e 7079 da10 7465 7374 5f75  _user.py..test_u
-00000440: 7365 725f 6372 6561 7465 0800 0000 7312  ser_create....s.
-00000450: 0000 000c 0208 018a 010e 0208 0150 010c  .............P..
-00000460: 0210 0122 ff72 2100 0000 290e da08 6275  ...".r!...)...bu
-00000470: 696c 7469 6e73 7211 0000 00da 195f 7079  iltinsr......_py
-00000480: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
-00000490: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
-000004a0: 6eda 0772 6577 7269 7465 720f 0000 0072  n..rewriter....r
-000004b0: 1700 0000 da08 6465 7674 6f6f 6c73 7202  ......devtoolsr.
-000004c0: 0000 00da 1770 7964 616e 7469 632e 6572  .....pydantic.er
-000004d0: 726f 725f 7772 6170 7065 7273 7203 0000  ror_wrappersr...
-000004e0: 00da 0773 6368 656d 6173 7204 0000 0072  ...schemasr....r
-000004f0: 2100 0000 721f 0000 0072 1f00 0000 721f  !...r....r....r.
-00000500: 0000 0072 2000 0000 da08 3c6d 6f64 756c  ...r .....<modul
-00000510: 653e 0100 0000 730a 0000 0022 000c 010c  e>....s...."....
-00000520: 010c 020c 03                             .....
+000001f0: 6400 0400 0400 8303 0100 6e08 3100 7399  d.........n.1.s.
+00000200: 7701 0100 0100 0100 5900 0100 640f 7d07  w.......Y...d.}.
+00000210: 7400 6401 6402 7c07 9b00 6410 9d02 6411  t.d.d.|...d...d.
+00000220: 8d03 7d00 7c00 6a0e 7d01 7c01 7c07 6b02  ..}.|.j.}.|.|.k.
+00000230: 7d03 7c03 73f4 7403 a004 6412 7c03 6601  }.|.s.t...d.|.f.
+00000240: 6413 7c01 7c07 6602 a104 6406 7405 a006  d.|.|.f...d.t...
+00000250: a100 7600 73c8 7403 a007 7c00 a101 72cd  ..v.s.t...|...r.
+00000260: 7403 a008 7c00 a101 6e01 6406 7403 a008  t...|...n.d.t...
+00000270: 7c01 a101 6414 7405 a006 a100 7600 73dd  |...d.t.....v.s.
+00000280: 7403 a007 7c07 a101 72e2 7403 a008 7c07  t...|...r.t...|.
+00000290: a101 6e01 6414 6415 9c03 1600 7d08 6416  ..n.d.d.....}.d.
+000002a0: 6417 7c08 6901 1600 7d09 7409 7403 a00a  d.|.i...}.t.t...
+000002b0: 7c09 a101 8301 8201 6400 0400 7d01 7d03  |.......d...}.}.
+000002c0: 740b a00c 740d a101 8f0f 7d0a 7400 6401  t...t.....}.t.d.
+000002d0: 6402 640e 6411 8d03 7d00 5700 6400 0400  d.d.d...}.W.d...
+000002e0: 0400 8303 0100 6e09 3100 9001 7310 7701  ......n.1...s.w.
+000002f0: 0100 0100 0100 5900 0100 7401 7c0a 6a0f  ......Y...t.|.j.
+00000300: 8301 0100 6418 7d0b 7c0a 6a0f a010 a100  ....d.}.|.j.....
+00000310: 6419 1900 641a 1900 7d03 7c0b 7c03 7600  d...d...}.|.|.v.
+00000320: 7d0c 7c0c 9001 734f 7403 a004 641b 7c0c  }.|...sOt...d.|.
+00000330: 6601 641c 7c0b 7c03 6602 a104 7403 a008  f.d.|.|.f...t...
+00000340: 7c0b a101 7403 a008 7c03 a101 641d 9c02  |...t...|...d...
+00000350: 1600 7d08 6416 6417 7c08 6901 1600 7d09  ..}.d.d.|.i...}.
+00000360: 7409 7403 a00a 7c09 a101 8301 8201 6400  t.t...|.......d.
+00000370: 0400 7d0b 0400 7d0c 7d03 740b a00c 740d  ..}...}.}.t...t.
+00000380: a101 8f0f 7d0a 7400 6401 6402 641e 6411  ....}.t.d.d.d.d.
+00000390: 8d03 7d00 5700 6400 0400 0400 8303 0100  ..}.W.d.........
+000003a0: 6e09 3100 9001 736d 7701 0100 0100 0100  n.1...smw.......
+000003b0: 5900 0100 7401 7c0a 6a0f 8301 0100 641f  Y...t.|.j.....d.
+000003c0: 7d0b 7c0a 6a0f a010 a100 6419 1900 641a  }.|.j.....d...d.
+000003d0: 1900 7d03 7c0b 7c03 7600 7d0c 7c0c 9001  ..}.|.|.v.}.|...
+000003e0: 73ac 7403 a004 641b 7c0c 6601 641c 7c0b  s.t...d.|.f.d.|.
+000003f0: 7c03 6602 a104 7403 a008 7c0b a101 7403  |.f...t...|...t.
+00000400: a008 7c03 a101 641d 9c02 1600 7d08 6416  ..|...d.....}.d.
+00000410: 6417 7c08 6901 1600 7d09 7409 7403 a00a  d.|.i...}.t.t...
+00000420: 7c09 a101 8301 8201 6400 0400 7d0b 0400  |.......d...}...
+00000430: 7d0c 7d03 6400 5300 2920 4e7a 0561 4062  }.}.d.S.) Nz.a@b
+00000440: 2e63 da03 6173 6429 02da 0565 6d61 696c  .c..asd)...email
+00000450: da08 7061 7373 776f 7264 2901 da02 6973  ..password)...is
+00000460: 2901 7a32 2528 7079 3229 730a 7b25 2870  ).z2%(py2)s.{%(p
+00000470: 7932 2973 203d 2025 2870 7930 2973 2e73  y2)s = %(py0)s.s
+00000480: 6c75 726d 5f75 7365 720a 7d20 6973 2025  lurm_user.} is %
+00000490: 2870 7935 2973 da01 7529 03da 0370 7930  (py5)s..u)...py0
+000004a0: da03 7079 32da 0370 7935 7a0e 6173 7365  ..py2..py5z.asse
+000004b0: 7274 2025 2870 7937 2973 da03 7079 37da  rt %(py7)s..py7.
+000004c0: 0a73 6c75 726d 5f75 7365 7229 0372 0600  .slurm_user).r..
+000004d0: 0000 7207 0000 0072 0e00 0000 7a2e 6173  ..r....r....z.as
+000004e0: 7365 7274 2025 2870 7932 2973 0a7b 2528  sert %(py2)s.{%(
+000004f0: 7079 3229 7320 3d20 2528 7079 3029 732e  py2)s = %(py0)s.
+00000500: 736c 7572 6d5f 7573 6572 0a7d 2902 720a  slurm_user.}).r.
+00000510: 0000 0072 0b00 0000 7a02 2020 7a04 2f78  ...r....z.  z./x
+00000520: 7878 7a03 2020 2029 0372 0600 0000 7207  xxz.   ).r....r.
+00000530: 0000 00da 0963 6163 6865 5f64 6972 2901  .....cache_dir).
+00000540: fa02 3d3d 2901 7a31 2528 7079 3229 730a  ..==).z1%(py2)s.
+00000550: 7b25 2870 7932 2973 203d 2025 2870 7930  {%(py2)s = %(py0
+00000560: 2973 2e63 6163 6865 5f64 6972 0a7d 203d  )s.cache_dir.} =
+00000570: 3d20 2528 7079 3429 73da 0943 4143 4845  = %(py4)s..CACHE
+00000580: 5f44 4952 2903 720a 0000 0072 0b00 0000  _DIR).r....r....
+00000590: da03 7079 347a 0e61 7373 6572 7420 2528  ..py4z.assert %(
+000005a0: 7079 3629 73da 0370 7936 7a0f 6361 6e6e  py6)s..py6z.cann
+000005b0: 6f74 2062 6520 656d 7074 7972 0100 0000  ot be emptyr....
+000005c0: da03 6d73 6729 01da 0269 6e29 017a 1225  ..msg)...in).z.%
+000005d0: 2870 7931 2973 2069 6e20 2528 7079 3429  (py1)s in %(py4)
+000005e0: 7329 02da 0370 7931 7212 0000 00da 0378  s)...py1r......x
+000005f0: 7878 7a18 6d75 7374 2062 6520 616e 2061  xxz.must be an a
+00000600: 6273 6f6c 7574 6520 7061 7468 2911 7204  bsolute path).r.
+00000610: 0000 0072 0200 0000 720e 0000 00da 0a40  ...r....r......@
+00000620: 7079 7465 7374 5f61 72da 115f 6361 6c6c  pytest_ar.._call
+00000630: 5f72 6570 7263 6f6d 7061 7265 da0c 4070  _reprcompare..@p
+00000640: 795f 6275 696c 7469 6e73 da06 6c6f 6361  y_builtins..loca
+00000650: 6c73 da18 5f73 686f 756c 645f 7265 7072  ls.._should_repr
+00000660: 5f67 6c6f 6261 6c5f 6e61 6d65 da09 5f73  _global_name.._s
+00000670: 6166 6572 6570 72da 0e41 7373 6572 7469  aferepr..Asserti
+00000680: 6f6e 4572 726f 72da 135f 666f 726d 6174  onError.._format
+00000690: 5f65 7870 6c61 6e61 7469 6f6e da06 7079  _explanation..py
+000006a0: 7465 7374 da06 7261 6973 6573 7203 0000  test..raisesr...
+000006b0: 0072 0f00 0000 da05 7661 6c75 65da 0665  .r......value..e
+000006c0: 7272 6f72 7329 0d72 0900 0000 da0b 4070  rrors).r......@p
+000006d0: 795f 6173 7365 7274 31da 0b40 7079 5f61  y_assert1..@py_a
+000006e0: 7373 6572 7434 da0b 4070 795f 6173 7365  ssert4..@py_asse
+000006f0: 7274 33da 0b40 7079 5f66 6f72 6d61 7436  rt3..@py_format6
+00000700: da0b 4070 795f 666f 726d 6174 38da 0b40  ..@py_format8..@
+00000710: 7079 5f66 6f72 6d61 7433 7211 0000 00da  py_format3r.....
+00000720: 0b40 7079 5f66 6f72 6d61 7435 da0b 4070  .@py_format5..@p
+00000730: 795f 666f 726d 6174 37da 0165 da0b 4070  y_format7..e..@p
+00000740: 795f 6173 7365 7274 30da 0b40 7079 5f61  y_assert0..@py_a
+00000750: 7373 6572 7432 a900 722f 0000 00fa 3f2f  ssert2..r/....?/
+00000760: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
+00000770: 6374 616c 2f66 7261 6374 616c 2f66 7261  ctal/fractal/fra
+00000780: 6374 616c 2f63 6f6d 6d6f 6e2f 7465 7374  ctal/common/test
+00000790: 732f 7465 7374 5f75 7365 722e 7079 da10  s/test_user.py..
+000007a0: 7465 7374 5f75 7365 725f 6372 6561 7465  test_user_create
+000007b0: 0800 0000 732c 0000 000c 0208 018a 010e  ....s,..........
+000007c0: 0208 0150 010c 0210 011c ff04 0314 019c  ...P............
+000007d0: 010c 0210 011e ff0a 0276 010c 0210 011e  .........v......
+000007e0: ff0a 027a 0172 3100 0000 290e da08 6275  ...z.r1...)...bu
+000007f0: 696c 7469 6e73 721a 0000 00da 195f 7079  iltinsr......_py
+00000800: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
+00000810: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
+00000820: 6eda 0772 6577 7269 7465 7218 0000 0072  n..rewriter....r
+00000830: 2000 0000 da08 6465 7674 6f6f 6c73 7202   .....devtoolsr.
+00000840: 0000 00da 1770 7964 616e 7469 632e 6572  .....pydantic.er
+00000850: 726f 725f 7772 6170 7065 7273 7203 0000  ror_wrappersr...
+00000860: 00da 0773 6368 656d 6173 7204 0000 0072  ...schemasr....r
+00000870: 3100 0000 722f 0000 0072 2f00 0000 722f  1...r/...r/...r/
+00000880: 0000 0072 3000 0000 da08 3c6d 6f64 756c  ...r0.....<modul
+00000890: 653e 0100 0000 730a 0000 0022 000c 010c  e>....s...."....
+000008a0: 010c 020c 03                             .....
```

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 14:42:57 2023 UTC, .py size: 2361 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,162 +1,182 @@
-00000000: 6f0d 0d0a 0000 0000 f1fb 0564 3909 0000  o..........d9...
+00000000: 6f0d 0d0a 0000 0000 dc12 5d64 240a 0000  o.........]d$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0b 6d0d 5a0d 0100  Z...d.d.l.m.Z...
 00000080: 6400 6406 6c0b 6d0e 5a0e 0100 6400 6407  d.d.l.m.Z...d.d.
 00000090: 6c0b 6d0f 5a0f 0100 6400 6408 6c0b 6d10  l.m.Z...d.d.l.m.
 000000a0: 5a10 0100 6400 6409 6c0b 6d11 5a11 0100  Z...d.d.l.m.Z...
 000000b0: 6400 640a 6c0b 6d12 5a12 0100 6400 640b  d.d.l.m.Z...d.d.
 000000c0: 6c0b 6d13 5a13 0100 6400 640c 6c0b 6d14  l.m.Z...d.d.l.m.
-000000d0: 5a14 0100 640d 640e 8400 5a15 640f 6410  Z...d.d...Z.d.d.
-000000e0: 8400 5a16 6411 6412 8400 5a17 6413 6414  ..Z.d.d...Z.d.d.
-000000f0: 8400 5a18 6415 6416 8400 5a19 6417 6418  ..Z.d.d...Z.d.d.
-00000100: 8400 5a1a 6401 5300 2919 e900 0000 004e  ..Z.d.S.)......N
-00000110: 2901 da05 6465 6275 6729 01da 0f56 616c  )...debug)...Val
-00000120: 6964 6174 696f 6e45 7272 6f72 2901 da0a  idationError)...
-00000130: 5461 736b 496d 706f 7274 2901 da08 5461  TaskImport)...Ta
-00000140: 736b 5265 6164 2901 da0e 576f 726b 666c  skRead)...Workfl
-00000150: 6f77 4372 6561 7465 2901 da0e 576f 726b  owCreate)...Work
-00000160: 666c 6f77 496d 706f 7274 2901 da0c 576f  flowImport)...Wo
-00000170: 726b 666c 6f77 5265 6164 2901 da12 576f  rkflowRead)...Wo
-00000180: 726b 666c 6f77 5461 736b 4372 6561 7465  rkflowTaskCreate
-00000190: 2901 da12 576f 726b 666c 6f77 5461 736b  )...WorkflowTask
-000001a0: 496d 706f 7274 2901 da10 576f 726b 666c  Import)...Workfl
-000001b0: 6f77 5461 736b 5265 6164 2901 da12 576f  owTaskRead)...Wo
-000001c0: 726b 666c 6f77 5461 736b 5570 6461 7465  rkflowTaskUpdate
-000001d0: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-000001e0: 0008 0000 0043 0000 0073 d000 0000 7400  .....C...s....t.
-000001f0: 6401 6402 8d01 7d00 7401 7c00 8301 0100  d.d...}.t.|.....
-00000200: 7402 a003 7404 a101 8f0d 0100 7400 6403  t...t.......t.d.
-00000210: 6402 8d01 0100 5700 6400 0400 0400 8303  d.....W.d.......
-00000220: 0100 6e08 3100 731e 7701 0100 0100 0100  ..n.1.s.w.......
-00000230: 5900 0100 7400 6401 6401 6404 8d02 7d00  Y...t.d.d.d...}.
-00000240: 7400 6401 6405 6404 8d02 7d00 7402 a003  t.d.d.d...}.t...
-00000250: 7404 a101 8f0e 0100 7400 6401 6403 6404  t.......t.d.d.d.
-00000260: 8d02 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000270: 6e08 3100 7345 7701 0100 0100 0100 5900  n.1.sEw.......Y.
-00000280: 0100 7402 a003 7404 a101 8f0f 0100 7400  ..t...t.......t.
-00000290: 6401 6400 6404 8d02 0100 5700 6400 0400  d.d.d.....W.d...
-000002a0: 0400 8303 0100 6400 5300 3100 7361 7701  ......d.S.1.saw.
-000002b0: 0100 0100 0100 5900 0100 6400 5300 2906  ......Y...d.S.).
-000002c0: 4ee9 0100 0000 2901 da07 7461 736b 5f69  N.....)...task_i
-000002d0: 64e9 ffff ffff 2902 720e 0000 00da 056f  d.....).r......o
-000002e0: 7264 6572 7201 0000 0029 0572 0900 0000  rderr....).r....
-000002f0: 7202 0000 00da 0670 7974 6573 74da 0672  r......pytest..r
-00000300: 6169 7365 7372 0300 0000 a901 da01 74a9  aisesr........t.
-00000310: 0072 1500 0000 fa43 2f68 6f6d 652f 746f  .r.....C/home/to
-00000320: 6d6d 6173 6f2f 4672 6163 7461 6c2f 6672  mmaso/Fractal/fr
-00000330: 6163 7461 6c2f 6672 6163 7461 6c2f 636f  actal/fractal/co
-00000340: 6d6d 6f6e 2f74 6573 7473 2f74 6573 745f  mmon/tests/test_
-00000350: 776f 726b 666c 6f77 2e70 79da 1974 6573  workflow.py..tes
-00000360: 745f 776f 726b 666c 6f77 5f74 6173 6b5f  t_workflow_task_
-00000370: 6372 6561 7465 1000 0000 731a 0000 000a  create....s.....
-00000380: 0208 010c 020c 011c ff0c 030c 010c 010e  ................
-00000390: 011c ff0c 020e 0122 ff72 1700 0000 6300  .......".r....c.
-000003a0: 0000 0000 0000 0000 0000 0001 0000 0008  ................
-000003b0: 0000 0043 0000 0073 5600 0000 7400 7401  ...C...sV...t.t.
-000003c0: 6401 6402 8d01 6403 8d01 7d00 7402 a003  d.d...d...}.t...
-000003d0: 7404 a101 8f10 0100 7400 7401 6404 6405  t.......t.t.d.d.
-000003e0: 8d01 6403 8d01 7d00 5700 6400 0400 0400  ..d...}.W.d.....
-000003f0: 8303 0100 6e08 3100 7320 7701 0100 0100  ....n.1.s w.....
-00000400: 0100 5900 0100 7405 7c00 8301 0100 6400  ..Y...t.|.....d.
-00000410: 5300 2906 4eda 0465 6c73 65a9 01da 0973  S.).N..else....s
-00000420: 6f6d 6574 6869 6e67 2901 da04 6d65 7461  omething)...meta
-00000430: da03 6e65 7729 01da 1570 6172 616c 6c65  ..new)...paralle
-00000440: 6c69 7a61 7469 6f6e 5f6c 6576 656c 2906  lization_level).
-00000450: 720c 0000 00da 0464 6963 7472 1100 0000  r......dictr....
-00000460: 7212 0000 0072 0300 0000 7202 0000 0072  r....r....r....r
-00000470: 1300 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00000480: 0000 00da 1974 6573 745f 776f 726b 666c  .....test_workfl
-00000490: 6f77 5f74 6173 6b5f 7570 6461 7465 2000  ow_task_update .
-000004a0: 0000 730a 0000 0010 020c 0212 011c ff0c  ..s.............
-000004b0: 0272 1f00 0000 6300 0000 0000 0000 0000  .r....c.........
-000004c0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-000004d0: 1800 0000 7400 6401 6402 6403 8d02 7d00  ....t.d.d.d...}.
-000004e0: 7401 7c00 8301 0100 6400 5300 2904 4eda  t.|.....d.S.).N.
-000004f0: 0877 6f72 6b66 6c6f 7772 0d00 0000 2902  .workflowr....).
-00000500: da04 6e61 6d65 da0a 7072 6f6a 6563 745f  ..name..project_
-00000510: 6964 2902 7206 0000 0072 0200 0000 a901  id).r....r......
-00000520: da01 7772 1500 0000 7215 0000 0072 1600  ..wr....r....r..
-00000530: 0000 da14 7465 7374 5f77 6f72 6b66 6c6f  ....test_workflo
-00000540: 775f 6372 6561 7465 2900 0000 7304 0000  w_create)...s...
-00000550: 000c 010c 0172 2500 0000 6300 0000 0000  .....r%...c.....
-00000560: 0000 0000 0000 0003 0000 0008 0000 0043  ...............C
-00000570: 0000 0073 6a00 0000 7400 6401 6402 6403  ...sj...t.d.d.d.
-00000580: 8d02 7d00 7401 7c00 6404 8d01 7d01 7402  ..}.t.|.d...}.t.
-00000590: 6405 7c01 6701 6406 8d02 7d02 7403 7c02  d.|.g.d...}.t.|.
-000005a0: 8301 0100 7404 a005 7406 a101 8f10 0100  ....t...t.......
-000005b0: 7402 6407 7c01 6701 6406 8d02 0100 5700  t.d.|.g.d.....W.
-000005c0: 6400 0400 0400 8303 0100 6400 5300 3100  d.........d.S.1.
-000005d0: 732e 7701 0100 0100 0100 5900 0100 6400  s.w.......Y...d.
-000005e0: 5300 2908 4e72 2100 0000 da06 736f 7572  S.).Nr!.....sour
-000005f0: 6365 2902 7221 0000 0072 2600 0000 2901  ce).r!...r&...).
-00000600: da04 7461 736b 7220 0000 0029 0272 2100  ..taskr ...).r!.
-00000610: 0000 da09 7461 736b 5f6c 6973 74da 0120  ....task_list.. 
-00000620: 2907 7204 0000 0072 0a00 0000 7207 0000  ).r....r....r...
-00000630: 0072 0200 0000 7211 0000 0072 1200 0000  .r....r....r....
-00000640: 7203 0000 0029 0372 1400 0000 da03 7766  r....).r......wf
-00000650: 7472 2400 0000 7215 0000 0072 1500 0000  tr$...r....r....
-00000660: 7216 0000 00da 1474 6573 745f 776f 726b  r......test_work
-00000670: 666c 6f77 5f69 6d70 6f72 742e 0000 0073  flow_import....s
-00000680: 0e00 0000 0c02 0a01 0e01 0801 0c02 1001  ................
-00000690: 22ff 722b 0000 0063 0000 0000 0000 0000  ".r+...c........
-000006a0: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
-000006b0: 731c 0000 0074 0064 0164 0264 0167 0064  s....t.d.d.d.g.d
-000006c0: 038d 047d 0074 017c 0083 0101 0064 0053  ...}.t.|.....d.S
-000006d0: 0029 044e 720d 0000 0072 2000 0000 a904  .).Nr....r .....
-000006e0: da02 6964 7221 0000 0072 2200 0000 7228  ..idr!...r"...r(
-000006f0: 0000 0029 0272 0800 0000 7202 0000 0072  ...).r....r....r
-00000700: 2300 0000 7215 0000 0072 1500 0000 7216  #...r....r....r.
-00000710: 0000 00da 2274 6573 745f 776f 726b 666c  ...."test_workfl
-00000720: 6f77 5f72 6561 645f 656d 7074 795f 7461  ow_read_empty_ta
-00000730: 736b 5f6c 6973 7439 0000 0073 0400 0000  sk_list9...s....
-00000740: 1001 0c01 722e 0000 0063 0000 0000 0000  ....r....c......
-00000750: 0000 0000 0000 0400 0000 0a00 0000 4300  ..............C.
-00000760: 0000 735c 0000 0074 0064 0164 0264 0364  ..s\...t.d.d.d.d
-00000770: 0464 0564 0674 0164 0764 088d 0164 098d  .d.d.t.d.d...d..
-00000780: 077d 0074 0264 0a64 0a64 0a7c 0064 0b8d  .}.t.d.d.d.|.d..
-00000790: 047d 0174 0264 0c64 0a64 0a7c 0064 0b8d  .}.t.d.d.d.|.d..
-000007a0: 047d 0274 0364 0a64 0d64 0a7c 017c 0267  .}.t.d.d.d.|.|.g
-000007b0: 0264 0e8d 047d 0374 047c 0383 0101 0064  .d...}.t.|.....d
-000007c0: 0053 0029 0f4e e909 0000 0072 2100 0000  .S.).N.....r!...
-000007d0: 7226 0000 00da 0763 6f6d 6d61 6e64 da0a  r&.....command..
-000007e0: 696e 7075 745f 7479 7065 da0b 6f75 7470  input_type..outp
-000007f0: 7574 5f74 7970 6572 1800 0000 7219 0000  ut_typer....r...
-00000800: 0029 0772 2d00 0000 7221 0000 0072 2600  .).r-...r!...r&.
-00000810: 0000 7230 0000 0072 3100 0000 7232 0000  ..r0...r1...r2..
-00000820: 0072 1b00 0000 720d 0000 0029 0472 2d00  .r....r....).r-.
-00000830: 0000 720e 0000 00da 0b77 6f72 6b66 6c6f  ..r......workflo
-00000840: 775f 6964 7227 0000 00e9 0200 0000 7220  w_idr'........r 
-00000850: 0000 0072 2c00 0000 2905 7205 0000 0072  ...r,...).r....r
-00000860: 1e00 0000 720b 0000 0072 0800 0000 7202  ....r....r....r.
-00000870: 0000 0029 04da 0274 31da 0477 6674 31da  ...)...t1..wft1.
-00000880: 0477 6674 3272 2400 0000 7215 0000 0072  .wft2r$...r....r
-00000890: 1500 0000 7216 0000 00da 2674 6573 745f  ....r.....&test_
-000008a0: 776f 726b 666c 6f77 5f72 6561 645f 6e6f  workflow_read_no
-000008b0: 6e5f 656d 7074 795f 7461 736b 5f6c 6973  n_empty_task_lis
-000008c0: 743e 0000 0073 1e00 0000 0202 0201 0201  t>...s..........
-000008d0: 0201 0201 0201 0201 0801 06f9 100a 1001  ................
-000008e0: 0202 0c01 06ff 0c03 7238 0000 0029 1bda  ........r8...)..
-000008f0: 0862 7569 6c74 696e 73da 0c40 7079 5f62  .builtins..@py_b
-00000900: 7569 6c74 696e 73da 195f 7079 7465 7374  uiltins.._pytest
-00000910: 2e61 7373 6572 7469 6f6e 2e72 6577 7269  .assertion.rewri
-00000920: 7465 da09 6173 7365 7274 696f 6eda 0772  te..assertion..r
-00000930: 6577 7269 7465 da0a 4070 7974 6573 745f  ewrite..@pytest_
-00000940: 6172 7211 0000 00da 0864 6576 746f 6f6c  arr......devtool
-00000950: 7372 0200 0000 da17 7079 6461 6e74 6963  sr......pydantic
-00000960: 2e65 7272 6f72 5f77 7261 7070 6572 7372  .error_wrappersr
-00000970: 0300 0000 da07 7363 6865 6d61 7372 0400  ......schemasr..
-00000980: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
-00000990: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
-000009a0: 720b 0000 0072 0c00 0000 7217 0000 0072  r....r....r....r
-000009b0: 1f00 0000 7225 0000 0072 2b00 0000 722e  ....r%...r+...r.
-000009c0: 0000 0072 3800 0000 7215 0000 0072 1500  ...r8...r....r..
-000009d0: 0000 7215 0000 0072 1600 0000 da08 3c6d  ..r....r......<m
-000009e0: 6f64 756c 653e 0100 0000 7324 0000 0022  odule>....s$..."
-000009f0: 000c 010c 010c 020c 010c 010c 010c 010c  ................
-00000a00: 010c 010c 010c 0108 0308 1008 0908 0508  ................
-00000a10: 0b0c 05                                  ...
+000000d0: 5a14 0100 6400 640d 6c0b 6d15 5a15 0100  Z...d.d.l.m.Z...
+000000e0: 640e 640f 8400 5a16 6410 6411 8400 5a17  d.d...Z.d.d...Z.
+000000f0: 6412 6413 8400 5a18 6414 6415 8400 5a19  d.d...Z.d.d...Z.
+00000100: 6416 6417 8400 5a1a 6418 6419 8400 5a1b  d.d...Z.d.d...Z.
+00000110: 641a 641b 8400 5a1c 6401 5300 291c e900  d.d...Z.d.S.)...
+00000120: 0000 004e 2901 da05 6465 6275 6729 01da  ...N)...debug)..
+00000130: 0f56 616c 6964 6174 696f 6e45 7272 6f72  .ValidationError
+00000140: 2901 da0a 5461 736b 496d 706f 7274 2901  )...TaskImport).
+00000150: da08 5461 736b 5265 6164 2901 da0e 576f  ..TaskRead)...Wo
+00000160: 726b 666c 6f77 4372 6561 7465 2901 da0e  rkflowCreate)...
+00000170: 576f 726b 666c 6f77 496d 706f 7274 2901  WorkflowImport).
+00000180: da0c 576f 726b 666c 6f77 5265 6164 2901  ..WorkflowRead).
+00000190: da12 576f 726b 666c 6f77 5461 736b 4372  ..WorkflowTaskCr
+000001a0: 6561 7465 2901 da12 576f 726b 666c 6f77  eate)...Workflow
+000001b0: 5461 736b 496d 706f 7274 2901 da10 576f  TaskImport)...Wo
+000001c0: 726b 666c 6f77 5461 736b 5265 6164 2901  rkflowTaskRead).
+000001d0: da12 576f 726b 666c 6f77 5461 736b 5570  ..WorkflowTaskUp
+000001e0: 6461 7465 2901 da0e 576f 726b 666c 6f77  date)...Workflow
+000001f0: 5570 6461 7465 6300 0000 0000 0000 0000  Updatec.........
+00000200: 0000 0001 0000 0008 0000 0043 0000 0073  ...........C...s
+00000210: 8000 0000 7400 6401 6402 8d01 7d00 7401  ....t.d.d...}.t.
+00000220: 7c00 8301 0100 7402 a003 7404 a101 8f0d  |.....t...t.....
+00000230: 0100 7400 6403 6402 8d01 0100 5700 6400  ..t.d.d.....W.d.
+00000240: 0400 0400 8303 0100 6e08 3100 731e 7701  ........n.1.s.w.
+00000250: 0100 0100 0100 5900 0100 7402 a003 7404  ......Y...t...t.
+00000260: a101 8f0e 0100 7400 6400 6402 8d01 0100  ......t.d.d.....
+00000270: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
+00000280: 3100 7339 7701 0100 0100 0100 5900 0100  1.s9w.......Y...
+00000290: 6400 5300 2904 4ee9 0100 0000 2901 da05  d.S.).N.....)...
+000002a0: 6f72 6465 72e9 ffff ffff 2905 7209 0000  order.....).r...
+000002b0: 0072 0200 0000 da06 7079 7465 7374 da06  .r......pytest..
+000002c0: 7261 6973 6573 7203 0000 00a9 01da 0174  raisesr........t
+000002d0: a900 7215 0000 00fa 432f 686f 6d65 2f74  ..r.....C/home/t
+000002e0: 6f6d 6d61 736f 2f46 7261 6374 616c 2f66  ommaso/Fractal/f
+000002f0: 7261 6374 616c 2f66 7261 6374 616c 2f63  ractal/fractal/c
+00000300: 6f6d 6d6f 6e2f 7465 7374 732f 7465 7374  ommon/tests/test
+00000310: 5f77 6f72 6b66 6c6f 772e 7079 da19 7465  _workflow.py..te
+00000320: 7374 5f77 6f72 6b66 6c6f 775f 7461 736b  st_workflow_task
+00000330: 5f63 7265 6174 6511 0000 0073 1000 0000  _create....s....
+00000340: 0a02 0801 0c02 0c01 1cff 0c02 0c01 22ff  ..............".
+00000350: 7217 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000360: 0000 0100 0000 0800 0000 4300 0000 7356  ..........C...sV
+00000370: 0000 0074 0074 0164 0164 028d 0164 038d  ...t.t.d.d...d..
+00000380: 017d 0074 02a0 0374 04a1 018f 1001 0074  .}.t...t.......t
+00000390: 0074 0164 0464 058d 0164 038d 017d 0057  .t.d.d...d...}.W
+000003a0: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+000003b0: 2077 0101 0001 0001 0059 0001 0074 057c   w.......Y...t.|
+000003c0: 0083 0101 0064 0053 0029 064e da04 656c  .....d.S.).N..el
+000003d0: 7365 a901 da09 736f 6d65 7468 696e 6729  se....something)
+000003e0: 01da 046d 6574 61da 036e 6577 2901 da15  ...meta..new)...
+000003f0: 7061 7261 6c6c 656c 697a 6174 696f 6e5f  parallelization_
+00000400: 6c65 7665 6c29 0672 0c00 0000 da04 6469  level).r......di
+00000410: 6374 7211 0000 0072 1200 0000 7203 0000  ctr....r....r...
+00000420: 0072 0200 0000 7213 0000 0072 1500 0000  .r....r....r....
+00000430: 7215 0000 0072 1600 0000 da19 7465 7374  r....r......test
+00000440: 5f77 6f72 6b66 6c6f 775f 7461 736b 5f75  _workflow_task_u
+00000450: 7064 6174 651c 0000 0073 0a00 0000 1002  pdate....s......
+00000460: 0c02 1201 1cff 0c02 721f 0000 0063 0000  ........r....c..
+00000470: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000480: 0000 4300 0000 7316 0000 0074 0064 0164  ..C...s....t.d.d
+00000490: 028d 017d 0074 017c 0083 0101 0064 0053  ...}.t.|.....d.S
+000004a0: 0029 034e da08 776f 726b 666c 6f77 a901  .).N..workflow..
+000004b0: da04 6e61 6d65 2902 7206 0000 0072 0200  ..name).r....r..
+000004c0: 0000 a901 da01 7772 1500 0000 7215 0000  ......wr....r...
+000004d0: 0072 1600 0000 da14 7465 7374 5f77 6f72  .r......test_wor
+000004e0: 6b66 6c6f 775f 6372 6561 7465 2500 0000  kflow_create%...
+000004f0: 7304 0000 000a 010c 0172 2500 0000 6300  s........r%...c.
+00000500: 0000 0000 0000 0000 0000 0003 0000 0008  ................
+00000510: 0000 0043 0000 0073 6a00 0000 7400 6401  ...C...sj...t.d.
+00000520: 6402 6403 8d02 7d00 7401 7c00 6404 8d01  d.d...}.t.|.d...
+00000530: 7d01 7402 6405 7c01 6701 6406 8d02 7d02  }.t.d.|.g.d...}.
+00000540: 7403 7c02 8301 0100 7404 a005 7406 a101  t.|.....t...t...
+00000550: 8f10 0100 7402 6407 7c01 6701 6406 8d02  ....t.d.|.g.d...
+00000560: 0100 5700 6400 0400 0400 8303 0100 6400  ..W.d.........d.
+00000570: 5300 3100 732e 7701 0100 0100 0100 5900  S.1.s.w.......Y.
+00000580: 0100 6400 5300 2908 4e72 2200 0000 da06  ..d.S.).Nr".....
+00000590: 736f 7572 6365 2902 7222 0000 0072 2600  source).r"...r&.
+000005a0: 0000 2901 da04 7461 736b 7220 0000 0029  ..)...taskr ...)
+000005b0: 0272 2200 0000 da09 7461 736b 5f6c 6973  .r".....task_lis
+000005c0: 74da 0120 2907 7204 0000 0072 0a00 0000  t.. ).r....r....
+000005d0: 7207 0000 0072 0200 0000 7211 0000 0072  r....r....r....r
+000005e0: 1200 0000 7203 0000 0029 0372 1400 0000  ....r....).r....
+000005f0: da03 7766 7472 2400 0000 7215 0000 0072  ..wftr$...r....r
+00000600: 1500 0000 7216 0000 00da 1474 6573 745f  ....r......test_
+00000610: 776f 726b 666c 6f77 5f69 6d70 6f72 742a  workflow_import*
+00000620: 0000 0073 0e00 0000 0c02 0a01 0e01 0801  ...s............
+00000630: 0c02 1001 22ff 722b 0000 0063 0000 0000  ....".r+...c....
+00000640: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00000650: 4300 0000 731c 0000 0074 0064 0164 0264  C...s....t.d.d.d
+00000660: 0167 0064 038d 047d 0074 017c 0083 0101  .g.d...}.t.|....
+00000670: 0064 0053 0029 044e 720e 0000 0072 2000  .d.S.).Nr....r .
+00000680: 0000 a904 da02 6964 7222 0000 00da 0a70  ......idr".....p
+00000690: 726f 6a65 6374 5f69 6472 2800 0000 2902  roject_idr(...).
+000006a0: 7208 0000 0072 0200 0000 7223 0000 0072  r....r....r#...r
+000006b0: 1500 0000 7215 0000 0072 1600 0000 da22  ....r....r....."
+000006c0: 7465 7374 5f77 6f72 6b66 6c6f 775f 7265  test_workflow_re
+000006d0: 6164 5f65 6d70 7479 5f74 6173 6b5f 6c69  ad_empty_task_li
+000006e0: 7374 3500 0000 7304 0000 0010 010c 0172  st5...s........r
+000006f0: 2f00 0000 6300 0000 0000 0000 0000 0000  /...c...........
+00000700: 0004 0000 000a 0000 0043 0000 0073 5c00  .........C...s\.
+00000710: 0000 7400 6401 6402 6403 6404 6405 6406  ..t.d.d.d.d.d.d.
+00000720: 7401 6407 6408 8d01 6409 8d07 7d00 7402  t.d.d...d...}.t.
+00000730: 640a 640a 640a 7c00 640b 8d04 7d01 7402  d.d.d.|.d...}.t.
+00000740: 640c 640a 640a 7c00 640b 8d04 7d02 7403  d.d.d.|.d...}.t.
+00000750: 640a 640d 640a 7c01 7c02 6702 640e 8d04  d.d.d.|.|.g.d...
+00000760: 7d03 7404 7c03 8301 0100 6400 5300 290f  }.t.|.....d.S.).
+00000770: 4ee9 0900 0000 7222 0000 0072 2600 0000  N.....r"...r&...
+00000780: da07 636f 6d6d 616e 64da 0a69 6e70 7574  ..command..input
+00000790: 5f74 7970 65da 0b6f 7574 7075 745f 7479  _type..output_ty
+000007a0: 7065 7218 0000 0072 1900 0000 2907 722d  per....r....).r-
+000007b0: 0000 0072 2200 0000 7226 0000 0072 3100  ...r"...r&...r1.
+000007c0: 0000 7232 0000 0072 3300 0000 721b 0000  ..r2...r3...r...
+000007d0: 0072 0e00 0000 2904 722d 0000 00da 0774  .r....).r-.....t
+000007e0: 6173 6b5f 6964 da0b 776f 726b 666c 6f77  ask_id..workflow
+000007f0: 5f69 6472 2700 0000 e902 0000 0072 2000  _idr'........r .
+00000800: 0000 722c 0000 0029 0572 0500 0000 721e  ..r,...).r....r.
+00000810: 0000 0072 0b00 0000 7208 0000 0072 0200  ...r....r....r..
+00000820: 0000 2904 da02 7431 da04 7766 7431 da04  ..)...t1..wft1..
+00000830: 7766 7432 7224 0000 0072 1500 0000 7215  wft2r$...r....r.
+00000840: 0000 0072 1600 0000 da26 7465 7374 5f77  ...r.....&test_w
+00000850: 6f72 6b66 6c6f 775f 7265 6164 5f6e 6f6e  orkflow_read_non
+00000860: 5f65 6d70 7479 5f74 6173 6b5f 6c69 7374  _empty_task_list
+00000870: 3a00 0000 731e 0000 0002 0202 0102 0102  :...s...........
+00000880: 0102 0102 0102 0108 0106 f910 0a10 0102  ................
+00000890: 020c 0106 ff0c 0372 3a00 0000 6300 0000  .......r:...c...
+000008a0: 0000 0000 0000 0000 0000 0000 0008 0000  ................
+000008b0: 0043 0000 0073 a200 0000 7400 6401 6700  .C...s....t.d.g.
+000008c0: 6402 a201 6403 8d02 0100 7400 6401 6404  d...d.....t.d.d.
+000008d0: 8d01 0100 7400 6700 6402 a201 6405 8d01  ....t.g.d...d...
+000008e0: 0100 7401 a002 7403 a101 8f10 0100 7400  ..t...t.......t.
+000008f0: 6401 6700 6406 a201 6403 8d02 0100 5700  d.g.d...d.....W.
+00000900: 6400 0400 0400 8303 0100 6e08 3100 732c  d.........n.1.s,
+00000910: 7701 0100 0100 0100 5900 0100 7401 a002  w.......Y...t...
+00000920: 7403 a101 8f11 0100 7400 6401 6700 6407  t.......t.d.g.d.
+00000930: a201 6403 8d02 0100 5700 6400 0400 0400  ..d.....W.d.....
+00000940: 8303 0100 6400 5300 3100 734a 7701 0100  ....d.S.1.sJw...
+00000950: 0100 0100 5900 0100 6400 5300 2908 4e72  ....Y...d.S.).Nr
+00000960: 2000 0000 2904 7201 0000 0072 0e00 0000   ...).r....r....
+00000970: e903 0000 0072 3600 0000 2902 7222 0000  .....r6...).r"..
+00000980: 00da 1a72 656f 7264 6572 6564 5f77 6f72  ...reordered_wor
+00000990: 6b66 6c6f 7774 6173 6b5f 6964 7372 2100  kflowtask_idsr!.
+000009a0: 0000 2901 723c 0000 0029 0372 0e00 0000  ..).r<...).r....
+000009b0: 723b 0000 0072 0e00 0000 2903 720e 0000  r;...r....).r...
+000009c0: 0072 3b00 0000 7210 0000 0029 0472 0d00  .r;...r....).r..
+000009d0: 0000 7211 0000 0072 1200 0000 7203 0000  ..r....r....r...
+000009e0: 0072 1500 0000 7215 0000 0072 1500 0000  .r....r....r....
+000009f0: 7216 0000 00da 1474 6573 745f 776f 726b  r......test_work
+00000a00: 666c 6f77 5f75 7064 6174 654f 0000 0073  flow_updateO...s
+00000a10: 1200 0000 1001 0a01 0e01 0c01 1201 1cff  ................
+00000a20: 0c02 1201 22ff 723d 0000 0029 1dda 0862  ....".r=...)...b
+00000a30: 7569 6c74 696e 73da 0c40 7079 5f62 7569  uiltins..@py_bui
+00000a40: 6c74 696e 73da 195f 7079 7465 7374 2e61  ltins.._pytest.a
+00000a50: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
+00000a60: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
+00000a70: 7269 7465 da0a 4070 7974 6573 745f 6172  rite..@pytest_ar
+00000a80: 7211 0000 00da 0864 6576 746f 6f6c 7372  r......devtoolsr
+00000a90: 0200 0000 da17 7079 6461 6e74 6963 2e65  ......pydantic.e
+00000aa0: 7272 6f72 5f77 7261 7070 6572 7372 0300  rror_wrappersr..
+00000ab0: 0000 da07 7363 6865 6d61 7372 0400 0000  ....schemasr....
+00000ac0: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+00000ad0: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+00000ae0: 0000 0072 0c00 0000 720d 0000 0072 1700  ...r....r....r..
+00000af0: 0000 721f 0000 0072 2500 0000 722b 0000  ..r....r%...r+..
+00000b00: 0072 2f00 0000 723a 0000 0072 3d00 0000  .r/...r:...r=...
+00000b10: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
+00000b20: 1600 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000b30: 0000 7328 0000 0022 000c 010c 010c 020c  ..s(..."........
+00000b40: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00000b50: 0108 0308 0b08 0908 0508 0b08 050c 15    ...............
```

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/test_dataset.py` & `fractal_client-1.3.0a0/fractal/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/test_manifest.py` & `fractal_client-1.3.0a0/fractal/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/test_project.py` & `fractal_client-1.3.0a0/fractal/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/test_state.py` & `fractal_client-1.3.0a0/fractal/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/test_task.py` & `fractal_client-1.3.0a0/fractal/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/test_user.py` & `fractal_client-1.3.0a0/fractal/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/common/tests/test_workflow.py` & `fractal_client-1.3.0a0/fractal/common/tests/test_workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,39 +12,34 @@
 from schemas import WorkflowTaskRead
 from schemas import WorkflowTaskUpdate
 from schemas import WorkflowUpdate
 
 
 def test_workflow_task_create():
     # Successful creation
-    t = WorkflowTaskCreate(task_id=1)
+    t = WorkflowTaskCreate(order=1)
     debug(t)
-    # Missing arguments
+    # Invalid arguments
     with pytest.raises(ValidationError):
-        WorkflowTaskCreate(task_id=-1)
-    # Several values of order
-    t = WorkflowTaskCreate(task_id=1, order=1)
-    t = WorkflowTaskCreate(task_id=1, order=0)
+        WorkflowTaskCreate(order=-1)
     with pytest.raises(ValidationError):
-        WorkflowTaskCreate(task_id=1, order=-1)
-    with pytest.raises(ValidationError):
-        WorkflowTaskCreate(task_id=1, order=None)
+        WorkflowTaskCreate(order=None)
 
 
 def test_workflow_task_update():
     # Successful creation
     t = WorkflowTaskUpdate(meta=dict(something="else"))
     # Forbidden key-value update
     with pytest.raises(ValidationError):
         t = WorkflowTaskUpdate(meta=dict(parallelization_level="new"))
     debug(t)
 
 
 def test_workflow_create():
-    w = WorkflowCreate(name="workflow", project_id=1)
+    w = WorkflowCreate(name="workflow")
     debug(w)
 
 
 def test_workflow_import():
     # Successful creation
     t = TaskImport(name="name", source="source")
     wft = WorkflowTaskImport(task=t)
```

### Comparing `fractal_client-1.2.0a0/fractal/config.py` & `fractal_client-1.3.0a0/fractal/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/interface.py` & `fractal_client-1.3.0a0/fractal/interface.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/fractal/parser.py` & `fractal_client-1.3.0a0/fractal/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,14 +114,19 @@
 project_add_dataset_parser.add_argument(
     "dataset_name", help="Name of new dataset"
 )
 project_add_dataset_parser.add_argument(
     "--metadata",
     help="Path to file containing dataset metadata in JSON format.",
 )
+project_add_dataset_parser.add_argument(
+    "--type",
+    help="Dataset type",
+)
+
 
 # project edit
 project_edit_parser = project_subparsers.add_parser(
     "edit",
     description="Edit details of a single project",
     allow_abbrev=False,
 )
@@ -312,15 +317,18 @@
     default=False,
     action="store_true",
     help="Also include task-collection logs",
 )
 task_check_collection_parser.add_argument(
     "--do-not-separate-logs",
     dest="do_not_separate_logs",
-    help="Show the job logs in the main output, instead of a separate field",
+    help=(
+        "Show the task-collection logs in the main output, "
+        "instead of a separate field"
+    ),
     action="store_true",
     required=False,
 )
 
 
 # task new
 task_new_parser = task_subparsers.add_parser(
@@ -416,79 +424,73 @@
 
 # workflow list
 workflow_list_parser = workflow_subparsers.add_parser(
     "list",
     description="List workflows for given project",
     allow_abbrev=False,
 )
-workflow_list_parser.add_argument(
-    "project_id",
-    help="Project ID",
-)
+workflow_list_parser.add_argument("project_id", type=int, help="Project ID")
 
 # workflow new
 workflow_new_parser = workflow_subparsers.add_parser(
     "new",
     description="Create new workflow",
     allow_abbrev=False,
 )
 workflow_new_parser.add_argument(
     "name",
     help="Workflow name (must be unique, and not only made of numbers only)",
+    type=str,
 )
-workflow_new_parser.add_argument(
-    "project_id",
-    help="Project ID",
-)
+workflow_new_parser.add_argument("project_id", type=int, help="Project ID")
 
 # workflow show
-workflow_new_parser = workflow_subparsers.add_parser(
+workflow_show_parser = workflow_subparsers.add_parser(
     "show",
     description="Show workflow",
     allow_abbrev=False,
 )
-workflow_new_parser.add_argument(
-    "workflow_id",
-    help="Workflow ID",
-)
+workflow_show_parser.add_argument("project_id", type=int, help="Project ID")
+workflow_show_parser.add_argument("workflow_id", type=int, help="Workflow ID")
 
 # workflow edit
 workflow_edit_parser = workflow_subparsers.add_parser(
     "edit",
     description="Edit workflow",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
-workflow_edit_parser.add_argument(
-    "workflow_id",
-    type=int,
-    help="Workflow ID",
-)
+workflow_edit_parser.add_argument("project_id", type=int, help="Project ID")
+workflow_edit_parser.add_argument("workflow_id", type=int, help="Workflow ID")
 workflow_edit_parser.add_argument("--name", type=str, help="New workflow name")
 
 # workflow delete
 workflow_delete_parser = workflow_subparsers.add_parser(
     "delete",
     description="Delete workflow",
     allow_abbrev=False,
 )
+workflow_delete_parser.add_argument("project_id", type=int, help="Project ID")
 workflow_delete_parser.add_argument(
-    "workflow_id",
-    help="Workflow ID",
+    "workflow_id", type=int, help="Workflow ID"
 )
 
 
 # workflow add task
 workflow_add_task_parser = workflow_subparsers.add_parser(
     "add-task",
     description="Add new task to specific workflow",
     allow_abbrev=False,
 )
 workflow_add_task_parser.add_argument(
+    "project_id", type=int, help="Project ID"
+)
+workflow_add_task_parser.add_argument(
     "workflow_id",
+    type=int,
     help="Workflow ID",
 )
 workflow_add_task_parser.add_argument(
     "task_id_or_name", help="ID or name of the new task", type=str
 )
 workflow_add_task_parser.add_argument(
     "--order", help="Order of this task within the workflow's task list"
@@ -511,15 +513,19 @@
 # workflow edit task
 workflow_edit_task_parser = workflow_subparsers.add_parser(
     "edit-task",
     description="Edit task within specific workflow",
     allow_abbrev=False,
 )
 workflow_edit_task_parser.add_argument(
+    "project_id", type=int, help="Project ID"
+)
+workflow_edit_task_parser.add_argument(
     "workflow_id",
+    type=int,
     help="Workflow ID",
 )
 workflow_edit_task_parser.add_argument(
     "workflow_task_id",
     help="Workflow task ID, the ID of a task inside the list of tasks",
 )
 workflow_edit_task_parser.add_argument(
@@ -540,45 +546,38 @@
 # workflow remove task
 workflow_remove_task_parser = workflow_subparsers.add_parser(
     "rm-task",
     description="Remove task from a specific workflow",
     allow_abbrev=False,
 )
 workflow_remove_task_parser.add_argument(
+    "project_id", type=int, help="Project ID"
+)
+workflow_remove_task_parser.add_argument(
     "workflow_id",
+    type=int,
     help="Workflow ID",
 )
 workflow_remove_task_parser.add_argument(
     "workflow_task_id",
     help="Workflow task ID (the ID of a task inside the list of tasks)",
 )
 
 # workflow apply
 workflow_apply_parser = workflow_subparsers.add_parser(
     "apply",
     description="Apply workflow to dataset",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
+
+workflow_apply_parser.add_argument("project_id")
 workflow_apply_parser.add_argument("workflow_id")
 workflow_apply_parser.add_argument("input_dataset_id")
-workflow_apply_parser.add_argument(
-    "-o", "--output_dataset_id", help="Output dataset ID"
-)
-workflow_apply_parser.add_argument(
-    "--overwrite-input",
-    default=False,
-    action="store_true",
-    help="Allow overwriting the content of the input dataset",
-)
-workflow_apply_parser.add_argument(
-    "-p",
-    "--project-id",
-    help="ID of project the workflow and dataset belong to",
-)
+workflow_apply_parser.add_argument("output_dataset_id")
 workflow_apply_parser.add_argument(
     "-w",
     "--worker-init",
     help="Command to be run before starting a worker",
 )
 
 # workflow import
@@ -600,15 +599,21 @@
 # workflow export
 workflow_export_parser = workflow_subparsers.add_parser(
     "export",
     description="Export workflow to file",
     allow_abbrev=False,
 )
 workflow_export_parser.add_argument(
+    "project_id",
+    type=int,
+    help="Project ID",
+)
+workflow_export_parser.add_argument(
     "workflow_id",
+    type=int,
     help="Workflow ID",
 )
 workflow_export_parser.add_argument(
     "--json-file",
     help="Path to the JSON file where the workflow will be exported",
     required=True,
 )
@@ -628,28 +633,27 @@
 job_list_parser = job_subparsers.add_parser(
     "list",
     description="List jobs for given project",
     allow_abbrev=False,
 )
 job_list_parser.add_argument(
     "project_id",
+    type=int,
     help="Project ID",
 )
 
 # job show
 job_show_parser = job_subparsers.add_parser(
     "show",
     description="Query status of workflow-execution job",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
-job_show_parser.add_argument(
-    "job_id",
-    help="ID of the job",
-)
+job_show_parser.add_argument("project_id", type=int, help="Project ID")
+job_show_parser.add_argument("job_id", type=int, help="Job ID")
 job_show_parser.add_argument(
     "--do-not-separate-logs",
     dest="do_not_separate_logs",
     help="Show the job logs in the main output, instead of a separate field",
     action="store_true",
     required=False,
 )
@@ -657,24 +661,33 @@
 # job download-logs
 job_download_logs_parser = job_subparsers.add_parser(
     "download-logs",
     description="Download full folder of workflow-execution job",
     allow_abbrev=False,
 )
 job_download_logs_parser.add_argument(
-    "job_id",
-    help="ID of the job",
+    "project_id", type=int, help="Project ID"
 )
+job_download_logs_parser.add_argument("job_id", type=int, help="Job ID")
 job_download_logs_parser.add_argument(
     "--output",
     dest="output_folder",
     help="Path of the output folder",
     required=True,
 )
 
+# job stop
+job_stop_parser = job_subparsers.add_parser(
+    "stop",
+    description="Stop workflow-execution job",
+    allow_abbrev=False,
+)
+job_stop_parser.add_argument("project_id", type=int, help="Project ID")
+job_stop_parser.add_argument("job_id", type=int, help="Job ID")
+
 
 # VERSION GROUP
 version_parser = subparsers_main.add_parser(
     "version",
     description="Print version and exit",
     allow_abbrev=False,
 )
```

### Comparing `fractal_client-1.2.0a0/fractal/response.py` & `fractal_client-1.3.0a0/fractal/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.2.0a0/pyproject.toml` & `fractal_client-1.3.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "1.2.0a0"
+version = "1.3.0a0"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -43,15 +43,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.bumpver]
-current_version = "1.2.0a0"
+current_version = "1.3.0a0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_client-1.2.0a0/setup.py` & `fractal_client-1.3.0a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 entry_points = \
 {'console_scripts': ['fractal = fractal.__main__:run',
                      'fractal_new = fractal.new:run',
                      'fractal_old = fractal.old:run']}
 
 setup_kwargs = {
     'name': 'fractal-client',
-    'version': '1.2.0a0',
+    'version': '1.3.0a0',
     'description': 'Client component of the Fractal analytics platform',
     'long_description': '# Fractal Client\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-client?color=gree)](https://pypi.org/project/fractal-client/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![Documentation Status](https://github.com/fractal-analytics-platform/fractal/actions/workflows/documentation.yaml/badge.svg)](https://fractal-analytics-platform.github.io/fractal)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high-content imaging data at scale and prepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nFractal provides distributed workflows that convert TBs of image data into OME-Zarr files. The platform then processes the 3D image data by applying tasks like illumination correction, maximum intensity projection, 3D segmentation using [cellpose](https://cellpose.readthedocs.io/en/latest/) and measurements using [napari workflows](https://github.com/haesleinhuepf/napari-workflows). The pyramidal OME-Zarr files enable interactive visualization in the napari viewer.\n\nThis is the repository that contains the **Fractal client**. Find more information about Fractal in general and the other repositories at the [Fractal home page](https://fractal-analytics-platform.github.io).\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa) & [@jacopo-exact](https://github.com/jacopo-exact) from [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Tommaso Comparin',
     'author_email': 'tommaso.comparin@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal',
```

### Comparing `fractal_client-1.2.0a0/PKG-INFO` & `fractal_client-1.3.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-client
-Version: 1.2.0a0
+Version: 1.3.0a0
 Summary: Client component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

