# Comparing `tmp/wiki-0.8.2.tar.gz` & `tmp/wiki-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiki-0.8.2.tar", last modified: Sat May  7 21:19:57 2022, max compression
+gzip compressed data, was "wiki-0.9.tar", last modified: Mon Jun 27 20:39:37 2022, max compression
```

## Comparing `wiki-0.8.2.tar` & `wiki-0.9.tar`

### file list

```diff
@@ -1,664 +1,664 @@
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.788533 wiki-0.8.2/
--rw-r--r--   0 balder    (1000) balder    (1000)    35143 2013-11-18 22:19:29.000000 wiki-0.8.2/COPYING
--rw-rw-r--   0 balder    (1000) balder    (1000)      281 2020-10-27 22:37:04.000000 wiki-0.8.2/MANIFEST.in
--rw-rw-r--   0 balder    (1000) balder    (1000)    12878 2022-05-07 21:19:57.788533 wiki-0.8.2/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)     9627 2022-02-14 21:10:11.000000 wiki-0.8.2/README.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)      295 2022-05-07 21:19:57.788533 wiki-0.8.2/setup.cfg
--rw-rw-r--   0 balder    (1000) balder    (1000)     3260 2022-05-07 21:00:18.000000 wiki-0.8.2/setup.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.696532 wiki-0.8.2/src/wiki/
--rw-rw-r--   0 balder    (1000) balder    (1000)      884 2022-05-07 21:19:50.000000 wiki-0.8.2/src/wiki/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     3027 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/admin.py
--rw-r--r--   0 balder    (1000) balder    (1000)      862 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/apps.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     4399 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/checks.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.696532 wiki-0.8.2/src/wiki/conf/
--rw-r--r--   0 balder    (1000) balder    (1000)        0 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/conf/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)    11603 2021-10-25 21:21:54.000000 wiki-0.8.2/src/wiki/conf/settings.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.696532 wiki-0.8.2/src/wiki/core/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/core/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      272 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/core/diff.py
--rw-r--r--   0 balder    (1000) balder    (1000)      162 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/core/exceptions.py
--rw-r--r--   0 balder    (1000) balder    (1000)     1705 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/core/http.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.696532 wiki-0.8.2/src/wiki/core/markdown/
--rw-rw-r--   0 balder    (1000) balder    (1000)     3918 2022-02-14 21:10:09.000000 wiki-0.8.2/src/wiki/core/markdown/__init__.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/core/markdown/mdx/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/core/markdown/mdx/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     4523 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/core/markdown/mdx/codehilite.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      839 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/core/markdown/mdx/previewlinks.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1797 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/core/markdown/mdx/responsivetable.py
--rw-r--r--   0 balder    (1000) balder    (1000)     1055 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/core/paginator.py
--rw-r--r--   0 balder    (1000) balder    (1000)     3032 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/core/permissions.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/core/plugins/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/core/plugins/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)     2039 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/core/plugins/base.py
--rw-r--r--   0 balder    (1000) balder    (1000)      128 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/core/plugins/loader.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     2013 2022-02-14 21:10:09.000000 wiki-0.8.2/src/wiki/core/plugins/registry.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      355 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/core/utils.py
--rw-r--r--   0 balder    (1000) balder    (1000)     4006 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/core/version.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     6823 2021-04-06 21:41:39.000000 wiki-0.8.2/src/wiki/decorators.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/editors/
--rw-r--r--   0 balder    (1000) balder    (1000)      368 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/editors/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)      585 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/editors/base.py
--rw-r--r--   0 balder    (1000) balder    (1000)     1579 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/editors/markitup.py
--rw-rw-r--   0 balder    (1000) balder    (1000)    22009 2022-05-07 21:00:18.000000 wiki-0.8.2/src/wiki/forms.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     3103 2021-12-28 23:42:50.000000 wiki-0.8.2/src/wiki/forms_account_handling.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/ca/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)      380 2021-02-28 12:24:18.000000 wiki-0.8.2/src/wiki/locale/ca/LC_MESSAGES/django.mo
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/cs/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    44514 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/cs/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    67826 2021-04-10 18:00:16.000000 wiki-0.8.2/src/wiki/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/da/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/locale/da/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    43486 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/da/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    66844 2021-04-10 18:00:33.000000 wiki-0.8.2/src/wiki/locale/da/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/de/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/locale/de/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    45256 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    68744 2021-04-10 18:00:40.000000 wiki-0.8.2/src/wiki/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/el/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/locale/el/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    14057 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/el/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    56967 2021-04-10 18:00:15.000000 wiki-0.8.2/src/wiki/locale/el/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/en/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/locale/en/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    49600 2021-02-28 12:24:18.000000 wiki-0.8.2/src/wiki/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/es/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.700532 wiki-0.8.2/src/wiki/locale/es/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    40147 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    66047 2021-04-10 18:00:49.000000 wiki-0.8.2/src/wiki/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/fi/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.704532 wiki-0.8.2/src/wiki/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    33339 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    62592 2021-04-10 18:00:16.000000 wiki-0.8.2/src/wiki/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/fr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.704532 wiki-0.8.2/src/wiki/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    46271 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    69950 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.676531 wiki-0.8.2/src/wiki/locale/hu/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.704532 wiki-0.8.2/src/wiki/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    44201 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/hu/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    67354 2021-04-10 18:00:38.000000 wiki-0.8.2/src/wiki/locale/hu/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/it/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.704532 wiki-0.8.2/src/wiki/locale/it/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    19821 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    57427 2021-04-10 18:00:41.000000 wiki-0.8.2/src/wiki/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/ja/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.704532 wiki-0.8.2/src/wiki/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    49498 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    72735 2021-04-10 18:00:20.000000 wiki-0.8.2/src/wiki/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/ko_KR/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.704532 wiki-0.8.2/src/wiki/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    46093 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/ko_KR/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    69523 2021-04-10 18:00:32.000000 wiki-0.8.2/src/wiki/locale/ko_KR/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/nb_NO/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.704532 wiki-0.8.2/src/wiki/locale/nb_NO/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     8946 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/nb_NO/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    52370 2021-04-10 18:00:31.000000 wiki-0.8.2/src/wiki/locale/nb_NO/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/nl/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.708532 wiki-0.8.2/src/wiki/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    45086 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    68402 2021-04-10 18:00:38.000000 wiki-0.8.2/src/wiki/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/pl_PL/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.708532 wiki-0.8.2/src/wiki/locale/pl_PL/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    45424 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/pl_PL/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    68758 2021-04-10 18:00:41.000000 wiki-0.8.2/src/wiki/locale/pl_PL/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/pt/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.708532 wiki-0.8.2/src/wiki/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    31813 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    62198 2021-04-10 18:00:31.000000 wiki-0.8.2/src/wiki/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/pt_BR/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.708532 wiki-0.8.2/src/wiki/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    44456 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    67805 2021-04-10 18:00:18.000000 wiki-0.8.2/src/wiki/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/pt_PT/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.708532 wiki-0.8.2/src/wiki/locale/pt_PT/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    31813 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/pt_PT/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    62198 2021-04-10 18:00:31.000000 wiki-0.8.2/src/wiki/locale/pt_PT/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/ro/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.708532 wiki-0.8.2/src/wiki/locale/ro/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    34462 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/ro/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    63439 2021-04-10 18:00:48.000000 wiki-0.8.2/src/wiki/locale/ro/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/ru/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.708532 wiki-0.8.2/src/wiki/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    58484 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    82146 2021-04-10 18:00:33.000000 wiki-0.8.2/src/wiki/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/sk/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.708532 wiki-0.8.2/src/wiki/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    39855 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/sk/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    65886 2021-04-10 18:00:50.000000 wiki-0.8.2/src/wiki/locale/sk/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/sv/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.708532 wiki-0.8.2/src/wiki/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    19807 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    57605 2021-04-10 18:00:51.000000 wiki-0.8.2/src/wiki/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/tr_TR/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.712532 wiki-0.8.2/src/wiki/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    44807 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/tr_TR/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    68115 2021-04-10 18:00:52.000000 wiki-0.8.2/src/wiki/locale/tr_TR/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/zh_CN/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.712532 wiki-0.8.2/src/wiki/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    40469 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/zh_CN/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    64017 2021-04-10 18:00:50.000000 wiki-0.8.2/src/wiki/locale/zh_CN/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/zh_Hans/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.712532 wiki-0.8.2/src/wiki/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    40469 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    64017 2021-04-10 18:00:50.000000 wiki-0.8.2/src/wiki/locale/zh_Hans/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/locale/zh_TW/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.712532 wiki-0.8.2/src/wiki/locale/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)    13263 2021-04-10 18:13:29.000000 wiki-0.8.2/src/wiki/locale/zh_TW/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)    54075 2021-04-10 18:00:17.000000 wiki-0.8.2/src/wiki/locale/zh_TW/LC_MESSAGES/django.po
--rw-rw-r--   0 balder    (1000) balder    (1000)     5264 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/managers.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.712532 wiki-0.8.2/src/wiki/migrations/
--rw-rw-r--   0 balder    (1000) balder    (1000)    16991 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/migrations/0001_initial.py
--rw-r--r--   0 balder    (1000) balder    (1000)      732 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/migrations/0002_urlpath_moved_to.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1321 2022-02-14 21:10:11.000000 wiki-0.8.2/src/wiki/migrations/0003_mptt_upgrade.py
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/migrations/__init__.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.712532 wiki-0.8.2/src/wiki/models/
--rw-rw-r--   0 balder    (1000) balder    (1000)     1599 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/models/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)    17707 2022-02-14 21:10:09.000000 wiki-0.8.2/src/wiki/models/article.py
--rw-rw-r--   0 balder    (1000) balder    (1000)    11298 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/models/pluginbase.py
--rw-rw-r--   0 balder    (1000) balder    (1000)    14406 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/models/urlpath.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.712532 wiki-0.8.2/src/wiki/plugins/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/__init__.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.716532 wiki-0.8.2/src/wiki/plugins/attachments/
--rw-r--r--   0 balder    (1000) balder    (1000)       71 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/attachments/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)      349 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/attachments/admin.py
--rw-r--r--   0 balder    (1000) balder    (1000)      237 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/attachments/apps.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     6159 2021-12-28 23:42:50.000000 wiki-0.8.2/src/wiki/plugins/attachments/forms.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     3658 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/plugins/attachments/markdown_extensions.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.716532 wiki-0.8.2/src/wiki/plugins/attachments/migrations/
--rw-rw-r--   0 balder    (1000) balder    (1000)     4838 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/attachments/migrations/0001_initial.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      493 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/attachments/migrations/0002_auto_20151118_1816.py
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/attachments/migrations/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     7500 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/attachments/models.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     3532 2021-01-11 06:47:50.000000 wiki-0.8.2/src/wiki/plugins/attachments/settings.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/attachments/templates/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.716532 wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/
--rw-r--r--   0 balder    (1000) balder    (1000)     2208 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/delete.html
--rw-r--r--   0 balder    (1000) balder    (1000)     2132 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/history.html
--rw-r--r--   0 balder    (1000) balder    (1000)     7123 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/index.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      420 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/render.html
--rw-r--r--   0 balder    (1000) balder    (1000)     2136 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/replace.html
--rw-rw-r--   0 balder    (1000) balder    (1000)     2719 2022-01-20 10:37:17.000000 wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/search.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1413 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/attachments/urls.py
--rw-rw-r--   0 balder    (1000) balder    (1000)    16508 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/attachments/views.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1440 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/attachments/wiki_plugin.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.716532 wiki-0.8.2/src/wiki/plugins/editsection/
--rw-r--r--   0 balder    (1000) balder    (1000)       71 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/editsection/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      238 2022-02-14 21:10:11.000000 wiki-0.8.2/src/wiki/plugins/editsection/apps.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     4200 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/plugins/editsection/markdown_extensions.py
--rw-r--r--   0 balder    (1000) balder    (1000)      577 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/editsection/settings.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     6986 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/editsection/views.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      640 2022-02-14 21:10:11.000000 wiki-0.8.2/src/wiki/plugins/editsection/wiki_plugin.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.716532 wiki-0.8.2/src/wiki/plugins/globalhistory/
--rw-r--r--   0 balder    (1000) balder    (1000)       75 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/globalhistory/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)      246 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/globalhistory/apps.py
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/globalhistory/forms.py
--rw-r--r--   0 balder    (1000) balder    (1000)        0 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/plugins/globalhistory/models.py
--rw-r--r--   0 balder    (1000) balder    (1000)       23 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/globalhistory/settings.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/globalhistory/templates/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/globalhistory/templates/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/globalhistory/templates/wiki/plugins/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.720532 wiki-0.8.2/src/wiki/plugins/globalhistory/templates/wiki/plugins/globalhistory/
--rw-r--r--   0 balder    (1000) balder    (1000)     4032 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/globalhistory/templates/wiki/plugins/globalhistory/globalhistory.html
--rw-r--r--   0 balder    (1000) balder    (1000)      205 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/globalhistory/templates/wiki/plugins/globalhistory/menubaritem.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1184 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/globalhistory/views.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      567 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/globalhistory/wiki_plugin.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.720532 wiki-0.8.2/src/wiki/plugins/help/
--rw-r--r--   0 balder    (1000) balder    (1000)       57 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/help/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)      209 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/help/apps.py
--rw-r--r--   0 balder    (1000) balder    (1000)        0 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/plugins/help/models.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/help/templates/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/help/templates/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/help/templates/wiki/plugins/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.720532 wiki-0.8.2/src/wiki/plugins/help/templates/wiki/plugins/help/
--rw-rw-r--   0 balder    (1000) balder    (1000)      966 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/help/templates/wiki/plugins/help/sidebar.html
--rw-rw-r--   0 balder    (1000) balder    (1000)       26 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/help/views.py
--rw-r--r--   0 balder    (1000) balder    (1000)      471 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/help/wiki_plugin.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.720532 wiki-0.8.2/src/wiki/plugins/images/
--rw-r--r--   0 balder    (1000) balder    (1000)       61 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/images/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)      935 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/images/admin.py
--rw-r--r--   0 balder    (1000) balder    (1000)      432 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/images/apps.py
--rw-r--r--   0 balder    (1000) balder    (1000)      398 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/images/checks.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     2376 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/images/forms.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     3430 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/plugins/images/markdown_extensions.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.720532 wiki-0.8.2/src/wiki/plugins/images/migrations/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2253 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/images/migrations/0001_initial.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      458 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/images/migrations/0002_auto_20151118_1811.py
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/migrations/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     5143 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/images/models.py
--rw-r--r--   0 balder    (1000) balder    (1000)     1684 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/images/settings.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.680532 wiki-0.8.2/src/wiki/plugins/images/static/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/images/static/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.720532 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.720532 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/
--rw-rw-r--   0 balder    (1000) balder    (1000)     4363 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/colorbox.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.724532 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/
--rw-rw-r--   0 balder    (1000) balder    (1000)      112 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/border.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     2893 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/controls.png
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.724532 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/
--rw-rw-r--   0 balder    (1000) balder    (1000)      111 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomCenter.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      215 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomLeft.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      217 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomRight.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      108 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderMiddleLeft.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      108 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderMiddleRight.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      111 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopCenter.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      216 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopLeft.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      214 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopRight.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     9427 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/loading.gif
--rw-rw-r--   0 balder    (1000) balder    (1000)      157 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/loading_background.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      182 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/overlay.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     5533 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/index.html
--rw-rw-r--   0 balder    (1000) balder    (1000)    11096 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/jquery.colorbox-min.js
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.724532 wiki-0.8.2/src/wiki/plugins/images/static/wiki/js/
--rw-rw-r--   0 balder    (1000) balder    (1000)      222 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/static/wiki/js/images.js
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/images/templates/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/images/templates/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.724532 wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/
--rw-rw-r--   0 balder    (1000) balder    (1000)     4407 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/index.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1140 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/purge.html
--rw-r--r--   0 balder    (1000) balder    (1000)      942 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/render.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1123 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/revision_add.html
--rw-r--r--   0 balder    (1000) balder    (1000)     6477 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/sidebar.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.724532 wiki-0.8.2/src/wiki/plugins/images/templatetags/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/images/templatetags/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      510 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/images/templatetags/wiki_images_tags.py
--rw-r--r--   0 balder    (1000) balder    (1000)       67 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/plugins/images/templatetags/wiki_thumbnails.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     7600 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/images/views.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     2770 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/images/wiki_plugin.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.724532 wiki-0.8.2/src/wiki/plugins/links/
--rw-r--r--   0 balder    (1000) balder    (1000)       59 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/links/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)      213 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/links/apps.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.724532 wiki-0.8.2/src/wiki/plugins/links/mdx/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/links/mdx/__init__.py
--rwxrwxr-x   0 balder    (1000) balder    (1000)     4938 2022-05-07 18:35:36.000000 wiki-0.8.2/src/wiki/plugins/links/mdx/djangowikilinks.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     5674 2022-05-07 18:35:36.000000 wiki-0.8.2/src/wiki/plugins/links/mdx/urlize.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       30 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/links/models.py
--rw-r--r--   0 balder    (1000) balder    (1000)      488 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/links/settings.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/links/templates/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/links/templates/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/links/templates/wiki/plugins/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.728532 wiki-0.8.2/src/wiki/plugins/links/templates/wiki/plugins/links/
--rw-r--r--   0 balder    (1000) balder    (1000)     1851 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/plugins/links/templates/wiki/plugins/links/sidebar.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1119 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/links/views.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1195 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/links/wiki_plugin.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.728532 wiki-0.8.2/src/wiki/plugins/macros/
--rw-r--r--   0 balder    (1000) balder    (1000)       61 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/macros/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)      217 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/macros/apps.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.728532 wiki-0.8.2/src/wiki/plugins/macros/mdx/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/macros/mdx/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     3297 2022-02-14 21:10:09.000000 wiki-0.8.2/src/wiki/plugins/macros/mdx/macro.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1015 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/macros/mdx/toc.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     2190 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/plugins/macros/mdx/wikilinks.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      403 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/macros/settings.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/macros/templates/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/macros/templates/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.684532 wiki-0.8.2/src/wiki/plugins/macros/templates/wiki/plugins/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.728532 wiki-0.8.2/src/wiki/plugins/macros/templates/wiki/plugins/macros/
--rw-rw-r--   0 balder    (1000) balder    (1000)      379 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/macros/templates/wiki/plugins/macros/article_list.html
--rw-r--r--   0 balder    (1000) balder    (1000)      461 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/plugins/macros/templates/wiki/plugins/macros/sidebar.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.728532 wiki-0.8.2/src/wiki/plugins/macros/templates/wiki/plugins/templatetags/
--rw-rw-r--   0 balder    (1000) balder    (1000)      564 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/macros/templates/wiki/plugins/templatetags/article_list.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.728532 wiki-0.8.2/src/wiki/plugins/macros/templatetags/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/macros/templatetags/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)      576 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/macros/templatetags/wiki_macro_tags.py
--rw-r--r--   0 balder    (1000) balder    (1000)      644 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/macros/wiki_plugin.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.728532 wiki-0.8.2/src/wiki/plugins/notifications/
--rw-r--r--   0 balder    (1000) balder    (1000)       75 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/notifications/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1894 2021-08-03 21:31:57.000000 wiki-0.8.2/src/wiki/plugins/notifications/apps.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     7834 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/notifications/forms.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.728532 wiki-0.8.2/src/wiki/plugins/notifications/management/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/notifications/management/__init__.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.728532 wiki-0.8.2/src/wiki/plugins/notifications/management/commands/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/notifications/management/commands/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     2433 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/notifications/management/commands/wiki_notifications_create_defaults.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.732532 wiki-0.8.2/src/wiki/plugins/notifications/migrations/
--rw-rw-r--   0 balder    (1000) balder    (1000)     1220 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/notifications/migrations/0001_initial.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      372 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/notifications/migrations/0002_auto_20151118_1811.py
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/notifications/migrations/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     2645 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/notifications/models.py
--rw-r--r--   0 balder    (1000) balder    (1000)      159 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/notifications/settings.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.688532 wiki-0.8.2/src/wiki/plugins/notifications/static/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.688532 wiki-0.8.2/src/wiki/plugins/notifications/static/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.688532 wiki-0.8.2/src/wiki/plugins/notifications/static/wiki/plugins/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.688532 wiki-0.8.2/src/wiki/plugins/notifications/static/wiki/plugins/notifications/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.732532 wiki-0.8.2/src/wiki/plugins/notifications/static/wiki/plugins/notifications/js/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2374 2021-11-16 00:30:21.000000 wiki-0.8.2/src/wiki/plugins/notifications/static/wiki/plugins/notifications/js/ui.js
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.688532 wiki-0.8.2/src/wiki/plugins/notifications/templates/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.688532 wiki-0.8.2/src/wiki/plugins/notifications/templates/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.688532 wiki-0.8.2/src/wiki/plugins/notifications/templates/wiki/plugins/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.732532 wiki-0.8.2/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/
--rw-rw-r--   0 balder    (1000) balder    (1000)      951 2021-08-01 12:42:33.000000 wiki-0.8.2/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/menubaritem.html
--rw-rw-r--   0 balder    (1000) balder    (1000)     1318 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/settings.html
--rw-r--r--   0 balder    (1000) balder    (1000)      435 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/plugins/notifications/util.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     2103 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/notifications/views.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      599 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/plugins/notifications/wiki_plugin.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.732532 wiki-0.8.2/src/wiki/plugins/redlinks/
--rw-r--r--   0 balder    (1000) balder    (1000)       65 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/redlinks/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)      226 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/redlinks/apps.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.732532 wiki-0.8.2/src/wiki/plugins/redlinks/mdx/
--rw-r--r--   0 balder    (1000) balder    (1000)        0 2018-08-05 16:43:35.000000 wiki-0.8.2/src/wiki/plugins/redlinks/mdx/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     3488 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/plugins/redlinks/mdx/redlinks.py
--rw-r--r--   0 balder    (1000) balder    (1000)      222 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/plugins/redlinks/wiki_plugin.py
--rw-rw-r--   0 balder    (1000) balder    (1000)    10680 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/sites.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.688532 wiki-0.8.2/src/wiki/static/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.692532 wiki-0.8.2/src/wiki/static/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.688532 wiki-0.8.2/src/wiki/static/wiki/bootstrap/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.732532 wiki-0.8.2/src/wiki/static/wiki/bootstrap/css/
--rw-rw-r--   0 balder    (1000) balder    (1000)   253717 2022-05-07 21:19:54.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/css/wiki-bootstrap.min.css
--rw-r--r--   0 balder    (1000) balder    (1000)    53475 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/css/wiki-bootstrap.min.css.map
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.732532 wiki-0.8.2/src/wiki/static/wiki/bootstrap/js/
--rw-r--r--   0 balder    (1000) balder    (1000)    80699 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 balder    (1000) balder    (1000)   318045 2020-10-27 22:37:04.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 balder    (1000) balder    (1000)    60011 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 balder    (1000) balder    (1000)   194435 2020-10-27 22:37:04.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/js/bootstrap.min.js.map
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.740532 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/
--rw-r--r--   0 balder    (1000) balder    (1000)     1148 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_alert.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1121 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_badge.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1335 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_breadcrumb.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     3626 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_button-group.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     2649 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_buttons.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     5616 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_card.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     4794 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_carousel.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      960 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_close.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1012 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_code.scss
--rw-r--r--   0 balder    (1000) balder    (1000)    15445 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_custom-forms.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     4373 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_dropdown.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     9058 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_forms.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     3896 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_functions.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1583 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_grid.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1157 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_images.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     5787 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_input-group.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      405 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_jumbotron.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     3886 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_list-group.scss
--rw-r--r--   0 balder    (1000) balder    (1000)       83 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_media.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1050 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_mixins.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     6278 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_modal.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     2082 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_nav.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     7399 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_navbar.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1740 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_pagination.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     4705 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_popover.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     3033 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_print.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1153 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_progress.scss
--rw-r--r--   0 balder    (1000) balder    (1000)    11504 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_reboot.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      627 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_root.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1051 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_spinners.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     3544 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_tables.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      990 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_toasts.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     2512 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_tooltip.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      261 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_transitions.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     2248 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_type.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      502 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_utilities.scss
--rw-r--r--   0 balder    (1000) balder    (1000)    48459 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_variables.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      572 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/bootstrap-grid.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      411 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/bootstrap-reboot.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      920 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/bootstrap.scss
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.748532 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/
--rw-r--r--   0 balder    (1000) balder    (1000)      242 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_alert.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      581 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_background-variant.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      320 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_badge.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1340 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_border-radius.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      532 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_box-shadow.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     4482 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_breakpoints.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     3492 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_buttons.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1422 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_caret.scss
--rw-r--r--   0 balder    (1000) balder    (1000)       93 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_clearfix.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      613 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_deprecate.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      392 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_float.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     5094 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_forms.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     2050 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_gradients.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1901 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_grid-framework.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1969 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_grid.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      757 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_hover.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1161 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_image.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      433 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_list-group.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      170 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_lists.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      369 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_nav-divider.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      462 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_pagination.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      481 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_reset-text.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      202 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_resize.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      811 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_screen-reader.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      148 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_size.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      794 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_table-row.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      474 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_text-emphasis.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      326 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_text-hide.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      168 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_text-truncate.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      364 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_transition.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      189 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_visibility.scss
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.752532 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/
--rw-r--r--   0 balder    (1000) balder    (1000)      420 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_align.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      403 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_background.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1765 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_borders.scss
--rw-r--r--   0 balder    (1000) balder    (1000)       37 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_clearfix.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      519 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_display.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      846 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_embed.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     2769 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_flex.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      376 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_float.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      133 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_overflow.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      484 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_position.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      115 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_screenreaders.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      249 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_shadows.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      498 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_sizing.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     2101 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_spacing.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      431 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_stretched-link.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     2018 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_text.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      174 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_visibility.scss
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.752532 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/vendor/
--rw-r--r--   0 balder    (1000) balder    (1000)     6473 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/vendor/_rfs.scss
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.752532 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/wiki/
--rw-r--r--   0 balder    (1000) balder    (1000)     4221 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/wiki/_codehilite.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     2254 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/wiki/_typeahead.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      208 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/wiki/wiki-bootstrap.scss
--rw-rw-r--   0 balder    (1000) balder    (1000)    10275 2021-08-01 12:42:33.000000 wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/wiki/wiki.scss
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.752532 wiki-0.8.2/src/wiki/static/wiki/font-awesome/
--rw-r--r--   0 balder    (1000) balder    (1000)     1548 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/LICENSE.txt
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.756533 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/
--rw-r--r--   0 balder    (1000) balder    (1000)      300 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_animated.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      428 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_bordered-pulled.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      332 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_core.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      121 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_fixed-width.scss
--rw-r--r--   0 balder    (1000) balder    (1000)   113790 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_icons.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      393 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_larger.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      322 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_list.scss
--rw-r--r--   0 balder    (1000) balder    (1000)     1266 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_mixins.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      833 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_rotated-flipped.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      130 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_screen-reader.scss
--rw-r--r--   0 balder    (1000) balder    (1000)    65387 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_shims.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      505 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_stacked.scss
--rw-r--r--   0 balder    (1000) balder    (1000)    37720 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_variables.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      803 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/brands.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      433 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/fontawesome.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      805 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/regular.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      798 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/solid.scss
--rw-r--r--   0 balder    (1000) balder    (1000)      224 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/v4-shims.scss
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.760532 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/
--rw-r--r--   0 balder    (1000) balder    (1000)   133034 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 balder    (1000) balder    (1000)   715447 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 balder    (1000) balder    (1000)   132728 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 balder    (1000) balder    (1000)    89824 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    76548 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)    34390 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 balder    (1000) balder    (1000)   144170 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 balder    (1000) balder    (1000)    34092 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 balder    (1000) balder    (1000)    16800 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    13600 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   194078 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 balder    (1000) balder    (1000)   848275 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 balder    (1000) balder    (1000)   193792 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 balder    (1000) balder    (1000)    99004 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    76120 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.woff2
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.764533 wiki-0.8.2/src/wiki/static/wiki/img/
--rw-rw-r--   0 balder    (1000) balder    (1000)     3902 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/img/github_icon.png
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.768533 wiki-0.8.2/src/wiki/static/wiki/js/
--rw-r--r--   0 balder    (1000) balder    (1000)      158 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/js/article.js
--rw-rw-r--   0 balder    (1000) balder    (1000)      312 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/js/core.js
--rw-r--r--   0 balder    (1000) balder    (1000)     1140 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/js/diff.js
--rw-rw-r--   0 balder    (1000) balder    (1000)     2455 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/js/diffview.js
--rw-rw-r--   0 balder    (1000) balder    (1000)     1806 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/js/editor.js
--rw-rw-r--   0 balder    (1000) balder    (1000)      809 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/js/forms.js
--rw-r--r--   0 balder    (1000) balder    (1000)    88145 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/js/jquery-3.4.1.min.js
--rw-rw-r--   0 balder    (1000) balder    (1000)    89501 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/static/wiki/js/jquery-3.6.0.min.js
--rw-r--r--   0 balder    (1000) balder    (1000)    16740 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/js/popper.js
--rw-rw-r--   0 balder    (1000) balder    (1000)    87922 2020-10-27 22:37:04.000000 wiki-0.8.2/src/wiki/static/wiki/js/popper.min.js.map
--rw-rw-r--   0 balder    (1000) balder    (1000)     4592 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/js/respond.min.js
--rw-rw-r--   0 balder    (1000) balder    (1000)     9215 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/js/urlify.js
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.768533 wiki-0.8.2/src/wiki/static/wiki/markitup/
--rw-rw-r--   0 balder    (1000) balder    (1000)      125 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/admin.init.js
--rw-rw-r--   0 balder    (1000) balder    (1000)       75 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/frontend.init.js
--rw-rw-r--   0 balder    (1000) balder    (1000)    20378 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/jquery.markitup.js
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.692532 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.768533 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.772533 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/
--rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/bold.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      859 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/code.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      276 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/h1.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/h2.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      306 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/h3.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      293 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/h4.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/h5.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      310 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/h6.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      223 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/italic.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      343 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/link.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      344 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/list-bullet.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      357 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/list-numeric.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      606 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/picture.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      537 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/preview.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      743 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/quotes.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      319 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/readme.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)     2405 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/set.js
--rw-rw-r--   0 balder    (1000) balder    (1000)     1713 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/style.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.772533 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.772533 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/
--rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/bold.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      667 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/clean.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      516 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/image.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      223 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/italic.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      343 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/link.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      344 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/list-bullet.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      357 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/list-numeric.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      606 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/picture.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      537 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/preview.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      269 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/stroke.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1869 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/set.js
--rw-rw-r--   0 balder    (1000) balder    (1000)      884 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/style.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.776533 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.776533 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/
--rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/bold.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      859 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/code.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      276 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/h1.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/h2.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      306 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/h3.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      293 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/h4.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/h5.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      310 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/h6.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      223 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/italic.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      343 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/link.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      344 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/list-bullet.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      357 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/list-numeric.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      606 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/picture.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      537 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/preview.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      743 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/quotes.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      319 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/readme.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)     2035 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/set.js
--rw-rw-r--   0 balder    (1000) balder    (1000)     1657 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/style.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.692532 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.776533 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.780533 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/
--rw-rw-r--   0 balder    (1000) balder    (1000)      322 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-container.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1642 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-bbcode.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1682 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-dotclear.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1534 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-html.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1529 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-json.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1783 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-markdown.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1659 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-textile.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1488 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-wiki.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1495 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-xml.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     1745 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      258 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/handle.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      254 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/menu.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      240 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/submenu.png
--rw-rw-r--   0 balder    (1000) balder    (1000)     3334 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/style.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.780533 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/simple/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.780533 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/simple/images/
--rw-rw-r--   0 balder    (1000) balder    (1000)      258 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/simple/images/handle.png
--rw-rw-r--   0 balder    (1000) balder    (1000)    27151 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/simple/images/menu.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      240 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/simple/images/submenu.png
--rw-rw-r--   0 balder    (1000) balder    (1000)      151 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/simple/readme.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)     2457 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/skins/simple/style.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.780533 wiki-0.8.2/src/wiki/static/wiki/markitup/templates/
--rw-rw-r--   0 balder    (1000) balder    (1000)      114 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/templates/preview.css
--rw-rw-r--   0 balder    (1000) balder    (1000)      406 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/static/wiki/markitup/templates/preview.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.692532 wiki-0.8.2/src/wiki/static/wiki/select2/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.780533 wiki-0.8.2/src/wiki/static/wiki/select2/css/
--rw-r--r--   0 balder    (1000) balder    (1000)    14966 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/select2/css/select2.min.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.780533 wiki-0.8.2/src/wiki/static/wiki/select2/js/
--rw-r--r--   0 balder    (1000) balder    (1000)    70852 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/static/wiki/select2/js/select2.min.js
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.692532 wiki-0.8.2/src/wiki/templates/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.784533 wiki-0.8.2/src/wiki/templates/wiki/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.784533 wiki-0.8.2/src/wiki/templates/wiki/accounts/
--rw-rw-r--   0 balder    (1000) balder    (1000)      467 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/accounts/account_settings.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      998 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/accounts/login.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      818 2021-04-10 17:57:27.000000 wiki-0.8.2/src/wiki/templates/wiki/accounts/signup.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1406 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/article.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      111 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/base.html
--rw-rw-r--   0 balder    (1000) balder    (1000)     6040 2021-08-28 19:22:13.000000 wiki-0.8.2/src/wiki/templates/wiki/base_site.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1377 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/create.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1327 2019-10-08 14:58:43.000000 wiki-0.8.2/src/wiki/templates/wiki/create_root.html
--rw-r--r--   0 balder    (1000) balder    (1000)     2310 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/delete.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1591 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/deleted.html
--rw-r--r--   0 balder    (1000) balder    (1000)      980 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/deleted_list.html
--rw-r--r--   0 balder    (1000) balder    (1000)     2604 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/dir.html
--rw-r--r--   0 balder    (1000) balder    (1000)     4569 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/edit.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1221 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/error.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.784533 wiki-0.8.2/src/wiki/templates/wiki/forms/
--rw-r--r--   0 balder    (1000) balder    (1000)      144 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/templates/wiki/forms/markitup-admin.html
--rw-r--r--   0 balder    (1000) balder    (1000)      155 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/templates/wiki/forms/markitup.html
--rw-r--r--   0 balder    (1000) balder    (1000)      169 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/forms/text.html
--rw-r--r--   0 balder    (1000) balder    (1000)     8767 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/history.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.788533 wiki-0.8.2/src/wiki/templates/wiki/includes/
--rw-r--r--   0 balder    (1000) balder    (1000)      391 2018-08-05 16:43:35.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/anonymous_blocked.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1969 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/article_menu.html
--rw-r--r--   0 balder    (1000) balder    (1000)     2752 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/breadcrumbs.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      294 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/editor.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1313 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/editor_sidebar.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      479 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/editormedia.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      302 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/form.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      287 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/formerrors.html
--rw-r--r--   0 balder    (1000) balder    (1000)      952 2021-04-10 14:51:07.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/formfield.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      253 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/messages.html
--rw-r--r--   0 balder    (1000) balder    (1000)      452 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/modals.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      683 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/move_tree.html
--rw-rw-r--   0 balder    (1000) balder    (1000)     1736 2022-05-07 18:46:14.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/pagination.html
--rw-r--r--   0 balder    (1000) balder    (1000)      750 2018-07-30 22:22:46.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/render.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1073 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/revision_info.html
--rw-r--r--   0 balder    (1000) balder    (1000)      781 2019-10-08 14:58:43.000000 wiki-0.8.2/src/wiki/templates/wiki/includes/searchresult.html
--rw-r--r--   0 balder    (1000) balder    (1000)     2425 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/move.html
--rw-r--r--   0 balder    (1000) balder    (1000)      926 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/permission_denied.html
--rw-rw-r--   0 balder    (1000) balder    (1000)     1733 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/preview_inline.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1273 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/root_missing.html
--rw-r--r--   0 balder    (1000) balder    (1000)     1525 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/search.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      731 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/settings.html
--rw-r--r--   0 balder    (1000) balder    (1000)      455 2020-04-15 14:16:44.000000 wiki-0.8.2/src/wiki/templates/wiki/source.html
--rw-rw-r--   0 balder    (1000) balder    (1000)      150 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templates/wiki/view.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.788533 wiki-0.8.2/src/wiki/templatetags/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/templatetags/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     6107 2020-10-18 20:17:21.000000 wiki-0.8.2/src/wiki/templatetags/wiki_tags.py
--rw-rw-r--   0 balder    (1000) balder    (1000)    12036 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/urls.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.788533 wiki-0.8.2/src/wiki/views/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.8.2/src/wiki/views/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     5375 2020-10-04 20:12:11.000000 wiki-0.8.2/src/wiki/views/accounts.py
--rw-rw-r--   0 balder    (1000) balder    (1000)    38407 2022-02-14 21:10:09.000000 wiki-0.8.2/src/wiki/views/article.py
--rw-r--r--   0 balder    (1000) balder    (1000)      800 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/views/deleted_list.py
--rw-r--r--   0 balder    (1000) balder    (1000)     1635 2020-04-14 16:55:09.000000 wiki-0.8.2/src/wiki/views/mixins.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-05-07 21:19:57.696532 wiki-0.8.2/src/wiki.egg-info/
--rw-rw-r--   0 balder    (1000) balder    (1000)    12878 2022-05-07 21:19:57.000000 wiki-0.8.2/src/wiki.egg-info/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)    24399 2022-05-07 21:19:57.000000 wiki-0.8.2/src/wiki.egg-info/SOURCES.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2022-05-07 21:19:57.000000 wiki-0.8.2/src/wiki.egg-info/dependency_links.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2022-05-07 21:19:55.000000 wiki-0.8.2/src/wiki.egg-info/not-zip-safe
--rw-rw-r--   0 balder    (1000) balder    (1000)      528 2022-05-07 21:19:57.000000 wiki-0.8.2/src/wiki.egg-info/requires.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        5 2022-05-07 21:19:57.000000 wiki-0.8.2/src/wiki.egg-info/top_level.txt
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.062076 wiki-0.9/
+-rw-r--r--   0 balder    (1000) balder    (1000)    35143 2013-11-18 22:19:29.000000 wiki-0.9/COPYING
+-rw-rw-r--   0 balder    (1000) balder    (1000)      281 2020-10-27 22:37:04.000000 wiki-0.9/MANIFEST.in
+-rw-rw-r--   0 balder    (1000) balder    (1000)    12959 2022-06-27 20:39:37.066078 wiki-0.9/PKG-INFO
+-rw-rw-r--   0 balder    (1000) balder    (1000)     9786 2022-06-27 20:32:58.000000 wiki-0.9/README.rst
+-rw-rw-r--   0 balder    (1000) balder    (1000)      295 2022-06-27 20:39:37.066078 wiki-0.9/setup.cfg
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3242 2022-06-27 20:32:58.000000 wiki-0.9/setup.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.982039 wiki-0.9/src/wiki/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      884 2022-06-27 20:39:27.000000 wiki-0.9/src/wiki/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3027 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/admin.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      862 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/apps.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4399 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/checks.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.982039 wiki-0.9/src/wiki/conf/
+-rw-r--r--   0 balder    (1000) balder    (1000)        0 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/conf/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)    11603 2021-10-25 21:21:54.000000 wiki-0.9/src/wiki/conf/settings.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.982039 wiki-0.9/src/wiki/core/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/core/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      272 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/core/diff.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      162 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/core/exceptions.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     1705 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/core/http.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.982039 wiki-0.9/src/wiki/core/markdown/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4081 2022-06-27 20:32:58.000000 wiki-0.9/src/wiki/core/markdown/__init__.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.982039 wiki-0.9/src/wiki/core/markdown/mdx/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/core/markdown/mdx/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4894 2022-06-27 20:32:58.000000 wiki-0.9/src/wiki/core/markdown/mdx/codehilite.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      839 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/core/markdown/mdx/previewlinks.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1797 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/core/markdown/mdx/responsivetable.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     1055 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/core/paginator.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     3032 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/core/permissions.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.982039 wiki-0.9/src/wiki/core/plugins/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/core/plugins/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     2039 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/core/plugins/base.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      128 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/core/plugins/loader.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2013 2022-02-14 21:10:09.000000 wiki-0.9/src/wiki/core/plugins/registry.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      355 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/core/utils.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     4006 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/core/version.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     6823 2021-04-06 21:41:39.000000 wiki-0.9/src/wiki/decorators.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.982039 wiki-0.9/src/wiki/editors/
+-rw-r--r--   0 balder    (1000) balder    (1000)      368 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/editors/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      585 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/editors/base.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     1579 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/editors/markitup.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)    22009 2022-05-08 22:32:44.000000 wiki-0.9/src/wiki/forms.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3103 2021-12-28 23:42:50.000000 wiki-0.9/src/wiki/forms_account_handling.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/ca/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      380 2021-02-28 12:24:18.000000 wiki-0.9/src/wiki/locale/ca/LC_MESSAGES/django.mo
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/cs/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    44514 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    67826 2021-04-10 18:00:16.000000 wiki-0.9/src/wiki/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/da/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    43486 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/da/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    66844 2021-04-10 18:00:33.000000 wiki-0.9/src/wiki/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/de/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    45256 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    68744 2021-04-10 18:00:40.000000 wiki-0.9/src/wiki/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/el/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/el/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    14057 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/el/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    56967 2021-04-10 18:00:15.000000 wiki-0.9/src/wiki/locale/el/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/en/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    49600 2021-02-28 12:24:18.000000 wiki-0.9/src/wiki/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/es/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    40147 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    66047 2021-04-10 18:00:49.000000 wiki-0.9/src/wiki/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/fi/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    33339 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    62592 2021-04-10 18:00:16.000000 wiki-0.9/src/wiki/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/fr/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    46271 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    69950 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/hu/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/hu/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    44201 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    67354 2021-04-10 18:00:38.000000 wiki-0.9/src/wiki/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/it/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.986041 wiki-0.9/src/wiki/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    19821 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    57427 2021-04-10 18:00:41.000000 wiki-0.9/src/wiki/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/ja/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.990043 wiki-0.9/src/wiki/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    49498 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    72735 2021-04-10 18:00:20.000000 wiki-0.9/src/wiki/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/ko_KR/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.990043 wiki-0.9/src/wiki/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    46093 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    69523 2021-04-10 18:00:32.000000 wiki-0.9/src/wiki/locale/ko_KR/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/nb_NO/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.990043 wiki-0.9/src/wiki/locale/nb_NO/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     8946 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    52370 2021-04-10 18:00:31.000000 wiki-0.9/src/wiki/locale/nb_NO/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/nl/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.990043 wiki-0.9/src/wiki/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    45086 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    68402 2021-04-10 18:00:38.000000 wiki-0.9/src/wiki/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/pl_PL/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.990043 wiki-0.9/src/wiki/locale/pl_PL/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    45424 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    68758 2021-04-10 18:00:41.000000 wiki-0.9/src/wiki/locale/pl_PL/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.966032 wiki-0.9/src/wiki/locale/pt/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.990043 wiki-0.9/src/wiki/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    31813 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    62198 2021-04-10 18:00:31.000000 wiki-0.9/src/wiki/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/pt_BR/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.990043 wiki-0.9/src/wiki/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    44456 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    67805 2021-04-10 18:00:18.000000 wiki-0.9/src/wiki/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/pt_PT/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.990043 wiki-0.9/src/wiki/locale/pt_PT/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    31813 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    62198 2021-04-10 18:00:31.000000 wiki-0.9/src/wiki/locale/pt_PT/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/ro/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.994045 wiki-0.9/src/wiki/locale/ro/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    34462 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/ro/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    63439 2021-04-10 18:00:48.000000 wiki-0.9/src/wiki/locale/ro/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/ru/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.994045 wiki-0.9/src/wiki/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    58484 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    82146 2021-04-10 18:00:33.000000 wiki-0.9/src/wiki/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/sk/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.994045 wiki-0.9/src/wiki/locale/sk/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    39855 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/sk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    65886 2021-04-10 18:00:50.000000 wiki-0.9/src/wiki/locale/sk/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/sv/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.994045 wiki-0.9/src/wiki/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    19807 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    57605 2021-04-10 18:00:51.000000 wiki-0.9/src/wiki/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/tr_TR/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.994045 wiki-0.9/src/wiki/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    44807 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    68115 2021-04-10 18:00:52.000000 wiki-0.9/src/wiki/locale/tr_TR/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/zh_CN/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.994045 wiki-0.9/src/wiki/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    40469 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    64017 2021-04-10 18:00:50.000000 wiki-0.9/src/wiki/locale/zh_CN/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/zh_Hans/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.994045 wiki-0.9/src/wiki/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    40469 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    64017 2021-04-10 18:00:50.000000 wiki-0.9/src/wiki/locale/zh_Hans/LC_MESSAGES/django.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/locale/zh_TW/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.994045 wiki-0.9/src/wiki/locale/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    13263 2021-04-10 18:13:29.000000 wiki-0.9/src/wiki/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-rw-r--   0 balder    (1000) balder    (1000)    54075 2021-04-10 18:00:17.000000 wiki-0.9/src/wiki/locale/zh_TW/LC_MESSAGES/django.po
+-rw-rw-r--   0 balder    (1000) balder    (1000)     5264 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/managers.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.994045 wiki-0.9/src/wiki/migrations/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    16991 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/migrations/0001_initial.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      732 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/migrations/0002_urlpath_moved_to.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1321 2022-02-14 21:10:11.000000 wiki-0.9/src/wiki/migrations/0003_mptt_upgrade.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/migrations/__init__.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.998046 wiki-0.9/src/wiki/models/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1599 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/models/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)    17707 2022-02-14 21:10:09.000000 wiki-0.9/src/wiki/models/article.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)    11298 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/models/pluginbase.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)    14406 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/models/urlpath.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.998046 wiki-0.9/src/wiki/plugins/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/__init__.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.998046 wiki-0.9/src/wiki/plugins/attachments/
+-rw-r--r--   0 balder    (1000) balder    (1000)       71 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/attachments/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      349 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/attachments/admin.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      237 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/attachments/apps.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     6159 2021-12-28 23:42:50.000000 wiki-0.9/src/wiki/plugins/attachments/forms.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3658 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/plugins/attachments/markdown_extensions.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.998046 wiki-0.9/src/wiki/plugins/attachments/migrations/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4838 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/attachments/migrations/0001_initial.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      493 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/attachments/migrations/0002_auto_20151118_1816.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/attachments/migrations/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     7500 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/attachments/models.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3532 2021-01-11 06:47:50.000000 wiki-0.9/src/wiki/plugins/attachments/settings.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/attachments/templates/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/attachments/templates/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.998046 wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2208 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/delete.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     2132 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/history.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     7123 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/index.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      420 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/render.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     2136 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/replace.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2719 2022-01-20 10:37:17.000000 wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/search.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1413 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/attachments/urls.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)    16508 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/attachments/views.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1440 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/attachments/wiki_plugin.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.998046 wiki-0.9/src/wiki/plugins/editsection/
+-rw-r--r--   0 balder    (1000) balder    (1000)       71 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/editsection/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      238 2022-02-14 21:10:11.000000 wiki-0.9/src/wiki/plugins/editsection/apps.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4200 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/plugins/editsection/markdown_extensions.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      577 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/editsection/settings.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     6986 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/editsection/views.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      640 2022-02-14 21:10:11.000000 wiki-0.9/src/wiki/plugins/editsection/wiki_plugin.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.002048 wiki-0.9/src/wiki/plugins/globalhistory/
+-rw-r--r--   0 balder    (1000) balder    (1000)       75 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/globalhistory/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      246 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/globalhistory/apps.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/globalhistory/forms.py
+-rw-r--r--   0 balder    (1000) balder    (1000)        0 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/plugins/globalhistory/models.py
+-rw-r--r--   0 balder    (1000) balder    (1000)       23 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/globalhistory/settings.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/globalhistory/templates/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/globalhistory/templates/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/globalhistory/templates/wiki/plugins/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.002048 wiki-0.9/src/wiki/plugins/globalhistory/templates/wiki/plugins/globalhistory/
+-rw-r--r--   0 balder    (1000) balder    (1000)     4032 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/globalhistory/templates/wiki/plugins/globalhistory/globalhistory.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      205 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/globalhistory/templates/wiki/plugins/globalhistory/menubaritem.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1184 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/globalhistory/views.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      567 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/globalhistory/wiki_plugin.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.002048 wiki-0.9/src/wiki/plugins/help/
+-rw-r--r--   0 balder    (1000) balder    (1000)       57 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/help/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      209 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/help/apps.py
+-rw-r--r--   0 balder    (1000) balder    (1000)        0 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/plugins/help/models.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/help/templates/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/help/templates/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/help/templates/wiki/plugins/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.002048 wiki-0.9/src/wiki/plugins/help/templates/wiki/plugins/help/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      966 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/help/templates/wiki/plugins/help/sidebar.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)       26 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/help/views.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      471 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/help/wiki_plugin.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.002048 wiki-0.9/src/wiki/plugins/images/
+-rw-r--r--   0 balder    (1000) balder    (1000)       61 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/images/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      935 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/images/admin.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      432 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/images/apps.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      398 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/images/checks.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2376 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/images/forms.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3430 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/plugins/images/markdown_extensions.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.002048 wiki-0.9/src/wiki/plugins/images/migrations/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2253 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/images/migrations/0001_initial.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      458 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/images/migrations/0002_auto_20151118_1811.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/migrations/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     5143 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/images/models.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     1684 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/images/settings.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/images/static/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/images/static/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.002048 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.002048 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4363 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/colorbox.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.006050 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      112 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/border.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2893 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/controls.png
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.006050 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      111 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomCenter.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      215 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomLeft.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      217 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomRight.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      108 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderMiddleLeft.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      108 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderMiddleRight.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      111 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopCenter.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      216 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopLeft.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      214 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopRight.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     9427 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/loading.gif
+-rw-rw-r--   0 balder    (1000) balder    (1000)      157 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/loading_background.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      182 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/overlay.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     5533 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/index.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)    11096 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/jquery.colorbox-min.js
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.006050 wiki-0.9/src/wiki/plugins/images/static/wiki/js/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      222 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/static/wiki/js/images.js
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.970034 wiki-0.9/src/wiki/plugins/images/templates/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/images/templates/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.006050 wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4407 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/index.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1140 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/purge.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      942 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/render.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1123 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/revision_add.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     6477 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/sidebar.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.006050 wiki-0.9/src/wiki/plugins/images/templatetags/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/images/templatetags/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      510 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/images/templatetags/wiki_images_tags.py
+-rw-r--r--   0 balder    (1000) balder    (1000)       67 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/plugins/images/templatetags/wiki_thumbnails.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     7600 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/images/views.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2770 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/images/wiki_plugin.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.006050 wiki-0.9/src/wiki/plugins/links/
+-rw-r--r--   0 balder    (1000) balder    (1000)       59 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/links/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      213 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/links/apps.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.006050 wiki-0.9/src/wiki/plugins/links/mdx/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/links/mdx/__init__.py
+-rwxrwxr-x   0 balder    (1000) balder    (1000)     4938 2022-05-08 22:32:44.000000 wiki-0.9/src/wiki/plugins/links/mdx/djangowikilinks.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     5674 2022-05-08 22:32:44.000000 wiki-0.9/src/wiki/plugins/links/mdx/urlize.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)       30 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/links/models.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      488 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/links/settings.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/links/templates/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/links/templates/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/links/templates/wiki/plugins/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.006050 wiki-0.9/src/wiki/plugins/links/templates/wiki/plugins/links/
+-rw-r--r--   0 balder    (1000) balder    (1000)     1851 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/plugins/links/templates/wiki/plugins/links/sidebar.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1119 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/links/views.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1195 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/links/wiki_plugin.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/macros/
+-rw-r--r--   0 balder    (1000) balder    (1000)       61 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/macros/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      217 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/macros/apps.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/macros/mdx/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/macros/mdx/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3297 2022-02-14 21:10:09.000000 wiki-0.9/src/wiki/plugins/macros/mdx/macro.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1015 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/macros/mdx/toc.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2190 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/plugins/macros/mdx/wikilinks.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      403 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/macros/settings.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/macros/templates/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/macros/templates/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/macros/templates/wiki/plugins/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/macros/templates/wiki/plugins/macros/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      379 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/macros/templates/wiki/plugins/macros/article_list.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      461 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/plugins/macros/templates/wiki/plugins/macros/sidebar.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/macros/templates/wiki/plugins/templatetags/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      564 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/macros/templates/wiki/plugins/templatetags/article_list.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/macros/templatetags/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/macros/templatetags/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      576 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/macros/templatetags/wiki_macro_tags.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      644 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/macros/wiki_plugin.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/notifications/
+-rw-r--r--   0 balder    (1000) balder    (1000)       75 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/notifications/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1894 2021-08-03 21:31:57.000000 wiki-0.9/src/wiki/plugins/notifications/apps.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     7834 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/notifications/forms.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/notifications/management/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/notifications/management/__init__.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/notifications/management/commands/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/notifications/management/commands/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2433 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/notifications/management/commands/wiki_notifications_create_defaults.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/notifications/migrations/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1220 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/notifications/migrations/0001_initial.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      372 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/notifications/migrations/0002_auto_20151118_1811.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/notifications/migrations/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2645 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/notifications/models.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      159 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/notifications/settings.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/notifications/static/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/notifications/static/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/notifications/static/wiki/plugins/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/notifications/static/wiki/plugins/notifications/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/notifications/static/wiki/plugins/notifications/js/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2374 2021-11-16 00:30:21.000000 wiki-0.9/src/wiki/plugins/notifications/static/wiki/plugins/notifications/js/ui.js
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/notifications/templates/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/notifications/templates/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/plugins/notifications/templates/wiki/plugins/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.010052 wiki-0.9/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      951 2021-08-01 12:42:33.000000 wiki-0.9/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/menubaritem.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1318 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/settings.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      435 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/plugins/notifications/util.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2103 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/notifications/views.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)      599 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/plugins/notifications/wiki_plugin.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.014054 wiki-0.9/src/wiki/plugins/redlinks/
+-rw-r--r--   0 balder    (1000) balder    (1000)       65 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/redlinks/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      226 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/redlinks/apps.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.014054 wiki-0.9/src/wiki/plugins/redlinks/mdx/
+-rw-r--r--   0 balder    (1000) balder    (1000)        0 2018-08-05 16:43:35.000000 wiki-0.9/src/wiki/plugins/redlinks/mdx/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3488 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/plugins/redlinks/mdx/redlinks.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      222 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/plugins/redlinks/wiki_plugin.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)    10680 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/sites.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/static/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.978037 wiki-0.9/src/wiki/static/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.974035 wiki-0.9/src/wiki/static/wiki/bootstrap/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.014054 wiki-0.9/src/wiki/static/wiki/bootstrap/css/
+-rw-rw-r--   0 balder    (1000) balder    (1000)   253717 2022-06-27 20:39:33.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/css/wiki-bootstrap.min.css
+-rw-r--r--   0 balder    (1000) balder    (1000)    53475 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/css/wiki-bootstrap.min.css.map
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.014054 wiki-0.9/src/wiki/static/wiki/bootstrap/js/
+-rw-r--r--   0 balder    (1000) balder    (1000)    80699 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)   318045 2020-10-27 22:37:04.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 balder    (1000) balder    (1000)    60011 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)   194435 2020-10-27 22:37:04.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/js/bootstrap.min.js.map
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.018056 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/
+-rw-r--r--   0 balder    (1000) balder    (1000)     1148 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_alert.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1121 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_badge.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1335 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_breadcrumb.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     3626 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_button-group.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     2649 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_buttons.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     5616 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_card.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     4794 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_carousel.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      960 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_close.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1012 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_code.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)    15445 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_custom-forms.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     4373 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_dropdown.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     9058 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_forms.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     3896 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_functions.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1583 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_grid.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1157 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_images.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     5787 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_input-group.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      405 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_jumbotron.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     3886 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_list-group.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)       83 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_media.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1050 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_mixins.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     6278 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_modal.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     2082 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_nav.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     7399 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_navbar.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1740 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_pagination.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     4705 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_popover.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     3033 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_print.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1153 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_progress.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)    11504 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_reboot.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      627 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_root.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1051 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_spinners.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     3544 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_tables.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      990 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_toasts.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     2512 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_tooltip.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      261 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_transitions.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     2248 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_type.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      502 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_utilities.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)    48459 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_variables.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      572 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/bootstrap-grid.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      411 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/bootstrap-reboot.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      920 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/bootstrap.scss
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.026059 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/
+-rw-r--r--   0 balder    (1000) balder    (1000)      242 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_alert.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      581 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_background-variant.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      320 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_badge.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1340 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_border-radius.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      532 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_box-shadow.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     4482 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_breakpoints.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     3492 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_buttons.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1422 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_caret.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)       93 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_clearfix.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      613 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_deprecate.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      392 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_float.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     5094 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_forms.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     2050 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_gradients.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1901 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_grid-framework.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1969 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_grid.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      757 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_hover.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1161 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_image.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      433 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_list-group.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      170 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_lists.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      369 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_nav-divider.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      462 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_pagination.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      481 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_reset-text.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      202 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_resize.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      811 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_screen-reader.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      148 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_size.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      794 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_table-row.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      474 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_text-emphasis.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      326 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_text-hide.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      168 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_text-truncate.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      364 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_transition.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      189 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_visibility.scss
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.026059 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/
+-rw-r--r--   0 balder    (1000) balder    (1000)      420 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_align.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      403 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_background.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1765 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_borders.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)       37 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_clearfix.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      519 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_display.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      846 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_embed.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     2769 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_flex.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      376 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_float.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      133 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_overflow.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      484 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_position.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      115 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_screenreaders.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      249 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_shadows.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      498 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_sizing.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     2101 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_spacing.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      431 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_stretched-link.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     2018 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_text.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      174 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_visibility.scss
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.026059 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/vendor/
+-rw-r--r--   0 balder    (1000) balder    (1000)     6473 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/vendor/_rfs.scss
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.026059 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/wiki/
+-rw-r--r--   0 balder    (1000) balder    (1000)     4221 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/wiki/_codehilite.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     2254 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/wiki/_typeahead.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      208 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/wiki/wiki-bootstrap.scss
+-rw-rw-r--   0 balder    (1000) balder    (1000)    10275 2021-08-01 12:42:33.000000 wiki-0.9/src/wiki/static/wiki/bootstrap/scss/wiki/wiki.scss
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.026059 wiki-0.9/src/wiki/static/wiki/font-awesome/
+-rw-r--r--   0 balder    (1000) balder    (1000)     1548 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/LICENSE.txt
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.030061 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/
+-rw-r--r--   0 balder    (1000) balder    (1000)      300 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_animated.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      428 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_bordered-pulled.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      332 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_core.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      121 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_fixed-width.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)   113790 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_icons.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      393 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_larger.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      322 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_list.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)     1266 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_mixins.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      833 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_rotated-flipped.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      130 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_screen-reader.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)    65387 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_shims.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      505 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_stacked.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)    37720 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_variables.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      803 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/brands.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      433 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/fontawesome.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      805 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/regular.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      798 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/solid.scss
+-rw-r--r--   0 balder    (1000) balder    (1000)      224 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/scss/v4-shims.scss
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.038065 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/
+-rw-r--r--   0 balder    (1000) balder    (1000)   133034 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 balder    (1000) balder    (1000)   715447 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 balder    (1000) balder    (1000)   132728 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 balder    (1000) balder    (1000)    89824 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)    76548 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)    34390 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 balder    (1000) balder    (1000)   144170 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 balder    (1000) balder    (1000)    34092 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 balder    (1000) balder    (1000)    16800 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)    13600 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   194078 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 balder    (1000) balder    (1000)   848275 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 balder    (1000) balder    (1000)   193792 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 balder    (1000) balder    (1000)    99004 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)    76120 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.woff2
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.038065 wiki-0.9/src/wiki/static/wiki/img/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3902 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/img/github_icon.png
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.038065 wiki-0.9/src/wiki/static/wiki/js/
+-rw-r--r--   0 balder    (1000) balder    (1000)      158 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/js/article.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)      312 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/js/core.js
+-rw-r--r--   0 balder    (1000) balder    (1000)     1140 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/js/diff.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2455 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/js/diffview.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1806 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/js/editor.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)      809 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/js/forms.js
+-rw-r--r--   0 balder    (1000) balder    (1000)    88145 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/js/jquery-3.4.1.min.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)    89501 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/static/wiki/js/jquery-3.6.0.min.js
+-rw-r--r--   0 balder    (1000) balder    (1000)    16740 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/js/popper.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)    87922 2020-10-27 22:37:04.000000 wiki-0.9/src/wiki/static/wiki/js/popper.min.js.map
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4592 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/js/respond.min.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)     9215 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/js/urlify.js
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.038065 wiki-0.9/src/wiki/static/wiki/markitup/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      125 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/admin.init.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)       75 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/frontend.init.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)    20378 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/jquery.markitup.js
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.978037 wiki-0.9/src/wiki/static/wiki/markitup/sets/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.042067 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.046069 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/bold.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      859 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/code.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      276 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/h1.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/h2.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      306 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/h3.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      293 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/h4.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/h5.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      310 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/h6.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      223 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/italic.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      343 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/link.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      344 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/list-bullet.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      357 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/list-numeric.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      606 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/picture.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      537 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/preview.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      743 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/quotes.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      319 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/readme.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2405 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/set.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1713 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/style.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.046069 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.050070 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/bold.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      667 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/clean.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      516 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/image.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      223 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/italic.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      343 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/link.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      344 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/list-bullet.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      357 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/list-numeric.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      606 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/picture.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      537 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/preview.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      269 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/stroke.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1869 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/set.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)      884 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/default/style.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.050070 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.050070 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/bold.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      859 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/code.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      276 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/h1.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/h2.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      306 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/h3.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      293 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/h4.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      304 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/h5.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      310 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/h6.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      223 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/italic.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      343 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/link.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      344 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/list-bullet.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      357 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/list-numeric.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      606 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/picture.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      537 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/preview.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      743 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/quotes.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      319 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/readme.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2035 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/set.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1657 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/style.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.978037 wiki-0.9/src/wiki/static/wiki/markitup/skins/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.054072 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.054072 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      322 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-container.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1642 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-bbcode.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1682 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-dotclear.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1534 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-html.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1529 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-json.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1783 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-markdown.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1659 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-textile.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1488 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-wiki.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1495 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-xml.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1745 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      258 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/handle.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      254 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/menu.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      240 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/submenu.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3334 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/style.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.054072 wiki-0.9/src/wiki/static/wiki/markitup/skins/simple/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.054072 wiki-0.9/src/wiki/static/wiki/markitup/skins/simple/images/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      258 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/simple/images/handle.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)    27151 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/simple/images/menu.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      240 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/simple/images/submenu.png
+-rw-rw-r--   0 balder    (1000) balder    (1000)      151 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/simple/readme.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2457 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/skins/simple/style.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.054072 wiki-0.9/src/wiki/static/wiki/markitup/templates/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      114 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/templates/preview.css
+-rw-rw-r--   0 balder    (1000) balder    (1000)      406 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/static/wiki/markitup/templates/preview.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.978037 wiki-0.9/src/wiki/static/wiki/select2/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.054072 wiki-0.9/src/wiki/static/wiki/select2/css/
+-rw-r--r--   0 balder    (1000) balder    (1000)    14966 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/select2/css/select2.min.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.058074 wiki-0.9/src/wiki/static/wiki/select2/js/
+-rw-r--r--   0 balder    (1000) balder    (1000)    70852 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/static/wiki/select2/js/select2.min.js
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.978037 wiki-0.9/src/wiki/templates/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.058074 wiki-0.9/src/wiki/templates/wiki/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.058074 wiki-0.9/src/wiki/templates/wiki/accounts/
+-rw-rw-r--   0 balder    (1000) balder    (1000)      467 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/accounts/account_settings.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      998 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/accounts/login.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      818 2021-04-10 17:57:27.000000 wiki-0.9/src/wiki/templates/wiki/accounts/signup.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1406 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/article.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      111 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/base.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)     6040 2021-08-28 19:22:13.000000 wiki-0.9/src/wiki/templates/wiki/base_site.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1377 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/create.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1327 2019-10-08 14:58:43.000000 wiki-0.9/src/wiki/templates/wiki/create_root.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     2310 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/delete.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1591 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/deleted.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      980 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/deleted_list.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     2604 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/dir.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     4569 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/edit.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1221 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/error.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.062076 wiki-0.9/src/wiki/templates/wiki/forms/
+-rw-r--r--   0 balder    (1000) balder    (1000)      144 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/templates/wiki/forms/markitup-admin.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      155 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/templates/wiki/forms/markitup.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      169 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/forms/text.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     8767 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/history.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.062076 wiki-0.9/src/wiki/templates/wiki/includes/
+-rw-r--r--   0 balder    (1000) balder    (1000)      391 2018-08-05 16:43:35.000000 wiki-0.9/src/wiki/templates/wiki/includes/anonymous_blocked.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1969 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/includes/article_menu.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     2752 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/includes/breadcrumbs.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      294 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/includes/editor.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1313 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/includes/editor_sidebar.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      479 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/includes/editormedia.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      302 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/includes/form.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      287 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/includes/formerrors.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      952 2021-04-10 14:51:07.000000 wiki-0.9/src/wiki/templates/wiki/includes/formfield.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      253 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/includes/messages.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      452 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/includes/modals.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      683 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/includes/move_tree.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1736 2022-05-08 22:32:44.000000 wiki-0.9/src/wiki/templates/wiki/includes/pagination.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      750 2018-07-30 22:22:46.000000 wiki-0.9/src/wiki/templates/wiki/includes/render.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1073 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/includes/revision_info.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      781 2019-10-08 14:58:43.000000 wiki-0.9/src/wiki/templates/wiki/includes/searchresult.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     2425 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/move.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      926 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/permission_denied.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1733 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/preview_inline.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1273 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/root_missing.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     1525 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/search.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      731 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/settings.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      455 2020-04-15 14:16:44.000000 wiki-0.9/src/wiki/templates/wiki/source.html
+-rw-rw-r--   0 balder    (1000) balder    (1000)      150 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templates/wiki/view.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.062076 wiki-0.9/src/wiki/templatetags/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/templatetags/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     6107 2020-10-18 20:17:21.000000 wiki-0.9/src/wiki/templatetags/wiki_tags.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)    12036 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/urls.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:37.062076 wiki-0.9/src/wiki/views/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2018-01-29 12:55:24.000000 wiki-0.9/src/wiki/views/__init__.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     5375 2020-10-04 20:12:11.000000 wiki-0.9/src/wiki/views/accounts.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)    38407 2022-02-14 21:10:09.000000 wiki-0.9/src/wiki/views/article.py
+-rw-r--r--   0 balder    (1000) balder    (1000)      800 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/views/deleted_list.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     1635 2020-04-14 16:55:09.000000 wiki-0.9/src/wiki/views/mixins.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-06-27 20:39:36.982039 wiki-0.9/src/wiki.egg-info/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    12959 2022-06-27 20:39:36.000000 wiki-0.9/src/wiki.egg-info/PKG-INFO
+-rw-rw-r--   0 balder    (1000) balder    (1000)    24399 2022-06-27 20:39:36.000000 wiki-0.9/src/wiki.egg-info/SOURCES.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)        1 2022-06-27 20:39:36.000000 wiki-0.9/src/wiki.egg-info/dependency_links.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)        1 2022-06-27 20:39:34.000000 wiki-0.9/src/wiki.egg-info/not-zip-safe
+-rw-rw-r--   0 balder    (1000) balder    (1000)      533 2022-06-27 20:39:36.000000 wiki-0.9/src/wiki.egg-info/requires.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)        5 2022-06-27 20:39:36.000000 wiki-0.9/src/wiki.egg-info/top_level.txt
```

### Comparing `wiki-0.8.2/COPYING` & `wiki-0.9/COPYING`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/PKG-INFO` & `wiki-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiki
-Version: 0.8.2
+Version: 0.9
 Summary: A wiki system written for the Django framework.
 Home-page: http://www.django-wiki.org
 Author: Benjamin Bach
 Author-email: benjamin@overtag.dk
 License: GPLv3
 Description: django-wiki
         ===========
@@ -28,14 +28,17 @@
         --------------
         
         The below table explains which Django versions are supported.
         
         +------------------+----------------+--------------+
         | Release          | Django         | Upgrade from |
         +==================+================+==============+
+        | 0.9.x            | 2.2, 3.0, 3.1, | 0.7          |
+        |                  | 3.2, 4.0       |              |
+        +------------------+----------------+--------------+
         | 0.8.x            | 2.2, 3.0, 3.1, | 0.7          |
         |                  | 3.2, 4.0       |              |
         +------------------+----------------+--------------+
         | 0.7.x            | 2.2, 3.0, 3.1, | 0.5 or 0.6   |
         |                  | 3.2            |              |
         +------------------+----------------+--------------+
         | 0.6.x            | 2.1, 2.2, 3.0  | 0.5          |
@@ -245,16 +248,14 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `wiki-0.8.2/README.rst` & `wiki-0.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 --------------
 
 The below table explains which Django versions are supported.
 
 +------------------+----------------+--------------+
 | Release          | Django         | Upgrade from |
 +==================+================+==============+
