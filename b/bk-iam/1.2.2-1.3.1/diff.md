# Comparing `tmp/bk-iam-1.2.2.tar.gz` & `tmp/bk-iam-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bk-iam-1.2.2.tar", last modified: Wed Aug 17 09:04:36 2022, max compression
+gzip compressed data, was "dist/bk-iam-1.3.1.tar", last modified: Mon May 15 03:01:19 2023, max compression
```

## Comparing `bk-iam-1.2.2.tar` & `bk-iam-1.3.1.tar`

### file list

```diff
@@ -1,93 +1,92 @@
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/
--rw-r--r--   0 wukunliang   (501) staff       (20)     1069 2022-03-21 09:26:47.000000 bk-iam-1.2.2/LICENSE.txt
--rw-r--r--   0 wukunliang   (501) staff       (20)      220 2022-03-21 09:26:47.000000 bk-iam-1.2.2/MANIFEST.in
--rw-r--r--   0 wukunliang   (501) staff       (20)      769 2022-08-17 09:04:36.000000 bk-iam-1.2.2/PKG-INFO
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/bk_iam.egg-info/
--rw-r--r--   0 wukunliang   (501) staff       (20)      769 2022-08-17 09:04:36.000000 bk-iam-1.2.2/bk_iam.egg-info/PKG-INFO
--rw-r--r--   0 wukunliang   (501) staff       (20)     1960 2022-08-17 09:04:36.000000 bk-iam-1.2.2/bk_iam.egg-info/SOURCES.txt
--rw-r--r--   0 wukunliang   (501) staff       (20)        1 2022-08-17 09:04:36.000000 bk-iam-1.2.2/bk_iam.egg-info/dependency_links.txt
--rw-r--r--   0 wukunliang   (501) staff       (20)       54 2022-08-17 09:04:36.000000 bk-iam-1.2.2/bk_iam.egg-info/requires.txt
--rw-r--r--   0 wukunliang   (501) staff       (20)       10 2022-08-17 09:04:36.000000 bk-iam-1.2.2/bk_iam.egg-info/top_level.txt
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/
--rw-r--r--   0 wukunliang   (501) staff       (20)     1911 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)       47 2022-08-17 09:03:52.000000 bk-iam-1.2.2/iam/__version__.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/api/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/api/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)    15672 2022-07-22 03:54:17.000000 bk-iam-1.2.2/iam/api/client.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     5536 2022-07-22 03:54:17.000000 bk-iam-1.2.2/iam/api/http.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/apply/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/apply/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     7594 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/apply/models.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/auth/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/auth/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)    14884 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/auth/models.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      827 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/cache.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     1286 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/collection.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/__init__.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/converter/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/converter/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     2226 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/converter/base.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     5859 2022-07-22 03:54:17.000000 bk-iam-1.2.2/iam/contrib/converter/queryset.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     5814 2022-07-22 03:54:17.000000 bk-iam-1.2.2/iam/contrib/converter/sql.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/django/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/django/__init__.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/django/dispatcher/
--rw-r--r--   0 wukunliang   (501) staff       (20)      865 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/django/dispatcher/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     9908 2022-08-17 09:03:52.000000 bk-iam-1.2.2/iam/contrib/django/dispatcher/dispatchers.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      923 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/django/dispatcher/exceptions.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     1347 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/django/middlewares.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     1308 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/django/response.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      781 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/http.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/iam_migration/
--rw-r--r--   0 wukunliang   (501) staff       (20)      818 2022-03-21 09:34:17.000000 bk-iam-1.2.2/iam/contrib/iam_migration/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      951 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/apps.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      916 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/conf.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      820 2022-03-21 09:34:17.000000 bk-iam-1.2.2/iam/contrib/iam_migration/constants.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      845 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/exceptions.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/iam_migration/management/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/management/__init__.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/iam_migration/management/commands/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/management/commands/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     3756 2022-03-21 09:34:17.000000 bk-iam-1.2.2/iam/contrib/iam_migration/management/commands/iam_makemigrations.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/iam_migration/migrations/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/migrations/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     2757 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/migrator.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     1343 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/template.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/iam_migration/templates/
--rw-r--r--   0 wukunliang   (501) staff       (20)      570 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/templates/migration.tmpl
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/iam_migration/utils/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/iam_migration/utils/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)    24787 2022-07-22 03:54:17.000000 bk-iam-1.2.2/iam/contrib/iam_migration/utils/do_migrate.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/contrib/tastypie/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/tastypie/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     8012 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/tastypie/authorization.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     4177 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/tastypie/resource.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     2090 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/contrib/tastypie/shortcuts.py
--rw-r--r--   0 wukunliang   (501) staff       (20)    10156 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/dummy_iam.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/eval/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/eval/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     1803 2022-07-22 03:54:17.000000 bk-iam-1.2.2/iam/eval/constants.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     2252 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/eval/expression.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     2079 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/eval/object.py
--rw-r--r--   0 wukunliang   (501) staff       (20)    11845 2022-07-22 03:54:17.000000 bk-iam-1.2.2/iam/eval/operators.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     2310 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/exceptions.py
--rw-r--r--   0 wukunliang   (501) staff       (20)    22754 2022-07-22 03:54:17.000000 bk-iam-1.2.2/iam/iam.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     1684 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/meta.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/model/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/model/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     3470 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/model/models.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/objects.py
-drwxr-xr-x   0 wukunliang   (501) staff       (20)        0 2022-08-17 09:04:36.000000 bk-iam-1.2.2/iam/resource/
--rw-r--r--   0 wukunliang   (501) staff       (20)      744 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/resource/__init__.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      982 2022-08-17 09:03:52.000000 bk-iam-1.2.2/iam/resource/constants.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      948 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/resource/dispatcher.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     3430 2022-08-17 09:03:52.000000 bk-iam-1.2.2/iam/resource/provider.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     1439 2022-08-17 09:03:52.000000 bk-iam-1.2.2/iam/resource/utils.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     1179 2022-03-21 09:26:47.000000 bk-iam-1.2.2/iam/shortcuts.py
--rw-r--r--   0 wukunliang   (501) staff       (20)     5087 2022-07-22 03:54:17.000000 bk-iam-1.2.2/iam/utils.py
--rw-r--r--   0 wukunliang   (501) staff       (20)      194 2022-03-21 09:26:47.000000 bk-iam-1.2.2/pyproject.toml
--rw-r--r--   0 wukunliang   (501) staff       (20)     3670 2022-08-17 09:03:52.000000 bk-iam-1.2.2/readme.md
--rw-r--r--   0 wukunliang   (501) staff       (20)     3109 2022-03-21 09:26:47.000000 bk-iam-1.2.2/readme_en.md
--rw-r--r--   0 wukunliang   (501) staff       (20)       38 2022-08-17 09:04:36.000000 bk-iam-1.2.2/setup.cfg
--rw-r--r--   0 wukunliang   (501) staff       (20)     1244 2022-03-21 09:26:47.000000 bk-iam-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-15 02:44:48.000000 bk-iam-1.3.1/iam/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/api/
+-rw-r--r--   0 root         (0) root         (0)    16124 2023-03-07 08:22:34.000000 bk-iam-1.3.1/iam/api/client.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/api/http.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/objects.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/dummy_iam.py
+-rw-r--r--   0 root         (0) root         (0)    23130 2023-03-07 08:59:27.000000 bk-iam-1.3.1/iam/iam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/apply/
+-rw-r--r--   0 root         (0) root         (0)     7594 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/apply/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/apply/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/eval/
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/eval/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/eval/object.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/eval/expression.py
+-rw-r--r--   0 root         (0) root         (0)    11845 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/eval/operators.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/eval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/model/
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/model/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/collection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/iam_migration/
+-rw-r--r--   0 root         (0) root         (0)      951 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/apps.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/iam_migration/templates/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/templates/migration.tmpl
+-rw-r--r--   0 root         (0) root         (0)      845 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/iam_migration/utils/
+-rw-r--r--   0 root         (0) root         (0)    25878 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/utils/do_migrate.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/migrator.py
+-rw-r--r--   0 root         (0) root         (0)      818 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/iam_migration/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/iam_migration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     3756 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/management/commands/iam_makemigrations.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/iam_migration/migrations/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/iam_migration/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/django/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/django/dispatcher/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/django/dispatcher/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9908 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/django/dispatcher/dispatchers.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/django/dispatcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/django/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/django/response.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/django/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/converter/
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/converter/base.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/converter/queryset.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/converter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5814 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/converter/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/contrib/tastypie/
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/tastypie/resource.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/tastypie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/tastypie/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/tastypie/shortcuts.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/contrib/http.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/resource/
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/resource/provider.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/resource/constants.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/resource/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/resource/utils.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/resource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/iam/auth/
+-rw-r--r--   0 root         (0) root         (0)    14884 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/auth/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-03-07 02:07:52.000000 bk-iam-1.3.1/iam/cache.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 03:01:19.000000 bk-iam-1.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      194 2023-03-07 02:07:52.000000 bk-iam-1.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-03-07 02:07:52.000000 bk-iam-1.3.1/readme_en.md
+-rw-r--r--   0 root         (0) root         (0)      220 2023-03-07 02:07:52.000000 bk-iam-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-15 03:01:19.000000 bk-iam-1.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-03-07 02:07:52.000000 bk-iam-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:01:19.000000 bk-iam-1.3.1/bk_iam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-05-15 03:01:19.000000 bk-iam-1.3.1/bk_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 03:01:19.000000 bk-iam-1.3.1/bk_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-15 03:01:19.000000 bk-iam-1.3.1/bk_iam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-15 03:01:19.000000 bk-iam-1.3.1/bk_iam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-15 03:01:19.000000 bk-iam-1.3.1/bk_iam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-03-07 03:43:00.000000 bk-iam-1.3.1/readme.md
```

### Comparing `bk-iam-1.2.2/PKG-INFO` & `bk-iam-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: bk-iam
-Version: 1.2.2
+Version: 1.3.1
 Summary: bk-iam python sdk
 Home-page: https://github.com/TencentBlueKing/iam-python-sdk
 Author: TencentBlueKing
 Author-email: contactus_bk@tencent.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/TencentBlueKing/iam-python-sdk/issues
