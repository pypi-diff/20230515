# Comparing `tmp/renku-2.4.1rc1.tar.gz` & `tmp/renku-2.4.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renku-2.4.1rc1.tar", max compression
+gzip compressed data, was "renku-2.4.1rc2.tar", max compression
```

## Comparing `renku-2.4.1rc1.tar` & `renku-2.4.1rc2.tar`

### file list

```diff
@@ -1,666 +1,666 @@
--rw-r--r--   0        0        0      900 2023-05-15 07:08:31.983182 renku-2.4.1rc1/AUTHORS.rst
--rw-r--r--   0        0        0   179540 2023-05-15 07:08:31.983182 renku-2.4.1rc1/CHANGES.rst
--rw-r--r--   0        0        0    11358 2023-05-15 07:08:31.983182 renku-2.4.1rc1/LICENSE
--rw-r--r--   0        0        0    12889 2023-05-15 07:08:31.983182 renku-2.4.1rc1/README.rst
--rw-r--r--   0        0        0    10401 2023-05-15 07:09:35.075213 renku-2.4.1rc1/pyproject.toml
--rw-r--r--   0        0        0     4391 2023-05-15 07:08:32.039181 renku-2.4.1rc1/renku/__init__.py
--rw-r--r--   0        0        0      784 2023-05-15 07:08:32.039181 renku-2.4.1rc1/renku/command/__init__.py
--rw-r--r--   0        0        0      209 2023-05-15 07:09:30.315212 renku-2.4.1rc1/renku/command/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      437 2023-05-15 07:09:30.319212 renku-2.4.1rc1/renku/command/__pycache__/options.cpython-39.pyc
--rw-r--r--   0        0        0     1057 2023-05-15 07:09:33.095212 renku-2.4.1rc1/renku/command/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     1343 2023-05-15 07:09:30.319212 renku-2.4.1rc1/renku/command/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0      593 2023-05-15 07:09:30.319212 renku-2.4.1rc1/renku/command/__pycache__/version.cpython-39.pyc
--rw-r--r--   0        0        0     2096 2023-05-15 07:08:32.039181 renku-2.4.1rc1/renku/command/checks/__init__.py
--rw-r--r--   0        0        0     4723 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/checks/activities.py
--rw-r--r--   0        0        0     8186 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/checks/datasets.py
--rw-r--r--   0        0        0     2769 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/checks/githooks.py
--rw-r--r--   0        0        0     1500 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/checks/migration.py
--rw-r--r--   0        0        0     2316 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/checks/project.py
--rw-r--r--   0        0        0     1487 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/checks/storage.py
--rw-r--r--   0        0        0     4262 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/checks/validate_shacl.py
--rw-r--r--   0        0        0     4881 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/checks/workflow.py
--rw-r--r--   0        0        0     3872 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/clone.py
--rw-r--r--   0        0        0      828 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/command_builder/__init__.py
--rw-r--r--   0        0        0      301 2023-05-15 07:09:30.859212 renku-2.4.1rc1/renku/command/command_builder/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    15431 2023-05-15 07:09:30.859212 renku-2.4.1rc1/renku/command/command_builder/__pycache__/command.cpython-39.pyc
--rw-r--r--   0        0        0    16678 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/command_builder/command.py
--rw-r--r--   0        0        0     1951 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/command_builder/communication.py
--rw-r--r--   0        0        0     5325 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/command_builder/database.py
--rw-r--r--   0        0        0     1701 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/command_builder/lock.py
--rw-r--r--   0        0        0     1481 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/command_builder/migration.py
--rw-r--r--   0        0        0     7694 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/command_builder/repo.py
--rw-r--r--   0        0        0     4803 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/config.py
--rw-r--r--   0        0        0     5640 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/dataset.py
--rw-r--r--   0        0        0     2718 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/doctor.py
--rw-r--r--   0        0        0      775 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/format/__init__.py
--rw-r--r--   0        0        0      220 2023-05-15 07:09:30.519212 renku-2.4.1rc1/renku/command/format/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5765 2023-05-15 07:09:30.523212 renku-2.4.1rc1/renku/command/format/__pycache__/dataset_files.cpython-39.pyc
--rw-r--r--   0        0        0     1508 2023-05-15 07:09:30.523212 renku-2.4.1rc1/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc
--rw-r--r--   0        0        0     2884 2023-05-15 07:09:30.523212 renku-2.4.1rc1/renku/command/format/__pycache__/datasets.cpython-39.pyc
--rw-r--r--   0        0        0      817 2023-05-15 07:09:32.347212 renku-2.4.1rc1/renku/command/format/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0     1754 2023-05-15 07:09:33.111212 renku-2.4.1rc1/renku/command/format/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     1929 2023-05-15 07:09:32.347212 renku-2.4.1rc1/renku/command/format/__pycache__/tabulate.cpython-39.pyc
--rw-r--r--   0        0        0     2416 2023-05-15 07:09:32.347212 renku-2.4.1rc1/renku/command/format/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0        0        0     2643 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/format/activity.py
--rw-r--r--   0        0        0     6230 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/format/dataset_files.py
--rw-r--r--   0        0        0     2098 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/format/dataset_tags.py
--rw-r--r--   0        0        0     3236 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/format/datasets.py
--rw-r--r--   0        0        0     1212 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/format/json.py
--rw-r--r--   0        0        0     2402 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/format/session.py
--rw-r--r--   0        0        0     2769 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/format/tabulate.py
--rw-r--r--   0        0        0     2728 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/format/workflow.py
--rw-r--r--   0        0        0     1012 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/gc.py
--rw-r--r--   0        0        0     1154 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/githooks.py
--rw-r--r--   0        0        0     9880 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/graph.py
--rw-r--r--   0        0        0     1081 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/group.py
--rw-r--r--   0        0        0     1203 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/init.py
--rw-r--r--   0        0        0     3124 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/log.py
--rw-r--r--   0        0        0     1241 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/login.py
--rw-r--r--   0        0        0     2822 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/mergetool.py
--rw-r--r--   0        0        0     7621 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/migrate.py
--rw-r--r--   0        0        0     9141 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/move.py
--rw-r--r--   0        0        0     1015 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/options.py
--rw-r--r--   0        0        0     1362 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/project.py
--rw-r--r--   0        0        0     4748 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/remove.py
--rw-r--r--   0        0        0     3146 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/rerun.py
--rw-r--r--   0        0        0    10987 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/rollback.py
--rw-r--r--   0        0        0     1600 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/run.py
--rw-r--r--   0        0        0     3375 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/save.py
--rw-r--r--   0        0        0      766 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/__init__.py
--rw-r--r--   0        0        0      211 2023-05-15 07:09:30.591212 renku-2.4.1rc1/renku/command/schema/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1560 2023-05-15 07:09:30.591212 renku-2.4.1rc1/renku/command/schema/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0      977 2023-05-15 07:09:30.731212 renku-2.4.1rc1/renku/command/schema/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     6652 2023-05-15 07:09:30.723212 renku-2.4.1rc1/renku/command/schema/__pycache__/calamus.cpython-39.pyc
--rw-r--r--   0        0        0     7584 2023-05-15 07:09:30.591212 renku-2.4.1rc1/renku/command/schema/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0     1345 2023-05-15 07:09:30.731212 renku-2.4.1rc1/renku/command/schema/__pycache__/entity.cpython-39.pyc
--rw-r--r--   0        0        0     5615 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/activity.py
--rw-r--r--   0        0        0     1744 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/agent.py
--rw-r--r--   0        0        0     1235 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/annotation.py
--rw-r--r--   0        0        0     8986 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/calamus.py
--rw-r--r--   0        0        0     3186 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/composite_plan.py
--rw-r--r--   0        0        0     8210 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/dataset.py
--rw-r--r--   0        0        0     1445 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/entity.py
--rw-r--r--   0        0        0     4016 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/parameter.py
--rw-r--r--   0        0        0     3427 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/plan.py
--rw-r--r--   0        0        0     3406 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/project.py
--rw-r--r--   0        0        0     1829 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/schema/workflow_file.py
--rw-r--r--   0        0        0     1578 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/session.py
--rw-r--r--   0        0        0     1036 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/status.py
--rw-r--r--   0        0        0     3944 2023-05-15 07:08:32.043181 renku-2.4.1rc1/renku/command/storage.py
--rw-r--r--   0        0        0     1919 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/template.py
--rw-r--r--   0        0        0     1254 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/update.py
--rw-r--r--   0        0        0     1726 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/util.py
--rw-r--r--   0        0        0     1088 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/version.py
--rw-r--r--   0        0        0      768 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/__init__.py
--rw-r--r--   0        0        0      217 2023-05-15 07:09:32.347212 renku-2.4.1rc1/renku/command/view_model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13077 2023-05-15 07:09:32.351212 renku-2.4.1rc1/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc
--rw-r--r--   0        0        0     1350 2023-05-15 07:09:32.383212 renku-2.4.1rc1/renku/command/view_model/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0     8157 2023-05-15 07:09:32.383212 renku-2.4.1rc1/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc
--rw-r--r--   0        0        0    11145 2023-05-15 07:09:33.059212 renku-2.4.1rc1/renku/command/view_model/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0     7823 2023-05-15 07:09:32.379212 renku-2.4.1rc1/renku/command/view_model/__pycache__/plan.cpython-39.pyc
--rw-r--r--   0        0        0    13979 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/activity_graph.py
--rw-r--r--   0        0        0     1657 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/agent.py
--rw-r--r--   0        0        0     8768 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/composite_plan.py
--rw-r--r--   0        0        0     2138 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/dataset.py
--rw-r--r--   0        0        0     7772 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/graph.py
--rw-r--r--   0        0        0    12497 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/log.py
--rw-r--r--   0        0        0     9377 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/plan.py
--rw-r--r--   0        0        0     3306 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/project.py
--rw-r--r--   0        0        0     5947 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/template.py
--rw-r--r--   0        0        0    14502 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/text_canvas.py
--rw-r--r--   0        0        0     4792 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/view_model/workflow_file.py
--rw-r--r--   0        0        0     4114 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/command/workflow.py
--rw-r--r--   0        0        0      745 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/__init__.py
--rw-r--r--   0        0        0      180 2023-05-15 07:09:30.319212 renku-2.4.1rc1/renku/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4501 2023-05-15 07:09:30.775212 renku-2.4.1rc1/renku/core/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     1707 2023-05-15 07:09:30.327212 renku-2.4.1rc1/renku/core/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0    34603 2023-05-15 07:09:30.323212 renku-2.4.1rc1/renku/core/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     4854 2023-05-15 07:09:32.387212 renku-2.4.1rc1/renku/core/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0     8039 2023-05-15 07:09:30.867212 renku-2.4.1rc1/renku/core/__pycache__/login.cpython-39.pyc
--rw-r--r--   0        0        0    16201 2023-05-15 07:09:30.839212 renku-2.4.1rc1/renku/core/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0        0        0     6170 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/config.py
--rw-r--r--   0        0        0     2717 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/constant.py
--rw-r--r--   0        0        0      765 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/__init__.py
--rw-r--r--   0        0        0      208 2023-05-15 07:09:30.523212 renku-2.4.1rc1/renku/core/dataset/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7431 2023-05-15 07:09:30.855212 renku-2.4.1rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc
--rw-r--r--   0        0        0     2954 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/context.py
--rw-r--r--   0        0        0    54038 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/dataset.py
--rw-r--r--   0        0        0    21429 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/dataset_add.py
--rw-r--r--   0        0        0     9747 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/datasets_provenance.py
--rw-r--r--   0        0        0     4296 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/pointer_file.py
--rw-r--r--   0        0        0      760 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/__init__.py
--rw-r--r--   0        0        0      213 2023-05-15 07:09:30.527212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    15669 2023-05-15 07:09:30.527212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc
--rw-r--r--   0        0        0     6716 2023-05-15 07:09:30.543212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc
--rw-r--r--   0        0        0     1646 2023-05-15 07:09:30.543212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc
--rw-r--r--   0        0        0    19281 2023-05-15 07:09:30.827211 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc
--rw-r--r--   0        0        0     2797 2023-05-15 07:09:30.827211 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc
--rw-r--r--   0        0        0     5069 2023-05-15 07:09:30.831212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc
--rw-r--r--   0        0        0     5945 2023-05-15 07:09:30.831212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc
--rw-r--r--   0        0        0     5562 2023-05-15 07:09:30.527212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0        0        0     5966 2023-05-15 07:09:30.835212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0     9328 2023-05-15 07:09:30.851212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc
--rw-r--r--   0        0        0     6028 2023-05-15 07:09:30.543212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     9555 2023-05-15 07:09:30.851212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc
--rw-r--r--   0        0        0    17162 2023-05-15 07:09:30.855212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc
--rw-r--r--   0        0        0     2538 2023-05-15 07:09:30.831212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc
--rw-r--r--   0        0        0     6242 2023-05-15 07:09:30.923212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc
--rw-r--r--   0        0        0     4868 2023-05-15 07:09:30.923212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc
--rw-r--r--   0        0        0    17896 2023-05-15 07:09:30.931212 renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc
--rw-r--r--   0        0        0    12028 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/api.py
--rw-r--r--   0        0        0     6966 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/azure.py
--rw-r--r--   0        0        0     2225 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/common.py
--rw-r--r--   0        0        0    20652 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/dataverse.py
--rw-r--r--   0        0        0     3317 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/dataverse_metadata_templates.py
--rw-r--r--   0        0        0     4808 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/doi.py
--rw-r--r--   0        0        0     5602 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/external.py
--rw-r--r--   0        0        0     5764 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/factory.py
--rw-r--r--   0        0        0     7300 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/git.py
--rw-r--r--   0        0        0    11965 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/local.py
--rw-r--r--   0        0        0     5869 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/models.py
--rw-r--r--   0        0        0    10097 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/olos.py
--rw-r--r--   0        0        0    22146 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/renku.py
--rw-r--r--   0        0        0     2553 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/repository.py
--rw-r--r--   0        0        0     6392 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/s3.py
--rw-r--r--   0        0        0     5813 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/web.py
--rw-r--r--   0        0        0    18624 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/providers/zenodo.py
--rw-r--r--   0        0        0     3973 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/request_model.py
--rw-r--r--   0        0        0     5361 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/dataset/tag.py
--rw-r--r--   0        0        0    25658 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/errors.py
--rw-r--r--   0        0        0     1115 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/gc.py
--rw-r--r--   0        0        0     7394 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/git.py
--rw-r--r--   0        0        0     2151 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/githooks.py
--rw-r--r--   0        0        0    16526 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/init.py
--rw-r--r--   0        0        0      775 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/interface/__init__.py
--rw-r--r--   0        0        0      207 2023-05-15 07:09:30.823212 renku-2.4.1rc1/renku/core/interface/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4269 2023-05-15 07:09:32.351212 renku-2.4.1rc1/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     1246 2023-05-15 07:09:32.387212 renku-2.4.1rc1/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     2159 2023-05-15 07:09:30.863211 renku-2.4.1rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     2057 2023-05-15 07:09:32.339212 renku-2.4.1rc1/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc
--rw-r--r--   0        0        0      959 2023-05-15 07:09:32.339212 renku-2.4.1rc1/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     4402 2023-05-15 07:09:30.823212 renku-2.4.1rc1/renku/core/interface/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0        0        0     1579 2023-05-15 07:09:32.267212 renku-2.4.1rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc
--rw-r--r--   0        0        0     3741 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/interface/activity_gateway.py
--rw-r--r--   0        0        0     1418 2023-05-15 07:08:32.047181 renku-2.4.1rc1/renku/core/interface/database_gateway.py
--rw-r--r--   0        0        0     2095 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/interface/dataset_gateway.py
--rw-r--r--   0        0        0     1996 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/interface/plan_gateway.py
--rw-r--r--   0        0        0     1212 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/interface/project_gateway.py
--rw-r--r--   0        0        0     4226 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/interface/storage.py
--rw-r--r--   0        0        0     1780 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/interface/workflow_file_parser.py
--rw-r--r--   0        0        0    10639 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/login.py
--rw-r--r--   0        0        0      764 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/__init__.py
--rw-r--r--   0        0        0      196 2023-05-15 07:09:30.775212 renku-2.4.1rc1/renku/core/migration/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1122 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0003__0_pyld2.py
--rw-r--r--   0        0        0    15324 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0003__1_jsonld.py
--rw-r--r--   0        0        0     9570 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0003__2_initial.py
--rw-r--r--   0        0        0     1122 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0004__0_pyld2.py
--rw-r--r--   0        0        0     5318 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0004__submodules.py
--rw-r--r--   0        0        0     1548 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0005__1_pyld2.py
--rw-r--r--   0        0        0    16122 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0005__2_cwl.py
--rw-r--r--   0        0        0     1015 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0006__dataset_context.py
--rw-r--r--   0        0        0     1430 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0007__source_url.py
--rw-r--r--   0        0        0     1175 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0008__dataset_metadata.py
--rw-r--r--   0        0        0    30683 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0009__new_metadata_storage.py
--rw-r--r--   0        0        0    14077 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/m_0010__metadata_fixes.py
--rw-r--r--   0        0        0    10119 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/migrate.py
--rw-r--r--   0        0        0      770 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/models/__init__.py
--rw-r--r--   0        0        0     5830 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/models/migration.py
--rw-r--r--   0        0        0     3861 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/models/refs.py
--rw-r--r--   0        0        0     5091 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/models/v10.py
--rw-r--r--   0        0        0    11828 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/models/v3.py
--rw-r--r--   0        0        0     2422 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/models/v7.py
--rw-r--r--   0        0        0     4587 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/models/v8.py
--rw-r--r--   0        0        0    74088 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/models/v9.py
--rw-r--r--   0        0        0     7865 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/utils/__init__.py
--rw-r--r--   0        0        0     6558 2023-05-15 07:09:30.775212 renku-2.4.1rc1/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8121 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/migration/utils/conversion.py
--rw-r--r--   0        0        0      824 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/plugin/__init__.py
--rw-r--r--   0        0        0      265 2023-05-15 07:09:30.527212 renku-2.4.1rc1/renku/core/plugin/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1033 2023-05-15 07:09:30.539212 renku-2.4.1rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc
--rw-r--r--   0        0        0     1049 2023-05-15 07:09:30.539212 renku-2.4.1rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc
--rw-r--r--   0        0        0     3246 2023-05-15 07:09:31.587211 renku-2.4.1rc1/renku/core/plugin/__pycache__/provider.cpython-39.pyc
--rw-r--r--   0        0        0     1467 2023-05-15 07:09:33.019212 renku-2.4.1rc1/renku/core/plugin/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0      985 2023-05-15 07:09:33.115212 renku-2.4.1rc1/renku/core/plugin/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     4177 2023-05-15 07:09:32.739212 renku-2.4.1rc1/renku/core/plugin/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0        0        0     2978 2023-05-15 07:09:32.355212 renku-2.4.1rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc
--rw-r--r--   0        0        0     1467 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/plugin/dataset_provider.py
--rw-r--r--   0        0        0     3046 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/plugin/implementations/__init__.py
--rw-r--r--   0        0        0     2540 2023-05-15 07:09:30.543212 renku-2.4.1rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1790 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/plugin/pluginmanager.py
--rw-r--r--   0        0        0     3357 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/plugin/provider.py
--rw-r--r--   0        0        0     1839 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/plugin/run.py
--rw-r--r--   0        0        0     1454 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/plugin/session.py
--rw-r--r--   0        0        0     4195 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/plugin/workflow.py
--rw-r--r--   0        0        0     3065 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/plugin/workflow_file_parser.py
--rw-r--r--   0        0        0     3355 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/project.py
--rw-r--r--   0        0        0      780 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/session/__init__.py
--rw-r--r--   0        0        0      210 2023-05-15 07:09:30.931212 renku-2.4.1rc1/renku/core/session/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11692 2023-05-15 07:09:30.931212 renku-2.4.1rc1/renku/core/session/__pycache__/docker.cpython-39.pyc
--rw-r--r--   0        0        0    15989 2023-05-15 07:09:31.079212 renku-2.4.1rc1/renku/core/session/__pycache__/renkulab.cpython-39.pyc
--rw-r--r--   0        0        0     1449 2023-05-15 07:09:31.083212 renku-2.4.1rc1/renku/core/session/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0    14350 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/session/docker.py
--rw-r--r--   0        0        0    20534 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/session/renkulab.py
--rw-r--r--   0        0        0    11815 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/session/session.py
--rw-r--r--   0        0        0     2215 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/session/utils.py
--rw-r--r--   0        0        0    21861 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/storage.py
--rw-r--r--   0        0        0      760 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/template/__init__.py
--rw-r--r--   0        0        0    22043 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/template/template.py
--rw-r--r--   0        0        0    14612 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/template/usecase.py
--rw-r--r--   0        0        0      756 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/util/__init__.py
--rw-r--r--   0        0        0      196 2023-05-15 07:09:30.327212 renku-2.4.1rc1/renku/core/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11124 2023-05-15 07:09:30.539212 renku-2.4.1rc1/renku/core/util/__pycache__/communication.cpython-39.pyc
--rw-r--r--   0        0        0     6320 2023-05-15 07:09:32.387212 renku-2.4.1rc1/renku/core/util/__pycache__/contexts.cpython-39.pyc
--rw-r--r--   0        0        0     1801 2023-05-15 07:09:30.771211 renku-2.4.1rc1/renku/core/util/__pycache__/datetime8601.cpython-39.pyc
--rw-r--r--   0        0        0      933 2023-05-15 07:09:30.539212 renku-2.4.1rc1/renku/core/util/__pycache__/doi.cpython-39.pyc
--rw-r--r--   0        0        0    33652 2023-05-15 07:09:30.335212 renku-2.4.1rc1/renku/core/util/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0      669 2023-05-15 07:09:31.103211 renku-2.4.1rc1/renku/core/util/__pycache__/jwt.cpython-39.pyc
--rw-r--r--   0        0        0     6008 2023-05-15 07:09:30.771211 renku-2.4.1rc1/renku/core/util/__pycache__/metadata.cpython-39.pyc
--rw-r--r--   0        0        0    11013 2023-05-15 07:09:30.499212 renku-2.4.1rc1/renku/core/util/__pycache__/os.cpython-39.pyc
--rw-r--r--   0        0        0     6893 2023-05-15 07:09:31.083212 renku-2.4.1rc1/renku/core/util/__pycache__/requests.cpython-39.pyc
--rw-r--r--   0        0        0     5971 2023-05-15 07:09:31.155212 renku-2.4.1rc1/renku/core/util/__pycache__/ssh.cpython-39.pyc
--rw-r--r--   0        0        0     4943 2023-05-15 07:09:30.779212 renku-2.4.1rc1/renku/core/util/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0        0        0     3737 2023-05-15 07:09:30.923212 renku-2.4.1rc1/renku/core/util/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     2663 2023-05-15 07:09:30.775212 renku-2.4.1rc1/renku/core/util/__pycache__/yaml.cpython-39.pyc
--rw-r--r--   0        0        0    10282 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/util/communication.py
--rw-r--r--   0        0        0     6617 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/util/contexts.py
--rw-r--r--   0        0        0     2313 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/util/datetime8601.py
--rw-r--r--   0        0        0     1376 2023-05-15 07:08:32.051181 renku-2.4.1rc1/renku/core/util/doi.py
--rw-r--r--   0        0        0    40689 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/git.py
--rw-r--r--   0        0        0     1244 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/jwt.py
--rw-r--r--   0        0        0     7036 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/metadata.py
--rw-r--r--   0        0        0    12140 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/os.py
--rw-r--r--   0        0        0     7626 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/requests.py
--rw-r--r--   0        0        0     1611 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/shacl.py
--rw-r--r--   0        0        0     6871 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/ssh.py
--rw-r--r--   0        0        0     2158 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/tabulate.py
--rw-r--r--   0        0        0     6228 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/urls.py
--rw-r--r--   0        0        0     3878 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/util.py
--rw-r--r--   0        0        0     2836 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/util/yaml.py
--rw-r--r--   0        0        0      773 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/__init__.py
--rw-r--r--   0        0        0      204 2023-05-15 07:09:31.155212 renku-2.4.1rc1/renku/core/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    18165 2023-05-15 07:09:32.391212 renku-2.4.1rc1/renku/core/workflow/__pycache__/activity.cpython-39.pyc
--rw-r--r--   0        0        0    14583 2023-05-15 07:09:33.099212 renku-2.4.1rc1/renku/core/workflow/__pycache__/execute.cpython-39.pyc
--rw-r--r--   0        0        0    26495 2023-05-15 07:09:32.343212 renku-2.4.1rc1/renku/core/workflow/__pycache__/plan.cpython-39.pyc
--rw-r--r--   0        0        0    23623 2023-05-15 07:09:32.399212 renku-2.4.1rc1/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc
--rw-r--r--   0        0        0    10067 2023-05-15 07:09:32.379212 renku-2.4.1rc1/renku/core/workflow/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     1660 2023-05-15 07:09:32.399212 renku-2.4.1rc1/renku/core/workflow/__pycache__/types.cpython-39.pyc
--rw-r--r--   0        0        0     8676 2023-05-15 07:09:32.359212 renku-2.4.1rc1/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc
--rw-r--r--   0        0        0     4780 2023-05-15 07:09:33.099212 renku-2.4.1rc1/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc
--rw-r--r--   0        0        0    22713 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/activity.py
--rw-r--r--   0        0        0      773 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/converters/__init__.py
--rw-r--r--   0        0        0      215 2023-05-15 07:09:31.155212 renku-2.4.1rc1/renku/core/workflow/converters/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11073 2023-05-15 07:09:31.159211 renku-2.4.1rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc
--rw-r--r--   0        0        0     4668 2023-05-15 07:09:32.263212 renku-2.4.1rc1/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc
--rw-r--r--   0        0        0    17930 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/converters/cwl.py
--rw-r--r--   0        0        0     5142 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/converters/renku.py
--rw-r--r--   0        0        0    18756 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/execute.py
--rw-r--r--   0        0        0      769 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/model/__init__.py
--rw-r--r--   0        0        0      206 2023-05-15 07:09:31.587211 renku-2.4.1rc1/renku/core/workflow/model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4825 2023-05-15 07:09:31.587211 renku-2.4.1rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc
--rw-r--r--   0        0        0    26172 2023-05-15 07:09:32.275212 renku-2.4.1rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc
--rw-r--r--   0        0        0     6530 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/model/concrete_execution_graph.py
--rw-r--r--   0        0        0    37866 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/model/workflow_file.py
--rw-r--r--   0        0        0      775 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/parser/__init__.py
--rw-r--r--   0        0        0      213 2023-05-15 07:09:32.263212 renku-2.4.1rc1/renku/core/workflow/parser/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8620 2023-05-15 07:09:32.267212 renku-2.4.1rc1/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc
--rw-r--r--   0        0        0    10631 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/parser/renku.py
--rw-r--r--   0        0        0    34209 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/plan.py
--rw-r--r--   0        0        0    33046 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/plan_factory.py
--rw-r--r--   0        0        0      772 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/providers/__init__.py
--rw-r--r--   0        0        0      213 2023-05-15 07:09:32.403212 renku-2.4.1rc1/renku/core/workflow/providers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4631 2023-05-15 07:09:32.407212 renku-2.4.1rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc
--rw-r--r--   0        0        0     3918 2023-05-15 07:09:32.739212 renku-2.4.1rc1/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc
--rw-r--r--   0        0        0    11194 2023-05-15 07:09:32.743212 renku-2.4.1rc1/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc
--rw-r--r--   0        0        0     5999 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/providers/cwltool.py
--rw-r--r--   0        0        0     4271 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/providers/local.py
--rw-r--r--   0        0        0    13372 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/providers/toil.py
--rw-r--r--   0        0        0    13562 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/run.py
--rw-r--r--   0        0        0     1681 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/types.py
--rw-r--r--   0        0        0     2869 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/update.py
--rw-r--r--   0        0        0     8335 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/value_resolution.py
--rw-r--r--   0        0        0     5089 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/core/workflow/workflow_file.py
--rw-r--r--   0        0        0      767 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/data/__init__.py
--rw-r--r--   0        0        0      114 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/data/defaults.ini
--rw-r--r--   0        0        0     3364 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/data/gitignore.default
--rwxr-xr-x   0        0        0     4372 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/data/pre-commit.sh
--rw-r--r--   0        0        0    48383 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/data/shacl_shape.json
--rw-r--r--   0        0        0      767 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/__init__.py
--rw-r--r--   0        0        0      210 2023-05-15 07:09:30.503212 renku-2.4.1rc1/renku/domain_model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      388 2023-05-15 07:09:30.523212 renku-2.4.1rc1/renku/domain_model/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0    26291 2023-05-15 07:09:30.739212 renku-2.4.1rc1/renku/domain_model/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0      988 2023-05-15 07:09:30.535212 renku-2.4.1rc1/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc
--rw-r--r--   0        0        0     2204 2023-05-15 07:09:32.399212 renku-2.4.1rc1/renku/domain_model/__pycache__/datastructures.cpython-39.pyc
--rw-r--r--   0        0        0     2539 2023-05-15 07:09:30.731212 renku-2.4.1rc1/renku/domain_model/__pycache__/entity.cpython-39.pyc
--rw-r--r--   0        0        0      575 2023-05-15 07:09:30.775212 renku-2.4.1rc1/renku/domain_model/__pycache__/enums.cpython-39.pyc
--rw-r--r--   0        0        0     6097 2023-05-15 07:09:32.259212 renku-2.4.1rc1/renku/domain_model/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0    12164 2023-05-15 07:09:30.507212 renku-2.4.1rc1/renku/domain_model/__pycache__/project_context.cpython-39.pyc
--rw-r--r--   0        0        0     7196 2023-05-15 07:09:31.079212 renku-2.4.1rc1/renku/domain_model/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     1092 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/constant.py
--rw-r--r--   0        0        0    29605 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/dataset.py
--rw-r--r--   0        0        0     1267 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/dataset_provider.py
--rw-r--r--   0        0        0     2754 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/datastructures.py
--rw-r--r--   0        0        0     2499 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/entity.py
--rw-r--r--   0        0        0      971 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/enums.py
--rw-r--r--   0        0        0     5059 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/git.py
--rw-r--r--   0        0        0     8329 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/project.py
--rw-r--r--   0        0        0    11817 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/project_context.py
--rw-r--r--   0        0        0      829 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/provenance/__init__.py
--rw-r--r--   0        0        0      283 2023-05-15 07:09:30.727212 renku-2.4.1rc1/renku/domain_model/provenance/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11882 2023-05-15 07:09:32.351212 renku-2.4.1rc1/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc
--rw-r--r--   0        0        0     4946 2023-05-15 07:09:30.731212 renku-2.4.1rc1/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0     1092 2023-05-15 07:09:30.731212 renku-2.4.1rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     1363 2023-05-15 07:09:32.355212 renku-2.4.1rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc
--rw-r--r--   0        0        0    13200 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/provenance/activity.py
--rw-r--r--   0        0        0     5155 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/provenance/agent.py
--rw-r--r--   0        0        0     1268 2023-05-15 07:08:32.055181 renku-2.4.1rc1/renku/domain_model/provenance/annotation.py
--rw-r--r--   0        0        0     1530 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/provenance/parameter.py
--rw-r--r--   0        0        0     6701 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/session.py
--rw-r--r--   0        0        0     1471 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/sort.py
--rw-r--r--   0        0        0    27042 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/template.py
--rw-r--r--   0        0        0      782 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/workflow/__init__.py
--rw-r--r--   0        0        0      234 2023-05-15 07:09:31.587211 renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13527 2023-05-15 07:09:31.971212 renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc
--rw-r--r--   0        0        0    15243 2023-05-15 07:09:31.975211 renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc
--rw-r--r--   0        0        0    15096 2023-05-15 07:09:31.979211 renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc
--rw-r--r--   0        0        0     1483 2023-05-15 07:09:31.587211 renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc
--rw-r--r--   0        0        0     4413 2023-05-15 07:09:32.355212 renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc
--rw-r--r--   0        0        0    15917 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/workflow/composite_plan.py
--rw-r--r--   0        0        0     1531 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/workflow/converters/__init__.py
--rw-r--r--   0        0        0     1391 2023-05-15 07:09:32.263212 renku-2.4.1rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    18124 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/workflow/parameter.py
--rw-r--r--   0        0        0    16602 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/workflow/plan.py
--rw-r--r--   0        0        0     1639 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/workflow/provider.py
--rw-r--r--   0        0        0     4349 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/domain_model/workflow/workflow_file.py
--rw-r--r--   0        0        0      780 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/__init__.py
--rw-r--r--   0        0        0      212 2023-05-15 07:09:30.335212 renku-2.4.1rc1/renku/infrastructure/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    34957 2023-05-15 07:09:32.087211 renku-2.4.1rc1/renku/infrastructure/__pycache__/database.cpython-39.pyc
--rw-r--r--   0        0        0     5073 2023-05-15 07:09:30.523212 renku-2.4.1rc1/renku/infrastructure/__pycache__/immutable.cpython-39.pyc
--rw-r--r--   0        0        0     2259 2023-05-15 07:09:30.779212 renku-2.4.1rc1/renku/infrastructure/__pycache__/persistent.cpython-39.pyc
--rw-r--r--   0        0        0    67759 2023-05-15 07:09:30.351212 renku-2.4.1rc1/renku/infrastructure/__pycache__/repository.cpython-39.pyc
--rw-r--r--   0        0        0    41333 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/database.py
--rw-r--r--   0        0        0      786 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/gateway/__init__.py
--rw-r--r--   0        0        0    12730 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/gateway/activity_gateway.py
--rw-r--r--   0        0        0     5845 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/gateway/database_gateway.py
--rw-r--r--   0        0        0     3743 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/gateway/dataset_gateway.py
--rw-r--r--   0        0        0     3529 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/gateway/plan_gateway.py
--rw-r--r--   0        0        0     1711 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/gateway/project_gateway.py
--rw-r--r--   0        0        0    18006 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/git_merger.py
--rw-r--r--   0        0        0     4969 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/immutable.py
--rw-r--r--   0        0        0     2394 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/persistent.py
--rw-r--r--   0        0        0    71947 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/repository.py
--rw-r--r--   0        0        0      784 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/storage/__init__.py
--rw-r--r--   0        0        0      224 2023-05-15 07:09:30.823212 renku-2.4.1rc1/renku/infrastructure/storage/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1523 2023-05-15 07:09:30.823212 renku-2.4.1rc1/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0        0        0     1989 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/storage/factory.py
--rw-r--r--   0        0        0     8859 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/infrastructure/storage/rclone.py
--rw-r--r--   0        0        0      913 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      553 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      637 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      523 2023-05-15 07:09:34.187212 renku-2.4.1rc1/renku/templates/.github/dependabot.yml
--rw-r--r--   0        0        0      396 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/.github/workflows/github-project.yml
--rw-r--r--   0        0        0     3940 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/.gitignore
--rw-r--r--   0        0        0       27 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       37 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      984 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2087 2023-05-15 07:09:34.187212 renku-2.4.1rc1/renku/templates/R-minimal/Dockerfile
--rw-r--r--   0        0        0     1603 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/README.md
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/environment.yml
--rw-r--r--   0        0        0      360 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/install.R
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0      205 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal/{{ __sanitized_project_name__ }}.Rproj
--rw-r--r--   0        0        0    14286 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/R-minimal.png
--rw-r--r--   0        0        0     4846 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/README.md
--rw-r--r--   0        0        0       27 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       37 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2077 2023-05-15 07:09:34.187212 renku-2.4.1rc1/renku/templates/bioc-minimal/Dockerfile
--rw-r--r--   0        0        0     1603 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/README.md
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/install.R
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0      205 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioc-minimal/{{ __sanitized_project_name__ }}.Rproj
--rw-r--r--   0        0        0    44589 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/bioconductor.png
--rw-r--r--   0        0        0       27 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/julia-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/julia-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/julia-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       50 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/julia-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-05-15 07:09:34.179212 renku-2.4.1rc1/renku/templates/julia-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2469 2023-05-15 07:09:34.187212 renku-2.4.1rc1/renku/templates/julia-minimal/Dockerfile
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/julia-minimal/Manifest.toml
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/julia-minimal/Project.toml
--rw-r--r--   0        0        0     1842 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/julia-minimal/README.md
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/julia-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/julia-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/julia-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/julia-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0    13782 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/julialang.png
--rw-r--r--   0        0        0     1174 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/manifest.yaml
--rw-r--r--   0        0        0       17 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/minimal/.dockerignore
--rw-r--r--   0        0        0       77 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       33 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/minimal/.renkulfsignore
--rw-r--r--   0        0        0     2414 2023-05-15 07:09:34.187212 renku-2.4.1rc1/renku/templates/minimal/Dockerfile
--rw-r--r--   0        0        0     1439 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0       27 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/.dockerignore
--rw-r--r--   0        0        0     5401 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       33 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2159 2023-05-15 07:09:34.187212 renku-2.4.1rc1/renku/templates/python-minimal/Dockerfile
--rw-r--r--   0        0        0     1597 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/README.md
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0    25599 2023-05-15 07:09:34.183212 renku-2.4.1rc1/renku/templates/python-minimal.png
--rw-r--r--   0        0        0      763 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/__init__.py
--rw-r--r--   0        0        0      184 2023-05-15 07:09:30.207212 renku-2.4.1rc1/renku/ui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1268 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/__init__.py
--rw-r--r--   0        0        0      763 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/graph/__init__.py
--rw-r--r--   0        0        0     2519 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/graph/rdf.py
--rw-r--r--   0        0        0      764 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/models/__init__.py
--rw-r--r--   0        0        0    16448 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/models/activity.py
--rw-r--r--   0        0        0     4648 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/models/dataset.py
--rw-r--r--   0        0        0    10361 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/models/parameter.py
--rw-r--r--   0        0        0     9227 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/models/plan.py
--rw-r--r--   0        0        0     3643 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/models/project.py
--rw-r--r--   0        0        0     2519 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/api/util.py
--rw-r--r--   0        0        0     9319 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/cli/__init__.py
--rw-r--r--   0        0        0      922 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/cli/__main__.py
--rw-r--r--   0        0        0     8150 2023-05-15 07:09:30.207212 renku-2.4.1rc1/renku/ui/cli/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2117 2023-05-15 07:09:30.507212 renku-2.4.1rc1/renku/ui/cli/__pycache__/clone.cpython-39.pyc
--rw-r--r--   0        0        0     7029 2023-05-15 07:09:30.511212 renku-2.4.1rc1/renku/ui/cli/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0    36528 2023-05-15 07:09:30.515212 renku-2.4.1rc1/renku/ui/cli/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0     1698 2023-05-15 07:09:33.039212 renku-2.4.1rc1/renku/ui/cli/__pycache__/doctor.cpython-39.pyc
--rw-r--r--   0        0        0      964 2023-05-15 07:09:33.039212 renku-2.4.1rc1/renku/ui/cli/__pycache__/env.cpython-39.pyc
--rw-r--r--   0        0        0     7957 2023-05-15 07:09:33.043212 renku-2.4.1rc1/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc
--rw-r--r--   0        0        0      645 2023-05-15 07:09:33.051212 renku-2.4.1rc1/renku/ui/cli/__pycache__/gc.cpython-39.pyc
--rw-r--r--   0        0        0     2168 2023-05-15 07:09:33.055212 renku-2.4.1rc1/renku/ui/cli/__pycache__/githooks.cpython-39.pyc
--rw-r--r--   0        0        0     4041 2023-05-15 07:09:33.055212 renku-2.4.1rc1/renku/ui/cli/__pycache__/graph.cpython-39.pyc
--rw-r--r--   0        0        0     9637 2023-05-15 07:09:33.055212 renku-2.4.1rc1/renku/ui/cli/__pycache__/init.cpython-39.pyc
--rw-r--r--   0        0        0     7264 2023-05-15 07:09:33.055212 renku-2.4.1rc1/renku/ui/cli/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0     4296 2023-05-15 07:09:33.063212 renku-2.4.1rc1/renku/ui/cli/__pycache__/login.cpython-39.pyc
--rw-r--r--   0        0        0     2066 2023-05-15 07:09:33.091212 renku-2.4.1rc1/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc
--rw-r--r--   0        0        0     4435 2023-05-15 07:09:33.091212 renku-2.4.1rc1/renku/ui/cli/__pycache__/migrate.cpython-39.pyc
--rw-r--r--   0        0        0     2306 2023-05-15 07:09:33.091212 renku-2.4.1rc1/renku/ui/cli/__pycache__/move.cpython-39.pyc
--rw-r--r--   0        0        0     4028 2023-05-15 07:09:33.091212 renku-2.4.1rc1/renku/ui/cli/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0     1283 2023-05-15 07:09:33.091212 renku-2.4.1rc1/renku/ui/cli/__pycache__/remove.cpython-39.pyc
--rw-r--r--   0        0        0     3485 2023-05-15 07:09:33.095212 renku-2.4.1rc1/renku/ui/cli/__pycache__/rerun.cpython-39.pyc
--rw-r--r--   0        0        0     2761 2023-05-15 07:09:33.095212 renku-2.4.1rc1/renku/ui/cli/__pycache__/rollback.cpython-39.pyc
--rw-r--r--   0        0        0    23646 2023-05-15 07:09:33.095212 renku-2.4.1rc1/renku/ui/cli/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     2890 2023-05-15 07:09:33.107212 renku-2.4.1rc1/renku/ui/cli/__pycache__/save.cpython-39.pyc
--rw-r--r--   0        0        0    10307 2023-05-15 07:09:33.111212 renku-2.4.1rc1/renku/ui/cli/__pycache__/service.cpython-39.pyc
--rw-r--r--   0        0        0    12372 2023-05-15 07:09:33.111212 renku-2.4.1rc1/renku/ui/cli/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     3715 2023-05-15 07:09:33.115212 renku-2.4.1rc1/renku/ui/cli/__pycache__/status.cpython-39.pyc
--rw-r--r--   0        0        0     5061 2023-05-15 07:09:33.115212 renku-2.4.1rc1/renku/ui/cli/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0        0        0    10944 2023-05-15 07:09:33.119212 renku-2.4.1rc1/renku/ui/cli/__pycache__/template.cpython-39.pyc
--rw-r--r--   0        0        0     5790 2023-05-15 07:09:33.119212 renku-2.4.1rc1/renku/ui/cli/__pycache__/update.cpython-39.pyc
--rw-r--r--   0        0        0    41957 2023-05-15 07:09:33.123212 renku-2.4.1rc1/renku/ui/cli/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0        0        0     2594 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/cli/clone.py
--rw-r--r--   0        0        0     7953 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/cli/config.py
--rw-r--r--   0        0        0    42970 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/cli/dataset.py
--rw-r--r--   0        0        0     2217 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/cli/doctor.py
--rw-r--r--   0        0        0     1600 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/cli/env.py
--rw-r--r--   0        0        0     7931 2023-05-15 07:08:32.059181 renku-2.4.1rc1/renku/ui/cli/exception_handler.py
--rw-r--r--   0        0        0     1139 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/gc.py
--rw-r--r--   0        0        0     2538 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/githooks.py
--rw-r--r--   0        0        0     4950 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/graph.py
--rw-r--r--   0        0        0    11113 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/init.py
--rw-r--r--   0        0        0     8581 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/log.py
--rw-r--r--   0        0        0     4845 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/login.py
--rw-r--r--   0        0        0     2499 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/mergetool.py
--rw-r--r--   0        0        0     5689 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/migrate.py
--rw-r--r--   0        0        0     2881 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/move.py
--rw-r--r--   0        0        0     5768 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/project.py
--rw-r--r--   0        0        0     1754 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/remove.py
--rw-r--r--   0        0        0     4227 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/rerun.py
--rw-r--r--   0        0        0     3249 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/rollback.py
--rw-r--r--   0        0        0    26417 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/run.py
--rw-r--r--   0        0        0     3510 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/save.py
--rw-r--r--   0        0        0    11830 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/service.py
--rw-r--r--   0        0        0    14005 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/session.py
--rw-r--r--   0        0        0     5489 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/status.py
--rw-r--r--   0        0        0     5604 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/storage.py
--rw-r--r--   0        0        0    13434 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/template.py
--rw-r--r--   0        0        0     6723 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/update.py
--rw-r--r--   0        0        0      768 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/utils/__init__.py
--rw-r--r--   0        0        0      203 2023-05-15 07:09:30.507212 renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5720 2023-05-15 07:09:33.067212 renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc
--rw-r--r--   0        0        0     3433 2023-05-15 07:09:30.511212 renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc
--rw-r--r--   0        0        0      301 2023-05-15 07:09:30.507212 renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/color.cpython-39.pyc
--rw-r--r--   0        0        0      998 2023-05-15 07:09:33.095212 renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc
--rw-r--r--   0        0        0     7369 2023-05-15 07:09:33.063212 renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc
--rw-r--r--   0        0        0     5422 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/utils/callback.py
--rw-r--r--   0        0        0     3982 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/utils/click.py
--rw-r--r--   0        0        0      855 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/utils/color.py
--rw-r--r--   0        0        0    14534 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/utils/curses.py
--rw-r--r--   0        0        0     1387 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/utils/plugins.py
--rw-r--r--   0        0        0     9929 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/utils/terminal.py
--rw-r--r--   0        0        0    48023 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/cli/workflow.py
--rw-r--r--   0        0        0      843 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/.env-example
--rw-r--r--   0        0        0      756 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/__init__.py
--rw-r--r--   0        0        0      189 2023-05-15 07:09:33.043212 renku-2.4.1rc1/renku/ui/service/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2012 2023-05-15 07:09:33.043212 renku-2.4.1rc1/renku/ui/service/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     1535 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/__init__.py
--rw-r--r--   0        0        0     2917 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/base.py
--rw-r--r--   0        0        0     1168 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/config.py
--rw-r--r--   0        0        0     3315 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/files.py
--rw-r--r--   0        0        0     2333 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/jobs.py
--rw-r--r--   0        0        0      769 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/models/__init__.py
--rw-r--r--   0        0        0     4356 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/models/file.py
--rw-r--r--   0        0        0     2273 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/models/job.py
--rw-r--r--   0        0        0     4043 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/models/project.py
--rw-r--r--   0        0        0     1127 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/models/user.py
--rw-r--r--   0        0        0     2558 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/projects.py
--rw-r--r--   0        0        0      774 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/serializers/__init__.py
--rw-r--r--   0        0        0     1821 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/serializers/file.py
--rw-r--r--   0        0        0     1711 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/serializers/job.py
--rw-r--r--   0        0        0     1812 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/serializers/project.py
--rw-r--r--   0        0        0     1227 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/serializers/user.py
--rw-r--r--   0        0        0     1657 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/cache/users.py
--rw-r--r--   0        0        0     2931 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/config.py
--rw-r--r--   0        0        0      773 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/controllers/__init__.py
--rw-r--r--   0        0        0      777 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/controllers/api/__init__.py
--rw-r--r--   0        0        0     1085 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/controllers/api/abstract.py
--rw-r--r--   0        0        0    15626 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/controllers/api/mixins.py
--rw-r--r--   0        0        0     2647 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/controllers/cache_files_delete_chunks.py
--rw-r--r--   0        0        0     7478 2023-05-15 07:08:32.063181 renku-2.4.1rc1/renku/ui/service/controllers/cache_files_upload.py
--rw-r--r--   0        0        0     2239 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/cache_list_projects.py
--rw-r--r--   0        0        0     1927 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/cache_list_uploaded.py
--rw-r--r--   0        0        0     4823 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/cache_migrate_project.py
--rw-r--r--   0        0        0     5110 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/cache_migrations_check.py
--rw-r--r--   0        0        0     2350 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/cache_project_clone.py
--rw-r--r--   0        0        0     2649 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/config_set.py
--rw-r--r--   0        0        0     2333 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/config_show.py
--rw-r--r--   0        0        0     5682 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/datasets_add_file.py
--rw-r--r--   0        0        0     3916 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/datasets_create.py
--rw-r--r--   0        0        0     5359 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/datasets_edit.py
--rw-r--r--   0        0        0     2132 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/datasets_files_list.py
--rw-r--r--   0        0        0     3333 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/datasets_import.py
--rw-r--r--   0        0        0     2065 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/datasets_list.py
--rw-r--r--   0        0        0     2637 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/datasets_remove.py
--rw-r--r--   0        0        0     3290 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/datasets_unlink.py
--rw-r--r--   0        0        0     5373 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/graph_export.py
--rw-r--r--   0        0        0     3936 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/project_edit.py
--rw-r--r--   0        0        0     3180 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/project_lock_status.py
--rw-r--r--   0        0        0     2096 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/project_show.py
--rw-r--r--   0        0        0     8043 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/templates_create_project.py
--rw-r--r--   0        0        0     3100 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/templates_read_manifest.py
--rw-r--r--   0        0        0      773 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/utils/__init__.py
--rw-r--r--   0        0        0     1083 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/utils/datasets.py
--rw-r--r--   0        0        0     3230 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/utils/project_clone.py
--rw-r--r--   0        0        0     2661 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/utils/remote_project.py
--rw-r--r--   0        0        0     1641 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/version.py
--rw-r--r--   0        0        0     2441 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/workflow_plans_export.py
--rw-r--r--   0        0        0     2257 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/workflow_plans_list.py
--rw-r--r--   0        0        0     2146 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/controllers/workflow_plans_show.py
--rw-r--r--   0        0        0     6150 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/entrypoint.py
--rw-r--r--   0        0        0    32040 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/errors.py
--rw-r--r--   0        0        0      774 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/gateways/__init__.py
--rw-r--r--   0        0        0     3339 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/gateways/gitlab_api_provider.py
--rw-r--r--   0        0        0      793 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/interfaces/__init__.py
--rw-r--r--   0        0        0     1228 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/interfaces/git_api_provider.py
--rw-r--r--   0        0        0      766 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/jobs/__init__.py
--rw-r--r--   0        0        0     3035 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/jobs/cleanup.py
--rw-r--r--   0        0        0      756 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/jobs/constants.py
--rw-r--r--   0        0        0     1186 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/jobs/contexts.py
--rw-r--r--   0        0        0     5244 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/jobs/datasets.py
--rw-r--r--   0        0        0     1829 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/jobs/delayed_ctrl.py
--rw-r--r--   0        0        0     2665 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/jobs/queues.py
--rw-r--r--   0        0        0     1269 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/logger.py
--rw-r--r--   0        0        0      644 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/logging.yaml
--rw-r--r--   0        0        0     2742 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/scheduler.py
--rw-r--r--   0        0        0      768 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/__init__.py
--rw-r--r--   0        0        0    13180 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/cache.py
--rw-r--r--   0        0        0     4045 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/common.py
--rw-r--r--   0        0        0     2228 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/config.py
--rw-r--r--   0        0        0     8754 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/datasets.py
--rw-r--r--   0        0        0     2195 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/graph.py
--rw-r--r--   0        0        0     5362 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/headers.py
--rw-r--r--   0        0        0     1961 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/jobs.py
--rw-r--r--   0        0        0     4510 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/project.py
--rw-r--r--   0        0        0      911 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/rpc.py
--rw-r--r--   0        0        0     5858 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/templates.py
--rw-r--r--   0        0        0      773 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/v1/__init__.py
--rw-r--r--   0        0        0     4212 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/v1/cache.py
--rw-r--r--   0        0        0     1880 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/v1/templates.py
--rw-r--r--   0        0        0     1170 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/version.py
--rw-r--r--   0        0        0     6907 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/serializers/workflows.py
--rw-r--r--   0        0        0     2186 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/utils/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/utils/callback.py
--rw-r--r--   0        0        0     1323 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/utils/json_encoder.py
--rw-r--r--   0        0        0     1260 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/utils/squash.py
--rw-r--r--   0        0        0     1427 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/utils/timeout.py
--rw-r--r--   0        0        0     1761 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/__init__.py
--rw-r--r--   0        0        0     2438 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/api_versions.py
--rw-r--r--   0        0        0     4771 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/apispec.py
--rw-r--r--   0        0        0     7427 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/cache.py
--rw-r--r--   0        0        0     2957 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/config.py
--rw-r--r--   0        0        0     8187 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/datasets.py
--rw-r--r--   0        0        0     2961 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/decorators.py
--rw-r--r--   0        0        0    14829 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/error_handlers.py
--rw-r--r--   0        0        0     2084 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/graph.py
--rw-r--r--   0        0        0     3267 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/jobs.py
--rw-r--r--   0        0        0     3805 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/project.py
--rw-r--r--   0        0        0     3592 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/templates.py
--rw-r--r--   0        0        0      767 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/v1/__init__.py
--rw-r--r--   0        0        0     3574 2023-05-15 07:08:32.067180 renku-2.4.1rc1/renku/ui/service/views/v1/cache.py
--rw-r--r--   0        0        0     2634 2023-05-15 07:08:32.071180 renku-2.4.1rc1/renku/ui/service/views/v1/templates.py
--rw-r--r--   0        0        0     1702 2023-05-15 07:08:32.071180 renku-2.4.1rc1/renku/ui/service/views/version.py
--rw-r--r--   0        0        0     3873 2023-05-15 07:08:32.071180 renku-2.4.1rc1/renku/ui/service/views/workflow_plans.py
--rw-r--r--   0        0        0     2890 2023-05-15 07:08:32.071180 renku-2.4.1rc1/renku/ui/service/worker.py
--rw-r--r--   0        0        0     1597 2023-05-15 07:08:32.071180 renku-2.4.1rc1/renku/version.py
--rw-r--r--   0        0        0    17302 1970-01-01 00:00:00.000000 renku-2.4.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-05-15 19:30:40.069354 renku-2.4.1rc2/AUTHORS.rst
+-rw-r--r--   0        0        0   179540 2023-05-15 19:30:40.069354 renku-2.4.1rc2/CHANGES.rst
+-rw-r--r--   0        0        0    11358 2023-05-15 19:30:40.069354 renku-2.4.1rc2/LICENSE
+-rw-r--r--   0        0        0    12889 2023-05-15 19:30:40.069354 renku-2.4.1rc2/README.rst
+-rw-r--r--   0        0        0    10401 2023-05-15 19:31:55.285766 renku-2.4.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     4391 2023-05-15 19:30:40.137359 renku-2.4.1rc2/renku/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-15 19:30:40.137359 renku-2.4.1rc2/renku/command/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-15 19:31:49.841441 renku-2.4.1rc2/renku/command/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      437 2023-05-15 19:31:49.841441 renku-2.4.1rc2/renku/command/__pycache__/options.cpython-39.pyc
+-rw-r--r--   0        0        0     1057 2023-05-15 19:31:53.097636 renku-2.4.1rc2/renku/command/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     1343 2023-05-15 19:31:49.841441 renku-2.4.1rc2/renku/command/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0      593 2023-05-15 19:31:49.845441 renku-2.4.1rc2/renku/command/__pycache__/version.cpython-39.pyc
+-rw-r--r--   0        0        0     2096 2023-05-15 19:30:40.137359 renku-2.4.1rc2/renku/command/checks/__init__.py
+-rw-r--r--   0        0        0     4723 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/checks/activities.py
+-rw-r--r--   0        0        0     8186 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/checks/datasets.py
+-rw-r--r--   0        0        0     2769 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/checks/githooks.py
+-rw-r--r--   0        0        0     1500 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/checks/migration.py
+-rw-r--r--   0        0        0     2316 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/checks/project.py
+-rw-r--r--   0        0        0     1487 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/checks/storage.py
+-rw-r--r--   0        0        0     4262 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/checks/validate_shacl.py
+-rw-r--r--   0        0        0     4881 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/checks/workflow.py
+-rw-r--r--   0        0        0     3872 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/clone.py
+-rw-r--r--   0        0        0      828 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/command_builder/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-15 19:31:50.469478 renku-2.4.1rc2/renku/command/command_builder/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    15431 2023-05-15 19:31:50.473479 renku-2.4.1rc2/renku/command/command_builder/__pycache__/command.cpython-39.pyc
+-rw-r--r--   0        0        0    16678 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/command_builder/command.py
+-rw-r--r--   0        0        0     1951 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/command_builder/communication.py
+-rw-r--r--   0        0        0     5325 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/command_builder/database.py
+-rw-r--r--   0        0        0     1701 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/command_builder/lock.py
+-rw-r--r--   0        0        0     1481 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/command_builder/migration.py
+-rw-r--r--   0        0        0     7694 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/command_builder/repo.py
+-rw-r--r--   0        0        0     4803 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/config.py
+-rw-r--r--   0        0        0     5640 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/dataset.py
+-rw-r--r--   0        0        0     2718 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/doctor.py
+-rw-r--r--   0        0        0      775 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/format/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-15 19:31:50.077455 renku-2.4.1rc2/renku/command/format/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5765 2023-05-15 19:31:50.077455 renku-2.4.1rc2/renku/command/format/__pycache__/dataset_files.cpython-39.pyc
+-rw-r--r--   0        0        0     1508 2023-05-15 19:31:50.081455 renku-2.4.1rc2/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc
+-rw-r--r--   0        0        0     2884 2023-05-15 19:31:50.081455 renku-2.4.1rc2/renku/command/format/__pycache__/datasets.cpython-39.pyc
+-rw-r--r--   0        0        0      817 2023-05-15 19:31:52.229584 renku-2.4.1rc2/renku/command/format/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0     1754 2023-05-15 19:31:53.113637 renku-2.4.1rc2/renku/command/format/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     1929 2023-05-15 19:31:52.229584 renku-2.4.1rc2/renku/command/format/__pycache__/tabulate.cpython-39.pyc
+-rw-r--r--   0        0        0     2416 2023-05-15 19:31:52.229584 renku-2.4.1rc2/renku/command/format/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0        0        0     2643 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/format/activity.py
+-rw-r--r--   0        0        0     6230 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/format/dataset_files.py
+-rw-r--r--   0        0        0     2098 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/format/dataset_tags.py
+-rw-r--r--   0        0        0     3236 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/format/datasets.py
+-rw-r--r--   0        0        0     1212 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/format/json.py
+-rw-r--r--   0        0        0     2402 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/format/session.py
+-rw-r--r--   0        0        0     2769 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/format/tabulate.py
+-rw-r--r--   0        0        0     2728 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/format/workflow.py
+-rw-r--r--   0        0        0     1012 2023-05-15 19:30:40.141359 renku-2.4.1rc2/renku/command/gc.py
+-rw-r--r--   0        0        0     1154 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/githooks.py
+-rw-r--r--   0        0        0     9880 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/graph.py
+-rw-r--r--   0        0        0     1081 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/group.py
+-rw-r--r--   0        0        0     1203 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/init.py
+-rw-r--r--   0        0        0     3124 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/log.py
+-rw-r--r--   0        0        0     1241 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/login.py
+-rw-r--r--   0        0        0     2822 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/mergetool.py
+-rw-r--r--   0        0        0     7621 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/migrate.py
+-rw-r--r--   0        0        0     9141 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/move.py
+-rw-r--r--   0        0        0     1015 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/options.py
+-rw-r--r--   0        0        0     1362 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/project.py
+-rw-r--r--   0        0        0     4748 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/remove.py
+-rw-r--r--   0        0        0     3146 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/rerun.py
+-rw-r--r--   0        0        0    10987 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/rollback.py
+-rw-r--r--   0        0        0     1600 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/run.py
+-rw-r--r--   0        0        0     3375 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/save.py
+-rw-r--r--   0        0        0      766 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/__init__.py
+-rw-r--r--   0        0        0      211 2023-05-15 19:31:50.161460 renku-2.4.1rc2/renku/command/schema/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1560 2023-05-15 19:31:50.161460 renku-2.4.1rc2/renku/command/schema/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0      977 2023-05-15 19:31:50.325470 renku-2.4.1rc2/renku/command/schema/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     6652 2023-05-15 19:31:50.317469 renku-2.4.1rc2/renku/command/schema/__pycache__/calamus.cpython-39.pyc
+-rw-r--r--   0        0        0     7584 2023-05-15 19:31:50.161460 renku-2.4.1rc2/renku/command/schema/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     1345 2023-05-15 19:31:50.329470 renku-2.4.1rc2/renku/command/schema/__pycache__/entity.cpython-39.pyc
+-rw-r--r--   0        0        0     5615 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/activity.py
+-rw-r--r--   0        0        0     1744 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/agent.py
+-rw-r--r--   0        0        0     1235 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/annotation.py
+-rw-r--r--   0        0        0     8986 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/calamus.py
+-rw-r--r--   0        0        0     3186 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/composite_plan.py
+-rw-r--r--   0        0        0     8210 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/dataset.py
+-rw-r--r--   0        0        0     1445 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/entity.py
+-rw-r--r--   0        0        0     4016 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/parameter.py
+-rw-r--r--   0        0        0     3427 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/plan.py
+-rw-r--r--   0        0        0     3406 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/project.py
+-rw-r--r--   0        0        0     1829 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/schema/workflow_file.py
+-rw-r--r--   0        0        0     1578 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/session.py
+-rw-r--r--   0        0        0     1036 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/status.py
+-rw-r--r--   0        0        0     3944 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/storage.py
+-rw-r--r--   0        0        0     1919 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/template.py
+-rw-r--r--   0        0        0     1254 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/update.py
+-rw-r--r--   0        0        0     1726 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/util.py
+-rw-r--r--   0        0        0     1088 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/version.py
+-rw-r--r--   0        0        0      768 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/__init__.py
+-rw-r--r--   0        0        0      217 2023-05-15 19:31:52.229584 renku-2.4.1rc2/renku/command/view_model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13077 2023-05-15 19:31:52.233584 renku-2.4.1rc2/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc
+-rw-r--r--   0        0        0     1350 2023-05-15 19:31:52.269586 renku-2.4.1rc2/renku/command/view_model/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0     8157 2023-05-15 19:31:52.273586 renku-2.4.1rc2/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc
+-rw-r--r--   0        0        0    11145 2023-05-15 19:31:53.053633 renku-2.4.1rc2/renku/command/view_model/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0     7823 2023-05-15 19:31:52.269586 renku-2.4.1rc2/renku/command/view_model/__pycache__/plan.cpython-39.pyc
+-rw-r--r--   0        0        0    13979 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/activity_graph.py
+-rw-r--r--   0        0        0     1657 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/agent.py
+-rw-r--r--   0        0        0     8768 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/composite_plan.py
+-rw-r--r--   0        0        0     2138 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/dataset.py
+-rw-r--r--   0        0        0     7772 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/graph.py
+-rw-r--r--   0        0        0    12497 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/log.py
+-rw-r--r--   0        0        0     9377 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/plan.py
+-rw-r--r--   0        0        0     3306 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/project.py
+-rw-r--r--   0        0        0     5947 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/template.py
+-rw-r--r--   0        0        0    14502 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/text_canvas.py
+-rw-r--r--   0        0        0     4792 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/view_model/workflow_file.py
+-rw-r--r--   0        0        0     4114 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/command/workflow.py
+-rw-r--r--   0        0        0      745 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/core/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-15 19:31:49.845441 renku-2.4.1rc2/renku/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4501 2023-05-15 19:31:50.373473 renku-2.4.1rc2/renku/core/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     1707 2023-05-15 19:31:49.853442 renku-2.4.1rc2/renku/core/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0    34603 2023-05-15 19:31:49.849441 renku-2.4.1rc2/renku/core/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     4854 2023-05-15 19:31:52.273586 renku-2.4.1rc2/renku/core/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0     8039 2023-05-15 19:31:50.481479 renku-2.4.1rc2/renku/core/__pycache__/login.cpython-39.pyc
+-rw-r--r--   0        0        0    16201 2023-05-15 19:31:50.449477 renku-2.4.1rc2/renku/core/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0        0        0     6170 2023-05-15 19:30:40.145359 renku-2.4.1rc2/renku/core/config.py
+-rw-r--r--   0        0        0     2717 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/constant.py
+-rw-r--r--   0        0        0      765 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/__init__.py
+-rw-r--r--   0        0        0      208 2023-05-15 19:31:50.081455 renku-2.4.1rc2/renku/core/dataset/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7431 2023-05-15 19:31:50.469478 renku-2.4.1rc2/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc
+-rw-r--r--   0        0        0     2954 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/context.py
+-rw-r--r--   0        0        0    54038 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/dataset.py
+-rw-r--r--   0        0        0    21429 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/dataset_add.py
+-rw-r--r--   0        0        0     9747 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/datasets_provenance.py
+-rw-r--r--   0        0        0     4296 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/pointer_file.py
+-rw-r--r--   0        0        0      760 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-15 19:31:50.085456 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    15669 2023-05-15 19:31:50.089456 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc
+-rw-r--r--   0        0        0     6716 2023-05-15 19:31:50.105457 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc
+-rw-r--r--   0        0        0     1646 2023-05-15 19:31:50.105457 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0        0        0    19281 2023-05-15 19:31:50.437476 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc
+-rw-r--r--   0        0        0     2797 2023-05-15 19:31:50.437476 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc
+-rw-r--r--   0        0        0     5069 2023-05-15 19:31:50.441477 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc
+-rw-r--r--   0        0        0     5945 2023-05-15 19:31:50.441477 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc
+-rw-r--r--   0        0        0     5562 2023-05-15 19:31:50.085456 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc
+-rw-r--r--   0        0        0     5966 2023-05-15 19:31:50.445477 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0     9328 2023-05-15 19:31:50.461478 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc
+-rw-r--r--   0        0        0     6028 2023-05-15 19:31:50.109457 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     9555 2023-05-15 19:31:50.465478 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc
+-rw-r--r--   0        0        0    17162 2023-05-15 19:31:50.469478 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc
+-rw-r--r--   0        0        0     2538 2023-05-15 19:31:50.441477 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc
+-rw-r--r--   0        0        0     6242 2023-05-15 19:31:50.549483 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc
+-rw-r--r--   0        0        0     4868 2023-05-15 19:31:50.553484 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc
+-rw-r--r--   0        0        0    17896 2023-05-15 19:31:50.561484 renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc
+-rw-r--r--   0        0        0    12028 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/api.py
+-rw-r--r--   0        0        0     6966 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/azure.py
+-rw-r--r--   0        0        0     2225 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/common.py
+-rw-r--r--   0        0        0    20652 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/dataverse.py
+-rw-r--r--   0        0        0     3317 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/dataverse_metadata_templates.py
+-rw-r--r--   0        0        0     4808 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/doi.py
+-rw-r--r--   0        0        0     5602 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/external.py
+-rw-r--r--   0        0        0     5764 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/factory.py
+-rw-r--r--   0        0        0     7300 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/git.py
+-rw-r--r--   0        0        0    11965 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/local.py
+-rw-r--r--   0        0        0     5869 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/models.py
+-rw-r--r--   0        0        0    10097 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/olos.py
+-rw-r--r--   0        0        0    22146 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/renku.py
+-rw-r--r--   0        0        0     2553 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/repository.py
+-rw-r--r--   0        0        0     6392 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/s3.py
+-rw-r--r--   0        0        0     5813 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/web.py
+-rw-r--r--   0        0        0    18624 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/providers/zenodo.py
+-rw-r--r--   0        0        0     3973 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/request_model.py
+-rw-r--r--   0        0        0     5361 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/dataset/tag.py
+-rw-r--r--   0        0        0    25658 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/errors.py
+-rw-r--r--   0        0        0     1115 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/gc.py
+-rw-r--r--   0        0        0     7394 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/git.py
+-rw-r--r--   0        0        0     2151 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/githooks.py
+-rw-r--r--   0        0        0    16526 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/init.py
+-rw-r--r--   0        0        0      775 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/interface/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-15 19:31:50.429476 renku-2.4.1rc2/renku/core/interface/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4269 2023-05-15 19:31:52.233584 renku-2.4.1rc2/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     1246 2023-05-15 19:31:52.277587 renku-2.4.1rc2/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     2159 2023-05-15 19:31:50.477479 renku-2.4.1rc2/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     2057 2023-05-15 19:31:52.221583 renku-2.4.1rc2/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0      959 2023-05-15 19:31:52.221583 renku-2.4.1rc2/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     4402 2023-05-15 19:31:50.429476 renku-2.4.1rc2/renku/core/interface/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0        0        0     1579 2023-05-15 19:31:52.137578 renku-2.4.1rc2/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc
+-rw-r--r--   0        0        0     3741 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/interface/activity_gateway.py
+-rw-r--r--   0        0        0     1418 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/interface/database_gateway.py
+-rw-r--r--   0        0        0     2095 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/interface/dataset_gateway.py
+-rw-r--r--   0        0        0     1996 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/interface/plan_gateway.py
+-rw-r--r--   0        0        0     1212 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/interface/project_gateway.py
+-rw-r--r--   0        0        0     4226 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/interface/storage.py
+-rw-r--r--   0        0        0     1780 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/interface/workflow_file_parser.py
+-rw-r--r--   0        0        0    10639 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/login.py
+-rw-r--r--   0        0        0      764 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/migration/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-15 19:31:50.377473 renku-2.4.1rc2/renku/core/migration/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1122 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/migration/m_0003__0_pyld2.py
+-rw-r--r--   0        0        0    15324 2023-05-15 19:30:40.149359 renku-2.4.1rc2/renku/core/migration/m_0003__1_jsonld.py
+-rw-r--r--   0        0        0     9570 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0003__2_initial.py
+-rw-r--r--   0        0        0     1122 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0004__0_pyld2.py
+-rw-r--r--   0        0        0     5318 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0004__submodules.py
+-rw-r--r--   0        0        0     1548 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0005__1_pyld2.py
+-rw-r--r--   0        0        0    16122 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0005__2_cwl.py
+-rw-r--r--   0        0        0     1015 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0006__dataset_context.py
+-rw-r--r--   0        0        0     1430 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0007__source_url.py
+-rw-r--r--   0        0        0     1175 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0008__dataset_metadata.py
+-rw-r--r--   0        0        0    30683 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0009__new_metadata_storage.py
+-rw-r--r--   0        0        0    14077 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/m_0010__metadata_fixes.py
+-rw-r--r--   0        0        0    10119 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/migrate.py
+-rw-r--r--   0        0        0      770 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/models/__init__.py
+-rw-r--r--   0        0        0     5830 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/models/migration.py
+-rw-r--r--   0        0        0     3861 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/models/refs.py
+-rw-r--r--   0        0        0     5091 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/models/v10.py
+-rw-r--r--   0        0        0    11828 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/models/v3.py
+-rw-r--r--   0        0        0     2422 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/models/v7.py
+-rw-r--r--   0        0        0     4587 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/models/v8.py
+-rw-r--r--   0        0        0    74088 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/models/v9.py
+-rw-r--r--   0        0        0     7865 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/utils/__init__.py
+-rw-r--r--   0        0        0     6558 2023-05-15 19:31:50.377473 renku-2.4.1rc2/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8121 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/migration/utils/conversion.py
+-rw-r--r--   0        0        0      824 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/plugin/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-15 19:31:50.089456 renku-2.4.1rc2/renku/core/plugin/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1033 2023-05-15 19:31:50.101456 renku-2.4.1rc2/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc
+-rw-r--r--   0        0        0     1049 2023-05-15 19:31:50.105457 renku-2.4.1rc2/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc
+-rw-r--r--   0        0        0     3246 2023-05-15 19:31:51.341531 renku-2.4.1rc2/renku/core/plugin/__pycache__/provider.cpython-39.pyc
+-rw-r--r--   0        0        0     1467 2023-05-15 19:31:53.005630 renku-2.4.1rc2/renku/core/plugin/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0      985 2023-05-15 19:31:53.113637 renku-2.4.1rc2/renku/core/plugin/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     4177 2023-05-15 19:31:52.685611 renku-2.4.1rc2/renku/core/plugin/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0        0        0     2978 2023-05-15 19:31:52.241584 renku-2.4.1rc2/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc
+-rw-r--r--   0        0        0     1467 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/plugin/dataset_provider.py
+-rw-r--r--   0        0        0     3046 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/plugin/implementations/__init__.py
+-rw-r--r--   0        0        0     2540 2023-05-15 19:31:50.105457 renku-2.4.1rc2/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1790 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/plugin/pluginmanager.py
+-rw-r--r--   0        0        0     3357 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/plugin/provider.py
+-rw-r--r--   0        0        0     1839 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/plugin/run.py
+-rw-r--r--   0        0        0     1454 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/plugin/session.py
+-rw-r--r--   0        0        0     4195 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/plugin/workflow.py
+-rw-r--r--   0        0        0     3065 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/plugin/workflow_file_parser.py
+-rw-r--r--   0        0        0     3355 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/project.py
+-rw-r--r--   0        0        0      780 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/session/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-15 19:31:50.561484 renku-2.4.1rc2/renku/core/session/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11692 2023-05-15 19:31:50.561484 renku-2.4.1rc2/renku/core/session/__pycache__/docker.cpython-39.pyc
+-rw-r--r--   0        0        0    15989 2023-05-15 19:31:50.737495 renku-2.4.1rc2/renku/core/session/__pycache__/renkulab.cpython-39.pyc
+-rw-r--r--   0        0        0     1449 2023-05-15 19:31:50.741495 renku-2.4.1rc2/renku/core/session/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0    14350 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/session/docker.py
+-rw-r--r--   0        0        0    20534 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/session/renkulab.py
+-rw-r--r--   0        0        0    11815 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/session/session.py
+-rw-r--r--   0        0        0     2215 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/session/utils.py
+-rw-r--r--   0        0        0    21861 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/storage.py
+-rw-r--r--   0        0        0      760 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/template/__init__.py
+-rw-r--r--   0        0        0    22043 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/template/template.py
+-rw-r--r--   0        0        0    14612 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/template/usecase.py
+-rw-r--r--   0        0        0      756 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/util/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-15 19:31:49.853442 renku-2.4.1rc2/renku/core/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11124 2023-05-15 19:31:50.101456 renku-2.4.1rc2/renku/core/util/__pycache__/communication.cpython-39.pyc
+-rw-r--r--   0        0        0     6320 2023-05-15 19:31:52.277587 renku-2.4.1rc2/renku/core/util/__pycache__/contexts.cpython-39.pyc
+-rw-r--r--   0        0        0     1801 2023-05-15 19:31:50.369473 renku-2.4.1rc2/renku/core/util/__pycache__/datetime8601.cpython-39.pyc
+-rw-r--r--   0        0        0      933 2023-05-15 19:31:50.101456 renku-2.4.1rc2/renku/core/util/__pycache__/doi.cpython-39.pyc
+-rw-r--r--   0        0        0    33652 2023-05-15 19:31:49.861442 renku-2.4.1rc2/renku/core/util/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0      669 2023-05-15 19:31:50.761496 renku-2.4.1rc2/renku/core/util/__pycache__/jwt.cpython-39.pyc
+-rw-r--r--   0        0        0     6008 2023-05-15 19:31:50.373473 renku-2.4.1rc2/renku/core/util/__pycache__/metadata.cpython-39.pyc
+-rw-r--r--   0        0        0    11013 2023-05-15 19:31:50.053454 renku-2.4.1rc2/renku/core/util/__pycache__/os.cpython-39.pyc
+-rw-r--r--   0        0        0     6893 2023-05-15 19:31:50.741495 renku-2.4.1rc2/renku/core/util/__pycache__/requests.cpython-39.pyc
+-rw-r--r--   0        0        0     5971 2023-05-15 19:31:50.821499 renku-2.4.1rc2/renku/core/util/__pycache__/ssh.cpython-39.pyc
+-rw-r--r--   0        0        0     4943 2023-05-15 19:31:50.381473 renku-2.4.1rc2/renku/core/util/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0        0        0     3737 2023-05-15 19:31:50.553484 renku-2.4.1rc2/renku/core/util/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     2663 2023-05-15 19:31:50.377473 renku-2.4.1rc2/renku/core/util/__pycache__/yaml.cpython-39.pyc
+-rw-r--r--   0        0        0    10282 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/util/communication.py
+-rw-r--r--   0        0        0     6617 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/util/contexts.py
+-rw-r--r--   0        0        0     2313 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/util/datetime8601.py
+-rw-r--r--   0        0        0     1376 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/util/doi.py
+-rw-r--r--   0        0        0    40689 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/util/git.py
+-rw-r--r--   0        0        0     1244 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/util/jwt.py
+-rw-r--r--   0        0        0     7036 2023-05-15 19:30:40.153360 renku-2.4.1rc2/renku/core/util/metadata.py
+-rw-r--r--   0        0        0    12140 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/util/os.py
+-rw-r--r--   0        0        0     7626 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/util/requests.py
+-rw-r--r--   0        0        0     1611 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/util/shacl.py
+-rw-r--r--   0        0        0     6871 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/util/ssh.py
+-rw-r--r--   0        0        0     2158 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/util/tabulate.py
+-rw-r--r--   0        0        0     6228 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/util/urls.py
+-rw-r--r--   0        0        0     3878 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/util/util.py
+-rw-r--r--   0        0        0     2836 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/util/yaml.py
+-rw-r--r--   0        0        0      773 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-15 19:31:50.821499 renku-2.4.1rc2/renku/core/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    18165 2023-05-15 19:31:52.281587 renku-2.4.1rc2/renku/core/workflow/__pycache__/activity.cpython-39.pyc
+-rw-r--r--   0        0        0    14583 2023-05-15 19:31:53.101636 renku-2.4.1rc2/renku/core/workflow/__pycache__/execute.cpython-39.pyc
+-rw-r--r--   0        0        0    26495 2023-05-15 19:31:52.229584 renku-2.4.1rc2/renku/core/workflow/__pycache__/plan.cpython-39.pyc
+-rw-r--r--   0        0        0    23623 2023-05-15 19:31:52.289587 renku-2.4.1rc2/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc
+-rw-r--r--   0        0        0    10067 2023-05-15 19:31:52.269586 renku-2.4.1rc2/renku/core/workflow/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     1660 2023-05-15 19:31:52.289587 renku-2.4.1rc2/renku/core/workflow/__pycache__/types.cpython-39.pyc
+-rw-r--r--   0        0        0     8676 2023-05-15 19:31:52.245585 renku-2.4.1rc2/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc
+-rw-r--r--   0        0        0     4780 2023-05-15 19:31:53.097636 renku-2.4.1rc2/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc
+-rw-r--r--   0        0        0    22713 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/activity.py
+-rw-r--r--   0        0        0      773 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/converters/__init__.py
+-rw-r--r--   0        0        0      215 2023-05-15 19:31:50.821499 renku-2.4.1rc2/renku/core/workflow/converters/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11073 2023-05-15 19:31:50.825500 renku-2.4.1rc2/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc
+-rw-r--r--   0        0        0     4668 2023-05-15 19:31:52.133578 renku-2.4.1rc2/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc
+-rw-r--r--   0        0        0    17930 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/converters/cwl.py
+-rw-r--r--   0        0        0     5142 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/converters/renku.py
+-rw-r--r--   0        0        0    18756 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/execute.py
+-rw-r--r--   0        0        0      769 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/model/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-15 19:31:51.341531 renku-2.4.1rc2/renku/core/workflow/model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4825 2023-05-15 19:31:51.345531 renku-2.4.1rc2/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc
+-rw-r--r--   0        0        0    26172 2023-05-15 19:31:52.145579 renku-2.4.1rc2/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc
+-rw-r--r--   0        0        0     6530 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/model/concrete_execution_graph.py
+-rw-r--r--   0        0        0    37866 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/model/workflow_file.py
+-rw-r--r--   0        0        0      775 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/parser/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-15 19:31:52.133578 renku-2.4.1rc2/renku/core/workflow/parser/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8620 2023-05-15 19:31:52.137578 renku-2.4.1rc2/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc
+-rw-r--r--   0        0        0    10631 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/parser/renku.py
+-rw-r--r--   0        0        0    34209 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/plan.py
+-rw-r--r--   0        0        0    33046 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/plan_factory.py
+-rw-r--r--   0        0        0      772 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/providers/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-15 19:31:52.297588 renku-2.4.1rc2/renku/core/workflow/providers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4631 2023-05-15 19:31:52.297588 renku-2.4.1rc2/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc
+-rw-r--r--   0        0        0     3918 2023-05-15 19:31:52.685611 renku-2.4.1rc2/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc
+-rw-r--r--   0        0        0    11194 2023-05-15 19:31:52.689611 renku-2.4.1rc2/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc
+-rw-r--r--   0        0        0     5999 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/providers/cwltool.py
+-rw-r--r--   0        0        0     4271 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/providers/local.py
+-rw-r--r--   0        0        0    13372 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/providers/toil.py
+-rw-r--r--   0        0        0    13562 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/run.py
+-rw-r--r--   0        0        0     1681 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/types.py
+-rw-r--r--   0        0        0     2869 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/update.py
+-rw-r--r--   0        0        0     8335 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/value_resolution.py
+-rw-r--r--   0        0        0     5089 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/core/workflow/workflow_file.py
+-rw-r--r--   0        0        0      767 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/data/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/data/defaults.ini
+-rw-r--r--   0        0        0     3364 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/data/gitignore.default
+-rwxr-xr-x   0        0        0     4372 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/data/pre-commit.sh
+-rw-r--r--   0        0        0    48383 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/data/shacl_shape.json
+-rw-r--r--   0        0        0      767 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/domain_model/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-15 19:31:50.057454 renku-2.4.1rc2/renku/domain_model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      388 2023-05-15 19:31:50.081455 renku-2.4.1rc2/renku/domain_model/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0    26291 2023-05-15 19:31:50.337471 renku-2.4.1rc2/renku/domain_model/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0      988 2023-05-15 19:31:50.097456 renku-2.4.1rc2/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc
+-rw-r--r--   0        0        0     2204 2023-05-15 19:31:52.293588 renku-2.4.1rc2/renku/domain_model/__pycache__/datastructures.cpython-39.pyc
+-rw-r--r--   0        0        0     2539 2023-05-15 19:31:50.329470 renku-2.4.1rc2/renku/domain_model/__pycache__/entity.cpython-39.pyc
+-rw-r--r--   0        0        0      575 2023-05-15 19:31:50.377473 renku-2.4.1rc2/renku/domain_model/__pycache__/enums.cpython-39.pyc
+-rw-r--r--   0        0        0     6097 2023-05-15 19:31:52.129578 renku-2.4.1rc2/renku/domain_model/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0    12164 2023-05-15 19:31:50.061454 renku-2.4.1rc2/renku/domain_model/__pycache__/project_context.cpython-39.pyc
+-rw-r--r--   0        0        0     7196 2023-05-15 19:31:50.733494 renku-2.4.1rc2/renku/domain_model/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     1092 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/domain_model/constant.py
+-rw-r--r--   0        0        0    29605 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/domain_model/dataset.py
+-rw-r--r--   0        0        0     1267 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/domain_model/dataset_provider.py
+-rw-r--r--   0        0        0     2754 2023-05-15 19:30:40.157360 renku-2.4.1rc2/renku/domain_model/datastructures.py
+-rw-r--r--   0        0        0     2499 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/entity.py
+-rw-r--r--   0        0        0      971 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/enums.py
+-rw-r--r--   0        0        0     5059 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/git.py
+-rw-r--r--   0        0        0     8329 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/project.py
+-rw-r--r--   0        0        0    11817 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/project_context.py
+-rw-r--r--   0        0        0      829 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/provenance/__init__.py
+-rw-r--r--   0        0        0      283 2023-05-15 19:31:50.321470 renku-2.4.1rc2/renku/domain_model/provenance/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11882 2023-05-15 19:31:52.237584 renku-2.4.1rc2/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc
+-rw-r--r--   0        0        0     4946 2023-05-15 19:31:50.325470 renku-2.4.1rc2/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0     1092 2023-05-15 19:31:50.325470 renku-2.4.1rc2/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     1363 2023-05-15 19:31:52.237584 renku-2.4.1rc2/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc
+-rw-r--r--   0        0        0    13200 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/provenance/activity.py
+-rw-r--r--   0        0        0     5155 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/provenance/agent.py
+-rw-r--r--   0        0        0     1268 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/provenance/annotation.py
+-rw-r--r--   0        0        0     1530 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/provenance/parameter.py
+-rw-r--r--   0        0        0     6701 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/session.py
+-rw-r--r--   0        0        0     1471 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/sort.py
+-rw-r--r--   0        0        0    27042 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/template.py
+-rw-r--r--   0        0        0      782 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/workflow/__init__.py
+-rw-r--r--   0        0        0      234 2023-05-15 19:31:51.341531 renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13527 2023-05-15 19:31:51.785557 renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc
+-rw-r--r--   0        0        0    15243 2023-05-15 19:31:51.789557 renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc
+-rw-r--r--   0        0        0    15096 2023-05-15 19:31:51.793558 renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc
+-rw-r--r--   0        0        0     1483 2023-05-15 19:31:51.341531 renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc
+-rw-r--r--   0        0        0     4413 2023-05-15 19:31:52.237584 renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc
+-rw-r--r--   0        0        0    15917 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/workflow/composite_plan.py
+-rw-r--r--   0        0        0     1531 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/workflow/converters/__init__.py
+-rw-r--r--   0        0        0     1391 2023-05-15 19:31:52.133578 renku-2.4.1rc2/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    18124 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/workflow/parameter.py
+-rw-r--r--   0        0        0    16602 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/workflow/plan.py
+-rw-r--r--   0        0        0     1639 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/workflow/provider.py
+-rw-r--r--   0        0        0     4349 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/domain_model/workflow/workflow_file.py
+-rw-r--r--   0        0        0      780 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/__init__.py
+-rw-r--r--   0        0        0      212 2023-05-15 19:31:49.861442 renku-2.4.1rc2/renku/infrastructure/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    34957 2023-05-15 19:31:51.917565 renku-2.4.1rc2/renku/infrastructure/__pycache__/database.cpython-39.pyc
+-rw-r--r--   0        0        0     5073 2023-05-15 19:31:50.081455 renku-2.4.1rc2/renku/infrastructure/__pycache__/immutable.cpython-39.pyc
+-rw-r--r--   0        0        0     2259 2023-05-15 19:31:50.381473 renku-2.4.1rc2/renku/infrastructure/__pycache__/persistent.cpython-39.pyc
+-rw-r--r--   0        0        0    67759 2023-05-15 19:31:49.881443 renku-2.4.1rc2/renku/infrastructure/__pycache__/repository.cpython-39.pyc
+-rw-r--r--   0        0        0    41333 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/database.py
+-rw-r--r--   0        0        0      786 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/gateway/__init__.py
+-rw-r--r--   0        0        0    12730 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/gateway/activity_gateway.py
+-rw-r--r--   0        0        0     5845 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/gateway/database_gateway.py
+-rw-r--r--   0        0        0     3743 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/gateway/dataset_gateway.py
+-rw-r--r--   0        0        0     3529 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/gateway/plan_gateway.py
+-rw-r--r--   0        0        0     1711 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/gateway/project_gateway.py
+-rw-r--r--   0        0        0    18006 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/git_merger.py
+-rw-r--r--   0        0        0     4969 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/immutable.py
+-rw-r--r--   0        0        0     2394 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/persistent.py
+-rw-r--r--   0        0        0    71947 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/repository.py
+-rw-r--r--   0        0        0      784 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/storage/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-15 19:31:50.433476 renku-2.4.1rc2/renku/infrastructure/storage/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1523 2023-05-15 19:31:50.433476 renku-2.4.1rc2/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc
+-rw-r--r--   0        0        0     1989 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/storage/factory.py
+-rw-r--r--   0        0        0     8859 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/infrastructure/storage/rclone.py
+-rw-r--r--   0        0        0      913 2023-05-15 19:31:54.125697 renku-2.4.1rc2/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      553 2023-05-15 19:31:54.125697 renku-2.4.1rc2/renku/templates/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      637 2023-05-15 19:31:54.125697 renku-2.4.1rc2/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      523 2023-05-15 19:31:54.133698 renku-2.4.1rc2/renku/templates/.github/dependabot.yml
+-rw-r--r--   0        0        0      396 2023-05-15 19:31:54.125697 renku-2.4.1rc2/renku/templates/.github/workflows/github-project.yml
+-rw-r--r--   0        0        0     3940 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/.gitignore
+-rw-r--r--   0        0        0       27 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       37 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      984 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2087 2023-05-15 19:31:54.133698 renku-2.4.1rc2/renku/templates/R-minimal/Dockerfile
+-rw-r--r--   0        0        0     1603 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/environment.yml
+-rw-r--r--   0        0        0      360 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/install.R
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0      205 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal/{{ __sanitized_project_name__ }}.Rproj
+-rw-r--r--   0        0        0    14286 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/R-minimal.png
+-rw-r--r--   0        0        0     4846 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/README.md
+-rw-r--r--   0        0        0       27 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       37 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2077 2023-05-15 19:31:54.133698 renku-2.4.1rc2/renku/templates/bioc-minimal/Dockerfile
+-rw-r--r--   0        0        0     1603 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/install.R
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0      205 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioc-minimal/{{ __sanitized_project_name__ }}.Rproj
+-rw-r--r--   0        0        0    44589 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/bioconductor.png
+-rw-r--r--   0        0        0       27 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       50 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2469 2023-05-15 19:31:54.133698 renku-2.4.1rc2/renku/templates/julia-minimal/Dockerfile
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/Manifest.toml
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/Project.toml
+-rw-r--r--   0        0        0     1842 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julia-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0    13782 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/julialang.png
+-rw-r--r--   0        0        0     1174 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/manifest.yaml
+-rw-r--r--   0        0        0       17 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/minimal/.dockerignore
+-rw-r--r--   0        0        0       77 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       33 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2414 2023-05-15 19:31:54.133698 renku-2.4.1rc2/renku/templates/minimal/Dockerfile
+-rw-r--r--   0        0        0     1439 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0       27 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/.dockerignore
+-rw-r--r--   0        0        0     5401 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       33 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2159 2023-05-15 19:31:54.133698 renku-2.4.1rc2/renku/templates/python-minimal/Dockerfile
+-rw-r--r--   0        0        0     1597 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0    25599 2023-05-15 19:31:54.129697 renku-2.4.1rc2/renku/templates/python-minimal.png
+-rw-r--r--   0        0        0      763 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/ui/__init__.py
+-rw-r--r--   0        0        0      184 2023-05-15 19:31:49.713433 renku-2.4.1rc2/renku/ui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1268 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/ui/api/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/ui/api/graph/__init__.py
+-rw-r--r--   0        0        0     2519 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/ui/api/graph/rdf.py
+-rw-r--r--   0        0        0      764 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/ui/api/models/__init__.py
+-rw-r--r--   0        0        0    16448 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/ui/api/models/activity.py
+-rw-r--r--   0        0        0     4648 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/ui/api/models/dataset.py
+-rw-r--r--   0        0        0    10361 2023-05-15 19:30:40.161360 renku-2.4.1rc2/renku/ui/api/models/parameter.py
+-rw-r--r--   0        0        0     9227 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/api/models/plan.py
+-rw-r--r--   0        0        0     3643 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/api/models/project.py
+-rw-r--r--   0        0        0     2519 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/api/util.py
+-rw-r--r--   0        0        0     9319 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/__init__.py
+-rw-r--r--   0        0        0      922 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/__main__.py
+-rw-r--r--   0        0        0     8150 2023-05-15 19:31:49.717434 renku-2.4.1rc2/renku/ui/cli/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2117 2023-05-15 19:31:50.061454 renku-2.4.1rc2/renku/ui/cli/__pycache__/clone.cpython-39.pyc
+-rw-r--r--   0        0        0     7029 2023-05-15 19:31:50.065454 renku-2.4.1rc2/renku/ui/cli/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0    36528 2023-05-15 19:31:50.073455 renku-2.4.1rc2/renku/ui/cli/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     1698 2023-05-15 19:31:53.029631 renku-2.4.1rc2/renku/ui/cli/__pycache__/doctor.cpython-39.pyc
+-rw-r--r--   0        0        0      964 2023-05-15 19:31:53.029631 renku-2.4.1rc2/renku/ui/cli/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0        0        0     7957 2023-05-15 19:31:53.033632 renku-2.4.1rc2/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc
+-rw-r--r--   0        0        0      645 2023-05-15 19:31:53.045632 renku-2.4.1rc2/renku/ui/cli/__pycache__/gc.cpython-39.pyc
+-rw-r--r--   0        0        0     2168 2023-05-15 19:31:53.045632 renku-2.4.1rc2/renku/ui/cli/__pycache__/githooks.cpython-39.pyc
+-rw-r--r--   0        0        0     4041 2023-05-15 19:31:53.045632 renku-2.4.1rc2/renku/ui/cli/__pycache__/graph.cpython-39.pyc
+-rw-r--r--   0        0        0     9637 2023-05-15 19:31:53.049633 renku-2.4.1rc2/renku/ui/cli/__pycache__/init.cpython-39.pyc
+-rw-r--r--   0        0        0     7264 2023-05-15 19:31:53.049633 renku-2.4.1rc2/renku/ui/cli/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0     4296 2023-05-15 19:31:53.057633 renku-2.4.1rc2/renku/ui/cli/__pycache__/login.cpython-39.pyc
+-rw-r--r--   0        0        0     2066 2023-05-15 19:31:53.085635 renku-2.4.1rc2/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc
+-rw-r--r--   0        0        0     4435 2023-05-15 19:31:53.089635 renku-2.4.1rc2/renku/ui/cli/__pycache__/migrate.cpython-39.pyc
+-rw-r--r--   0        0        0     2306 2023-05-15 19:31:53.089635 renku-2.4.1rc2/renku/ui/cli/__pycache__/move.cpython-39.pyc
+-rw-r--r--   0        0        0     4028 2023-05-15 19:31:53.089635 renku-2.4.1rc2/renku/ui/cli/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0     1283 2023-05-15 19:31:53.093635 renku-2.4.1rc2/renku/ui/cli/__pycache__/remove.cpython-39.pyc
+-rw-r--r--   0        0        0     3485 2023-05-15 19:31:53.093635 renku-2.4.1rc2/renku/ui/cli/__pycache__/rerun.cpython-39.pyc
+-rw-r--r--   0        0        0     2761 2023-05-15 19:31:53.093635 renku-2.4.1rc2/renku/ui/cli/__pycache__/rollback.cpython-39.pyc
+-rw-r--r--   0        0        0    23646 2023-05-15 19:31:53.093635 renku-2.4.1rc2/renku/ui/cli/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     2890 2023-05-15 19:31:53.109636 renku-2.4.1rc2/renku/ui/cli/__pycache__/save.cpython-39.pyc
+-rw-r--r--   0        0        0    10307 2023-05-15 19:31:53.109636 renku-2.4.1rc2/renku/ui/cli/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0        0        0    12372 2023-05-15 19:31:53.113637 renku-2.4.1rc2/renku/ui/cli/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     3715 2023-05-15 19:31:53.117637 renku-2.4.1rc2/renku/ui/cli/__pycache__/status.cpython-39.pyc
+-rw-r--r--   0        0        0     5061 2023-05-15 19:31:53.117637 renku-2.4.1rc2/renku/ui/cli/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0        0        0    10944 2023-05-15 19:31:53.121637 renku-2.4.1rc2/renku/ui/cli/__pycache__/template.cpython-39.pyc
+-rw-r--r--   0        0        0     5790 2023-05-15 19:31:53.121637 renku-2.4.1rc2/renku/ui/cli/__pycache__/update.cpython-39.pyc
+-rw-r--r--   0        0        0    41957 2023-05-15 19:31:53.125637 renku-2.4.1rc2/renku/ui/cli/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0        0        0     2594 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/clone.py
+-rw-r--r--   0        0        0     7953 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/config.py
+-rw-r--r--   0        0        0    42970 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/dataset.py
+-rw-r--r--   0        0        0     2217 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/doctor.py
+-rw-r--r--   0        0        0     1600 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/env.py
+-rw-r--r--   0        0        0     7931 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/exception_handler.py
+-rw-r--r--   0        0        0     1139 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/gc.py
+-rw-r--r--   0        0        0     2538 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/githooks.py
+-rw-r--r--   0        0        0     4950 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/graph.py
+-rw-r--r--   0        0        0    11113 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/init.py
+-rw-r--r--   0        0        0     8581 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/log.py
+-rw-r--r--   0        0        0     4845 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/login.py
+-rw-r--r--   0        0        0     2499 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/mergetool.py
+-rw-r--r--   0        0        0     5689 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/migrate.py
+-rw-r--r--   0        0        0     2881 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/move.py
+-rw-r--r--   0        0        0     5768 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/project.py
+-rw-r--r--   0        0        0     1754 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/remove.py
+-rw-r--r--   0        0        0     4227 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/rerun.py
+-rw-r--r--   0        0        0     3249 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/rollback.py
+-rw-r--r--   0        0        0    26417 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/run.py
+-rw-r--r--   0        0        0     3510 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/save.py
+-rw-r--r--   0        0        0    11830 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/service.py
+-rw-r--r--   0        0        0    14005 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/session.py
+-rw-r--r--   0        0        0     5489 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/status.py
+-rw-r--r--   0        0        0     5604 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/storage.py
+-rw-r--r--   0        0        0    13434 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/template.py
+-rw-r--r--   0        0        0     6723 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/update.py
+-rw-r--r--   0        0        0      768 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/utils/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-15 19:31:50.065454 renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5720 2023-05-15 19:31:53.061633 renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc
+-rw-r--r--   0        0        0     3433 2023-05-15 19:31:50.065454 renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc
+-rw-r--r--   0        0        0      301 2023-05-15 19:31:50.065454 renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/color.cpython-39.pyc
+-rw-r--r--   0        0        0      998 2023-05-15 19:31:53.093635 renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc
+-rw-r--r--   0        0        0     7369 2023-05-15 19:31:53.057633 renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc
+-rw-r--r--   0        0        0     5422 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/utils/callback.py
+-rw-r--r--   0        0        0     3982 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/utils/click.py
+-rw-r--r--   0        0        0      855 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/utils/color.py
+-rw-r--r--   0        0        0    14534 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/utils/curses.py
+-rw-r--r--   0        0        0     1387 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/utils/plugins.py
+-rw-r--r--   0        0        0     9929 2023-05-15 19:30:40.165360 renku-2.4.1rc2/renku/ui/cli/utils/terminal.py
+-rw-r--r--   0        0        0    48023 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/cli/workflow.py
+-rw-r--r--   0        0        0      843 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/.env-example
+-rw-r--r--   0        0        0      756 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-15 19:31:53.033632 renku-2.4.1rc2/renku/ui/service/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2012 2023-05-15 19:31:53.033632 renku-2.4.1rc2/renku/ui/service/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     1535 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/__init__.py
+-rw-r--r--   0        0        0     2917 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/base.py
+-rw-r--r--   0        0        0     1168 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/config.py
+-rw-r--r--   0        0        0     3315 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/files.py
+-rw-r--r--   0        0        0     2333 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/jobs.py
+-rw-r--r--   0        0        0      769 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/models/__init__.py
+-rw-r--r--   0        0        0     4356 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/models/file.py
+-rw-r--r--   0        0        0     2273 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/models/job.py
+-rw-r--r--   0        0        0     4043 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/models/project.py
+-rw-r--r--   0        0        0     1127 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/models/user.py
+-rw-r--r--   0        0        0     2558 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/projects.py
+-rw-r--r--   0        0        0      774 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/serializers/__init__.py
+-rw-r--r--   0        0        0     1821 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/serializers/file.py
+-rw-r--r--   0        0        0     1711 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/serializers/job.py
+-rw-r--r--   0        0        0     1812 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/serializers/project.py
+-rw-r--r--   0        0        0     1227 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/serializers/user.py
+-rw-r--r--   0        0        0     1657 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/cache/users.py
+-rw-r--r--   0        0        0     2931 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/config.py
+-rw-r--r--   0        0        0      773 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/__init__.py
+-rw-r--r--   0        0        0      777 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/api/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/api/abstract.py
+-rw-r--r--   0        0        0    15626 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/api/mixins.py
+-rw-r--r--   0        0        0     2647 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/cache_files_delete_chunks.py
+-rw-r--r--   0        0        0     7478 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/cache_files_upload.py
+-rw-r--r--   0        0        0     2239 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/cache_list_projects.py
+-rw-r--r--   0        0        0     1927 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/cache_list_uploaded.py
+-rw-r--r--   0        0        0     4823 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/cache_migrate_project.py
+-rw-r--r--   0        0        0     5110 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/cache_migrations_check.py
+-rw-r--r--   0        0        0     2350 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/cache_project_clone.py
+-rw-r--r--   0        0        0     2649 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/config_set.py
+-rw-r--r--   0        0        0     2333 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/config_show.py
+-rw-r--r--   0        0        0     5682 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/datasets_add_file.py
+-rw-r--r--   0        0        0     3916 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/datasets_create.py
+-rw-r--r--   0        0        0     5359 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/datasets_edit.py
+-rw-r--r--   0        0        0     2132 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/datasets_files_list.py
+-rw-r--r--   0        0        0     3333 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/datasets_import.py
+-rw-r--r--   0        0        0     2065 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/datasets_list.py
+-rw-r--r--   0        0        0     2637 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/datasets_remove.py
+-rw-r--r--   0        0        0     3290 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/datasets_unlink.py
+-rw-r--r--   0        0        0     5373 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/graph_export.py
+-rw-r--r--   0        0        0     3936 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/project_edit.py
+-rw-r--r--   0        0        0     3180 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/project_lock_status.py
+-rw-r--r--   0        0        0     2096 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/project_show.py
+-rw-r--r--   0        0        0     8043 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/templates_create_project.py
+-rw-r--r--   0        0        0     3100 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/templates_read_manifest.py
+-rw-r--r--   0        0        0      773 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/utils/__init__.py
+-rw-r--r--   0        0        0     1083 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/utils/datasets.py
+-rw-r--r--   0        0        0     3230 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/utils/project_clone.py
+-rw-r--r--   0        0        0     2661 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/utils/remote_project.py
+-rw-r--r--   0        0        0     1641 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/version.py
+-rw-r--r--   0        0        0     2441 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/workflow_plans_export.py
+-rw-r--r--   0        0        0     2257 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/workflow_plans_list.py
+-rw-r--r--   0        0        0     2146 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/controllers/workflow_plans_show.py
+-rw-r--r--   0        0        0     6150 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/entrypoint.py
+-rw-r--r--   0        0        0    32040 2023-05-15 19:30:40.169360 renku-2.4.1rc2/renku/ui/service/errors.py
+-rw-r--r--   0        0        0      774 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/gateways/__init__.py
+-rw-r--r--   0        0        0     3339 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/gateways/gitlab_api_provider.py
+-rw-r--r--   0        0        0      793 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/interfaces/__init__.py
+-rw-r--r--   0        0        0     1228 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/interfaces/git_api_provider.py
+-rw-r--r--   0        0        0      766 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/jobs/__init__.py
+-rw-r--r--   0        0        0     3035 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/jobs/cleanup.py
+-rw-r--r--   0        0        0      756 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/jobs/constants.py
+-rw-r--r--   0        0        0     1186 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/jobs/contexts.py
+-rw-r--r--   0        0        0     5244 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/jobs/datasets.py
+-rw-r--r--   0        0        0     1829 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/jobs/delayed_ctrl.py
+-rw-r--r--   0        0        0     2665 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/jobs/queues.py
+-rw-r--r--   0        0        0     1269 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/logger.py
+-rw-r--r--   0        0        0      644 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/logging.yaml
+-rw-r--r--   0        0        0     2742 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/scheduler.py
+-rw-r--r--   0        0        0      768 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/__init__.py
+-rw-r--r--   0        0        0    13180 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/cache.py
+-rw-r--r--   0        0        0     4045 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/common.py
+-rw-r--r--   0        0        0     2228 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/config.py
+-rw-r--r--   0        0        0     8754 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/datasets.py
+-rw-r--r--   0        0        0     2195 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/graph.py
+-rw-r--r--   0        0        0     5362 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/headers.py
+-rw-r--r--   0        0        0     1961 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/jobs.py
+-rw-r--r--   0        0        0     4510 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/project.py
+-rw-r--r--   0        0        0      911 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/rpc.py
+-rw-r--r--   0        0        0     5858 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/templates.py
+-rw-r--r--   0        0        0      773 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/v1/__init__.py
+-rw-r--r--   0        0        0     4212 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/v1/cache.py
+-rw-r--r--   0        0        0     1880 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/v1/templates.py
+-rw-r--r--   0        0        0     1170 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/version.py
+-rw-r--r--   0        0        0     6907 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/serializers/workflows.py
+-rw-r--r--   0        0        0     2186 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/utils/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/utils/callback.py
+-rw-r--r--   0        0        0     1323 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/utils/json_encoder.py
+-rw-r--r--   0        0        0     1260 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/utils/squash.py
+-rw-r--r--   0        0        0     1427 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/utils/timeout.py
+-rw-r--r--   0        0        0     1761 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/__init__.py
+-rw-r--r--   0        0        0     2438 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/api_versions.py
+-rw-r--r--   0        0        0     4771 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/apispec.py
+-rw-r--r--   0        0        0     7427 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/cache.py
+-rw-r--r--   0        0        0     2957 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/config.py
+-rw-r--r--   0        0        0     8187 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/datasets.py
+-rw-r--r--   0        0        0     2961 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/decorators.py
+-rw-r--r--   0        0        0    14829 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/error_handlers.py
+-rw-r--r--   0        0        0     2084 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/graph.py
+-rw-r--r--   0        0        0     3267 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/jobs.py
+-rw-r--r--   0        0        0     3805 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/project.py
+-rw-r--r--   0        0        0     3592 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/templates.py
+-rw-r--r--   0        0        0      767 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/v1/__init__.py
+-rw-r--r--   0        0        0     3574 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/v1/cache.py
+-rw-r--r--   0        0        0     2634 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/v1/templates.py
+-rw-r--r--   0        0        0     1702 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/version.py
+-rw-r--r--   0        0        0     3873 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/views/workflow_plans.py
+-rw-r--r--   0        0        0     2890 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/ui/service/worker.py
+-rw-r--r--   0        0        0     1597 2023-05-15 19:30:40.173361 renku-2.4.1rc2/renku/version.py
+-rw-r--r--   0        0        0    17302 1970-01-01 00:00:00.000000 renku-2.4.1rc2/PKG-INFO
```

### Comparing `renku-2.4.1rc1/AUTHORS.rst` & `renku-2.4.1rc2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/CHANGES.rst` & `renku-2.4.1rc2/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/LICENSE` & `renku-2.4.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/README.rst` & `renku-2.4.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/pyproject.toml` & `renku-2.4.1rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool]
 
 [tool.poetry]
 name = "renku"
