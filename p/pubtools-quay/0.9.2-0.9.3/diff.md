# Comparing `tmp/pubtools-quay-0.9.2.tar.gz` & `tmp/pubtools-quay-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubtools-quay-0.9.2.tar", last modified: Wed Mar  2 13:00:39 2022, max compression
+gzip compressed data, was "pubtools-quay-0.9.3.tar", last modified: Fri Apr  1 10:41:37 2022, max compression
```

## Comparing `pubtools-quay-0.9.2.tar` & `pubtools-quay-0.9.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:39.933796 pubtools-quay-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7283 2022-03-02 13:00:39.933796 pubtools-quay-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:39.925795 pubtools-quay-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:39.929795 pubtools-quay-0.9.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/clear_repo.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/command_executor.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4913 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/container_image_pusher.rst
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/entrypoints_reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/iib_operations.rst
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/image_untagger.rst
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/manifest_list_merger.rst
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/merge_manifest_list.rst
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/modules_reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/operator_pusher.rst
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/push_docker.rst
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/quay_api_client.rst
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/quay_client.rst
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/quay_session.rst
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/remove_repo.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/signature_handler.rst
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/signature_remover.rst
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/tag_docker.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/tag_images.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/untag_images.rst
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/docs/source/utilities.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:39.929795 pubtools-quay-0.9.2/pubtools/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:39.929795 pubtools-quay-0.9.2/pubtools/_quay/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4385 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/clear_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)    16033 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/command_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    12232 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/container_image_pusher.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)    13568 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/iib_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     7478 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/image_untagger.py
--rw-r--r--   0 runner    (1001) docker     (121)     8999 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/manifest_claims_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/manifest_list_merger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2705 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/merge_manifest_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    18302 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/operator_pusher.py
--rw-r--r--   0 runner    (1001) docker     (121)    28815 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/push_docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5640 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/push_docker2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/quay_api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    11453 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/quay_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/quay_session.py
--rw-r--r--   0 runner    (1001) docker     (121)    24977 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/quay_steps.py
--rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/remove_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)    30154 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/signature_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    15085 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/signature_remover.py
--rw-r--r--   0 runner    (1001) docker     (121)    34232 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/tag_docker.py
--rw-r--r--   0 runner    (1001) docker     (121)    11312 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/tag_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/untag_images.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:39.929795 pubtools-quay-0.9.2/pubtools/_quay/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    11549 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/utils/misc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12359 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/pubtools/_quay/utils/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:39.933796 pubtools-quay-0.9.2/pubtools_quay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7283 2022-03-02 13:00:39.000000 pubtools-quay-0.9.2/pubtools_quay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-03-02 13:00:39.000000 pubtools-quay-0.9.2/pubtools_quay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-02 13:00:39.000000 pubtools-quay-0.9.2/pubtools_quay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-03-02 13:00:39.000000 pubtools-quay-0.9.2/pubtools_quay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-03-02 13:00:39.000000 pubtools-quay-0.9.2/pubtools_quay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-02 13:00:39.000000 pubtools-quay-0.9.2/pubtools_quay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-03-02 13:00:39.933796 pubtools-quay-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5210 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:39.925795 pubtools-quay-0.9.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:39.933796 pubtools-quay-0.9.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/tests/utils/caplog_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-03-02 13:00:31.000000 pubtools-quay-0.9.2/tests/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:37.439293 pubtools-quay-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-04-01 10:41:37.439293 pubtools-quay-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:37.431292 pubtools-quay-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:37.435293 pubtools-quay-0.9.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (121)     3399 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/clear_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/command_executor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4913 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/container_image_pusher.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/entrypoints_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/iib_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/image_untagger.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/manifest_list_merger.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/merge_manifest_list.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/modules_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/operator_pusher.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      590 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/push_docker.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/quay_api_client.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/quay_client.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/quay_session.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/remove_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/signature_handler.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/signature_remover.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/tag_docker.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/tag_images.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/untag_images.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/docs/source/utilities.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:37.435293 pubtools-quay-0.9.3/pubtools/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:37.439293 pubtools-quay-0.9.3/pubtools/_quay/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4385 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/clear_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16033 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/command_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12302 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/container_image_pusher.py
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13568 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/iib_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7789 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/image_untagger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17419 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/manifest_claims_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/manifest_list_merger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2705 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/merge_manifest_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18302 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/operator_pusher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29413 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/push_docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5640 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/push_docker2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/quay_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11453 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/quay_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5049 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/quay_session.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24977 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/quay_steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/remove_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30086 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/signature_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15085 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/signature_remover.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34232 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/tag_docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11475 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/tag_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/untag_images.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:37.439293 pubtools-quay-0.9.3/pubtools/_quay/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11549 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/utils/misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12359 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/pubtools/_quay/utils/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:37.439293 pubtools-quay-0.9.3/pubtools_quay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-04-01 10:41:37.000000 pubtools-quay-0.9.3/pubtools_quay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-04-01 10:41:37.000000 pubtools-quay-0.9.3/pubtools_quay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 10:41:37.000000 pubtools-quay-0.9.3/pubtools_quay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-04-01 10:41:37.000000 pubtools-quay-0.9.3/pubtools_quay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-04-01 10:41:37.000000 pubtools-quay-0.9.3/pubtools_quay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-01 10:41:37.000000 pubtools-quay-0.9.3/pubtools_quay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-04-01 10:41:37.439293 pubtools-quay-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5210 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:37.431292 pubtools-quay-0.9.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:37.439293 pubtools-quay-0.9.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/tests/utils/caplog_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-04-01 10:41:25.000000 pubtools-quay-0.9.3/tests/utils/misc.py
```

### Comparing `pubtools-quay-0.9.2/LICENSE` & `pubtools-quay-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/PKG-INFO` & `pubtools-quay-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubtools-quay
-Version: 0.9.2
+Version: 0.9.3
 Summary: Pubtools-quay
 Home-page: https://github.com/release-engineering/pubtools-quay
 Author: Lubomir Gallovic
 Author-email: lgallovi@redhat.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -132,14 +132,21 @@
     --reference quay.io/src/image:1 \
     --remove-last \
     --quay-user quay+username \
 
 ChangeLog
 =========
 
