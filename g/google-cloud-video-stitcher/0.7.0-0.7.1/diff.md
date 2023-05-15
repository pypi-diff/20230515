# Comparing `tmp/google-cloud-video-stitcher-0.7.0.tar.gz` & `tmp/google-cloud-video-stitcher-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-video-stitcher-0.7.0.tar", last modified: Mon Mar 27 14:04:51 2023, max compression
+gzip compressed data, was "google-cloud-video-stitcher-0.7.1.tar", last modified: Mon May 15 19:00:23 2023, max compression
```

## Comparing `google-cloud-video-stitcher-0.7.0.tar` & `google-cloud-video-stitcher-0.7.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.919667 google-cloud-video-stitcher-0.7.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4771 2023-03-27 14:04:51.919667 google-cloud-video-stitcher-0.7.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3847 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.907666 google-cloud-video-stitcher-0.7.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.907666 google-cloud-video-stitcher-0.7.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.907666 google-cloud-video-stitcher-0.7.0/google/cloud/video/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.911666 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher/
--rw-rw-r--   0 root         (0)     1003     4629 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.911666 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/
--rw-rw-r--   0 root         (0)     1003     4178 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6599 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.911666 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.915667 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/
--rw-rw-r--   0 root         (0)     1003      793 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   134964 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   152140 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py
--rw-rw-r--   0 root         (0)     1003    32467 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.915667 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/
--rw-rw-r--   0 root         (0)     1003     1255 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    18084 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43836 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    44712 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   110180 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.919667 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/
--rw-rw-r--   0 root         (0)     1003     3812 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4835 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/ad_tag_details.py
--rw-rw-r--   0 root         (0)     1003     4222 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/cdn_keys.py
--rw-rw-r--   0 root         (0)     1003     6930 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/companions.py
--rw-rw-r--   0 root         (0)     1003     5153 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/events.py
--rw-rw-r--   0 root         (0)     1003     7784 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/live_configs.py
--rw-rw-r--   0 root         (0)     1003    15092 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/sessions.py
--rw-rw-r--   0 root         (0)     1003     2314 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/slates.py
--rw-rw-r--   0 root         (0)     1003     3049 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/stitch_details.py
--rw-rw-r--   0 root         (0)     1003    26456 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/video_stitcher_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.919667 google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/
--rw-r--r--   0 root         (0)     1003     4771 2023-03-27 14:04:51.000000 google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2180 2023-03-27 14:04:51.000000 google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:04:51.000000 google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       39 2023-03-27 14:04:51.000000 google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:04:51.000000 google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:04:51.000000 google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:04:51.000000 google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:04:51.919667 google-cloud-video-stitcher-0.7.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2977 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.919667 google-cloud-video-stitcher-0.7.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.919667 google-cloud-video-stitcher-0.7.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.919667 google-cloud-video-stitcher-0.7.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:04:51.919667 google-cloud-video-stitcher-0.7.0/tests/unit/gapic/stitcher_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/tests/unit/gapic/stitcher_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   336343 2023-03-27 14:01:56.000000 google-cloud-video-stitcher-0.7.0/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.614704 google-cloud-video-stitcher-0.7.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4771 2023-05-15 19:00:23.614704 google-cloud-video-stitcher-0.7.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3847 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.602698 google-cloud-video-stitcher-0.7.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.602698 google-cloud-video-stitcher-0.7.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.602698 google-cloud-video-stitcher-0.7.1/google/cloud/video/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.606700 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher/
+-rw-rw-r--   0 root         (0)     1003     4591 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.606700 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/
+-rw-rw-r--   0 root         (0)     1003     4140 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6599 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.606700 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.610702 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/
+-rw-rw-r--   0 root         (0)     1003      793 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   134907 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   152083 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py
+-rw-rw-r--   0 root         (0)     1003    32467 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.610702 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1255 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18084 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43836 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    44712 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   110180 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.610702 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3774 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4835 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/ad_tag_details.py
+-rw-rw-r--   0 root         (0)     1003     4222 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/cdn_keys.py
+-rw-rw-r--   0 root         (0)     1003     6930 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/companions.py
+-rw-rw-r--   0 root         (0)     1003     5153 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/events.py
+-rw-rw-r--   0 root         (0)     1003     7320 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/live_configs.py
+-rw-rw-r--   0 root         (0)     1003    13278 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/sessions.py
+-rw-rw-r--   0 root         (0)     1003     2314 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/slates.py
+-rw-rw-r--   0 root         (0)     1003     3049 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/stitch_details.py
+-rw-rw-r--   0 root         (0)     1003    26456 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/video_stitcher_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.614704 google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/
+-rw-r--r--   0 root         (0)     1003     4771 2023-05-15 19:00:23.000000 google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2180 2023-05-15 19:00:23.000000 google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-15 19:00:23.000000 google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       39 2023-05-15 19:00:23.000000 google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-15 19:00:23.000000 google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-05-15 19:00:23.000000 google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-15 19:00:23.000000 google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-15 19:00:23.614704 google-cloud-video-stitcher-0.7.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2977 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.614704 google-cloud-video-stitcher-0.7.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.614704 google-cloud-video-stitcher-0.7.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.614704 google-cloud-video-stitcher-0.7.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-15 19:00:23.614704 google-cloud-video-stitcher-0.7.1/tests/unit/gapic/stitcher_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/tests/unit/gapic/stitcher_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   336343 2023-05-15 18:57:43.000000 google-cloud-video-stitcher-0.7.1/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py
```

### Comparing `google-cloud-video-stitcher-0.7.0/LICENSE` & `google-cloud-video-stitcher-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/MANIFEST.in` & `google-cloud-video-stitcher-0.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/PKG-INFO` & `google-cloud-video-stitcher-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-stitcher
-Version: 0.7.0
+Version: 0.7.1
 Summary: Google Cloud Video Stitcher API client library
 Home-page: https://github.com/googleapis/python-video-stitcher
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-video-stitcher-0.7.0/README.rst` & `google-cloud-video-stitcher-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher/__init__.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 from google.cloud.video.stitcher_v1.types.live_configs import (
     AdTracking,
     GamLiveConfig,
     LiveConfig,
     PrefetchConfig,
 )
 from google.cloud.video.stitcher_v1.types.sessions import (
-    GamVodConfig,
     Interstitials,
     LiveSession,
     ManifestOptions,
     RenditionFilter,
     VodSession,
     VodSessionAd,
     VodSessionAdBreak,
@@ -120,15 +119,14 @@
     "StaticAdResource",
     "Event",
     "ProgressEvent",
     "GamLiveConfig",
     "LiveConfig",
     "PrefetchConfig",
     "AdTracking",
-    "GamVodConfig",
     "Interstitials",
     "LiveSession",
     "ManifestOptions",
     "RenditionFilter",
     "VodSession",
     "VodSessionAd",
     "VodSessionAdBreak",
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher/gapic_version.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.7.0"  # {x-release-please-version}
+__version__ = "0.7.1"  # {x-release-please-version}
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/__init__.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     HtmlAdResource,
     IframeAdResource,
     StaticAdResource,
 )
 from .types.events import Event, ProgressEvent
 from .types.live_configs import AdTracking, GamLiveConfig, LiveConfig, PrefetchConfig
 from .types.sessions import (
-    GamVodConfig,
     Interstitials,
     LiveSession,
     ManifestOptions,
     RenditionFilter,
     VodSession,
     VodSessionAd,
     VodSessionAdBreak,
@@ -101,15 +100,14 @@
     "CreateSlateRequest",
     "CreateVodSessionRequest",
     "DeleteCdnKeyRequest",
     "DeleteLiveConfigRequest",
     "DeleteSlateRequest",
     "Event",
     "GamLiveConfig",
-    "GamVodConfig",
     "GetCdnKeyRequest",
     "GetLiveAdTagDetailRequest",
     "GetLiveConfigRequest",
     "GetLiveSessionRequest",
     "GetSlateRequest",
     "GetVodAdTagDetailRequest",
     "GetVodSessionRequest",
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/gapic_metadata.json` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/gapic_version.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.7.0"  # {x-release-please-version}
+__version__ = "0.7.1"  # {x-release-please-version}
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/__init__.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.longrunning import operations_pb2
-from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
 from google.cloud.video.stitcher_v1.services.video_stitcher_service import pagers
 from google.cloud.video.stitcher_v1.types import (
     ad_tag_details,
     cdn_keys,
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.longrunning import operations_pb2
-from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
 from google.cloud.video.stitcher_v1.services.video_stitcher_service import pagers
 from google.cloud.video.stitcher_v1.types import (
     ad_tag_details,
     cdn_keys,
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/__init__.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     HtmlAdResource,
     IframeAdResource,
     StaticAdResource,
 )
 from .events import Event, ProgressEvent
 from .live_configs import AdTracking, GamLiveConfig, LiveConfig, PrefetchConfig
 from .sessions import (
-    GamVodConfig,
     Interstitials,
     LiveSession,
     ManifestOptions,
     RenditionFilter,
     VodSession,
     VodSessionAd,
     VodSessionAdBreak,
@@ -94,15 +93,14 @@
     "StaticAdResource",
     "Event",
     "ProgressEvent",
     "GamLiveConfig",
     "LiveConfig",
     "PrefetchConfig",
     "AdTracking",
-    "GamVodConfig",
     "Interstitials",
     "LiveSession",
     "ManifestOptions",
     "RenditionFilter",
     "VodSession",
     "VodSessionAd",
     "VodSessionAdBreak",
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/ad_tag_details.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/ad_tag_details.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/cdn_keys.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/cdn_keys.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/companions.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/companions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/events.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/events.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/live_configs.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/live_configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,21 +28,21 @@
         "PrefetchConfig",
         "GamLiveConfig",
     },
 )
 
 
 class AdTracking(proto.Enum):
-    r"""Determines the Ad tracking policy.
+    r"""Determines the ad tracking policy.
 
     Values:
         AD_TRACKING_UNSPECIFIED (0):
             The ad tracking policy is not specified.
         CLIENT (1):
-            Client side ad tracking is specified. The
+            Client-side ad tracking is specified. The
             client player is expected to trigger playback
             and activity events itself.
         SERVER (2):
             The Video Stitcher API will trigger playback
             events on behalf of the client player.
     """
     AD_TRACKING_UNSPECIFIED = 0
@@ -66,35 +66,29 @@
             stream config.
         gam_live_config (google.cloud.video.stitcher_v1.types.GamLiveConfig):
             Additional metadata used to register a live
             stream with Google Ad Manager (GAM)
         state (google.cloud.video.stitcher_v1.types.LiveConfig.State):
             Output only. State of the live config.
         ad_tracking (google.cloud.video.stitcher_v1.types.AdTracking):
-            Required. Determines how the ads should be tracked. If
+            Required. Determines how the ads are tracked. If
             [gam_live_config][google.cloud.video.stitcher.v1.LiveConfig.gam_live_config]
             is set, the value must be ``CLIENT`` because the IMA SDK
             handles ad tracking.
         default_slate (str):
-            This must refer to a slate in the same
-            project. In case Google Ad Manager (GAM) is
-            being used for ads this will be used to set the
-            appropriate value of slateCreativeId in
+            This must refer to a slate in the same project. If Google Ad
+            Manager (GAM) is used for ads, this string sets the value of
+            ``slateCreativeId`` in
             https://developers.google.com/ad-manager/api/reference/v202211/LiveStreamEventService.LiveStreamEvent#slateCreativeId
         stitching_policy (google.cloud.video.stitcher_v1.types.LiveConfig.StitchingPolicy):
             Defines the stitcher behavior in case an ad does not align
             exactly with the ad break boundaries. If not specified, the
             default is ``CUT_CURRENT``.
         prefetch_config (google.cloud.video.stitcher_v1.types.PrefetchConfig):
             The configuration for prefetching ads.
-        default_ad_break_duration (google.protobuf.duration_pb2.Duration):
-            The default ad pod duration in seconds that
-            will be requested when a cue-out does not
-            specify a duration. The default value of this
-            field is 30s.
     """
 
     class State(proto.Enum):
         r"""State of the live config.
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -110,15 +104,15 @@
         CREATING = 1
         READY = 2
         DELETING = 3
 
     class StitchingPolicy(proto.Enum):
         r"""Defines the ad stitching behavior in case the ad duration does not
         align exactly with the ad break boundaries. If not specified, the
-        default is CUT_CURRENT.
+        default is ``CUT_CURRENT``.
 
         Values:
             STITCHING_POLICY_UNSPECIFIED (0):
                 Stitching policy is not specified.
             CUT_CURRENT (1):
                 Cuts an ad short and returns to content in
                 the middle of the ad.
@@ -167,19 +161,14 @@
         enum=StitchingPolicy,
     )
     prefetch_config: "PrefetchConfig" = proto.Field(
         proto.MESSAGE,
         number=10,
         message="PrefetchConfig",
     )
-    default_ad_break_duration: duration_pb2.Duration = proto.Field(
-        proto.MESSAGE,
-        number=11,
-        message=duration_pb2.Duration,
-    )
 
 
 class PrefetchConfig(proto.Message):
     r"""The configuration for prefetch ads.
 
     Attributes:
         enabled (bool):
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/sessions.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/sessions.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,49 +21,26 @@
 import proto  # type: ignore
 
 from google.cloud.video.stitcher_v1.types import companions, events, live_configs
 
 __protobuf__ = proto.module(
     package="google.cloud.video.stitcher.v1",
     manifest={
-        "GamVodConfig",
         "VodSession",
         "Interstitials",
         "VodSessionAd",
         "VodSessionContent",
         "VodSessionAdBreak",
         "LiveSession",
         "ManifestOptions",
         "RenditionFilter",
     },
 )
 
 
-class GamVodConfig(proto.Message):
-    r"""Metadata for registering a VOD Session with Google Ad Manager
-    (GAM).
-
-    Attributes:
-        network_code (str):
-            Required. Ad Manager network code.
-        stream_id (str):
-            Required. The stream ID generated by Ad
-            Manager.
-    """
-
-    network_code: str = proto.Field(
-        proto.STRING,
-        number=1,
-    )
-    stream_id: str = proto.Field(
-        proto.STRING,
-        number=2,
-    )
-
-
 class VodSession(proto.Message):
     r"""Metadata for a VOD session. The session expires 4 hours after
     its creation.
 
     Attributes:
         name (str):
             Output only. The name of the VOD session, in the form of
@@ -99,20 +76,40 @@
             Output only. The generated ID of the
             VodSession's source media.
         ad_tracking (google.cloud.video.stitcher_v1.types.AdTracking):
             Required. Determines how the ad should be tracked. If
             [gam_vod_config][google.cloud.video.stitcher.v1.VodSession.gam_vod_config]
             is set, the value must be ``CLIENT`` because the IMA SDK
             handles ad tracking.
-        gam_vod_config (google.cloud.video.stitcher_v1.types.GamVodConfig):
-            This has the Google Ad Manager (GAM) related
-            metadata in the case where GAM is used for the
-            ads.
+        gam_settings (google.cloud.video.stitcher_v1.types.VodSession.GamSettings):
+            This field should be set with appropriate
+            values if GAM is being used for ads.
     """
 
+    class GamSettings(proto.Message):
+        r"""Defines fields related to Google Ad Manager (GAM). This
+        should be set if GAM is being used for ads.
+
+        Attributes:
+            network_code (str):
+                Required. Ad Manager network code.
+            stream_id (str):
+                Required. The stream ID generated by Ad
+                Manager.
+        """
+
+        network_code: str = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        stream_id: str = proto.Field(
+            proto.STRING,
+            number=2,
+        )
+
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     interstitials: "Interstitials" = proto.Field(
         proto.MESSAGE,
         number=2,
@@ -145,18 +142,18 @@
         number=10,
     )
     ad_tracking: live_configs.AdTracking = proto.Field(
         proto.ENUM,
         number=11,
         enum=live_configs.AdTracking,
     )
-    gam_vod_config: "GamVodConfig" = proto.Field(
+    gam_settings: GamSettings = proto.Field(
         proto.MESSAGE,
-        number=12,
-        message="GamVodConfig",
+        number=13,
+        message=GamSettings,
     )
 
 
 class Interstitials(proto.Message):
     r"""Describes what was stitched into a VOD session's manifest.
 
     Attributes:
@@ -309,68 +306,20 @@
     """
 
     class GamSettings(proto.Message):
         r"""Defines fields related to Google Ad Manager (GAM). This
         should be set if GAM
         is being used for ads.
 
-        This message has `oneof`_ fields (mutually exclusive fields).
-        For each oneof, at most one member field can be set at the same time.
-        Setting any member of the oneof automatically clears all other
-        members.
-
-        .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
-
         Attributes:
-            gam_hls (google.cloud.video.stitcher_v1.types.LiveSession.GamSettings.GamHls):
-                Fields that are specific to HLS manifests.
-
-                This field is a member of `oneof`_ ``manifest_fields``.
-            gam_dash (google.cloud.video.stitcher_v1.types.LiveSession.GamSettings.GamDash):
-                Fields that are specific to DASH manifests.
-
-                This field is a member of `oneof`_ ``manifest_fields``.
             stream_id (str):
                 Required. The stream ID generated by Ad
                 Manager.
         """
 
-        class GamHls(proto.Message):
-            r"""GamHls is a container for any HLS specific input fields for
-            GAM Live Stitching.
-
-            """
-
-        class GamDash(proto.Message):
-            r"""GamDash is a container for any DASH specific input fields for
-            GAM Live Stitching.
-
-            Attributes:
-                period_template_uri (str):
-                    Required. The session template url by Ad
-                    Manager for DASH periods.
-            """
-
-            period_template_uri: str = proto.Field(
-                proto.STRING,
-                number=1,
-            )
-
-        gam_hls: "LiveSession.GamSettings.GamHls" = proto.Field(
-            proto.MESSAGE,
-            number=2,
-            oneof="manifest_fields",
-            message="LiveSession.GamSettings.GamHls",
-        )
-        gam_dash: "LiveSession.GamSettings.GamDash" = proto.Field(
-            proto.MESSAGE,
-            number=3,
-            oneof="manifest_fields",
-            message="LiveSession.GamSettings.GamDash",
-        )
         stream_id: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
     name: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/slates.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/slates.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             Output only. The name of the slate, in the form of
             ``projects/{project_number}/locations/{location}/slates/{id}``.
         uri (str):
             The URI to fetch the source content for the
             slate. This URI must return an MP4 video with at
             least one audio track.
         gam_slate (google.cloud.video.stitcher_v1.types.Slate.GamSlate):
-            gam_slate has all the GAM related attributes of slates.
+            gam_slate has all the GAM-related attributes of slates.
     """
 
     class GamSlate(proto.Message):
         r"""GamSlate object has Google Ad Manager (GAM) related
         properties for the slate.
 
         Attributes:
```

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/stitch_details.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/stitch_details.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google/cloud/video/stitcher_v1/types/video_stitcher_service.py` & `google-cloud-video-stitcher-0.7.1/google/cloud/video/stitcher_v1/types/video_stitcher_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/PKG-INFO` & `google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-stitcher
-Version: 0.7.0
+Version: 0.7.1
 Summary: Google Cloud Video Stitcher API client library
 Home-page: https://github.com/googleapis/python-video-stitcher
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-video-stitcher-0.7.0/google_cloud_video_stitcher.egg-info/SOURCES.txt` & `google-cloud-video-stitcher-0.7.1/google_cloud_video_stitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/setup.py` & `google-cloud-video-stitcher-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/tests/__init__.py` & `google-cloud-video-stitcher-0.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/tests/unit/__init__.py` & `google-cloud-video-stitcher-0.7.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/tests/unit/gapic/__init__.py` & `google-cloud-video-stitcher-0.7.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/tests/unit/gapic/stitcher_v1/__init__.py` & `google-cloud-video-stitcher-0.7.1/tests/unit/gapic/stitcher_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.0/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py` & `google-cloud-video-stitcher-0.7.1/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py`

 * *Files identical despite different names*