-version = "2.4.1rc1" # placeholder, see poetry-dynamic-versioning
+version = "2.4.1rc2" # placeholder, see poetry-dynamic-versioning
 description = "Python SDK and CLI for the Renku platform."
 license = "Apache License 2.0"
 keywords = ["Renku", "CLI"]
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
```

### Comparing `renku-2.4.1rc1/renku/__init__.py` & `renku-2.4.1rc2/renku/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/__init__.py` & `renku-2.4.1rc2/renku/command/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/__pycache__/run.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1600 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 4006 0000  a.......p.ad@...
+00000000: 610d 0d0a 0000 0000 6088 6264 4006 0000  a.......`.bd@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6406 6407 8400 5a0a 650b  m.Z...d.d...Z.e.
 00000070: 6503 6502 650c 1900 1900 6408 9c02 6409  e.e.e.....d...d.
```

### Comparing `renku-2.4.1rc1/renku/command/__pycache__/util.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/__pycache__/util.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 be06 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 be06 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6503 6a04 6403  Z.d.d.l.Z.e.j.d.
 00000050: 6404 6405 6406 8d03 5a05 6503 6a04 6407  d.d.d...Z.e.j.d.
 00000060: 6404 6408 6406 8d03 5a06 6503 6a04 6409  d.d.d...Z.e.j.d.
 00000070: 6404 640a 6406 8d03 5a07 640b 640c 8400  d.d.d...Z.d.d...
