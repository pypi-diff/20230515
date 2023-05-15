# Comparing `tmp/taskflow-5.1.0.tar.gz` & `tmp/taskflow-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskflow-5.1.0.tar", last modified: Thu Jan  5 10:10:08 2023, max compression
+gzip compressed data, was "taskflow-5.2.0.tar", last modified: Mon May 15 08:31:01 2023, max compression
```

## Comparing `taskflow-5.1.0.tar` & `taskflow-5.2.0.tar`

### file list

```diff
@@ -1,370 +1,374 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.173206 taskflow-5.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-01-05 10:09:36.000000 taskflow-5.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-01-05 10:09:36.000000 taskflow-5.1.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-01-05 10:09:36.000000 taskflow-5.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-01-05 10:09:36.000000 taskflow-5.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-01-05 10:09:36.000000 taskflow-5.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-01-05 10:10:07.000000 taskflow-5.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2023-01-05 10:09:36.000000 taskflow-5.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77100 2023-01-05 10:10:07.000000 taskflow-5.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-01-05 10:09:36.000000 taskflow-5.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4212 2023-01-05 10:10:08.173206 taskflow-5.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2380 2023-01-05 10:09:36.000000 taskflow-5.1.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-01-05 10:09:36.000000 taskflow-5.1.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.089202 taskflow-5.1.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.093202 taskflow-5.1.0/doc/diagrams/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/diagrams/area_of_influence.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16344 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/diagrams/core.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27254 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/diagrams/jobboard.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    99579 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/diagrams/tasks.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6967 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/diagrams/worker-engine.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.093202 taskflow-5.1.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2881 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.093202 taskflow-5.1.0/doc/source/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/templates/layout.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.097202 taskflow-5.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14336 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/arguments_and_results.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8573 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/atoms.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2743 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/conductors.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21501 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/engines.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8567 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/examples.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/exceptions.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/history.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.101203 taskflow-5.1.0/doc/source/user/img/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7242 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/area_of_influence.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9664 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/conductor.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36940 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/conductor_cycle.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    68549 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/distributed_flow_rpc.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24407 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/engine_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26861 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/flow_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13531 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/job_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   110260 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/jobboard.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21971 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/mandelbrot.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22538 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/retry_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20666 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/task_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   241180 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/tasks.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16727 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/wbe_request_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25165 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/img/worker-engine.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5696 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/inputs_and_outputs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13665 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/jobs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6370 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/notifications.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/patterns.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12122 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/persistence.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7141 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/resumption.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/shelf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10022 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/states.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/types.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/utils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16388 2023-01-05 10:09:36.000000 taskflow-5.1.0/doc/source/user/workers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2023-01-05 10:09:36.000000 taskflow-5.1.0/pylintrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.081202 taskflow-5.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.105203 taskflow-5.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/notes/add-sentinel-redis-support-9fd16e2a5dd5c0c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/notes/fix-endless-loop-on-storage-error-dd4467f0bbc66abf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/notes/zookeeper-ssl-support-b9abf24a39096b62.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.105203 taskflow-5.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.105203 taskflow-5.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.109203 taskflow-5.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9262 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-01-05 10:09:36.000000 taskflow-5.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-01-05 10:09:36.000000 taskflow-5.1.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1988 2023-01-05 10:09:36.000000 taskflow-5.1.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2798 2023-01-05 10:10:08.177206 taskflow-5.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-01-05 10:09:36.000000 taskflow-5.1.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.109203 taskflow-5.1.0/taskflow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17342 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/atom.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.113203 taskflow-5.1.0/taskflow/conductors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/conductors/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.113203 taskflow-5.1.0/taskflow/conductors/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/conductors/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/conductors/backends/impl_blocking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14816 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/conductors/backends/impl_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/conductors/backends/impl_nonblocking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7332 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/conductors/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.113203 taskflow-5.1.0/taskflow/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3402 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/deciders.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.117203 taskflow-5.1.0/taskflow/engines/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.117203 taskflow-5.1.0/taskflow/engines/action_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.121204 taskflow-5.1.0/taskflow/engines/action_engine/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/actions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1668 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/actions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/actions/retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/actions/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17015 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/builder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16164 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/compiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9028 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/completer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7254 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/deciders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29532 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7749 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27828 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/process_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13845 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/runtime.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4048 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/scopes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11558 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/selector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4552 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/action_engine/traversal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4841 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10952 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.121204 taskflow-5.1.0/taskflow/engines/worker_based/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7145 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/dispatcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4379 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13811 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20238 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/protocol.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9525 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11559 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9887 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6331 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/engines/worker_based/worker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.137204 taskflow-5.1.0/taskflow/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8893 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/99_bottles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3255 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/alphabet_soup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6554 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/build_a_car.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3909 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/buildsystem.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3917 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/calculate_in_parallel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4614 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/calculate_linear.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4336 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/create_parallel_volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/delayed_return.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4453 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/distance_calculator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/dump_memory_backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/echo_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3312 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/example_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6832 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/fake_billing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3461 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/graph_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4216 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/hello_world.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6821 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/jobboard_produce_consume_colors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/parallel_table_multiply.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3906 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/persistence_example.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/pseudo_scoping.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/pseudo_scoping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/resume_from_backend.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4992 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/resume_from_backend.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.137204 taskflow-5.1.0/taskflow/examples/resume_many_flows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1288 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/resume_many_flows/my_flows.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/resume_many_flows/resume_all.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/resume_many_flows/run_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/resume_many_flows.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3192 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/resume_many_flows.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9636 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/resume_vm_boot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/resume_volume_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/retry_flow.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/retry_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/reverting_linear.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3543 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/reverting_linear.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/run_by_iter.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2620 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/run_by_iter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/run_by_iter_enumerate.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/run_by_iter_enumerate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2742 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/share_engine_thread.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/simple_linear.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/simple_linear.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/simple_linear_listening.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3958 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/simple_linear_listening.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/simple_linear_pass.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/simple_linear_pass.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3762 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/simple_map_reduce.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/switch_graph_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/timing_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8472 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/tox_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5547 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/wbe_event_sender.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/wbe_mandelbrot.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8842 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/wbe_mandelbrot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/wbe_simple_linear.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5413 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/wbe_simple_linear.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4732 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/examples/wrapped_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11565 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4822 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7441 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/formatters.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.137204 taskflow-5.1.0/taskflow/jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/jobs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.137204 taskflow-5.1.0/taskflow/jobs/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2902 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/jobs/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43520 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/jobs/backends/impl_redis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37555 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/jobs/backends/impl_zookeeper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22043 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/jobs/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.141204 taskflow-5.1.0/taskflow/listeners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/listeners/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7391 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/listeners/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4329 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/listeners/capturing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4115 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/listeners/claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8516 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/listeners/logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/listeners/printing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6943 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/listeners/timing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/logging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.141204 taskflow-5.1.0/taskflow/patterns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/patterns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15292 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/patterns/graph_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/patterns/linear_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/patterns/unordered_flow.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.141204 taskflow-5.1.0/taskflow/persistence/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.145204 taskflow-5.1.0/taskflow/persistence/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/impl_dir.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13390 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/impl_memory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25408 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/impl_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6096 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/impl_zookeeper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.145204 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.145204 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2467 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.149205 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/0bc3e1a3c135_set_result_meduimtext_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/14b227d79a87_add_intention_column.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1c783c0c2875_replace_exception_an.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1cea328f0f65_initial_logbook_deta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1778 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/2ad4984f2864_switch_postgres_to_json_native.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/3162c0f3f8e4_add_revert_results_and_revert_failure_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/40fc8c914bd2_fix_atomdetails_failure_size.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/589dccdf2b6e_rename_taskdetails_to_atomdetails.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1072 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/6df9422fcb43_fix_flowdetails_meta_size.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/84d6e888850_add_task_detail_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1140 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4819 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4060 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40762 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9545 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/persistence/path_based.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14537 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6901 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52046 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10052 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10317 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.149205 taskflow-5.1.0/taskflow/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/test_examples.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.157205 taskflow-5.1.0/taskflow/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.161205 taskflow-5.1.0/taskflow/tests/unit/action_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/action_engine/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12866 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/action_engine/test_builder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23759 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/action_engine/test_compile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3517 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/action_engine/test_creation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/action_engine/test_process_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11327 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/action_engine/test_scoping.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.161205 taskflow-5.1.0/taskflow/tests/unit/jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/jobs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8447 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/jobs/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/jobs/test_entrypoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5174 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/jobs/test_redis_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12225 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/jobs/test_zk_job.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.161205 taskflow-5.1.0/taskflow/tests/unit/patterns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/patterns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12464 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/patterns/test_graph_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5145 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/patterns/test_linear_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4985 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/patterns/test_unordered_flow.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.165205 taskflow-5.1.0/taskflow/tests/unit/persistence/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/persistence/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16547 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/persistence/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3929 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/persistence/test_dir_persistence.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7871 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/persistence/test_memory_persistence.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10260 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/persistence/test_sql_persistence.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3648 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/persistence/test_zk_persistence.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9204 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_arguments_passing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6173 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_check_transition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18996 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_conductors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2733 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_deciders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5399 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_engine_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64393 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_engines.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4362 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17982 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_failure.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18086 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_flow_dependencies.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3921 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_formatters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_functor_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15304 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_listeners.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_mapfunctor_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7894 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5259 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_progress.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_reducefunctor_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56365 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_retries.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3660 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23520 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9900 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_suspend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15947 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20225 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11029 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_utils_async_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3168 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_utils_binary.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5716 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_utils_iter_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5503 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/test_utils_threading_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.165205 taskflow-5.1.0/taskflow/tests/unit/worker_based/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4045 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_creation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2915 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_dispatcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3128 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13622 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_message_pump.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3812 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_pipeline.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7745 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_protocol.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9920 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14344 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7109 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/unit/worker_based/test_worker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11163 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.169206 taskflow-5.1.0/taskflow/types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/types/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/types/entity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21189 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/types/failure.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10504 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/types/graph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2193 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/types/latch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14071 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/types/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4004 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/types/sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/types/timing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15820 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/types/tree.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.173206 taskflow-5.1.0/taskflow/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/async_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/banner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/eventlet_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/iter_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9521 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/kazoo_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/kombu_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18504 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/misc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3899 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/persistence_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4369 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/redis_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1434 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/schema_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5849 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/utils/threading_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2023-01-05 10:09:36.000000 taskflow-5.1.0/taskflow/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.113203 taskflow-5.1.0/taskflow.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4212 2023-01-05 10:10:07.000000 taskflow-5.1.0/taskflow.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12353 2023-01-05 10:10:08.000000 taskflow-5.1.0/taskflow.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-01-05 10:10:07.000000 taskflow-5.1.0/taskflow.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2023-01-05 10:10:07.000000 taskflow-5.1.0/taskflow.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-01-05 10:10:07.000000 taskflow-5.1.0/taskflow.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-01-05 10:10:07.000000 taskflow-5.1.0/taskflow.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2023-01-05 10:10:07.000000 taskflow-5.1.0/taskflow.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-01-05 10:10:07.000000 taskflow-5.1.0/taskflow.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-01-05 10:09:36.000000 taskflow-5.1.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:10:08.173206 taskflow-5.1.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      367 2023-01-05 10:09:36.000000 taskflow-5.1.0/tools/clear_zk.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3941 2023-01-05 10:09:36.000000 taskflow-5.1.0/tools/env_builder.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      444 2023-01-05 10:09:36.000000 taskflow-5.1.0/tools/pretty_tox.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3002 2023-01-05 10:09:36.000000 taskflow-5.1.0/tools/schema_generator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3999 2023-01-05 10:09:36.000000 taskflow-5.1.0/tools/speed_test.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7181 2023-01-05 10:09:36.000000 taskflow-5.1.0/tools/state_graph.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10572 2023-01-05 10:09:36.000000 taskflow-5.1.0/tools/subunit_trace.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1883 2023-01-05 10:09:36.000000 taskflow-5.1.0/tools/test-setup.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1521 2023-01-05 10:09:36.000000 taskflow-5.1.0/tools/update_states.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2271 2023-01-05 10:09:36.000000 taskflow-5.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.534478 taskflow-5.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-15 08:30:33.000000 taskflow-5.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-05-15 08:30:33.000000 taskflow-5.2.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-05-15 08:30:33.000000 taskflow-5.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-05-15 08:30:33.000000 taskflow-5.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-05-15 08:30:33.000000 taskflow-5.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4485 2023-05-15 08:31:01.000000 taskflow-5.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2023-05-15 08:30:33.000000 taskflow-5.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77501 2023-05-15 08:31:01.000000 taskflow-5.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-15 08:30:33.000000 taskflow-5.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4263 2023-05-15 08:31:01.534478 taskflow-5.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2380 2023-05-15 08:30:33.000000 taskflow-5.2.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-15 08:30:33.000000 taskflow-5.2.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.446476 taskflow-5.2.0/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.446476 taskflow-5.2.0/doc/diagrams/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/diagrams/area_of_influence.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16344 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/diagrams/core.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27254 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/diagrams/jobboard.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    99579 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/diagrams/tasks.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6967 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/diagrams/worker-engine.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.446476 taskflow-5.2.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2885 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.446476 taskflow-5.2.0/doc/source/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/templates/layout.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.450476 taskflow-5.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14336 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/arguments_and_results.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8573 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/atoms.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2743 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/conductors.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21501 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/engines.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8567 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/examples.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/exceptions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/history.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.458477 taskflow-5.2.0/doc/source/user/img/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7242 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/area_of_influence.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9664 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/conductor.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36940 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/conductor_cycle.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    68549 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/distributed_flow_rpc.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24407 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/engine_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26861 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/flow_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13531 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/job_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   110260 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/jobboard.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21971 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/mandelbrot.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22538 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/retry_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20666 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/task_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   241180 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/tasks.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16727 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/wbe_request_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25165 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/img/worker-engine.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5696 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/inputs_and_outputs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13665 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/jobs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6370 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/notifications.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/patterns.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12122 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/persistence.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7141 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/resumption.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/shelf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10022 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/states.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/types.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/utils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16388 2023-05-15 08:30:33.000000 taskflow-5.2.0/doc/source/user/workers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2023-05-15 08:30:33.000000 taskflow-5.2.0/pylintrc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.434476 taskflow-5.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.458477 taskflow-5.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/notes/add-sentinel-redis-support-9fd16e2a5dd5c0c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/notes/fix-endless-loop-on-storage-error-dd4467f0bbc66abf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/notes/fix-zookeeper-option-parsing-f9d37fbc39af47f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/notes/remove-strict-redis-f2a5a924b314de41.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/notes/zookeeper-ssl-support-b9abf24a39096b62.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.462477 taskflow-5.2.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.462477 taskflow-5.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.462477 taskflow-5.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9262 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-15 08:30:33.000000 taskflow-5.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-05-15 08:30:33.000000 taskflow-5.2.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1988 2023-05-15 08:30:33.000000 taskflow-5.2.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2838 2023-05-15 08:31:01.534478 taskflow-5.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-05-15 08:30:33.000000 taskflow-5.2.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.466477 taskflow-5.2.0/taskflow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17342 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/atom.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.470477 taskflow-5.2.0/taskflow/conductors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/conductors/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.470477 taskflow-5.2.0/taskflow/conductors/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/conductors/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/conductors/backends/impl_blocking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14816 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/conductors/backends/impl_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/conductors/backends/impl_nonblocking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7332 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/conductors/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.470477 taskflow-5.2.0/taskflow/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3402 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/deciders.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.470477 taskflow-5.2.0/taskflow/engines/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.474477 taskflow-5.2.0/taskflow/engines/action_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.474477 taskflow-5.2.0/taskflow/engines/action_engine/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/actions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1668 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/actions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/actions/retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/actions/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17015 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/builder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16164 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/compiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9028 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/completer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7254 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/deciders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29532 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7749 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27828 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/process_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13845 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/runtime.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4048 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/scopes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11558 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/selector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4552 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/action_engine/traversal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4865 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10952 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.478477 taskflow-5.2.0/taskflow/engines/worker_based/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7145 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/dispatcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4379 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13811 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20238 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/protocol.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9525 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11559 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9887 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6331 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/engines/worker_based/worker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.490477 taskflow-5.2.0/taskflow/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8893 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/99_bottles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3255 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/alphabet_soup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6554 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/build_a_car.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3909 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/buildsystem.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3917 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/calculate_in_parallel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4614 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/calculate_linear.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4336 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/create_parallel_volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/delayed_return.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4453 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/distance_calculator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/dump_memory_backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/echo_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3312 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/example_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6832 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/fake_billing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3461 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/graph_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4216 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/hello_world.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6821 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/jobboard_produce_consume_colors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/parallel_table_multiply.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3906 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/persistence_example.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/pseudo_scoping.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/pseudo_scoping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/resume_from_backend.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4992 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/resume_from_backend.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.494477 taskflow-5.2.0/taskflow/examples/resume_many_flows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1288 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/resume_many_flows/my_flows.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/resume_many_flows/resume_all.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/resume_many_flows/run_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/resume_many_flows.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3192 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/resume_many_flows.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9636 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/resume_vm_boot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/resume_volume_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/retry_flow.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/retry_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/reverting_linear.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3543 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/reverting_linear.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/run_by_iter.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2620 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/run_by_iter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/run_by_iter_enumerate.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/run_by_iter_enumerate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2742 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/share_engine_thread.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/simple_linear.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/simple_linear.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/simple_linear_listening.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3958 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/simple_linear_listening.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/simple_linear_pass.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/simple_linear_pass.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3762 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/simple_map_reduce.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/switch_graph_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/timing_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8472 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/tox_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5547 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/wbe_event_sender.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/wbe_mandelbrot.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8842 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/wbe_mandelbrot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/wbe_simple_linear.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5413 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/wbe_simple_linear.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4732 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/examples/wrapped_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11565 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7441 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/formatters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.494477 taskflow-5.2.0/taskflow/jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/jobs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.494477 taskflow-5.2.0/taskflow/jobs/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2902 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/jobs/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43520 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/jobs/backends/impl_redis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37643 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/jobs/backends/impl_zookeeper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22115 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/jobs/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.498478 taskflow-5.2.0/taskflow/listeners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/listeners/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7391 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/listeners/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4329 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/listeners/capturing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4115 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/listeners/claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8516 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/listeners/logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/listeners/printing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6943 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/listeners/timing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/logging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.498478 taskflow-5.2.0/taskflow/patterns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/patterns/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15292 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/patterns/graph_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/patterns/linear_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/patterns/unordered_flow.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.498478 taskflow-5.2.0/taskflow/persistence/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.502478 taskflow-5.2.0/taskflow/persistence/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/impl_dir.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13390 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/impl_memory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25656 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/impl_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6188 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/impl_zookeeper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.502478 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.502478 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2467 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.506478 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/0bc3e1a3c135_set_result_meduimtext_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/14b227d79a87_add_intention_column.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1c783c0c2875_replace_exception_an.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1cea328f0f65_initial_logbook_deta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1778 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/2ad4984f2864_switch_postgres_to_json_native.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/3162c0f3f8e4_add_revert_results_and_revert_failure_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/40fc8c914bd2_fix_atomdetails_failure_size.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/589dccdf2b6e_rename_taskdetails_to_atomdetails.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1072 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/6df9422fcb43_fix_flowdetails_meta_size.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/84d6e888850_add_task_detail_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1140 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4819 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4072 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40762 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9545 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/persistence/path_based.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14537 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6901 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52046 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10052 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10317 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.506478 taskflow-5.2.0/taskflow/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/test_examples.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.514478 taskflow-5.2.0/taskflow/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.518478 taskflow-5.2.0/taskflow/tests/unit/action_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/action_engine/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12866 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/action_engine/test_builder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23759 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/action_engine/test_compile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3517 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/action_engine/test_creation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/action_engine/test_process_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11327 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/action_engine/test_scoping.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.518478 taskflow-5.2.0/taskflow/tests/unit/jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/jobs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8447 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/jobs/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/jobs/test_entrypoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5174 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/jobs/test_redis_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13797 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/jobs/test_zk_job.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.518478 taskflow-5.2.0/taskflow/tests/unit/patterns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/patterns/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12464 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/patterns/test_graph_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5145 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/patterns/test_linear_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4985 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/patterns/test_unordered_flow.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.522478 taskflow-5.2.0/taskflow/tests/unit/persistence/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/persistence/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16547 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/persistence/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3929 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/persistence/test_dir_persistence.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7871 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/persistence/test_memory_persistence.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10260 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/persistence/test_sql_persistence.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3648 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/persistence/test_zk_persistence.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9204 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_arguments_passing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6173 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_check_transition.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18996 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_conductors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2733 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_deciders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5399 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_engine_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64393 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_engines.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4362 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17982 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_failure.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18086 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_flow_dependencies.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3921 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_formatters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_functor_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15304 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_listeners.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_mapfunctor_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7894 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5259 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_progress.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_reducefunctor_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56365 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_retries.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3660 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23520 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9900 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_suspend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15947 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20225 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11029 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_utils_async_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3168 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_utils_binary.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5716 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_utils_iter_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_utils_kazoo_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5503 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/test_utils_threading_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.522478 taskflow-5.2.0/taskflow/tests/unit/worker_based/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4045 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_creation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2915 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_dispatcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3128 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13622 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_message_pump.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3812 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_pipeline.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7745 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_protocol.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9920 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14344 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7109 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/unit/worker_based/test_worker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11157 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.526478 taskflow-5.2.0/taskflow/types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/types/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/types/entity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21189 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/types/failure.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10504 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/types/graph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2193 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/types/latch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14071 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/types/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4004 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/types/sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/types/timing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15820 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/types/tree.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.530478 taskflow-5.2.0/taskflow/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/async_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/banner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/eventlet_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/iter_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9915 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/kazoo_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/kombu_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18504 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/misc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3899 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/persistence_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4345 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/redis_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1434 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/schema_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5849 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/utils/threading_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2023-05-15 08:30:33.000000 taskflow-5.2.0/taskflow/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.470477 taskflow-5.2.0/taskflow.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4263 2023-05-15 08:31:01.000000 taskflow-5.2.0/taskflow.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12561 2023-05-15 08:31:01.000000 taskflow-5.2.0/taskflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:31:01.000000 taskflow-5.2.0/taskflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2023-05-15 08:31:01.000000 taskflow-5.2.0/taskflow.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:31:01.000000 taskflow-5.2.0/taskflow.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-05-15 08:31:01.000000 taskflow-5.2.0/taskflow.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2023-05-15 08:31:01.000000 taskflow-5.2.0/taskflow.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-05-15 08:31:01.000000 taskflow-5.2.0/taskflow.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-05-15 08:30:33.000000 taskflow-5.2.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:31:01.534478 taskflow-5.2.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      367 2023-05-15 08:30:33.000000 taskflow-5.2.0/tools/clear_zk.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3941 2023-05-15 08:30:33.000000 taskflow-5.2.0/tools/env_builder.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      444 2023-05-15 08:30:33.000000 taskflow-5.2.0/tools/pretty_tox.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3002 2023-05-15 08:30:33.000000 taskflow-5.2.0/tools/schema_generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3999 2023-05-15 08:30:33.000000 taskflow-5.2.0/tools/speed_test.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7181 2023-05-15 08:30:33.000000 taskflow-5.2.0/tools/state_graph.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10572 2023-05-15 08:30:33.000000 taskflow-5.2.0/tools/subunit_trace.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1883 2023-05-15 08:30:33.000000 taskflow-5.2.0/tools/test-setup.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1521 2023-05-15 08:30:33.000000 taskflow-5.2.0/tools/update_states.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2271 2023-05-15 08:30:33.000000 taskflow-5.2.0/tox.ini
```

### Comparing `taskflow-5.1.0/.mailmap` & `taskflow-5.2.0/.mailmap`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/.pre-commit-config.yaml` & `taskflow-5.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/AUTHORS` & `taskflow-5.2.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 Doug Hellmann <doug.hellmann@dreamhost.com>
 Doug Hellmann <doug@doughellmann.com>
 Elod Illes <elod.illes@est.tech>
 Eric Harney <eharney@redhat.com>
 Flavio Percoco <flaper87@gmail.com>
 Fredrik Bergroth <fbergroth@gmail.com>
 Gevorg Davoian <gdavoian@mirantis.com>
+Ghanshyam <gmann@ghanshyammann.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Greg Hill <greg.hill@rackspace.com>
 Gregory Thiemonge <gthiemon@redhat.com>
 Ha Manh Dong <donghm@vn.fujitsu.com>
 Hervé Beraud <hberaud@redhat.com>
 Ihar Hrachyshka <ihrachys@redhat.com>
 Ivan A. Melnikov <imelnikov@griddynamics.com>
@@ -70,14 +71,15 @@
 Stephen Finucane <stephenfin@redhat.com>
 Suneel Bomminayuni <suneelb@yahoo-inc.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Theodoros Tsioutsias <theodoros.tsioutsias@cern.ch>
 Thomas Bechtold <tbechtold@suse.com>
 Thomas Bechtold <thomasbechtold@jpberlin.de>
 Timofey Durakov <tdurakov@mirantis.com>
+Tobias Urdin <tobias.urdin@binero.com>
 Tony Breeds <tony@bakeyournoodle.com>
 Victor Rodionov <vito.ordaz@gmail.com>
 Vilobh Meshram <vilobhmm@yahoo-inc.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
 XiaojueGuan <guanalbertjone@gmail.com>
 YAMAMOTO Takashi <yamamoto@valinux.co.jp>
 Zhao Lei <zhaolei@cn.fujitsu.com>
@@ -90,14 +92,15 @@
 howardlee <lihongweibj@inspur.com>
 ji-xuepeng <ji.xuepeng@zte.com.cn>
 jiansong <jiansong19941206@gmail.com>
 leizhang <lei.a.zhang@intel.com>
 lin-hua-cheng <os.lcheng@gmail.com>
 liuqing <jing.liuqing@99cloud.net>
 liuwei <liuw147@chinaunicom.cn>
+ljhuang <huang.liujie@99cloud.net>
 luke.li <lilu7189@fiberhome.com>
 maaoyu <maaoyu@inspur.com>
 melissaml <ma.lei@99cloud.net>
 niuke <niuke19970315@163.com>
 qinchunhua <qin.chunhua@zte.com.cn>
 rahulram <rahurama@cisco.com>
 skudriashev <skudriashev@griddynamics.com>
```