+| 0.9.x            | 2.2, 3.0, 3.1, | 0.7          |
+|                  | 3.2, 4.0       |              |
++------------------+----------------+--------------+
 | 0.8.x            | 2.2, 3.0, 3.1, | 0.7          |
 |                  | 3.2, 4.0       |              |
 +------------------+----------------+--------------+
 | 0.7.x            | 2.2, 3.0, 3.1, | 0.5 or 0.6   |
 |                  | 3.2            |              |
 +------------------+----------------+--------------+
 | 0.6.x            | 2.1, 2.2, 3.0  | 0.5          |
```

### Comparing `wiki-0.8.2/setup.py` & `wiki-0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 # string in below ...
 def get_path(fname):
     return os.path.join(os.path.dirname(__file__), fname)
 
 
 install_requirements = [
     "Django>=2.1,<4.1",
-    "bleach>=3.3.0,<4.2",
+    "bleach[css]>=5",
+    "tinycss2",  # bleach complains ModuleNotFoundError: No module named 'tinycss2'
     "Pillow",
     "django-nyt>=1.2.2,<1.3",
     "django-mptt>=0.13,<0.14",
     "django-sekizai>=0.10",
     "sorl-thumbnail>=12.8,<13",
     "Markdown>=3.3,<3.4",
 ]
