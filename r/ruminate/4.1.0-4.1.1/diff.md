# Comparing `tmp/ruminate-4.1.0.tar.gz` & `tmp/ruminate-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruminate-4.1.0.tar", last modified: Thu May 11 14:38:52 2023, max compression
+gzip compressed data, was "ruminate-4.1.1.tar", last modified: Mon May 15 09:47:51 2023, max compression
```

## Comparing `ruminate-4.1.0.tar` & `ruminate-4.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.513258 ruminate-4.1.0/
--rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 ruminate-4.1.0/AUTHORS.txt
--rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 ruminate-4.1.0/LICENSE.txt
--rw-r--r--   0 work       (505) staff       (20)      285 2022-11-21 19:51:25.000000 ruminate-4.1.0/MANIFEST.in
--rw-r--r--   0 work       (505) staff       (20)     1270 2023-05-11 14:38:52.513395 ruminate-4.1.0/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)      562 2023-05-11 13:34:00.000000 ruminate-4.1.0/README.md
--rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 ruminate-4.1.0/pyproject.toml
--rw-r--r--   0 work       (505) staff       (20)     1351 2023-05-11 14:38:52.514855 ruminate-4.1.0/setup.cfg
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.433602 ruminate-4.1.0/src/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.468110 ruminate-4.1.0/src/ruminate/
--rw-r--r--   0 work       (505) staff       (20)       77 2022-04-08 09:33:08.000000 ruminate-4.1.0/src/ruminate/__init__.py
--rw-r--r--   0 work       (505) staff       (20)      446 2023-02-17 09:43:25.000000 ruminate-4.1.0/src/ruminate/admin_urls.py
--rw-r--r--   0 work       (505) staff       (20)     1706 2023-03-08 12:43:47.000000 ruminate-4.1.0/src/ruminate/apps.py
--rw-r--r--   0 work       (505) staff       (20)    18096 2023-03-30 17:09:47.000000 ruminate-4.1.0/src/ruminate/blocks.py
--rw-r--r--   0 work       (505) staff       (20)      818 2023-03-30 17:09:37.000000 ruminate-4.1.0/src/ruminate/default_settings.py
--rw-r--r--   0 work       (505) staff       (20)      168 2022-10-21 23:47:25.000000 ruminate-4.1.0/src/ruminate/html_to_text.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.484188 ruminate-4.1.0/src/ruminate/migrations/
--rw-r--r--   0 work       (505) staff       (20)     9321 2023-05-11 13:35:28.000000 ruminate-4.1.0/src/ruminate/migrations/0001_initial.py
--rw-r--r--   0 work       (505) staff       (20)        0 2022-03-23 11:18:41.000000 ruminate-4.1.0/src/ruminate/migrations/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     1710 2023-02-17 09:56:57.000000 ruminate-4.1.0/src/ruminate/model_admin.py
--rw-r--r--   0 work       (505) staff       (20)     1333 2023-02-16 20:52:58.000000 ruminate-4.1.0/src/ruminate/model_fields.py
--rw-r--r--   0 work       (505) staff       (20)     1412 2023-02-18 22:30:10.000000 ruminate-4.1.0/src/ruminate/model_porter.py
--rw-r--r--   0 work       (505) staff       (20)    15736 2023-05-11 13:35:28.000000 ruminate-4.1.0/src/ruminate/models.py
--rw-r--r--   0 work       (505) staff       (20)     4005 2023-02-17 09:45:29.000000 ruminate-4.1.0/src/ruminate/preview.py
--rw-r--r--   0 work       (505) staff       (20)     1086 2023-02-17 09:39:27.000000 ruminate-4.1.0/src/ruminate/side_panels.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.433996 ruminate-4.1.0/src/ruminate/static/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.434086 ruminate-4.1.0/src/ruminate/static/ruminate/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.486407 ruminate-4.1.0/src/ruminate/static/ruminate/css/
--rw-r--r--   0 work       (505) staff       (20)     8459 2022-05-12 17:49:22.000000 ruminate-4.1.0/src/ruminate/static/ruminate/css/fonts.css
--rw-r--r--   0 work       (505) staff       (20)       76 2023-02-04 22:17:34.000000 ruminate-4.1.0/src/ruminate/static/ruminate/css/ruminate_admin.css
--rw-r--r--   0 work       (505) staff       (20)     8243 2022-07-18 22:56:35.000000 ruminate-4.1.0/src/ruminate/static/ruminate/css/text.css
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.434328 ruminate-4.1.0/src/ruminate/templates/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.490713 ruminate-4.1.0/src/ruminate/templates/ruminate/
--rw-r--r--   0 work       (505) staff       (20)       92 2023-02-18 21:24:32.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/article.html
--rw-r--r--   0 work       (505) staff       (20)      605 2023-05-11 13:35:28.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/article_endnotes.html
--rw-r--r--   0 work       (505) staff       (20)        0 2023-03-05 21:37:11.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/article_index_page.html
--rw-r--r--   0 work       (505) staff       (20)      288 2023-03-30 17:22:02.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/article_page.html
--rw-r--r--   0 work       (505) staff       (20)     1066 2023-02-17 10:14:27.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/article_preview.html
--rw-r--r--   0 work       (505) staff       (20)     1526 2023-02-18 21:30:32.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/base_page.html
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.512507 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/
--rw-r--r--   0 work       (505) staff       (20)      440 2023-02-17 16:05:08.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/article_block.html
--rw-r--r--   0 work       (505) staff       (20)     1836 2023-03-30 17:09:11.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/article_boilerplate.html
--rw-r--r--   0 work       (505) staff       (20)      342 2023-02-27 12:44:00.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/article_boilerplate_block.html
--rw-r--r--   0 work       (505) staff       (20)     1233 2023-05-11 13:35:28.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/article_content_block.html
--rw-r--r--   0 work       (505) staff       (20)      752 2023-05-11 13:35:28.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/article_references_block.html
--rw-r--r--   0 work       (505) staff       (20)       50 2023-03-30 17:08:10.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/article_tags_block.html
--rw-r--r--   0 work       (505) staff       (20)      202 2023-02-17 19:47:24.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/minimal_intro_block.html
--rw-r--r--   0 work       (505) staff       (20)      174 2023-02-07 13:37:37.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/none_intro_block.html
--rw-r--r--   0 work       (505) staff       (20)      354 2023-05-11 13:35:28.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/note_block.html
--rw-r--r--   0 work       (505) staff       (20)      268 2023-05-11 13:35:28.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/person_block.html
--rw-r--r--   0 work       (505) staff       (20)      861 2022-04-19 12:09:05.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/preface_block.html
--rw-r--r--   0 work       (505) staff       (20)      305 2023-05-11 13:35:28.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/section_block.html
--rw-r--r--   0 work       (505) staff       (20)      542 2023-02-20 14:18:57.000000 ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/spread_intro_block.html
--rw-r--r--   0 work       (505) staff       (20)       60 2022-03-23 11:18:41.000000 ruminate-4.1.0/src/ruminate/tests.py
--rw-r--r--   0 work       (505) staff       (20)     1468 2023-02-18 18:17:27.000000 ruminate-4.1.0/src/ruminate/wagtail_hooks.py
--rw-r--r--   0 work       (505) staff       (20)      702 2023-02-18 21:21:33.000000 ruminate-4.1.0/src/ruminate/wagtail_settings.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:38:52.478057 ruminate-4.1.0/src/ruminate.egg-info/
--rw-r--r--   0 work       (505) staff       (20)     1270 2023-05-11 14:38:52.000000 ruminate-4.1.0/src/ruminate.egg-info/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)     2008 2023-05-11 14:38:52.000000 ruminate-4.1.0/src/ruminate.egg-info/SOURCES.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 14:38:52.000000 ruminate-4.1.0/src/ruminate.egg-info/dependency_links.txt
--rw-r--r--   0 work       (505) staff       (20)      495 2023-05-11 14:38:52.000000 ruminate-4.1.0/src/ruminate.egg-info/requires.txt
--rw-r--r--   0 work       (505) staff       (20)        9 2023-05-11 14:38:52.000000 ruminate-4.1.0/src/ruminate.egg-info/top_level.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 14:38:52.000000 ruminate-4.1.0/src/ruminate.egg-info/zip-safe
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.542030 ruminate-4.1.1/
+-rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 ruminate-4.1.1/AUTHORS.txt
+-rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 ruminate-4.1.1/LICENSE.txt
+-rw-r--r--   0 work       (505) staff       (20)      285 2022-11-21 19:51:25.000000 ruminate-4.1.1/MANIFEST.in
+-rw-r--r--   0 work       (505) staff       (20)     1270 2023-05-15 09:47:51.542152 ruminate-4.1.1/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)      562 2023-05-11 13:34:00.000000 ruminate-4.1.1/README.md
+-rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 ruminate-4.1.1/pyproject.toml
+-rw-r--r--   0 work       (505) staff       (20)     1351 2023-05-15 09:47:51.543387 ruminate-4.1.1/setup.cfg
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.521915 ruminate-4.1.1/src/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.528178 ruminate-4.1.1/src/ruminate/
+-rw-r--r--   0 work       (505) staff       (20)       77 2022-04-08 09:33:08.000000 ruminate-4.1.1/src/ruminate/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)      446 2023-02-17 09:43:25.000000 ruminate-4.1.1/src/ruminate/admin_urls.py
+-rw-r--r--   0 work       (505) staff       (20)     1706 2023-03-08 12:43:47.000000 ruminate-4.1.1/src/ruminate/apps.py
+-rw-r--r--   0 work       (505) staff       (20)    18096 2023-03-30 17:09:47.000000 ruminate-4.1.1/src/ruminate/blocks.py
+-rw-r--r--   0 work       (505) staff       (20)      818 2023-03-30 17:09:37.000000 ruminate-4.1.1/src/ruminate/default_settings.py
+-rw-r--r--   0 work       (505) staff       (20)      168 2022-10-21 23:47:25.000000 ruminate-4.1.1/src/ruminate/html_to_text.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.535988 ruminate-4.1.1/src/ruminate/migrations/
+-rw-r--r--   0 work       (505) staff       (20)     9321 2023-05-11 13:35:28.000000 ruminate-4.1.1/src/ruminate/migrations/0001_initial.py
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-03-23 11:18:41.000000 ruminate-4.1.1/src/ruminate/migrations/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     1710 2023-02-17 09:56:57.000000 ruminate-4.1.1/src/ruminate/model_admin.py
+-rw-r--r--   0 work       (505) staff       (20)     1333 2023-02-16 20:52:58.000000 ruminate-4.1.1/src/ruminate/model_fields.py
+-rw-r--r--   0 work       (505) staff       (20)     1412 2023-02-18 22:30:10.000000 ruminate-4.1.1/src/ruminate/model_porter.py
+-rw-r--r--   0 work       (505) staff       (20)    17231 2023-05-15 09:47:39.000000 ruminate-4.1.1/src/ruminate/models.py
+-rw-r--r--   0 work       (505) staff       (20)     4005 2023-02-17 09:45:29.000000 ruminate-4.1.1/src/ruminate/preview.py
+-rw-r--r--   0 work       (505) staff       (20)     1086 2023-02-17 09:39:27.000000 ruminate-4.1.1/src/ruminate/side_panels.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.522273 ruminate-4.1.1/src/ruminate/static/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.522357 ruminate-4.1.1/src/ruminate/static/ruminate/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.536728 ruminate-4.1.1/src/ruminate/static/ruminate/css/
+-rw-r--r--   0 work       (505) staff       (20)     8459 2022-05-12 17:49:22.000000 ruminate-4.1.1/src/ruminate/static/ruminate/css/fonts.css
+-rw-r--r--   0 work       (505) staff       (20)       76 2023-02-04 22:17:34.000000 ruminate-4.1.1/src/ruminate/static/ruminate/css/ruminate_admin.css
+-rw-r--r--   0 work       (505) staff       (20)     8243 2022-07-18 22:56:35.000000 ruminate-4.1.1/src/ruminate/static/ruminate/css/text.css
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.522574 ruminate-4.1.1/src/ruminate/templates/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.538208 ruminate-4.1.1/src/ruminate/templates/ruminate/
+-rw-r--r--   0 work       (505) staff       (20)       92 2023-02-18 21:24:32.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/article.html
+-rw-r--r--   0 work       (505) staff       (20)      605 2023-05-11 13:35:28.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/article_endnotes.html
+-rw-r--r--   0 work       (505) staff       (20)        0 2023-03-05 21:37:11.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/article_index_page.html
+-rw-r--r--   0 work       (505) staff       (20)      288 2023-03-30 17:22:02.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/article_page.html
+-rw-r--r--   0 work       (505) staff       (20)     1066 2023-02-17 10:14:27.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/article_preview.html
+-rw-r--r--   0 work       (505) staff       (20)     1526 2023-02-18 21:30:32.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/base_page.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.541792 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/
+-rw-r--r--   0 work       (505) staff       (20)      440 2023-02-17 16:05:08.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/article_block.html
+-rw-r--r--   0 work       (505) staff       (20)     1836 2023-03-30 17:09:11.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/article_boilerplate.html
+-rw-r--r--   0 work       (505) staff       (20)      342 2023-02-27 12:44:00.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/article_boilerplate_block.html
+-rw-r--r--   0 work       (505) staff       (20)     1233 2023-05-11 13:35:28.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/article_content_block.html
+-rw-r--r--   0 work       (505) staff       (20)      752 2023-05-11 13:35:28.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/article_references_block.html
+-rw-r--r--   0 work       (505) staff       (20)       50 2023-03-30 17:08:10.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/article_tags_block.html
+-rw-r--r--   0 work       (505) staff       (20)      202 2023-02-17 19:47:24.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/minimal_intro_block.html
+-rw-r--r--   0 work       (505) staff       (20)      174 2023-02-07 13:37:37.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/none_intro_block.html
+-rw-r--r--   0 work       (505) staff       (20)      354 2023-05-11 13:35:28.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/note_block.html
+-rw-r--r--   0 work       (505) staff       (20)      268 2023-05-11 13:35:28.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/person_block.html
+-rw-r--r--   0 work       (505) staff       (20)      861 2022-04-19 12:09:05.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/preface_block.html
+-rw-r--r--   0 work       (505) staff       (20)      305 2023-05-11 13:35:28.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/section_block.html
+-rw-r--r--   0 work       (505) staff       (20)      542 2023-02-20 14:18:57.000000 ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/spread_intro_block.html
+-rw-r--r--   0 work       (505) staff       (20)       60 2022-03-23 11:18:41.000000 ruminate-4.1.1/src/ruminate/tests.py
+-rw-r--r--   0 work       (505) staff       (20)     1468 2023-02-18 18:17:27.000000 ruminate-4.1.1/src/ruminate/wagtail_hooks.py
+-rw-r--r--   0 work       (505) staff       (20)      702 2023-02-18 21:21:33.000000 ruminate-4.1.1/src/ruminate/wagtail_settings.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-15 09:47:51.535375 ruminate-4.1.1/src/ruminate.egg-info/
+-rw-r--r--   0 work       (505) staff       (20)     1270 2023-05-15 09:47:51.000000 ruminate-4.1.1/src/ruminate.egg-info/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)     2008 2023-05-15 09:47:51.000000 ruminate-4.1.1/src/ruminate.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-15 09:47:51.000000 ruminate-4.1.1/src/ruminate.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (505) staff       (20)      495 2023-05-15 09:47:51.000000 ruminate-4.1.1/src/ruminate.egg-info/requires.txt
+-rw-r--r--   0 work       (505) staff       (20)        9 2023-05-15 09:47:51.000000 ruminate-4.1.1/src/ruminate.egg-info/top_level.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-15 09:47:51.000000 ruminate-4.1.1/src/ruminate.egg-info/zip-safe
```

### Comparing `ruminate-4.1.0/LICENSE.txt` & `ruminate-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/PKG-INFO` & `ruminate-4.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruminate
-Version: 4.1.0
+Version: 4.1.1
 Summary: A Wagtail app for publishing article pages in an academic/scientifically-oriented setting.
 Home-page: https://github.com/high-dimensional/ruminate
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `ruminate-4.1.0/README.md` & `ruminate-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/setup.cfg` & `ruminate-4.1.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ruminate
-version = 4.1.0
+version = 4.1.1
 url = https://github.com/high-dimensional/ruminate
 author = High Dimensional Neurology Group, UCL
 author_email = pypi@highdimensional.net
 description = A Wagtail app for publishing article pages in an academic/scientifically-oriented setting.
 long_description = file:README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
```