### Comparing `taskflow-5.1.0/CONTRIBUTING.rst` & `taskflow-5.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/ChangeLog` & `taskflow-5.2.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 CHANGES
 =======
 
+5.2.0
+-----
+
+* Revert "Moves supported python runtimes from version 3.8 to 3.10"
+* Moves supported python runtimes from version 3.8 to 3.10
+* Fix doc building with Sphinx 6.0
+* Prepare taskflow for sqlalchemy2
+* Update master for stable/2023.1
+* Fix parsing of zookeeper jobboard backend options
+
 5.1.0
 -----
 
 * Fix test\_while\_is\_not with python 3.11
+* Change StrictRedis usage to Redis
 * remove unicode prefix from code
 * Adapt to new jsonschema versions
+* Replace abc.abstractproperty with property and abc.abstractmethod
 
 5.0.0
 -----
 
 * Quote string representations
 * Fix formattiing of release list
 * Remove six
```

### Comparing `taskflow-5.1.0/LICENSE` & `taskflow-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/PKG-INFO` & `taskflow-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskflow
-Version: 5.1.0
+Version: 5.2.0
 Summary: Taskflow structured state management library.
 Home-page: https://docs.openstack.org/taskflow/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -89,14 +89,15 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Provides-Extra: database
 Provides-Extra: eventlet
