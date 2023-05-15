# Comparing `tmp/pyunifiprotect-4.8.3.tar.gz` & `tmp/pyunifiprotect-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunifiprotect-4.8.3.tar", last modified: Sat Apr 29 16:01:30 2023, max compression
+gzip compressed data, was "pyunifiprotect-4.9.0.tar", last modified: Mon May 15 01:00:11 2023, max compression
```

## Comparing `pyunifiprotect-4.8.3.tar` & `pyunifiprotect-4.9.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.774006 pyunifiprotect-4.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/format-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/install-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.bin/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/lib/common.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/lint-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/test-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/update-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.docker/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.758006 pyunifiprotect-4.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/test-live-AngellusMortis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/LIVE_DATA_CI.md
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-29 16:01:30.774006 pyunifiprotect-4.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/TESTDATA.md
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/docs/overrides/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/overrides/partials/toc-item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/pyunifiprotect/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47822 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.766006 pyunifiprotect-4.8.3/pyunifiprotect/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/chimes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/doorlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/lights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/liveviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.766006 pyunifiprotect-4.8.3/pyunifiprotect/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35653 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    73235 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    33721 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/release_cache.json
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.766006 pyunifiprotect-4.8.3/pyunifiprotect/test_util/
--rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/test_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/test_util/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.766006 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 16:01:30.774006 pyunifiprotect-4.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.770006 pyunifiprotect-4.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.770006 pyunifiprotect-4.8.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_chime.py
--rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_doorlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_light.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.774006 pyunifiprotect-4.8.3/tests/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_bootstrap.json
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera_heatmap.png
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera_snapshot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera_thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera_video.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_chime.json
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_constants.json
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_doorlock.json
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_event_smart_track.json
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_light.json
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_liveview.json
--rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_raw_events.json
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_viewport.json
--rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_ws_messages.json
--rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/test_api_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/test_api_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.394236 pyunifiprotect-4.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/format-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/install-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.bin/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/lib/common.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/lint-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/test-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.bin/update-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.378235 pyunifiprotect-4.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.github/workflows/test-live-AngellusMortis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/LIVE_DATA_CI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-15 01:00:11.394236 pyunifiprotect-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/TESTDATA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/docs/overrides/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/docs/overrides/partials/toc-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/pyunifiprotect/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47861 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.386236 pyunifiprotect-4.9.0/pyunifiprotect/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/chimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/doorlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/liveviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/cli/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.386236 pyunifiprotect-4.9.0/pyunifiprotect/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73524 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33878 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/data/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/release_cache.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.386236 pyunifiprotect-4.9.0/pyunifiprotect/test_util/
+-rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/test_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/test_util/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/pyunifiprotect/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.382236 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 01:00:11.000000 pyunifiprotect-4.9.0/pyunifiprotect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 01:00:11.394236 pyunifiprotect-4.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.386236 pyunifiprotect-4.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.390236 pyunifiprotect-4.9.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_chime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_doorlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/data/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:00:11.390236 pyunifiprotect-4.9.0/tests/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_bootstrap.json
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera_heatmap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera_snapshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera_thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_camera_video.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_chime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_constants.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_doorlock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_event_smart_track.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_light.json
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_liveview.json
+-rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_raw_events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_viewport.json
+-rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/sample_data/sample_ws_messages.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/test_api_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/test_api_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-15 00:59:57.000000 pyunifiprotect-4.9.0/tests/test_utils.py
```

### Comparing `pyunifiprotect-4.8.3/.bin/lib/common.sh` & `pyunifiprotect-4.9.0/.bin/lib/common.sh`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.bin/lint-code` & `pyunifiprotect-4.9.0/.bin/lint-code`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.bin/update-requirements` & `pyunifiprotect-4.9.0/.bin/update-requirements`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.devcontainer/devcontainer.json` & `pyunifiprotect-4.9.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.github/workflows/ci.yaml` & `pyunifiprotect-4.9.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.github/workflows/docker.yml` & `pyunifiprotect-4.9.0/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.github/workflows/docs.yml` & `pyunifiprotect-4.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.github/workflows/pypi.yml` & `pyunifiprotect-4.9.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.github/workflows/test-live-AngellusMortis.yml` & `pyunifiprotect-4.9.0/.github/workflows/test-live-AngellusMortis.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.gitignore` & `pyunifiprotect-4.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.vscode/launch.json` & `pyunifiprotect-4.9.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/.vscode/tasks.json` & `pyunifiprotect-4.9.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/Dockerfile` & `pyunifiprotect-4.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/LICENSE` & `pyunifiprotect-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/LIVE_DATA_CI.md` & `pyunifiprotect-4.9.0/LIVE_DATA_CI.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/PKG-INFO` & `pyunifiprotect-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.8.3
+Version: 4.9.0
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.8.3/README.md` & `pyunifiprotect-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/TESTDATA.md` & `pyunifiprotect-4.9.0/TESTDATA.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/dev-requirements.txt` & `pyunifiprotect-4.9.0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/docs/api.md` & `pyunifiprotect-4.9.0/docs/api.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/docs/cli.md` & `pyunifiprotect-4.9.0/docs/cli.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/docs/dev.md` & `pyunifiprotect-4.9.0/docs/dev.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/mkdocs.yml` & `pyunifiprotect-4.9.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyproject.toml` & `pyunifiprotect-4.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/api.py` & `pyunifiprotect-4.9.0/pyunifiprotect/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """UniFi Protect Server Wrapper."""
 from __future__ import annotations
 
 import asyncio
 from datetime import datetime, timedelta
 from http.cookies import Morsel
-from ipaddress import IPv4Address
+from ipaddress import IPv4Address, IPv6Address
 import logging
 from pathlib import Path
 from tempfile import gettempdir
 import time
 from typing import Any, Callable, Dict, List, Optional, Set, Type, Union, cast
 from urllib.parse import urljoin
 from uuid import UUID
@@ -499,15 +499,15 @@
 
     _minimum_score: int
     _subscribed_models: Set[ModelType]
     _ignore_stats: bool
     _ws_subscriptions: List[Callable[[WSSubscriptionMessage], None]]
     _bootstrap: Optional[Bootstrap] = None
     _last_update_dt: Optional[datetime] = None
-    _connection_host: Optional[Union[IPv4Address, str]] = None
+    _connection_host: Optional[Union[IPv4Address, IPv6Address, str]] = None
 
     cache_dir: Path
     ignore_unadopted: bool
 
     def __init__(
         self,
         host: str,
@@ -554,15 +554,15 @@
     def bootstrap(self) -> Bootstrap:
         if self._bootstrap is None:
             raise BadRequest("Client not initalized, run `update` first")
 
         return self._bootstrap
 
     @property
-    def connection_host(self) -> Union[IPv4Address, str]:
+    def connection_host(self) -> Union[IPv4Address, IPv6Address, str]:
         """Connection host to use for generating RTSP URLs"""
 
         if self._connection_host is None:
             # fallback if cannot find user supplied host
             index = 0
             try:
                 # check if user supplied host is avaiable
```

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/__init__.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/backup.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/backup.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/base.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/cameras.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/cameras.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/chimes.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/chimes.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/doorlocks.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/doorlocks.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/events.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/events.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/lights.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/lights.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/liveviews.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/liveviews.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/nvr.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/sensors.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/sensors.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/cli/viewers.py` & `pyunifiprotect-4.9.0/pyunifiprotect/cli/viewers.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/data/__init__.py` & `pyunifiprotect-4.9.0/pyunifiprotect/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/data/base.py` & `pyunifiprotect-4.9.0/pyunifiprotect/data/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     List,
     Optional,
     Set,
     Type,
     TypeVar,
     Union,
 )