### Comparing `ruminate-4.1.0/src/ruminate/apps.py` & `ruminate-4.1.1/src/ruminate/apps.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/blocks.py` & `ruminate-4.1.1/src/ruminate/blocks.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/default_settings.py` & `ruminate-4.1.1/src/ruminate/default_settings.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/migrations/0001_initial.py` & `ruminate-4.1.1/src/ruminate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/model_admin.py` & `ruminate-4.1.1/src/ruminate/model_admin.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/model_fields.py` & `ruminate-4.1.1/src/ruminate/model_fields.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/model_porter.py` & `ruminate-4.1.1/src/ruminate/model_porter.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/models.py` & `ruminate-4.1.1/src/ruminate/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 import modelcluster.models
 from django.db import models as django_models
 from django.db.models import ForeignKey
 from django.db import transaction
 from django.conf import settings
 from django.http import Http404
 from django.utils import timezone
-from django.utils.translation import gettext_lazy as _
+from django.utils.translation import gettext_lazy as _, get_language_from_request
 from django.utils.functional import cached_property, classproperty
 from django.template.loader import render_to_string
 from django.core.exceptions import ValidationError
 from django.shortcuts import redirect
 
 from django.template.response import TemplateResponse
 
 # Wagtail
 
 from wagtail.snippets.models import register_snippet
 from wagtail.contrib.routable_page.models import RoutablePageMixin, path