```

### Comparing `taskflow-5.1.0/README.rst` & `taskflow-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/diagrams/area_of_influence.graffle.tgz` & `taskflow-5.2.0/doc/diagrams/area_of_influence.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/diagrams/core.graffle.tgz` & `taskflow-5.2.0/doc/diagrams/core.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/diagrams/jobboard.graffle.tgz` & `taskflow-5.2.0/doc/diagrams/jobboard.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/diagrams/tasks.graffle.tgz` & `taskflow-5.2.0/doc/diagrams/tasks.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/diagrams/worker-engine.graffle.tgz` & `taskflow-5.2.0/doc/diagrams/worker-engine.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/conf.py` & `taskflow-5.2.0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 
 # Prefixes that are ignored for sorting the Python module index
 modindex_common_prefix = ['taskflow.']
 
 # Shortened external links.
 source_tree = 'https://opendev.org/openstack/taskflow/src/branch/master/'
 extlinks = {
-    'example': (source_tree + '/taskflow/examples/%s.py', ''),
-    'pybug': ('http://bugs.python.org/issue%s', ''),
+    'example': (source_tree + '/taskflow/examples/%s.py', '%s'),
+    'pybug': ('http://bugs.python.org/issue%s', '%s'),
 }
 
 
 # -- Options for HTML output --------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  Major themes that come with
 # Sphinx are currently 'default' and 'sphinxdoc'.