```

### Comparing `renku-2.4.1rc1/renku/command/__pycache__/version.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/__pycache__/version.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1088 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 4004 0000  a.......p.ad@...
+00000000: 610d 0d0a 0000 0000 6088 6264 4004 0000  a.......`.bd@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6403 6404 8400  Z.d.d.l.Z.d.d...
 00000040: 5a02 6402 5300 2905 7a15 5665 7273 696f  Z.d.S.).z.Versio
 00000050: 6e69 6e67 2075 7469 6c69 7469 6573 2ee9  ning utilities..
 00000060: 0000 0000 4e63 0300 0000 0000 0000 0000  ....Nc..........
 00000070: 0000 0400 0000 0300 0000 4300 0000 7330  ..........C...s0
```

### Comparing `renku-2.4.1rc1/renku/command/checks/__init__.py` & `renku-2.4.1rc2/renku/command/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/checks/activities.py` & `renku-2.4.1rc2/renku/command/checks/activities.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/checks/datasets.py` & `renku-2.4.1rc2/renku/command/checks/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/checks/githooks.py` & `renku-2.4.1rc2/renku/command/checks/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/checks/migration.py` & `renku-2.4.1rc2/renku/command/checks/migration.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/checks/project.py` & `renku-2.4.1rc2/renku/command/checks/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/checks/storage.py` & `renku-2.4.1rc2/renku/command/checks/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/checks/validate_shacl.py` & `renku-2.4.1rc2/renku/command/checks/validate_shacl.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/checks/workflow.py` & `renku-2.4.1rc2/renku/command/checks/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/clone.py` & `renku-2.4.1rc2/renku/command/clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/command_builder/__init__.py` & `renku-2.4.1rc2/renku/command/command_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/command_builder/__pycache__/command.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/command_builder/__pycache__/command.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 16678 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 2641 0000  a.......p.ad&A..
+00000000: 610d 0d0a 0000 0000 6088 6264 2641 0000  a.......`.bd&A..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/command/command_builder/command.py` & `renku-2.4.1rc2/renku/command/command_builder/command.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/command_builder/communication.py` & `renku-2.4.1rc2/renku/command/command_builder/communication.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/command_builder/database.py` & `renku-2.4.1rc2/renku/command/command_builder/database.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/command_builder/lock.py` & `renku-2.4.1rc2/renku/command/command_builder/lock.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/command_builder/migration.py` & `renku-2.4.1rc2/renku/command/command_builder/migration.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/command_builder/repo.py` & `renku-2.4.1rc2/renku/command/command_builder/repo.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/config.py` & `renku-2.4.1rc2/renku/command/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/dataset.py` & `renku-2.4.1rc2/renku/command/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/doctor.py` & `renku-2.4.1rc2/renku/command/doctor.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/format/__init__.py` & `renku-2.4.1rc2/renku/command/format/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/format/__pycache__/dataset_files.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/format/__pycache__/dataset_files.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6230 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 5618 0000  a.......p.adV...
+00000000: 610d 0d0a 0000 0000 6088 6264 5618 0000  a.......`.bdV...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 b800 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 6d05 5a05 0100  l.m.Z.m.Z.m.Z...
 00000050: 6401 6404 6c06 6d07 5a07 6d08 5a08 6d09  d.d.l.m.Z.m.Z.m.
 00000060: 5a09 6d0a 5a0a 0100 6401 6405 6c0b 6d0c  Z.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6402 6406 9c01 6407 6408 8402  Z...d.d...d.d...