-from wagtail.models import (Page, Orderable, TranslatableMixin, DraftStateMixin, RevisionMixin, PreviewableMixin, Site)
+from wagtail.models import (Page, Orderable, TranslatableMixin, DraftStateMixin, RevisionMixin, PreviewableMixin, Site,
+                            Locale)
 
 from wagtail.rich_text import RichText
 from wagtail_preference_blocks.decorators import provides_preferences_context
 
 from modelcluster.fields import ParentalKey
 from modelcluster.contrib.taggit import ClusterTaggableManager
 from taggit.models import TagBase, ItemBase
@@ -335,21 +336,21 @@
             self.locale = self.get_default_locale()
 
         super().full_clean(*args, **kwargs)
 
     def clean(self):
         super().clean()
 
-        queryset = Article.objects.all().filter(year=self.year, month=self.month, day=self.day, slug=self.slug)
+        queryset = Article.objects.all().filter(year=self.year, month=self.month, day=self.day, slug=self.slug, locale=self.locale)
 
         if self.id:
             queryset = queryset.exclude(id=self.id)
 
         if queryset.exists():
-            raise ValidationError({"slug": _("This slug is already in use")})
+            raise ValidationError({"slug": _("The slug '%s' is already in use for locale %s" % (self.slug, str(self.locale)))})
 
     def sync_synopsis(self, synopsis):
         super(Article, self).sync_synopsis(synopsis)
 
         synopsis.heading = self.title
         synopsis.created_at = self.first_published_at or timezone.now()
         synopsis.updated_at = self.last_published_at
