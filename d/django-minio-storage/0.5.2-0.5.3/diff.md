# Comparing `tmp/django-minio-storage-0.5.2.tar.gz` & `tmp/django-minio-storage-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-minio-storage-0.5.2.tar", last modified: Sat May  6 04:01:56 2023, max compression
+gzip compressed data, was "django-minio-storage-0.5.3.tar", last modified: Mon May 15 18:27:11 2023, max compression
```

## Comparing `django-minio-storage-0.5.2.tar` & `django-minio-storage-0.5.3.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.595380 django-minio-storage-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.flake8rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.579380 django-minio-storage-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.583380 django-minio-storage-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 04:01:56.595380 django-minio-storage-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.587380 django-minio-storage-0.5.2/django_minio_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.587380 django-minio-storage-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/contributors.md
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/licences.md
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.587380 django-minio-storage-0.5.2/minio_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.587380 django-minio-storage-0.5.2/minio_storage/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/minio_storage/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/management/commands/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/minio_storage/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 04:01:56.595380 django-minio-storage-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/tests/django_minio_storage_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/django_minio_storage_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/django_minio_storage_tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/django_minio_storage_tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/django_minio_storage_tests/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/tests/test_app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/bucket_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/custom_storage_class_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/managementcommand_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/retrieve_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/upload_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/watermelon-cat.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.flake8rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.310950 django-minio-storage-0.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.314951 django-minio-storage-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.314951 django-minio-storage-0.5.3/django_minio_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.314951 django-minio-storage-0.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/licences.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/minio_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/minio_storage/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/minio_storage/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/management/commands/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/minio_storage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/tests/django_minio_storage_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/django_minio_storage_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/django_minio_storage_tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/django_minio_storage_tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/django_minio_storage_tests/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/tests/test_app/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/bucket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/custom_storage_class_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/managementcommand_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/retrieve_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/upload_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/watermelon-cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tox.ini
```

### Comparing `django-minio-storage-0.5.2/.github/workflows/release.yml` & `django-minio-storage-0.5.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/.github/workflows/tox.yml` & `django-minio-storage-0.5.3/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/CHANGELOG.md` & `django-minio-storage-0.5.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/LICENSE-APACHE` & `django-minio-storage-0.5.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/LICENSE-MIT` & `django-minio-storage-0.5.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/PKG-INFO` & `django-minio-storage-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.2
+Version: 0.5.3
 Summary: Django file storage using the minio python client
 Home-page: https://github.com/py-pa/django-minio-storage
-Author: Tom Houlé
-Author-email: tom@kafunsho.be
+Author: Thomas Frössman
+Author-email: thomasf@jossystem.se
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `django-minio-storage-0.5.2/README.md` & `django-minio-storage-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/django_minio_storage.egg-info/PKG-INFO` & `django-minio-storage-0.5.3/django_minio_storage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.2
+Version: 0.5.3
 Summary: Django file storage using the minio python client
 Home-page: https://github.com/py-pa/django-minio-storage
-Author: Tom Houlé
-Author-email: tom@kafunsho.be
+Author: Thomas Frössman
+Author-email: thomasf@jossystem.se
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `django-minio-storage-0.5.2/django_minio_storage.egg-info/SOURCES.txt` & `django-minio-storage-0.5.3/django_minio_storage.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 .github/workflows/tox.yml
 django_minio_storage.egg-info/PKG-INFO
 django_minio_storage.egg-info/SOURCES.txt
 django_minio_storage.egg-info/dependency_links.txt
 django_minio_storage.egg-info/requires.txt
 django_minio_storage.egg-info/top_level.txt
 docs/contributing.md
-docs/contributors.md
 docs/development.md
 docs/index.md
 docs/licences.md
 docs/usage.md
 minio_storage/__init__.py
 minio_storage/apps.py
 minio_storage/errors.py
```

### Comparing `django-minio-storage-0.5.2/docs/development.md` & `django-minio-storage-0.5.3/docs/development.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-## Running tests
+## Testing strategy
+
+Test coverage is and should remain near 100%.
 