@@ -86,16 +87,14 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
```

### Comparing `wiki-0.8.2/src/wiki/__init__.py` & `wiki-0.9/src/wiki/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with django-wiki. If not, see <http://www.gnu.org/licenses/>.
 from wiki.core.version import get_version
 
 default_app_config = "wiki.apps.WikiConfig"
 
-VERSION = (0, 8, 2, "final", 0)
+VERSION = (0, 9, 0, "final", 0)
 __version__ = get_version(VERSION)
```

### Comparing `wiki-0.8.2/src/wiki/admin.py` & `wiki-0.9/src/wiki/admin.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/apps.py` & `wiki-0.9/src/wiki/apps.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/checks.py` & `wiki-0.9/src/wiki/checks.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/conf/settings.py` & `wiki-0.9/src/wiki/conf/settings.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/core/http.py` & `wiki-0.9/src/wiki/core/http.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/core/markdown/__init__.py` & `wiki-0.9/src/wiki/core/markdown/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import bleach
 import markdown
+from bleach.css_sanitizer import CSSSanitizer
 from wiki.conf import settings
 from wiki.core.plugins import registry as plugin_registry
 
 
 class ArticleMarkdown(markdown.Markdown):
     def __init__(self, article, preview=False, user=None, *args, **kwargs):
         kwargs.update(settings.MARKDOWN_KWARGS)