-Description: bk-iam python sdk
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4
 Description-Content-Type: text/markdown
+
+bk-iam python sdk
+
```

### Comparing `bk-iam-1.2.2/bk_iam.egg-info/PKG-INFO` & `bk-iam-1.3.1/bk_iam.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: bk-iam
-Version: 1.2.2
+Version: 1.3.1
 Summary: bk-iam python sdk
 Home-page: https://github.com/TencentBlueKing/iam-python-sdk
 Author: TencentBlueKing
 Author-email: contactus_bk@tencent.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/TencentBlueKing/iam-python-sdk/issues
-Description: bk-iam python sdk
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4
 Description-Content-Type: text/markdown
+
+bk-iam python sdk
+
```

### Comparing `bk-iam-1.2.2/bk_iam.egg-info/SOURCES.txt` & `bk-iam-1.3.1/bk_iam.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.txt
 MANIFEST.in
 pyproject.toml
 readme.md
 readme_en.md
 setup.py
 bk_iam.egg-info/PKG-INFO
 bk_iam.egg-info/SOURCES.txt
```

### Comparing `bk-iam-1.2.2/iam/__init__.py` & `bk-iam-1.3.1/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/api/__init__.py` & `bk-iam-1.3.1/iam/api/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/api/client.py` & `bk-iam-1.3.1/iam/api/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,19 +55,21 @@
             if not (bk_iam_host and bk_paas_host):
                 raise AuthAPIError("init client fail, bk_iam_host and bk_paas_host should not be empty")
 
             self._host = bk_iam_host
             self._bk_paas_host = bk_paas_host
 
         # will add ?debug=true in url, for debug api/policy, show the details