+from uuid import UUID
 
-from async_timeout import timeout
 from pydantic import BaseModel
 from pydantic.fields import SHAPE_DICT, SHAPE_LIST, PrivateAttr
 
 from pyunifiprotect.data.types import (
     ModelType,
     PercentFloat,
     PermissionNode,
@@ -34,14 +34,15 @@
 from pyunifiprotect.data.websocket import (
     WSJSONPacketFrame,
     WSPacket,
     WSPacketFrameHeader,
 )
 from pyunifiprotect.exceptions import BadRequest, ClientError, NotAuthorized
 from pyunifiprotect.utils import (
+    asyncio_timeout,
     convert_unifi_data,
     dict_diff,
     is_debug,
     process_datetime,
     serialize_unifi_obj,
     to_snake_case,
 )
@@ -616,15 +617,15 @@
         self._update_queue.put_nowait(callback)
 
         self._update_event.set()
         await asyncio.sleep(0.001)  # release execution so other `queue_update` calls can abort
         self._update_event.clear()
 
         try:
-            async with timeout(0.05):
+            async with asyncio_timeout(0.05):
                 await self._update_event.wait()
             self._update_event.clear()
             return
         except asyncio.TimeoutError:
             async with self._update_lock:
                 # Important! Now that we have the lock, we yield to the event loop so any
                 # updates from the websocket are processed before we generate the diff
@@ -838,14 +839,16 @@
     is_connected: bool
     # requires 1.21+
     market_name: Optional[str]
     # requires 2.7.5+
     fw_update_state: Optional[str] = None
     # requires 2.8.14+
     nvr_mac: Optional[str] = None
+    # requires 2.8.22+
+    guid: Optional[UUID] = None
 
     wired_connection_state: Optional[WiredConnectionState] = None
     wifi_connection_state: Optional[WifiConnectionState] = None
     bluetooth_connection_state: Optional[BluetoothConnectionState] = None
     bridge_id: Optional[str]
     is_downloading_firmware: Optional[bool]
```

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/data/bootstrap.py` & `pyunifiprotect-4.9.0/pyunifiprotect/data/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/data/convert.py` & `pyunifiprotect-4.9.0/pyunifiprotect/data/convert.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/data/devices.py` & `pyunifiprotect-4.9.0/pyunifiprotect/data/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,14 +399,16 @@
 
         return data
 
 
 class SmartDetectSettings(ProtectBaseObject):
     object_types: List[SmartDetectObjectType]
     audio_types: Optional[List[SmartDetectAudioType]] = None
+    # requires 2.8.22+
+    auto_tracking_object_types: Optional[List[SmartDetectObjectType]] = None
 
     @classmethod
     def unifi_dict_to_dict(cls, data: Dict[str, Any]) -> Dict[str, Any]:
         if "objectTypes" in data:
             data["objectTypes"] = convert_smart_types(data.pop("objectTypes"))
         if "audioTypes" in data:
             data["audioTypes"] = convert_smart_audio_types(data.pop("audioTypes"))
@@ -694,14 +696,16 @@
     mount_positions: List[MountPosition] = []
     has_infrared: Optional[bool] = None
     lens_type: Optional[LensType] = None
     hotplug: Optional[Hotplug] = None
     smart_detect_audio_types: Optional[List[SmartDetectAudioType]] = None
     # 2.7.18+
     is_doorbell: bool
+    # 2.8.22+
+    lens_model: Optional[str] = None
 
     # TODO:
     # focus
     # pan
     # tilt
     # zoom
 
@@ -798,14 +802,16 @@
     # requires 2.7.5+
     is_waterproof_case_attached: Optional[bool] = None
     last_disconnect: Optional[datetime] = None
     # requires 2.8.14+
     is_2k: Optional[bool] = None
     is_4k: Optional[bool] = None
     use_global: Optional[bool] = None
+    # requires 2.8.22+
+    user_configured_ap: Optional[bool] = None
 
     # TODO: used for adopting
     # apMac read only
     # apRssi read only
     # elementInfo read only
 
     # TODO:
@@ -2129,14 +2135,16 @@
     last_ring: Optional[datetime]
     is_wireless_uplink_enabled: bool
     camera_ids: List[str]
     # requires 2.6.17+
     ap_mgmt_ip: Optional[IPv4Address] = None
     # requires 2.7.15+
     feature_flags: Optional[ChimeFeatureFlags] = None
+    # requires 2.8.22+
+    user_configured_ap: Optional[bool] = None
 
     # TODO: used for adoption
     # apMac  read only
     # apRssi  read only
     # elementInfo  read only
 
     @classmethod
```

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/data/nvr.py` & `pyunifiprotect-4.9.0/pyunifiprotect/data/nvr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """UniFi Protect Data."""
 from __future__ import annotations
 
 import asyncio
 from datetime import datetime, timedelta, tzinfo
 from functools import cache
-from ipaddress import IPv4Address
+from ipaddress import IPv4Address, IPv6Address
 import logging
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Dict,
@@ -187,15 +187,15 @@
         # all metadata keys optionally appear
         for key, value in list(data.items()):
             if value is None:
                 del data[key]
 
         for key in self._collapse_keys.intersection(data.keys()):
             # AI Theta/Hotplug exception
-            if key != "type" or data[key] not in ("audio", "video"):
+            if key != "type" or data[key] not in ("audio", "video", "extender"):
                 data[key] = {"text": data[key]}
 
         return data
 
 
 class Event(ProtectModelWithId):
     type: EventType
@@ -563,22 +563,25 @@
     total_bytes: int
     used_bytes: int
     action: str
     progress: Optional[PercentFloat] = None
     estimate: Optional[timedelta] = None
     # requires 2.8.14+
     health: Optional[str] = None
+    # requires 2.8.22+
+    space_type: Optional[str] = None
 
     @classmethod
     @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "total_bytes": "totalBytes",
             "used_bytes": "usedBytes",
+            "space_type": "spaceType",
         }
 
     @classmethod
     def unifi_dict_to_dict(cls, data: Dict[str, Any]) -> Dict[str, Any]:
         if "estimate" in data and data["estimate"] is not None:
             data["estimate"] = timedelta(seconds=data.pop("estimate"))
 