+0.9.3 (2022-04-01)
+--------------------
+* Fixing signing issues
+* Skip getting v2s1 digest for non-amd64 images
+* Less skopeo login to source registry
+* Tolerate get_manifest 404 in image untagger
+
 0.9.2 (2022-03-02)
 --------------------
 * Add a timeout to all HTTP requests
 * Removed the option for entrypoints to send UMB messages
 
 0.9.1 (2022-02-02)
 ------------------
```

### Comparing `pubtools-quay-0.9.2/README.rst` & `pubtools-quay-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/Makefile` & `pubtools-quay-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/CHANGELOG.rst` & `pubtools-quay-0.9.3/docs/source/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 ChangeLog
 =========
 
+0.9.3 (2022-04-01)
+--------------------
+* Fixing signing issues
+* Skip getting v2s1 digest for non-amd64 images
+* Less skopeo login to source registry
+* Tolerate get_manifest 404 in image untagger
+
 0.9.2 (2022-03-02)
 --------------------
 * Add a timeout to all HTTP requests
 * Removed the option for entrypoints to send UMB messages
 
 0.9.1 (2022-02-02)
 ------------------
```

### Comparing `pubtools-quay-0.9.2/docs/source/README.rst` & `pubtools-quay-0.9.3/docs/source/README.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/clear_repo.rst` & `pubtools-quay-0.9.3/docs/source/clear_repo.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/command_executor.rst` & `pubtools-quay-0.9.3/docs/source/command_executor.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/conf.py` & `pubtools-quay-0.9.3/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 # -- Project information -----------------------------------------------------
 
 project = u"pubtools-quay"
 copyright = u"2021, Red Hat"
 author = u"Red Hat"
 
 # The short X.Y version
-version = u"0.9.2"
+version = u"0.9.3"
 # The full version, including alpha/beta/rc tags