```

### Comparing `renku-2.4.1rc1/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2098 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 3208 0000  a.......p.ad2...
+00000000: 610d 0d0a 0000 0000 6088 6264 3208 0000  a.......`.bd2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 5500  .....@...sP...U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6401 6403 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6404 6405 8400 5a06 6406 6407 8400 5a07  d.d...Z.d.d...Z.
 00000060: 6506 6507 6408 9c02 5a08 6505 6509 6504  e.e.d...Z.e.e.e.
 00000070: 6602 1900 650a 6409 3c00 640a 5300 290b  f...e.d.<.d.S.).
```

### Comparing `renku-2.4.1rc1/renku/command/format/__pycache__/datasets.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/format/__pycache__/datasets.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3236 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 a40c 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 a40c 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 9200 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6402 6405 9c01 6406  l.m.Z...d.d...d.
 00000060: 6407 8402 5a07 6408 6409 8400 5a08 640a  d...Z.d.d...Z.d.
 00000070: 640b 8400 5a09 640c 640d 8400 5a0a 6507  d...Z.d.d...Z.e.
```

### Comparing `renku-2.4.1rc1/renku/command/format/__pycache__/json.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/format/__pycache__/json.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 bc04 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 bc04 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6503 6a06 8303 5a06 6502 6a07 6503 6a08  e.j...Z.e.j.e.j.
 00000070: 6506 6406 8d02 5a08 6402 5300 2907 7a1b  e.d...Z.d.S.).z.