@@ -400,16 +401,26 @@
         if current_site is None:
             current_site = Site.objects.get(is_default_site=True)
 
         ruminate_settings = RuminateSiteSettings.for_site(current_site)
 
         if not ruminate_settings.canonical_article_index_page or not self.first_published_at:
             return ''
+        
+        canonical_index_page = ruminate_settings.canonical_article_index_page
+        localized_index_page = canonical_index_page.get_translation_or_none(self.locale)
+
+        if localized_index_page is None:
+            default_locale = canonical_index_page.get_default_locale()
+            localized_index_page = canonical_index_page.get_translation_or_none(default_locale)
 
-        result = ruminate_settings.canonical_article_index_page.get_url(request=request, current_site=current_site)
+        if localized_index_page is None:
+            localized_index_page = canonical_index_page
+
+        result = localized_index_page.get_url(request=request, current_site=current_site)
         result = f"{result}{self.first_published_at.year}/{self.first_published_at.month}/{self.first_published_at.day}/{self.slug}/"
         return result
 
     _edit_handler = None
 
     @classproperty
     def edit_handler(cls):
@@ -494,15 +505,41 @@
             raise Http404('Not found.')
 
         return self.index_route(request)
 
     @path('<int:year>/<int:month>/<int:day>/<str:slug>/')
     def serve_article(self, request, year, month, day, slug):
 