-release = u"0.9.2"
+release = u"0.9.3"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `pubtools-quay-0.9.2/docs/source/container_image_pusher.rst` & `pubtools-quay-0.9.3/docs/source/container_image_pusher.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/merge_manifest_list.rst` & `pubtools-quay-0.9.3/docs/source/merge_manifest_list.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/modules_reference.rst` & `pubtools-quay-0.9.3/docs/source/modules_reference.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/operator_pusher.rst` & `pubtools-quay-0.9.3/docs/source/operator_pusher.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/push_docker.rst` & `pubtools-quay-0.9.3/docs/source/push_docker.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/quay_client.rst` & `pubtools-quay-0.9.3/docs/source/quay_client.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/remove_repo.rst` & `pubtools-quay-0.9.3/docs/source/remove_repo.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/signature_handler.rst` & `pubtools-quay-0.9.3/docs/source/signature_handler.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/signature_remover.rst` & `pubtools-quay-0.9.3/docs/source/signature_remover.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/tag_docker.rst` & `pubtools-quay-0.9.3/docs/source/tag_docker.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/tag_images.rst` & `pubtools-quay-0.9.3/docs/source/tag_images.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/untag_images.rst` & `pubtools-quay-0.9.3/docs/source/untag_images.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/docs/source/utilities.rst` & `pubtools-quay-0.9.3/docs/source/utilities.rst`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/clear_repo.py` & `pubtools-quay-0.9.3/pubtools/_quay/clear_repo.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/command_executor.py` & `pubtools-quay-0.9.3/pubtools/_quay/command_executor.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/container_image_pusher.py` & `pubtools-quay-0.9.3/pubtools/_quay/container_image_pusher.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         tag_images_partial = functools.partial(
             tag_images,
             source_ref,
             dest_refs,
             all_arch=all_arch,
             quay_user=target_settings["dest_quay_user"],
             quay_password=target_settings["dest_quay_password"],
+            source_quay_host=target_settings.get("source_quay_host"),
             source_quay_user=target_settings.get("source_quay_user"),
             source_quay_password=target_settings.get("source_quay_password"),
             container_exec=True,
             container_image=target_settings["skopeo_image"],
             docker_url=target_settings.get("docker_host") or "unix://var/run/docker.sock",
             docker_timeout=target_settings.get("docker_timeout"),
             docker_verify_tls=target_settings.get("docker_tls_verify") or False,
```

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/exceptions.py` & `pubtools-quay-0.9.3/pubtools/_quay/exceptions.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/hooks.py` & `pubtools-quay-0.9.3/pubtools/_quay/hooks.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/iib_operations.py` & `pubtools-quay-0.9.3/pubtools/_quay/iib_operations.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/image_untagger.py` & `pubtools-quay-0.9.3/pubtools/_quay/image_untagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import requests
 
 from .quay_client import QuayClient
 from .quay_api_client import QuayApiClient
 
 LOG = logging.getLogger("pubtools.quay")
 
 
@@ -100,15 +101,22 @@
         tag_digest_mapping = {}
         digest_tag_mapping = {}
         image_schema = "{0}/{1}:{2}"
         repo_tags = self._quay_client.get_repository_tags(repository)
 
         for tag in repo_tags["tags"]:
             image = image_schema.format(self.host, repository, tag)
-            manifest = self._quay_client.get_manifest(image)
+            try:
+                manifest = self._quay_client.get_manifest(image)
+            except requests.exceptions.HTTPError as e:
+                # Just removed tags could still be in tags list while manifests are removed
+                if e.response.status_code == 404:
+                    continue
+                else:
+                    raise
             digest = self._quay_client.get_manifest_digest(image)
 
             # Option 1: No manifest list, only manifest
             if manifest["mediaType"] == QuayClient.MANIFEST_V2S2_TYPE:
                 tag_digest_mapping[tag] = [digest]
                 digest_tag_mapping.setdefault(digest, []).append(tag)
```

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/manifest_list_merger.py` & `pubtools-quay-0.9.3/pubtools/_quay/manifest_list_merger.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/merge_manifest_list.py` & `pubtools-quay-0.9.3/pubtools/_quay/merge_manifest_list.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/operator_pusher.py` & `pubtools-quay-0.9.3/pubtools/_quay/operator_pusher.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/push_docker.py` & `pubtools-quay-0.9.3/pubtools/_quay/push_docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,23 @@
                 raise BadPushItem("Push item {0} doesn't contain pull data.".format(item))
             LOG.info("Docker push item found: {0}".format(item))
             pull_url = item.metadata["pull_url"]
             if pull_url in url_items:
                 url_items[pull_url].append(item)
             else:
                 url_items[pull_url] = [item]
-        for _, items in sorted(url_items.items()):
-            docker_push_items.append(items[0])
+        for _, items in url_items.items():
+            non_amd64 = True
+            for item in items:
+                if item.metadata["arch"] == "amd64":
+                    docker_push_items.append(item)
+                    non_amd64 = False
+                    break
+            if non_amd64:
+                docker_push_items.append(items[0])
 
         return docker_push_items
 
     @log_step("Get operator push items")
     def get_operator_push_items(self):
         """
         Filter out push items to only include operator ones.
@@ -325,17 +332,21 @@
                         continue
                     # tag exists in the repo, add to backup tags
                     if tag in repo_tags.get("tags", {}):
                         image_tag = image_schema_tag.format(
                             host=self.quay_host, repo=full_repo, tag=tag
                         )
                         digest = self.dest_quay_client.get_manifest_digest(image_tag)
-                        v2s1_digest = self.dest_quay_client.get_manifest_digest(
-                            image_tag, media_type=QuayClient.MANIFEST_V2S1_TYPE
-                        )
+                        # skip getting v2s1 for non-amd64 image
+                        if item.metadata["arch"] == "amd64":
+                            v2s1_digest = self.dest_quay_client.get_manifest_digest(
+                                image_tag, media_type=QuayClient.MANIFEST_V2S1_TYPE
+                            )
+                        else:
+                            v2s1_digest = None
                         # for backup tags store also digest
                         image_data = PushDocker.ImageData(full_repo, tag, digest, v2s1_digest)
                         image = image_schema.format(
                             host=self.quay_host,
                             repo=full_repo,
                             digest=digest,
                         )
@@ -434,15 +445,16 @@
             ext_repo = get_external_container_repo_name(image_data.repo.split("/")[1])
             if "manifests" in manifest:
                 for arch_manifest in manifest["manifests"]:
                     outdated_signatures.append((arch_manifest["digest"], image_data.tag, ext_repo))
             else:
                 outdated_signatures.append((image_data.digest, image_data.tag, ext_repo))
             # also add V2S1 signature (only one per tag)
-            outdated_signatures.append((image_data.v2s1_digest, image_data.tag, ext_repo))
+            if image_data.v2s1_digest:
+                outdated_signatures.append((image_data.v2s1_digest, image_data.tag, ext_repo))
 
         signatures_to_remove = []
         for existing_signature in container_signature_handler.get_signatures_from_pyxis(
             [sig[0] for sig in outdated_signatures]
         ):
             if (
                 existing_signature["manifest_digest"],
@@ -542,15 +554,16 @@
                     for mtype in missing_media_types:
                         if mtype == QuayClient.MANIFEST_V2S2_TYPE:
                             if repo not in v2_sch2_cache:
                                 v2_sch2_cache[repo] = self._fetch_digest(internal_repo, tag, mtype)
                             item.metadata["new_digests"].setdefault((repo, tag), {})[
                                 mtype
                             ] = v2_sch2_cache[repo]
-                        else:
+                        # Fetch v2s1 only for amd64 image
+                        elif item.metadata["arch"] == "amd64":
                             item.metadata["new_digests"].setdefault((repo, tag), {})[
                                 mtype
                             ] = self._fetch_digest(internal_repo, tag, mtype)
 
     def run(self):
         """
         Perform the full push-docker workflow.
```

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/push_docker2.py` & `pubtools-quay-0.9.3/pubtools/_quay/push_docker2.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/quay_api_client.py` & `pubtools-quay-0.9.3/pubtools/_quay/quay_api_client.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/quay_client.py` & `pubtools-quay-0.9.3/pubtools/_quay/quay_client.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/quay_session.py` & `pubtools-quay-0.9.3/pubtools/_quay/quay_session.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/quay_steps.py` & `pubtools-quay-0.9.3/pubtools/_quay/quay_steps.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/remove_repo.py` & `pubtools-quay-0.9.3/pubtools/_quay/remove_repo.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/signature_handler.py` & `pubtools-quay-0.9.3/pubtools/_quay/signature_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import base64
 from datetime import datetime
 import json
 import logging
 import uuid
 import tempfile
 
-import proton
-
 from .exceptions import SigningError
 from .utils.misc import (
     run_entrypoint,
     log_step,
     get_pyxis_ssl_paths,
 )
 from .quay_client import QuayClient
-from .manifest_claims_handler import ManifestClaimsHandler
+from .manifest_claims_handler import _ManifestClaimsRunner, UMBSettings
 
 LOG = logging.getLogger("pubtools.quay")
 
 
 class SignatureHandler:
     """Base class implementing operations common for container and operator signing."""
 
@@ -303,31 +301,28 @@
             )
         )
 
         address = (
             "queue://Consumer.msg-producer-pub"
             ".{task_id}.VirtualTopic.eng.robosignatory.container.sign".format(task_id=self.task_id)
         )
-
         docker_settings = self.target_settings["docker_settings"]
-        claims_handler = ManifestClaimsHandler(
-            umb_urls=docker_settings["umb_urls"],
+        umb_settings = UMBSettings(
+            broker_urls=docker_settings["umb_urls"],
             radas_address=docker_settings.get("umb_radas_address", address),
-            claim_messages=claim_messages,
             pub_cert=docker_settings.get("umb_pub_cert", "/etc/pub/umb-pub-cert-key.pem"),
             ca_cert=docker_settings.get("umb_ca_cert", "/etc/pki/tls/certs/ca-bundle.crt"),
-            timeout=docker_settings.get("umb_signing_timeout", 600),
-            throttle=docker_settings.get("umb_signing_throttle", 100),
-            retry=docker_settings.get("umb_signing_retry", 3),
-            message_sender_callback=message_sender_callback,
+            signing_timeout=docker_settings.get("umb_signing_timeout", 600),
+            signing_throttle=docker_settings.get("umb_signing_throttle", 100),
+            signing_retry=docker_settings.get("umb_signing_retry", 3),
         )
-        container = proton.reactor.Container(claims_handler)
-        container.run()
 
-        return claims_handler.received_messages
+        runner = _ManifestClaimsRunner(umb_settings, claim_messages, message_sender_callback)
+        runner.start()
+        return runner.received_messages
 
     def upload_signatures_to_pyxis(self, claim_mesages, signature_messages):
         """
         Upload signatures to Pyxis by using a pubtools-pyxis entrypoint.
 
         Data required for a Pyxis POST request:
         - manifest_digest
```

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/signature_remover.py` & `pubtools-quay-0.9.3/pubtools/_quay/signature_remover.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/tag_docker.py` & `pubtools-quay-0.9.3/pubtools/_quay/tag_docker.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/tag_images.py` & `pubtools-quay-0.9.3/pubtools/_quay/tag_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,19 @@
     },
     ("--quay-password",): {
         "help": "Password for Quay. Can be specified by env variable QUAY_PASSWORD.",
         "required": False,
         "type": str,
         "env_variable": "QUAY_PASSWORD",
     },