@@ -30,23 +31,27 @@
     def convert(self, text, *args, **kwargs):
         html = super().convert(text, *args, **kwargs)
         if settings.MARKDOWN_SANITIZE_HTML:
             tags = (
                 settings.MARKDOWN_HTML_WHITELIST + plugin_registry.get_html_whitelist()
             )
 
+            css_sanitizer = CSSSanitizer(
+                allowed_css_properties=settings.MARKDOWN_HTML_STYLES
+            )
+
             attrs = {}
             attrs.update(settings.MARKDOWN_HTML_ATTRIBUTES)
             attrs.update(plugin_registry.get_html_attributes().items())
 
             html = bleach.clean(
                 html,
                 tags=tags,
                 attributes=attrs,
-                styles=settings.MARKDOWN_HTML_STYLES,
+                css_sanitizer=css_sanitizer,
                 strip=True,
             )
         return html
 
 
 def article_markdown(text, article, *args, **kwargs):
     md = ArticleMarkdown(article, *args, **kwargs)
```

### Comparing `wiki-0.8.2/src/wiki/core/markdown/mdx/codehilite.py` & `wiki-0.9/src/wiki/core/markdown/mdx/codehilite.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,20 +72,32 @@
                 break
         return text.split("\n")
 
 
 class HiliteTreeprocessor(Treeprocessor):
     """Hilight source code in code blocks."""
 