```

### Comparing `renku-2.4.1rc1/renku/command/format/__pycache__/session.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/format/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2402 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6209 0000  a.......p.adb...
+00000000: 610d 0d0a 0000 0000 6088 6264 6209 0000  a.......`.bdb...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6405 6406 9c01  d.l.m.Z...d.d...
 00000060: 6502 6507 1900 6503 6508 1900 6407 9c02  e.e...e.e...d...
 00000070: 6408 6409 8406 5a09 6405 6406 9c01 6502  d.d...Z.d.d...e.
```

### Comparing `renku-2.4.1rc1/renku/command/format/__pycache__/tabulate.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/format/__pycache__/tabulate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2769 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 d10a 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 d10a 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 640d 6507 6408 9c01 6409  m.Z...d.e.d...d.
 00000060: 640a 8405 5a08 640b 640c 8400 5a09 6405  d...Z.d.d...Z.d.
 00000070: 5300 290e 7a20 5461 6275 6c61 7220 666f  S.).z Tabular fo
```

### Comparing `renku-2.4.1rc1/renku/command/format/__pycache__/workflow.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/format/__pycache__/workflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2728 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 a80a 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 a80a 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9600 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6401 6405 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a08 0100 6402 6406 9c01 6407 6408 8402  Z...d.d...d.d...
 00000070: 5a09 6409 640a 8400 5a0a 640b 640c 8400  Z.d.d...Z.d.d...
```

### Comparing `renku-2.4.1rc1/renku/command/format/activity.py` & `renku-2.4.1rc2/renku/command/format/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/format/dataset_files.py` & `renku-2.4.1rc2/renku/command/format/dataset_files.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/format/dataset_tags.py` & `renku-2.4.1rc2/renku/command/format/dataset_tags.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/format/datasets.py` & `renku-2.4.1rc2/renku/command/format/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/format/json.py` & `renku-2.4.1rc2/renku/command/format/json.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/format/session.py` & `renku-2.4.1rc2/renku/command/format/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/format/tabulate.py` & `renku-2.4.1rc2/renku/command/format/tabulate.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/format/workflow.py` & `renku-2.4.1rc2/renku/command/format/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/gc.py` & `renku-2.4.1rc2/renku/command/gc.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/githooks.py` & `renku-2.4.1rc2/renku/command/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/graph.py` & `renku-2.4.1rc2/renku/command/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/group.py` & `renku-2.4.1rc2/renku/command/group.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/init.py` & `renku-2.4.1rc2/renku/command/init.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/log.py` & `renku-2.4.1rc2/renku/command/log.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/login.py` & `renku-2.4.1rc2/renku/command/login.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/mergetool.py` & `renku-2.4.1rc2/renku/command/mergetool.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/migrate.py` & `renku-2.4.1rc2/renku/command/migrate.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/move.py` & `renku-2.4.1rc2/renku/command/move.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/options.py` & `renku-2.4.1rc2/renku/command/options.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/project.py` & `renku-2.4.1rc2/renku/command/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/remove.py` & `renku-2.4.1rc2/renku/command/remove.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/rerun.py` & `renku-2.4.1rc2/renku/command/rerun.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/rollback.py` & `renku-2.4.1rc2/renku/command/rollback.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/run.py` & `renku-2.4.1rc2/renku/command/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/save.py` & `renku-2.4.1rc2/renku/command/save.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/__init__.py` & `renku-2.4.1rc2/renku/command/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/__pycache__/agent.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/schema/__pycache__/agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1744 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 d006 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 d006 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
 00000070: 0100 4700 6406 6407 8400 6407 6502 8303  ..G.d.d...d.e...
```

### Comparing `renku-2.4.1rc1/renku/command/schema/__pycache__/annotation.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/schema/__pycache__/annotation.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1235 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 d304 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 d304 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a0a 6407 5300 2908 7a1a 416e 6e6f 7461  Z.d.S.).z.Annota
```

### Comparing `renku-2.4.1rc1/renku/command/schema/__pycache__/calamus.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/schema/__pycache__/calamus.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 8986 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 1a23 0000  a.......p.ad.#..
+00000000: 610d 0d0a 0000 0000 6088 6264 1a23 0000  a.......`.bd.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6406 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/command/schema/__pycache__/dataset.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/schema/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 8210 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 1220 0000  a.......p.ad. ..
+00000000: 610d 0d0a 0000 0000 6088 6264 1220 0000  a.......`.bd. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/command/schema/__pycache__/entity.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/schema/__pycache__/entity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1445 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 a505 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 a505 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c07 6d08 5a08 6d09 5a09 0100 4700  d.l.m.Z.m.Z...G.
 00000060: 6404 6405 8400 6405 6502 8303 5a0a 4700  d.d...d.e...Z.G.
 00000070: 6406 6407 8400 6407 650a 8303 5a0b 6408  d.d...d.e...Z.d.
```

### Comparing `renku-2.4.1rc1/renku/command/schema/activity.py` & `renku-2.4.1rc2/renku/command/schema/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/agent.py` & `renku-2.4.1rc2/renku/command/schema/agent.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/annotation.py` & `renku-2.4.1rc2/renku/command/schema/annotation.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/calamus.py` & `renku-2.4.1rc2/renku/command/schema/calamus.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/composite_plan.py` & `renku-2.4.1rc2/renku/command/schema/composite_plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/dataset.py` & `renku-2.4.1rc2/renku/command/schema/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/entity.py` & `renku-2.4.1rc2/renku/command/schema/entity.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/parameter.py` & `renku-2.4.1rc2/renku/command/schema/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/plan.py` & `renku-2.4.1rc2/renku/command/schema/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/project.py` & `renku-2.4.1rc2/renku/command/schema/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/schema/workflow_file.py` & `renku-2.4.1rc2/renku/command/schema/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/session.py` & `renku-2.4.1rc2/renku/command/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/status.py` & `renku-2.4.1rc2/renku/command/status.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/storage.py` & `renku-2.4.1rc2/renku/command/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/template.py` & `renku-2.4.1rc2/renku/command/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/update.py` & `renku-2.4.1rc2/renku/command/update.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/util.py` & `renku-2.4.1rc2/renku/command/util.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/version.py` & `renku-2.4.1rc2/renku/command/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/__init__.py` & `renku-2.4.1rc2/renku/command/view_model/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 13979 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 9b36 0000  a.......p.ad.6..
+00000000: 610d 0d0a 0000 0000 6088 6264 9b36 0000  a.......`.bd.6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6401 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/command/view_model/__pycache__/agent.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/view_model/__pycache__/agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1657 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 7906 0000  a.......p.ady...
+00000000: 610d 0d0a 0000 0000 6088 6264 7906 0000  a.......`.bdy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a05 6406 5300 2907 7a11  ..d...Z.d.S.).z.
 00000060: 4167 656e 7420 7669 6577 206d 6f64 656c  Agent view model
 00000070: 2ee9 0000 0000 2901 da08 4f70 7469 6f6e  ......)...Option
```

### Comparing `renku-2.4.1rc1/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 8768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 4022 0000  a.......p.ad@"..
+00000000: 610d 0d0a 0000 0000 6088 6264 4022 0000  a.......`.bd@"..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 3001 0000 5500  .....@...s0...U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d02 5a02 6d03 5a03 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c04 6d05 5a05 6d06 5a06 6d07 5a07 6d08  l.m.Z.m.Z.m.Z.m.
 00000060: 5a08 6d09 5a09 6d0a 5a0a 0100 6401 6405  Z.m.Z.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 6401 6406 6c0d 6d0e  l.m.Z...d.d.l.m.
```