@@ -740,15 +743,15 @@
     hardware_platform: str
     ports: PortConfig
     last_update_at: Optional[datetime]
     is_station: bool
     enable_automatic_backups: bool
     enable_stats_reporting: bool
     release_channel: FirmwareReleaseChannel
-    hosts: List[Union[IPv4Address, str]]
+    hosts: List[Union[IPv4Address, IPv6Address, str]]
     enable_bridge_auto_adoption: bool
     hardware_id: UUID
     host_type: int
     host_shortname: str
     is_hardware: bool
     is_wireless_uplink_enabled: bool
     time_format: Literal["12h", "24h"]
@@ -788,15 +791,15 @@
     # requires 2.8.14+
     corruption_state: Optional[str] = None
     country_code: Optional[str] = None
     has_gateway: Optional[bool] = None
     is_vault_registered: Optional[bool] = None
     public_ip: Optional[IPv4Address] = None
     ulp_version: Optional[str] = None
-    wan_ip: Optional[IPv4Address] = None
+    wan_ip: Optional[Union[IPv4Address, IPv6Address]] = None
 
     # TODO:
     # errorCode   read only
     # wifiSettings
     # smartDetectAgreement
     # dbRecoveryOptions
     # globalCameraSettings
```

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/data/types.py` & `pyunifiprotect-4.9.0/pyunifiprotect/data/types.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/data/user.py` & `pyunifiprotect-4.9.0/pyunifiprotect/data/user.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/data/websocket.py` & `pyunifiprotect-4.9.0/pyunifiprotect/data/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/exceptions.py` & `pyunifiprotect-4.9.0/pyunifiprotect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/stream.py` & `pyunifiprotect-4.9.0/pyunifiprotect/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,18 @@
         if not self.is_started:
             await self.start()
 
         if self.process is None:
             raise StreamError("Could not start stream")
 
         await asyncio.wait(
-            [self._read_stream(self.process.stdout, "stdout"), self._read_stream(self.process.stderr, "stderr")]
+            [
+                asyncio.create_task(self._read_stream(self.process.stdout, "stdout")),
+                asyncio.create_task(self._read_stream(self.process.stderr, "stderr")),
+            ]
         )
         await self.process.wait()
 
 
 class TalkbackStream(FfmpegCommand):
     camera: Camera
     content_url: str
```

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/test_util/__init__.py` & `pyunifiprotect-4.9.0/pyunifiprotect/test_util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/test_util/anonymize.py` & `pyunifiprotect-4.9.0/pyunifiprotect/test_util/anonymize.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/utils.py` & `pyunifiprotect-4.9.0/pyunifiprotect/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from datetime import datetime, timedelta, timezone, tzinfo
 from decimal import Decimal
 from enum import Enum
 from functools import lru_cache
 from hashlib import sha224
 from http.cookies import Morsel
 from inspect import isclass