```

### Comparing `taskflow-5.1.0/doc/source/index.rst` & `taskflow-5.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/templates/layout.html` & `taskflow-5.2.0/doc/source/templates/layout.html`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/arguments_and_results.rst` & `taskflow-5.2.0/doc/source/user/arguments_and_results.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/atoms.rst` & `taskflow-5.2.0/doc/source/user/atoms.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/conductors.rst` & `taskflow-5.2.0/doc/source/user/conductors.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/engines.rst` & `taskflow-5.2.0/doc/source/user/engines.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/examples.rst` & `taskflow-5.2.0/doc/source/user/examples.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/area_of_influence.svg` & `taskflow-5.2.0/doc/source/user/img/area_of_influence.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/conductor.png` & `taskflow-5.2.0/doc/source/user/img/conductor.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/conductor_cycle.png` & `taskflow-5.2.0/doc/source/user/img/conductor_cycle.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/distributed_flow_rpc.png` & `taskflow-5.2.0/doc/source/user/img/distributed_flow_rpc.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/engine_states.svg` & `taskflow-5.2.0/doc/source/user/img/engine_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/flow_states.svg` & `taskflow-5.2.0/doc/source/user/img/flow_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/job_states.svg` & `taskflow-5.2.0/doc/source/user/img/job_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/jobboard.png` & `taskflow-5.2.0/doc/source/user/img/jobboard.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/mandelbrot.png` & `taskflow-5.2.0/doc/source/user/img/mandelbrot.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/retry_states.svg` & `taskflow-5.2.0/doc/source/user/img/retry_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/task_states.svg` & `taskflow-5.2.0/doc/source/user/img/task_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/tasks.png` & `taskflow-5.2.0/doc/source/user/img/tasks.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/wbe_request_states.svg` & `taskflow-5.2.0/doc/source/user/img/wbe_request_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/img/worker-engine.svg` & `taskflow-5.2.0/doc/source/user/img/worker-engine.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/index.rst` & `taskflow-5.2.0/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/inputs_and_outputs.rst` & `taskflow-5.2.0/doc/source/user/inputs_and_outputs.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/jobs.rst` & `taskflow-5.2.0/doc/source/user/jobs.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/notifications.rst` & `taskflow-5.2.0/doc/source/user/notifications.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/persistence.rst` & `taskflow-5.2.0/doc/source/user/persistence.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/resumption.rst` & `taskflow-5.2.0/doc/source/user/resumption.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/shelf.rst` & `taskflow-5.2.0/doc/source/user/shelf.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/states.rst` & `taskflow-5.2.0/doc/source/user/states.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/types.rst` & `taskflow-5.2.0/doc/source/user/types.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/utils.rst` & `taskflow-5.2.0/doc/source/user/utils.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/doc/source/user/workers.rst` & `taskflow-5.2.0/doc/source/user/workers.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/pylintrc` & `taskflow-5.2.0/pylintrc`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/releasenotes/source/conf.py` & `taskflow-5.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/requirements.txt` & `taskflow-5.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/run_tests.sh` & `taskflow-5.2.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/setup.cfg` & `taskflow-5.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development :: Libraries
 	Topic :: System :: Distributed Computing
 
 [files]
 packages =