### Comparing `renku-2.4.1rc1/renku/command/view_model/__pycache__/log.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/view_model/__pycache__/log.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 12497 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 d130 0000  a.......p.ad.0..
+00000000: 610d 0d0a 0000 0000 6088 6264 d130 0000  a.......`.bd.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d04 5a04 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6406 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/command/view_model/__pycache__/plan.cpython-39.pyc` & `renku-2.4.1rc2/renku/command/view_model/__pycache__/plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 9377 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 a124 0000  a.......p.ad.$..
+00000000: 610d 0d0a 0000 0000 6088 6264 a124 0000  a.......`.bd.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 e400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6401 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6401 6407 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/command/view_model/activity_graph.py` & `renku-2.4.1rc2/renku/command/view_model/activity_graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/agent.py` & `renku-2.4.1rc2/renku/command/view_model/agent.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/composite_plan.py` & `renku-2.4.1rc2/renku/command/view_model/composite_plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/dataset.py` & `renku-2.4.1rc2/renku/command/view_model/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/graph.py` & `renku-2.4.1rc2/renku/command/view_model/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/log.py` & `renku-2.4.1rc2/renku/command/view_model/log.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/plan.py` & `renku-2.4.1rc2/renku/command/view_model/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/project.py` & `renku-2.4.1rc2/renku/command/view_model/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/template.py` & `renku-2.4.1rc2/renku/command/view_model/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/text_canvas.py` & `renku-2.4.1rc2/renku/command/view_model/text_canvas.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/view_model/workflow_file.py` & `renku-2.4.1rc2/renku/command/view_model/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/command/workflow.py` & `renku-2.4.1rc2/renku/command/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/__init__.py` & `renku-2.4.1rc2/renku/core/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/__pycache__/config.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/__pycache__/config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6170 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 1a18 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 1a18 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6407 6408 8400 5a0b 6409 640a 8400  ..d.d...Z.d.d...
```

### Comparing `renku-2.4.1rc1/renku/core/__pycache__/constant.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/__pycache__/constant.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2717 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 9d0a 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 9d0a 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 d200 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6401 6404 6c04 6d05  l.m.Z...d.d.l.m.
 00000050: 5a05 0100 6405 5a06 6406 5a07 6407 5a08  Z...d.Z.d.Z.d.Z.
 00000060: 6408 5a09 6409 5a0a 6501 6a0b a00c 6507  d.Z.d.Z.e.j...e.
 00000070: 650a a102 5a0d 640a 5a0e 640b 5a0f 6510  e...Z.d.Z.d.Z.e.
```

### Comparing `renku-2.4.1rc1/renku/core/__pycache__/errors.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/__pycache__/errors.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 25658 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 3a64 0000  a.......p.ad:d..
+00000000: 610d 0d0a 0000 0000 6088 6264 3a64 0000  a.......`.bd:d..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5c06 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6401 6404 6c07 5a07 6401 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 650c 8303  ..G.d.d...d.e...
```

### Comparing `renku-2.4.1rc1/renku/core/__pycache__/git.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 7394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 e21c 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 e21c 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/__pycache__/login.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/__pycache__/login.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 10639 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8f29 0000  a.......p.ad.)..
+00000000: 610d 0d0a 0000 0000 6088 6264 8f29 0000  a.......`.bd.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 0100 6401 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/__pycache__/storage.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/__pycache__/storage.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 21861 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6555 0000  a.......p.adeU..
+00000000: 610d 0d0a 0000 0000 6088 6264 6555 0000  a.......`.bdeU..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c02 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6402 6c07 5a07 6401 6403 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 6d09 5a09 0100 6401 6404 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/config.py` & `renku-2.4.1rc2/renku/core/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/constant.py` & `renku-2.4.1rc2/renku/core/constant.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/__init__.py` & `renku-2.4.1rc2/renku/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 9747 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 1326 0000  a.......p.ad.&..
+00000000: 610d 0d0a 0000 0000 6088 6264 1326 0000  a.......`.bd.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6401 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/context.py` & `renku-2.4.1rc2/renku/core/dataset/context.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/dataset.py` & `renku-2.4.1rc2/renku/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/dataset_add.py` & `renku-2.4.1rc2/renku/core/dataset/dataset_add.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/datasets_provenance.py` & `renku-2.4.1rc2/renku/core/dataset/datasets_provenance.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/pointer_file.py` & `renku-2.4.1rc2/renku/core/dataset/pointer_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__init__.py` & `renku-2.4.1rc2/renku/core/dataset/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 12028 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 fc2e 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 fc2e 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6c01 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6966 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 361b 0000  a.......p.ad6...
+00000000: 610d 0d0a 0000 0000 6088 6264 361b 0000  a.......`.bd6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1401 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2225 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 b108 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 b108 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6408 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 20652 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 ac50 0000  a.......p.ad.P..
+00000000: 610d 0d0a 0000 0000 6088 6264 ac50 0000  a.......`.bd.P..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 da01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3317 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 f50c 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 f50c 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5300 2905 7a1d 4461 7461 7665 7273 6520  S.).z.Dataverse 
 00000050: 6d65 7461 6461 7461 2074 656d 706c 6174  metadata templat
 00000060: 6573 2e61 fc06 0000 0a7b 0a20 2020 2022  es.a.....{.    "
 00000070: 6461 7461 7365 7456 6572 7369 6f6e 223a  datasetVersion":
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 4808 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 c812 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 c812 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6407 5a0e 4700  m.Z.m.Z...d.Z.G.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5602 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 e215 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 e215 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0173 1001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6401 6407 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5764 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8416 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 8416 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6404 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 0100 6401 6406 6c0f  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 7300 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 841c 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 841c 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 f600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6406 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 11965 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 bd2e 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 bd2e 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5869 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 ed16 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 ed16 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 10097 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 7127 0000  a.......p.adq'..
+00000000: 610d 0d0a 0000 0000 6088 6264 7127 0000  a.......`.bdq'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 f000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c02 6d09 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6401  d.l.m.Z.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 22146 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8256 0000  a.......p.ad.V..
+00000000: 610d 0d0a 0000 0000 6088 6264 8256 0000  a.......`.bd.V..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2553 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 f909 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 f909 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6401  d.l.m.Z.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6506 7258 6401  d.l.m.Z...e.rXd.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6401 6407 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6392 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 f818 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 f818 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5813 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 b516 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 b516 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 18624 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 c048 0000  a.......p.ad.H..
+00000000: 610d 0d0a 0000 0000 6088 6264 c048 0000  a.......`.bd.H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/api.py` & `renku-2.4.1rc2/renku/core/dataset/providers/api.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/azure.py` & `renku-2.4.1rc2/renku/core/dataset/providers/azure.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/common.py` & `renku-2.4.1rc2/renku/core/dataset/providers/common.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/dataverse.py` & `renku-2.4.1rc2/renku/core/dataset/providers/dataverse.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/dataverse_metadata_templates.py` & `renku-2.4.1rc2/renku/core/dataset/providers/dataverse_metadata_templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/doi.py` & `renku-2.4.1rc2/renku/core/dataset/providers/doi.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/external.py` & `renku-2.4.1rc2/renku/core/dataset/providers/external.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/factory.py` & `renku-2.4.1rc2/renku/core/dataset/providers/factory.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/git.py` & `renku-2.4.1rc2/renku/core/dataset/providers/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/local.py` & `renku-2.4.1rc2/renku/core/dataset/providers/local.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/models.py` & `renku-2.4.1rc2/renku/core/dataset/providers/models.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/olos.py` & `renku-2.4.1rc2/renku/core/dataset/providers/olos.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/renku.py` & `renku-2.4.1rc2/renku/core/dataset/providers/renku.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/repository.py` & `renku-2.4.1rc2/renku/core/dataset/providers/repository.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/s3.py` & `renku-2.4.1rc2/renku/core/dataset/providers/s3.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/web.py` & `renku-2.4.1rc2/renku/core/dataset/providers/web.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/providers/zenodo.py` & `renku-2.4.1rc2/renku/core/dataset/providers/zenodo.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/request_model.py` & `renku-2.4.1rc2/renku/core/dataset/request_model.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/dataset/tag.py` & `renku-2.4.1rc2/renku/core/dataset/tag.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/errors.py` & `renku-2.4.1rc2/renku/core/errors.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/gc.py` & `renku-2.4.1rc2/renku/core/gc.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/git.py` & `renku-2.4.1rc2/renku/core/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/githooks.py` & `renku-2.4.1rc2/renku/core/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/init.py` & `renku-2.4.1rc2/renku/core/init.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/interface/__init__.py` & `renku-2.4.1rc2/renku/core/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3741 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 9d0e 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 9d0e 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 6d0d 5a0d 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
```

### Comparing `renku-2.4.1rc1/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1418 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8a05 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 8a05 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6504  d.l.m.Z.m.Z...e.
 00000050: 7230 6401 6404 6c06 6d07 5a07 0100 4700  r0d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6502 8303 5a08 6407  d.d...d.e...Z.d.
 00000070: 5300 2908 7a21 5265 6e6b 7520 6461 7461  S.).z!Renku data
```

### Comparing `renku-2.4.1rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2095 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 2f08 0000  a.......p.ad/...
+00000000: 610d 0d0a 0000 0000 6088 6264 2f08 0000  a.......`.bd/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6504 7238 6401 6404 6c07 6d08 5a08  ..e.r8d.d.l.m.Z.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6502 8303 5a0a 6407 5300 2908 7a20 5265  e...Z.d.S.).z Re
```

### Comparing `renku-2.4.1rc1/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1996 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 cc07 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 cc07 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6401 6404 6c07 6d08 5a08 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6502 8303 5a09 6407  d.d...d.e...Z.d.
 00000070: 5300 2908 7a1d 5265 6e6b 7520 706c 616e  S.).z.Renku plan
```

### Comparing `renku-2.4.1rc1/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 bc04 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 bc04 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6504 722c 6401  d.l.m.Z...e.r,d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6502 8303 5a07 6407 5300 2908  ..d.e...Z.d.S.).
 00000070: 7a20 5265 6e6b 7520 7072 6f6a 6563 7420  z Renku project
```

### Comparing `renku-2.4.1rc1/renku/core/interface/__pycache__/storage.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/interface/__pycache__/storage.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 4226 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8210 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 8210 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6507  m.Z.m.Z.m.Z...e.
 00000070: 7254 6401 6406 6c0c 6d0d 5a0d 6d0e 5a0e  rTd.d.l.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1780 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 f406 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 f406 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6509  m.Z.m.Z.m.Z...e.
 00000070: 7250 6401 6406 6c0c 6d0d 5a0d 0100 4700  rPd.d.l.m.Z...G.
```

### Comparing `renku-2.4.1rc1/renku/core/interface/activity_gateway.py` & `renku-2.4.1rc2/renku/core/interface/activity_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/interface/database_gateway.py` & `renku-2.4.1rc2/renku/core/interface/database_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/interface/dataset_gateway.py` & `renku-2.4.1rc2/renku/core/interface/dataset_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/interface/plan_gateway.py` & `renku-2.4.1rc2/renku/core/interface/plan_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/interface/project_gateway.py` & `renku-2.4.1rc2/renku/core/interface/project_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/interface/storage.py` & `renku-2.4.1rc2/renku/core/interface/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/interface/workflow_file_parser.py` & `renku-2.4.1rc2/renku/core/interface/workflow_file_parser.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/login.py` & `renku-2.4.1rc2/renku/core/login.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/__init__.py` & `renku-2.4.1rc2/renku/core/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0003__0_pyld2.py` & `renku-2.4.1rc2/renku/core/migration/m_0003__0_pyld2.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0003__1_jsonld.py` & `renku-2.4.1rc2/renku/core/migration/m_0003__1_jsonld.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0003__2_initial.py` & `renku-2.4.1rc2/renku/core/migration/m_0003__2_initial.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0004__0_pyld2.py` & `renku-2.4.1rc2/renku/core/migration/m_0004__0_pyld2.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0004__submodules.py` & `renku-2.4.1rc2/renku/core/migration/m_0004__submodules.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0005__1_pyld2.py` & `renku-2.4.1rc2/renku/core/migration/m_0005__1_pyld2.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0005__2_cwl.py` & `renku-2.4.1rc2/renku/core/migration/m_0005__2_cwl.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0006__dataset_context.py` & `renku-2.4.1rc2/renku/core/migration/m_0006__dataset_context.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0007__source_url.py` & `renku-2.4.1rc2/renku/core/migration/m_0007__source_url.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0008__dataset_metadata.py` & `renku-2.4.1rc2/renku/core/migration/m_0008__dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0009__new_metadata_storage.py` & `renku-2.4.1rc2/renku/core/migration/m_0009__new_metadata_storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/m_0010__metadata_fixes.py` & `renku-2.4.1rc2/renku/core/migration/m_0010__metadata_fixes.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/migrate.py` & `renku-2.4.1rc2/renku/core/migration/migrate.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/models/__init__.py` & `renku-2.4.1rc2/renku/core/migration/models/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/models/migration.py` & `renku-2.4.1rc2/renku/core/migration/models/migration.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/models/refs.py` & `renku-2.4.1rc2/renku/core/migration/models/refs.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/models/v10.py` & `renku-2.4.1rc2/renku/core/migration/models/v10.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/models/v3.py` & `renku-2.4.1rc2/renku/core/migration/models/v3.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/models/v7.py` & `renku-2.4.1rc2/renku/core/migration/models/v7.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/models/v8.py` & `renku-2.4.1rc2/renku/core/migration/models/v8.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/models/v9.py` & `renku-2.4.1rc2/renku/core/migration/models/v9.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/utils/__init__.py` & `renku-2.4.1rc2/renku/core/migration/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 7865 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 b91e 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 b91e 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 ec00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6404 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/migration/utils/conversion.py` & `renku-2.4.1rc2/renku/core/migration/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/plugin/__init__.py` & `renku-2.4.1rc2/renku/core/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1467 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 bb05 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 bb05 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 5a05 6502  m.Z...d.d.l.Z.e.
 00000050: 7230 6401 6404 6c06 6d07 5a07 0100 6505  r0d.d.l.m.Z...e.
 00000060: a008 6405 a101 5a09 6509 6406 6407 9c01  ..d...Z.e.d.d...
 00000070: 6408 6409 8404 8301 5a0a 640a 6407 9c01  d.d.....Z.d.d...
```

### Comparing `renku-2.4.1rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1790 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 fe06 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 fe06 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6502 6403 8301 6404 6405  d.l.Z.e.d...d.d.
 00000050: 8400 8301 5a04 6403 5300 2906 7a14 706c  ....Z.d.S.).z.pl
 00000060: 7567 6779 2050 6c75 6769 6e20 7365 7475  uggy Plugin setu
 00000070: 702e e900 0000 0029 01da 096c 7275 5f63  p......)...lru_c
```

### Comparing `renku-2.4.1rc1/renku/core/plugin/__pycache__/provider.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/plugin/__pycache__/provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3357 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 1d0d 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 1d0d 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6504 7238 6401  m.Z.m.Z...e.r8d.
 00000060: 6404 6c09 5a0a 6401 6404 6c0b 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6401 6406 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/plugin/__pycache__/run.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/plugin/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1839 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 2f07 0000  a.......p.ad/...
+00000000: 610d 0d0a 0000 0000 6088 6264 2f07 0000  a.......`.bd/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 6403  Z.d.d.l.Z.e...d.
 00000040: a101 5a03 6503 6404 6405 8400 8301 5a04  ..Z.e.d.d.....Z.
 00000050: 6503 6406 6407 8400 8301 5a05 6503 6408  e.d.d.....Z.e.d.
 00000060: 6409 8400 8301 5a06 6402 5300 290a 7a29  d.....Z.d.S.).z)
 00000070: 506c 7567 696e 2068 6f6f 6b73 2066 6f72  Plugin hooks for
```

### Comparing `renku-2.4.1rc1/renku/core/plugin/__pycache__/session.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/plugin/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1454 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 ae05 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 ae05 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a04 6401 6404 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6504 a007 6405 a101 5a08  m.Z...e...d...Z.
 00000060: 6508 6503 6506 6509 6602 1900 6406 9c01  e.e.e.e.f...d...
 00000070: 6407 6408 8404 8301 5a0a 6502 6506 1900  d.d.....Z.e.e...
```

### Comparing `renku-2.4.1rc1/renku/core/plugin/__pycache__/workflow.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/plugin/__pycache__/workflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 4195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6310 0000  a.......p.adc...
+00000000: 610d 0d0a 0000 0000 6088 6264 6310 0000  a.......`.bdc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3065 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 f90b 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 f90b 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6504 7258 6401 6407 6c0d  m.Z...e.rXd.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/plugin/dataset_provider.py` & `renku-2.4.1rc2/renku/core/plugin/dataset_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/plugin/implementations/__init__.py` & `renku-2.4.1rc2/renku/core/plugin/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3046 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 e60b 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 e60b 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 ca01 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 6d03  d.Z.d.d.l.m.Z.m.
 00000040: 5a03 6d04 5a04 0100 6401 6403 6c05 6d06  Z.m.Z...d.d.l.m.
 00000050: 5a06 0100 6401 6404 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 6401 6405 6c09 6d0a 5a0a 0100 6401 6406  d.d.l.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 6401 6407 6c0d 6d0e  l.m.Z...d.d.l.m.
```

### Comparing `renku-2.4.1rc1/renku/core/plugin/pluginmanager.py` & `renku-2.4.1rc2/renku/core/plugin/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/plugin/provider.py` & `renku-2.4.1rc2/renku/core/plugin/provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/plugin/run.py` & `renku-2.4.1rc2/renku/core/plugin/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/plugin/session.py` & `renku-2.4.1rc2/renku/core/plugin/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/plugin/workflow.py` & `renku-2.4.1rc2/renku/core/plugin/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/plugin/workflow_file_parser.py` & `renku-2.4.1rc2/renku/core/plugin/workflow_file_parser.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/project.py` & `renku-2.4.1rc2/renku/core/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/session/__init__.py` & `renku-2.4.1rc2/renku/core/session/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/session/__pycache__/docker.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/session/__pycache__/docker.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 14350 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 0e38 0000  a.......p.ad.8..
+00000000: 610d 0d0a 0000 0000 6088 6264 0e38 0000  a.......`.bd.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 f800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/session/__pycache__/renkulab.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/session/__pycache__/renkulab.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 20534 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 3650 0000  a.......p.ad6P..
+00000000: 610d 0d0a 0000 0000 6088 6264 3650 0000  a.......`.bd6P..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6406 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/session/__pycache__/utils.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/session/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2215 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 a708 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 a708 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 650b 6407 9c01 6408 6409 8404 5a0c  ..e.d...d.d...Z.
```

### Comparing `renku-2.4.1rc1/renku/core/session/docker.py` & `renku-2.4.1rc2/renku/core/session/docker.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/session/renkulab.py` & `renku-2.4.1rc2/renku/core/session/renkulab.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/session/session.py` & `renku-2.4.1rc2/renku/core/session/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/session/utils.py` & `renku-2.4.1rc2/renku/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/storage.py` & `renku-2.4.1rc2/renku/core/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/template/__init__.py` & `renku-2.4.1rc2/renku/core/template/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/template/template.py` & `renku-2.4.1rc2/renku/core/template/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/template/usecase.py` & `renku-2.4.1rc2/renku/core/template/usecase.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/__init__.py` & `renku-2.4.1rc2/renku/core/util/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/communication.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/communication.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 10282 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 2a28 0000  a.......p.ad*(..
+00000000: 610d 0d0a 0000 0000 6088 6264 2a28 0000  a.......`.bd*(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5201 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 8302 5a08 6407 6408 8400 5a09  ..d...Z.d.d...Z.
 00000070: 6409 640a 8400 5a0a 4700 640b 640c 8400  d.d...Z.G.d.d...
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/contexts.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/contexts.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6617 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 d919 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 d919 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 5601 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6401 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/datetime8601.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/datetime8601.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2313 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 0909 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 0909 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a02 6d03 5a03 0100 6401 6404 6c04  m.Z.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6405 5a06 6501 a007 6506  m.Z...d.Z.e...e.
 00000060: a101 6a08 5a09 6406 6407 8400 5a0a 6408  ..j.Z.d.d...Z.d.
 00000070: 6409 8400 5a0b 6505 6502 1900 640a 9c01  d...Z.e.e...d...
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/doi.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/doi.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1376 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6005 0000  a.......p.ad`...
+00000000: 610d 0d0a 0000 0000 6088 6264 6005 0000  a.......`.bd`...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6501 6a03 6403 6501 6a04 6404 8d02  Z.e.j.d.e.j.d...
 00000050: 5a05 6405 6406 8400 5a06 6407 6408 8400  Z.d.d...Z.d.d...
 00000060: 5a07 6508 6409 9c01 640a 640b 8404 5a09  Z.e.d...d.d...Z.
 00000070: 6402 5300 290c 7a23 4865 6c70 6572 2075  d.S.).z#Helper u
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/git.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 40689 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 f19e 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 f19e 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 5c04 0000 5500  .....@...s\...U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6402 6c03 5a03 6401 6402  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 5a04 6401 6402 6c05 5a05 6401 6402  l.Z.d.d.l.Z.d.d.
 00000060: 6c06 5a06 6401 6402 6c07 5a07 6401 6402  l.Z.d.d.l.Z.d.d.
 00000070: 6c08 5a08 6401 6403 6c09 6d0a 5a0a 0100  l.Z.d.d.l.m.Z...
@@ -627,17 +627,17 @@
 00002720: 2020 2020 2020 2020 7061 7468 2855 6e69          path(Uni
 00002730: 6f6e 5b50 6174 682c 2073 7472 5d29 3a20  on[Path, str]): 
 00002740: 5468 6520 7061 7468 2074 6f20 6368 6563  The path to chec
 00002750: 6b2e 0a0a 2020 2020 5265 7475 726e 733a  k...    Returns:
 00002760: 0a20 2020 2020 2020 2062 6f6f 6c3a 2054  .        bool: T
 00002770: 7275 6520 6966 2074 6865 2070 6174 6820  rue if the path 
 00002780: 6973 2073 6166 6520 656c 7365 2046 616c  is safe else Fal
-00002790: 7365 2e0a 2020 2020 3e02 0000 007a 0e2e  se..    >....z..
-000027a0: 6769 7461 7474 7269 6275 7465 737a 0a2e  gitattributesz..
-000027b0: 6769 7469 676e 6f72 6546 7a06 2e72 656e  gitignoreFz..ren
+00002790: 7365 2e0a 2020 2020 3e02 0000 007a 0a2e  se..    >....z..
+000027a0: 6769 7469 676e 6f72 657a 0e2e 6769 7461  gitignorez..gita
+000027b0: 7474 7269 6275 7465 7346 7a06 2e72 656e  ttributesFz..ren
 000027c0: 6b75 5429 02da 0373 7472 725b 0000 00a9  kuT)...strr[....
 000027d0: 0172 3700 0000 722e 0000 0072 2e00 0000  .r7...r....r....
 000027e0: 722f 0000 00da 0c69 735f 7061 7468 5f73  r/.....is_path_s
 000027f0: 6166 655d 0100 0073 0c00 0000 0009 0803  afe]...s........
 00002800: 0801 0403 0a01 0402 7293 0000 0046 7214  ........r....Fr.
 00002810: 0000 0029 0672 3100 0000 7237 0000 00da  ...).r1...r7....
 00002820: 0872 6576 6973 696f 6eda 0c62 7970 6173  .revision..bypas
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/jwt.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/jwt.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1244 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 dc04 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 dc04 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 6d02 5a02  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c03 5a03 6504 6505 6404  ..d.d.l.Z.e.e.d.
 00000050: 9c02 6405 6406 8404 5a06 6403 5300 2907  ..d.d...Z.d.S.).
 00000060: 7a0e 4a57 5420 7574 696c 6974 6965 732e  z.JWT utilities.
 00000070: e900 0000 0029 02da 0864 6174 6574 696d  .....)...datetim
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/metadata.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/metadata.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 7036 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 7c1b 0000  a.......p.ad|...
+00000000: 610d 0d0a 0000 0000 6088 6264 7c1b 0000  a.......`.bd|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1e02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/os.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/os.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 12140 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6c2f 0000  a.......p.adl/..
+00000000: 610d 0d0a 0000 0000 6088 6264 6c2f 0000  a.......`.bdl/..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0015 0000 0040 0000 0073 5a03 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6402 6c07 5a07 6401 6402 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 5a08 6401 6403 6c09 6d0a 5a0a 0100 6401  Z.d.d.l.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/requests.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/requests.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 7626 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 ca1d 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 ca1d 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5801 0000 6400  .....@...sX...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6402 6c0a 5a0a 6401 6402 6c0b 5a0b 6401  d.l.Z.d.d.l.Z.d.
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/ssh.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/ssh.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6871 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 d71a 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 d71a 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6403 6c04 6d05 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0c 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0d 6d0e 5a0e 0100 6401 6407 6c0f  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/urls.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/urls.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6228 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 5418 0000  a.......p.adT...
+00000000: 610d 0d0a 0000 0000 6088 6264 5418 0000  a.......`.bdT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4601 0000 6400  .....@...sF...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6405 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/util.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/util.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3878 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 260f 0000  a.......p.ad&...
+00000000: 610d 0d0a 0000 0000 6088 6264 260f 0000  a.......`.bd&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 f200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 5a04 6401 6403 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6401 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 0100 6401 6402 6c0e 5a0e 6401  m.Z...d.d.l.Z.d.
```

### Comparing `renku-2.4.1rc1/renku/core/util/__pycache__/yaml.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/util/__pycache__/yaml.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2836 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 140b 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 140b 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 5a05 7a1c 6401 6405 6c05 6d06 5a07 0100  Z.z.d.d.l.m.Z...
 00000060: 6401 6406 6c05 6d08 5a09 0100 5700 6e22  d.d.l.m.Z...W.n"
 00000070: 0400 650a 7962 0100 0100 0100 6401 6407  ..e.yb......d.d.