+        locale = self.locale
+
+        if locale is None:
+
+            language = get_language_from_request(request)
+
+            try:
+                locale = Locale.objects.get_for_language(language)
+            except Locale.DoesNotExist:
+                locale = Locale.get_active()
+
         try:
             article = Article.objects.get(live=True,
                                           first_published_at__year=year, first_published_at__month=month,
-                                          first_published_at__day=day, slug__iexact=slug)
+                                          first_published_at__day=day, slug__iexact=slug, locale_id=locale.id)
         except Article.DoesNotExist:
-            raise Http404('Not found.')
+
+            try:
+                locale = Locale.objects.get_for_language('en')
+            except Locale.DoesNotExist:
+                locale = None
+
+            articles = Article.objects.filter(
+                                        live=True,
+                                        first_published_at__year=year, first_published_at__month=month,
+                                        first_published_at__day=day, slug__iexact=slug, locale_id=locale.id).order_by(
+                'locale__language_code')
+
+            if not articles.exists():
+                raise Http404('Not found.')
+
+            article = articles.first()
 
         return article.serve(request)
```

### Comparing `ruminate-4.1.0/src/ruminate/preview.py` & `ruminate-4.1.1/src/ruminate/preview.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/side_panels.py` & `ruminate-4.1.1/src/ruminate/side_panels.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/static/ruminate/css/fonts.css` & `ruminate-4.1.1/src/ruminate/static/ruminate/css/fonts.css`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/static/ruminate/css/text.css` & `ruminate-4.1.1/src/ruminate/static/ruminate/css/text.css`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/templates/ruminate/article_endnotes.html` & `ruminate-4.1.1/src/ruminate/templates/ruminate/article_endnotes.html`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/templates/ruminate/article_preview.html` & `ruminate-4.1.1/src/ruminate/templates/ruminate/article_preview.html`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/templates/ruminate/base_page.html` & `ruminate-4.1.1/src/ruminate/templates/ruminate/base_page.html`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/article_boilerplate.html` & `ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/article_boilerplate.html`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/article_content_block.html` & `ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/article_content_block.html`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/article_references_block.html` & `ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/article_references_block.html`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/preface_block.html` & `ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/preface_block.html`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/templates/ruminate/blocks/spread_intro_block.html` & `ruminate-4.1.1/src/ruminate/templates/ruminate/blocks/spread_intro_block.html`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/wagtail_hooks.py` & `ruminate-4.1.1/src/ruminate/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate/wagtail_settings.py` & `ruminate-4.1.1/src/ruminate/wagtail_settings.py`

 * *Files identical despite different names*

### Comparing `ruminate-4.1.0/src/ruminate.egg-info/PKG-INFO` & `ruminate-4.1.1/src/ruminate.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruminate
-Version: 4.1.0
+Version: 4.1.1
 Summary: A Wagtail app for publishing article pages in an academic/scientifically-oriented setting.
 Home-page: https://github.com/high-dimensional/ruminate
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `ruminate-4.1.0/src/ruminate.egg-info/SOURCES.txt` & `ruminate-4.1.1/src/ruminate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