-        is_api_debug_enabled = (os.environ.get("IAM_API_DEBUG") == "true"
-                                or os.environ.get("BKAPP_IAM_API_DEBUG") == "true")
+        is_api_debug_enabled = (
+            os.environ.get("IAM_API_DEBUG") == "true" or os.environ.get("BKAPP_IAM_API_DEBUG") == "true"
+        )
         # will add ?force=true in url, for api/policy run without cache(all data from database)
-        is_api_force_enabled = (os.environ.get("IAM_API_FORCE") == "true"
-                                or os.environ.get("BKAPP_IAM_API_FORCE") == "true")
+        is_api_force_enabled = (
+            os.environ.get("IAM_API_FORCE") == "true" or os.environ.get("BKAPP_IAM_API_FORCE") == "true"
+        )
 
         self._extra_url_params = {}
         if is_api_debug_enabled:
             self._extra_url_params["debug"] = "true"
         if is_api_force_enabled:
             self._extra_url_params["force"] = "true"
 
@@ -318,19 +320,30 @@
 
     # --------- policy
     def policy_query(self, data):
         path = "/api/v1/policy/query"
         ok, message, data = self._call_iam_api(http_post, path, data)
         return ok, message, data
 
+    # --------- policy v2
+    def v2_policy_query(self, system_id, data):
+        path = f"/api/v2/policy/systems/{system_id}/query/"
+        ok, message, data = self._call_iam_api(http_post, path, data)
+        return ok, message, data
+
     def policy_query_by_actions(self, data):
         path = "/api/v1/policy/query_by_actions"
         ok, message, data = self._call_iam_api(http_post, path, data)
         return ok, message, data
 