```

### Comparing `renku-2.4.1rc1/renku/core/util/communication.py` & `renku-2.4.1rc2/renku/core/util/communication.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/contexts.py` & `renku-2.4.1rc2/renku/core/util/contexts.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/datetime8601.py` & `renku-2.4.1rc2/renku/core/util/datetime8601.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/doi.py` & `renku-2.4.1rc2/renku/core/util/doi.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/git.py` & `renku-2.4.1rc2/renku/core/util/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/jwt.py` & `renku-2.4.1rc2/renku/core/util/jwt.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/metadata.py` & `renku-2.4.1rc2/renku/core/util/metadata.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/os.py` & `renku-2.4.1rc2/renku/core/util/os.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/requests.py` & `renku-2.4.1rc2/renku/core/util/requests.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/shacl.py` & `renku-2.4.1rc2/renku/core/util/shacl.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/ssh.py` & `renku-2.4.1rc2/renku/core/util/ssh.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/tabulate.py` & `renku-2.4.1rc2/renku/core/util/tabulate.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/urls.py` & `renku-2.4.1rc2/renku/core/util/urls.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/util.py` & `renku-2.4.1rc2/renku/core/util/util.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/util/yaml.py` & `renku-2.4.1rc2/renku/core/util/yaml.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/__init__.py` & `renku-2.4.1rc2/renku/core/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/__pycache__/activity.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/__pycache__/activity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 22713 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 b958 0000  a.......p.ad.X..
+00000000: 610d 0d0a 0000 0000 6088 6264 b958 0000  a.......`.bd.X..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 4402 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/__pycache__/execute.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/__pycache__/execute.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 18756 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 4449 0000  a.......p.adDI..
+00000000: 610d 0d0a 0000 0000 6088 6264 4449 0000  a.......`.bdDI..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 8402 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/__pycache__/plan.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/__pycache__/plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 34209 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 a185 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 a185 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0016 0000 0040 0000 0073 2406 0000 6400  .....@...s$...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d03 5a03 6d04 5a04  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c05 6d06 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 33046 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 1681 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 1681 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ee01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/__pycache__/run.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 13562 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 fa34 0000  a.......p.ad.4..
+00000000: 610d 0d0a 0000 0000 6088 6264 fa34 0000  a.......`.bd.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 e201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/__pycache__/types.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/__pycache__/types.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1681 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 9106 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 9106 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 4700 6405 6406  m.Z.m.Z...G.d.d.
 00000060: 8400 6406 8302 5a08 4700 6407 6408 8400  ..d...Z.G.d.d...
 00000070: 6408 6508 8303 5a09 4700 6409 640a 8400  d.e...Z.G.d.d...
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 8335 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8f20 0000  a.......p.ad. ..
+00000000: 610d 0d0a 0000 0000 6088 6264 8f20 0000  a.......`.bd. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5089 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 e113 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 e113 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0173 3401 0000 6400  .....@...s4...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6403 6c0a 5a0b 6401  m.Z...d.d.l.Z.d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6401 6407 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/activity.py` & `renku-2.4.1rc2/renku/core/workflow/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/converters/__init__.py` & `renku-2.4.1rc2/renku/core/workflow/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 17930 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 0a46 0000  a.......p.ad.F..
+00000000: 610d 0d0a 0000 0000 6088 6264 0a46 0000  a.......`.bd.F..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6405 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5142 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 1614 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 1614 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/converters/cwl.py` & `renku-2.4.1rc2/renku/core/workflow/converters/cwl.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/converters/renku.py` & `renku-2.4.1rc2/renku/core/workflow/converters/renku.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/execute.py` & `renku-2.4.1rc2/renku/core/workflow/execute.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/model/__init__.py` & `renku-2.4.1rc2/renku/core/workflow/model/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8219 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 8219 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 5a0b 6401 6406 6c0c  ..d.d.l.Z.d.d.l.
 00000070: 6d0d 5a0d 0100 6401 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 37866 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 ea93 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 ea93 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 1802 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c05 6d06 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/model/concrete_execution_graph.py` & `renku-2.4.1rc2/renku/core/workflow/model/concrete_execution_graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/model/workflow_file.py` & `renku-2.4.1rc2/renku/core/workflow/model/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/parser/__init__.py` & `renku-2.4.1rc2/renku/core/workflow/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 10631 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8729 0000  a.......p.ad.)..
+00000000: 610d 0d0a 0000 0000 6088 6264 8729 0000  a.......`.bd.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 3e01 0000 6400  .....@...s>...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6405 6c0e 6d0f 5a0f 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/parser/renku.py` & `renku-2.4.1rc2/renku/core/workflow/parser/renku.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/plan.py` & `renku-2.4.1rc2/renku/core/workflow/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/plan_factory.py` & `renku-2.4.1rc2/renku/core/workflow/plan_factory.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/providers/__init__.py` & `renku-2.4.1rc2/renku/core/workflow/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5999 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6f17 0000  a.......p.ado...
+00000000: 610d 0d0a 0000 0000 6088 6264 6f17 0000  a.......`.bdo...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 6401  d.l.m.Z.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6401 6406 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 4271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 af10 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 af10 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc` & `renku-2.4.1rc2/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 13372 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 3c34 0000  a.......p.ad<4..
+00000000: 610d 0d0a 0000 0000 6088 6264 3c34 0000  a.......`.bd<4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 0a02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/core/workflow/providers/cwltool.py` & `renku-2.4.1rc2/renku/core/workflow/providers/cwltool.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/providers/local.py` & `renku-2.4.1rc2/renku/core/workflow/providers/local.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/providers/toil.py` & `renku-2.4.1rc2/renku/core/workflow/providers/toil.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/run.py` & `renku-2.4.1rc2/renku/core/workflow/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/types.py` & `renku-2.4.1rc2/renku/core/workflow/types.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/update.py` & `renku-2.4.1rc2/renku/core/workflow/update.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/value_resolution.py` & `renku-2.4.1rc2/renku/core/workflow/value_resolution.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/core/workflow/workflow_file.py` & `renku-2.4.1rc2/renku/core/workflow/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/data/__init__.py` & `renku-2.4.1rc2/renku/data/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/data/gitignore.default` & `renku-2.4.1rc2/renku/data/gitignore.default`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/data/pre-commit.sh` & `renku-2.4.1rc2/renku/data/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/data/shacl_shape.json` & `renku-2.4.1rc2/renku/data/shacl_shape.json`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/__init__.py` & `renku-2.4.1rc2/renku/domain_model/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/__pycache__/dataset.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 29605 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 a573 0000  a.......p.ad.s..
+00000000: 610d 0d0a 0000 0000 6088 6264 a573 0000  a.......`.bd.s..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4e02 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1267 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 f304 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 f304 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6503 722c 6401  m.Z.m.Z...e.r,d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6501 6a07 8303 5a08 6402 5300  ..d.e.j...Z.d.S.
 00000070: 2907 7a12 4461 7461 7365 7420 7072 6f76  ).z.Dataset prov
```

### Comparing `renku-2.4.1rc1/renku/domain_model/__pycache__/datastructures.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/__pycache__/datastructures.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 c20a 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 c20a 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
 00000070: 650a 8303 5a0b 6402 5300 2908 7a32 4261  e...Z.d.S.).z2Ba
```

### Comparing `renku-2.4.1rc1/renku/domain_model/__pycache__/entity.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/__pycache__/entity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2499 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 c309 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 c309 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c0a 6d0b 5a0b 0100 6401 6406 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/__pycache__/enums.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/__pycache__/enums.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 cb03 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 cb03 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 4700  Z.d.d.l.m.Z...G.
 00000040: 6403 6404 8400 6404 6502 8303 5a03 6405  d.d...d.e...Z.d.
 00000050: 5300 2906 7a14 456e 756d 7320 7573 6564  S.).z.Enums used
 00000060: 2069 6e20 7265 6e6b 752e e900 0000 0029   in renku......)
 00000070: 01da 0445 6e75 6d63 0000 0000 0000 0000  ...Enumc........
```

### Comparing `renku-2.4.1rc1/renku/domain_model/__pycache__/project.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/__pycache__/project.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 8329 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8920 0000  a.......p.ad. ..
+00000000: 610d 0d0a 0000 0000 6088 6264 8920 0000  a.......`.bd. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0c 5a0c 6401 6407 6c0d  ..d.d.l.Z.d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/__pycache__/project_context.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/__pycache__/project_context.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 11817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 292e 0000  a.......p.ad)...
+00000000: 610d 0d0a 0000 0000 6088 6264 292e 0000  a.......`.bd)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1601 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6402 6c03 5a03 6401 6403  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 6d05 5a05 0100 6401 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 0100 6401 6405 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000070: 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  Z.m.Z.m.Z.m.Z.m.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/__pycache__/session.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6701 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 2d1a 0000  a.......p.ad-...
+00000000: 610d 0d0a 0000 0000 6088 6264 2d1a 0000  a.......`.bd-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 9800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/constant.py` & `renku-2.4.1rc2/renku/domain_model/constant.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/dataset.py` & `renku-2.4.1rc2/renku/domain_model/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/dataset_provider.py` & `renku-2.4.1rc2/renku/domain_model/dataset_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/datastructures.py` & `renku-2.4.1rc2/renku/domain_model/datastructures.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/entity.py` & `renku-2.4.1rc2/renku/domain_model/entity.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/enums.py` & `renku-2.4.1rc2/renku/domain_model/enums.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/git.py` & `renku-2.4.1rc2/renku/domain_model/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/project.py` & `renku-2.4.1rc2/renku/domain_model/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/project_context.py` & `renku-2.4.1rc2/renku/domain_model/project_context.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/provenance/__init__.py` & `renku-2.4.1rc2/renku/domain_model/provenance/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 13200 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 9033 0000  a.......p.ad.3..
+00000000: 610d 0d0a 0000 0000 6088 6264 9033 0000  a.......`.bd.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0c 5a0c 6401 6407 6c0d  ..d.d.l.Z.d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5155 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 2314 0000  a.......p.ad#...
+00000000: 610d 0d0a 0000 0000 6088 6264 2314 0000  a.......`.bd#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6401 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1268 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 f404 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 f404 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 8302 5a04 6402 5300 2906 7a27 5265 7072  ..Z.d.S.).z'Repr
 00000060: 6573 656e 7420 616e 2061 6e6e 6f74 6174  esent an annotat
 00000070: 696f 6e20 666f 7220 6120 776f 726b 666c  ion for a workfl
```

### Comparing `renku-2.4.1rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 fa05 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 fa05 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 8302 5a07 6407 5300 2908 7a34 436c 6173  ..Z.d.S.).z4Clas
 00000070: 7365 7320 666f 7220 7472 6163 6b69 6e67  ses for tracking
```

### Comparing `renku-2.4.1rc1/renku/domain_model/provenance/activity.py` & `renku-2.4.1rc2/renku/domain_model/provenance/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/provenance/agent.py` & `renku-2.4.1rc2/renku/domain_model/provenance/agent.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/provenance/annotation.py` & `renku-2.4.1rc2/renku/domain_model/provenance/annotation.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/provenance/parameter.py` & `renku-2.4.1rc2/renku/domain_model/provenance/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/session.py` & `renku-2.4.1rc2/renku/domain_model/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/sort.py` & `renku-2.4.1rc2/renku/domain_model/sort.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/template.py` & `renku-2.4.1rc2/renku/domain_model/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/__init__.py` & `renku-2.4.1rc2/renku/domain_model/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 15917 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 2d3e 0000  a.......p.ad->..
+00000000: 610d 0d0a 0000 0000 6088 6264 2d3e 0000  a.......`.bd->..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6406 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 18124 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 cc46 0000  a.......p.ad.F..
+00000000: 610d 0d0a 0000 0000 6088 6264 cc46 0000  a.......`.bd.F..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6401 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 16602 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 da40 0000  a.......p.ad.@..
+00000000: 610d 0d0a 0000 0000 6088 6264 da40 0000  a.......`.bd.@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3201 0000 6400  .....@...s2...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1639 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6706 0000  a.......p.adg...
+00000000: 610d 0d0a 0000 0000 6088 6264 6706 0000  a.......`.bdg...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6509 7250 6401 6406 6c0d 5a0e 4700  ..e.rPd.d.l.Z.G.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 4349 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 fd10 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 fd10 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6401 6407 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/composite_plan.py` & `renku-2.4.1rc2/renku/domain_model/workflow/composite_plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/converters/__init__.py` & `renku-2.4.1rc2/renku/domain_model/workflow/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc` & `renku-2.4.1rc2/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1531 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 fb05 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 fb05 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 4700 6407 6408  d.l.m.Z...G.d.d.
```

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/parameter.py` & `renku-2.4.1rc2/renku/domain_model/workflow/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/plan.py` & `renku-2.4.1rc2/renku/domain_model/workflow/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/provider.py` & `renku-2.4.1rc2/renku/domain_model/workflow/provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/domain_model/workflow/workflow_file.py` & `renku-2.4.1rc2/renku/domain_model/workflow/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/__init__.py` & `renku-2.4.1rc2/renku/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/__pycache__/database.cpython-39.pyc` & `renku-2.4.1rc2/renku/infrastructure/__pycache__/database.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 41333 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 75a1 0000  a.......p.adu...
+00000000: 610d 0d0a 0000 0000 6088 6264 75a1 0000  a.......`.bdu...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2602 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/infrastructure/__pycache__/immutable.cpython-39.pyc` & `renku-2.4.1rc2/renku/infrastructure/__pycache__/immutable.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 4969 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6913 0000  a.......p.adi...
+00000000: 610d 0d0a 0000 0000 6088 6264 6913 0000  a.......`.bdi...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 8302 5a06  ..G.d.d...d...Z.
 00000060: 4700 6406 6407 8400 6407 6506 8303 5a07  G.d.d...d.e...Z.
 00000070: 4700 6408 6409 8400 6409 8302 5a08 6402  G.d.d...d...Z.d.
```

### Comparing `renku-2.4.1rc1/renku/infrastructure/__pycache__/persistent.cpython-39.pyc` & `renku-2.4.1rc2/renku/infrastructure/__pycache__/persistent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 5a09 0000  a.......p.adZ...
+00000000: 610d 0d0a 0000 0000 6088 6264 5a09 0000  a.......`.bdZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 5a00 6401 6402 6c01 5a01 4700 6403 6404  Z.d.d.l.Z.G.d.d.
 00000040: 8400 6404 6501 6a02 8303 5a02 6402 5300  ..d.e.j...Z.d.S.
 00000050: 2905 7a1c 4261 7365 2052 656e 6b75 2070  ).z.Base Renku p
 00000060: 6572 7369 7374 656e 7420 636c 6173 732e  ersistent class.
 00000070: e900 0000 004e 6300 0000 0000 0000 0000  .....Nc.........
```

### Comparing `renku-2.4.1rc1/renku/infrastructure/__pycache__/repository.cpython-39.pyc` & `renku-2.4.1rc2/renku/infrastructure/__pycache__/repository.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 71947 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 0b19 0100  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 0b19 0100  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 fc02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6402 6c07 5a07 6401 6403 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 6d09 5a09 0100 6401 6404 6c0a 6d0a 5a0a  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/infrastructure/database.py` & `renku-2.4.1rc2/renku/infrastructure/database.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/gateway/__init__.py` & `renku-2.4.1rc2/renku/infrastructure/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/gateway/activity_gateway.py` & `renku-2.4.1rc2/renku/infrastructure/gateway/activity_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/gateway/database_gateway.py` & `renku-2.4.1rc2/renku/infrastructure/gateway/database_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/gateway/dataset_gateway.py` & `renku-2.4.1rc2/renku/infrastructure/gateway/dataset_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/gateway/plan_gateway.py` & `renku-2.4.1rc2/renku/infrastructure/gateway/plan_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/gateway/project_gateway.py` & `renku-2.4.1rc2/renku/infrastructure/gateway/project_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/git_merger.py` & `renku-2.4.1rc2/renku/infrastructure/git_merger.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/immutable.py` & `renku-2.4.1rc2/renku/infrastructure/immutable.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/persistent.py` & `renku-2.4.1rc2/renku/infrastructure/persistent.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/repository.py` & `renku-2.4.1rc2/renku/infrastructure/repository.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/storage/__init__.py` & `renku-2.4.1rc2/renku/infrastructure/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc` & `renku-2.4.1rc2/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1989 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 c507 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 c507 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6502 7238 6401 6404 6c07 6d08 5a08  ..e.r8d.d.l.m.Z.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6506 8303 5a0a 6407 5300 2908 7a1f 5374  e...Z.d.S.).z.St
```

### Comparing `renku-2.4.1rc1/renku/infrastructure/storage/factory.py` & `renku-2.4.1rc2/renku/infrastructure/storage/factory.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/infrastructure/storage/rclone.py` & `renku-2.4.1rc2/renku/infrastructure/storage/rclone.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md` & `renku-2.4.1rc2/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml` & `renku-2.4.1rc2/renku/templates/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md` & `renku-2.4.1rc2/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/.github/dependabot.yml` & `renku-2.4.1rc2/renku/templates/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/.gitignore` & `renku-2.4.1rc2/renku/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/R-minimal/.gitignore` & `renku-2.4.1rc2/renku/templates/R-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/R-minimal/.renkulfsignore` & `renku-2.4.1rc2/renku/templates/R-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/R-minimal/Dockerfile` & `renku-2.4.1rc2/renku/templates/R-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/R-minimal/README.md` & `renku-2.4.1rc2/renku/templates/R-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/R-minimal/workflows/my-workflow.yaml` & `renku-2.4.1rc2/renku/templates/R-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/R-minimal.png` & `renku-2.4.1rc2/renku/templates/R-minimal.png`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/README.md` & `renku-2.4.1rc2/renku/templates/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/bioc-minimal/.gitignore` & `renku-2.4.1rc2/renku/templates/bioc-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/bioc-minimal/.renkulfsignore` & `renku-2.4.1rc2/renku/templates/bioc-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/bioc-minimal/Dockerfile` & `renku-2.4.1rc2/renku/templates/bioc-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/bioc-minimal/README.md` & `renku-2.4.1rc2/renku/templates/bioc-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml` & `renku-2.4.1rc2/renku/templates/bioc-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/bioconductor.png` & `renku-2.4.1rc2/renku/templates/bioconductor.png`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/julia-minimal/.gitignore` & `renku-2.4.1rc2/renku/templates/julia-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/julia-minimal/.renkulfsignore` & `renku-2.4.1rc2/renku/templates/julia-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/julia-minimal/Dockerfile` & `renku-2.4.1rc2/renku/templates/julia-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/julia-minimal/README.md` & `renku-2.4.1rc2/renku/templates/julia-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml` & `renku-2.4.1rc2/renku/templates/julia-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/julialang.png` & `renku-2.4.1rc2/renku/templates/julialang.png`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/manifest.yaml` & `renku-2.4.1rc2/renku/templates/manifest.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/minimal/.renkulfsignore` & `renku-2.4.1rc2/renku/templates/minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/minimal/Dockerfile` & `renku-2.4.1rc2/renku/templates/minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/minimal/workflows/my-workflow.yaml` & `renku-2.4.1rc2/renku/templates/minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/python-minimal/.gitignore` & `renku-2.4.1rc2/renku/templates/python-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/python-minimal/.renkulfsignore` & `renku-2.4.1rc2/renku/templates/python-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/python-minimal/Dockerfile` & `renku-2.4.1rc2/renku/templates/python-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/python-minimal/README.md` & `renku-2.4.1rc2/renku/templates/python-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/python-minimal/workflows/my-workflow.yaml` & `renku-2.4.1rc2/renku/templates/python-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/templates/python-minimal.png` & `renku-2.4.1rc2/renku/templates/python-minimal.png`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/__init__.py` & `renku-2.4.1rc2/renku/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/__init__.py` & `renku-2.4.1rc2/renku/ui/api/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/graph/__init__.py` & `renku-2.4.1rc2/renku/ui/api/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/graph/rdf.py` & `renku-2.4.1rc2/renku/ui/api/graph/rdf.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/models/__init__.py` & `renku-2.4.1rc2/renku/ui/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/models/activity.py` & `renku-2.4.1rc2/renku/ui/api/models/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/models/dataset.py` & `renku-2.4.1rc2/renku/ui/api/models/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/models/parameter.py` & `renku-2.4.1rc2/renku/ui/api/models/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/models/plan.py` & `renku-2.4.1rc2/renku/ui/api/models/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/models/project.py` & `renku-2.4.1rc2/renku/ui/api/models/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/api/util.py` & `renku-2.4.1rc2/renku/ui/api/util.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/__init__.py` & `renku-2.4.1rc2/renku/ui/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/__main__.py` & `renku-2.4.1rc2/renku/ui/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/__init__.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 9319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6724 0000  a.......p.adg$..
+00000000: 610d 0d0a 0000 0000 6088 6264 6724 0000  a.......`.bdg$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 5404 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6402 6c06 5a06 6401  m.Z...d.d.l.Z.d.
 00000060: 6402 6c07 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/clone.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/clone.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2594 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 220a 0000  a.......p.ad"...
+00000000: 610d 0d0a 0000 0000 6088 6264 220a 0000  a.......`.bd"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6501 a007 a100 6501  ..m.Z...e.....e.
 00000060: 6a08 6403 6404 6405 6406 6407 8d04 6501  j.d.d.d.d.d...e.
 00000070: a009 6408 a101 6501 6a09 6409 6406 6402  ..d...e.j.d.d.d.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/config.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 7953 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 111f 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 111f 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 a009 a100 6404 6405 8400  Z...e.....d.d...
 00000070: 8301 5a0a 650a a00b a100 6501 6a0c 6406  ..Z.e.....e.j.d.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/dataset.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 42970 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 daa7 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 daa7 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0015 0000 0040 0000 0073 0408 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6402 6c09 5a09 6401 6405 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6402 6c0c 6d0d 0200  m.Z...d.d.l.m...
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/doctor.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/doctor.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2217 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 a908 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 a908 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6502  Z.d.d.l.m.Z...e.
 00000050: a005 a100 6502 6a06 6502 6a07 6404 6405  ....e.j.e.j.d.d.
 00000060: 6406 6407 8d03 6502 6a07 6408 6409 6405  d.d...e.j.d.d.d.
 00000070: 640a 6407 8d04 640b 640c 8400 8301 8301  d.d...d.d.......
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/env.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/env.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1600 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 4006 0000  a.......p.ad@...
+00000000: 610d 0d0a 0000 0000 6088 6264 4006 0000  a.......`.bd@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 a100  Z.d.d.l.Z.e.....
 00000040: 6501 6a03 6403 6404 6405 6406 6407 8d04  e.j.d.d.d.d.d...
 00000050: 6501 6a04 6408 6409 8400 8301 8301 8301  e.j.d.d.........
 00000060: 5a05 6402 5300 290a 7a23 5265 6e6b 7520  Z.d.S.).z#Renku 
 00000070: 656e 7669 726f 6e6d 656e 7420 7265 6c61  environment rela
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 7931 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 fb1e 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 fb1e 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6403 6c07 6d08 5a08 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6402 6c09 5a09 6401 6402 6c0a 6d0b 0200  d.l.Z.d.d.l.m...
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/gc.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/gc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1139 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 7304 0000  a.......p.ads...
+00000000: 610d 0d0a 0000 0000 6088 6264 7304 0000  a.......`.bds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 a100  Z.d.d.l.Z.e.....
 00000040: 6403 6404 8400 8301 5a03 6402 5300 2905  d.d.....Z.d.S.).
 00000050: 7adf 4672 6565 2075 7020 6469 736b 2073  z.Free up disk s
 00000060: 7061 6365 2062 7920 7265 6d6f 7669 6e67  pace by removing
 00000070: 2074 656d 706f 7261 7279 2066 696c 6573   temporary files
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/githooks.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/githooks.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2538 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 ea09 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 ea09 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6402 6c05 6d06 0200 0100 6d07 0200 0100  d.l.m.....m.....
 00000060: 6d08 0200 0100 6d09 5a09 0100 6504 a00a  m.....m.Z...e...
 00000070: a100 6404 6405 8400 8301 5a0b 650b a00c  ..d.d.....Z.e...
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/graph.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/graph.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 4950 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 5613 0000  a.......p.adV...
+00000000: 610d 0d0a 0000 0000 6088 6264 5613 0000  a.......`.bdV...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6404 6404 6405 6406 6407  m.Z...d.d.d.d.d.
 00000050: 6408 6409 640a 9c07 5a04 6501 a005 a100  d.d.d...Z.e.....
 00000060: 640b 640c 8400 8301 5a06 6506 a007 a100  d.d.....Z.e.....
 00000070: 6501 6a08 640d 6503 6509 6504 a00a a100  e.j.d.e.e.e.....
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/init.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/init.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 11113 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 692b 0000  a.......p.adi+..
+00000000: 610d 0d0a 0000 0000 6088 6264 692b 0000  a.......`.bdi+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0013 0000 0040 0000 0073 a001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6700 6407 a201  d.l.m.Z...g.d...
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/log.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/log.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 8581 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8521 0000  a.......p.ad.!..
+00000000: 610d 0d0a 0000 0000 6088 6264 8521 0000  a.......`.bd.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0c 0100 6401 6404 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/login.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/login.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 4845 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 ed12 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 ed12 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 a009 a100 6501 6a0a 6404  Z...e.....e.j.d.
 00000070: 6405 6402 6406 8d03 6501 6a0b 6407 6408  d.d.d...e.j.d.d.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2499 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 c309 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 c309 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 a004 a100 6404 6405  m.Z...e.....d.d.
 00000050: 8400 8301 5a05 6505 6a06 6406 6407 8d01  ....Z.e.j.d.d...
 00000060: 6501 6a07 6408 6501 6a08 6406 6409 8d01  e.j.d.e.j.d.d...
 00000070: 640a 8d02 6501 6a07 640b 6501 6a08 6406  d...e.j.d.e.j.d.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/migrate.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/migrate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5689 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 3916 0000  a.......p.ad9...
+00000000: 610d 0d0a 0000 0000 6088 6264 3916 0000  a.......`.bd9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 1e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 0200 0100 6d06 0200 0100 6d07 0200  m.....m.....m...
 00000060: 0100 6d08 5a08 0100 6401 6403 6c09 6d0a  ..m.Z...d.d.l.m.
 00000070: 5a0a 6d0b 5a0b 0100 6401 6404 6c0c 6d0d  Z.m.Z...d.d.l.m.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/move.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/move.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2881 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 410b 0000  a.......p.adA...
