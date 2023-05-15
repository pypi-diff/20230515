# Comparing `tmp/gitlab-ci-generator-1.0.3.tar.gz` & `tmp/gitlab-ci-generator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-ci-generator-1.0.3.tar", last modified: Wed Sep  7 16:43:48 2022, max compression
+gzip compressed data, was "gitlab-ci-generator-1.0.4.tar", last modified: Mon May 15 17:33:34 2023, max compression
```

## Comparing `gitlab-ci-generator-1.0.3.tar` & `gitlab-ci-generator-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2022-09-07 16:43:48.754757 gitlab-ci-generator-1.0.3/
--rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.3/MANIFEST.in
--rw-r--r--   0 developer  (9999) developer  (9999)     8742 2022-09-07 16:43:48.754757 gitlab-ci-generator-1.0.3/PKG-INFO
--rw-rw-rw-   0 developer  (9999) developer  (9999)     8374 2022-09-07 16:43:31.000000 gitlab-ci-generator-1.0.3/README.md
--rw-r--r--   0 developer  (9999) developer  (9999)        6 2022-09-07 16:43:48.000000 gitlab-ci-generator-1.0.3/VERSION.txt
--rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2022-09-07 16:43:48.754757 gitlab-ci-generator-1.0.3/setup.cfg
--rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.3/setup.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2022-09-07 16:43:48.754757 gitlab-ci-generator-1.0.3/src/
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2022-09-07 16:43:48.754757 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator.egg-info/
--rw-r--r--   0 developer  (9999) developer  (9999)     8742 2022-09-07 16:43:48.000000 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator.egg-info/PKG-INFO
--rw-r--r--   0 developer  (9999) developer  (9999)      499 2022-09-07 16:43:48.000000 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (9999) developer  (9999)        1 2022-09-07 16:43:48.000000 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       94 2022-09-07 16:43:48.000000 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator.egg-info/entry_points.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       29 2022-09-07 16:43:48.000000 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator.egg-info/requires.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       28 2022-09-07 16:43:48.000000 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2022-09-07 16:43:48.754757 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator_package/
--rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator_package/__init__.py
--rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator_package/gitlab_ci_generator.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2022-09-07 16:43:48.754757 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator_package/templates/
--rw-rw-rw-   0 developer  (9999) developer  (9999)     1896 2022-09-06 14:08:49.000000 gitlab-ci-generator-1.0.3/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.4/MANIFEST.in
+-rw-r--r--   0 developer  (9999) developer  (9999)     8723 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/PKG-INFO
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     8374 2022-09-07 16:43:31.000000 gitlab-ci-generator-1.0.4/README.md
+-rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-05-15 17:33:33.000000 gitlab-ci-generator-1.0.4/VERSION.txt
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/setup.cfg
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.4/setup.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/src/
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/
+-rw-r--r--   0 developer  (9999) developer  (9999)     8723 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/requires.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/__init__.py
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/gitlab_ci_generator.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/templates/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     1896 2022-09-06 14:08:49.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
```

### Comparing `gitlab-ci-generator-1.0.3/PKG-INFO` & `gitlab-ci-generator-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: gitlab-ci-generator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generates a mono-repo ci file.
 Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
 Author: Gary Schaetz
 Author-email: gary@schaetzkc.com
 License: MIT
 Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # gitlab-ci-generator
 This project builds a dynamic gitlab ci file that is intended to be used for monorepos.  The concept is to simplify the amount of work that is needed to manage the monorepo.
 
 ## Installation
 You can download and run directly with python or install using:
@@ -227,8 +226,7 @@
   variables:
     PARENT_PIPELINE_ID: $CI_PIPELINE_ID
     PARENT_PIPELINE_SOURCE: $CI_PIPELINE_SOURCE
 ```
 
 ## License
 MIT License
-
```

### Comparing `gitlab-ci-generator-1.0.3/README.md` & `gitlab-ci-generator-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.3/setup.py` & `gitlab-ci-generator-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.3/src/gitlab_ci_generator.egg-info/PKG-INFO` & `gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: gitlab-ci-generator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generates a mono-repo ci file.
 Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
 Author: Gary Schaetz
 Author-email: gary@schaetzkc.com
 License: MIT
 Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # gitlab-ci-generator
 This project builds a dynamic gitlab ci file that is intended to be used for monorepos.  The concept is to simplify the amount of work that is needed to manage the monorepo.
 
 ## Installation
 You can download and run directly with python or install using:
@@ -227,8 +226,7 @@
   variables:
     PARENT_PIPELINE_ID: $CI_PIPELINE_ID
     PARENT_PIPELINE_SOURCE: $CI_PIPELINE_SOURCE
 ```
 
 ## License
 MIT License
-
```

### Comparing `gitlab-ci-generator-1.0.3/src/gitlab_ci_generator_package/gitlab_ci_generator.py` & `gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/gitlab_ci_generator.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.3/src/gitlab_ci_generator_package/templates/gitlab-template.jinja` & `gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/templates/gitlab-template.jinja`

 * *Files identical despite different names*