+    def code_unescape(self, text):
+        """Unescape &, <, > and " characters."""
+        text = text.replace("&amp;", "&")
+        text = text.replace("&lt;", "<")
+        text = text.replace("&gt;", ">")
+        text = text.replace("&quot;", '"')
+        return text
+
     def run(self, root):
         """Find code blocks and store in htmlStash."""
         blocks = root.iter("pre")
         for block in blocks:
             if len(block) == 1 and block[0].tag == "code":
-                html = highlight(block[0].text, self.config, self.markdown.tab_length)
+                html = highlight(
+                    self.code_unescape(block[0].text),
+                    self.config,
+                    self.markdown.tab_length,
+                )
                 placeholder = self.markdown.htmlStash.store(html)
                 # Clear codeblock in etree instance
                 block.clear()
                 # Change to p element which will later
                 # be removed when inserting raw html
                 block.tag = "p"
                 block.text = placeholder
```

### Comparing `wiki-0.8.2/src/wiki/core/markdown/mdx/previewlinks.py` & `wiki-0.9/src/wiki/core/markdown/mdx/previewlinks.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/core/markdown/mdx/responsivetable.py` & `wiki-0.9/src/wiki/core/markdown/mdx/responsivetable.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/core/paginator.py` & `wiki-0.9/src/wiki/core/paginator.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/core/permissions.py` & `wiki-0.9/src/wiki/core/permissions.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/core/plugins/base.py` & `wiki-0.9/src/wiki/core/plugins/base.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/core/plugins/registry.py` & `wiki-0.9/src/wiki/core/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/core/version.py` & `wiki-0.9/src/wiki/core/version.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/decorators.py` & `wiki-0.9/src/wiki/decorators.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/editors/base.py` & `wiki-0.9/src/wiki/editors/base.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/editors/markitup.py` & `wiki-0.9/src/wiki/editors/markitup.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/forms.py` & `wiki-0.9/src/wiki/forms.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/forms_account_handling.py` & `wiki-0.9/src/wiki/forms_account_handling.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/cs/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/cs/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/da/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/da/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/de/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/de/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/el/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/el/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/en/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/es/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/es/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/fi/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/fi/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/fr/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/fr/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/hu/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/hu/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/it/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/it/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/ja/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/ja/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/ko_KR/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/ko_KR/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/nb_NO/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/nb_NO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/nb_NO/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/nl/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/nl/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/pl_PL/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/pl_PL/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/pt/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/pt/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/pt_BR/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/pt_BR/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/pt_PT/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/pt_PT/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/ro/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/ro/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/ru/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/ru/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/sk/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/sk/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/sv/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/sv/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/tr_TR/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/tr_TR/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/zh_CN/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/zh_CN/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/zh_Hans/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/zh_Hans/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/zh_TW/LC_MESSAGES/django.mo` & `wiki-0.9/src/wiki/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/locale/zh_TW/LC_MESSAGES/django.po` & `wiki-0.9/src/wiki/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/managers.py` & `wiki-0.9/src/wiki/managers.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/migrations/0001_initial.py` & `wiki-0.9/src/wiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/migrations/0002_urlpath_moved_to.py` & `wiki-0.9/src/wiki/migrations/0002_urlpath_moved_to.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/migrations/0003_mptt_upgrade.py` & `wiki-0.9/src/wiki/migrations/0003_mptt_upgrade.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/models/__init__.py` & `wiki-0.9/src/wiki/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/models/article.py` & `wiki-0.9/src/wiki/models/article.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/models/pluginbase.py` & `wiki-0.9/src/wiki/models/pluginbase.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/models/urlpath.py` & `wiki-0.9/src/wiki/models/urlpath.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/forms.py` & `wiki-0.9/src/wiki/plugins/attachments/forms.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/markdown_extensions.py` & `wiki-0.9/src/wiki/plugins/attachments/markdown_extensions.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/migrations/0001_initial.py` & `wiki-0.9/src/wiki/plugins/attachments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/models.py` & `wiki-0.9/src/wiki/plugins/attachments/models.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/settings.py` & `wiki-0.9/src/wiki/plugins/attachments/settings.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/delete.html` & `wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/delete.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/history.html` & `wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/history.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/index.html` & `wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/index.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/replace.html` & `wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/replace.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/search.html` & `wiki-0.9/src/wiki/plugins/attachments/templates/wiki/plugins/attachments/search.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/urls.py` & `wiki-0.9/src/wiki/plugins/attachments/urls.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/views.py` & `wiki-0.9/src/wiki/plugins/attachments/views.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/attachments/wiki_plugin.py` & `wiki-0.9/src/wiki/plugins/attachments/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/editsection/markdown_extensions.py` & `wiki-0.9/src/wiki/plugins/editsection/markdown_extensions.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/editsection/settings.py` & `wiki-0.9/src/wiki/plugins/editsection/settings.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/editsection/views.py` & `wiki-0.9/src/wiki/plugins/editsection/views.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/editsection/wiki_plugin.py` & `wiki-0.9/src/wiki/plugins/editsection/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/globalhistory/templates/wiki/plugins/globalhistory/globalhistory.html` & `wiki-0.9/src/wiki/plugins/globalhistory/templates/wiki/plugins/globalhistory/globalhistory.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/globalhistory/views.py` & `wiki-0.9/src/wiki/plugins/globalhistory/views.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/globalhistory/wiki_plugin.py` & `wiki-0.9/src/wiki/plugins/globalhistory/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/help/templates/wiki/plugins/help/sidebar.html` & `wiki-0.9/src/wiki/plugins/help/templates/wiki/plugins/help/sidebar.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/admin.py` & `wiki-0.9/src/wiki/plugins/images/admin.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/forms.py` & `wiki-0.9/src/wiki/plugins/images/forms.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/markdown_extensions.py` & `wiki-0.9/src/wiki/plugins/images/markdown_extensions.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/migrations/0001_initial.py` & `wiki-0.9/src/wiki/plugins/images/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/models.py` & `wiki-0.9/src/wiki/plugins/images/models.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/settings.py` & `wiki-0.9/src/wiki/plugins/images/settings.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/colorbox.css` & `wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/colorbox.css`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/controls.png` & `wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/controls.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/images/loading.gif` & `wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/images/loading.gif`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/example1/index.html` & `wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/example1/index.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/static/wiki/colorbox/jquery.colorbox-min.js` & `wiki-0.9/src/wiki/plugins/images/static/wiki/colorbox/jquery.colorbox-min.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/index.html` & `wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/index.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/purge.html` & `wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/purge.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/render.html` & `wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/render.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/revision_add.html` & `wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/revision_add.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/templates/wiki/plugins/images/sidebar.html` & `wiki-0.9/src/wiki/plugins/images/templates/wiki/plugins/images/sidebar.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/views.py` & `wiki-0.9/src/wiki/plugins/images/views.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/images/wiki_plugin.py` & `wiki-0.9/src/wiki/plugins/images/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/links/mdx/djangowikilinks.py` & `wiki-0.9/src/wiki/plugins/links/mdx/djangowikilinks.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/links/mdx/urlize.py` & `wiki-0.9/src/wiki/plugins/links/mdx/urlize.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/links/templates/wiki/plugins/links/sidebar.html` & `wiki-0.9/src/wiki/plugins/links/templates/wiki/plugins/links/sidebar.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/links/views.py` & `wiki-0.9/src/wiki/plugins/links/views.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/links/wiki_plugin.py` & `wiki-0.9/src/wiki/plugins/links/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/macros/mdx/macro.py` & `wiki-0.9/src/wiki/plugins/macros/mdx/macro.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/macros/mdx/toc.py` & `wiki-0.9/src/wiki/plugins/macros/mdx/toc.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/macros/mdx/wikilinks.py` & `wiki-0.9/src/wiki/plugins/macros/mdx/wikilinks.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/macros/templates/wiki/plugins/templatetags/article_list.html` & `wiki-0.9/src/wiki/plugins/macros/templates/wiki/plugins/templatetags/article_list.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/macros/templatetags/wiki_macro_tags.py` & `wiki-0.9/src/wiki/plugins/macros/templatetags/wiki_macro_tags.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/macros/wiki_plugin.py` & `wiki-0.9/src/wiki/plugins/macros/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/apps.py` & `wiki-0.9/src/wiki/plugins/notifications/apps.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/forms.py` & `wiki-0.9/src/wiki/plugins/notifications/forms.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/management/commands/wiki_notifications_create_defaults.py` & `wiki-0.9/src/wiki/plugins/notifications/management/commands/wiki_notifications_create_defaults.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/migrations/0001_initial.py` & `wiki-0.9/src/wiki/plugins/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/models.py` & `wiki-0.9/src/wiki/plugins/notifications/models.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/static/wiki/plugins/notifications/js/ui.js` & `wiki-0.9/src/wiki/plugins/notifications/static/wiki/plugins/notifications/js/ui.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/menubaritem.html` & `wiki-0.9/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/menubaritem.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/settings.html` & `wiki-0.9/src/wiki/plugins/notifications/templates/wiki/plugins/notifications/settings.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/views.py` & `wiki-0.9/src/wiki/plugins/notifications/views.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/notifications/wiki_plugin.py` & `wiki-0.9/src/wiki/plugins/notifications/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/plugins/redlinks/mdx/redlinks.py` & `wiki-0.9/src/wiki/plugins/redlinks/mdx/redlinks.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/sites.py` & `wiki-0.9/src/wiki/sites.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/css/wiki-bootstrap.min.css` & `wiki-0.9/src/wiki/static/wiki/bootstrap/css/wiki-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/css/wiki-bootstrap.min.css.map` & `wiki-0.9/src/wiki/static/wiki/bootstrap/css/wiki-bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/js/bootstrap.bundle.min.js` & `wiki-0.9/src/wiki/static/wiki/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/js/bootstrap.bundle.min.js.map` & `wiki-0.9/src/wiki/static/wiki/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/js/bootstrap.min.js` & `wiki-0.9/src/wiki/static/wiki/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/js/bootstrap.min.js.map` & `wiki-0.9/src/wiki/static/wiki/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_alert.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_badge.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_breadcrumb.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_button-group.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_buttons.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_card.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_carousel.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_close.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_code.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_code.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_custom-forms.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_custom-forms.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_dropdown.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_forms.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_forms.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_functions.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_grid.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_images.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_input-group.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_input-group.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_list-group.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_mixins.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_modal.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_nav.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_navbar.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_pagination.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_popover.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_print.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_print.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_progress.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_reboot.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_root.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_spinners.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_tables.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_toasts.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_tooltip.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_type.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/_variables.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/bootstrap-grid.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/bootstrap.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_background-variant.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_background-variant.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_border-radius.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_box-shadow.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_box-shadow.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_breakpoints.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_buttons.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_caret.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_deprecate.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_forms.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_gradients.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_grid-framework.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_grid.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_hover.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_hover.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_image.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_screen-reader.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_screen-reader.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/mixins/_table-row.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_borders.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_borders.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_display.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_display.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_embed.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_embed.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_flex.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_flex.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_spacing.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/utilities/_text.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/vendor/_rfs.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/wiki/_codehilite.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/wiki/_codehilite.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/wiki/_typeahead.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/wiki/_typeahead.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/bootstrap/scss/wiki/wiki.scss` & `wiki-0.9/src/wiki/static/wiki/bootstrap/scss/wiki/wiki.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/LICENSE.txt` & `wiki-0.9/src/wiki/static/wiki/font-awesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_icons.scss` & `wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_icons.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_mixins.scss` & `wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_rotated-flipped.scss` & `wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_rotated-flipped.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_shims.scss` & `wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_shims.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/_variables.scss` & `wiki-0.9/src/wiki/static/wiki/font-awesome/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/brands.scss` & `wiki-0.9/src/wiki/static/wiki/font-awesome/scss/brands.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/regular.scss` & `wiki-0.9/src/wiki/static/wiki/font-awesome/scss/regular.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/scss/solid.scss` & `wiki-0.9/src/wiki/static/wiki/font-awesome/scss/solid.scss`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.eot` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.svg` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.ttf` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.woff` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.woff2` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.eot` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.svg` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.ttf` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.woff` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.woff2` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.eot` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.svg` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.ttf` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.woff` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.woff2` & `wiki-0.9/src/wiki/static/wiki/font-awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/img/github_icon.png` & `wiki-0.9/src/wiki/static/wiki/img/github_icon.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/diff.js` & `wiki-0.9/src/wiki/static/wiki/js/diff.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/diffview.js` & `wiki-0.9/src/wiki/static/wiki/js/diffview.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/editor.js` & `wiki-0.9/src/wiki/static/wiki/js/editor.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/forms.js` & `wiki-0.9/src/wiki/static/wiki/js/forms.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/jquery-3.4.1.min.js` & `wiki-0.9/src/wiki/static/wiki/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/jquery-3.6.0.min.js` & `wiki-0.9/src/wiki/static/wiki/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/popper.js` & `wiki-0.9/src/wiki/static/wiki/js/popper.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/popper.min.js.map` & `wiki-0.9/src/wiki/static/wiki/js/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/respond.min.js` & `wiki-0.9/src/wiki/static/wiki/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/js/urlify.js` & `wiki-0.9/src/wiki/static/wiki/js/urlify.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/jquery.markitup.js` & `wiki-0.9/src/wiki/static/wiki/markitup/jquery.markitup.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/code.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/code.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/picture.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/picture.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/preview.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/preview.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/images/quotes.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/images/quotes.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/set.js` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/set.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/admin/style.css` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/admin/style.css`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/clean.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/clean.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/image.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/image.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/picture.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/picture.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/images/preview.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/default/images/preview.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/set.js` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/default/set.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/default/style.css` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/default/style.css`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/code.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/code.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/picture.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/picture.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/preview.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/preview.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/images/quotes.png` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/images/quotes.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/set.js` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/set.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/sets/frontend/style.css` & `wiki-0.9/src/wiki/static/wiki/markitup/sets/frontend/style.css`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-bbcode.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-bbcode.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-dotclear.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-dotclear.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-html.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-html.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-json.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-json.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-markdown.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-markdown.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-textile.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-textile.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-wiki.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-wiki.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-xml.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-xml.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/images/bg-editor.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/markitup/style.css` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/markitup/style.css`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/simple/images/menu.png` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/simple/images/menu.png`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/markitup/skins/simple/style.css` & `wiki-0.9/src/wiki/static/wiki/markitup/skins/simple/style.css`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/select2/css/select2.min.css` & `wiki-0.9/src/wiki/static/wiki/select2/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/static/wiki/select2/js/select2.min.js` & `wiki-0.9/src/wiki/static/wiki/select2/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/accounts/login.html` & `wiki-0.9/src/wiki/templates/wiki/accounts/login.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/accounts/signup.html` & `wiki-0.9/src/wiki/templates/wiki/accounts/signup.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/article.html` & `wiki-0.9/src/wiki/templates/wiki/article.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/base_site.html` & `wiki-0.9/src/wiki/templates/wiki/base_site.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/create.html` & `wiki-0.9/src/wiki/templates/wiki/create.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/create_root.html` & `wiki-0.9/src/wiki/templates/wiki/create_root.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/delete.html` & `wiki-0.9/src/wiki/templates/wiki/delete.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/deleted.html` & `wiki-0.9/src/wiki/templates/wiki/deleted.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/deleted_list.html` & `wiki-0.9/src/wiki/templates/wiki/deleted_list.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/dir.html` & `wiki-0.9/src/wiki/templates/wiki/dir.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/edit.html` & `wiki-0.9/src/wiki/templates/wiki/edit.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/error.html` & `wiki-0.9/src/wiki/templates/wiki/error.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/history.html` & `wiki-0.9/src/wiki/templates/wiki/history.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/includes/article_menu.html` & `wiki-0.9/src/wiki/templates/wiki/includes/article_menu.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/includes/breadcrumbs.html` & `wiki-0.9/src/wiki/templates/wiki/includes/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/includes/editor_sidebar.html` & `wiki-0.9/src/wiki/templates/wiki/includes/editor_sidebar.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/includes/formfield.html` & `wiki-0.9/src/wiki/templates/wiki/includes/formfield.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/includes/move_tree.html` & `wiki-0.9/src/wiki/templates/wiki/includes/move_tree.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/includes/pagination.html` & `wiki-0.9/src/wiki/templates/wiki/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/includes/render.html` & `wiki-0.9/src/wiki/templates/wiki/includes/render.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/includes/revision_info.html` & `wiki-0.9/src/wiki/templates/wiki/includes/revision_info.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/includes/searchresult.html` & `wiki-0.9/src/wiki/templates/wiki/includes/searchresult.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/move.html` & `wiki-0.9/src/wiki/templates/wiki/move.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/permission_denied.html` & `wiki-0.9/src/wiki/templates/wiki/permission_denied.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/preview_inline.html` & `wiki-0.9/src/wiki/templates/wiki/preview_inline.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/root_missing.html` & `wiki-0.9/src/wiki/templates/wiki/root_missing.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/search.html` & `wiki-0.9/src/wiki/templates/wiki/search.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templates/wiki/settings.html` & `wiki-0.9/src/wiki/templates/wiki/settings.html`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/templatetags/wiki_tags.py` & `wiki-0.9/src/wiki/templatetags/wiki_tags.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/urls.py` & `wiki-0.9/src/wiki/urls.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/views/accounts.py` & `wiki-0.9/src/wiki/views/accounts.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/views/article.py` & `wiki-0.9/src/wiki/views/article.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/views/deleted_list.py` & `wiki-0.9/src/wiki/views/deleted_list.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki/views/mixins.py` & `wiki-0.9/src/wiki/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki.egg-info/PKG-INFO` & `wiki-0.9/src/wiki.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiki
-Version: 0.8.2
+Version: 0.9
 Summary: A wiki system written for the Django framework.
 Home-page: http://www.django-wiki.org
 Author: Benjamin Bach
 Author-email: benjamin@overtag.dk
 License: GPLv3
 Description: django-wiki
         ===========
