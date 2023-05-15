# Comparing `tmp/fractal_server-1.3.0a0.tar.gz` & `tmp/fractal_server-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.3.0a0.tar", max compression
+gzip compressed data, was "fractal_server-1.3.0a1.tar", max compression
```

## Comparing `fractal_server-1.3.0a0.tar` & `fractal_server-1.3.0a1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a0/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.3.0a0/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a0/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-05-12 12:35:12.629324 fractal_server-1.3.0a0/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-04-19 11:52:26.187278 fractal_server-1.3.0a0/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a0/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a0/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a0/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     6314 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/_aux_functions.py
--rw-r--r--   0        0        0     6974 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/dataset.py
--rw-r--r--   0        0        0     4817 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0     8401 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    12661 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    12202 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a0/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3370 2023-05-12 09:56:36.874307 fractal_server-1.3.0a0/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     2295 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     2534 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.3.0a0/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.3.0a0/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5464 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a0/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     8968 2023-05-12 09:56:36.874307 fractal_server-1.3.0a0/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19458 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.3.0a0/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a0/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a0/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4334 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19861 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    42000 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     7900 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a0/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a0/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1658 2023-05-12 09:55:08.603302 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-05-08 12:02:12.597892 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-05-08 12:02:12.605892 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     4943 2023-05-09 12:55:27.450288 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1135 2023-05-12 09:55:08.619302 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     3957 2023-05-09 12:55:27.454288 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1135 2023-05-12 09:54:53.927466 fractal_server-1.3.0a0/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4323 2023-05-09 11:24:30.681084 fractal_server-1.3.0a0/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      980 2023-05-12 09:54:53.927466 fractal_server-1.3.0a0/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2502 2023-05-09 11:24:30.681084 fractal_server-1.3.0a0/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-05-08 12:02:13.009887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-05-08 12:02:13.013887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2227 2023-05-08 12:02:13.017887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a0/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a0/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12164 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a0/fractal_server/logger.py
--rw-r--r--   0        0        0     5726 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a0/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a0/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a0/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      751 2023-05-12 09:56:36.874307 fractal_server-1.3.0a0/fractal_server/migrations/versions/bb1cca2acc40_add_applyworkflow_end_timestamp.py
--rw-r--r--   0        0        0     8438 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/migrations/versions/e8f4051440be_new_initial_schema.py
--rw-r--r--   0        0        0      745 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/migrations/versions/fda995215ae9_drop_applyworkflow_overwrite_input.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a0/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a0/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a0/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12869 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a0/fractal_server/utils.py
--rw-r--r--   0        0        0     2592 2023-05-12 12:35:12.625325 fractal_server-1.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 fractal_server-1.3.0a0/setup.py
--rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 fractal_server-1.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a1/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.3.0a1/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a1/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-05-15 10:44:39.530576 fractal_server-1.3.0a1/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-04-19 11:52:26.187278 fractal_server-1.3.0a1/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a1/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a1/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a1/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     6314 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     6974 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4817 2023-05-12 12:34:32.122055 fractal_server-1.3.0a1/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a1/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    12661 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    12202 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a1/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3370 2023-05-12 09:56:36.874307 fractal_server-1.3.0a1/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2295 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2534 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.3.0a1/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.3.0a1/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5464 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a1/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     8969 2023-05-15 10:36:57.758906 fractal_server-1.3.0a1/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19458 2023-05-12 12:34:32.122055 fractal_server-1.3.0a1/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a1/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.3.0a1/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a1/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a1/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19861 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42127 2023-05-15 10:36:57.758906 fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     7900 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a1/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a1/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a1/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a1/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a1/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a1/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       48 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.3.0a1/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1658 2023-05-12 09:55:08.603302 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2023-05-08 12:02:12.597892 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1205 2023-05-08 12:02:12.605892 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     4943 2023-05-09 12:55:27.450288 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     1135 2023-05-12 09:55:08.619302 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     3957 2023-05-09 12:55:27.454288 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1135 2023-05-12 09:54:53.927466 fractal_server-1.3.0a1/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.3.0a1/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     4323 2023-05-09 11:24:30.681084 fractal_server-1.3.0a1/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0      980 2023-05-12 09:54:53.927466 fractal_server-1.3.0a1/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2502 2023-05-09 11:24:30.681084 fractal_server-1.3.0a1/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      873 2023-05-08 12:02:13.009887 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2236 2023-05-08 12:02:13.013887 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2227 2023-05-08 12:02:13.017887 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a1/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-05-08 12:01:46.018194 fractal_server-1.3.0a1/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a1/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12164 2023-05-12 12:34:32.122055 fractal_server-1.3.0a1/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a1/fractal_server/logger.py
+-rw-r--r--   0        0        0     5726 2023-05-12 12:34:32.122055 fractal_server-1.3.0a1/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a1/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a1/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a1/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      751 2023-05-12 09:56:36.874307 fractal_server-1.3.0a1/fractal_server/migrations/versions/bb1cca2acc40_add_applyworkflow_end_timestamp.py
+-rw-r--r--   0        0        0     8438 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/migrations/versions/e8f4051440be_new_initial_schema.py
+-rw-r--r--   0        0        0      745 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/migrations/versions/fda995215ae9_drop_applyworkflow_overwrite_input.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a1/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a1/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a1/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    12869 2023-05-12 06:48:40.382595 fractal_server-1.3.0a1/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a1/fractal_server/utils.py
+-rw-r--r--   0        0        0     2667 2023-05-15 10:44:39.526576 fractal_server-1.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4078 1970-01-01 00:00:00.000000 fractal_server-1.3.0a1/setup.py
+-rw-r--r--   0        0        0     3596 1970-01-01 00:00:00.000000 fractal_server-1.3.0a1/PKG-INFO
```

### Comparing `fractal_server-1.3.0a0/LICENSE` & `fractal_server-1.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/README.md` & `fractal_server-1.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/__main__.py` & `fractal_server-1.3.0a1/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/alembic.ini` & `fractal_server-1.3.0a1/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/api/__init__.py` & `fractal_server-1.3.0a1/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/api/v1/_aux_functions.py` & `fractal_server-1.3.0a1/fractal_server/app/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/api/v1/dataset.py` & `fractal_server-1.3.0a1/fractal_server/app/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.0a1/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/api/v1/project.py` & `fractal_server-1.3.0a1/fractal_server/app/api/v1/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,29 @@
     project_update: ProjectUpdate,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ):
     project = await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