-from ipaddress import AddressValueError, IPv4Address
+from ipaddress import IPv4Address, IPv6Address, ip_address
 import json
 import logging
 import math
 import os
 from pathlib import Path
 import re
 import socket
+import sys
 import time
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Coroutine,
     Dict,
@@ -57,25 +58,46 @@
 DEBUG_ENV = "UFP_DEBUG"
 PROGRESS_CALLABLE = Callable[[int, str], Coroutine[Any, Any, None]]
 SNAKE_CASE_KEYS = [
     "life_span",
     "bad_sector",
     "total_bytes",
     "used_bytes",
+    "space_type",
 ]
 TIMEZONE_GLOBAL: tzinfo | None = None
 
 SNAKE_CASE_MATCH_1 = re.compile("(.)([A-Z0-9][a-z]+)")
 SNAKE_CASE_MATCH_2 = re.compile("__([A-Z0-9])")
 SNAKE_CASE_MATCH_3 = re.compile("([a-z0-9])([A-Z])")
 
 _LOGGER = logging.getLogger(__name__)
 
 RELEASE_CACHE = Path(__file__).parent / "release_cache.json"
 
+IP_TYPES = (
+    Union[IPv4Address, str, None],
+    Union[IPv4Address, str],
+    Union[IPv6Address, str, None],
+    Union[IPv6Address, str],
+    Union[IPv6Address, IPv4Address, str, None],
+    Union[IPv6Address, IPv4Address, str],
+    Union[IPv6Address, IPv4Address],
+    Union[IPv6Address, IPv4Address, None],
+)
+
+if sys.version_info[:2] < (3, 11):
+    from async_timeout import (  # pylint: disable=unused-import # noqa: F401
+        timeout as asyncio_timeout,
+    )
+else:
+    from asyncio import (  # pylint: disable=unused-import # noqa: F401
+        timeout as asyncio_timeout,
+    )
+
 
 def set_debug() -> None:
     """Sets ENV variable for UFP_DEBUG to on (True)"""
     os.environ[DEBUG_ENV] = str(True)
 
 
 def set_no_debug() -> None:
@@ -185,27 +207,29 @@
 
     if field.shape == SHAPE_LIST and isinstance(value, list):
         value = [convert_unifi_data(v, field) for v in value]
     elif field.shape == SHAPE_SET and isinstance(value, list):
         value = {convert_unifi_data(v, field) for v in value}
     elif field.shape == SHAPE_DICT and isinstance(value, dict):
         value = {k: convert_unifi_data(v, field) for k, v in value.items()}
-    elif field.type_ in (Union[IPv4Address, str, None], Union[IPv4Address, str]) and value is not None:
+    elif field.type_ in IP_TYPES and value is not None:
         try:
-            value = IPv4Address(value)
-        except AddressValueError:
+            value = ip_address(value)
+        except ValueError:
             pass
     elif (
         value is None
         or not isclass(field.type_)
         or issubclass(field.type_, ProtectBaseObject)
         or isinstance(value, field.type_)
     ):
         return value
-    elif field.type_ in (IPv4Address, UUID, Color, Decimal, Path, Version) or issubclass(field.type_, Enum):
+    elif field.type_ in (IPv6Address, IPv4Address, UUID, Color, Decimal, Path, Version) or issubclass(
+        field.type_, Enum
+    ):
         value = field.type_(value)
     elif field.type_ == datetime:
         value = from_js_time(value)
 
     return value
 
 
@@ -220,15 +244,15 @@
         value = value.unifi_dict()
     if isinstance(value, dict):
         value = serialize_dict(value)
     elif isinstance(value, Iterable) and not isinstance(value, str):
         value = serialize_list(value)
     elif isinstance(value, Enum):
         value = value.value
-    elif isinstance(value, (IPv4Address, UUID, Path, tzinfo, Version)):
+    elif isinstance(value, (IPv4Address, IPv6Address, UUID, Path, tzinfo, Version)):
         value = str(value)
     elif isinstance(value, datetime):
         value = to_js_time(value)
     elif isinstance(value, timedelta):
         value = to_ms(value)
     elif isinstance(value, Color):
         value = value.as_hex().upper()
@@ -308,21 +332,21 @@
         try:
             types.append(VideoMode(video_mode))
         except ValueError:
             _LOGGER.warning("Unknown video mode: %s", video_mode)
     return types
 
 
-def ip_from_host(host: str) -> IPv4Address:
+def ip_from_host(host: str) -> IPv4Address | IPv6Address:
     try:
-        return IPv4Address(host)
-    except AddressValueError:
+        return ip_address(host)
+    except ValueError:
         pass
 
-    return IPv4Address(socket.gethostbyname(host))
+    return ip_address(socket.gethostbyname(host))
 
 
 def dict_diff(orig: Optional[Dict[str, Any]], new: Dict[str, Any]) -> Dict[str, Any]:
     changed: Dict[str, Any] = {}
 
     if orig is None:
         return new