```

### Comparing `taskflow-5.1.0/setup.py` & `taskflow-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/atom.py` & `taskflow-5.2.0/taskflow/atom.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/conductors/backends/__init__.py` & `taskflow-5.2.0/taskflow/conductors/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/conductors/backends/impl_blocking.py` & `taskflow-5.2.0/taskflow/conductors/backends/impl_blocking.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/conductors/backends/impl_executor.py` & `taskflow-5.2.0/taskflow/conductors/backends/impl_executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/conductors/backends/impl_nonblocking.py` & `taskflow-5.2.0/taskflow/conductors/backends/impl_nonblocking.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/conductors/base.py` & `taskflow-5.2.0/taskflow/conductors/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/deciders.py` & `taskflow-5.2.0/taskflow/deciders.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/__init__.py` & `taskflow-5.2.0/taskflow/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/actions/base.py` & `taskflow-5.2.0/taskflow/engines/action_engine/actions/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/actions/retry.py` & `taskflow-5.2.0/taskflow/engines/action_engine/actions/retry.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/actions/task.py` & `taskflow-5.2.0/taskflow/engines/action_engine/actions/task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/builder.py` & `taskflow-5.2.0/taskflow/engines/action_engine/builder.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/compiler.py` & `taskflow-5.2.0/taskflow/engines/action_engine/compiler.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/completer.py` & `taskflow-5.2.0/taskflow/engines/action_engine/completer.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/deciders.py` & `taskflow-5.2.0/taskflow/engines/action_engine/deciders.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/engine.py` & `taskflow-5.2.0/taskflow/engines/action_engine/engine.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/executor.py` & `taskflow-5.2.0/taskflow/engines/action_engine/executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/process_executor.py` & `taskflow-5.2.0/taskflow/engines/action_engine/process_executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/runtime.py` & `taskflow-5.2.0/taskflow/engines/action_engine/runtime.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/scheduler.py` & `taskflow-5.2.0/taskflow/engines/action_engine/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/scopes.py` & `taskflow-5.2.0/taskflow/engines/action_engine/scopes.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/selector.py` & `taskflow-5.2.0/taskflow/engines/action_engine/selector.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/action_engine/traversal.py` & `taskflow-5.2.0/taskflow/engines/action_engine/traversal.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/base.py` & `taskflow-5.2.0/taskflow/engines/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,21 @@
         return self._atom_notifier
 
     @property
     def options(self):
         """The options that were passed to this engine on construction."""
         return self._options
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def storage(self):
         """The storage unit for this engine."""
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def statistics(self):
         """A dictionary of runtime statistics this engine has gathered.
 
         This dictionary will be empty when the engine has never been
         ran. When it is running or has ran previously it should have (but
         may not) have useful and/or informational keys and values when
         running is underway and/or completed.
```

### Comparing `taskflow-5.1.0/taskflow/engines/helpers.py` & `taskflow-5.2.0/taskflow/engines/helpers.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/worker_based/dispatcher.py` & `taskflow-5.2.0/taskflow/engines/worker_based/dispatcher.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/worker_based/endpoint.py` & `taskflow-5.2.0/taskflow/engines/worker_based/endpoint.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/worker_based/engine.py` & `taskflow-5.2.0/taskflow/engines/worker_based/engine.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/worker_based/executor.py` & `taskflow-5.2.0/taskflow/engines/worker_based/executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/worker_based/protocol.py` & `taskflow-5.2.0/taskflow/engines/worker_based/protocol.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/worker_based/proxy.py` & `taskflow-5.2.0/taskflow/engines/worker_based/proxy.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/worker_based/server.py` & `taskflow-5.2.0/taskflow/engines/worker_based/server.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/worker_based/types.py` & `taskflow-5.2.0/taskflow/engines/worker_based/types.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/engines/worker_based/worker.py` & `taskflow-5.2.0/taskflow/engines/worker_based/worker.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/99_bottles.py` & `taskflow-5.2.0/taskflow/examples/99_bottles.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/alphabet_soup.py` & `taskflow-5.2.0/taskflow/examples/alphabet_soup.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/build_a_car.py` & `taskflow-5.2.0/taskflow/examples/build_a_car.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/buildsystem.py` & `taskflow-5.2.0/taskflow/examples/buildsystem.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/calculate_in_parallel.py` & `taskflow-5.2.0/taskflow/examples/calculate_in_parallel.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/calculate_linear.py` & `taskflow-5.2.0/taskflow/examples/calculate_linear.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/create_parallel_volume.py` & `taskflow-5.2.0/taskflow/examples/create_parallel_volume.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/delayed_return.py` & `taskflow-5.2.0/taskflow/examples/delayed_return.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/distance_calculator.py` & `taskflow-5.2.0/taskflow/examples/distance_calculator.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/dump_memory_backend.py` & `taskflow-5.2.0/taskflow/examples/dump_memory_backend.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/echo_listener.py` & `taskflow-5.2.0/taskflow/examples/echo_listener.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/example_utils.py` & `taskflow-5.2.0/taskflow/examples/example_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/fake_billing.py` & `taskflow-5.2.0/taskflow/examples/fake_billing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/graph_flow.py` & `taskflow-5.2.0/taskflow/examples/graph_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/hello_world.py` & `taskflow-5.2.0/taskflow/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/jobboard_produce_consume_colors.py` & `taskflow-5.2.0/taskflow/examples/jobboard_produce_consume_colors.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/parallel_table_multiply.py` & `taskflow-5.2.0/taskflow/examples/parallel_table_multiply.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/persistence_example.py` & `taskflow-5.2.0/taskflow/examples/persistence_example.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/pseudo_scoping.py` & `taskflow-5.2.0/taskflow/examples/pseudo_scoping.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/resume_from_backend.out.txt` & `taskflow-5.2.0/taskflow/examples/resume_from_backend.out.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/resume_from_backend.py` & `taskflow-5.2.0/taskflow/examples/resume_from_backend.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/resume_many_flows/my_flows.py` & `taskflow-5.2.0/taskflow/examples/resume_many_flows/my_flows.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/resume_many_flows/resume_all.py` & `taskflow-5.2.0/taskflow/examples/resume_many_flows/resume_all.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/resume_many_flows/run_flow.py` & `taskflow-5.2.0/taskflow/examples/resume_many_flows/run_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/resume_many_flows.out.txt` & `taskflow-5.2.0/taskflow/examples/resume_many_flows.out.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/resume_many_flows.py` & `taskflow-5.2.0/taskflow/examples/resume_many_flows.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/resume_vm_boot.py` & `taskflow-5.2.0/taskflow/examples/resume_vm_boot.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/resume_volume_create.py` & `taskflow-5.2.0/taskflow/examples/resume_volume_create.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/retry_flow.py` & `taskflow-5.2.0/taskflow/examples/retry_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/reverting_linear.py` & `taskflow-5.2.0/taskflow/examples/reverting_linear.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/run_by_iter.out.txt` & `taskflow-5.2.0/taskflow/examples/run_by_iter.out.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/run_by_iter.py` & `taskflow-5.2.0/taskflow/examples/run_by_iter.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/run_by_iter_enumerate.out.txt` & `taskflow-5.2.0/taskflow/examples/run_by_iter_enumerate.out.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/run_by_iter_enumerate.py` & `taskflow-5.2.0/taskflow/examples/run_by_iter_enumerate.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/share_engine_thread.py` & `taskflow-5.2.0/taskflow/examples/share_engine_thread.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/simple_linear.py` & `taskflow-5.2.0/taskflow/examples/simple_linear.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/simple_linear_listening.py` & `taskflow-5.2.0/taskflow/examples/simple_linear_listening.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/simple_linear_pass.py` & `taskflow-5.2.0/taskflow/examples/simple_linear_pass.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/simple_map_reduce.py` & `taskflow-5.2.0/taskflow/examples/simple_map_reduce.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/switch_graph_flow.py` & `taskflow-5.2.0/taskflow/examples/switch_graph_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/timing_listener.py` & `taskflow-5.2.0/taskflow/examples/timing_listener.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/tox_conductor.py` & `taskflow-5.2.0/taskflow/examples/tox_conductor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/wbe_event_sender.py` & `taskflow-5.2.0/taskflow/examples/wbe_event_sender.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/wbe_mandelbrot.py` & `taskflow-5.2.0/taskflow/examples/wbe_mandelbrot.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/wbe_simple_linear.py` & `taskflow-5.2.0/taskflow/examples/wbe_simple_linear.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/examples/wrapped_exception.py` & `taskflow-5.2.0/taskflow/examples/wrapped_exception.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/exceptions.py` & `taskflow-5.2.0/taskflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/flow.py` & `taskflow-5.2.0/taskflow/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,10 +124,11 @@
         provides = set()
         if self._retry is not None:
             provides.update(self._retry.provides)
         for item in self:
             provides.update(item.provides)
         return frozenset(provides)
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def requires(self):
         """Set of *unsatisfied* symbol names required by the flow."""
```

### Comparing `taskflow-5.1.0/taskflow/formatters.py` & `taskflow-5.2.0/taskflow/formatters.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/jobs/backends/__init__.py` & `taskflow-5.2.0/taskflow/jobs/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/jobs/backends/impl_redis.py` & `taskflow-5.2.0/taskflow/jobs/backends/impl_redis.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/jobs/backends/impl_zookeeper.py` & `taskflow-5.2.0/taskflow/jobs/backends/impl_zookeeper.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import futurist
 from kazoo import exceptions as k_exceptions
 from kazoo.protocol import paths as k_paths
 from kazoo.protocol import states as k_states
 from kazoo.recipe import watchers
 from oslo_serialization import jsonutils
 from oslo_utils import excutils
+from oslo_utils import strutils
 from oslo_utils import timeutils
 from oslo_utils import uuidutils
 
 from taskflow.conductors import base as c_base
 from taskflow import exceptions as excp
 from taskflow.jobs import base
 from taskflow import logging
@@ -825,15 +826,16 @@
             self._client.start(timeout=timeout)
             self._closing = False
         except (self._client.handler.timeout_exception,
                 k_exceptions.KazooException):
             excp.raise_with_cause(excp.JobFailure,
                                   "Failed to connect to zookeeper")
         try:
-            if self._conf.get('check_compatible', True):
+            if strutils.bool_from_string(
+                    self._conf.get('check_compatible'), default=True):
                 kazoo_utils.check_compatible(self._client, self.MIN_ZK_VERSION)
             if self._worker is None and self._emit_notifications:
                 self._worker = futurist.ThreadPoolExecutor(max_workers=1)
             self._client.ensure_path(self.path)
             self._client.ensure_path(self.trash_path)
             if self._job_watcher is None:
                 self._job_watcher = watchers.ChildrenWatch(
```

### Comparing `taskflow-5.1.0/taskflow/jobs/base.py` & `taskflow-5.2.0/taskflow/jobs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,32 +138,36 @@
         self._backend = backend
         self._board = board
         self._book = book
         if not book_data:
             book_data = {}
         self._book_data = book_data
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def last_modified(self):
         """The datetime the job was last modified."""
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def created_on(self):
         """The datetime the job was created on."""
 
     @property
     def board(self):
         """The board this job was posted on or was created from."""
         return self._board
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def state(self):
         """Access the current state of this job."""
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def priority(self):
         """The :py:class:`~.JobPriority` of this job."""
 
     def wait(self, timeout=None,
              delay=0.01, delay_multiplier=2.0, max_delay=60.0,
              sleep_func=time.sleep):
         """Wait for job to enter completion state.