+
+    # Check that there is no project with the same user and name
+    stm = (
+        select(Project)
+        .join(LinkUserProject)
+        .where(Project.name == project_update.name)
+        .where(LinkUserProject.user_id == user.id)
+    )
+    res = await db.execute(stm)
+    if res.scalars().all():
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=f"Project name ({project_update.name}) already in use",
+        )
+
     for key, value in project_update.dict(exclude_unset=True).items():
         setattr(project, key, value)
 
     await db.commit()
     await db.refresh(project)
     await db.close()
     return project
```

### Comparing `fractal_server-1.3.0a0/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.0a1/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.0a1/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/db/__init__.py` & `fractal_server-1.3.0a1/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/models/job.py` & `fractal_server-1.3.0a1/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/models/project.py` & `fractal_server-1.3.0a1/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/models/security.py` & `fractal_server-1.3.0a1/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/models/state.py` & `fractal_server-1.3.0a1/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/models/task.py` & `fractal_server-1.3.0a1/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/models/workflow.py` & `fractal_server-1.3.0a1/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     This function wraps the process_workflow one, which is different for each
     backend (e.g. local or slurm backend).
 
     Args:
         workflow_id:
             ID of the workflow being applied
-        input_dataset_id
+        input_dataset_id:
             Input dataset ID
         output_dataset_id:
             ID of the destination dataset of the workflow.
         job_id:
             Id of the job record which stores the state for the current
             workflow application.
         worker_init:
```

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_common.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 paths=filenames, user=self.slurm_user
             )
             if all_files_exist:
                 self.callback(self.waiting[filenames])
                 del self.waiting[filenames]
         if self.shutdown_file and os.path.exists(self.shutdown_file):
             logger.info(
-                "Detected executor-shutdown file " f"{str(self.shutdown_file)}"
+                f"Detected executor-shutdown file {str(self.shutdown_file)}"
             )
             self.shutdown = True
 
     def run(self):
         """
         Overrides the original clusterfutures.FileWaitThread.run, adding a call
         to self.shutdown_callback.
```

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -672,23 +672,26 @@
         failures may not be captured by the main thread; we use a broad
         try/except block, so that those exceptions are reported to the main
         thread via `fut.set_exception(...)`.
 
         Arguments:
             jobid: ID of the SLURM job
         """
-
-        with self.jobs_lock:
-            fut, job = self.jobs.pop(jobid)
-            if not self.jobs:
-                self.jobs_empty_cond.notify_all()
-
         # Handle all uncaught exceptions in this broad try/except block
         try:
 
+            # Retrieve job
+            with self.jobs_lock:
+                try:
+                    fut, job = self.jobs.pop(jobid)
+                except KeyError:
+                    return
+                if not self.jobs:
+                    self.jobs_empty_cond.notify_all()
+
             # Copy all relevant files from self.working_dir_user to
             # self.working_dir
 
             self._copy_files_from_user_to_server(job)
 
             # Update the paths to use the files in self.working_dir (rather
             # than the user's ones in self.working_dir_user)
```

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/runner/common.py` & `fractal_server-1.3.0a1/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/app/security/__init__.py` & `fractal_server-1.3.0a1/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.3.0a1/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.3.0a1/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/README.md` & `fractal_server-1.3.0a1/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.3.0a1/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.0a1/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.3.0a1/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/manifest.py` & `fractal_server-1.3.0a1/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/project.py` & `fractal_server-1.3.0a1/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/state.py` & `fractal_server-1.3.0a1/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/task.py` & `fractal_server-1.3.0a1/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/user.py` & `fractal_server-1.3.0a1/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.0a1/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.3.0a1/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.3.0a1/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/test_project.py` & `fractal_server-1.3.0a1/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/test_state.py` & `fractal_server-1.3.0a1/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/test_task.py` & `fractal_server-1.3.0a1/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/test_user.py` & `fractal_server-1.3.0a1/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.3.0a1/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/config.py` & `fractal_server-1.3.0a1/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/logger.py` & `fractal_server-1.3.0a1/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/main.py` & `fractal_server-1.3.0a1/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/migrations/env.py` & `fractal_server-1.3.0a1/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.0a1/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/migrations/versions/bb1cca2acc40_add_applyworkflow_end_timestamp.py` & `fractal_server-1.3.0a1/fractal_server/migrations/versions/bb1cca2acc40_add_applyworkflow_end_timestamp.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/migrations/versions/e8f4051440be_new_initial_schema.py` & `fractal_server-1.3.0a1/fractal_server/migrations/versions/e8f4051440be_new_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/migrations/versions/fda995215ae9_drop_applyworkflow_overwrite_input.py` & `fractal_server-1.3.0a1/fractal_server/migrations/versions/fda995215ae9_drop_applyworkflow_overwrite_input.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/syringe.py` & `fractal_server-1.3.0a1/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/tasks/collection.py` & `fractal_server-1.3.0a1/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/fractal_server/utils.py` & `fractal_server-1.3.0a1/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a0/pyproject.toml` & `fractal_server-1.3.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.3.0a0"
+version = "1.3.0a1"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -21,21 +21,22 @@
 fastapi-users = {extras = ["oauth"], version = "^10.1"}
 alembic = "^1.9.1"
 uvicorn = "^0.20.0"
 sqlalchemy = "^1.4"
 SQLAlchemy-Utils = "^0.38.3"
 
 clusterfutures = { version = "^0.5", optional = true}
+cloudpickle = {version = ">=2.2.1 <2.3.0", optional = true}
 
 asyncpg = { version = "^0.27.0", optional = true }
 psycopg2 = { version = "^2.9.5", optional = true }
 gunicorn = { version = "^20.1.0", optional = true }
 
 [tool.poetry.extras]
-slurm = ["clusterfutures"]
+slurm = ["clusterfutures", "cloudpickle"]
 postgres = ["asyncpg", "psycopg2"]
 gunicorn = ["gunicorn"]
 
 [tool.poetry.group.dev.dependencies]
 asgi-lifespan = "^2"
 pytest = "^7.2"
 httpx = "^0.23"
@@ -70,15 +71,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.3.0a0"
+current_version = "1.3.0a1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.3.0a0/setup.py` & `fractal_server-1.3.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,22 @@
  'sqlalchemy>=1.4,<2.0',
  'sqlmodel>=0.0.8,<0.0.9',
  'uvicorn>=0.20.0,<0.21.0']
 
 extras_require = \
 {'gunicorn': ['gunicorn>=20.1.0,<21.0.0'],
  'postgres': ['asyncpg>=0.27.0,<0.28.0', 'psycopg2>=2.9.5,<3.0.0'],
- 'slurm': ['clusterfutures>=0.5,<0.6']}
+ 'slurm': ['clusterfutures>=0.5,<0.6', 'cloudpickle>=2.2.1,<2.3.0']}
 
 entry_points = \
 {'console_scripts': ['fractalctl = fractal_server.__main__:run']}
 
 setup_kwargs = {
     'name': 'fractal-server',
-    'version': '1.3.0a0',
+    'version': '1.3.0a1',
     'description': 'Server component of the Fractal analytics platform',
     'long_description': '# Fractal Server\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high content imaging data at scale and\nprepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nThis is the server component of the fractal analytics platform.\nFind more information about Fractal in general and the other repositories at\nthe [Fractal home page](https://fractal-analytics-platform.github.io).\n\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-server.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are\nreleased according to a BSD 3-Clause License, and Copyright is with Friedrich\nMiescher Institute for Biomedical Research and University of Zurich.\n\nThe SLURM compatibility layer is based on\n[`clusterfutures`](https://github.com/sampsyo/clusterfutures), by\n[@sampsyo](https://github.com/sampsyo) and collaborators, and it is released\nunder the terms of the MIT license.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute\nfor Biomedical Research and in the Pelkmans Lab at the University of Zurich\n(both in Switzerland). The project lead is with\n[@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).\nThe core development is done under contract by\n[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)\n& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-server',
```

### Comparing `fractal_server-1.3.0a0/PKG-INFO` & `fractal_server-1.3.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.3.0a0
+Version: 1.3.0a1
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -15,14 +15,15 @@
 Provides-Extra: gunicorn
 Provides-Extra: postgres
 Provides-Extra: slurm
 Requires-Dist: SQLAlchemy-Utils (>=0.38.3,<0.39.0)
 Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
 Requires-Dist: alembic (>=1.9.1,<2.0.0)
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0) ; extra == "postgres"
+Requires-Dist: cloudpickle (>=2.2.1,<2.3.0) ; extra == "slurm"
 Requires-Dist: clusterfutures (>=0.5,<0.6) ; extra == "slurm"
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: fastapi-users[oauth] (>=10.1,<11.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "gunicorn"
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "postgres"
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
```