+    def v2_policy_query_by_actions(self, system_id, data):
+        path = f"/api/v2/policy/systems/{system_id}/query_by_actions/"
+        ok, message, data = self._call_iam_api(http_post, path, data)
+        return ok, message, data
+
     def get_token(self, system_id):
         path = "/api/v1/model/systems/{system_id}/token".format(system_id=system_id)
         ok, message, _data = self._call_iam_api(http_get, path, {})
         if not ok:
             return False, message, ""
 
         return True, "success", _data.get("token", "")
```

### Comparing `bk-iam-1.2.2/iam/api/http.py` & `bk-iam-1.3.1/iam/api/http.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/apply/__init__.py` & `bk-iam-1.3.1/iam/objects.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/apply/models.py` & `bk-iam-1.3.1/iam/apply/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/auth/__init__.py` & `bk-iam-1.3.1/iam/apply/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/auth/models.py` & `bk-iam-1.3.1/iam/auth/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/cache.py` & `bk-iam-1.3.1/iam/cache.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/collection.py` & `bk-iam-1.3.1/iam/collection.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/__init__.py` & `bk-iam-1.3.1/iam/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/converter/__init__.py` & `bk-iam-1.3.1/iam/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/converter/base.py` & `bk-iam-1.3.1/iam/contrib/converter/base.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/converter/queryset.py` & `bk-iam-1.3.1/iam/contrib/converter/queryset.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/converter/sql.py` & `bk-iam-1.3.1/iam/contrib/converter/sql.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/django/__init__.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/django/dispatcher/__init__.py` & `bk-iam-1.3.1/iam/contrib/django/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/django/dispatcher/dispatchers.py` & `bk-iam-1.3.1/iam/contrib/django/dispatcher/dispatchers.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/django/dispatcher/exceptions.py` & `bk-iam-1.3.1/iam/contrib/django/dispatcher/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/django/middlewares.py` & `bk-iam-1.3.1/iam/contrib/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/django/response.py` & `bk-iam-1.3.1/iam/contrib/django/response.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/http.py` & `bk-iam-1.3.1/iam/contrib/http.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/__init__.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/apps.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/apps.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/conf.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/conf.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/constants.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/exceptions.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/management/__init__.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/management/commands/__init__.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/management/commands/iam_makemigrations.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/management/commands/iam_makemigrations.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/migrations/__init__.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/migrator.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/migrator.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/template.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/template.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/templates/migration.tmpl` & `bk-iam-1.3.1/iam/contrib/iam_migration/templates/migration.tmpl`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/utils/__init__.py` & `bk-iam-1.3.1/iam/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/iam_migration/utils/do_migrate.py` & `bk-iam-1.3.1/iam/contrib/iam_migration/utils/do_migrate.py`

 * *Files 9% similar despite different names*