@@ -393,15 +397,16 @@
         jobs after the iterator has been created (be aware of this when
         using it).
 
         :param timeout: float that indicates how long to wait for a job to
             appear (if None then waits forever).
         """
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def job_count(self):
         """Returns how many jobs are on this jobboard.
 
         NOTE(harlowja): this count may change as jobs appear or are removed so
         the accuracy of this count should not be used in a way that requires
         it to be exact & absolute.
         """
@@ -512,15 +517,16 @@
         """Register an entity to the jobboard('s backend), e.g: a conductor.
 
         :param entity: entity to register as being associated with the
                        jobboard('s backend)
         :type entity: :py:class:`~taskflow.types.entity.Entity`
         """
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def connected(self):
         """Returns if this jobboard is connected."""
 
     @abc.abstractmethod
     def connect(self):
         """Opens the connection to any backend system."""
```

### Comparing `taskflow-5.1.0/taskflow/listeners/base.py` & `taskflow-5.2.0/taskflow/listeners/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/listeners/capturing.py` & `taskflow-5.2.0/taskflow/listeners/capturing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/listeners/claims.py` & `taskflow-5.2.0/taskflow/listeners/claims.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/listeners/logging.py` & `taskflow-5.2.0/taskflow/listeners/logging.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/listeners/printing.py` & `taskflow-5.2.0/taskflow/listeners/printing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/listeners/timing.py` & `taskflow-5.2.0/taskflow/listeners/timing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/logging.py` & `taskflow-5.2.0/taskflow/logging.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/patterns/graph_flow.py` & `taskflow-5.2.0/taskflow/patterns/graph_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/patterns/linear_flow.py` & `taskflow-5.2.0/taskflow/patterns/linear_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/patterns/unordered_flow.py` & `taskflow-5.2.0/taskflow/patterns/unordered_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/__init__.py` & `taskflow-5.2.0/taskflow/persistence/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/impl_dir.py` & `taskflow-5.2.0/taskflow/persistence/backends/impl_dir.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/impl_memory.py` & `taskflow-5.2.0/taskflow/persistence/backends/impl_memory.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/impl_sqlalchemy.py` & `taskflow-5.2.0/taskflow/persistence/backends/impl_sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,23 +201,25 @@
     @staticmethod
     def convert_atom_detail(row):
         row = dict(row.items())
         atom_cls = models.atom_detail_class(row.pop('atom_type'))
         return atom_cls.from_dict(row)
 
     def atom_query_iter(self, conn, parent_uuid):
-        q = (sql.select([self._tables.atomdetails]).
+        q = (sql.select(self._tables.atomdetails).
              where(self._tables.atomdetails.c.parent_uuid == parent_uuid))
         for row in conn.execute(q):
+            row = row._mapping
             yield self.convert_atom_detail(row)
 
     def flow_query_iter(self, conn, parent_uuid):
-        q = (sql.select([self._tables.flowdetails]).
+        q = (sql.select(self._tables.flowdetails).
              where(self._tables.flowdetails.c.parent_uuid == parent_uuid))
         for row in conn.execute(q):
+            row = row._mapping
             yield self.convert_flow_detail(row)
 
     def populate_book(self, conn, book):
         for fd in self.flow_query_iter(conn, book.uuid):
             book.add(fd)
             self.populate_flow_detail(conn, fd)
 
@@ -253,15 +255,14 @@
     @staticmethod
     def _create_engine(conf):
         # NOTE(harlowja): copy the internal one so that we don't modify it via
         # all the popping that will happen below.
         conf = copy.deepcopy(conf)
         engine_args = {
             'echo': _as_bool(conf.pop('echo', False)),
-            'convert_unicode': _as_bool(conf.pop('convert_unicode', True)),
             'pool_recycle': 3600,
         }
         if 'idle_timeout' in conf:
             idle_timeout = misc.as_int(conf.pop('idle_timeout'))
             engine_args['pool_recycle'] = idle_timeout
         sql_connection = conf.pop('connection')
         e_url = sa.engine.url.make_url(sql_connection)
@@ -417,40 +418,41 @@
             exc.raise_with_cause(exc.StorageFailure,
                                  "Failed clearing all entries")
 
     def update_atom_details(self, atom_detail):
         try:
             atomdetails = self._tables.atomdetails
             with self._engine.begin() as conn:
-                q = (sql.select([atomdetails]).
+                q = (sql.select(atomdetails).
                      where(atomdetails.c.uuid == atom_detail.uuid))
                 row = conn.execute(q).first()
                 if not row:
                     raise exc.NotFound("No atom details found with uuid"
                                        " '%s'" % atom_detail.uuid)
+                row = row._mapping
                 e_ad = self._converter.convert_atom_detail(row)
                 self._update_atom_details(conn, atom_detail, e_ad)
             return e_ad
         except sa_exc.SQLAlchemyError:
             exc.raise_with_cause(exc.StorageFailure,
                                  "Failed updating atom details"
                                  " with uuid '%s'" % atom_detail.uuid)
 
     def _insert_flow_details(self, conn, fd, parent_uuid):
         value = fd.to_dict()
         value['parent_uuid'] = parent_uuid
-        conn.execute(sql.insert(self._tables.flowdetails, value))
+        conn.execute(sql.insert(self._tables.flowdetails).values(**value))
         for ad in fd:
             self._insert_atom_details(conn, ad, fd.uuid)
 
     def _insert_atom_details(self, conn, ad, parent_uuid):
         value = ad.to_dict()
         value['parent_uuid'] = parent_uuid
         value['atom_type'] = models.atom_detail_type(ad)
-        conn.execute(sql.insert(self._tables.atomdetails, value))
+        conn.execute(sql.insert(self._tables.atomdetails).values(**value))
 
     def _update_atom_details(self, conn, ad, e_ad):
         e_ad.merge(ad)
         conn.execute(sql.update(self._tables.atomdetails)
                      .where(self._tables.atomdetails.c.uuid == e_ad.uuid)
                      .values(e_ad.to_dict()))
 
@@ -467,20 +469,21 @@
             else:
                 self._update_atom_details(conn, ad, e_ad)
 
     def update_flow_details(self, flow_detail):
         try:
             flowdetails = self._tables.flowdetails
             with self._engine.begin() as conn:
-                q = (sql.select([flowdetails]).
+                q = (sql.select(flowdetails).
                      where(flowdetails.c.uuid == flow_detail.uuid))
                 row = conn.execute(q).first()
                 if not row:
                     raise exc.NotFound("No flow details found with"
                                        " uuid '%s'" % flow_detail.uuid)
+                row = row._mapping
                 e_fd = self._converter.convert_flow_detail(row)
                 self._converter.populate_flow_detail(conn, e_fd)
                 self._update_flow_details(conn, flow_detail, e_fd)
             return e_fd
         except sa_exc.SQLAlchemyError:
             exc.raise_with_cause(exc.StorageFailure,
                                  "Failed updating flow details with"
@@ -499,18 +502,19 @@
             exc.raise_with_cause(exc.StorageFailure,
                                  "Failed destroying logbook '%s'" % book_uuid)
 
     def save_logbook(self, book):
         try:
             logbooks = self._tables.logbooks
             with self._engine.begin() as conn:
-                q = (sql.select([logbooks]).
+                q = (sql.select(logbooks).
                      where(logbooks.c.uuid == book.uuid))
                 row = conn.execute(q).first()
                 if row:
+                    row = row._mapping
                     e_lb = self._converter.convert_book(row)
                     self._converter.populate_book(conn, e_lb)
                     e_lb.merge(book)
                     conn.execute(sql.update(logbooks)
                                  .where(logbooks.c.uuid == e_lb.uuid)
                                  .values(e_lb.to_dict()))
                     for fd in book:
@@ -518,47 +522,49 @@
                         if e_fd is None:
                             e_lb.add(fd)
                             self._insert_flow_details(conn, fd, e_lb.uuid)
                         else:
                             self._update_flow_details(conn, fd, e_fd)
                     return e_lb
                 else:
-                    conn.execute(sql.insert(logbooks, book.to_dict()))
+                    conn.execute(sql.insert(logbooks).values(**book.to_dict()))
                     for fd in book:
                         self._insert_flow_details(conn, fd, book.uuid)
                     return book
         except sa_exc.DBAPIError:
             exc.raise_with_cause(
                 exc.StorageFailure,
                 "Failed saving logbook '%s'" % book.uuid)
 
     def get_logbook(self, book_uuid, lazy=False):
         try:
             logbooks = self._tables.logbooks
             with contextlib.closing(self._engine.connect()) as conn:
-                q = (sql.select([logbooks]).
+                q = (sql.select(logbooks).
                      where(logbooks.c.uuid == book_uuid))
                 row = conn.execute(q).first()
                 if not row:
                     raise exc.NotFound("No logbook found with"
                                        " uuid '%s'" % book_uuid)
+                row = row._mapping
                 book = self._converter.convert_book(row)
                 if not lazy:
                     self._converter.populate_book(conn, book)
                 return book
         except sa_exc.DBAPIError:
             exc.raise_with_cause(exc.StorageFailure,
                                  "Failed getting logbook '%s'" % book_uuid)
 
     def get_logbooks(self, lazy=False):
         gathered = []
         try:
             with contextlib.closing(self._engine.connect()) as conn:
-                q = sql.select([self._tables.logbooks])
+                q = sql.select(self._tables.logbooks)
                 for row in conn.execute(q):
+                    row = row._mapping
                     book = self._converter.convert_book(row)
                     if not lazy:
                         self._converter.populate_book(conn, book)
                     gathered.append(book)
         except sa_exc.DBAPIError:
             exc.raise_with_cause(exc.StorageFailure,
                                  "Failed getting logbooks")
@@ -580,39 +586,41 @@
         for flow_details in gathered:
             yield flow_details
 
     def get_flow_details(self, fd_uuid, lazy=False):
         try:
             flowdetails = self._tables.flowdetails
             with self._engine.begin() as conn:
-                q = (sql.select([flowdetails]).
+                q = (sql.select(flowdetails).
                      where(flowdetails.c.uuid == fd_uuid))
                 row = conn.execute(q).first()
                 if not row:
                     raise exc.NotFound("No flow details found with uuid"
                                        " '%s'" % fd_uuid)
+                row = row._mapping
                 fd = self._converter.convert_flow_detail(row)
                 if not lazy:
                     self._converter.populate_flow_detail(conn, fd)
                 return fd
         except sa_exc.SQLAlchemyError:
             exc.raise_with_cause(exc.StorageFailure,
                                  "Failed getting flow details with"
                                  " uuid '%s'" % fd_uuid)
 
     def get_atom_details(self, ad_uuid):
         try:
             atomdetails = self._tables.atomdetails
             with self._engine.begin() as conn:
-                q = (sql.select([atomdetails]).
+                q = (sql.select(atomdetails).
                      where(atomdetails.c.uuid == ad_uuid))
                 row = conn.execute(q).first()
                 if not row:
                     raise exc.NotFound("No atom details found with uuid"
                                        " '%s'" % ad_uuid)
+                row = row._mapping
                 return self._converter.convert_atom_detail(row)
         except sa_exc.SQLAlchemyError:
             exc.raise_with_cause(exc.StorageFailure,
                                  "Failed getting atom details with"
                                  " uuid '%s'" % ad_uuid)
 
     def get_atoms_for_flow(self, fd_uuid):
```

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/impl_zookeeper.py` & `taskflow-5.2.0/taskflow/persistence/backends/impl_zookeeper.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #    under the License.
 
 import contextlib
 
 from kazoo import exceptions as k_exc
 from kazoo.protocol import paths
 from oslo_serialization import jsonutils
+from oslo_utils import strutils
 
 from taskflow import exceptions as exc
 from taskflow.persistence import path_based
 from taskflow.utils import kazoo_utils as k_utils
 from taskflow.utils import misc
 
 
@@ -157,12 +158,13 @@
         with self._exc_wrapper():
             yield transaction
             k_utils.checked_commit(transaction)
 
     def validate(self):
         with self._exc_wrapper():
             try:
-                if self._conf.get('check_compatible', True):
+                if strutils.bool_from_string(
+                        self._conf.get('check_compatible'), default=True):
                     k_utils.check_compatible(self._client, MIN_ZK_VERSION)
             except exc.IncompatibleVersion:
                 exc.raise_with_cause(exc.StorageFailure, "Backend storage is"
                                      " not a compatible version")
```

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/env.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/0bc3e1a3c135_set_result_meduimtext_type.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/0bc3e1a3c135_set_result_meduimtext_type.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/14b227d79a87_add_intention_column.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/14b227d79a87_add_intention_column.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1c783c0c2875_replace_exception_an.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1c783c0c2875_replace_exception_an.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1cea328f0f65_initial_logbook_deta.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1cea328f0f65_initial_logbook_deta.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/2ad4984f2864_switch_postgres_to_json_native.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/2ad4984f2864_switch_postgres_to_json_native.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/3162c0f3f8e4_add_revert_results_and_revert_failure_.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/3162c0f3f8e4_add_revert_results_and_revert_failure_.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/40fc8c914bd2_fix_atomdetails_failure_size.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/40fc8c914bd2_fix_atomdetails_failure_size.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/589dccdf2b6e_rename_taskdetails_to_atomdetails.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/589dccdf2b6e_rename_taskdetails_to_atomdetails.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/6df9422fcb43_fix_flowdetails_meta_size.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/6df9422fcb43_fix_flowdetails_meta_size.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/84d6e888850_add_task_detail_type.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/84d6e888850_add_task_detail_type.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/migration.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/backends/sqlalchemy/tables.py` & `taskflow-5.2.0/taskflow/persistence/backends/sqlalchemy/tables.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/base.py` & `taskflow-5.2.0/taskflow/persistence/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     def close(self):
         """Closes any resources this backend has open."""
 
 
 class Connection(object, metaclass=abc.ABCMeta):
     """Base class for backend connections."""
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def backend(self):
         """Returns the backend this connection is associated with."""
 
     @abc.abstractmethod
     def close(self):
         """Closes any resources this connection has open."""
```

### Comparing `taskflow-5.1.0/taskflow/persistence/models.py` & `taskflow-5.2.0/taskflow/persistence/models.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/persistence/path_based.py` & `taskflow-5.2.0/taskflow/persistence/path_based.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/retry.py` & `taskflow-5.2.0/taskflow/retry.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/states.py` & `taskflow-5.2.0/taskflow/states.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/storage.py` & `taskflow-5.2.0/taskflow/storage.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/task.py` & `taskflow-5.2.0/taskflow/task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/test.py` & `taskflow-5.2.0/taskflow/test.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/test_examples.py` & `taskflow-5.2.0/taskflow/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/action_engine/test_builder.py` & `taskflow-5.2.0/taskflow/tests/unit/action_engine/test_builder.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/action_engine/test_compile.py` & `taskflow-5.2.0/taskflow/tests/unit/action_engine/test_compile.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/action_engine/test_creation.py` & `taskflow-5.2.0/taskflow/tests/unit/action_engine/test_creation.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/action_engine/test_process_executor.py` & `taskflow-5.2.0/taskflow/tests/unit/action_engine/test_process_executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/action_engine/test_scoping.py` & `taskflow-5.2.0/taskflow/tests/unit/action_engine/test_scoping.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/jobs/base.py` & `taskflow-5.2.0/taskflow/tests/unit/jobs/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/jobs/test_entrypoint.py` & `taskflow-5.2.0/taskflow/tests/unit/jobs/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/jobs/test_redis_job.py` & `taskflow-5.2.0/taskflow/tests/unit/jobs/test_redis_job.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/jobs/test_zk_job.py` & `taskflow-5.2.0/taskflow/tests/unit/jobs/test_zk_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -289,7 +289,51 @@
         entity_instance_2 = entity.Entity("non-sense",
                                           "other_name",
                                           {})
         with base.connect_close(self.board):
             self.assertRaises(excp.NotImplementedError,
                               self.board.register_entity,
                               entity_instance_2)
+
+    def test_connect_check_compatible(self):
+        # Valid version
+        client = fake_client.FakeClient()
+        board = impl_zookeeper.ZookeeperJobBoard(
+            'test-board', {'check_compatible': True},
+            client=client)
+        self.addCleanup(board.close)
+        self.addCleanup(self.close_client, client)
+
+        with base.connect_close(board):
+            pass
+
+        # Invalid version, no check
+        client = fake_client.FakeClient(server_version=(3, 2, 0))
+        board = impl_zookeeper.ZookeeperJobBoard(
+            'test-board', {'check_compatible': False},
+            client=client)
+        self.addCleanup(board.close)
+        self.addCleanup(self.close_client, client)
+
+        with base.connect_close(board):
+            pass
+
+        # Invalid version, check_compatible=True
+        client = fake_client.FakeClient(server_version=(3, 2, 0))
+        board = impl_zookeeper.ZookeeperJobBoard(
+            'test-board', {'check_compatible': True},
+            client=client)
+        self.addCleanup(board.close)
+        self.addCleanup(self.close_client, client)
+
+        self.assertRaises(excp.IncompatibleVersion, board.connect)
+
+        # Invalid version, check_compatible='False'
+        client = fake_client.FakeClient(server_version=(3, 2, 0))
+        board = impl_zookeeper.ZookeeperJobBoard(
+            'test-board', {'check_compatible': 'False'},
+            client=client)
+        self.addCleanup(board.close)
+        self.addCleanup(self.close_client, client)
+
+        with base.connect_close(board):
+            pass
```

### Comparing `taskflow-5.1.0/taskflow/tests/unit/patterns/test_graph_flow.py` & `taskflow-5.2.0/taskflow/tests/unit/patterns/test_graph_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/patterns/test_linear_flow.py` & `taskflow-5.2.0/taskflow/tests/unit/patterns/test_linear_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/patterns/test_unordered_flow.py` & `taskflow-5.2.0/taskflow/tests/unit/patterns/test_unordered_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/persistence/base.py` & `taskflow-5.2.0/taskflow/tests/unit/persistence/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/persistence/test_dir_persistence.py` & `taskflow-5.2.0/taskflow/tests/unit/persistence/test_dir_persistence.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/persistence/test_memory_persistence.py` & `taskflow-5.2.0/taskflow/tests/unit/persistence/test_memory_persistence.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/persistence/test_sql_persistence.py` & `taskflow-5.2.0/taskflow/tests/unit/persistence/test_sql_persistence.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/persistence/test_zk_persistence.py` & `taskflow-5.2.0/taskflow/tests/unit/persistence/test_zk_persistence.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_arguments_passing.py` & `taskflow-5.2.0/taskflow/tests/unit/test_arguments_passing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_check_transition.py` & `taskflow-5.2.0/taskflow/tests/unit/test_check_transition.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_conductors.py` & `taskflow-5.2.0/taskflow/tests/unit/test_conductors.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_deciders.py` & `taskflow-5.2.0/taskflow/tests/unit/test_deciders.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_engine_helpers.py` & `taskflow-5.2.0/taskflow/tests/unit/test_engine_helpers.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_engines.py` & `taskflow-5.2.0/taskflow/tests/unit/test_engines.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_exceptions.py` & `taskflow-5.2.0/taskflow/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_failure.py` & `taskflow-5.2.0/taskflow/tests/unit/test_failure.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_flow_dependencies.py` & `taskflow-5.2.0/taskflow/tests/unit/test_flow_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_formatters.py` & `taskflow-5.2.0/taskflow/tests/unit/test_formatters.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_functor_task.py` & `taskflow-5.2.0/taskflow/tests/unit/test_functor_task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_listeners.py` & `taskflow-5.2.0/taskflow/tests/unit/test_listeners.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_mapfunctor_task.py` & `taskflow-5.2.0/taskflow/tests/unit/test_mapfunctor_task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_notifier.py` & `taskflow-5.2.0/taskflow/tests/unit/test_notifier.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_progress.py` & `taskflow-5.2.0/taskflow/tests/unit/test_progress.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_reducefunctor_task.py` & `taskflow-5.2.0/taskflow/tests/unit/test_reducefunctor_task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_retries.py` & `taskflow-5.2.0/taskflow/tests/unit/test_retries.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_states.py` & `taskflow-5.2.0/taskflow/tests/unit/test_states.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_storage.py` & `taskflow-5.2.0/taskflow/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_suspend.py` & `taskflow-5.2.0/taskflow/tests/unit/test_suspend.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_task.py` & `taskflow-5.2.0/taskflow/tests/unit/test_task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_types.py` & `taskflow-5.2.0/taskflow/tests/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_utils.py` & `taskflow-5.2.0/taskflow/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_utils_async_utils.py` & `taskflow-5.2.0/taskflow/tests/unit/test_utils_async_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_utils_binary.py` & `taskflow-5.2.0/taskflow/tests/unit/test_utils_binary.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_utils_iter_utils.py` & `taskflow-5.2.0/taskflow/tests/unit/test_utils_iter_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/test_utils_threading_utils.py` & `taskflow-5.2.0/taskflow/tests/unit/test_utils_threading_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_creation.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_creation.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_dispatcher.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_endpoint.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_executor.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_message_pump.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_message_pump.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_pipeline.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_protocol.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_protocol.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_proxy.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_proxy.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_server.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_server.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_types.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_types.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/unit/worker_based/test_worker.py` & `taskflow-5.2.0/taskflow/tests/unit/worker_based/test_worker.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/tests/utils.py` & `taskflow-5.2.0/taskflow/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     except Exception:
         return False
     finally:
         kazoo_utils.finalize_client(client)
 
 
 def redis_available(min_version):
-    client = redis.StrictRedis()
+    client = redis.Redis()
     try:
         client.ping()
     except Exception:
         return False
     else:
         ok, redis_version = redis_utils.is_server_new_enough(client,
                                                              min_version)
```

### Comparing `taskflow-5.1.0/taskflow/types/entity.py` & `taskflow-5.2.0/taskflow/types/entity.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/types/failure.py` & `taskflow-5.2.0/taskflow/types/failure.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/types/graph.py` & `taskflow-5.2.0/taskflow/types/graph.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/types/latch.py` & `taskflow-5.2.0/taskflow/types/latch.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/types/notifier.py` & `taskflow-5.2.0/taskflow/types/notifier.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/types/sets.py` & `taskflow-5.2.0/taskflow/types/sets.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/types/timing.py` & `taskflow-5.2.0/taskflow/types/timing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/types/tree.py` & `taskflow-5.2.0/taskflow/types/tree.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/utils/async_utils.py` & `taskflow-5.2.0/taskflow/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/utils/banner.py` & `taskflow-5.2.0/taskflow/utils/banner.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/utils/eventlet_utils.py` & `taskflow-5.2.0/taskflow/utils/eventlet_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/utils/iter_utils.py` & `taskflow-5.2.0/taskflow/utils/iter_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/utils/kazoo_utils.py` & `taskflow-5.2.0/taskflow/utils/kazoo_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,31 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from kazoo import client
 from kazoo import exceptions as k_exc
 from oslo_utils import reflection
+from oslo_utils import strutils
 
 from taskflow import exceptions as exc
 from taskflow import logging
 
 
 LOG = logging.getLogger(__name__)
 
+CONF_TRANSFERS = (
+    ('read_only', strutils.bool_from_string, False),
+    ('randomize_hosts', strutils.bool_from_string, False),
+    ('keyfile', None, None),
+    ('keyfile_password', None, None),
+    ('certfile', None, None),
+    ('use_ssl', strutils.bool_from_string, False),
+    ('verify_certs', strutils.bool_from_string, True))
+
 
 def _parse_hosts(hosts):
     if isinstance(hosts, str):
         return hosts.strip()
     if isinstance(hosts, (dict)):
         host_ports = []
         for (k, v) in hosts.items():
@@ -189,24 +199,27 @@
     .. _eventlet: https://kazoo.readthedocs.io/en/latest/api/\
                   handlers/eventlet.html
     .. _thread: https://kazoo.readthedocs.io/en/latest/api/\
                 handlers/threading.html
     """
     # See: https://kazoo.readthedocs.io/en/latest/api/client.html
     client_kwargs = {
-        'read_only': bool(conf.get('read_only')),
-        'randomize_hosts': bool(conf.get('randomize_hosts')),
         'logger': LOG,
-        'keyfile': conf.get('keyfile', None),
-        'keyfile_password': conf.get('keyfile_password', None),
-        'certfile': conf.get('certfile', None),
-        'use_ssl': conf.get('use_ssl', False),
-        'verify_certs': conf.get('verify_certs', True),
-
     }
+
+    for key, value_type_converter, default in CONF_TRANSFERS:
+        if key in conf:
+            if value_type_converter is not None:
+                client_kwargs[key] = value_type_converter(conf[key],
+                                                          default=default)
+            else:
+                client_kwargs[key] = conf[key]
+        else:
+            client_kwargs[key] = default
+
     # See: https://kazoo.readthedocs.io/en/latest/api/retry.html
     if 'command_retry' in conf:
         client_kwargs['command_retry'] = conf['command_retry']
     if 'connection_retry' in conf:
         client_kwargs['connection_retry'] = conf['connection_retry']
     hosts = _parse_hosts(conf.get("hosts", "localhost:2181"))
     if not hosts or not isinstance(hosts, str):
```

### Comparing `taskflow-5.1.0/taskflow/utils/kombu_utils.py` & `taskflow-5.2.0/taskflow/utils/kombu_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/utils/misc.py` & `taskflow-5.2.0/taskflow/utils/misc.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/utils/persistence_utils.py` & `taskflow-5.2.0/taskflow/utils/persistence_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/utils/redis_utils.py` & `taskflow-5.2.0/taskflow/utils/redis_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,32 +29,32 @@
             raise redis_exceptions.ConnectionError("Connection has been"
                                                    " closed")
         return meth(self, *args, **kwargs)
 
     return wrapper
 
 
-class RedisClient(redis.StrictRedis):
+class RedisClient(redis.Redis):
     """A redis client that can be closed (and raises on-usage after closed).
 
     TODO(harlowja): if https://github.com/andymccurdy/redis-py/issues/613 ever
     gets resolved or merged or other then we can likely remove this.
     """
 
     def __init__(self, *args, **kwargs):
         super(RedisClient, self).__init__(*args, **kwargs)
         self.closed = False
 
     def close(self):
         self.closed = True
         self.connection_pool.disconnect()
 
-    execute_command = _raise_on_closed(redis.StrictRedis.execute_command)
-    transaction = _raise_on_closed(redis.StrictRedis.transaction)
-    pubsub = _raise_on_closed(redis.StrictRedis.pubsub)
+    execute_command = _raise_on_closed(redis.Redis.execute_command)
+    transaction = _raise_on_closed(redis.Redis.transaction)
+    pubsub = _raise_on_closed(redis.Redis.pubsub)
 
 
 class UnknownExpire(enum.IntEnum):
     """Non-expiry (not ttls) results return from :func:`.get_expiry`.
 
     See: http://redis.io/commands/ttl or http://redis.io/commands/pttl
     """
```

### Comparing `taskflow-5.1.0/taskflow/utils/schema_utils.py` & `taskflow-5.2.0/taskflow/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/utils/threading_utils.py` & `taskflow-5.2.0/taskflow/utils/threading_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow/version.py` & `taskflow-5.2.0/taskflow/version.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow.egg-info/PKG-INFO` & `taskflow-5.2.0/taskflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskflow
-Version: 5.1.0
+Version: 5.2.0
 Summary: Taskflow structured state management library.
 Home-page: https://docs.openstack.org/taskflow/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -89,14 +89,15 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Provides-Extra: database
 Provides-Extra: eventlet
```

### Comparing `taskflow-5.1.0/taskflow.egg-info/SOURCES.txt` & `taskflow-5.2.0/taskflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,18 @@
 doc/source/user/img/tasks.png
 doc/source/user/img/wbe_request_states.svg
 doc/source/user/img/worker-engine.svg
 releasenotes/notes/.placeholder
 releasenotes/notes/add-sentinel-redis-support-9fd16e2a5dd5c0c9.yaml
 releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
 releasenotes/notes/fix-endless-loop-on-storage-error-dd4467f0bbc66abf.yaml
+releasenotes/notes/fix-zookeeper-option-parsing-f9d37fbc39af47f4.yaml
+releasenotes/notes/remove-strict-redis-f2a5a924b314de41.yaml
 releasenotes/notes/zookeeper-ssl-support-b9abf24a39096b62.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
@@ -257,14 +260,15 @@
 taskflow/tests/unit/test_suspend.py
 taskflow/tests/unit/test_task.py
 taskflow/tests/unit/test_types.py
 taskflow/tests/unit/test_utils.py
 taskflow/tests/unit/test_utils_async_utils.py
 taskflow/tests/unit/test_utils_binary.py
 taskflow/tests/unit/test_utils_iter_utils.py
+taskflow/tests/unit/test_utils_kazoo_utils.py
 taskflow/tests/unit/test_utils_threading_utils.py
 taskflow/tests/unit/action_engine/__init__.py
 taskflow/tests/unit/action_engine/test_builder.py
 taskflow/tests/unit/action_engine/test_compile.py
 taskflow/tests/unit/action_engine/test_creation.py
 taskflow/tests/unit/action_engine/test_process_executor.py
 taskflow/tests/unit/action_engine/test_scoping.py
```

### Comparing `taskflow-5.1.0/taskflow.egg-info/entry_points.txt` & `taskflow-5.2.0/taskflow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/taskflow.egg-info/requires.txt` & `taskflow-5.2.0/taskflow.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/test-requirements.txt` & `taskflow-5.2.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/tools/env_builder.sh` & `taskflow-5.2.0/tools/env_builder.sh`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/tools/schema_generator.py` & `taskflow-5.2.0/tools/schema_generator.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/tools/speed_test.py` & `taskflow-5.2.0/tools/speed_test.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/tools/state_graph.py` & `taskflow-5.2.0/tools/state_graph.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/tools/subunit_trace.py` & `taskflow-5.2.0/tools/subunit_trace.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/tools/test-setup.sh` & `taskflow-5.2.0/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/tools/update_states.sh` & `taskflow-5.2.0/tools/update_states.sh`

 * *Files identical despite different names*

### Comparing `taskflow-5.1.0/tox.ini` & `taskflow-5.2.0/tox.ini`

 * *Files identical despite different names*