-Test coverage is and should remain 100%. The library is very small and a minio
-server can be very easily brought up with docker, so there is no reason to use
-mocking most of the time, the tests should run directly against a real minio
-instance.
+This package is very small and a minio server can be very easily brought up
+with docker so there is typically no reason to use mocking at all. The tests
+should run directly against a real minio server instance.
+
+## Running tests
 
 To run the tests you need to have minio running locally with some specific
 settings, you can start it using docker-compose:
 
 ```sh
 docker-compose up -d
 ```
```

### Comparing `django-minio-storage-0.5.2/docs/licences.md` & `django-minio-storage-0.5.3/docs/licences.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/docs/usage.md` & `django-minio-storage-0.5.3/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/minio_storage/files.py` & `django-minio-storage-0.5.3/minio_storage/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             self.file.release_conn()
 
 
 class ReadOnlySpooledTemporaryFile(MinioStorageFile, ReadOnlyMixin):
     """A django File class which buffers the minio object into a local
     SpooledTemporaryFile."""
 
-    max_memory_size: int = 1024 * 1024 * 10
+    max_memory_size: int = 10 * 1024 * 1024
 
     def __init__(
         self,
         name: str,
         mode: str,
         storage: "MinioStorage",
         max_memory_size: T.Optional[int] = None,
```

### Comparing `django-minio-storage-0.5.2/minio_storage/management/commands/minio.py` & `django-minio-storage-0.5.3/minio_storage/management/commands/minio.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/minio_storage/policy.py` & `django-minio-storage-0.5.3/minio_storage/policy.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/minio_storage/storage.py` & `django-minio-storage-0.5.3/minio_storage/storage.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/setup.py` & `django-minio-storage-0.5.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,16 @@
         "write_to": "minio_storage/version.py",
         "write_to_template": '__version__ = "{version}"\n',
         "tag_regex": r"^v(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$",
     },
     description="Django file storage using the minio python client",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author="Tom Houlé",
-    author_email="tom@kafunsho.be",
+    author="Thomas Frössman",
+    author_email="thomasf@jossystem.se",
     url="https://github.com/py-pa/django-minio-storage",
     packages=[
         "minio_storage",
         "minio_storage/management/",
         "minio_storage/management/commands/",
     ],
     setup_requires=["setuptools_scm"],
```

### Comparing `django-minio-storage-0.5.2/tests/django_minio_storage_tests/settings.py` & `django-minio-storage-0.5.3/tests/django_minio_storage_tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tests/django_minio_storage_tests/urls.py` & `django-minio-storage-0.5.3/tests/django_minio_storage_tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tests/test_app/tests/bucket_tests.py` & `django-minio-storage-0.5.3/tests/test_app/tests/bucket_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tests/test_app/tests/custom_storage_class_tests.py` & `django-minio-storage-0.5.3/tests/test_app/tests/custom_storage_class_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tests/test_app/tests/delete_tests.py` & `django-minio-storage-0.5.3/tests/test_app/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tests/test_app/tests/managementcommand_tests.py` & `django-minio-storage-0.5.3/tests/test_app/tests/managementcommand_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tests/test_app/tests/retrieve_tests.py` & `django-minio-storage-0.5.3/tests/test_app/tests/retrieve_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tests/test_app/tests/upload_tests.py` & `django-minio-storage-0.5.3/tests/test_app/tests/upload_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tests/test_app/tests/utils.py` & `django-minio-storage-0.5.3/tests/test_app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tests/watermelon-cat.jpg` & `django-minio-storage-0.5.3/tests/watermelon-cat.jpg`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.2/tox.ini` & `django-minio-storage-0.5.3/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,17 @@
     coverage html
 depends=py311-django42-minioknown
 
 [testenv:pyright]
 basepython = python3
 deps =
         pyright
-        django-stubs==4.2.0
+        minio
+        django-stubs==4.2.*
+        Django==4.2.*
         -rdev-requirements.txt
 commands =
     pyright --level WARNING
 
 
 [testenv:lint]
 setenv=
```