+00000000: 610d 0d0a 0000 0000 6088 6264 410b 0000  a.......`.bdA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 6a04 6404 6405 8d01  m.Z...e.j.d.d...
 00000050: 6501 6a05 6406 6501 6a06 6407 6408 8d01  e.j.d.e.j.d.d...
 00000060: 6409 640a 8d03 6501 6a05 640b 6501 a006  d.d...e.j.d.e...
 00000070: a100 640c 640a 8d03 6501 6a07 640d 640e  ..d.d...e.j.d.d.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/project.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/project.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8816 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 8816 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6402 6c05 6d06 0200 0100 6d07 0200 0100  d.l.m.....m.....
 00000060: 6d08 0200 0100 6d09 5a09 0100 6401 6404  m.....m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6401 6405 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/remove.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/remove.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 da06 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 da06 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 6a04 6404 6405 8d01  m.Z...e.j.d.d...
 00000050: 6501 6a05 6406 6501 6a06 6407 6408 8d01  e.j.d.e.j.d.d...
 00000060: 6409 6407 640a 8d04 640b 640c 8400 8301  d.d.d...d.d.....
 00000070: 8301 5a07 6402 5300 290d 6121 0200 0052  ..Z.d.S.).a!...R
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/rerun.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/rerun.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 4227 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8310 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 8310 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6501 a00a a100  d.l.m.Z...e.....
 00000070: 6501 6a0b 6407 6408 6409 640a 640b 640c  e.j.d.d.d.d.d.d.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/rollback.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/rollback.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3249 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 b10c 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 b10c 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 a004 a100 6501 6a05  m.Z...e.....e.j.
 00000050: 6404 6405 8400 8301 8301 5a06 6402 5300  d.d.......Z.d.S.
 00000060: 2906 75f8 0700 0052 6f6c 6c62 6163 6b20  ).u....Rollback 
 00000070: 7072 6f6a 6563 7420 746f 2061 2070 7265  project to a pre
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/run.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 26417 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 3167 0000  a.......p.ad1g..
+00000000: 610d 0d0a 0000 0000 6088 6264 3167 0000  a.......`.bd1g..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0019 0000 0040 0000 0073 0e02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/save.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/save.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3510 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 b60d 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 b60d 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 6a09 6404 6405 8d01 6501  Z...e.j.d.d...e.
 00000070: 6a0a 6406 6407 6402 6408 6409 8d04 6501  j.d.d.d.d.d...e.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/service.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/service.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 11830 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 362e 0000  a.......p.ad6...
+00000000: 610d 0d0a 0000 0000 6088 6264 362e 0000  a.......`.bd6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 8002 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6403 6c07 6d07 5a07 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6404 6c08 6d09 5a09 0100 6401 6402 6c0a  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/session.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 14005 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 b536 0000  a.......p.ad.6..
+00000000: 610d 0d0a 0000 0000 6088 6264 b536 0000  a.......`.bd.6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 b402 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/status.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/status.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5489 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 7115 0000  a.......p.adq...
+00000000: 610d 0d0a 0000 0000 6088 6264 7115 0000  a.......`.bdq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 a009 a100 6501 6a0a 6501  Z...e.....e.j.e.
 00000070: 6a0b 6404 6405 6406 6407 6408 8d04 6501  j.d.d.d.d.d...e.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/storage.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/storage.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5604 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 e415 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 e415 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 4801 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 6d04 0200 0100 6d05  Z.d.d.l.m.....m.
 00000050: 0200 0100 6d06 0200 0100 6d07 5a07 0100  ....m.....m.Z...
 00000060: 6401 6403 6c08 6d09 5a09 0100 6401 6404  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6502 a00c a100 6405  l.m.Z...e.....d.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/template.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/template.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 13434 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 7a34 0000  a.......p.adz4..
+00000000: 610d 0d0a 0000 0000 6088 6264 7a34 0000  a.......`.bdz4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 7402 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6401 6402 6c08  m.Z.m.Z...d.d.l.
 00000060: 5a08 6401 6402 6c09 6d0a 0200 0100 6d0b  Z.d.d.l.m.....m.
 00000070: 0200 0100 6d0c 0200 0100 6d0d 5a0d 0100  ....m.....m.Z...
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/update.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/update.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 6723 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 431a 0000  a.......p.adC...
+00000000: 610d 0d0a 0000 0000 6088 6264 431a 0000  a.......`.bdC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6501 a00c a100 6501 6a0d  m.Z...e.....e.j.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/__pycache__/workflow.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/__pycache__/workflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 48023 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 97bb 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 97bb 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0016 0000 0040 0000 0073 6207 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6402 6c07 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6402 6c0a 6d0b 0200 0100 6d0c  ..d.d.l.m.....m.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/clone.py` & `renku-2.4.1rc2/renku/ui/cli/clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/config.py` & `renku-2.4.1rc2/renku/ui/cli/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/dataset.py` & `renku-2.4.1rc2/renku/ui/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/doctor.py` & `renku-2.4.1rc2/renku/ui/cli/doctor.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/env.py` & `renku-2.4.1rc2/renku/ui/cli/env.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/exception_handler.py` & `renku-2.4.1rc2/renku/ui/cli/exception_handler.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/gc.py` & `renku-2.4.1rc2/renku/ui/cli/gc.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/githooks.py` & `renku-2.4.1rc2/renku/ui/cli/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/graph.py` & `renku-2.4.1rc2/renku/ui/cli/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/init.py` & `renku-2.4.1rc2/renku/ui/cli/init.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/log.py` & `renku-2.4.1rc2/renku/ui/cli/log.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/login.py` & `renku-2.4.1rc2/renku/ui/cli/login.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/mergetool.py` & `renku-2.4.1rc2/renku/ui/cli/mergetool.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/migrate.py` & `renku-2.4.1rc2/renku/ui/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/move.py` & `renku-2.4.1rc2/renku/ui/cli/move.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/project.py` & `renku-2.4.1rc2/renku/ui/cli/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/remove.py` & `renku-2.4.1rc2/renku/ui/cli/remove.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/rerun.py` & `renku-2.4.1rc2/renku/ui/cli/rerun.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/rollback.py` & `renku-2.4.1rc2/renku/ui/cli/rollback.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/run.py` & `renku-2.4.1rc2/renku/ui/cli/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/save.py` & `renku-2.4.1rc2/renku/ui/cli/save.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/service.py` & `renku-2.4.1rc2/renku/ui/cli/service.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/session.py` & `renku-2.4.1rc2/renku/ui/cli/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/status.py` & `renku-2.4.1rc2/renku/ui/cli/status.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/storage.py` & `renku-2.4.1rc2/renku/ui/cli/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/template.py` & `renku-2.4.1rc2/renku/ui/cli/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/update.py` & `renku-2.4.1rc2/renku/ui/cli/update.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/__init__.py` & `renku-2.4.1rc2/renku/ui/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 5422 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 2e15 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 2e15 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d05 5a05 0100 6401 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d06 5a06 0100 6401 6402 6c07 6d08 0200  m.Z...d.d.l.m...
 00000070: 0100 6d09 0200 0100 6d0a 0200 0100 6d0b  ..m.....m.....m.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 3982 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 8e0f 0000  a.......p.ad....
+00000000: 610d 0d0a 0000 0000 6088 6264 8e0f 0000  a.......`.bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a04 6502 722c 6401  ..d.d.l.Z.e.r,d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6504 6a07 8303 5a08 4700 6407  ..d.e.j...Z.G.d.
 00000070: 6408 8400 6408 6504 6a09 8303 5a0a 650b  d...d.e.j...Z.e.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 1387 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 6b05 0000  a.......p.adk...
+00000000: 610d 0d0a 0000 0000 6088 6264 6b05 0000  a.......`.bdk...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 8400 5a01 6403 6404 8400  Z.d.d...Z.d.d...
 00000040: 5a02 6405 6406 8400 5a03 6407 5300 2908  Z.d.d...Z.d.S.).
 00000050: 7a1e 5574 696c 6974 7920 6675 6e63 7469  z.Utility functi
 00000060: 6f6e 7320 666f 7220 706c 7567 696e 732e  ons for plugins.
 00000070: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 9929 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 c926 0000  a.......p.ad.&..
+00000000: 610d 0d0a 0000 0000 6088 6264 c926 0000  a.......`.bd.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6e01 0000 6400  .....@...sn...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6402 6c07 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6506 7270 6401 6405 6c0a 6d0b 5a0b  ..e.rpd.d.l.m.Z.
```

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/callback.py` & `renku-2.4.1rc2/renku/ui/cli/utils/callback.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/click.py` & `renku-2.4.1rc2/renku/ui/cli/utils/click.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/color.py` & `renku-2.4.1rc2/renku/ui/cli/utils/color.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/curses.py` & `renku-2.4.1rc2/renku/ui/cli/utils/curses.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/plugins.py` & `renku-2.4.1rc2/renku/ui/cli/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/utils/terminal.py` & `renku-2.4.1rc2/renku/ui/cli/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/cli/workflow.py` & `renku-2.4.1rc2/renku/ui/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/.env-example` & `renku-2.4.1rc2/renku/ui/service/.env-example`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/__init__.py` & `renku-2.4.1rc2/renku/ui/service/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/__pycache__/config.cpython-39.pyc` & `renku-2.4.1rc2/renku/ui/service/__pycache__/config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 15 07:08:32 2023 UTC, .py size: 2931 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70da 6164 730b 0000  a.......p.ads...
+00000000: 610d 0d0a 0000 0000 6088 6264 730b 0000  a.......`.bds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 be01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 7a0c  Z.d.d.l.m.Z...z.
 00000050: 6401 6402 6c05 5a05 5700 6e1e 0400 6506  d.d.l.Z.W.n...e.
 00000060: 794a 0100 0100 0100 6401 6402 6c07 6d08  yJ......d.d.l.m.
 00000070: 5a05 0100 5900 6e02 3000 6401 5a09 6404  Z...Y.n.0.d.Z.d.
```

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/__init__.py` & `renku-2.4.1rc2/renku/ui/service/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/base.py` & `renku-2.4.1rc2/renku/ui/service/cache/base.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/config.py` & `renku-2.4.1rc2/renku/ui/service/cache/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/files.py` & `renku-2.4.1rc2/renku/ui/service/cache/files.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/jobs.py` & `renku-2.4.1rc2/renku/ui/service/cache/jobs.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/models/__init__.py` & `renku-2.4.1rc2/renku/ui/service/cache/models/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/models/file.py` & `renku-2.4.1rc2/renku/ui/service/cache/models/file.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/models/job.py` & `renku-2.4.1rc2/renku/ui/service/cache/models/job.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/models/project.py` & `renku-2.4.1rc2/renku/ui/service/cache/models/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/models/user.py` & `renku-2.4.1rc2/renku/ui/service/cache/models/user.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/projects.py` & `renku-2.4.1rc2/renku/ui/service/cache/projects.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/serializers/__init__.py` & `renku-2.4.1rc2/renku/ui/service/cache/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/serializers/file.py` & `renku-2.4.1rc2/renku/ui/service/cache/serializers/file.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/serializers/job.py` & `renku-2.4.1rc2/renku/ui/service/cache/serializers/job.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/serializers/project.py` & `renku-2.4.1rc2/renku/ui/service/cache/serializers/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/serializers/user.py` & `renku-2.4.1rc2/renku/ui/service/cache/serializers/user.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/cache/users.py` & `renku-2.4.1rc2/renku/ui/service/cache/users.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/config.py` & `renku-2.4.1rc2/renku/ui/service/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/__init__.py` & `renku-2.4.1rc2/renku/ui/service/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/api/__init__.py` & `renku-2.4.1rc2/renku/ui/service/controllers/api/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/api/abstract.py` & `renku-2.4.1rc2/renku/ui/service/controllers/api/abstract.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/api/mixins.py` & `renku-2.4.1rc2/renku/ui/service/controllers/api/mixins.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/cache_files_delete_chunks.py` & `renku-2.4.1rc2/renku/ui/service/controllers/cache_files_delete_chunks.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/cache_files_upload.py` & `renku-2.4.1rc2/renku/ui/service/controllers/cache_files_upload.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/cache_list_projects.py` & `renku-2.4.1rc2/renku/ui/service/controllers/cache_list_projects.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/cache_list_uploaded.py` & `renku-2.4.1rc2/renku/ui/service/controllers/cache_list_uploaded.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/cache_migrate_project.py` & `renku-2.4.1rc2/renku/ui/service/controllers/cache_migrate_project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/cache_migrations_check.py` & `renku-2.4.1rc2/renku/ui/service/controllers/cache_migrations_check.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/cache_project_clone.py` & `renku-2.4.1rc2/renku/ui/service/controllers/cache_project_clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/config_set.py` & `renku-2.4.1rc2/renku/ui/service/controllers/config_set.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/config_show.py` & `renku-2.4.1rc2/renku/ui/service/controllers/config_show.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/datasets_add_file.py` & `renku-2.4.1rc2/renku/ui/service/controllers/datasets_add_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/datasets_create.py` & `renku-2.4.1rc2/renku/ui/service/controllers/datasets_create.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/datasets_edit.py` & `renku-2.4.1rc2/renku/ui/service/controllers/datasets_edit.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/datasets_files_list.py` & `renku-2.4.1rc2/renku/ui/service/controllers/datasets_files_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/datasets_import.py` & `renku-2.4.1rc2/renku/ui/service/controllers/datasets_import.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/datasets_list.py` & `renku-2.4.1rc2/renku/ui/service/controllers/datasets_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/datasets_remove.py` & `renku-2.4.1rc2/renku/ui/service/controllers/datasets_remove.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/datasets_unlink.py` & `renku-2.4.1rc2/renku/ui/service/controllers/datasets_unlink.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/graph_export.py` & `renku-2.4.1rc2/renku/ui/service/controllers/graph_export.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/project_edit.py` & `renku-2.4.1rc2/renku/ui/service/controllers/project_edit.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/project_lock_status.py` & `renku-2.4.1rc2/renku/ui/service/controllers/project_lock_status.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/project_show.py` & `renku-2.4.1rc2/renku/ui/service/controllers/project_show.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/templates_create_project.py` & `renku-2.4.1rc2/renku/ui/service/controllers/templates_create_project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/templates_read_manifest.py` & `renku-2.4.1rc2/renku/ui/service/controllers/templates_read_manifest.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/utils/__init__.py` & `renku-2.4.1rc2/renku/ui/service/controllers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/utils/datasets.py` & `renku-2.4.1rc2/renku/ui/service/controllers/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/utils/project_clone.py` & `renku-2.4.1rc2/renku/ui/service/controllers/utils/project_clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/utils/remote_project.py` & `renku-2.4.1rc2/renku/ui/service/controllers/utils/remote_project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/version.py` & `renku-2.4.1rc2/renku/ui/service/controllers/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/workflow_plans_export.py` & `renku-2.4.1rc2/renku/ui/service/controllers/workflow_plans_export.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/workflow_plans_list.py` & `renku-2.4.1rc2/renku/ui/service/controllers/workflow_plans_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/controllers/workflow_plans_show.py` & `renku-2.4.1rc2/renku/ui/service/controllers/workflow_plans_show.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/entrypoint.py` & `renku-2.4.1rc2/renku/ui/service/entrypoint.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/errors.py` & `renku-2.4.1rc2/renku/ui/service/errors.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/gateways/__init__.py` & `renku-2.4.1rc2/renku/ui/service/gateways/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/gateways/gitlab_api_provider.py` & `renku-2.4.1rc2/renku/ui/service/gateways/gitlab_api_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/interfaces/__init__.py` & `renku-2.4.1rc2/renku/ui/service/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/interfaces/git_api_provider.py` & `renku-2.4.1rc2/renku/ui/service/interfaces/git_api_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/jobs/__init__.py` & `renku-2.4.1rc2/renku/ui/service/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/jobs/cleanup.py` & `renku-2.4.1rc2/renku/ui/service/jobs/cleanup.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/jobs/constants.py` & `renku-2.4.1rc2/renku/ui/service/jobs/constants.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/jobs/contexts.py` & `renku-2.4.1rc2/renku/ui/service/jobs/contexts.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/jobs/datasets.py` & `renku-2.4.1rc2/renku/ui/service/jobs/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/jobs/delayed_ctrl.py` & `renku-2.4.1rc2/renku/ui/service/jobs/delayed_ctrl.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/jobs/queues.py` & `renku-2.4.1rc2/renku/ui/service/jobs/queues.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/logger.py` & `renku-2.4.1rc2/renku/ui/service/logger.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/logging.yaml` & `renku-2.4.1rc2/renku/ui/service/logging.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/scheduler.py` & `renku-2.4.1rc2/renku/ui/service/scheduler.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/__init__.py` & `renku-2.4.1rc2/renku/ui/service/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/cache.py` & `renku-2.4.1rc2/renku/ui/service/serializers/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/common.py` & `renku-2.4.1rc2/renku/ui/service/serializers/common.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/config.py` & `renku-2.4.1rc2/renku/ui/service/serializers/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/datasets.py` & `renku-2.4.1rc2/renku/ui/service/serializers/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/graph.py` & `renku-2.4.1rc2/renku/ui/service/serializers/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/headers.py` & `renku-2.4.1rc2/renku/ui/service/serializers/headers.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/jobs.py` & `renku-2.4.1rc2/renku/ui/service/serializers/jobs.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/project.py` & `renku-2.4.1rc2/renku/ui/service/serializers/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/rpc.py` & `renku-2.4.1rc2/renku/ui/service/serializers/rpc.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/templates.py` & `renku-2.4.1rc2/renku/ui/service/serializers/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/v1/__init__.py` & `renku-2.4.1rc2/renku/ui/service/serializers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/v1/cache.py` & `renku-2.4.1rc2/renku/ui/service/serializers/v1/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/v1/templates.py` & `renku-2.4.1rc2/renku/ui/service/serializers/v1/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/version.py` & `renku-2.4.1rc2/renku/ui/service/serializers/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/serializers/workflows.py` & `renku-2.4.1rc2/renku/ui/service/serializers/workflows.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/utils/__init__.py` & `renku-2.4.1rc2/renku/ui/service/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/utils/callback.py` & `renku-2.4.1rc2/renku/ui/service/utils/callback.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/utils/json_encoder.py` & `renku-2.4.1rc2/renku/ui/service/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/utils/squash.py` & `renku-2.4.1rc2/renku/ui/service/utils/squash.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/utils/timeout.py` & `renku-2.4.1rc2/renku/ui/service/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/__init__.py` & `renku-2.4.1rc2/renku/ui/service/views/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/api_versions.py` & `renku-2.4.1rc2/renku/ui/service/views/api_versions.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/apispec.py` & `renku-2.4.1rc2/renku/ui/service/views/apispec.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/cache.py` & `renku-2.4.1rc2/renku/ui/service/views/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/config.py` & `renku-2.4.1rc2/renku/ui/service/views/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/datasets.py` & `renku-2.4.1rc2/renku/ui/service/views/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/decorators.py` & `renku-2.4.1rc2/renku/ui/service/views/decorators.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/error_handlers.py` & `renku-2.4.1rc2/renku/ui/service/views/error_handlers.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/graph.py` & `renku-2.4.1rc2/renku/ui/service/views/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/jobs.py` & `renku-2.4.1rc2/renku/ui/service/views/jobs.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/project.py` & `renku-2.4.1rc2/renku/ui/service/views/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/templates.py` & `renku-2.4.1rc2/renku/ui/service/views/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/v1/__init__.py` & `renku-2.4.1rc2/renku/ui/service/views/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/v1/cache.py` & `renku-2.4.1rc2/renku/ui/service/views/v1/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/v1/templates.py` & `renku-2.4.1rc2/renku/ui/service/views/v1/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/version.py` & `renku-2.4.1rc2/renku/ui/service/views/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/views/workflow_plans.py` & `renku-2.4.1rc2/renku/ui/service/views/workflow_plans.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/ui/service/worker.py` & `renku-2.4.1rc2/renku/ui/service/worker.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/renku/version.py` & `renku-2.4.1rc2/renku/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.4.1rc1/PKG-INFO` & `renku-2.4.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renku
-Version: 2.4.1rc1
+Version: 2.4.1rc2
 Summary: Python SDK and CLI for the Renku platform.
 Home-page: https://github.com/swissdatasciencecenter/renku-python
 License: Apache-2.0
 Keywords: Renku,CLI
 Author: Swiss Data Science Center
 Author-email: contact@datascience.ch
 Requires-Python: >=3.8.1,<4.0.0
```