```diff
@@ -203,14 +203,17 @@
         "upsert_resource_creator_actions": "update_resource_creator_actions",
         "add_common_actions": "add_common_actions",
         "update_common_actions": "update_common_actions",
         "upsert_common_actions": "update_common_actions",
         "add_feature_shield_rules": "add_feature_shield_rules",
         "update_feature_shield_rules": "update_feature_shield_rules",
         "upsert_feature_shield_rules": "update_feature_shield_rules",
+        "add_custom_frontend_settings": "add_custom_frontend_settings",
+        "update_custom_frontend_settings": "update_custom_frontend_settings",
+        "upsert_custom_frontend_settings": "update_custom_frontend_settings"
     }
 
     """
     index:
     - Add system
     - Update system
 
@@ -335,14 +338,25 @@
         return ok, message
 
     def api_update_feature_shield_rules(self, system_id, data):
         path = "/api/v1/model/systems/{system_id}/configs/feature_shield_rules".format(system_id=system_id)
         ok, message, data = self._call_iam_api(http_put, path, data)
         return ok, message
 
+    # ---------- custom_frontend_settings
+    def api_add_custom_frontend_settings(self, system_id, data):
+        path = "/api/v1/model/systems/{system_id}/configs/custom_frontend_settings".format(system_id=system_id)
+        ok, message, data = self._call_iam_api(http_post, path, data)
+        return ok, message
+
+    def api_update_custom_frontend_settings(self, system_id, data):
+        path = "/api/v1/model/systems/{system_id}/configs/custom_frontend_settings".format(system_id=system_id)
+        ok, message, data = self._call_iam_api(http_put, path, data)
+        return ok, message
+
     # ---------- query
 
     def api_query(self, system_id):
         path = "/api/v1/model/systems/{system_id}/query".format(system_id=system_id)
         ok, message, data = self._call_iam_api(http_get, path, None)
         return ok, message, data
 
@@ -462,14 +476,20 @@
 
     def add_feature_shield_rules(self, system_id, data):
         return self.api_add_feature_shield_rules(system_id, data)
 
     def update_feature_shield_rules(self, system_id, data):
         return self.api_update_feature_shield_rules(system_id, data)
 
+    def add_custom_frontend_settings(self, system_id, data):
+        return self.api_add_custom_frontend_settings(system_id, data)
+
+    def update_custom_frontend_settings(self, system_id, data):
+        return self.api_update_custom_frontend_settings(system_id, data)
+
     def upsert_system(self, system_id, data):
         if system_id not in self.system_id_set:
             return self.add_system(system_id, data)
         return self.update_system(system_id, data)
 
     def upsert_resource_type(self, system_id, data):
         d_resource_type_id = data.get("id")
```

### Comparing `bk-iam-1.2.2/iam/contrib/tastypie/__init__.py` & `bk-iam-1.3.1/iam/contrib/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/tastypie/authorization.py` & `bk-iam-1.3.1/iam/contrib/tastypie/authorization.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/tastypie/resource.py` & `bk-iam-1.3.1/iam/contrib/tastypie/resource.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/contrib/tastypie/shortcuts.py` & `bk-iam-1.3.1/iam/contrib/tastypie/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/dummy_iam.py` & `bk-iam-1.3.1/iam/dummy_iam.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/eval/__init__.py` & `bk-iam-1.3.1/iam/contrib/tastypie/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/eval/constants.py` & `bk-iam-1.3.1/iam/eval/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/eval/expression.py` & `bk-iam-1.3.1/iam/eval/expression.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/eval/object.py` & `bk-iam-1.3.1/iam/eval/object.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/eval/operators.py` & `bk-iam-1.3.1/iam/eval/operators.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/exceptions.py` & `bk-iam-1.3.1/iam/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/iam.py` & `bk-iam-1.3.1/iam/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,35 +33,42 @@
 
 
 class IAM(object):
     """
     input: object
     """
 
-    def __init__(self, app_code, app_secret, bk_iam_host=None, bk_paas_host=None, bk_apigateway_url=None):
+    def __init__(
+        self, app_code, app_secret, bk_iam_host=None, bk_paas_host=None, bk_apigateway_url=None, api_version="v2"
+    ):
         """
         如果有 APIGateway 且权限中心网关接入, 则可以统一API请求全部走APIGateway
         - 没有APIGateway的用法: IAM(app_code, app_secret, bk_iam_host, bk_paas_host)
         - 有APIGateway的用法: IAM(app_code, app_secret, bk_apigateway_url)
 
         NOTE: 未来将会下线`没有 APIGateway的用法`
         TODO: 切换后, 所有暴露接口将不再依赖 bk_token/bk_username, 需考虑兼容调用方, 并文档说明
         """
         self._client = Client(app_code, app_secret, bk_iam_host, bk_paas_host, bk_apigateway_url)
 
+        self._api_version = api_version
+
     def _do_policy_query(self, request, with_resources=True):
         data = request.to_dict()
         logger.debug("the request: %s", data)
 
         # NOTE: 不向服务端传任何resource, 用于统一类资源的批量鉴权
         # 将会返回所有策略, 然后遍历资源列表和策略列表, 逐一计算
         if not with_resources:
             data["resources"] = []
 