+    ("--source-quay-host",): {
+        "help": "Host of source_ref.",
+        "required": False,
+        "type": str,
+    },
     ("--source-quay-user",): {
         "help": "Username for source_ref registry login.",
         "required": False,
         "type": str,
     },
     ("--source-quay-password",): {
         "help": "Password for source_ref registry. Can be specified by env "
@@ -161,14 +166,15 @@
 
 def tag_images(
     source_ref,
     dest_refs,
     all_arch=False,
     quay_user=None,
     quay_password=None,
+    source_quay_host=None,
     source_quay_user=None,
     source_quay_password=None,
     remote_exec=False,
     ssh_remote_host=None,
     ssh_remote_host_port=None,
     ssh_reject_unknown_host=False,
     ssh_username=None,
@@ -193,14 +199,16 @@
             List of destination image references.
         all_arch (bool):
             Whether to copy all architectures.
         quay_user (str):
             Quay username for Docker HTTP API.
         quay_password (str):
             Quay password for Docker HTTP API.
+        source_quay_host (str):
+            Host of source ref.
         source_quay_user (str):
             Quay username for Docker HTTP API for the source ref.
         source_quay_password (str):
             Quay password for Docker HTTP API for the source ref.
         remote_exec (bool):
             Whether to execute the command remotely. Takes precedence over container_exec.
         ssh_remote_host (str):
@@ -271,18 +279,17 @@
             registry_password,
         )
     else:
         executor_class = functools.partial(LocalExecutor)
 
     with executor_class() as executor:
         dest_host = dest_refs[0].split("/", 1)[0]
-        source_host = source_ref.split("/", 1)[0]
         executor.skopeo_login(dest_host, quay_user, quay_password)
-        if source_quay_user and source_quay_password and dest_host != source_host:
-            executor.skopeo_login(source_host, source_quay_user, source_quay_password)
+        if source_quay_host and source_quay_user and source_quay_password:
+            executor.skopeo_login(source_quay_host, source_quay_user, source_quay_password)
         executor.tag_images(source_ref, dest_refs, all_arch)
 
     pm.hook.quay_images_tagged(source_ref=source_ref, dest_refs=sorted(dest_refs))
 
 
 def verify_tag_images_args(
     quay_user,
```

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/untag_images.py` & `pubtools-quay-0.9.3/pubtools/_quay/untag_images.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/utils/logger.py` & `pubtools-quay-0.9.3/pubtools/_quay/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/utils/misc.py` & `pubtools-quay-0.9.3/pubtools/_quay/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools/_quay/utils/stepper.py` & `pubtools-quay-0.9.3/pubtools/_quay/utils/stepper.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools_quay.egg-info/PKG-INFO` & `pubtools-quay-0.9.3/pubtools_quay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubtools-quay
-Version: 0.9.2
+Version: 0.9.3
 Summary: Pubtools-quay
 Home-page: https://github.com/release-engineering/pubtools-quay
 Author: Lubomir Gallovic
 Author-email: lgallovi@redhat.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -132,14 +132,21 @@
     --reference quay.io/src/image:1 \
     --remove-last \
     --quay-user quay+username \
 
 ChangeLog
 =========
 
+0.9.3 (2022-04-01)
+--------------------
+* Fixing signing issues
+* Skip getting v2s1 digest for non-amd64 images
+* Less skopeo login to source registry
+* Tolerate get_manifest 404 in image untagger
+
 0.9.2 (2022-03-02)
 --------------------
 * Add a timeout to all HTTP requests
 * Removed the option for entrypoints to send UMB messages
 
 0.9.1 (2022-02-02)
 ------------------
```

### Comparing `pubtools-quay-0.9.2/pubtools_quay.egg-info/SOURCES.txt` & `pubtools-quay-0.9.3/pubtools_quay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/pubtools_quay.egg-info/entry_points.txt` & `pubtools-quay-0.9.3/pubtools_quay.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/setup.py` & `pubtools-quay-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 extras_require = {"reST": ["Sphinx"]}
 if os.environ.get("READTHEDOCS", None):
     extras_require["reST"].append("recommonmark")
 
 setup(
     name="pubtools-quay",
-    version="0.9.2",
+    version="0.9.3",
     description="Pubtools-quay",
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author="Lubomir Gallovic",
     author_email="lgallovi@redhat.com",
     url="https://github.com/release-engineering/pubtools-quay",
     classifiers=classifiers,
```

### Comparing `pubtools-quay-0.9.2/tests/utils/caplog_compat.py` & `pubtools-quay-0.9.3/tests/utils/caplog_compat.py`

 * *Files identical despite different names*

### Comparing `pubtools-quay-0.9.2/tests/utils/misc.py` & `pubtools-quay-0.9.3/tests/utils/misc.py`

 * *Files identical despite different names*

