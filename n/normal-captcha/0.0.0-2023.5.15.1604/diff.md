# Comparing `tmp/normal_captcha-0.0.0.tar.gz` & `tmp/normal_captcha-2023.5.15.1604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normal_captcha-0.0.0.tar", last modified: Mon May 15 14:38:26 2023, max compression
+gzip compressed data, was "normal_captcha-2023.5.15.1604.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `normal_captcha-0.0.0.tar` & `normal_captcha-2023.5.15.1604.tar`

### file list

```diff
@@ -1,21 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:38:26.095462 normal_captcha-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:38:26.091462 normal_captcha-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:38:26.091462 normal_captcha-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-15 14:38:14.000000 normal_captcha-0.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 14:38:14.000000 normal_captcha-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 14:38:26.095462 normal_captcha-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-15 14:38:14.000000 normal_captcha-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:38:26.091462 normal_captcha-0.0.0/nomal_captcha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:38:14.000000 normal_captcha-0.0.0/nomal_captcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-15 14:38:14.000000 normal_captcha-0.0.0/nomal_captcha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:38:26.095462 normal_captcha-0.0.0/normal_captcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 14:38:26.000000 normal_captcha-0.0.0/normal_captcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-15 14:38:26.000000 normal_captcha-0.0.0/normal_captcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:38:26.000000 normal_captcha-0.0.0/normal_captcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 14:38:26.000000 normal_captcha-0.0.0/normal_captcha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-15 14:38:26.000000 normal_captcha-0.0.0/normal_captcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 14:38:26.000000 normal_captcha-0.0.0/normal_captcha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 14:38:14.000000 normal_captcha-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-15 14:38:14.000000 normal_captcha-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 14:38:14.000000 normal_captcha-0.0.0/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:38:26.095462 normal_captcha-0.0.0/setup.cfg
+-rw-r--r--   0        0        0      189 2023-05-15 16:04:17.789279 normal_captcha-2023.5.15.1604/README.md
+-rw-r--r--   0        0        0       79 2023-05-15 16:04:17.789279 normal_captcha-2023.5.15.1604/normal_captcha/__init__.py
+-rw-r--r--   0        0        0      473 2023-05-15 16:04:17.789279 normal_captcha-2023.5.15.1604/normal_captcha/main.py
+-rw-r--r--   0        0        0      536 2023-05-15 16:04:17.793279 normal_captcha-2023.5.15.1604/pyproject.toml
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 normal_captcha-2023.5.15.1604/PKG-INFO
```