-        ok, message, policies = self._client.policy_query(data)
+        if self._api_version == "v2":
+            ok, message, policies = self._client.v2_policy_query(request.system, data)
+        else:
+            ok, message, policies = self._client.policy_query(data)
         if not ok:
             raise AuthAPIError(message)
         return policies
 
     @cached(cache=TTLCache(maxsize=1024, ttl=60), key=hash_key)
     def _do_policy_query_with_cache(self, request):
         return self._do_policy_query(request)
@@ -71,15 +78,18 @@
         logger.debug("the request: %s", data)
 
         # NOTE: 不向服务端传任何resource, 用于统一类资源的批量鉴权
         # 将会返回所有策略, 然后遍历资源列表和策略列表, 逐一计算
         if not with_resources:
             data["resources"] = []
 
-        ok, message, action_policies = self._client.policy_query_by_actions(data)
+        if self._api_version == "v2":
+            ok, message, action_policies = self._client.v2_policy_query_by_actions(request.system, data)
+        else:
+            ok, message, action_policies = self._client.policy_query_by_actions(data)
         if not ok:
             raise AuthAPIError(message)
         return action_policies
 
     def _eval_expr(self, expr, obj_set):
         logger.debug("the return expr: %s", expr.expr())
         logger.debug("the return expr render: %s", expr.render(obj_set))
@@ -397,15 +407,15 @@
         # 4. do convert and return
         converted_filters = c.convert(policies)
         logger.debug("the converted filters: %s", converted_filters)
         return converted_filters
 
     # TODO: add the register model apis
     def get_token(self, system):
-        """ 获取token
+        """获取token
         return bool, message, token
         """
         return self._client.get_token(system)
 
     def is_basic_auth_allowed(self, system, basic_auth):
         logger.debug("calling IAM.is_basic_auth_allowed(basic_aut)......")
```

### Comparing `bk-iam-1.2.2/iam/meta.py` & `bk-iam-1.3.1/iam/meta.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/model/__init__.py` & `bk-iam-1.3.1/iam/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/model/models.py` & `bk-iam-1.3.1/iam/model/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/objects.py` & `bk-iam-1.3.1/iam/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/resource/__init__.py` & `bk-iam-1.3.1/iam/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/resource/constants.py` & `bk-iam-1.3.1/iam/resource/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/resource/dispatcher.py` & `bk-iam-1.3.1/iam/resource/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/resource/provider.py` & `bk-iam-1.3.1/iam/resource/provider.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/resource/utils.py` & `bk-iam-1.3.1/iam/resource/utils.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/shortcuts.py` & `bk-iam-1.3.1/iam/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/iam/utils.py` & `bk-iam-1.3.1/iam/utils.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/readme.md` & `bk-iam-1.3.1/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 - [TencentBlueKing/bk-iam](https://github.com/TencentBlueKing/bk-iam)
 - [TencentBlueKing/bk-iam-saas](https://github.com/TencentBlueKing/bk-iam-saas)
 - [TencentBlueKing/bk-iam-search-engine](https://github.com/TencentBlueKing/bk-iam-search-engine)
 - [TencentBlueKing/bk-iam-cli](https://github.com/TencentBlueKing/bk-iam-cli)
 - [TencentBlueKing/iam-python-sdk](https://github.com/TencentBlueKing/iam-python-sdk)
 - [TencentBlueKing/iam-go-sdk](https://github.com/TencentBlueKing/iam-go-sdk)
 - [TencentBlueKing/iam-php-sdk](https://github.com/TencentBlueKing/iam-php-sdk)
+- [TencentBlueKing/iam-java-sdk](https://github.com/TencentBlueKing/iam-java-sdk)
 
 ## Support
 
 - [蓝鲸论坛](https://bk.tencent.com/s-mart/community)
 - [蓝鲸 DevOps 在线视频教程](https://bk.tencent.com/s-mart/video/)
 - 联系我们，技术交流QQ群：
```

### Comparing `bk-iam-1.2.2/readme_en.md` & `bk-iam-1.3.1/readme_en.md`

 * *Files identical despite different names*

### Comparing `bk-iam-1.2.2/setup.py` & `bk-iam-1.3.1/setup.py`

 * *Files identical despite different names*