```

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect/websocket.py` & `pyunifiprotect-4.9.0/pyunifiprotect/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     ClientError,
     ClientSession,
     ClientWebSocketResponse,
     WSMessage,
     WSMsgType,
 )
 
+from .utils import asyncio_timeout
+
 _LOGGER = logging.getLogger(__name__)
 CALLBACK_TYPE = Callable[..., Coroutine[Any, Any, Optional[Dict[str, str]]]]
 RECENT_FAILURE_CUT_OFF = 30
 
 
 class Websocket:
     url: str
@@ -150,24 +152,26 @@
     async def connect(self) -> bool:
         """Connect the websocket."""
 
         if self._connect_lock.locked():
             _LOGGER.debug("Another connect is already happening")
             return False
         try:
-            await asyncio.wait_for(self._connect_lock.acquire(), timeout=0.1)
+            async with asyncio_timeout(0.1):
+                await self._connect_lock.acquire()
         except asyncio.TimeoutError:
             _LOGGER.debug("Failed to get connection lock")
 
         start_event = asyncio.Event()
         _LOGGER.debug("Scheduling WS connect...")
         self._websocket_loop_task = asyncio.create_task(self._websocket_loop(start_event))
 
         try:
-            await asyncio.wait_for(start_event.wait(), timeout=self.timeout_interval)
+            async with asyncio_timeout(self.timeout_interval):
+                await start_event.wait()
         except asyncio.TimeoutError:
             _LOGGER.warning("Timed out while waiting for Websocket to connect")
             await self.disconnect()
 
         self._connect_lock.release()
         if self._ws_connection is None:
             _LOGGER.debug("Failed to connect to Websocket")
```

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect.egg-info/PKG-INFO` & `pyunifiprotect-4.9.0/pyunifiprotect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.8.3
+Version: 4.9.0
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect.egg-info/SOURCES.txt` & `pyunifiprotect-4.9.0/pyunifiprotect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/pyunifiprotect.egg-info/requires.txt` & `pyunifiprotect-4.9.0/pyunifiprotect.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/requirements.txt` & `pyunifiprotect-4.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/conftest.py` & `pyunifiprotect-4.9.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -530,25 +530,30 @@
     "ulpVersion",
     "wanIp",
     "publicIp",
     "isVaultRegistered",
     "hasGateway",
     "corruptionState",
     "countryCode",
+    # 2.8.22+
+    "guid",
+    "userConfiguredAp",
 }
 
 NEW_CAMERA_FEATURE_FLAGS = {
     "audio",
     "audioCodecs",
     "hasInfrared",
     "hotplug",
     "smartDetectAudioTypes",
     "lensType",
     # 2.7.18+
     "isDoorbell",
+    # 2.8.22+
+    "lensModel",
 }
 
 NEW_NVR_FEATURE_FLAGS = {
     # 2.8.14+
     "ulpRoleManagement",
 }
 
@@ -596,14 +601,19 @@
             expected["eventStats"]["motion"].pop("recentHours", None)
             actual["eventStats"]["motion"].pop("recentHours", None)
         if expected["eventStats"]["smart"].get("recentHours") == [[None], None, []]:
             expected["eventStats"]["smart"].pop("recentHours", None)
             actual["eventStats"]["smart"].pop("recentHours", None)
         if "audioTypes" in actual["smartDetectSettings"] and "audioTypes" not in expected["smartDetectSettings"]:
             del actual["smartDetectSettings"]["audioTypes"]
+        if (
+            "autoTrackingObjectTypes" in actual["smartDetectSettings"]
+            and "autoTrackingObjectTypes" not in expected["smartDetectSettings"]
+        ):
+            del actual["smartDetectSettings"]["autoTrackingObjectTypes"]
 
         for flag in NEW_CAMERA_FEATURE_FLAGS:
             if flag not in expected["featureFlags"]:
                 del actual["featureFlags"][flag]
 
         # ignore changes to motion for live tests
         assert type(actual["isMotionDetected"]) == bool
@@ -674,14 +684,16 @@
             for index, device in enumerate(expected["systemInfo"]["ustorage"]["space"]):
                 actual_device = actual["systemInfo"]["ustorage"]["space"][index]
                 estimate = device.get("estimate")
                 actual_estimate = actual_device.get("estimate")
                 if estimate is not None and actual_estimate is not None:
                     if math.isclose(estimate, actual_estimate, rel_tol=0.01):
                         actual["systemInfo"]["ustorage"]["space"][index]["estimate"] = estimate