@@ -28,14 +28,17 @@
         --------------
         
         The below table explains which Django versions are supported.
         
         +------------------+----------------+--------------+
         | Release          | Django         | Upgrade from |
         +==================+================+==============+
+        | 0.9.x            | 2.2, 3.0, 3.1, | 0.7          |
+        |                  | 3.2, 4.0       |              |
+        +------------------+----------------+--------------+
         | 0.8.x            | 2.2, 3.0, 3.1, | 0.7          |
         |                  | 3.2, 4.0       |              |
         +------------------+----------------+--------------+
         | 0.7.x            | 2.2, 3.0, 3.1, | 0.5 or 0.6   |
         |                  | 3.2            |              |
         +------------------+----------------+--------------+
         | 0.6.x            | 2.1, 2.2, 3.0  | 0.5          |
@@ -245,16 +248,14 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `wiki-0.8.2/src/wiki.egg-info/SOURCES.txt` & `wiki-0.9/src/wiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wiki-0.8.2/src/wiki.egg-info/requires.txt` & `wiki-0.9/src/wiki.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Django<4.1,>=2.1
-bleach<4.2,>=3.3.0
+bleach[css]>=5
+tinycss2
 Pillow
 django-nyt<1.3,>=1.2.2
 django-mptt<0.14,>=0.13
 django-sekizai>=0.10
 sorl-thumbnail<13,>=12.8
 Markdown<3.4,>=3.3
```