+                if "space_type" not in device:
+                    del actual_device["space_type"]
 
         for flag in NEW_NVR_FEATURE_FLAGS:
             if flag not in expected["featureFlags"]:
                 del actual["featureFlags"][flag]
 
     if "bluetoothConnectionState" in expected:
         expected["bluetoothConnectionState"]["experienceScore"] = expected["bluetoothConnectionState"].get(
```

### Comparing `pyunifiprotect-4.8.3/tests/data/test_camera.py` & `pyunifiprotect-4.9.0/tests/data/test_camera.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/data/test_chime.py` & `pyunifiprotect-4.9.0/tests/data/test_chime.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/data/test_common.py` & `pyunifiprotect-4.9.0/tests/data/test_common.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/data/test_doorlock.py` & `pyunifiprotect-4.9.0/tests/data/test_doorlock.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/data/test_light.py` & `pyunifiprotect-4.9.0/tests/data/test_light.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/data/test_nvr.py` & `pyunifiprotect-4.9.0/tests/data/test_nvr.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # type: ignore
 # pylint: disable=protected-access
 
+from __future__ import annotations
+
 from datetime import timedelta
+from ipaddress import IPv4Address, IPv6Address
 
 from pydantic.error_wrappers import ValidationError
 import pytest
 
 from pyunifiprotect.data import (
     NVR,
     AnalyticsOption,
@@ -145,7 +148,24 @@
                 text=DoorbellMessageType.LEAVE_PACKAGE_AT_DOOR.value.replace("_", " "),
             ),
             DoorbellMessage(
                 type=DoorbellMessageType.DO_NOT_DISTURB,
                 text=DoorbellMessageType.DO_NOT_DISTURB.value.replace("_", " "),
             ),
         ]
+
+
+@pytest.mark.parametrize(
+    "ip,expected",
+    [
+        ("192.168.1.1", IPv4Address("192.168.1.1")),
+        ("fe80::1ff:fe23:4567:890a", IPv6Address("fe80::1ff:fe23:4567:890a")),
+    ],
+)
+@pytest.mark.asyncio
+async def test_nvr_wan_ip(nvr_obj: NVR, ip: str, expected: IPv4Address | IPv6Address):
+    nvr_dict = nvr_obj.unifi_dict()
+    nvr_dict["wanIp"] = ip
+
+    nvr = NVR.from_unifi_dict(**nvr_dict)
+    assert nvr.wan_ip == expected
+    assert nvr.unifi_dict()["wanIp"] == ip
```

### Comparing `pyunifiprotect-4.8.3/tests/data/test_sensor.py` & `pyunifiprotect-4.9.0/tests/data/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/data/test_viewer.py` & `pyunifiprotect-4.9.0/tests/data/test_viewer.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/constants.py` & `pyunifiprotect-4.9.0/tests/sample_data/constants.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_bootstrap.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_bootstrap.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_bridge.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_bridge.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_camera.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_camera.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_camera_heatmap.png` & `pyunifiprotect-4.9.0/tests/sample_data/sample_camera_heatmap.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_camera_snapshot.png` & `pyunifiprotect-4.9.0/tests/sample_data/sample_camera_snapshot.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_camera_thumbnail.png` & `pyunifiprotect-4.9.0/tests/sample_data/sample_camera_thumbnail.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_camera_video.mp4` & `pyunifiprotect-4.9.0/tests/sample_data/sample_camera_video.mp4`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_chime.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_chime.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_constants.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_constants.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_doorlock.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_doorlock.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_event_smart_track.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_event_smart_track.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_light.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_light.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_liveview.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_liveview.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_raw_events.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_raw_events.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_sensor.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_sensor.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_viewport.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_viewport.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/sample_data/sample_ws_messages.json` & `pyunifiprotect-4.9.0/tests/sample_data/sample_ws_messages.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/test_api.py` & `pyunifiprotect-4.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/test_api_polling.py` & `pyunifiprotect-4.9.0/tests/test_api_polling.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/test_api_ws.py` & `pyunifiprotect-4.9.0/tests/test_api_ws.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.3/tests/test_utils.py` & `pyunifiprotect-4.9.0/tests/test_utils.py`

 * *Files identical despite different names*

