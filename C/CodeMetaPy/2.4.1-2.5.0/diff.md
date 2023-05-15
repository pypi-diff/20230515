# Comparing `tmp/CodeMetaPy-2.4.1.tar.gz` & `tmp/CodeMetaPy-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodeMetaPy-2.4.1.tar", last modified: Wed Mar 15 21:40:48 2023, max compression
+gzip compressed data, was "CodeMetaPy-2.5.0.tar", last modified: Mon May 15 16:13:05 2023, max compression
```

## Comparing `CodeMetaPy-2.4.1.tar` & `CodeMetaPy-2.5.0.tar`

### file list

```diff
@@ -1,91 +1,52 @@
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-15 21:40:48.244331 CodeMetaPy-2.4.1/
--rw-r--r--   0 proycon   (1000) users      (100)       98 2018-04-16 08:54:17.000000 CodeMetaPy-2.4.1/.gitmodules
--rw-r--r--   0 proycon   (1000) users      (100)    35147 2018-04-16 12:03:01.000000 CodeMetaPy-2.4.1/COPYING
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-15 21:40:48.234332 CodeMetaPy-2.4.1/CodeMetaPy.egg-info/
--rw-r--r--   0 proycon   (1000) users      (100)    11485 2023-03-15 21:40:48.000000 CodeMetaPy-2.4.1/CodeMetaPy.egg-info/PKG-INFO
--rw-r--r--   0 proycon   (1000) users      (100)     2505 2023-03-15 21:40:48.000000 CodeMetaPy-2.4.1/CodeMetaPy.egg-info/SOURCES.txt
--rw-r--r--   0 proycon   (1000) users      (100)        1 2023-03-15 21:40:48.000000 CodeMetaPy-2.4.1/CodeMetaPy.egg-info/dependency_links.txt
--rw-r--r--   0 proycon   (1000) users      (100)       55 2023-03-15 21:40:48.000000 CodeMetaPy-2.4.1/CodeMetaPy.egg-info/entry_points.txt
--rw-r--r--   0 proycon   (1000) users      (100)        1 2019-11-20 15:03:05.000000 CodeMetaPy-2.4.1/CodeMetaPy.egg-info/not-zip-safe
--rw-r--r--   0 proycon   (1000) users      (100)      127 2023-03-15 21:40:48.000000 CodeMetaPy-2.4.1/CodeMetaPy.egg-info/requires.txt
--rw-r--r--   0 proycon   (1000) users      (100)        9 2023-03-15 21:40:48.000000 CodeMetaPy-2.4.1/CodeMetaPy.egg-info/top_level.txt
--rw-r--r--   0 proycon   (1000) users      (100)       83 2018-04-23 13:28:45.000000 CodeMetaPy-2.4.1/MANIFEST.in
--rw-r--r--   0 proycon   (1000) users      (100)    11485 2023-03-15 21:40:48.240998 CodeMetaPy-2.4.1/PKG-INFO
--rw-r--r--   0 proycon   (1000) users      (100)    10538 2022-10-19 11:24:40.000000 CodeMetaPy-2.4.1/README.md
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-15 21:40:48.234332 CodeMetaPy-2.4.1/codemeta/
--rw-r--r--   0 proycon   (1000) users      (100)        0 2018-04-23 13:28:45.000000 CodeMetaPy-2.4.1/codemeta/__init__.py
--rwxr-xr-x   0 proycon   (1000) users      (100)    26387 2023-02-28 14:22:42.000000 CodeMetaPy-2.4.1/codemeta/codemeta.py
--rw-r--r--   0 proycon   (1000) users      (100)    51902 2023-03-14 22:34:13.000000 CodeMetaPy-2.4.1/codemeta/common.py
--rw-r--r--   0 proycon   (1000) users      (100)     1489 2022-03-08 14:45:00.000000 CodeMetaPy-2.4.1/codemeta/crosswalk.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-15 21:40:48.234332 CodeMetaPy-2.4.1/codemeta/parsers/
--rw-r--r--   0 proycon   (1000) users      (100)        0 2022-03-03 09:35:06.000000 CodeMetaPy-2.4.1/codemeta/parsers/__init__.py
--rw-r--r--   0 proycon   (1000) users      (100)      844 2022-03-21 12:54:21.000000 CodeMetaPy-2.4.1/codemeta/parsers/authors.py
--rw-r--r--   0 proycon   (1000) users      (100)     4395 2022-10-17 13:23:41.000000 CodeMetaPy-2.4.1/codemeta/parsers/debian.py
--rw-r--r--   0 proycon   (1000) users      (100)    11312 2022-10-10 10:05:12.000000 CodeMetaPy-2.4.1/codemeta/parsers/gitapi.py
--rw-r--r--   0 proycon   (1000) users      (100)     6974 2023-03-02 12:17:41.000000 CodeMetaPy-2.4.1/codemeta/parsers/java.py
--rw-r--r--   0 proycon   (1000) users      (100)     7965 2022-11-21 16:18:41.000000 CodeMetaPy-2.4.1/codemeta/parsers/jsonld.py
--rw-r--r--   0 proycon   (1000) users      (100)     8381 2023-03-14 10:06:56.000000 CodeMetaPy-2.4.1/codemeta/parsers/nodejs.py
--rw-r--r--   0 proycon   (1000) users      (100)    16781 2023-03-01 11:48:34.000000 CodeMetaPy-2.4.1/codemeta/parsers/python.py
--rw-r--r--   0 proycon   (1000) users      (100)     3033 2023-03-01 13:18:45.000000 CodeMetaPy-2.4.1/codemeta/parsers/rust.py
--rw-r--r--   0 proycon   (1000) users      (100)     9519 2022-10-16 21:04:03.000000 CodeMetaPy-2.4.1/codemeta/parsers/web.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-15 21:40:48.237665 CodeMetaPy-2.4.1/codemeta/resources/
--rw-r--r--   0 proycon   (1000) users      (100)     9860 2023-03-15 21:34:36.000000 CodeMetaPy-2.4.1/codemeta/resources/codemeta.css
--rw-r--r--   0 proycon   (1000) users      (100)    92136 2022-03-23 23:19:48.000000 CodeMetaPy-2.4.1/codemeta/resources/fa-brands-400.woff
--rw-r--r--   0 proycon   (1000) users      (100)    78460 2022-03-23 23:19:48.000000 CodeMetaPy-2.4.1/codemeta/resources/fa-brands-400.woff2
--rw-r--r--   0 proycon   (1000) users      (100)    16772 2022-03-23 23:19:48.000000 CodeMetaPy-2.4.1/codemeta/resources/fa-regular-400.woff
--rw-r--r--   0 proycon   (1000) users      (100)    13548 2022-03-23 23:19:48.000000 CodeMetaPy-2.4.1/codemeta/resources/fa-regular-400.woff2
--rw-r--r--   0 proycon   (1000) users      (100)   104280 2022-03-23 23:19:48.000000 CodeMetaPy-2.4.1/codemeta/resources/fa-solid-900.woff
--rw-r--r--   0 proycon   (1000) users      (100)    80300 2022-03-23 23:19:48.000000 CodeMetaPy-2.4.1/codemeta/resources/fa-solid-900.woff2
--rw-r--r--   0 proycon   (1000) users      (100)    69146 2022-03-23 23:29:07.000000 CodeMetaPy-2.4.1/codemeta/resources/fontawesome.css
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-15 21:40:48.237665 CodeMetaPy-2.4.1/codemeta/schema/
--rw-r--r--   0 proycon   (1000) users      (100)       43 2018-04-16 08:54:17.000000 CodeMetaPy-2.4.1/codemeta/schema/.git
--rw-r--r--   0 proycon   (1000) users      (100)       60 2022-03-06 15:55:01.000000 CodeMetaPy-2.4.1/codemeta/schema/.gitignore
--rw-r--r--   0 proycon   (1000) users      (100)       82 2022-03-23 13:34:21.000000 CodeMetaPy-2.4.1/codemeta/schema/.gitmodules
--rw-r--r--   0 proycon   (1000) users      (100)      367 2019-11-14 10:56:02.000000 CodeMetaPy-2.4.1/codemeta/schema/.travis.yml
--rw-r--r--   0 proycon   (1000) users      (100)     2326 2019-11-14 10:56:02.000000 CodeMetaPy-2.4.1/codemeta/schema/CONTRIBUTING.md
--rw-r--r--   0 proycon   (1000) users      (100)     1391 2019-11-14 10:56:02.000000 CodeMetaPy-2.4.1/codemeta/schema/CONTRIBUTORS.MD
--rw-r--r--   0 proycon   (1000) users      (100)    11324 2018-04-16 08:54:17.000000 CodeMetaPy-2.4.1/codemeta/schema/LICENSE
--rw-r--r--   0 proycon   (1000) users      (100)     5912 2019-11-14 10:56:02.000000 CodeMetaPy-2.4.1/codemeta/schema/README.md
--rw-r--r--   0 proycon   (1000) users      (100)     4727 2022-03-06 15:55:01.000000 CodeMetaPy-2.4.1/codemeta/schema/codemeta.json
--rw-r--r--   0 proycon   (1000) users      (100)     4376 2022-03-06 15:55:01.000000 CodeMetaPy-2.4.1/codemeta/schema/codemeta.jsonld
--rw-r--r--   0 proycon   (1000) users      (100)    14995 2022-03-06 15:55:01.000000 CodeMetaPy-2.4.1/codemeta/schema/crosswalk.csv
--rw-r--r--   0 proycon   (1000) users      (100)     9200 2022-03-06 15:55:01.000000 CodeMetaPy-2.4.1/codemeta/schema/properties_description.csv
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-15 21:40:48.240998 CodeMetaPy-2.4.1/codemeta/serializers/
--rw-r--r--   0 proycon   (1000) users      (100)        0 2022-03-08 10:50:22.000000 CodeMetaPy-2.4.1/codemeta/serializers/__init__.py
--rw-r--r--   0 proycon   (1000) users      (100)    13211 2023-03-01 12:34:05.000000 CodeMetaPy-2.4.1/codemeta/serializers/html.py
--rw-r--r--   0 proycon   (1000) users      (100)    14738 2023-02-28 19:06:57.000000 CodeMetaPy-2.4.1/codemeta/serializers/jsonld.py
--rw-r--r--   0 proycon   (1000) users      (100)      655 2022-10-16 21:04:03.000000 CodeMetaPy-2.4.1/codemeta/serializers/turtle.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-15 21:40:48.240998 CodeMetaPy-2.4.1/codemeta/templates/
--rw-r--r--   0 proycon   (1000) users      (100)      296 2022-03-23 14:14:54.000000 CodeMetaPy-2.4.1/codemeta/templates/badge.html
--rw-r--r--   0 proycon   (1000) users      (100)    11390 2023-03-01 12:31:19.000000 CodeMetaPy-2.4.1/codemeta/templates/card_service.html
--rw-r--r--   0 proycon   (1000) users      (100)    12648 2022-10-19 12:17:29.000000 CodeMetaPy-2.4.1/codemeta/templates/card_softwaresourcecode.html
--rw-r--r--   0 proycon   (1000) users      (100)      866 2022-11-07 12:55:05.000000 CodeMetaPy-2.4.1/codemeta/templates/cardindex.html
--rw-r--r--   0 proycon   (1000) users      (100)     1142 2022-10-18 11:42:19.000000 CodeMetaPy-2.4.1/codemeta/templates/citation.html
--rw-r--r--   0 proycon   (1000) users      (100)     1382 2022-10-14 16:40:08.000000 CodeMetaPy-2.4.1/codemeta/templates/developmentstatus.html
--rw-r--r--   0 proycon   (1000) users      (100)      997 2022-10-13 20:29:16.000000 CodeMetaPy-2.4.1/codemeta/templates/footer.html
--rw-r--r--   0 proycon   (1000) users      (100)      725 2022-03-25 12:11:02.000000 CodeMetaPy-2.4.1/codemeta/templates/generic.html
--rw-r--r--   0 proycon   (1000) users      (100)     2440 2022-11-03 11:37:04.000000 CodeMetaPy-2.4.1/codemeta/templates/head.html
--rw-r--r--   0 proycon   (1000) users      (100)     1165 2023-03-15 21:28:41.000000 CodeMetaPy-2.4.1/codemeta/templates/header.html
--rw-r--r--   0 proycon   (1000) users      (100)     1925 2022-11-09 10:49:25.000000 CodeMetaPy-2.4.1/codemeta/templates/index.html
--rw-r--r--   0 proycon   (1000) users      (100)      901 2022-10-13 20:28:26.000000 CodeMetaPy-2.4.1/codemeta/templates/indexfooter.html
--rw-r--r--   0 proycon   (1000) users      (100)       76 2022-10-13 21:10:44.000000 CodeMetaPy-2.4.1/codemeta/templates/intro.html
--rw-r--r--   0 proycon   (1000) users      (100)     3546 2022-08-29 20:32:48.000000 CodeMetaPy-2.4.1/codemeta/templates/iodata.html
--rw-r--r--   0 proycon   (1000) users      (100)     5550 2023-03-01 12:34:00.000000 CodeMetaPy-2.4.1/codemeta/templates/item_softwaresourcecode.html
--rw-r--r--   0 proycon   (1000) users      (100)     3145 2022-11-02 16:27:19.000000 CodeMetaPy-2.4.1/codemeta/templates/item_targetproduct.html
--rw-r--r--   0 proycon   (1000) users      (100)      512 2022-04-07 22:35:36.000000 CodeMetaPy-2.4.1/codemeta/templates/page_generic.html
--rw-r--r--   0 proycon   (1000) users      (100)      401 2022-04-07 22:35:47.000000 CodeMetaPy-2.4.1/codemeta/templates/page_person_or_org.html
--rw-r--r--   0 proycon   (1000) users      (100)      456 2022-04-08 09:54:07.000000 CodeMetaPy-2.4.1/codemeta/templates/page_softwaresourcecode.html
--rw-r--r--   0 proycon   (1000) users      (100)      405 2022-09-01 11:51:27.000000 CodeMetaPy-2.4.1/codemeta/templates/page_targetproduct.html
--rw-r--r--   0 proycon   (1000) users      (100)     5011 2022-10-20 11:27:37.000000 CodeMetaPy-2.4.1/codemeta/templates/person_or_org.html
--rw-r--r--   0 proycon   (1000) users      (100)     1807 2022-04-08 10:12:06.000000 CodeMetaPy-2.4.1/codemeta/templates/person_or_org_minimal.html
--rw-r--r--   0 proycon   (1000) users      (100)     2075 2022-10-18 11:40:41.000000 CodeMetaPy-2.4.1/codemeta/templates/reference.html
--rw-r--r--   0 proycon   (1000) users      (100)     1642 2022-10-19 13:21:08.000000 CodeMetaPy-2.4.1/codemeta/templates/reference_author.html
--rw-r--r--   0 proycon   (1000) users      (100)     1109 2022-11-07 12:46:49.000000 CodeMetaPy-2.4.1/codemeta/templates/serviceindex.html
--rw-r--r--   0 proycon   (1000) users      (100)    22027 2023-03-15 21:36:49.000000 CodeMetaPy-2.4.1/codemeta/templates/softwaresourcecode.html
--rw-r--r--   0 proycon   (1000) users      (100)    13927 2023-03-15 21:39:37.000000 CodeMetaPy-2.4.1/codemeta/templates/targetproduct.html
--rw-r--r--   0 proycon   (1000) users      (100)     1043 2022-08-31 10:35:18.000000 CodeMetaPy-2.4.1/codemeta/templates/validationrating.html
--rw-r--r--   0 proycon   (1000) users      (100)     6304 2022-10-19 13:47:01.000000 CodeMetaPy-2.4.1/codemeta/validation.py
--rw-r--r--   0 proycon   (1000) users      (100)       38 2023-03-15 21:40:48.244331 CodeMetaPy-2.4.1/setup.cfg
--rwxr-xr-x   0 proycon   (1000) users      (100)     1942 2023-03-14 10:15:52.000000 CodeMetaPy-2.4.1/setup.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-15 21:40:48.240998 CodeMetaPy-2.4.1/tests/
--rw-r--r--   0 proycon   (1000) users      (100)    29681 2023-02-22 22:32:31.000000 CodeMetaPy-2.4.1/tests/tests.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:13:05.269822 CodeMetaPy-2.5.0/
+-rw-r--r--   0 proycon   (1000) users      (100)       98 2018-04-16 08:54:17.000000 CodeMetaPy-2.5.0/.gitmodules
+-rw-r--r--   0 proycon   (1000) users      (100)    35147 2018-04-16 12:03:01.000000 CodeMetaPy-2.5.0/COPYING
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:13:05.269822 CodeMetaPy-2.5.0/CodeMetaPy.egg-info/
+-rw-r--r--   0 proycon   (1000) users      (100)    11805 2023-05-15 16:13:05.000000 CodeMetaPy-2.5.0/CodeMetaPy.egg-info/PKG-INFO
+-rw-r--r--   0 proycon   (1000) users      (100)     1124 2023-05-15 16:13:05.000000 CodeMetaPy-2.5.0/CodeMetaPy.egg-info/SOURCES.txt
+-rw-r--r--   0 proycon   (1000) users      (100)        1 2023-05-15 16:13:05.000000 CodeMetaPy-2.5.0/CodeMetaPy.egg-info/dependency_links.txt
+-rw-r--r--   0 proycon   (1000) users      (100)       54 2023-05-15 16:13:05.000000 CodeMetaPy-2.5.0/CodeMetaPy.egg-info/entry_points.txt
+-rw-r--r--   0 proycon   (1000) users      (100)        1 2019-11-20 15:03:05.000000 CodeMetaPy-2.5.0/CodeMetaPy.egg-info/not-zip-safe
+-rw-r--r--   0 proycon   (1000) users      (100)      128 2023-05-15 16:13:05.000000 CodeMetaPy-2.5.0/CodeMetaPy.egg-info/requires.txt
+-rw-r--r--   0 proycon   (1000) users      (100)        9 2023-05-15 16:13:05.000000 CodeMetaPy-2.5.0/CodeMetaPy.egg-info/top_level.txt
+-rw-r--r--   0 proycon   (1000) users      (100)       83 2018-04-23 13:28:45.000000 CodeMetaPy-2.5.0/MANIFEST.in
+-rw-r--r--   0 proycon   (1000) users      (100)    11805 2023-05-15 16:13:05.269822 CodeMetaPy-2.5.0/PKG-INFO
+-rw-r--r--   0 proycon   (1000) users      (100)    10878 2023-05-12 12:52:49.000000 CodeMetaPy-2.5.0/README.md
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:13:05.269822 CodeMetaPy-2.5.0/codemeta/
+-rw-r--r--   0 proycon   (1000) users      (100)        0 2018-04-23 13:28:45.000000 CodeMetaPy-2.5.0/codemeta/__init__.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)    28483 2023-05-10 17:21:39.000000 CodeMetaPy-2.5.0/codemeta/codemeta.py
+-rw-r--r--   0 proycon   (1000) users      (100)    52327 2023-05-15 16:07:44.000000 CodeMetaPy-2.5.0/codemeta/common.py
+-rw-r--r--   0 proycon   (1000) users      (100)     1557 2023-05-10 13:31:57.000000 CodeMetaPy-2.5.0/codemeta/crosswalk.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:13:05.269822 CodeMetaPy-2.5.0/codemeta/parsers/
+-rw-r--r--   0 proycon   (1000) users      (100)        0 2022-03-03 09:35:06.000000 CodeMetaPy-2.5.0/codemeta/parsers/__init__.py
+-rw-r--r--   0 proycon   (1000) users      (100)      826 2023-05-10 13:41:52.000000 CodeMetaPy-2.5.0/codemeta/parsers/authors.py
+-rw-r--r--   0 proycon   (1000) users      (100)     4668 2023-05-10 13:41:58.000000 CodeMetaPy-2.5.0/codemeta/parsers/debian.py
+-rw-r--r--   0 proycon   (1000) users      (100)    11973 2023-05-10 13:42:16.000000 CodeMetaPy-2.5.0/codemeta/parsers/gitapi.py
+-rw-r--r--   0 proycon   (1000) users      (100)     7986 2023-05-10 13:42:41.000000 CodeMetaPy-2.5.0/codemeta/parsers/java.py
+-rw-r--r--   0 proycon   (1000) users      (100)     8533 2023-05-10 13:43:11.000000 CodeMetaPy-2.5.0/codemeta/parsers/jsonld.py
+-rw-r--r--   0 proycon   (1000) users      (100)    10151 2023-05-10 13:43:28.000000 CodeMetaPy-2.5.0/codemeta/parsers/nodejs.py
+-rw-r--r--   0 proycon   (1000) users      (100)    19621 2023-05-10 13:44:58.000000 CodeMetaPy-2.5.0/codemeta/parsers/python.py
+-rw-r--r--   0 proycon   (1000) users      (100)     3376 2023-05-10 13:45:54.000000 CodeMetaPy-2.5.0/codemeta/parsers/rust.py
+-rw-r--r--   0 proycon   (1000) users      (100)    11209 2023-05-12 13:46:24.000000 CodeMetaPy-2.5.0/codemeta/parsers/web.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:13:05.269822 CodeMetaPy-2.5.0/codemeta/schema/
+-rw-r--r--   0 proycon   (1000) users      (100)       43 2018-04-16 08:54:17.000000 CodeMetaPy-2.5.0/codemeta/schema/.git
+-rw-r--r--   0 proycon   (1000) users      (100)       60 2022-03-06 15:55:01.000000 CodeMetaPy-2.5.0/codemeta/schema/.gitignore
+-rw-r--r--   0 proycon   (1000) users      (100)       82 2022-03-23 13:34:21.000000 CodeMetaPy-2.5.0/codemeta/schema/.gitmodules
+-rw-r--r--   0 proycon   (1000) users      (100)      367 2019-11-14 10:56:02.000000 CodeMetaPy-2.5.0/codemeta/schema/.travis.yml
+-rw-r--r--   0 proycon   (1000) users      (100)     2326 2019-11-14 10:56:02.000000 CodeMetaPy-2.5.0/codemeta/schema/CONTRIBUTING.md
+-rw-r--r--   0 proycon   (1000) users      (100)     1391 2019-11-14 10:56:02.000000 CodeMetaPy-2.5.0/codemeta/schema/CONTRIBUTORS.MD
+-rw-r--r--   0 proycon   (1000) users      (100)    11324 2018-04-16 08:54:17.000000 CodeMetaPy-2.5.0/codemeta/schema/LICENSE
+-rw-r--r--   0 proycon   (1000) users      (100)     5912 2019-11-14 10:56:02.000000 CodeMetaPy-2.5.0/codemeta/schema/README.md
+-rw-r--r--   0 proycon   (1000) users      (100)     4727 2022-03-06 15:55:01.000000 CodeMetaPy-2.5.0/codemeta/schema/codemeta.json
+-rw-r--r--   0 proycon   (1000) users      (100)     4376 2022-03-06 15:55:01.000000 CodeMetaPy-2.5.0/codemeta/schema/codemeta.jsonld
+-rw-r--r--   0 proycon   (1000) users      (100)    14995 2022-03-06 15:55:01.000000 CodeMetaPy-2.5.0/codemeta/schema/crosswalk.csv
+-rw-r--r--   0 proycon   (1000) users      (100)     9200 2022-03-06 15:55:01.000000 CodeMetaPy-2.5.0/codemeta/schema/properties_description.csv
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:13:05.269822 CodeMetaPy-2.5.0/codemeta/serializers/
+-rw-r--r--   0 proycon   (1000) users      (100)        0 2022-03-08 10:50:22.000000 CodeMetaPy-2.5.0/codemeta/serializers/__init__.py
+-rw-r--r--   0 proycon   (1000) users      (100)    16111 2023-05-10 13:47:46.000000 CodeMetaPy-2.5.0/codemeta/serializers/jsonld.py
+-rw-r--r--   0 proycon   (1000) users      (100)      659 2023-05-10 13:48:09.000000 CodeMetaPy-2.5.0/codemeta/serializers/turtle.py
+-rw-r--r--   0 proycon   (1000) users      (100)     7391 2023-05-10 13:41:34.000000 CodeMetaPy-2.5.0/codemeta/validation.py
+-rw-r--r--   0 proycon   (1000) users      (100)       38 2023-05-15 16:13:05.269822 CodeMetaPy-2.5.0/setup.cfg
+-rwxr-xr-x   0 proycon   (1000) users      (100)     1943 2023-05-11 15:52:48.000000 CodeMetaPy-2.5.0/setup.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:13:05.269822 CodeMetaPy-2.5.0/tests/
+-rw-r--r--   0 proycon   (1000) users      (100)    28836 2023-05-10 09:41:41.000000 CodeMetaPy-2.5.0/tests/tests.py
```

### Comparing `CodeMetaPy-2.4.1/COPYING` & `CodeMetaPy-2.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `CodeMetaPy-2.4.1/CodeMetaPy.egg-info/PKG-INFO` & `CodeMetaPy-2.5.0/CodeMetaPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: CodeMetaPy
-Version: 2.4.1
+Version: 2.5.0
 Summary: Generate and manage CodeMeta software metadata
 Home-page: https://github.com/proycon/codemetapy
 Author: Maarten van Gompel
 Author-email: proycon@anaproy.nl
 License: GPL-3.0-only
 Keywords: software metadata,codemeta,schema.org,rdf,linked data
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -238,8 +237,13 @@
 is not installed, and that the command will be available if codemetapy
 is available.
 
 If you want to ship your package with the generated `codemeta.json`,
 then simply add a line saying `codemeta.json` to the file `MANIFEST.in`
 in the root of your project.
 
+## Acknowledgements
 
+This work is conducted at the [KNAW Humanities Cluster](https://huc.knaw.nl/)'s
+[Digital Infrastructure department](https://di.huc.knaw.nl/) in the scope of the 
+[CLARIAH](https://www.clariah.nl) project (CLARIAH-PLUS, NWO grant 184.034.023) as
+part of the FAIR Tool Discovery track of the Shared Development Roadmap.
```

### Comparing `CodeMetaPy-2.4.1/PKG-INFO` & `CodeMetaPy-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: CodeMetaPy
-Version: 2.4.1
+Version: 2.5.0
 Summary: Generate and manage CodeMeta software metadata
 Home-page: https://github.com/proycon/codemetapy
 Author: Maarten van Gompel
 Author-email: proycon@anaproy.nl
 License: GPL-3.0-only
 Keywords: software metadata,codemeta,schema.org,rdf,linked data
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -238,8 +237,13 @@
 is not installed, and that the command will be available if codemetapy
 is available.
 
 If you want to ship your package with the generated `codemeta.json`,
 then simply add a line saying `codemeta.json` to the file `MANIFEST.in`
 in the root of your project.
 
+## Acknowledgements
 
+This work is conducted at the [KNAW Humanities Cluster](https://huc.knaw.nl/)'s
+[Digital Infrastructure department](https://di.huc.knaw.nl/) in the scope of the 
+[CLARIAH](https://www.clariah.nl) project (CLARIAH-PLUS, NWO grant 184.034.023) as
+part of the FAIR Tool Discovery track of the Shared Development Roadmap.
```

### Comparing `CodeMetaPy-2.4.1/README.md` & `CodeMetaPy-2.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -213,7 +213,14 @@
 This will ensure your `setup.py` works in all cases, even if codemetapy
 is not installed, and that the command will be available if codemetapy
 is available.
 
 If you want to ship your package with the generated `codemeta.json`,
 then simply add a line saying `codemeta.json` to the file `MANIFEST.in`
 in the root of your project.
+
+## Acknowledgements
+
+This work is conducted at the [KNAW Humanities Cluster](https://huc.knaw.nl/)'s
+[Digital Infrastructure department](https://di.huc.knaw.nl/) in the scope of the 
+[CLARIAH](https://www.clariah.nl) project (CLARIAH-PLUS, NWO grant 184.034.023) as
+part of the FAIR Tool Discovery track of the Shared Development Roadmap.
```

### Comparing `CodeMetaPy-2.4.1/codemeta/codemeta.py` & `CodeMetaPy-2.5.0/codemeta/codemeta.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,65 +8,84 @@
 # & KNAW Humanities Cluster
 # GPL v3
 import re
 import sys
 import argparse
 import json
 import os.path
-import glob
 import random
-from collections import OrderedDict, defaultdict
-from typing import Union, IO, Optional, Sequence, Tuple
-import copy
-import datetime
+from typing import Union, Optional, Sequence, Tuple
 from pathlib import Path
-import distutils.cmd #note: will be removed in python 3.12! TODO constraint <= 3.11 in apk/apt-get in Dockerfile
-#pylint: disable=C0413
+import distutils.cmd  # note: will be removed in python 3.12! TODO constraint <= 3.11 in apk/apt-get in Dockerfile
 
-from rdflib import Graph, BNode, URIRef, Literal
-from rdflib.namespace import RDF, OWL
-from rdflib.plugins.shared.jsonld.context import Context
-import rdflib.plugins.serializers.jsonld
+# pylint: disable=C0413
 
-from codemeta.common import init_graph, CODEMETA, AttribDict, getstream, SDO, reconcile, add_triple, generate_uri, remap_uri, query, enrich, compose, correct, bind_graph
+from rdflib import Graph, BNode, URIRef
+from rdflib.namespace import RDF, OWL  # type: ignore
+
+from codemeta.common import (
+    init_graph,
+    CODEMETA,
+    AttribDict,
+    getstream,
+    SDO,
+    reconcile,
+    add_triple,
+    generate_uri,
+    remap_uri,
+    query,
+    enrich,
+    compose,
+    correct,
+    bind_graph,
+)
 import codemeta.crosswalk
 import codemeta.parsers.python
 import codemeta.parsers.debian
 import codemeta.parsers.jsonld
 import codemeta.parsers.nodejs
 import codemeta.parsers.java
 import codemeta.parsers.rust
 import codemeta.parsers.web
 import codemeta.parsers.gitapi
 import codemeta.parsers.authors
 import codemeta.validation
 from codemeta.serializers.jsonld import serialize_to_jsonld
-from codemeta.serializers.html import serialize_to_html
 from codemeta.serializers.turtle import serialize_to_turtle
 
 
-#class PostDevelopCommand(setuptools.command.develop.develop):
+# class PostDevelopCommand(setuptools.command.develop.develop):
 #    """Post development installation hook"""
 #    def run(self):
 #        setuptools_update(self)
 #        super(PostDevelopCommand, self).run()
 #
-#class PostInstallCommand(setuptools.command.install.install):
+# class PostInstallCommand(setuptools.command.install.install):
 #    """Post installation hook"""
 #    def run(self):
 #        setuptools_update(self)
 #        super(PostInstallCommand, self).run()
 
+
 class CodeMetaCommand(distutils.cmd.Command):
     description = "Generate a codemeta.json file or update an existing one, note that the package must be installed first for this to work!"
     user_options = [
-        ('with-entrypoints','e','Generate entrypoints as well (custom codemeta extension not part of the official specification)'),
-        ('with-stypes','t','Generate software types using targetProduct (custom extension not part of the official codemeta/schema.org specification yet)'),
-        ('dry-run','n','Write to stdout instead of codemeta.json')
+        (
+            "with-entrypoints",
+            "e",
+            "Generate entrypoints as well (custom codemeta extension not part of the official specification)",
+        ),
+        (
+            "with-stypes",
+            "t",
+            "Generate software types using targetProduct (custom extension not part of the official codemeta/schema.org specification yet)",
+        ),
+        ("dry-run", "n", "Write to stdout instead of codemeta.json"),
     ]
+
     def initialize_options(self):
         self.with_entrypoints = False
         self.dry_run = False
 
     def finalize_options(self):
         self.with_entrypoints = bool(self.with_entrypoints)
         self.dry_run = bool(self.dry_run)
@@ -74,197 +93,417 @@
     def run(self):
         """Updates the codemeta.json for this package during the setup process. Hook to be (indirectly) called from setuptools"""
         codemetafile = "codemeta.json"
         if self.dry_run:
             outputfile = "-"
         else:
             outputfile = codemetafile
-        print("Writing codemeta metadata to " + outputfile,file=sys.stderr)
+        print("Writing codemeta metadata to " + outputfile, file=sys.stderr)
         if os.path.exists(codemetafile):
-            build(input="json,python",output="json",outputfile=outputfile, inputsources=[codemetafile, self.distribution.metadata.name], with_entrypoints=self.with_entrypoints)
+            build(
+                input="json,python",
+                output="json",
+                outputfile=outputfile,
+                inputsources=[codemetafile, self.distribution.metadata.name],
+                with_entrypoints=self.with_entrypoints,
+            )
         else:
-            build(input="python",output="json",outputfile=outputfile, inputsources=[self.distribution.metadata.name], with_entrypoints=self.with_entrypoints)
+            build(
+                input="python",
+                output="json",
+                outputfile=outputfile,
+                inputsources=[self.distribution.metadata.name],
+                with_entrypoints=self.with_entrypoints,
+            )
 
 
 props, crosswalk = codemeta.crosswalk.readcrosswalk()
 
+
 def main():
     """Main entrypoint for command-line usage"""
 
-    parser = argparse.ArgumentParser(description="Converter for Python Distutils (PyPI) Metadata to CodeMeta (JSON-LD) converter. Also supports conversion from other metadata types such as those from Debian packages. The tool can combine metadata from multiple sources.")
-    parser.add_argument('-t', '--with-stypes', dest="with_stypes", help="Convert entrypoints to targetProduct and classes reflecting software type (https://github.com/codemeta/codemeta/issues/#271), linking softwareSourceCode to softwareApplication or WebAPI. If enabled, any remote URLs passed to codemetapy will automatically be encoded via targetProduct.", action='store_true',required=False)
-    parser.add_argument('--exact-python-version', dest="exactplatformversion", help="Register the exact python interpreter used to generate the metadata as the runtime platform. Will only register the major version otherwise.", action='store_true',required=False)
-    parser.add_argument('--single-author', dest="single_author", help="CodemetaPy will attempt to check if there are multiple authors specified in the author field, if you want to disable this behaviour, set this flag", action='store_true',required=False)
-    parser.add_argument('-b', '--baseuri',type=str,help="Base URI for resulting SoftwareSourceCode instances (make sure to add a trailing slash)", action='store',required=False)
-    parser.add_argument('-B', '--baseurl',type=str,help="Base URL in HTML visualizations (make sure to add a trailing slash)", action='store',required=False)
-    parser.add_argument('-o', '--outputtype', dest='output',type=str,help="Output type: json (default), turtle, html", action='store',required=False, default="json")
-    parser.add_argument('-O','--outputfile',  dest='outputfile',type=str,help="Output file", action='store',required=False)
-    parser.add_argument('-i','--inputtype', dest='inputtypes',type=str,help="Metadata input type: python, apt (debian packages), registry, json, yaml. May be a comma seperated list of multiple types if files are passed on the command line", action='store',required=False)
-    parser.add_argument('-g','--graph', dest='graph',help="Output a knowledge graph that groups all input files together. Only JSON input files are supported.", action='store_true',required=False)
-    parser.add_argument('-s','--select', type=str, help="Output only the selected resource (by URI) from the graph", action='store',required=False)
-    parser.add_argument('-V','--validate', type=str, help="Validate against the provided SHACL file. Adds a review property with the condensed validation results.", action='store',required=False)
-    parser.add_argument('--enrich', help="Enable automatic inference and enrichment of the metadata where possible", action='store_true',required=False)
-    parser.add_argument('--addcontext', help="Add the specified jsonld (must be a URL) to the context (and to the context graph). May be specified multiple times.", action='append',required=False)
-    parser.add_argument('--addcontextgraph', help="Add the specified jsonld or turtle (must be a URL) to the context graph, but NOT to the main json-ld context. May be specified multiple times.", action='append',required=False)
-    parser.add_argument('--includecontext', help="Include all context vocabularies in the main graph and express it verbosely in serialisations. This makes the resoluting codemeta.json richer without the need to query certain external vocabularies, at the cost of added redundancy.", action='store_true',required=False)
-    parser.add_argument('--interpreter', help="Start interactive python interpreter after loading the graph", action='store_true',required=False)
-    parser.add_argument('--exitv', help="Set exit status according to validation result. Use with --validate", action='store_true',required=False)
-    parser.add_argument('--textv', type=str, help="Set extra text to add to a validation report. Use with --validate", action='store',required=False)
-    parser.add_argument('--intro', type=str, help="Set extra text (HTML) to add to the index page as an introduction", action='store',required=False)
-    parser.add_argument('--css',type=str, help="Associate a CSS stylesheet (URL) with the HTML output, multiple stylesheets can be separated by a comma", action='store',  required=False)
-    parser.add_argument('--no-cache',dest="no_cache", help="Do not cache context files, force redownload", action='store_true',  required=False)
-    parser.add_argument('--no-extras',dest="no_extras", help="Do not include dependencies that are marked as 'extras', applies only to Python", action='store_true',  required=False)
-    parser.add_argument('--codemetaserver', '--toolstore', dest="toolstore", help="When converting to HTML, link pages together for use with codemeta-server", action='store_true',  required=False)
-    parser.add_argument('--strict', dest='strict', help="Strictly adhere to the codemeta standard and disable any extensions on top of it", action='store_true')
-    parser.add_argument('--released', help="Signal that this software is released, this affects whether development status maps to either WIP or active", action='store_true')
-    parser.add_argument('--trl', help="Attempt to add technology readiness level based on the vocabulary used by the CLARIAH project", action='store_true')
-    parser.add_argument('--title', type=str, help="Title to add when generating HTML pages", action='store')
-    parser.add_argument('--identifier-from-file', dest='identifier_from_file', help="Derive the identifier from the filename/module name passed to codemetapy, not from the metadata itself", action='store_true',required=False)
-    parser.add_argument('inputsources', nargs='*', help='Input sources, the nature of the source depends on the type, often a file (or use - for standard input, /dev/null to start from scratch without external input), set -i accordingly with the types (must contain as many items as passed!)')
+    parser = argparse.ArgumentParser(
+        description="Converter for Python Distutils (PyPI) Metadata to CodeMeta (JSON-LD) converter. Also supports conversion from other metadata types such as those from Debian packages. The tool can combine metadata from multiple sources."
+    )
+    parser.add_argument(
+        "-t",
+        "--with-stypes",
+        dest="with_stypes",
+        help="Convert entrypoints to targetProduct and classes reflecting software type (https://github.com/codemeta/codemeta/issues/#271), linking softwareSourceCode to softwareApplication or WebAPI. If enabled, any remote URLs passed to codemetapy will automatically be encoded via targetProduct.",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "--exact-python-version",
+        dest="exactplatformversion",
+        help="Register the exact python interpreter used to generate the metadata as the runtime platform. Will only register the major version otherwise.",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "--single-author",
+        dest="single_author",
+        help="CodemetaPy will attempt to check if there are multiple authors specified in the author field, if you want to disable this behaviour, set this flag",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "-b",
+        "--baseuri",
+        type=str,
+        help="Base URI for resulting SoftwareSourceCode instances (make sure to add a trailing slash)",
+        action="store",
+        required=False,
+    )
+    parser.add_argument(
+        "-o",
+        "--outputtype",
+        dest="output",
+        type=str,
+        help="Output type: json (default), turtle",
+        action="store",
+        required=False,
+        default="json",
+    )
+    parser.add_argument(
+        "-O",
+        "--outputfile",
+        dest="outputfile",
+        type=str,
+        help="Output file",
+        action="store",
+        required=False,
+    )
+    parser.add_argument(
+        "-i",
+        "--inputtype",
+        dest="inputtypes",
+        type=str,
+        help="Metadata input type: python, apt (debian packages), registry, json, yaml. May be a comma seperated list of multiple types if files are passed on the command line",
+        action="store",
+        required=False,
+    )
+    parser.add_argument(
+        "-g",
+        "--graph",
+        dest="graph",
+        help="Output a knowledge graph that groups all input files together. Only JSON input files are supported.",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "-s",
+        "--select",
+        type=str,
+        help="Output only the selected resource (by URI) from the graph",
+        action="store",
+        required=False,
+    )
+    parser.add_argument(
+        "-V",
+        "--validate",
+        type=str,
+        help="Validate against the provided SHACL file. Adds a review property with the condensed validation results.",
+        action="store",
+        required=False,
+    )
+    parser.add_argument(
+        "--enrich",
+        help="Enable automatic inference and enrichment of the metadata where possible",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "--addcontext",
+        help="Add the specified jsonld (must be a URL) to the context (and to the context graph). May be specified multiple times.",
+        action="append",
+        required=False,
+    )
+    parser.add_argument(
+        "--addcontextgraph",
+        help="Add the specified jsonld or turtle (must be a URL) to the context graph, but NOT to the main json-ld context. May be specified multiple times.",
+        action="append",
+        required=False,
+    )
+    parser.add_argument(
+        "--includecontext",
+        help="Include all context vocabularies in the main graph and express it verbosely in serialisations. This makes the resulting codemeta.json richer without the need to query certain external vocabularies, at the cost of added redundancy.",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "--interpreter",
+        help="Start interactive python interpreter after loading the graph",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "--exitv",
+        help="Set exit status according to validation result. Use with --validate",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "--textv",
+        type=str,
+        help="Set extra text to add to a validation report. Use with --validate",
+        action="store",
+        required=False,
+    )
+    parser.add_argument(
+        "--no-cache",
+        dest="no_cache",
+        help="Do not cache context files, force redownload",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "--no-extras",
+        dest="no_extras",
+        help="Do not include dependencies that are marked as 'extras', applies only to Python",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "--strict",
+        dest="strict",
+        help="Strictly adhere to the codemeta standard and disable any extensions on top of it",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--released",
+        help="Signal that this software is released, this affects whether development status maps to either WIP or active",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--trl",
+        help="Attempt to add technology readiness level based on the vocabulary used by the CLARIAH project",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--identifier-from-file",
+        dest="identifier_from_file",
+        help="Derive the identifier from the filename/module name passed to codemetapy, not from the metadata itself",
+        action="store_true",
+        required=False,
+    )
+    parser.add_argument(
+        "inputsources",
+        nargs="*",
+        help="Input sources, the nature of the source depends on the type, often a file (or use - for standard input, /dev/null to start from scratch without external input), set -i accordingly with the types (must contain as many items as passed!)",
+    )
 
     for key, prop in sorted(props.items()):
         if key:
-            parser.add_argument('--' + key,dest=key, type=str, help=prop['DESCRIPTION'] + " (Type: "  + prop['TYPE'] + ", Parent: " + prop['PARENT'] + ") [you can format the value string in json if needed]", action='store',required=False)
+            parser.add_argument(
+                "--" + key,
+                dest=key,
+                type=str,
+                help=prop["DESCRIPTION"]
+                + " (Type: "
+                + prop["TYPE"]
+                + ", Parent: "
+                + prop["PARENT"]
+                + ") [you can format the value string in json if needed]",
+                action="store",
+                required=False,
+            )
 
     args = parser.parse_args()
     if not args.strict:
         args.with_stypes = True
-    if args.css:
-        args.css = [ x.strip() for x in args.css.split(",") ]
-
-    if args.baseuri and not args.baseurl:
-        args.baseurl = args.baseuri
 
     if args.trl:
-        if args.addcontext is None: args.addcontext = []
-        if "https://w3id.org/research-technology-readiness-levels" not in args.addcontext:
-            args.addcontext.append("https://w3id.org/research-technology-readiness-levels")
+        if args.addcontext is None:
+            args.addcontext = []
+        if (
+            "https://w3id.org/research-technology-readiness-levels"
+            not in args.addcontext
+        ):
+            args.addcontext.append(
+                "https://w3id.org/research-technology-readiness-levels"
+            )
 
     valid = False
     if args.graph:
-        #join multiple inputs into a larger graph
-        g, res, args, contextgraph = read(**args.__dict__) #may deliver a res when args.select is set
+        # join multiple inputs into a larger graph
+        g, res, args, contextgraph = read(
+            **args.__dict__
+        )  # may deliver a res when args.select is set
     else:
-        #normal behaviour
+        # normal behaviour
         g, res, args, contextgraph = build(**args.__dict__)
-    if args.validate: 
+    if args.validate:
         if res:
             valid, _ = codemeta.validation.validate(g, res, args, contextgraph)
         else:
-            raise Exception("Validation can only be done on single resources, not when --graph is set and multiple are loaded/aggregated""")
+            raise Exception(
+                "Validation can only be done on single resources, not when --graph is set and multiple are loaded/aggregated"
+                ""
+            )
 
     if args.includecontext:
         g += contextgraph
     output = serialize(g, res, args, contextgraph)
     if output:
         print(output)
 
     if args.interpreter:
         print("Starting interactive shell: variable 'g' holds the rdflib.Graph")
-        import readline # optional, will allow Up/Down/History in the console
+        import readline  # optional, will allow Up/Down/History in the console
         import code
+
         variables = globals().copy()
         variables.update(locals())
         shell = code.InteractiveConsole(variables)
         shell.interact()
 
     if args.exitv and args.validate:
         return 0 if valid else 1
 
 
+def load(*files, **kwargs) -> Tuple[Graph, Union[URIRef, None], AttribDict, Graph]:
+    """Main entrypoint for library usage"""
 
+    # defaults
+    if not "strict" in kwargs:
+        kwargs["with_stypes"] = True
+
+    if "baseuri" in kwargs and not "baseurl" in kwargs:
+        kwargs["baseurl"] = kwargs["baseuri"]
+
+    kwargs["graph"] = True
+    kwargs["inputsources"] = files
+    if "includecontext" not in kwargs:
+        kwargs["includecontext"] = True
+
+    g, res, args, contextgraph = read(
+        **kwargs
+    )  # may deliver a res when args.select is set
 
-def serialize(g: Graph, res: Union[Sequence,URIRef,BNode,None], args: AttribDict, contextgraph: Union[Graph,None] = None, sparql_query: Optional[str] = None, **kwargs) -> str:
+    if args.includecontext:
+        g += contextgraph
+
+    return g, res, args, contextgraph
+
+
+def serialize(
+    g: Graph,
+    res: Union[Sequence, URIRef, BNode, None],
+    args: AttribDict,
+    contextgraph: Union[Graph, None] = None,
+    sparql_query: Optional[str] = None,
+    **kwargs,
+) -> Optional[str]:
     if args.output == "json":
-        if sparql_query: res = [ x[0]  for x in query(g, sparql_query) ]
+        if sparql_query:
+            res = [x[0] for x in query(g, sparql_query)]
         doc = serialize_to_jsonld(g, res, args)
         if args.outputfile and args.outputfile != "-":
-            with open(args.outputfile,'w',encoding='utf-8') as fp:
+            with open(args.outputfile, "w", encoding="utf-8") as fp:
                 fp.write(json.dumps(doc, indent=4, ensure_ascii=False, sort_keys=True))
         else:
             return json.dumps(doc, indent=4, ensure_ascii=False, sort_keys=True)
-    elif args.output in ("turtle","ttl"):
-        if sparql_query: res = [ x[0]  for x in query(g, sparql_query) ]
+    elif args.output in ("turtle", "ttl"):
+        if sparql_query:
+            res = [x[0] for x in query(g, sparql_query)]
         doc = serialize_to_turtle(g, res)
         if args.outputfile and args.outputfile != "-":
-            with open(args.outputfile,'wb') as fp:
-                fp.write(doc)
+            with open(args.outputfile, "wb") as fp:
+                fp.write(doc.encode('utf-8'))
         else:
             return doc
     elif args.output == "html":
-        if not isinstance(contextgraph, Graph):
-            raise Exception("No contextgraph provided, required for HTML serialisation")
-        doc = serialize_to_html(g, res, args, contextgraph, sparql_query,  **kwargs) #note: sparql query is applied in serialization function if needed
-        if args.outputfile and args.outputfile != "-":
-            with open(args.outputfile,'w',encoding='utf-8') as fp:
-                fp.write(doc)
-        else:
-            return doc
+        raise Exception(
+            "Output type html is no longer handled by codemetapy but has moved to codemeta2html: https://github.com/proycon/codemeta2html"
+        )
     else:
         raise Exception("No such output type: ", args.output)
 
-def reidentify(g: Graph, res: Union[URIRef,BNode], identifier: Optional[str], founduris: list, args: AttribDict) -> Union[URIRef,BNode]:
+
+def reidentify(
+    g: Graph,
+    res: Union[URIRef, BNode],
+    identifier: Optional[str],
+    founduris: list,
+    args: AttribDict,
+) -> Union[URIRef, BNode]:
     """Reassign a new URI for the resource, or assign an original found one. The former will include a version component"""
     if founduris and not args.baseuri:
-        #restore the exact original URI because we did not set a baseuri
+        # restore the exact original URI because we did not set a baseuri
         founduri = founduris[0]
-        print(f"Remapping URI to found URI: {res} -> {founduri}",file=sys.stderr)
-        remap_uri(g, res, founduri)
-        res = URIRef(founduri)
+        if res != founduri:
+            print(f"Remapping URI to found URI: {res} -> {founduri}", file=sys.stderr)
+            remap_uri(g, res, founduri)
+            res = URIRef(founduri)
     elif args.baseuri:
         for founduri in founduris:
-            if not founduri.startswith("file://"): #non-local ones only
-                #we've rewritten the URI, add the old one via owl:sameAs
+            if not founduri.startswith("file://"):  # non-local ones only
+                # we've rewritten the URI, add the old one via owl:sameAs
                 g.add((res, OWL.sameAs, URIRef(founduri)))
         if not args.identifier and not args.identifier_from_file:
-            #see if we can find a better one from the data itself:
+            # see if we can find a better one from the data itself:
             identifier = get_identifier(g, res) or identifier
-        if not identifier: 
+        if not identifier:
             if g.value(res, SDO.name):
-                identifier = str(g.value(res, SDO.name)).strip().lower().replace(" ","-").replace(":","-")
+                identifier = (
+                    str(g.value(res, SDO.name))
+                    .strip()
+                    .lower()
+                    .replace(" ", "-")
+                    .replace(":", "-")
+                )
             else:
                 identifier = "N" + "%032x" % random.getrandbits(128)
-        version = g.value(res,SDO.version)
-        if not version: version = "snapshot" #if we find no version, we append /snapshot to the URI as a version component, usually referring to the git master/main branch but not any specific version
+        version = g.value(res, SDO.version)
+        if not version:
+            version = "snapshot"  # if we find no version, we append /snapshot to the URI as a version component, usually referring to the git master/main branch but not any specific version
         uri = args.baseuri + identifier + "/" + str(version)
-        print(f"Remapping URI to (possibly) new identifier and version component: {res} -> {uri}",file=sys.stderr)
-        remap_uri(g, res, uri)
-        res = URIRef(uri)
+        if res != URIRef(uri):
+            print(
+                f"Remapping URI to (possibly) new identifier and version component: {res} -> {uri}",
+                file=sys.stderr,
+            )
+            remap_uri(g, res, uri)
+            res = URIRef(uri)
     return res
 
-def get_identifier(g: Graph, res: Union[URIRef,BNode])  -> Optional[str]:
-    for _,_,o in g.triples((res, SDO.identifier,None)):
-        if not str(o).startswith(("http://","https://")) and not ':' in str(o):
+
+def get_identifier(g: Graph, res: Union[URIRef, BNode]) -> Optional[str]:
+    for _, _, o in g.triples((res, SDO.identifier, None)):
+        if not str(o).startswith(("http://", "https://")) and not ":" in str(o):
             return str(o).strip("/ ")
 
-def read(**kwargs) -> Tuple[Graph, Union[URIRef,None], AttribDict, Graph]:
+
+def read(**kwargs) -> Tuple[Graph, Union[URIRef, None], AttribDict, Graph]:
     """Read multiple resources together in a codemeta graph, and either output it all or output a selection"""
 
     args = AttribDict(kwargs)
 
     g, contextgraph = init_graph(args)
 
     if not args.inputsources:
         raise Exception("No inputsources specified")
 
     for source in args.inputsources:
-        print(f"Adding json-ld file from {source} to graph",file=sys.stderr)
+        print(f"Adding json-ld file from {source} to graph", file=sys.stderr)
         codemeta.parsers.jsonld.parse_jsonld(g, None, getstream(source), args)
 
-    #remap resource identifiers (URIs) when needed
-    for s,_,_ in g.triples((None, RDF.type,SDO.SoftwareSourceCode)):
-        if isinstance(s, (URIRef,BNode)):
-            identifier = get_identifier(g,s)
+    # remap resource identifiers (URIs) when needed
+    for s, _, _ in g.triples((None, RDF.type, SDO.SoftwareSourceCode)):
+        if isinstance(s, (URIRef, BNode)):
+            identifier = get_identifier(g, s)
             if isinstance(s, URIRef) and str(s).startswith("http"):
                 founduris = [str(s)]
             else:
                 founduris = []
-            #ensure the proper URI is set
+            # ensure the proper URI is set
             s = reidentify(g, s, identifier, founduris, args)
-            #run some automatic corrections on the graph for this resource
+            # run some automatic corrections on the graph for this resource
             correct(g, s, args)
             reconcile(g, s, args)
 
     if args.select:
         res = URIRef(args.select)
         if (res, None, None) not in g:
             raise KeyError("Selected resource does not exists")
@@ -280,193 +519,231 @@
 
     inputsources = []
     if args.inputsources:
         inputfiles = args.inputsources
         inputtypes = args.inputtypes.split(",") if args.inputtypes else []
         guess = False
         if len(inputtypes) != len(inputfiles):
-            print(f"Passed {len(inputfiles)} files/sources but specified {len(inputtypes)} input types! Automatically guessing types...",  file=sys.stderr)
+            print(
+                f"Passed {len(inputfiles)} files/sources but specified {len(inputtypes)} input types! Automatically guessing types...",
+                file=sys.stderr,
+            )
             guess = True
-            for inputsource in inputfiles[len(inputtypes):]:
+            for inputsource in inputfiles[len(inputtypes) :]:
                 if inputsource == "/dev/null":
                     inputtypes.append("null")
                 elif inputsource.lower().endswith("setup.py"):
                     inputtypes.append("python")
                 elif inputsource.endswith("package.json"):
                     inputtypes.append("nodejs")
                 elif inputsource.endswith("pyproject.toml"):
                     inputtypes.append("python")
                 elif inputsource.endswith("pom.xml"):
                     inputtypes.append("java")
                 elif inputsource.endswith("Cargo.toml"):
                     inputtypes.append("rust")
-                elif inputsource.lower().endswith(".json") or inputsource.lower().endswith(".jsonld"):
+                elif inputsource.lower().endswith(
+                    ".json"
+                ) or inputsource.lower().endswith(".jsonld"):
                     inputtypes.append("json")
                 elif inputsource.upper().endswith("CONTRIBUTORS"):
                     inputtypes.append("contributors")
                 elif inputsource.upper().endswith("AUTHORS"):
                     inputtypes.append("authors")
                 elif inputsource.upper().endswith("MAINTAINERS"):
                     inputtypes.append("maintainers")
-                elif inputsource.lower().startswith("https") or inputsource.lower().startswith("git@"):
-                    #test if this is a known git platform we can query via an API
+                elif inputsource.lower().startswith(
+                    "https"
+                ) or inputsource.lower().startswith("git@"):
+                    # test if this is a known git platform we can query via an API
                     repo_kind = codemeta.parsers.gitapi.get_repo_kind(inputsource)
                     if repo_kind:
                         inputtypes.append(repo_kind)
                     elif not inputsource.lower().startswith("git@"):
-                        #otherwise it is just a website
+                        # otherwise it is just a website
                         inputtypes.append("web")
                 elif inputsource.lower().startswith("http"):
                     inputtypes.append("web")
         inputsources = list(zip(inputfiles, inputtypes))
         if guess:
             while len(inputtypes) < len(inputfiles):
                 inputfile = inputfiles[len(inputtypes)]
-                print(f"No input type specified for {inputfile}, guessing this is an installed python package (may be wrong)",file=sys.stderr)
+                print(
+                    f"No input type specified for {inputfile}, guessing this is an installed python package (may be wrong)",
+                    file=sys.stderr,
+                )
                 inputtypes.append("python")
             inputsources = list(zip(inputfiles, inputtypes))
-            print(f"Detected input types: {inputsources}",file=sys.stderr)
+            print(f"Detected input types: {inputsources}", file=sys.stderr)
     else:
-        #no input was specified
-        if os.path.exists('setup.py'):
-            print("No input files specified, but found python project (setup.py) in current dir, using that...",file=sys.stderr)
-            print("Generating egg_info",file=sys.stderr)
+        # no input was specified
+        if os.path.exists("setup.py"):
+            print(
+                "No input files specified, but found python project (setup.py) in current dir, using that...",
+                file=sys.stderr,
+            )
+            print("Generating egg_info", file=sys.stderr)
             r = os.system("python3 setup.py egg_info >&2")
-            #we ignore the return code for now because it may be non-zero but still have sueful results
-            for path in Path('.').rglob('*.egg-info'):
-                inputsources = [(".".join(str(path).split(".")[:-1]),"python")]
+            # we ignore the return code for now because it may be non-zero but still have sueful results
+            for path in Path(".").rglob("*.egg-info"):
+                inputsources = [(".".join(str(path).split(".")[:-1]), "python")]
                 break
             if not inputsources:
                 if r != 0:
-                    raise Exception("Could not generate egg_info (is python3 pointing to the right interpreter?)")
+                    raise Exception(
+                        "Could not generate egg_info (is python3 pointing to the right interpreter?)"
+                    )
                 raise Exception("Could not found egg_info results")
-        elif os.path.exists('pyproject.toml'):
-            print("No input files specified, but found python project (pyproject.toml) in current dir, using that...",file=sys.stderr)
-            inputsources = [("pyproject.toml","python")]
+        elif os.path.exists("pyproject.toml"):
+            print(
+                "No input files specified, but found python project (pyproject.toml) in current dir, using that...",
+                file=sys.stderr,
+            )
+            inputsources = [("pyproject.toml", "python")]
         else:
             raise Exception("No input files specified (use - for stdin)")
 
     g, contextgraph = init_graph(args)
 
-
     if args.baseuri:
         args.baseuri = args.baseuri.strip('" ')
-        if args.baseuri[-1] not in ('/','#','?'):
+        if args.baseuri[-1] not in ("/", "#", "?"):
             args.baseuri += "/"
     else:
-        print("Note: You did not specify a --baseuri so we will not provide identifiers (IRIs) for your SoftwareSourceCode resources (and others)", file=sys.stderr)
+        print(
+            "Note: You did not specify a --baseuri so we will not provide identifiers (IRIs) for your SoftwareSourceCode resources (and others)",
+            file=sys.stderr,
+        )
 
-    #Generate a temporary ID to use for the SoftwareSourceCode resource
-    #The ID will be overwritten with a more fitting one upon serialisation
+    # Generate a temporary ID to use for the SoftwareSourceCode resource
+    # The ID will be overwritten with a more fitting one upon serialisation
     if args.identifier:
         identifier = args.identifier.strip('"')
     else:
         identifier = os.path.basename(inputsources[0][0]).lower()
     if identifier:
-        identifier = identifier.replace(".codemeta.json","").replace("codemeta.json","")
-        identifier = identifier.replace(".pom.xml","").replace("pom.xml","")
-        identifier = identifier.replace(".package.json","").replace("package.json","")
+        identifier = identifier.replace(".codemeta.json", "").replace(
+            "codemeta.json", ""
+        )
+        identifier = identifier.replace(".pom.xml", "").replace("pom.xml", "")
+        identifier = identifier.replace(".package.json", "").replace("package.json", "")
     uri = generate_uri(identifier, args.baseuri)
-    print(f"Initial URI automatically generated, may be overriden later: {uri}",file=sys.stderr)
+    print(
+        f"Initial URI automatically generated, may be overriden later: {uri}",
+        file=sys.stderr,
+    )
 
-    #add the root resource
+    # add the root resource
     res = URIRef(uri)
     g.add((res, RDF.type, SDO.SoftwareSourceCode))
 
-
-    founduris = [] #stores all fully qualified URIs we find fot the main resource
+    founduris = []  # stores all fully qualified URIs we find fot the main resource
 
     l = len(inputsources)
     for i, (source, inputtype) in enumerate(inputsources):
-        print(f"Processing source #{i+1} of {l}",file=sys.stderr)
+        print(f"Processing source #{i+1} of {l}", file=sys.stderr)
 
         newgraph = Graph()
         bind_graph(newgraph)
-          
+
         if inputtype == "null":
-            print(f"Starting from scratch, using command line parameters to build",file=sys.stderr)
+            print(
+                f"Starting from scratch, using command line parameters to build",
+                file=sys.stderr,
+            )
         elif inputtype == "python":
-            print(f"Obtaining python package metadata for: {source}",file=sys.stderr)
-            #source is a name of a package or path to a pyproject.toml file
+            print(f"Obtaining python package metadata for: {source}", file=sys.stderr)
+            # source is a name of a package or path to a pyproject.toml file
             codemeta.parsers.python.parse_python(newgraph, res, source, crosswalk, args)
         elif inputtype == "debian":
-            print(f"Parsing debian package from {source}",file=sys.stderr)
+            print(f"Parsing debian package from {source}", file=sys.stderr)
             with getstream(source) as f:
                 aptlines = f.read().split("\n")
-            codemeta.parsers.debian.parse_debian(newgraph, res, aptlines, crosswalk, args)
+            codemeta.parsers.debian.parse_debian(
+                newgraph, res, aptlines, crosswalk, args
+            )
         elif inputtype == "nodejs":
-            print(f"Parsing npm package.json from {source}",file=sys.stderr)
+            print(f"Parsing npm package.json from {source}", file=sys.stderr)
             with getstream(source) as f:
                 codemeta.parsers.nodejs.parse_nodejs(newgraph, res, f, crosswalk, args)
         elif inputtype == "rust":
-            print(f"Parsing rust Cargo.toml from {source}",file=sys.stderr)
+            print(f"Parsing rust Cargo.toml from {source}", file=sys.stderr)
             with getstream(source) as f:
                 codemeta.parsers.rust.parse_rust(newgraph, res, f, args)
         elif inputtype == "java":
-            print(f"Parsing java/maven pom.xml from {source}",file=sys.stderr)
+            print(f"Parsing java/maven pom.xml from {source}", file=sys.stderr)
             with getstream(source) as f:
                 codemeta.parsers.java.parse_java(newgraph, res, f, crosswalk, args)
         elif inputtype == "json":
-            print(f"Parsing json-ld file from {source}",file=sys.stderr)
+            print(f"Parsing json-ld file from {source}", file=sys.stderr)
             with getstream(source) as f:
                 founduri = codemeta.parsers.jsonld.parse_jsonld(newgraph, res, f, args)
-            if founduri and founduri not in founduris: founduris.append(founduri)
+            if founduri and founduri not in founduris:
+                founduris.append(founduri)
         elif inputtype == "web":
-            print(f"Fallback: Obtaining metadata from remote URL {source}",file=sys.stderr)
+            print(
+                f"Fallback: Obtaining metadata from remote URL {source}",
+                file=sys.stderr,
+            )
             found = False
-            for targetres in codemeta.parsers.web.parse_web(newgraph, res, source, args):
+            for targetres in codemeta.parsers.web.parse_web(
+                newgraph, res, source, args
+            ):
                 if targetres and args.with_stypes:
                     found = True
-                    print(f"Adding service (targetProduct) {source}",file=sys.stderr)
+                    print(f"Adding service (targetProduct) {source}", file=sys.stderr)
                     g.add((res, SDO.targetProduct, targetres))
             if not found:
-                print(f"(no metadata found at remote URL)",file=sys.stderr)
+                print(f"(no metadata found at remote URL)", file=sys.stderr)
         elif inputtype in ("github", "gitlab", "gitapi"):
-            #e.g. transform git@gitlab.com/X in https://gitlab.com/X
-            source = re.sub(r'git@(.*):', r'https://\1/', source)
-            if source.endswith(".git"): source = source[:-4]
-            if inputtype == "gitapi": #disambiguate
+            # e.g. transform git@gitlab.com/X in https://gitlab.com/X
+            source = re.sub(r"git@(.*):", r"https://\1/", source)
+            if source.endswith(".git"):
+                source = source[:-4]
+            if inputtype == "gitapi":  # disambiguate
                 inputtype = codemeta.parsers.gitapi.get_repo_kind(source)
             if inputtype:
-                print(f"Querying GitAPI parser for {source}",file=sys.stderr)
-                codemeta.parsers.gitapi.parse(newgraph, res, source, inputtype ,args)
+                print(f"Querying GitAPI parser for {source}", file=sys.stderr)
+                codemeta.parsers.gitapi.parse(newgraph, res, source, inputtype, args)
             else:
                 raise ValueError(f"Unable to disambiguate gitapi type")
-        elif inputtype in ('authors', 'contributors','maintainers'):
-            print(f"Extracting {inputtype} from {source}",file=sys.stderr)
-            if inputtype == 'authors':
+        elif inputtype in ("authors", "contributors", "maintainers"):
+            print(f"Extracting {inputtype} from {source}", file=sys.stderr)
+            if inputtype == "authors":
                 prop = SDO.author
-            elif inputtype == 'contributors':
+            elif inputtype == "contributors":
                 prop = SDO.contributor
-            elif inputtype == 'maintainers':
+            elif inputtype == "maintainers":
                 prop = CODEMETA.maintainer
             with getstream(source) as f:
-                codemeta.parsers.authors.parse_authors(newgraph, res, f, args, property=prop )
+                codemeta.parsers.authors.parse_authors(
+                    newgraph, res, f, args, property=prop
+                )
         elif inputtype is not None:
             raise ValueError(f"Unknown input type: {inputtype}")
 
         compose(g, newgraph, res, args)
 
-    #Process command-line arguments last
+    # Process command-line arguments last
     for key in props:
         if hasattr(args, key):
             value = getattr(args, key)
-            if value: value = value.strip('"')
+            if value:
+                value = value.strip('"')
             if value:
                 add_triple(g, res, key, value, args, replace=True)
 
-    #Reassign a new URI to the resource (if needed)
-    res = reidentify(g,res, identifier, founduris, args)
+    # Reassign a new URI to the resource (if needed)
+    res = reidentify(g, res, identifier, founduris, args)
 
-    #Test and fix conflicts in the graph (and report them)
+    # Test and fix conflicts in the graph (and report them)
     reconcile(g, res, args)
-    
+
     if args.enrich:
-        #Some automatic infererence and enrichment
+        # Some automatic infererence and enrichment
         enrich(g, res, args)
 
-    return (g,res,args, contextgraph)
-
+    return (g, res, args, contextgraph)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `CodeMetaPy-2.4.1/codemeta/common.py` & `CodeMetaPy-2.5.0/codemeta/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
 import os
 import json
 import requests
 import random
 import re
+import unicodedata
+
 from collections import Counter, defaultdict
 from tempfile import gettempdir
 from rdflib import Graph, Namespace, URIRef, BNode, Literal
-from rdflib.namespace import RDF, RDFS, SKOS
-from rdflib.compare import graph_diff
-from typing import Union, IO, Sequence, Optional,Generator
+from rdflib.namespace import RDF, RDFS, SKOS #type: ignore
+from typing import Union, Sequence, Optional,Generator
 from collections import OrderedDict
 from nameparser import HumanName
 
 
 PROGLANG_PYTHON = {
     "@type": "ComputerLanguage",
     "name": "Python",
@@ -181,25 +182,15 @@
    ('~=', '-ge-'),
    ('>=', '-le-'),
    ('==', '-eq-'),
    ('!=', '-ne-'),
    ('^', '-ge-'), #used in npm version
    ('>', '-gt-'),
    ('<', '-lt-'),
-   ('=', '-eq-'),
-   (' ', '-'),
-   ('&', '-',),
-   ('/', '-',),
-   ('+', '-',),
-   (':', '-',),
-   (';', '-'),
-   (',',''),
-   ('----', '-'),
-   ('---', '-'),
-   ('--', '-'),
+   ('=', '-eq-')
 ]
 
 #keywords that may be indicative of a certain interface type
 INTERFACE_CLUES = [ #order matters, only one is picked
    ("web application", SDO.WebApplication),
    ("webapp", SDO.WebApplication),
    ("web-based", SDO.WebApplication),
@@ -281,16 +272,19 @@
         self.__dict__ = d
 
     def __getattr__(self, key):
         if key in self:
             return self[key]
         return None
 
+    def __setattr__(self, key, value):
+        super().__setattr__(key,value)
+
 def init_context(args: AttribDict):
-    """Initialized the context, ensures all context JSONLDs are downloaded and local filesystem references are used instead"""
+    """Initialize the context, ensures all context JSONLDs are downloaded and local filesystem references are used instead"""
 
     sources = [ (CODEMETA_LOCAL_SOURCE, CODEMETA_SOURCE), (SCHEMA_LOCAL_SOURCE, SCHEMA_SOURCE), (STYPE_LOCAL_SOURCE, STYPE_SOURCE), (IODATA_LOCAL_SOURCE, IODATA_SOURCE), (REPOSTATUS_LOCAL_SOURCE, REPOSTATUS_SOURCE) ]
     
     if args.addcontext:
         for remote_url in args.addcontext:
             if not remote_url.startswith("http"):
                 raise Exception(f"Explicitly added context (--addcontext) must be a remote URL, got {remote_url} instead")
@@ -378,15 +372,21 @@
                 accept = "application/ld+json;q=1.0;application/json;q=0.9;text/turtle;q=0.8,text/plain;q=0.5"
                 r = requests.get(url, headers={ "Accept": accept})
                 r.raise_for_status()
                 with open(localfile, 'wb') as f:
                     f.write(r.content)
             print(f"Adding to contextgraph: {localfile}", file=sys.stderr)
             with open(localfile, 'r') as f:
-                contextgraph.parse(f)
+                c = f.read(1)
+                if c == '{':
+                    format = "json-ld"
+                else:
+                    format = None #autodetect (works for turtle)
+                f.seek(0)
+                contextgraph.parse(f, format=format)
 
     return g, contextgraph
 
 
 def license_to_spdx(value: Union[str,list,tuple]) -> Union[str,list]:
     """Attempts to converts a license name or acronym to a full SPDX URI (https://spdx.org/licenses/)"""
     if isinstance(value, (list,tuple)):
@@ -850,15 +850,15 @@
         name = g.value(res,SDO.name)
         if name:
             g.set((targetres, SDO.name, name))
         g.set((res, SDO.targetProduct, targetres))
         return targetres
 
 
-def get_subgraph(g: Graph, reslist: Sequence[Union[URIRef,BNode]], subgraph: Union[Graph,None] = None, history: set = None ) -> Graph:
+def get_subgraph(g: Graph, reslist: Sequence[Union[URIRef,BNode]], subgraph: Union[Graph,None] = None, history: Optional[set] = None ) -> Graph:
     """Add everything referenced from the specified resource to the new subgraph"""
 
     if subgraph is None:
         subgraph = Graph()
         bind_graph(subgraph)
 
     if history is None:
@@ -889,18 +889,18 @@
     assert from_uri is not None and to_uri is not None
     if not isinstance(from_uri, URIRef):
         from_uri = URIRef(from_uri)
     if not isinstance(to_uri, URIRef):
         to_uri = URIRef(to_uri)
     for s,p,o in g.triples((from_uri,None,None)):
         g.remove((s,p,o))
-        g.add((to_uri,p,o))
+        g.add((to_uri,p,o)) #type: ignore
     for s,p,o in g.triples((None,None,from_uri)):
         g.remove((s,p,o))
-        g.add((s,p,to_uri))
+        g.add((s,p,to_uri)) #type: ignore
 
 
 def compose(g: Graph, newgraph: Graph, res: URIRef, args: AttribDict):
     """Merges two graphs that cover the same resource (= metadata composition). Later properties will overwrite earlier ones. Newgraph will be merged into g at the end of this process."""
    
     IDENTIFIER = g.value(res, SDO.identifier) or newgraph.value(res, SDO.identifier)
     if not IDENTIFIER: IDENTIFIER = str(res)
@@ -920,24 +920,24 @@
                     g.remove((s,p,o_old))
 
     #some correcting operations on the newgraph
     correct(newgraph, res, args)
 
     #there must be NO blank nodes anymore at this point!!! They might collide
     g += newgraph
-    print(f"{HEAD} processed {len(newgraph)} new triples, total is now {len(g)}",file=sys.stderr)
+    print(f"{HEAD} processed {len(newgraph)} new triples, total is now {len(g)}",file=sys.stderr) #type: ignore
 
 def different_domain(res: URIRef, res2: URIRef) -> bool:
     if res.startswith("http") and res2.startswith("http"):
         return res.split('/')[2] != res2.split('/')[2]
     else:
         return False
 
 
-def correct(g:Graph, res: URIRef, args: AttribDict):
+def correct(g:Graph, res: Union[URIRef,BNode], args: AttribDict):
     """Runs several automatic correction operations on the graph"""
 
     IDENTIFIER = g.value(res, SDO.identifier)
     if not IDENTIFIER: IDENTIFIER = str(res)
     HEAD = f"[CODEMETA CORRECTION ({IDENTIFIER})]"
 
     #when developmentStatus is a repostatus id, convert it to the full URI
@@ -992,35 +992,38 @@
     s = ""
     for arg in args:
         if s and s[-1] != "/": s += "/"
         s += arg
     return s
 
 def generate_uri(identifier: Union[str,None] = None, baseuri: Union[str,None] = None, prefix: str= ""):
-    """Generate an URI (aka IRI)"""
+    """Generate an URI"""
     if not identifier:
         identifier = "N" + "%032x" % random.getrandbits(128)
     else:
         identifier = identifier.lower()
+        #some symbols we handle specially:
         for pattern, replacement in IDENTIFIER_MAP:
             identifier = identifier.replace(pattern,replacement) #not the most efficient but it'll do
-        identifier = identifier.strip("-")
+        identifier = unicodedata.normalize("NFKD", identifier)
+        identifier = re.sub(r"[^a-z0-9]+", "-", identifier).strip("-")
+        identifier = re.sub(r"[-]+", "-", identifier)
     if prefix and prefix[-1] not in ('/','#'):
         prefix += '/'
     if not baseuri:
         baseuri = "file:///" #relative URI! (authority part file:// to be compatible with what rdflib assumes by default)
     elif baseuri[-1] not in ('/','#'):
         baseuri += '/'
     return baseuri + prefix + identifier
 
 def query(g: Graph, sparql_query: str, restype=SDO.SoftwareSourceCode):
     results = []
     for result in g.query(sparql_query):
         try:
-            if result.res and (result.res, RDF.type, restype) in g:
-                label = g.value(result.res, SDO.name)
+            if result.res and (result.res, RDF.type, restype) in g: # type: ignore
+                label = g.value(result.res, SDO.name) # type: ignore
                 if label:
-                    results.append((result.res, label))
+                    results.append((result.res, label)) # type: ignore
         except AttributeError:
             raise ValueError("Invalid query: Expected ?res in SPARQL query")
     results.sort(key=lambda x: x[1].lower())
     return results
```

### Comparing `CodeMetaPy-2.4.1/codemeta/crosswalk.py` & `CodeMetaPy-2.5.0/codemeta/crosswalk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 import csv
 import os.path
 from collections import defaultdict
 
+
 class CWKey:
     """Crosswalk Keys, corresponds with header label in crosswalk.csv, as
     provided by the CodeMeta project"""
+
     PROP = "Property"
     PARENT = "Parent Type"
     TYPE = "Type"
     DESCRIPTION = "Description"
     PYPI = "Python Distutils (PyPI)"
     DEBIAN = "Debian Package"
     R = "R Package Description"
     NODEJS = "NodeJS"
     MAVEN = "Java (Maven)"
     DOAP = "DOAP"
 
-def readcrosswalk(sourcekeys=(CWKey.PYPI,CWKey.DEBIAN,CWKey.NODEJS, CWKey.MAVEN)):
+
+def readcrosswalk(sourcekeys=(CWKey.PYPI, CWKey.DEBIAN, CWKey.NODEJS, CWKey.MAVEN)):
     """Read the crosswalk.csv as provided by codemeta into memory"""
-    #pylint: disable=W0621
+    # pylint: disable=W0621
     crosswalk = defaultdict(dict)
-    #pip may output things differently than recorded in distutils/setup.py, so we register some aliases:
+    # pip may output things differently than recorded in distutils/setup.py, so we register some aliases:
     crosswalk[CWKey.PYPI]["home-page"] = "url"
     crosswalk[CWKey.PYPI]["summary"] = "description"
     props = {}
-    crosswalkfile = os.path.join(os.path.dirname(__file__), 'schema','crosswalk.csv')
-    with open(crosswalkfile, 'r', encoding="utf-8") as f:
+    crosswalkfile = os.path.join(os.path.dirname(__file__), "schema", "crosswalk.csv")
+    with open(crosswalkfile, "r", encoding="utf-8") as f:
         reader = csv.DictReader(f)
         for row in reader:
-            props[row[CWKey.PROP]] = {"PARENT": row[CWKey.PARENT], "TYPE": row[CWKey.TYPE], "DESCRIPTION": row[CWKey.DESCRIPTION] }
+            props[row[CWKey.PROP]] = {
+                "PARENT": row[CWKey.PARENT],
+                "TYPE": row[CWKey.TYPE],
+                "DESCRIPTION": row[CWKey.DESCRIPTION],
+            }
             for sourcekey in sourcekeys:
                 if row[sourcekey]:
-                    for key in [ x.strip().lower() for x in row[sourcekey].split("/") ]:
+                    for key in [x.strip().lower() for x in row[sourcekey].split("/")]:
                         crosswalk[sourcekey][key] = row[CWKey.PROP]
 
     return props, crosswalk
```

### Comparing `CodeMetaPy-2.4.1/codemeta/parsers/debian.py` & `CodeMetaPy-2.5.0/codemeta/parsers/debian.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,75 @@
 import sys
 from typing import Union
 from rdflib import Graph, URIRef, BNode, Literal
-from rdflib.namespace import RDF
-from codemeta.common import AttribDict, add_triple, CODEMETA, SOFTWARETYPES, SDO, SOFTWARETYPES, generate_uri
+from rdflib.namespace import RDF #type: ignore
+from codemeta.common import (
+    AttribDict,
+    add_triple,
+    CODEMETA,
+    SOFTWARETYPES,
+    SDO,
+    SOFTWARETYPES,
+    generate_uri,
+)
 from codemeta.crosswalk import readcrosswalk, CWKey
 
-def parse_debian(g: Graph, res: Union[URIRef, BNode], lines, crosswalk, args: AttribDict):
+
+def parse_debian(
+    g: Graph, res: Union[URIRef, BNode], lines, crosswalk, args: AttribDict
+):
     """Parses apt show output and converts to codemeta"""
     if crosswalk is None:
         _, crosswalk = readcrosswalk((CWKey.DEBIAN,))
 
     name = None
     interfacetype = None
     description = ""
     parsedescription = False
     for line in lines:
-        if parsedescription and line and line[0] == ' ':
+        if parsedescription and line and line[0] == " ":
             description += line[1:] + " "
         else:
             try:
-                key, value = (x.strip() for x in line.split(':',1))
+                key, value = (x.strip() for x in line.split(":", 1))
             except:
                 continue
             if key == "Origin":
                 if value == "Debian":
                     provider = URIRef("https://www.debian.org")
                     g.add((provider, RDF.type, SDO.Organization))
                     g.add((provider, SDO.name, Literal("The Debian Project")))
                     g.add((provider, SDO.url, Literal("https://www.debian.org")))
-                    g.add((res,SDO.provider,provider))
+                    g.add((res, SDO.provider, provider))
                 elif value == "Ubuntu":
                     provider = URIRef("https://ubuntu.com")
                     g.add((provider, RDF.type, SDO.Organization))
                     g.add((provider, SDO.name, Literal("Ubuntu")))
                     g.add((provider, SDO.url, Literal("https://ubuntu.com")))
-                    g.add((res,SDO.provider,provider))
+                    g.add((res, SDO.provider, provider))
                 else:
-                    print(f"WARNING: Don't know how to convert Origin: {value}",file=sys.stderr)
+                    print(
+                        f"WARNING: Don't know how to convert Origin: {value}",
+                        file=sys.stderr,
+                    )
             elif key == "Depends":
                 for dependency in value.split(","):
                     dependency = dependency.strip().split(" ")[0].strip()
                     if dependency:
-                        depnode = URIRef(generate_uri(dependency, baseuri=args.baseuri,prefix="dependency"))
+                        depnode = URIRef(
+                            generate_uri(
+                                dependency, baseuri=args.baseuri, prefix="dependency"
+                            )
+                        )
                         g.add((depnode, RDF.type, SDO.SoftwareApplication))
                         g.add((depnode, SDO.identifier, Literal(dependency)))
                         g.add((depnode, SDO.name, Literal(dependency)))
                         g.add((res, CODEMETA.softwareRequirements, depnode))
             elif key == "Section":
-                #attempt to make an educated guess for the audience and interface type
+                # attempt to make an educated guess for the audience and interface type
                 if "libs" in value or "libraries" in value:
                     if args.with_stypes:
                         interfacetype = SOFTWARETYPES.SoftwareLibrary
                         add_triple(g, res, "audience", "Developers", args)
                 elif "utils" in value or "text" in value:
                     if args.with_stypes:
                         interfacetype = SOFTWARETYPES.CommandLineApplication
@@ -69,22 +87,23 @@
             elif key.lower() in crosswalk[CWKey.DEBIAN]:
                 if key == "Package":
                     name = value
                 else:
                     key = crosswalk[CWKey.DEBIAN][key.lower()]
                     add_triple(g, res, key, value, args)
             else:
-                print("WARNING: No translation for APT key " + key,file=sys.stderr)
+                print("WARNING: No translation for APT key " + key, file=sys.stderr)
     if name:
         g.add((res, SDO.name, Literal(name)))
         g.add((res, SDO.identifier, Literal(name)))
     else:
-        print("No name found for package, should not happen",file=sys.stderr)
+        print("No name found for package, should not happen", file=sys.stderr)
         return False
     if description:
         g.add((res, SDO.description, Literal(description)))
     if interfacetype and args.with_stypes:
-        sapp = URIRef(generate_uri(name, baseuri=args.baseuri,prefix=str(interfacetype).lower()))
+        sapp = URIRef(
+            generate_uri(name, baseuri=args.baseuri, prefix=str(interfacetype).lower())
+        )
         g.add((sapp, RDF.type, interfacetype))
         g.add((sapp, SDO.name, name))
         g.add((res, SDO.targetProduct, sapp))
-
```

### Comparing `CodeMetaPy-2.4.1/codemeta/parsers/gitapi.py` & `CodeMetaPy-2.5.0/codemeta/parsers/gitapi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,245 +1,310 @@
 import sys
 import requests
 import time
 from os import environ
 from datetime import datetime
-from io import StringIO
-from typing import Union, IO, Optional, Tuple
+from typing import Union, Optional, Tuple
 from rdflib import Graph, URIRef, BNode, Literal
-from rdflib.namespace import RDF
-from codemeta.common import AttribDict, SDO, CODEMETA, license_to_spdx, parse_human_name, generate_uri
-from codemeta.parsers.jsonld import parse_jsonld_data
-
-GITAPI_REPO_BLACKLIST=["https://codeberg.org/","http://codeberg.org", "https://git.sr.ht/", "https://bitbucket.com/"]
-#it shall be persistent because each new yaml a new invoke of codemetapy is performed and so memory reset
+from rdflib.namespace import RDF #type: ignore
+from codemeta.common import (
+    AttribDict,
+    SDO,
+    CODEMETA,
+    license_to_spdx,
+    parse_human_name,
+    generate_uri,
+)
+
+GITAPI_REPO_BLACKLIST = [
+    "https://codeberg.org/",
+    "http://codeberg.org",
+    "https://git.sr.ht/",
+    "https://bitbucket.com/",
+]
+# it shall be persistent because each new yaml a new invoke of codemetapy is performed and so memory reset
 repo_type_cache = {}
 
-def _parse_source(source:str) -> Tuple[str,str,str]:
-    source=source.strip("/")
-    cleaned_url= source
-    scheme=""
+
+def _parse_source(source: str) -> Tuple[str, str, str]:
+    source = source.strip("/")
+    cleaned_url = source
+    scheme = ""
     if source.startswith("https://"):
-        host = cleaned_url.replace('https://','').split('/')[0]
-        scheme="https://"
+        host = cleaned_url.replace("https://", "").split("/")[0]
+        scheme = "https://"
     else:
         raise ValueError(source + " source url format not recognized!!")
     return cleaned_url, scheme, host
- 
 
 
 def get_repo_kind(source: str) -> Optional[str]:
     source, scheme, host = _parse_source(source)
- 
+
     repo_kind = None
     if "github.com/" in source:
         repo_kind = "github"
     elif "gitlab.com/" in source:
         repo_kind = "gitlab"
     elif f"{scheme}{host}/" not in GITAPI_REPO_BLACKLIST:
-        #we have another URL that may or may not be a private gitlab instance, test
+        # we have another URL that may or may not be a private gitlab instance, test
         if f"{scheme}{host}/" in repo_type_cache:
             repo_kind = repo_type_cache[f"{scheme}{host}/"]
         else:
-            test_url = f"{scheme}{host}/-/manifest.json"  #this seems a relatively cheap way to test if it's a gitlab instance
+            test_url = f"{scheme}{host}/-/manifest.json"  # this seems a relatively cheap way to test if it's a gitlab instance
             response = requests.get(test_url)
-            if response.status_code == 200 and response.headers['Content-Type'].startswith("application/json"):
+            if response.status_code == 200 and response.headers[
+                "Content-Type"
+            ].startswith("application/json"):
                 response = response.json()
-                if response['short_name'] == 'GitLab':
+                if response["short_name"] == "GitLab":
                     repo_kind = "gitlab"
 
-    #Populate the cache even when there is a 4xx failure
+    # Populate the cache even when there is a 4xx failure
     repo_type_cache[f"{scheme}{host}/"] = repo_kind
 
     return repo_kind
 
-def parse(g: Graph, res: Union[URIRef, BNode], source: str, repo_kind:str, args: AttribDict) -> str:
+
+def parse(
+    g: Graph, res: Union[URIRef, BNode], source: str, repo_kind: str, args: AttribDict
+) -> str:
     source, scheme, host = _parse_source(source)
- 
-    github_suffix=source.replace(scheme + host,'')[1:]
-    gitlab_suffix=github_suffix.replace('/', '%2F')
+
+    github_suffix = source.replace(scheme + host, "")[1:]
+    gitlab_suffix = github_suffix.replace("/", "%2F")
     gitlab_repo_api_url = f"{scheme}{host}/api/v4/projects/{gitlab_suffix}"
 
     if repo_kind == "github":
-        response = rate_limit_get(f"{scheme}api.github.com/repos/{github_suffix}", "github")
-        _parse_github(response, g,res,f"{scheme}{host}", args)
+        response = rate_limit_get(
+            f"{scheme}api.github.com/repos/{github_suffix}", "github"
+        )
+        _parse_github(response, g, res, f"{scheme}{host}", args)
     elif repo_kind == "gitlab":
         response = rate_limit_get(gitlab_repo_api_url, "gitlab")
-        _parse_gitlab(response, g,res,f"{scheme}{host}", args)  
+        _parse_gitlab(response, g, res, f"{scheme}{host}", args)
     else:
         raise ValueError(f"Not a git API, repo_kind={repo_kind}")
 
     return source
 
+
 github_crosswalk_table = {
     SDO.codeRepository: "html_url",
     SDO.dateCreated: "created_at",
     SDO.dateModified: "pushed_at",
     SDO.description: "description",
     SDO.name: "name",
 }
-#"owner": ["owner", "login"],
-#"ownerType": ["owner", "type"],  # used to determine if owner is User or Organization
+# "owner": ["owner", "login"],
+# "ownerType": ["owner", "type"],  # used to determine if owner is User or Organization
+
 
 # the same as requests.get(args).json(), but protects against rate limiting
 # Adapted from source: https://github.com/KnowledgeCaptureAndDiscovery/somef (MIT licensed)
-def rate_limit_get(url:str, repo_kind: Optional[str], backoff_rate=2, initial_backoff=1, **kwargs) -> dict: 
+def rate_limit_get(
+    url: str, repo_kind: Optional[str], backoff_rate=2, initial_backoff=1, **kwargs
+) -> dict:
     rate_limited = True
     data = {}
-    has_token=False
-    if not kwargs: kwargs = {}
-    if repo_kind == "github" and 'GITHUB_TOKEN' in environ and environ['GITHUB_TOKEN']:
-        if 'headers' not in kwargs: kwargs['headers'] = {}
-        kwargs['headers']["Authorization"] = "token " + environ['GITHUB_TOKEN']
+    has_token = False
+    if not kwargs:
+        kwargs = {}
+    if repo_kind == "github" and "GITHUB_TOKEN" in environ and environ["GITHUB_TOKEN"]:
+        if "headers" not in kwargs:
+            kwargs["headers"] = {}
+        kwargs["headers"]["Authorization"] = "token " + environ["GITHUB_TOKEN"]
         has_token = True
-    elif repo_kind == "gitlab" and 'GITLAB_TOKEN' in environ and environ['GITLAB_TOKEN']:
-        if 'headers' not in kwargs: kwargs['headers'] = {}
-        kwargs['headers']["PRIVATE-TOKEN"] = environ['GITLAB_TOKEN']
+    elif (
+        repo_kind == "gitlab" and "GITLAB_TOKEN" in environ and environ["GITLAB_TOKEN"]
+    ):
+        if "headers" not in kwargs:
+            kwargs["headers"] = {}
+        kwargs["headers"]["PRIVATE-TOKEN"] = environ["GITLAB_TOKEN"]
         has_token = True
     while rate_limited:
         print(f"Querying {url}")
         response = requests.get(url, **kwargs)
-        rate_limit_remaining = int(response.headers.get("RateLimit-Remaining" if repo_kind == "gitlab" else "x-ratelimit-remaining",-1))
-        epochtime = int(response.headers.get("RateLimit-Reset" if repo_kind == "gitlab" else  "x-ratelimit-reset",0))
+        rate_limit_remaining = int(
+            response.headers.get(
+                "RateLimit-Remaining"
+                if repo_kind == "gitlab"
+                else "x-ratelimit-remaining",
+                -1,
+            )
+        )
+        epochtime = int(
+            response.headers.get(
+                "RateLimit-Reset" if repo_kind == "gitlab" else "x-ratelimit-reset", 0
+            )
+        )
         if rate_limit_remaining > -1 and epochtime > 0:
             date_reset = datetime.fromtimestamp(epochtime)
-            print(f"Remaining {repo_kind} API requests: {rate_limit_remaining} ### Next rate limit reset at: {date_reset} (has_token={has_token})")
+            print(
+                f"Remaining {repo_kind} API requests: {rate_limit_remaining} ### Next rate limit reset at: {date_reset} (has_token={has_token})"
+            )
         else:
             rate_limited = False
         data = response.json()
-        if 'message' in data and 'API rate limit exceeded' in data['message']:
+        if "message" in data and "API rate limit exceeded" in data["message"]:
             rate_limited = True
-            print(f"{repo_kind} API: rate limited. Backing off for {initial_backoff} seconds (has_token={has_token})", file=sys.stderr)
+            print(
+                f"{repo_kind} API: rate limited. Backing off for {initial_backoff} seconds (has_token={has_token})",
+                file=sys.stderr,
+            )
             sys.stderr.flush()
             if initial_backoff > 120:
-                raise Exception(f"{repo_kind} API timed out because of rate limiting, giving up... (has_token={has_token})")
+                raise Exception(
+                    f"{repo_kind} API timed out because of rate limiting, giving up... (has_token={has_token})"
+                )
             time.sleep(initial_backoff)
             # increase the backoff for next time
             initial_backoff *= backoff_rate
         else:
             response.raise_for_status()
             rate_limited = False
     return data
 
-def _parse_github(response: dict, g: Graph, res: Union[URIRef, BNode], source: str, args: AttribDict):
+
+def _parse_github(
+    response: dict, g: Graph, res: Union[URIRef, BNode], source: str, args: AttribDict
+):
     """Query and parse from the github API"""
-    print(f"    Parsing Github API response",file=sys.stderr)
-    users_api_url=f"https://api.github.com/users/"
-    
-    #repo = response['name']
+    print(f"    Parsing Github API response", file=sys.stderr)
+    users_api_url = f"https://api.github.com/users/"
+
+    # repo = response['name']
     for prop, github_key in github_crosswalk_table.items():
         if github_key in response and response[github_key]:
             g.add((res, prop, Literal(response[github_key])))
 
-    if response.get('license') and response['license'].get('spdx_id'):
-        g.add((res, SDO.license, Literal(license_to_spdx(response['license']['spdx_id']))))
+    if response.get("license") and response["license"].get("spdx_id"):
+        g.add(
+            (res, SDO.license, Literal(license_to_spdx(response["license"]["spdx_id"])))
+        )
 
     if response.get("topics"):
-        for topic in response['topics']:
+        for topic in response["topics"]:
             g.add((res, SDO.keywords, Literal(topic)))
 
     if response.get("homepage"):
-        g.add((res, SDO.url, Literal(response['homepage'])))
+        g.add((res, SDO.url, Literal(response["homepage"])))
 
-    if response.get('has_issues', False) and response.get("html_url"):
-        g.add((res, CODEMETA.issueTracker, Literal(response['html_url'] + "/issues")))
+    if response.get("has_issues", False) and response.get("html_url"):
+        g.add((res, CODEMETA.issueTracker, Literal(response["html_url"] + "/issues")))
 
-    if 'owner' in response:
-        owner = response['owner']['login']
+    if "owner" in response:
+        owner = response["owner"]["login"]
         owner_api_url = f"{users_api_url}{owner}"
         response = rate_limit_get(owner_api_url, "github")
-        owner_type = response.get("type","").lower()
+        owner_type = response.get("type", "").lower()
         owner_res = None
-        if owner_type == "user" and response.get('name'):
-            firstname, lastname = parse_human_name(response['name'])
-            owner_res = URIRef(generate_uri(firstname + "-" + lastname, args.baseuri, prefix="person"))
+        if owner_type == "user" and response.get("name"):
+            firstname, lastname = parse_human_name(response["name"])
+            owner_res = URIRef(
+                generate_uri(firstname + "-" + lastname, args.baseuri, prefix="person")
+            )
             g.add((owner_res, RDF.type, SDO.Person))
             g.add((owner_res, SDO.givenName, Literal(firstname)))
             g.add((owner_res, SDO.familyName, Literal(lastname)))
             g.add((res, SDO.author, owner_res))
             g.add((res, SDO.maintainer, owner_res))
-            if response.get('company'):
-                affil_res = URIRef(generate_uri(response.get('company'), args.baseuri, prefix="org"))
+            if response.get("company"):
+                affil_res = URIRef(
+                    generate_uri(response.get("company"), args.baseuri, prefix="org")
+                )
                 g.add((affil_res, RDF.type, SDO.Organization))
-                g.add((affil_res, SDO.name, Literal(response['company'])))
+                g.add((affil_res, SDO.name, Literal(response["company"])))
                 g.add((owner_res, SDO.affiliation, affil_res))
-        elif owner_type == "organization" and response.get('name'):
-            owner_res = URIRef(generate_uri(response.get('name'), args.baseuri, prefix="org"))
+        elif owner_type == "organization" and response.get("name"):
+            owner_res = URIRef(
+                generate_uri(response.get("name"), args.baseuri, prefix="org")
+            )
             g.add((owner_res, RDF.type, SDO.Organization))
-            g.add((owner_res, SDO.name, Literal(response.get('name'))))
+            g.add((owner_res, SDO.name, Literal(response.get("name"))))
             g.add((res, SDO.producer, owner_res))
         if owner_res:
-            if response.get('email'):
-                g.add((owner_res, SDO.email, Literal(response.get('email'))))
-            if response.get('blog'):
-                g.add((owner_res, SDO.url, Literal(response.get('blog'))))
+            if response.get("email"):
+                g.add((owner_res, SDO.email, Literal(response.get("email"))))
+            if response.get("blog"):
+                g.add((owner_res, SDO.url, Literal(response.get("blog"))))
 
 
 gitlab_crosswalk_table = {
     SDO.codeRepository: "web_url",
     SDO.dateCreated: "created_at",
     SDO.dateModified: "last_activity_at",
     SDO.description: "description",
     SDO.name: "name",
-    SDO.url: "web_url"
+    SDO.url: "web_url",
 }
-def _parse_gitlab(response: dict, g: Graph, res: Union[URIRef, BNode], source, args: AttribDict):
+
+
+def _parse_gitlab(
+    response: dict, g: Graph, res: Union[URIRef, BNode], source, args: AttribDict
+):
     """Query and parse from the gitlab API"""
     users_api_url = f"{source}/api/v4/users/"
-    #Processing start
+    # Processing start
     for prop, gitlab_key in gitlab_crosswalk_table.items():
         if gitlab_key in response and response[gitlab_key]:
             g.add((res, prop, Literal(response[gitlab_key])))
 
-    if response.get('license') and response['license'].get('nickname'):
-        g.add((res, SDO.license, Literal(license_to_spdx(response['license']['nickname']))))
+    if response.get("license") and response["license"].get("nickname"):
+        g.add(
+            (
+                res,
+                SDO.license,
+                Literal(license_to_spdx(response["license"]["nickname"])),
+            )
+        )
     if response.get("topics"):
-        for topic in response['topics']:
+        for topic in response["topics"]:
             g.add((res, SDO.keywords, Literal(topic)))
     if response.get("homepage"):
-        g.add((res, SDO.url, Literal(response['homepage'])))
+        g.add((res, SDO.url, Literal(response["homepage"])))
     elif response.get("web_url"):
-        g.add((res, SDO.url, Literal(response['web_url'])))
-    if response.get('open_issues_count', False) > 0:
-        g.add((res, CODEMETA.issueTracker, Literal(response['_links']['issues'])))
-
-    #https://docs.gitlab.com/ee/api/users.html
-    #namespace kind can be just group or user
-    owner_id_str=""
-    owner_name=""
-    user_url=""
-    public_mail=""
-    if 'namespace' in response and response['namespace']['kind'] == 'user':
-        owner_id_str=str(response['namespace']['id'])
+        g.add((res, SDO.url, Literal(response["web_url"])))
+    if response.get("open_issues_count", False) > 0:
+        g.add((res, CODEMETA.issueTracker, Literal(response["_links"]["issues"])))
+
+    # https://docs.gitlab.com/ee/api/users.html
+    # namespace kind can be just group or user
+    owner_id_str = ""
+    owner_name = ""
+    user_url = ""
+    public_mail = ""
+    if "namespace" in response and response["namespace"]["kind"] == "user":
+        owner_id_str = str(response["namespace"]["id"])
         owner_api_url = users_api_url + owner_id_str
-        owner_name=response['namespace']['name']
-        user_url=response['namespace']['web_url']
-    elif 'owner' in response:
-        owner_id_str=str(response['owner']['id'])
+        owner_name = response["namespace"]["name"]
+        user_url = response["namespace"]["web_url"]
+    elif "owner" in response:
+        owner_id_str = str(response["owner"]["id"])
         owner_api_url = users_api_url + owner_id_str
         response_owner = rate_limit_get(owner_api_url, "gitlab")
-        owner_name=response_owner['owner']['name']
-        user_url=response_owner['owner']['web_url']
-        if response_owner.get('public_email'):
-            public_mail = response_owner.get('public_email')
-    else:  
+        owner_name = response_owner["owner"]["name"]
+        user_url = response_owner["owner"]["web_url"]
+        if response_owner.get("public_email"):
+            public_mail = response_owner.get("public_email")
+    else:
         return
     firstname, lastname = parse_human_name(owner_name)
     owner_res = URIRef(user_url)
     g.add((owner_res, RDF.type, SDO.Person))
     g.add((owner_res, SDO.givenName, Literal(firstname)))
     g.add((owner_res, SDO.familyName, Literal(lastname)))
     g.add((owner_res, SDO.url, Literal(user_url)))
     if public_mail != "":
         g.add((owner_res, SDO.email, Literal(public_mail)))
-    #Creator considered as author
-    response_creator_url_field=user_url
-    response_creator_name=owner_name
-    if 'creator_id' in response:
-     creator_id_str = str(response['creator_id'])
-     if creator_id_str != owner_id_str:
-        creator_api_url = users_api_url +  creator_id_str
-        response_creator = rate_limit_get(creator_api_url, "gitlab")
-        response_creator_url_field=response_creator['web_url']
-    #Object X must be an rdflib term:  g.add((URIRef(response_creator_url_field), SDO.author, response_creator_name))
-    #g.add((res, SDO.maintainer, owner_res))
-    #if response_owner.get('work_information'): is like company?
+    # Creator considered as author
+    response_creator_url_field = user_url
+    response_creator_name = owner_name
+    if "creator_id" in response:
+        creator_id_str = str(response["creator_id"])
+        if creator_id_str != owner_id_str:
+            creator_api_url = users_api_url + creator_id_str
+            response_creator = rate_limit_get(creator_api_url, "gitlab")
+            response_creator_url_field = response_creator["web_url"]
+    # Object X must be an rdflib term:  g.add((URIRef(response_creator_url_field), SDO.author, response_creator_name))
+    # g.add((res, SDO.maintainer, owner_res))
+    # if response_owner.get('work_information'): is like company?
```

### Comparing `CodeMetaPy-2.4.1/codemeta/parsers/java.py` & `CodeMetaPy-2.5.0/codemeta/parsers/java.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,70 @@
-import sys
-import json
-import os.path
 from typing import Union, IO
 from rdflib import Graph, URIRef, BNode, Literal
-from rdflib.namespace import RDF
+from rdflib.namespace import RDF #type: ignore
 import lxml.etree
-from codemeta.common import AttribDict, add_triple, CODEMETA, SOFTWARETYPES, add_authors, SDO, COMMON_SOURCEREPOS, SOFTWARETYPES, license_to_spdx, generate_uri
-from codemeta.crosswalk import readcrosswalk, CWKey
+from codemeta.common import (
+    AttribDict,
+    add_triple,
+    CODEMETA,
+    add_authors,
+    SDO,
+    license_to_spdx,
+    generate_uri,
+)
+from codemeta.crosswalk import CWKey
 
 POM_NAMESPACE = "http://maven.apache.org/POM/4.0.0"
 
+
 def parse_node(node):
     for subnode in node:
-        if isinstance(subnode.tag, str) and subnode.tag.startswith("{" + POM_NAMESPACE + "}"):
-            key = subnode.tag[len(POM_NAMESPACE) + 2:]
+        if isinstance(subnode.tag, str) and subnode.tag.startswith(
+            "{" + POM_NAMESPACE + "}"
+        ):
+            key = subnode.tag[len(POM_NAMESPACE) + 2 :]
             yield key, subnode
 
+
 def parse_author(g, res, node, property=SDO.author):
     author_name = ""
     author_mail = ""
     author_url = ""
     org = ""
     for key3, node3 in parse_node(node):
         if key3 == "name":
             author_name = node3.text
         elif key3 == "email":
             author_mail = node3.text
         elif key3 == "url":
             author_url = node3.text
         elif key3 == "organisation":
             org = node3.text
-    return add_authors(g, res, author_name, property=property, single_author=True, mail=author_mail, url=author_url,org=org)
+    return add_authors(
+        g,
+        res,
+        author_name,
+        property=property,
+        single_author=True,
+        mail=author_mail,
+        url=author_url,
+        org=org,
+    )
 
 
-def parse_java(g: Graph, res: Union[URIRef, BNode], file: IO , crosswalk, args: AttribDict):
+def parse_java(
+    g: Graph, res: Union[URIRef, BNode], file: IO, crosswalk, args: AttribDict
+):
     data = lxml.etree.parse(file)
 
     root = data.getroot()
     if root.tag != "{" + POM_NAMESPACE + "}project":
-        raise Exception(f"Expected root tag 'project' in {POM_NAMESPACE} namespace, got {root.tag} instead")
+        raise Exception(
+            f"Expected root tag 'project' in {POM_NAMESPACE} namespace, got {root.tag} instead"
+        )
 
     group_id = None
     artifact_id = None
 
     g.add((res, SDO.runtimePlatform, Literal("Java")))
     g.add((res, SDO.programmingLanguage, Literal("Java")))
 
@@ -50,97 +72,131 @@
         if key == "licenses":
             for key2, node2 in parse_node(node):
                 if key2 == "license":
                     license = ""
                     for key3, node3 in parse_node(node2):
                         if key3 == "name":
                             license = license_to_spdx(node3.text)
-                        if isinstance(license, str) and license.find("spdx") == -1 and key3 == "url":
+                        if (
+                            isinstance(license, str)
+                            and license.find("spdx") == -1
+                            and key3 == "url"
+                        ):
                             license = node3.text
                     if license:
-                        add_triple(g,res, "license", license, args)
+                        add_triple(g, res, "license", license, args)
         elif key == "issueManagement":
             for key2, node2 in parse_node(node):
-                if key2 == "url" and '$' not in node2.text: #only if there are no variables in the url!
-                    add_triple(g,res, "issueTracker", node2.text, args)
+                if (
+                    key2 == "url" and "$" not in node2.text
+                ):  # only if there are no variables in the url!
+                    add_triple(g, res, "issueTracker", node2.text, args)
         elif key == "ciManagement":
             for key2, node2 in parse_node(node):
-                if key2 == "url" and '$' not in node2.text: #only if there are no variables in the url!
-                    add_triple(g,res, "contIntegration", node2.text, args)
+                if (
+                    key2 == "url" and "$" not in node2.text
+                ):  # only if there are no variables in the url!
+                    add_triple(g, res, "contIntegration", node2.text, args)
         elif key == "scm":
             for key2, node2 in parse_node(node):
-                if key2 == "url" and '$' not in node2.text: #only if there are no variables in the url!
-                    add_triple(g,res, "codeRepository", node2.text, args)
+                if (
+                    key2 == "url" and "$" not in node2.text
+                ):  # only if there are no variables in the url!
+                    add_triple(g, res, "codeRepository", node2.text, args)
         elif key == "repositories":
             for key2, node2 in parse_node(node):
                 if key2 == "repository":
                     for key3, node3 in parse_node(node2):
-                        if key3 == "url" and '$' not in node3.text: #only if there are no variables in the url!
-                            add_triple(g,res, "repository", node3.text, args)
+                        if (
+                            key3 == "url" and "$" not in node3.text
+                        ):  # only if there are no variables in the url!
+                            add_triple(g, res, "repository", node3.text, args)
         elif key == "properties":
             for key2, node2 in parse_node(node):
                 if key2 == "java.version":
                     g.add((res, SDO.runtimePlatform, Literal("Java " + node2.text)))
-        elif key == 'groupId':
+        elif key == "groupId":
             group_id = node.text
-        elif key == 'artifactId':
+        elif key == "artifactId":
             artifact_id = node.text
-        elif key == 'dependencies':
+        elif key == "dependencies":
             for key2, node2 in parse_node(node):
                 if key2 == "dependency":
                     dep_group_id = dep_art_id = dep_version = ""
                     for key3, node3 in parse_node(node2):
                         if key3 == "groupId":
                             dep_group_id = node3.text
                         elif key3 == "artifactId":
                             dep_art_id = node3.text
-                        elif key3 == "version" and node3.text and not node3.text.startswith('$'):
+                        elif (
+                            key3 == "version"
+                            and node3.text
+                            and not node3.text.startswith("$")
+                        ):
                             dep_version = node3.text
 
                     if dep_group_id and dep_art_id:
-                        depres = URIRef(generate_uri(dep_group_id +"." + dep_art_id + "." + dep_version.replace(" ",""), baseuri=args.baseuri,prefix="dependency"))
-                        g.add((depres, SDO.identifier, Literal(dep_group_id + "." + dep_art_id)))
+                        depres = URIRef(
+                            generate_uri(
+                                dep_group_id
+                                + "."
+                                + dep_art_id
+                                + "."
+                                + dep_version.replace(" ", ""),
+                                baseuri=args.baseuri,
+                                prefix="dependency",
+                            )
+                        )
+                        g.add(
+                            (
+                                depres,
+                                SDO.identifier,
+                                Literal(dep_group_id + "." + dep_art_id),
+                            )
+                        )
                         g.add((depres, SDO.name, Literal(dep_art_id)))
                         if dep_version:
                             g.add((depres, SDO.version, Literal(dep_version)))
                         g.add((depres, RDF.type, SDO.SoftwareApplication))
                         g.add((res, CODEMETA.softwareRequirements, depres))
-        elif key == 'developers':
+        elif key == "developers":
             for key2, node2 in parse_node(node):
                 if key2 == "developer":
                     parse_author(g, res, node2)
-        elif key == 'contributors':
+        elif key == "contributors":
             for key2, node2 in parse_node(node):
                 if key2 == "contributor":
                     parse_author(g, res, node2, property=SDO.contributor)
-        elif key == 'mailingLists':
+        elif key == "mailingLists":
             for key2, node2 in parse_node(node):
                 if key2 == "mailingList":
                     for key3, node3 in parse_node(node2):
                         if key3 == "post":
                             add_triple(g, res, "email", node3.text, args)
-        elif key == 'organization':
+        elif key == "organization":
             org_name = None
             org_url = None
             for key2, node2 in parse_node(node):
                 if key2 == "name":
                     org_name = node2.text
                 elif key2 == "url":
                     org_url = node2.text
             if org_name:
-                orgres = URIRef(generate_uri(org_name, baseuri=args.baseuri, prefix="org"))
+                orgres = URIRef(
+                    generate_uri(org_name, baseuri=args.baseuri, prefix="org")
+                )
                 g.add((orgres, SDO.name, Literal(org_name)))
                 if org_url:
                     g.add((orgres, SDO.url, Literal(org_url)))
                 g.add((res, SDO.producer, orgres))
         elif key.lower() in crosswalk[CWKey.MAVEN]:
             value = node.text
             if group_id and value.find("${project.groupId}") != -1:
                 value = value.replace("${project.groupId}", group_id)
             if artifact_id and value.find("${project.artifactId}") != -1:
                 value = value.replace("${project.artifactId}", artifact_id)
             key = crosswalk[CWKey.MAVEN][key.lower()]
-            if key != 'identifier':
+            if key != "identifier":
                 add_triple(g, res, key, value, args)
 
     if group_id and artifact_id:
         add_triple(g, res, "identifier", group_id + "." + artifact_id, args)
```

### Comparing `CodeMetaPy-2.4.1/codemeta/parsers/jsonld.py` & `CodeMetaPy-2.5.0/codemeta/parsers/jsonld.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,182 +1,239 @@
 import sys
 import json
 import os
 from rdflib import Graph, URIRef, BNode, Literal
 from typing import Union, IO, Optional
-from codemeta.common import  PREFER_URIREF_PROPERTIES, AttribDict, REPOSTATUS, license_to_spdx, SDO, CODEMETA, SCHEMA_SOURCE, CODEMETA_SOURCE, SCHEMA_LOCAL_SOURCE, SCHEMA_SOURCE, CODEMETA_LOCAL_SOURCE, CODEMETA_SOURCE, STYPE_SOURCE, STYPE_LOCAL_SOURCE, IODATA_SOURCE, IODATA_LOCAL_SOURCE, init_context, SINGULAR_PROPERTIES, generate_uri, bind_graph, DEVIANT_CONTEXT
+from codemeta.common import (
+    PREFER_URIREF_PROPERTIES,
+    AttribDict,
+    SCHEMA_SOURCE,
+    CODEMETA_SOURCE,
+    SCHEMA_LOCAL_SOURCE,
+    SCHEMA_SOURCE,
+    CODEMETA_LOCAL_SOURCE,
+    CODEMETA_SOURCE,
+    STYPE_SOURCE,
+    STYPE_LOCAL_SOURCE,
+    IODATA_LOCAL_SOURCE,
+    init_context,
+    DEVIANT_CONTEXT,
+)
 
 
-def rewrite_context(context: Union[list,str], args: AttribDict) -> list:
+def rewrite_context(context: Union[list, str], args: AttribDict) -> list:
     """Rewrite remote contexts to their local counterparts"""
-    local_contexts = [ x[0] for x in init_context(args) ]
+    local_contexts = [x[0] for x in init_context(args)]
     if isinstance(context, list):
         for i, v in enumerate(context):
             if isinstance(v, str):
-                if v.startswith(("https://schema.org", "http://schema.org", "//schema.org")) or v == SCHEMA_SOURCE:
+                if (
+                    v.startswith(
+                        ("https://schema.org", "http://schema.org", "//schema.org")
+                    )
+                    or v == SCHEMA_SOURCE
+                ):
                     context[i] = SCHEMA_LOCAL_SOURCE
-                elif v.startswith("https://doi.org/10.5063/schema") or v == CODEMETA_SOURCE:
+                elif (
+                    v.startswith("https://doi.org/10.5063/schema")
+                    or v == CODEMETA_SOURCE
+                ):
                     context[i] = CODEMETA_LOCAL_SOURCE
                 elif v.startswith(STYPE_SOURCE):
                     context[i] = STYPE_LOCAL_SOURCE
                 elif v.startswith(IODATA_LOCAL_SOURCE):
                     context[i] = IODATA_LOCAL_SOURCE
-                elif v.startswith(("file://","//")) and v not in local_contexts:
-                    raise Exception(f"Refusing to load non-authorized local context: {v}")
+                elif v.startswith(("file://", "//")) and v not in local_contexts:
+                    raise Exception(
+                        f"Refusing to load non-authorized local context: {v}"
+                    )
 
-        #remove some legacy contexts which we may encounter but would choke on if parsed
+        # remove some legacy contexts which we may encounter but would choke on if parsed
         try:
             context.remove("https://github.com/CLARIAH/tool-metadata")
         except ValueError:
             pass
     elif isinstance(context, str):
         context = rewrite_context([context], args)
-    #ammend context
+    # ammend context
     if SCHEMA_LOCAL_SOURCE not in context:
         context.append(SCHEMA_LOCAL_SOURCE)
     if STYPE_LOCAL_SOURCE not in context:
         context.append(STYPE_LOCAL_SOURCE)
     if IODATA_LOCAL_SOURCE not in context:
         context.append(IODATA_LOCAL_SOURCE)
 
-    for key,value in DEVIANT_CONTEXT.items():
-        if {key:value} not in context:
-            context.append({key:value})
+    for key, value in DEVIANT_CONTEXT.items():
+        if {key: value} not in context:
+            context.append({key: value})
     return context
 
-def parse_jsonld(g: Graph, res: Union[BNode, URIRef,None], file_descriptor: IO, args: AttribDict) -> Union[str,None]:
+
+def parse_jsonld(
+    g: Graph, res: Union[BNode, URIRef, None], file_descriptor: IO, args: AttribDict
+) -> Union[str, None]:
     data = json.load(file_descriptor)
-    return parse_jsonld_data(g,res, data, args)
+    return parse_jsonld_data(g, res, data, args)
 
 
-def find_main_id(data: dict)  -> Union[str,None]:
+def find_main_id(data: dict) -> Union[str, None]:
     """Find the main URI in the JSON-LD resource, if there is only one, return None otherwise"""
-    if '@graph' in data and len(data['@graph']) == 1:
-        root = data['@graph'][0]
+    if "@graph" in data and len(data["@graph"]) == 1:
+        root = data["@graph"][0]
     else:
         root = data
 
-    for k in ('@id','id'):
+    for k in ("@id", "id"):
         if k in root:
             return root[k]
 
     return None
 
 
 def inject_uri(data: dict, res: URIRef):
-    if '@graph' in data and len(data['@graph']) == 1:
-        data['@graph'][0]["@id"] = str(res)
-        if 'id' in data['@graph'][0]: del data['@graph'][0]['id']
-        print(f"    Injected (possibly temporary) URI {res}",file=sys.stderr)
-    elif '@graph' in data and len(data['@graph']) == 0:
-        print("    NOTE: Graph is empty!",file=sys.stderr)
-    elif '@graph' not in data:
+    if "@graph" in data and len(data["@graph"]) == 1:
+        data["@graph"][0]["@id"] = str(res)
+        if "id" in data["@graph"][0]:
+            del data["@graph"][0]["id"]
+        print(f"    Injected (possibly temporary) URI {res}", file=sys.stderr)
+    elif "@graph" in data and len(data["@graph"]) == 0:
+        print("    NOTE: Graph is empty!", file=sys.stderr)
+    elif "@graph" not in data:
         data["@id"] = str(res)
-        if 'id' in data: del data['id']
-        print(f"    Injected (possibly temporary) URI {res}",file=sys.stderr)
+        if "id" in data:
+            del data["id"]
+        print(f"    Injected (possibly temporary) URI {res}", file=sys.stderr)
     else:
-        raise Exception("JSON-LD file does not describe a single resource (did you mean to use --graph instead?)")
+        raise Exception(
+            "JSON-LD file does not describe a single resource (did you mean to use --graph instead?)"
+        )
 
 
-def compute_hash(g: Graph, s: Union[URIRef,BNode], history: Optional[set] = None) -> int:
+def compute_hash(
+    g: Graph, s: Union[URIRef, BNode], history: Optional[set] = None
+) -> int:
     """Computes a content hash for all contents in a resource"""
     values = []
-    if not history: 
+    if not history:
         history = set(s)
     else:
         history.add(s)
     if isinstance(s, URIRef):
         values.append(s)
-    for s,p,o in g.triples((s,None,None)):
-        values += [p,o]
-        if isinstance(o, (URIRef,BNode)) and o not in history and (o,None,None) in g:
-            #recursion step
-            values.append( compute_hash(g, o, history) )
+    for s, p, o in g.triples((s, None, None)):
+        values += [p, o]
+        if isinstance(o, (URIRef, BNode)) and o not in history and (o, None, None) in g:
+            # recursion step
+            values.append(compute_hash(g, o, history))
     return hash(tuple(values))
-        
 
 
 def skolemize(g: Graph, baseuri: Optional[str] = None):
     """In-place skolemization, turns blank nodes into uris"""
-    #unlike Graph.skolemize, this one is in-place and edits the same graph rather than returning a copy
-    #also, if blank nodes have identical content, they receive the same stub ID based on a hash of the content
+    # unlike Graph.skolemize, this one is in-place and edits the same graph rather than returning a copy
+    # also, if blank nodes have identical content, they receive the same stub ID based on a hash of the content
 
     if baseuri:
         authority = baseuri
-        if authority[-1] != "/": authority += "/"
+        if authority[-1] != "/":
+            authority += "/"
         basepath = "stub/"
     else:
-        authority = "file://" #for compatibility with rdflib
+        authority = "file://"  # for compatibility with rdflib
         basepath = "/stub/"
 
     hashes = {}
-    for s,p,o in g.triples((None,None,None)):
+    for s, p, o in g.triples((None, None, None)):
         if isinstance(s, BNode) and s not in hashes:
-            hashes[s] = compute_hash(g,s)
+            hashes[s] = compute_hash(g, s)
 
-    for s,p,o in g.triples((None,None,None)):
+    for s, p, o in g.triples((None, None, None)):
         if isinstance(s, BNode):
-            g.remove((s,p,o))
-            #skolemize using hashes
+            g.remove((s, p, o))
+            # skolemize using hashes
             s = URIRef(authority + basepath + "H" + "%016x" % hashes[s])
-            g.add((s,p,o))
+            g.add((s, p, o)) #type: ignore
         if isinstance(o, BNode):
-            g.remove((s,p,o))
+            g.remove((s, p, o))
             if o in hashes:
-                #skolemize using hashes
+                # skolemize using hashes
                 o = URIRef(authority + basepath + "H" + "%016x" % hashes[o])
             else:
                 o = o.skolemize(authority=authority, basepath=basepath)
-            g.add((s,p,o))
+            g.add((s, p, o)) #type: ignore
+
 
-def correct_wrong_uris(g:Graph, baseuri: Optional[str]):
+def correct_wrong_uris(g: Graph, baseuri: Optional[str]):
     """Certain Literals should be URIRefs when possible, and some URIRefs are misinterpreted by rdflib and should be Literals."""
-    for s,p,o in g:
+    for s, p, o in g:
         new_obj = o
         if str(o).startswith("//"):
-            #we interpret this as a schemeless URL and will blatantly assume HTTPS (which is the most common source when fetching info, but this may be wrong)
+            # we interpret this as a schemeless URL and will blatantly assume HTTPS (which is the most common source when fetching info, but this may be wrong)
             if isinstance(o, Literal):
                 new_obj = Literal("https:" + o)
             elif isinstance(o, URIRef):
                 new_obj = URIRef("https:" + o)
         if p in PREFER_URIREF_PROPERTIES:
-            #turn Literals into URIRef for properties that prefer a URIRef
+            # turn Literals into URIRef for properties that prefer a URIRef
             if isinstance(o, Literal) and str(o).startswith("http"):
-                new_obj =  URIRef(str(o))
+                new_obj = URIRef(str(o))
 
-            #these often get misinterpreted if they're not URIs, because rdflib prepends its baseuri
+            # these often get misinterpreted if they're not URIs, because rdflib prepends its baseuri
             cwd = os.getcwd()
-            prefixes = [baseuri, cwd + "/", "file://" +cwd + "/", cwd, "file://" +cwd, "file://"]
+            prefixes = [
+                baseuri,
+                cwd + "/",
+                "file://" + cwd + "/",
+                cwd,
+                "file://" + cwd,
+                "file://",
+            ]
             for prefix in prefixes:
                 if prefix and str(o).startswith(prefix):
-                    new_obj =  Literal(str(o)[len(prefix):])
+                    new_obj = Literal(str(o)[len(prefix) :])
                     break
-        #commit the change
+        # commit the change
         if new_obj != o:
-            g.remove((s,p,o))
-            g.add((s,p,new_obj))
+            g.remove((s, p, o))
+            g.add((s, p, new_obj)) #type: ignore
 
 
-def parse_jsonld_data(g: Graph, res: Union[BNode, URIRef,None], data: dict, args: AttribDict, baseuri: Optional[str] = None) -> Union[str,None]:
-    #preprocess json
-    if '@context' not in data:
-        data['@context'] = [ x[0] for x in init_context(args) ] + [DEVIANT_CONTEXT]
-        print("    NOTE: Not a valid JSON-LD document, @context missing! Attempting to inject automatically...", file=sys.stderr)
+def parse_jsonld_data(
+    g: Graph,
+    res: Union[BNode, URIRef, None],
+    data: dict,
+    args: AttribDict,
+    baseuri: Optional[str] = None,
+) -> Union[str, None]:
+    # preprocess json
+    if "@context" not in data:
+        data["@context"] = [x[0] for x in init_context(args)] + [DEVIANT_CONTEXT]
+        print(
+            "    NOTE: Not a valid JSON-LD document, @context missing! Attempting to inject automatically...",
+            file=sys.stderr,
+        )
     else:
-        #rewrite context using the local schemas (also adds DEVIANT_CONTEXT)
-        data['@context'] = rewrite_context(data['@context'], args)
+        # rewrite context using the local schemas (also adds DEVIANT_CONTEXT)
+        data["@context"] = rewrite_context(data["@context"], args)
 
     founduri = find_main_id(data)
     if founduri:
-        print(f"    Found main resource with URI {founduri}",file=sys.stderr)
+        print(f"    Found main resource with URI {founduri}", file=sys.stderr)
     if isinstance(res, URIRef) and founduri != str(res):
-        #we're handling a single resource. Inject our own URI prior to parsing with rdflib
+        # we're handling a single resource. Inject our own URI prior to parsing with rdflib
         inject_uri(data, res)
 
-    #reserialize after edits
+    # reserialize after edits
     reserialised_data: str = json.dumps(data, indent=4)
 
-    #parse as RDF, add to main graph, and skolemize (turn blank nodes into URIs)
-    skolemize(g.parse(data=reserialised_data, format="json-ld", publicID=baseuri if baseuri else args.baseuri), args.baseuri)
+    # parse as RDF, add to main graph, and skolemize (turn blank nodes into URIs)
+    skolemize(
+        g.parse(
+            data=reserialised_data,
+            format="json-ld",
+            publicID=baseuri if baseuri else args.baseuri,
+        ),
+        args.baseuri,
+    )
     correct_wrong_uris(g, args.baseuri)
 
-    return founduri #return found uri (if any)
+    return founduri  # return found uri (if any)
```

### Comparing `CodeMetaPy-2.4.1/codemeta/parsers/nodejs.py` & `CodeMetaPy-2.5.0/codemeta/parsers/nodejs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,141 +1,221 @@
 import sys
 import json
 import os.path
 from typing import Union, IO
 from rdflib import Graph, URIRef, BNode, Literal
-from rdflib.namespace import RDF
-from codemeta.common import AttribDict, add_triple, CODEMETA, SOFTWARETYPES, add_authors, SDO, COMMON_SOURCEREPOS, SOFTWARETYPES, generate_uri
-from codemeta.crosswalk import readcrosswalk, CWKey
+from rdflib.namespace import RDF #type: ignore 
+from codemeta.common import (
+    AttribDict,
+    add_triple,
+    CODEMETA,
+    SOFTWARETYPES,
+    add_authors,
+    SDO,
+    COMMON_SOURCEREPOS,
+    SOFTWARETYPES,
+    generate_uri,
+)
+from codemeta.crosswalk import CWKey
 
 
 def parse_sourcerepo(value):
     """npm allows some shortcuts, resolve them"""
     if value.startswith("github:"):
-        value = "https://github.com/" + value[len("github:"):]
+        value = "https://github.com/" + value[len("github:") :]
     elif value.startswith("gitlab:"):
-        value = "https://gitlab.com/" + value[len("gitlab:"):]
+        value = "https://gitlab.com/" + value[len("gitlab:") :]
     elif value.startswith("bitbucket:"):
-        value = "https://bitbucket.com/" + value[len("bitbucket:"):]
-    value = value.replace("git://","https://").replace("git+ssh://","https://") #always prefer https in URLs
+        value = "https://bitbucket.com/" + value[len("bitbucket:") :]
+    value = value.replace("git://", "https://").replace(
+        "git+ssh://", "https://"
+    )  # always prefer https in URLs
     return value
 
-def parse_nodejs(g: Graph, res: Union[URIRef, BNode], file: IO , crosswalk, args: AttribDict):
+
+def parse_nodejs(
+    g: Graph, res: Union[URIRef, BNode], file: IO, crosswalk, args: AttribDict
+):
     data = json.load(file)
     iswebapp = False
     foundrepo = False
     for key, value in data.items():
         if key.lower() in crosswalk[CWKey.NODEJS]:
-            if key == 'name' and value:
-                #remove the 'scope' from the name
-                if value[0] == '@' and value.find('/') != -1:
-                    value = value.split('/')[1]
+            if key == "name" and value:
+                # remove the 'scope' from the name
+                if value[0] == "@" and value.find("/") != -1:
+                    value = value.split("/")[1]
                 add_triple(g, res, key, value, args)
-            elif key == 'bugs':
-                if isinstance(value,dict) and 'url' in value:
-                    g.add((res, CODEMETA.issueTracker, Literal(value['url'])))
-                    if 'email' in value:
-                        g.add((res, SDO.email, Literal(value['email'])))
+            elif key == "bugs":
+                if isinstance(value, dict) and "url" in value:
+                    g.add((res, CODEMETA.issueTracker, Literal(value["url"])))
+                    if "email" in value:
+                        g.add((res, SDO.email, Literal(value["email"])))
                 elif isinstance(value, str):
                     g.add((res, CODEMETA.issueTracker, Literal(value)))
-            elif key == 'license':
-                if isinstance(value, dict) and 'type' in value:
-                    add_triple(g, res, "license", value['type'], args)
-                elif isinstance(value, (list,tuple)):
+            elif key == "license":
+                if isinstance(value, dict) and "type" in value:
+                    add_triple(g, res, "license", value["type"], args)
+                elif isinstance(value, (list, tuple)):
                     for item in value:
-                        if isinstance(item, dict) and 'type' in item:
-                            add_triple(g, res, "license", item['type'], args)
+                        if isinstance(item, dict) and "type" in item:
+                            add_triple(g, res, "license", item["type"], args)
                         elif isinstance(item, str):
                             add_triple(g, res, "license", item, args)
                 elif isinstance(value, str):
                     add_triple(g, res, "license", value, args)
-            elif key == 'keywords':
-                if isinstance(value, (list,tuple)):
+            elif key == "keywords":
+                if isinstance(value, (list, tuple)):
                     for keyword in value:
                         add_triple(g, res, "keywords", keyword, args)
                 else:
-                    print("WARNING: keywords in package.json should be a list",file=sys.stderr)
-            elif key == 'private' and value:
-                    print("WARNING: private=true was set on package.json! This package is marked not to be published!",file=sys.stderr)
-            elif key == 'repository':
+                    print(
+                        "WARNING: keywords in package.json should be a list",
+                        file=sys.stderr,
+                    )
+            elif key == "private" and value:
+                print(
+                    "WARNING: private=true was set on package.json! This package is marked not to be published!",
+                    file=sys.stderr,
+                )
+            elif key == "repository":
                 if isinstance(value, str):
                     value = parse_sourcerepo(value)
                     add_triple(g, res, "codeRepository", value, args)
                     foundrepo = True
-                elif isinstance(value, dict) and 'url' in value:
-                    value = parse_sourcerepo(value['url'])
+                elif isinstance(value, dict) and "url" in value:
+                    value = parse_sourcerepo(value["url"])
                     add_triple(g, res, "codeRepository", value, args)
                     foundrepo = True
-            elif key == 'homepage':
+            elif key == "homepage":
                 for sourcerepo in COMMON_SOURCEREPOS:
                     if value.startswith(sourcerepo) and not foundrepo:
-                        #catch if we're describing the source code repo instead
+                        # catch if we're describing the source code repo instead
                         add_triple(g, res, "codeRepository", value, args)
                         break
                 add_triple(g, res, "url", value, args)
-            elif key == 'author':
-                #npm prescribes that author is only one person
-                if isinstance(value, dict) and 'name' in value:
-                    authors = add_authors(g, res, value['name'], single_author=True, mail=value.get("email"), baseuri=args.baseuri)
-                    if authors and 'url' in value:
-                        g.add((authors[0], SDO.url, Literal(value['url'])))
+            elif key == "author":
+                # npm prescribes that author is only one person
+                if isinstance(value, dict) and "name" in value:
+                    authors = add_authors(
+                        g,
+                        res,
+                        value["name"],
+                        single_author=True,
+                        mail=value.get("email"),
+                        baseuri=args.baseuri,
+                    )
+                    if authors and "url" in value:
+                        g.add((authors[0], SDO.url, Literal(value["url"])))
                 elif isinstance(value, str):
-                    #npm allows strings like "Barney Rubble <b@rubble.com> (http://barnyrubble.tumblr.com/)"
-                    #our add_authors function can handle that directly
+                    # npm allows strings like "Barney Rubble <b@rubble.com> (http://barnyrubble.tumblr.com/)"
+                    # our add_authors function can handle that directly
                     add_authors(g, res, value, single_author=True, baseuri=args.baseuri)
-            elif key == 'contributors':
-                if isinstance(value, dict) and 'name' in value:
-                    authors = add_authors(g, res, value['name'], property=SDO.contributor, single_author=True, mail=value.get("email"), baseuri=args.baseuri)
+            elif key == "contributors":
+                if isinstance(value, dict) and "name" in value:
+                    authors = add_authors(
+                        g,
+                        res,
+                        value["name"],
+                        property=SDO.contributor,
+                        single_author=True,
+                        mail=value.get("email"),
+                        baseuri=args.baseuri,
+                    )
                 elif isinstance(value, str):
-                    add_authors(g, res, value, property=SDO.contributor, baseuri=args.baseuri)
-                elif isinstance(value, (list,tuple)):
+                    add_authors(
+                        g, res, value, property=SDO.contributor, baseuri=args.baseuri
+                    )
+                elif isinstance(value, (list, tuple)):
                     for value in value:
-                        authors = add_authors(g, res, value['name'], property=SDO.contributor, single_author=True, mail=value.get("email"), baseuri=args.baseuri)
-            elif key in ('dependencies','devDependencies'):
+                        authors = add_authors(
+                            g,
+                            res,
+                            value["name"],
+                            property=SDO.contributor,
+                            single_author=True,
+                            mail=value.get("email"),
+                            baseuri=args.baseuri,
+                        )
+            elif key in ("dependencies", "devDependencies"):
                 if isinstance(value, dict):
                     for key, versioninfo in value.items():
-                        depres = URIRef(generate_uri(key+versioninfo, baseuri=args.baseuri,prefix="dependency"))
+                        depres = URIRef(
+                            generate_uri(
+                                key + versioninfo,
+                                baseuri=args.baseuri,
+                                prefix="dependency",
+                            )
+                        )
                         g.add((depres, RDF.type, SDO.SoftwareApplication))
                         g.add((depres, SDO.name, Literal(key)))
                         g.add((depres, SDO.identifier, Literal(key)))
                         g.add((depres, SDO.version, Literal(versioninfo)))
-                        g.add((res,  CODEMETA.softwareRequirements, depres))
-                    #detect some common web application frameworks or other
-                    #dependencies that indicate this is a web-app
-                    iswebapp = iswebapp or 'react' in value or 'vue' in value or 'sitemap' in value or  'gatsby' in value
-            elif key in ('bundledDependencies','peerDependencies'):
-                pass #ignore
-            elif key == 'bin':
-                #note: assuming CommandLineApplication may be a bit presumptuous here
-                if isinstance(value, dict) and 'name' in value and args.with_stypes:
+                        g.add((res, CODEMETA.softwareRequirements, depres))
+                    # detect some common web application frameworks or other
+                    # dependencies that indicate this is a web-app
+                    iswebapp = (
+                        iswebapp
+                        or "react" in value
+                        or "vue" in value
+                        or "sitemap" in value
+                        or "gatsby" in value
+                    )
+            elif key in ("bundledDependencies", "peerDependencies"):
+                pass  # ignore
+            elif key == "bin":
+                # note: assuming CommandLineApplication may be a bit presumptuous here
+                if isinstance(value, dict) and "name" in value and args.with_stypes:
                     for progname, execname in value.items():
-                        sapp = URIRef(generate_uri(key, baseuri=args.baseuri,prefix="commandlineapplication"))
+                        sapp = URIRef(
+                            generate_uri(
+                                key,
+                                baseuri=args.baseuri,
+                                prefix="commandlineapplication",
+                            )
+                        )
                         g.add((sapp, RDF.type, SOFTWARETYPES.CommandLineApplication))
                         g.add((sapp, SDO.name, progname))
-                        g.add((sapp, SOFTWARETYPES.executableName, os.path.basename(execname)))
+                        g.add(
+                            (
+                                sapp,
+                                SOFTWARETYPES.executableName,
+                                os.path.basename(execname),
+                            )
+                        )
                         g.add((res, SDO.targetProduct, sapp))
                 elif isinstance(value, str) and args.with_stypes:
-                    sapp = URIRef(generate_uri(data['name'], baseuri=args.baseuri,prefix="commandlineapplication"))
+                    sapp = URIRef(
+                        generate_uri(
+                            data["name"],
+                            baseuri=args.baseuri,
+                            prefix="commandlineapplication",
+                        )
+                    )
                     g.add((sapp, RDF.type, SOFTWARETYPES.CommandLineApplication))
-                    g.add((sapp, SDO.name, data['name'])) #from parent
+                    g.add((sapp, SDO.name, data["name"]))  # from parent
                     g.add((sapp, SOFTWARETYPES.executableName, os.path.basename(value)))
                     g.add((res, SDO.targetProduct, sapp))
-            elif key == 'engines':
+            elif key == "engines":
                 if isinstance(value, dict):
                     for key, versioninfo in value.items():
-                        g.add((res, SDO.runtimePlatform, Literal(key + " " + versioninfo)))
+                        g.add(
+                            (res, SDO.runtimePlatform, Literal(key + " " + versioninfo))
+                        )
             else:
                 key = crosswalk[CWKey.NODEJS][key.lower()]
                 add_triple(g, res, key, value, args)
 
-    if 'devDependencies' in data and "typescript" in data['devDependencies']:
+    if "devDependencies" in data and "typescript" in data["devDependencies"]:
         g.add((res, SDO.programmingLanguage, Literal("Typescript")))
     else:
         g.add((res, SDO.programmingLanguage, Literal("Javascript")))
 
-    if args.with_stypes and 'browser' in data or 'browserslist' in data or iswebapp:
-        #assume this is a web-application
-        sapp = URIRef(generate_uri(data['name'], baseuri=args.baseuri,prefix="webapplication"))
+    if args.with_stypes and "browser" in data or "browserslist" in data or iswebapp:
+        # assume this is a web-application
+        sapp = URIRef(
+            generate_uri(data["name"], baseuri=args.baseuri, prefix="webapplication")
+        )
         g.add((sapp, RDF.type, SDO.WebApplication))
-        g.add((sapp, SDO.name, Literal(data['name']))) #from parent
-        g.add((sapp, SDO.version, Literal(data['version']))) #from parent
+        g.add((sapp, SDO.name, Literal(data["name"])))  # from parent
+        g.add((sapp, SDO.version, Literal(data["version"])))  # from parent
         g.add((res, SDO.targetProduct, sapp))
```

### Comparing `CodeMetaPy-2.4.1/codemeta/parsers/rust.py` & `CodeMetaPy-2.5.0/codemeta/parsers/rust.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,84 @@
 import sys
 import tomlkit
 from rdflib import Graph, URIRef, BNode, Literal
-from rdflib.namespace import RDF
+from rdflib.namespace import RDF #type: ignore
 from typing import Union, IO
-from codemeta.common import AttribDict, add_triple, CODEMETA, SOFTWARETYPES, add_authors, SDO, COMMON_SOURCEREPOS, SOFTWARETYPES, generate_uri
+from codemeta.common import (
+    AttribDict,
+    add_triple,
+    CODEMETA,
+    add_authors,
+    SDO,
+    COMMON_SOURCEREPOS,
+    SOFTWARETYPES,
+    generate_uri,
+)
 
 
-def parse_rust(g: Graph, res: Union[URIRef, BNode], file: IO ,  args: AttribDict):
+def parse_rust(g: Graph, res: Union[URIRef, BNode], file: IO, args: AttribDict):
     data = tomlkit.parse(file.read())
-    if 'package' in data:
-        for key, value in data['package'].items():
-            if key == 'repository':
-                add_triple(g, res, 'codeRepository', value, args)
-            elif key == 'authors':
+    if "package" in data:
+        for key, value in data["package"].items(): #type: ignore
+            if key == "repository":
+                add_triple(g, res, "codeRepository", value, args)
+            elif key == "authors":
                 if isinstance(value, str):
-                    add_authors(g, res, value, single_author=False, baseuri=args.baseuri)
+                    add_authors(
+                        g, res, value, single_author=False, baseuri=args.baseuri
+                    )
                 elif isinstance(value, list):
                     for value in value:
-                        add_authors(g, res, value, single_author=True, baseuri=args.baseuri)
-            elif key == 'keywords':
-                if isinstance(value, (list,tuple)):
+                        add_authors(
+                            g, res, value, single_author=True, baseuri=args.baseuri
+                        )
+            elif key == "keywords":
+                if isinstance(value, (list, tuple)):
                     for keyword in value:
                         add_triple(g, res, "keywords", keyword, args)
                 else:
-                    print("WARNING: keywords in Cargo.toml should be a list",file=sys.stderr)
-            elif key == 'homepage':
+                    print(
+                        "WARNING: keywords in Cargo.toml should be a list",
+                        file=sys.stderr,
+                    )
+            elif key == "homepage":
                 for sourcerepo in COMMON_SOURCEREPOS:
-                    if value.startswith(sourcerepo) and 'repository' not in data['package']:
-                        #catch if we're describing the source code repo instead
+                    if (
+                        value.startswith(sourcerepo)
+                        and "repository" not in data["package"] #type: ignore
+                    ):
+                        # catch if we're describing the source code repo instead
                         add_triple(g, res, "codeRepository", value, args)
                         break
                 add_triple(g, res, "url", value, args)
-            elif key == 'documentation':
+            elif key == "documentation":
                 add_triple(g, res, "softwareHelp", value, args)
-            elif key == 'categories':
+            elif key == "categories":
                 add_triple(g, res, "applicationCategory", value, args)
-            elif key in ('name','description','readme','license','version'):
+            elif key in ("name", "description", "readme", "license", "version"):
                 add_triple(g, res, key, value, args)
-    if 'dependencies' in data:
-        for key, value in data['dependencies'].items():
-            if isinstance(value, dict) and 'version' in value:
-                add_dependency(g, res, key, value['version'], args)
+    if "dependencies" in data:
+        for key, value in data["dependencies"].items(): #type: ignore
+            if isinstance(value, dict) and "version" in value:
+                add_dependency(g, res, key, value["version"], args)
             elif isinstance(value, str):
                 add_dependency(g, res, key, value, args)
-            
+
     g.add((res, SDO.programmingLanguage, Literal("Rust")))
 
-#pylint: disable=W0621
-def add_dependency(g: Graph, res: Union[URIRef, BNode], name: str, version: str, args: AttribDict):
+
+# pylint: disable=W0621
+def add_dependency(
+    g: Graph, res: Union[URIRef, BNode], name: str, version: str, args: AttribDict
+):
     if version and version[0].isalnum():
         version_id = "-" + version
     else:
         version_id = version
-    depres = URIRef(generate_uri(name+version_id.replace(' ',''),args.baseuri,"dependency")) #version number is deliberately in ID here!
+    depres = URIRef(
+        generate_uri(name + version_id.replace(" ", ""), args.baseuri, "dependency")
+    )  # version number is deliberately in ID here!
     g.add((depres, RDF.type, SDO.SoftwareApplication))
     g.add((depres, SDO.identifier, Literal(name)))
     g.add((depres, SDO.name, Literal(name)))
     g.add((depres, SDO.version, Literal(version)))
     g.add((res, CODEMETA.softwareRequirements, depres))
```

### Comparing `CodeMetaPy-2.4.1/codemeta/parsers/web.py` & `CodeMetaPy-2.5.0/codemeta/parsers/web.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,207 +1,307 @@
 import sys
 import json
 import os.path
 from typing import Union, Iterator
 import requests
 import yaml
 from rdflib import Graph, URIRef, BNode, Literal
-from rdflib.namespace import RDF
-from codemeta.common import AttribDict, SDO, generate_uri, add_authors, get_last_component
+from rdflib.namespace import RDF #type: ignore
+from codemeta.common import (
+    AttribDict,
+    SDO,
+    generate_uri,
+    add_authors,
+    get_last_component,
+)
 from codemeta.parsers.jsonld import parse_jsonld_data
 from bs4 import BeautifulSoup
 
 
 class MiddlewareObstructionException(Exception):
     pass
 
+
 def detect_type(data):
     if "@context" in data and "@type" in data:
-        value = data['@context']
-        if isinstance(value,str):
+        value = data["@context"]
+        if isinstance(value, str):
             if value.find("schema.org") != -1 or value.find("codemeta") != -1:
-                return  "schema"
-        elif isinstance(value,list):
-            if any( x.find("schema.org") != -1 or x.find("codemeta") != -1 for x in value ):
                 return "schema"
-    elif isinstance(data, dict) and 'openapi' in data:
+        elif isinstance(value, list):
+            if any(
+                x.find("schema.org") != -1 or x.find("codemeta") != -1 for x in value
+            ):
+                return "schema"
+    elif isinstance(data, dict) and "openapi" in data:
         return "openapi"
     return None
 
+
 def get_meta(soup, *keys, default=""):
     for key in keys:
-        for value in  soup.find("head").find_all("meta", itemprop=key):
-            if value.get('content'):
-                return value.get('content')
-        for value in  soup.find("head").find_all("meta", property=key):
-            if value.get('content'):
-                return value.get('content')
-        for value in soup.find("head").find_all("meta", {"name": key }):
-            if value.get('content'):
-                return value.get('content')
+        for value in soup.find("head").find_all("meta", itemprop=key):
+            if value.get("content"):
+                return value.get("content")
+        for value in soup.find("head").find_all("meta", property=key):
+            if value.get("content"):
+                return value.get("content")
+        for value in soup.find("head").find_all("meta", {"name": key}):
+            if value.get("content"):
+                return value.get("content")
     return default
 
 
-def get_soup(soup,elementname, attribname=None):
+def get_soup(soup, elementname, attribname=None):
     for e in soup.find_all(elementname):
         if attribname:
             v = e.get(attribname)
             return v
         elif e.text:
             return e.text
     return ""
 
+
 def parse_clam(soup):
     return {
-        "name": get_soup(soup,"clam","name"),
+        "name": get_soup(soup, "clam", "name"),
         "url": get_soup(soup, "clam", "baseurl"),
         "description": get_soup(soup, "description"),
         "author": get_soup(soup, "author"),
         "provider": get_soup(soup, "affiliation"),
         "email": get_soup(soup, "email"),
         "version": get_soup(soup, "version"),
-        "license": get_soup(soup, "license")
+        "license": get_soup(soup, "license"),
     }
 
+
 def detect_sso_middleware(r: requests.Response):
-    return r.history and 'location' in r.history[-1].headers and r.history[-1].headers['location'].lower().find("shibboleth") != -1
+    return (
+        r.history
+        and "location" in r.history[-1].headers
+        and r.history[-1].headers["location"].lower().find("shibboleth") != -1
+    )
+
 
 def add_missing_url_scheme(data, original_url: str):
     """Add URL scheme when missing"""
     if isinstance(data, dict):
         return {k: add_missing_url_scheme(v, original_url) for k, v in data.items()}
-    elif isinstance(data, (list,tuple)):
-        return [ add_missing_url_scheme(v, original_url) for v in data ]
+    elif isinstance(data, (list, tuple)):
+        return [add_missing_url_scheme(v, original_url) for v in data]
     elif isinstance(data, str) and data.startswith("//"):
         return original_url.split("/")[0] + data
     return data
 
-def parse_web(g: Graph, res: Union[URIRef, BNode], url, args: AttribDict) -> Iterator[Union[URIRef,BNode,None]]:
-    r = requests.get(url, headers={ "Accept": "application/json+ld;q=1.0,application/json;q=0.9,application/x-yaml;q=0.8,application/xml;q=0.7;text/html;q=0.6;text/plain;q=0.1" })
+
+def parse_web(
+    g: Graph, res: Union[URIRef, BNode], url, args: AttribDict
+) -> Iterator[Union[URIRef, BNode, None]]:
+    r = requests.get(
+        url,
+        headers={
+            "Accept": "application/json+ld;q=1.0,application/json;q=0.9,application/x-yaml;q=0.8,application/xml;q=0.7;text/html;q=0.6;text/plain;q=0.1"
+        },
+    )
     r.raise_for_status()
-    contenttype = r.headers.get('content-type',"").split(';')[0].strip()
-    print(f"    Service replied with content-type {contenttype}",file=sys.stderr)
+    contenttype = r.headers.get("content-type", "").split(";")[0].strip()
+    print(f"    Service replied with content-type {contenttype}", file=sys.stderr)
     datatype = None
     data = None
 
-
-    if contenttype in ("application/json", "application/ld+json") or url.endswith(".json") or url.endswith(".jsonld"):
-        print("    Parsing json...",file=sys.stderr)
+    if (
+        contenttype in ("application/json", "application/ld+json")
+        or url.endswith(".json")
+        or url.endswith(".jsonld")
+    ):
+        print("    Parsing json...", file=sys.stderr)
         data = json.loads(r.text)
-    elif contenttype in ("application/x-yaml", "text/yaml") or url.endswith(".yml") or url.endswith(".yaml"):
-        print("    Parsing yaml...",file=sys.stderr)
-        #may be OpenAPI
-        with open(r.text,'r', encoding="utf-8") as f:
+    elif (
+        contenttype in ("application/x-yaml", "text/yaml")
+        or url.endswith(".yml")
+        or url.endswith(".yaml")
+    ):
+        print("    Parsing yaml...", file=sys.stderr)
+        # may be OpenAPI
+        with open(r.text, "r", encoding="utf-8") as f:
             data = yaml.load(f, yaml.Loader)
     elif contenttype == "text/html":
         if detect_sso_middleware(r):
-            #we've been redirected to a login page directly
-            #so we can't extract any useful metadata
-            #we add a dummy entry:
-            raise MiddlewareObstructionException(f"Unable to extract metadata from {url} because it immediately redirects to an external (SSO) login page rather than a proper landing page")
-        #normal behaviour
-        print("    Parsing html...",file=sys.stderr)
-        soup = BeautifulSoup(r.text, 'html.parser')
-        scriptblock = soup.find("script", {"type":"application/ld+json"})
+            # we've been redirected to a login page directly
+            # so we can't extract any useful metadata
+            # we add a dummy entry:
+            raise MiddlewareObstructionException(
+                f"Unable to extract metadata from {url} because it immediately redirects to an external (SSO) login page rather than a proper landing page"
+            )
+        # normal behaviour
+        print("    Parsing html...", file=sys.stderr)
+        soup = BeautifulSoup(r.text, "html.parser")
+        scriptblock = soup.find("script", {"type": "application/ld+json"})
         if scriptblock:
-            #Does the site provide proper JSON-LD metadata itself?
-            print("    Found a json-ld script block",file=sys.stderr)
-            data = json.loads("".join(scriptblock.contents))            
+            # Does the site provide proper JSON-LD metadata itself?
+            print("    Found a json-ld script block", file=sys.stderr)
+            data = json.loads("".join(scriptblock.contents)) #type: ignore
         else:
-            print("    Parsing site metadata",file=sys.stderr)
-            name = get_meta(soup, "schema:name", "og:site_name", "og:title", "twitter:title")
+            print("    Parsing site metadata", file=sys.stderr)
+            name = get_meta(
+                soup, "schema:name", "og:site_name", "og:title", "twitter:title"
+            )
             if not name and soup.title:
                 name = soup.title.text
                 name = name.strip()
+            if not name:
+                for e in soup.find("h1"): #type: ignore
+                    name = e.text
+                    name = name.strip()
 
             if args.with_stypes:
-                targetres = URIRef(generate_uri(name, baseuri=args.baseuri,prefix="webapplication"))
+                targetres = URIRef(
+                    generate_uri(name, baseuri=args.baseuri, prefix="webapplication")
+                )
             else:
                 targetres = res
             if name:
                 g.add((targetres, SDO.name, Literal(name)))
 
             targetrestype = SDO.WebApplication
             for e in (soup.find("head"), soup.find("html")):
-                itemtype = e.get("itemtype")
-                if itemtype in ("https://schema.org/WebApplication", "http://schema.org/WebApplication"):
+                itemtype = e.get("itemtype") #type: ignore
+                if itemtype in (
+                    "https://schema.org/WebApplication",
+                    "http://schema.org/WebApplication",
+                ):
                     targetrestype = SDO.WebApplication
-                elif itemtype in ("https://schema.org/WebPage", "http://schema.org/WebPage"):
+                elif itemtype in (
+                    "https://schema.org/WebPage",
+                    "http://schema.org/WebPage",
+                ):
                     targetrestype = SDO.WebPage
-                elif itemtype in ("https://schema.org/WebSite", "http://schema.org/WebSite"):
+                elif itemtype in (
+                    "https://schema.org/WebSite",
+                    "http://schema.org/WebSite",
+                ):
                     targetrestype = SDO.WebSite
-                elif itemtype in ("https://schema.org/WebAPI", "http://schema.org/WebAPI"):
+                elif itemtype in (
+                    "https://schema.org/WebAPI",
+                    "http://schema.org/WebAPI",
+                ):
                     targetrestype = SDO.WebAPI
                 if itemtype:
                     break
 
             g.add((targetres, RDF.type, targetrestype))
-            g.add((targetres, SDO.url, Literal(get_meta(soup, "og:url", "url", default=url))))
-
-            v = get_meta(soup, "schema:description", "og:description", "twitter:description", "description")
-            if v: g.add((targetres, SDO.description, Literal(v)))
+            g.add(
+                (
+                    targetres,
+                    SDO.url,
+                    Literal(get_meta(soup, "og:url", "url", default=url)),
+                )
+            )
+
+            v = get_meta(
+                soup,
+                "schema:description",
+                "og:description",
+                "twitter:description",
+                "description",
+            )
+            if v:
+                g.add((targetres, SDO.description, Literal(v)))
 
             v = get_meta(soup, "schema:url")
-            if v: g.add((targetres, SDO.url, Literal(add_missing_url_scheme(v,url))))
+            if v:
+                g.add((targetres, SDO.url, Literal(add_missing_url_scheme(v, url))))
 
-            v = get_meta(soup, "schema:thumbnailUrl", "og:image", "twitter:image", "thumbnail")
-            if v: g.add((targetres, SDO.thumbnailUrl, Literal(add_missing_url_scheme(v,url))))
+            v = get_meta(
+                soup, "schema:thumbnailUrl", "og:image", "twitter:image", "thumbnail"
+            )
+            if v:
+                g.add(
+                    (
+                        targetres,
+                        SDO.thumbnailUrl,
+                        Literal(add_missing_url_scheme(v, url)),
+                    )
+                )
 
             v = get_meta(soup, "schema:author", "author")
-            if v: add_authors(g, targetres, v, baseuri=args.baseuri)
+            if v:
+                add_authors(g, targetres, v, baseuri=args.baseuri)
 
             v = get_meta(soup, "schema:keywords", "keywords")
             if v:
                 for item in v.split(","):
                     item = item.strip()
-                    if item: g.add((targetres, SDO.keywords, Literal(item)))
+                    if item:
+                        g.add((targetres, SDO.keywords, Literal(item)))
 
             yield targetres
             data = None
     elif contenttype in ("application/xml", "text/xml"):
-        soup = BeautifulSoup(r.text, 'xml')
+        soup = BeautifulSoup(r.text, "xml")
         if soup.find("clam") and args.with_stypes:
-            print("    Parsing CLAM metadata",file=sys.stderr)
+            print("    Parsing CLAM metadata", file=sys.stderr)
             clamdata = parse_clam(soup)
             for restype in (SDO.WebApplication, SDO.WebAPI):
-                assert clamdata['name']
-                targetres = URIRef(generate_uri(clamdata['name'], baseuri=args.baseuri,prefix=get_last_component(str(restype).lower())))
+                assert clamdata["name"]
+                targetres = URIRef(
+                    generate_uri(
+                        clamdata["name"],
+                        baseuri=args.baseuri,
+                        prefix=get_last_component(str(restype).lower()),
+                    )
+                )
                 g.add((targetres, RDF.type, restype))
-                if clamdata['name']:
-                    g.add((targetres, SDO.name, Literal(clamdata['name'])))
-                if clamdata['description']:
-                    g.add((targetres, SDO.description, Literal(clamdata['description'])))
-                if clamdata['author']:
-                    add_authors(g, targetres, clamdata['author'], baseuri=args.baseuri)
-                if clamdata['email']:
-                    g.add((targetres, SDO.email, Literal(clamdata['email'])))
-                if clamdata['url']:
-                    g.add((targetres, SDO.url, Literal(clamdata['url'])))
+                if clamdata["name"]:
+                    g.add((targetres, SDO.name, Literal(clamdata["name"])))
+                if clamdata["description"]:
+                    g.add(
+                        (targetres, SDO.description, Literal(clamdata["description"]))
+                    )
+                if clamdata["author"]:
+                    add_authors(g, targetres, clamdata["author"], baseuri=args.baseuri)
+                if clamdata["email"]:
+                    g.add((targetres, SDO.email, Literal(clamdata["email"])))
+                if clamdata["url"]:
+                    g.add((targetres, SDO.url, Literal(clamdata["url"])))
                     if restype == SDO.WebAPI:
-                        g.add((targetres, SDO.documentation, Literal(os.path.join(clamdata['url'],"info")))) #Proposed in schemaorg/schemaorg#1423
+                        g.add(
+                            (
+                                targetres,
+                                SDO.documentation,
+                                Literal(os.path.join(clamdata["url"], "info")),
+                            )
+                        )  # Proposed in schemaorg/schemaorg#1423
                 else:
                     g.add((targetres, SDO.url, Literal(url)))
-                if clamdata['provider']:
-                    g.add((targetres, SDO.provider, Literal(clamdata['provider'])))
-                if clamdata['version']:
-                    g.add((targetres, SDO.version, Literal(clamdata['version'])))
+                if clamdata["provider"]:
+                    g.add((targetres, SDO.provider, Literal(clamdata["provider"])))
+                if clamdata["version"]:
+                    g.add((targetres, SDO.version, Literal(clamdata["version"])))
                 yield targetres
             data = None
         else:
-            print("    Remote returned unrecognized XML",file=sys.stderr)
+            print("    Remote returned unrecognized XML", file=sys.stderr)
     else:
-        print(f"    Remote returned unknown contenttype: {contenttype}",file=sys.stderr)
+        print(
+            f"    Remote returned unknown contenttype: {contenttype}", file=sys.stderr
+        )
 
     if data:
         datatype = detect_type(data)
-        if datatype == 'schema':
+        if datatype == "schema":
             if args.with_stypes:
-                targetres = URIRef(generate_uri(baseuri=args.baseuri,prefix="webapplication"))
+                targetres = URIRef(
+                    generate_uri(baseuri=args.baseuri, prefix="webapplication")
+                )
             else:
                 targetres = res
             data = add_missing_url_scheme(data, url)
-            parse_jsonld_data(g, targetres, data, args)
+            parse_jsonld_data(g, targetres, data, args) #type: ignore
             yield targetres
-        elif datatype == 'openapi':
-            raise NotImplementedError #TODO
+        elif datatype == "openapi":
+            raise NotImplementedError  # TODO
         else:
-            print(f"    Unable to detect data type of data returned by {url}",file=sys.stderr)
+            print(
+                f"    Unable to detect data type of data returned by {url}",
+                file=sys.stderr,
+            )
```

### Comparing `CodeMetaPy-2.4.1/codemeta/schema/CONTRIBUTING.md` & `CodeMetaPy-2.5.0/codemeta/schema/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `CodeMetaPy-2.4.1/codemeta/schema/CONTRIBUTORS.MD` & `CodeMetaPy-2.5.0/codemeta/schema/CONTRIBUTORS.MD`

 * *Files identical despite different names*

### Comparing `CodeMetaPy-2.4.1/codemeta/schema/LICENSE` & `CodeMetaPy-2.5.0/codemeta/schema/LICENSE`

 * *Files identical despite different names*

### Comparing `CodeMetaPy-2.4.1/codemeta/schema/README.md` & `CodeMetaPy-2.5.0/codemeta/schema/README.md`

 * *Files identical despite different names*

### Comparing `CodeMetaPy-2.4.1/codemeta/schema/codemeta.json` & `CodeMetaPy-2.5.0/codemeta/schema/codemeta.json`

 * *Files identical despite different names*

### Comparing `CodeMetaPy-2.4.1/codemeta/schema/codemeta.jsonld` & `CodeMetaPy-2.5.0/codemeta/schema/codemeta.jsonld`

 * *Files identical despite different names*

### Comparing `CodeMetaPy-2.4.1/codemeta/schema/crosswalk.csv` & `CodeMetaPy-2.5.0/codemeta/schema/crosswalk.csv`

 * *Files identical despite different names*

### Comparing `CodeMetaPy-2.4.1/codemeta/schema/properties_description.csv` & `CodeMetaPy-2.5.0/codemeta/schema/properties_description.csv`

 * *Files identical despite different names*

### Comparing `CodeMetaPy-2.4.1/codemeta/serializers/jsonld.py` & `CodeMetaPy-2.5.0/codemeta/serializers/jsonld.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,219 +1,329 @@
 import sys
 import json
 import os.path
 from typing import Union, IO, Sequence, Optional
 from rdflib import Graph, URIRef, BNode, Literal
-from rdflib.namespace import SKOS
+from rdflib.namespace import SKOS #type: ignore
 from copy import copy
-from codemeta.common import AttribDict, license_to_spdx, SDO, CODEMETA_SOURCE, CODEMETA_LOCAL_SOURCE, SCHEMA_SOURCE, SCHEMA_LOCAL_SOURCE, STYPE_SOURCE, STYPE_LOCAL_SOURCE, IODATA_SOURCE, IODATA_LOCAL_SOURCE, init_context, REPOSTATUS_LOCAL_SOURCE, REPOSTATUS_SOURCE, get_subgraph, PREFER_URIREF_PROPERTIES, TMPDIR, DEVIANT_CONTEXT, ORDEREDLIST_PROPERTIES
+from codemeta.common import (
+    AttribDict,
+    CODEMETA_SOURCE,
+    CODEMETA_LOCAL_SOURCE,
+    SCHEMA_SOURCE,
+    SCHEMA_LOCAL_SOURCE,
+    STYPE_SOURCE,
+    STYPE_LOCAL_SOURCE,
+    IODATA_SOURCE,
+    IODATA_LOCAL_SOURCE,
+    init_context,
+    REPOSTATUS_LOCAL_SOURCE,
+    REPOSTATUS_SOURCE,
+    PREFER_URIREF_PROPERTIES,
+    TMPDIR,
+    DEVIANT_CONTEXT,
+    ORDEREDLIST_PROPERTIES,
+)
 
 ORDEREDLIST_PROPERTIES_NAMES = list(os.path.basename(x) for x in ORDEREDLIST_PROPERTIES)
-NSPREFIXES = ('schema:','codemeta:','rdf:','rdfs:','skos:','trl:','dct:','dc:','dc11:','xsd:','stype:','softwaretypes:','iodata:','softwareiodata:','owl:','og:','sh:','nwo:','repostatus:','clariah:')
-#do not embed items under theme properties
-NOEMBED = ("skos:broader","skos:narrower","skos:hasTopConcept","skos:inScheme", SKOS.broader, SKOS.narrower, SKOS.hasTopConcept, SKOS.inScheme)
+NSPREFIXES = (
+    "schema:",
+    "codemeta:",
+    "rdf:",
+    "rdfs:",
+    "skos:",
+    "trl:",
+    "dct:",
+    "dc:",
+    "dc11:",
+    "xsd:",
+    "stype:",
+    "softwaretypes:",
+    "iodata:",
+    "softwareiodata:",
+    "owl:",
+    "og:",
+    "sh:",
+    "nwo:",
+    "repostatus:",
+    "clariah:",
+)
+# do not embed items under theme properties
+NOEMBED = (
+    "skos:broader",
+    "skos:narrower",
+    "skos:hasTopConcept",
+    "skos:inScheme",
+    SKOS.broader,
+    SKOS.narrower,
+    SKOS.hasTopConcept,
+    SKOS.inScheme,
+)
+
 
 def remove_blank_ids(data):
     """Recursively remove all blank node IDs"""
     if isinstance(data, dict):
-        if '@id' in data and data['@id'].startswith("_:"):
-            del data['@id']
-        if 'id' in data and data['id'].startswith("_:"):
-            del data['id']
-        return { k: remove_blank_ids(v) for k,v in data.items() }
+        if "@id" in data and data["@id"].startswith("_:"):
+            del data["@id"]
+        if "id" in data and data["id"].startswith("_:"):
+            del data["id"]
+        return {k: remove_blank_ids(v) for k, v in data.items()}
     elif isinstance(data, (list, tuple)):
-        return [ remove_blank_ids(v) for v in data ]
+        return [remove_blank_ids(v) for v in data]
     else:
         return data
 
+
 def alt_sort_key(data) -> str:
     if isinstance(data, dict):
-        if 'name' in data:
-            return data['name']
-        if '@id' in data:
-            return data['@id']
-        if 'identifier' in data:
-            return data['identifier']
+        if "name" in data:
+            return data["name"]
+        if "@id" in data:
+            return data["@id"]
+        if "identifier" in data:
+            return data["identifier"]
     elif isinstance(data, str):
         return data
-    return "~" #just a high alphanumeric character so it ends up after normal (ascii) stuff
+    return "~"  # just a high alphanumeric character so it ends up after normal (ascii) stuff
 
 
-def sort_by_position(data: Union[list,dict,tuple,str]) -> Union[list,dict,str]:
+def sort_by_position(data: Union[list, dict, tuple, str]) -> Union[list, dict, str]:
     """If list items have a position (schema:position) index, make sure to use it for sorting. If not, sort alphabetically of name of id"""
     if isinstance(data, (list, tuple)):
-        if any( isinstance(x, dict) and 'position' in x for x in data ):
+        if any(isinstance(x, dict) and "position" in x for x in data):
             try:
-                return list(sorted( ( sort_by_position(x) for x in data) , key=lambda x: x['position'] if isinstance(x, dict) and 'position' in x else 99999999 ) )
-            except TypeError: #in rare cases this might fail because of some inconsistency, return unsorted then
-                return [ sort_by_position(x) for x in data ]
+                return list(
+                    sorted(
+                        (sort_by_position(x) for x in data),
+                        key=lambda x: x["position"]
+                        if isinstance(x, dict) and "position" in x
+                        else 99999999,
+                    )
+                )
+            except (
+                TypeError
+            ):  # in rare cases this might fail because of some inconsistency, return unsorted then
+                return [sort_by_position(x) for x in data]
         else:
             try:
-                return list(sorted( ( sort_by_position(x) for x in data) , key=lambda x: alt_sort_key(x) ) )
-            except TypeError: #in rare cases this might fail because of some inconsistency, return unsorted then
-                return [ sort_by_position(x) for x in data ]
+                return list(
+                    sorted(
+                        (sort_by_position(x) for x in data),
+                        key=lambda x: alt_sort_key(x),
+                    )
+                )
+            except (
+                TypeError
+            ):  # in rare cases this might fail because of some inconsistency, return unsorted then
+                return [sort_by_position(x) for x in data]
     elif isinstance(data, dict):
-        if 'rdf:first' in data:
-            #ordered rdf list
+        if "rdf:first" in data:
+            # ordered rdf list
             return list(rdf_list_to_normal_list(data))
         else:
             for key, value in data.items():
                 data[key] = sort_by_position(value)
     return data
 
+
 def rdf_list_to_normal_list(data):
-    if 'rdf:first' in data:
-        yield data['rdf:first']
-    if 'rdf:rest' in data and data['rdf:rest']:
-        assert isinstance(data['rdf:rest'], dict)
-        for e in rdf_list_to_normal_list(data['rdf:rest']):
+    if "rdf:first" in data:
+        yield data["rdf:first"]
+    if "rdf:rest" in data and data["rdf:rest"]:
+        assert isinstance(data["rdf:rest"], dict)
+        for e in rdf_list_to_normal_list(data["rdf:rest"]):
             yield e
 
 
-def cleanup(data: Union[dict,list,tuple,str], baseuri: Optional[str] = None) -> Union[dict,list,str]:
+def cleanup(
+    data: Union[dict, list, tuple, str], baseuri: Optional[str] = None
+) -> Union[dict, list, str]:
     """This cleans up the serialisation:
-       * It Recursively removes namespace prefixes from dictionary keys
-       * It removes the IDs of all former blank nodes (stubs) (making them blank again)
-       * It enforces @id and @type rather than the id/type aliases
-       * It removes file:// prefixes from URIs
-       * It removes the _embedding_done helper
+    * It Recursively removes namespace prefixes from dictionary keys
+    * It removes the IDs of all former blank nodes (stubs) (making them blank again)
+    * It enforces @id and @type rather than the id/type aliases
+    * It removes file:// prefixes from URIs
+    * It removes the _embedding_done helper
     """
     if isinstance(data, dict):
-        if 'id' in data:
-            data['@id'] = data['id']
-            del data['id']
-        if 'type' in data:
-            data['@type'] = data['type']
-            del data['type']
-        if '_embedding_done' in data:
-            del data['_embedding_done']
-        if '@id' in data:
-            if (data['@id'].startswith('_') or data['@id'].startswith("file://") or (baseuri and data['@id'].startswith(baseuri + "stub/"))) and len(data) > 1:
-                del data['@id']
-        return { key.replace('schema:','').replace('http://schema.org/','').replace('codemeta:','').replace('stypes:','') : cleanup(value, baseuri) for key, value in data.items() }
-    elif isinstance(data, (list,tuple)):
-        return [ cleanup(x, baseuri) for x in data ]
-    elif isinstance(data,str) and data.startswith('file://'):
+        if "id" in data:
+            data["@id"] = data["id"]
+            del data["id"]
+        if "type" in data:
+            data["@type"] = data["type"]
+            del data["type"]
+        if "_embedding_done" in data:
+            del data["_embedding_done"]
+        if "@id" in data:
+            if (
+                data["@id"].startswith("_")
+                or data["@id"].startswith("file://")
+                or (baseuri and data["@id"].startswith(baseuri + "stub/"))
+            ) and len(data) > 1:
+                del data["@id"]
+        return {
+            key.replace("schema:", "")
+            .replace("http://schema.org/", "")
+            .replace("codemeta:", "")
+            .replace("stypes:", ""): cleanup(value, baseuri)
+            for key, value in data.items()
+        }
+    elif isinstance(data, (list, tuple)):
+        return [cleanup(x, baseuri) for x in data]
+    elif isinstance(data, str) and data.startswith("file://"):
         return data[7:]
     else:
         return data
 
-def find_main(data, res: Union[URIRef,None]):
+
+def find_main(data, res: Union[URIRef, None]):
     """Find the main item in the graph"""
-    if '@graph' in data:
+    if "@graph" in data:
         for item in data:
             if isinstance(item, dict) and item.get("@id") == str(res):
                 return item, data
         return None, None
     else:
         return data, None
 
+
 def expand_implicit_id_nodes(data, idref_properties):
     """Turn nodes like `key: uri` into `key: { "@id": uri }`"""
     if isinstance(data, dict):
         for k, v in data.items():
-            if k in idref_properties and isinstance(v, str) and (v.startswith(("http","_","/")) or v.startswith(NSPREFIXES)):
-                data[k] = {"@id": v }
+            if (
+                k in idref_properties
+                and isinstance(v, str)
+                and (v.startswith(("http", "_", "/")) or v.startswith(NSPREFIXES))
+            ):
+                data[k] = {"@id": v}
             elif k in idref_properties and isinstance(v, list):
-                data[k] = [ {"@id": e } if isinstance(e, str) and (e.startswith(("http","_","/")) or e.startswith(NSPREFIXES)) else expand_implicit_id_nodes(e, idref_properties) if isinstance(e, dict) else e for e in v ]
+                data[k] = [
+                    {"@id": e}
+                    if isinstance(e, str)
+                    and (e.startswith(("http", "_", "/")) or e.startswith(NSPREFIXES))
+                    else expand_implicit_id_nodes(e, idref_properties)
+                    if isinstance(e, dict)
+                    else e
+                    for e in v
+                ]
             elif isinstance(v, dict):
                 data[k] = expand_implicit_id_nodes(data[k], idref_properties)
             elif isinstance(v, list):
-                data[k] = [ expand_implicit_id_nodes(e, idref_properties) if isinstance(e,dict) else e for e in v ]
+                data[k] = [
+                    expand_implicit_id_nodes(e, idref_properties)
+                    if isinstance(e, dict)
+                    else e
+                    for e in v
+                ]
     return data
 
-def do_object_framing(data: dict, res_id: str, history: set = set(), preserve_context: bool = True):
+
+def do_object_framing(
+    data: dict, res_id: str, history: set = set(), preserve_context: bool = True
+):
     """JSON-LD object framing. Rdflib's json-ld serialiser doesn't implement this so we do this ourselves"""
-    itemmap = {} #mapping from ids to python dicts
-    if '@graph' in data:
-        gather_items(data['@graph'], itemmap)
+    itemmap = {}  # mapping from ids to python dicts
+    if "@graph" in data:
+        gather_items(data["@graph"], itemmap)
     else:
         gather_items(data, itemmap)
-    #print("DEBUG itemmap", repr(itemmap))
+    # print("DEBUG itemmap", repr(itemmap))
     if res_id not in itemmap:
         raise Exception(f"Resource {res_id} not found in tree, framing not possible")
     embed_items(itemmap[res_id], itemmap, history)
-    if '@context' in data and preserve_context:
-        #preserve context
-        itemmap[res_id]['@context'] = data['@context']
+    if "@context" in data and preserve_context:
+        # preserve context
+        itemmap[res_id]["@context"] = data["@context"]
     return itemmap[res_id]
-        
+
+
 def gather_items(data, itemmap: dict):
     """Gather all items from a JSON-LD tree, auxiliary function for object framing"""
-    if isinstance(data, list): 
+    if isinstance(data, list):
         for item in data:
             gather_items(item, itemmap)
-    elif isinstance(data, dict): 
-        for idkey in ('@id', 'id'):
+    elif isinstance(data, dict):
+        for idkey in ("@id", "id"):
             if idkey in data and len(data) > 1 and isinstance(idkey, str):
                 item_id = data[idkey]
                 if idkey in itemmap:
-                    #print(f"DEBUG gathered {item_id} (duplicate)",file=sys.stderr)
+                    # print(f"DEBUG gathered {item_id} (duplicate)",file=sys.stderr)
                     itemmap[item_id].update(data)
                 else:
-                    #print(f"DEBUG gathered {item_id} (new)",file=sys.stderr)
+                    # print(f"DEBUG gathered {item_id} (new)",file=sys.stderr)
                     itemmap[item_id] = data
         for v in data.values():
             gather_items(v, itemmap)
 
+
 def embed_items(data, itemmap: dict, history: set):
     """Replace all references with items, auxiliary function for object framing. The history prevents circular references."""
-    if isinstance(data, list): 
+    if isinstance(data, list):
         for i, item in enumerate(data):
-            #print(f"DEBUG processing list, #history: {len(history)}", file=sys.stderr)
-            data[i] = embed_items(item, itemmap, copy(history)) #recursion step
-    elif isinstance(data, dict): 
-        for idkey in ('@id', 'id'):
+            # print(f"DEBUG processing list, #history: {len(history)}", file=sys.stderr)
+            data[i] = embed_items(item, itemmap, copy(history))  # recursion step
+    elif isinstance(data, dict):
+        for idkey in ("@id", "id"):
             if idkey in data and data[idkey] in itemmap and data[idkey] not in history:
-                #print(f"DEBUG embedded {data[idkey]} (explicit)", file=sys.stderr)
+                # print(f"DEBUG embedded {data[idkey]} (explicit)", file=sys.stderr)
                 history.add(data[idkey])
-                #print(f"DEBUG (recursing over embedded content)", file=sys.stderr)
-                if '_embedding_done' in itemmap[data[idkey]]:
+                # print(f"DEBUG (recursing over embedded content)", file=sys.stderr)
+                if "_embedding_done" in itemmap[data[idkey]]:
                     data = itemmap[data[idkey]]
                 else:
                     data = embed_items(itemmap[data[idkey]], itemmap, copy(history))
-                    data['_embedding_done'] = True
+                    data["_embedding_done"] = True
                 return data
-            #elif idkey in data and data[idkey] not in itemmap:
+            # elif idkey in data and data[idkey] not in itemmap:
             #    print(f"DEBUG could not embed {data[idkey]}, not in graph", file=sys.stderr)
-            #elif idkey in data and data[idkey] and data[idkey] in history:
+            # elif idkey in data and data[idkey] and data[idkey] in history:
             #    print(f"DEBUG could not embed {data[idkey]}, already in history, returning a reference", file=sys.stderr)
             #    return { idkey: data[idkey] }
         for k, v in data.items():
-            if k not in ('@id','id') and k not in NOEMBED:
-                #print(f"DEBUG processing key {k}, #history: {len(history)}", file=sys.stderr)
-                data[k] = embed_items(v, itemmap, copy(history)) #recursion step
-    elif isinstance(data, str) and (data.startswith(("http","file://","/","_")) or data.startswith(NSPREFIXES)) and data in itemmap and data not in history: #this is probably a reference even though it's not explicit
-        #data is an URI reference we can resolve
+            if k not in ("@id", "id") and k not in NOEMBED:
+                # print(f"DEBUG processing key {k}, #history: {len(history)}", file=sys.stderr)
+                data[k] = embed_items(v, itemmap, copy(history))  # recursion step
+    elif (
+        isinstance(data, str)
+        and (
+            data.startswith(("http", "file://", "/", "_"))
+            or data.startswith(NSPREFIXES)
+        )
+        and data in itemmap
+        and data not in history
+    ):  # this is probably a reference even though it's not explicit
+        # data is an URI reference we can resolve
         history.add(data)
-        #print(f"DEBUG embedded {data} (implicit), recursing over embedded content", file=sys.stderr)
-        if '_embedding_done' in itemmap[data]:
+        # print(f"DEBUG embedded {data} (implicit), recursing over embedded content", file=sys.stderr)
+        if "_embedding_done" in itemmap[data]:
             data = itemmap[data]
         else:
             data = embed_items(itemmap[data], itemmap, copy(history))
-            data['_embedding_done'] = True
+            data["_embedding_done"] = True
     return data
 
 
-def hide_ordered_lists(data: Union[dict,list,tuple,str], key: Optional[str] = None) -> Union[dict,list,str]:
+def hide_ordered_lists(
+    data: Union[dict, list, tuple, str], key: Optional[str] = None
+) -> Union[dict, list, str]:
     """Hide explicit @list nodes on known ordered list properties, on read-in they will be assumed agained via the (manipulated) context"""
     if isinstance(data, dict):
-        if '@list' in data and key in ORDEREDLIST_PROPERTIES_NAMES:
-            return hide_ordered_lists(data['@list'])
+        if "@list" in data and key in ORDEREDLIST_PROPERTIES_NAMES:
+            return hide_ordered_lists(data["@list"])
         else:
             for k, v in data.items():
                 data[k] = hide_ordered_lists(v, k)
-    elif isinstance(data, (list,tuple)):
-        return [ hide_ordered_lists(v) for v in data ]
+    elif isinstance(data, (list, tuple)):
+        return [hide_ordered_lists(v) for v in data]
     return data
 
 
-    
-
-def rewrite_context(context, addcontext = None) -> list:
+def rewrite_context(context, addcontext=None) -> list:
     """Rewrite local contexts to their remote counterparts"""
     if isinstance(context, list):
         for i, value in enumerate(context):
             if value == CODEMETA_LOCAL_SOURCE:
                 context[i] = CODEMETA_SOURCE
             elif value == SCHEMA_LOCAL_SOURCE:
                 context[i] = SCHEMA_SOURCE
@@ -222,71 +332,87 @@
             elif value == IODATA_LOCAL_SOURCE:
                 context[i] = IODATA_SOURCE
             elif value == REPOSTATUS_LOCAL_SOURCE:
                 context[i] = REPOSTATUS_SOURCE
             elif addcontext:
                 for remote_url in addcontext:
                     if not remote_url.startswith("http"):
-                        raise Exception(f"Explicitly added context (--addcontext) must be a remote URL, got {remote_url} instead")
-                    local = "file://" + os.path.join(TMPDIR, os.path.basename(remote_url))
+                        raise Exception(
+                            f"Explicitly added context (--addcontext) must be a remote URL, got {remote_url} instead"
+                        )
+                    local = "file://" + os.path.join(
+                        TMPDIR, os.path.basename(remote_url)
+                    )
                     if value == local:
                         context[i] = remote_url
     elif isinstance(context, str):
         context = rewrite_context([context])
 
     if context and context[-1] == DEVIANT_CONTEXT:
-        #we strip the internal 'deviant' context so it's never explicitly outputted
+        # we strip the internal 'deviant' context so it's never explicitly outputted
         context = context[:-1]
     return context
 
-def serialize_to_jsonld(g: Graph, res: Union[Sequence,URIRef,None], args: AttribDict) -> dict:
-    """Serializes the RDF graph to JSON, taking care of 'object framing' for embedded nodes"""
 
+def serialize_to_jsonld(
+    g: Graph, res: Union[Sequence, URIRef, None], args: AttribDict
+) -> dict:
+    """Serializes the RDF graph to JSON, taking care of 'object framing' for embedded nodes"""
 
     #                                              v--- the internal 'deviant' context is required for the serialisation to work, it will be stripped later in rewrite_context()
-    context =[ x[0] for x in init_context(args)] + [DEVIANT_CONTEXT] 
-    data = json.loads(g.serialize(format='json-ld', auto_compact=True, context=context))
+    context = [x[0] for x in init_context(args)] + [DEVIANT_CONTEXT]
+    data = json.loads(g.serialize(format="json-ld", auto_compact=True, context=context))
 
-    #rdflib doesn't do 'object framing' so we have to do it in this post-processing step
-    #if we have a single resource, it'll be the focus object the whole frame will be built around
-    if res and (not isinstance(res, (list,tuple)) or len(res) == 1):
+    # rdflib doesn't do 'object framing' so we have to do it in this post-processing step
+    # if we have a single resource, it'll be the focus object the whole frame will be built around
+    if res and (not isinstance(res, (list, tuple)) or len(res) == 1):
         assert isinstance(res, URIRef)
         if args.includecontext:
-            data = expand_implicit_id_nodes(data, [ str(x).split("/")[-1] for x in PREFER_URIREF_PROPERTIES])
+            data = expand_implicit_id_nodes(
+                data, [str(x).split("/")[-1] for x in PREFER_URIREF_PROPERTIES]
+            )
         data = do_object_framing(data, str(res))
         # Hide explicit @list nodes, on read-in they will be assumed agained via the (manipulated) context
         data = hide_ordered_lists(data)
         assert isinstance(data, dict)
 
         root, parent = find_main(data, res)
-        if parent and len(data['@graph']) == 1 and res:
-            #No need for @graph if it contains only one item now:
+        if parent and len(data["@graph"]) == 1 and res:
+            # No need for @graph if it contains only one item now:
             assert isinstance(root, dict)
             parent.update(root)
-            del data['@graph']
+            del data["@graph"]
             root = parent
         data = sort_by_position(data)
     else:
-        #we have a graph of multiple resources, structure is mostly stand-off: we do object framing on each SoftwareSourceCode instance (this does lead to some redundancy)
+        # we have a graph of multiple resources, structure is mostly stand-off: we do object framing on each SoftwareSourceCode instance (this does lead to some redundancy)
         if args.includecontext:
-            data = expand_implicit_id_nodes(data, [ str(x).split("/")[-1] for x in PREFER_URIREF_PROPERTIES])
-        if '@graph' in data:
+            data = expand_implicit_id_nodes(
+                data, [str(x).split("/")[-1] for x in PREFER_URIREF_PROPERTIES]
+            )
+        if "@graph" in data:
             new_graph = []
-            for item in data['@graph']:
-                if isinstance(item, dict) and item.get('@type', item.get('type',None)) == 'SoftwareSourceCode':
-                    item_id = item.get('@id', item.get('id', None))
+            for item in data["@graph"]:
+                if (
+                    isinstance(item, dict)
+                    and item.get("@type", item.get("type", None))
+                    == "SoftwareSourceCode"
+                ):
+                    item_id = item.get("@id", item.get("id", None))
                     if item_id:
-                        new_graph.append(do_object_framing(data, item_id, preserve_context=False))
-            data['@graph'] = new_graph
+                        new_graph.append(
+                            do_object_framing(data, item_id, preserve_context=False)
+                        )
+            data["@graph"] = new_graph
         data = hide_ordered_lists(data)
         data = sort_by_position(data)
 
     assert isinstance(data, dict)
-    if '@context' in data:
-        #remap local context references to URLs
-        data['@context'] = rewrite_context(data['@context'], args.addcontext)
+    if "@context" in data:
+        # remap local context references to URLs
+        data["@context"] = rewrite_context(data["@context"], args.addcontext)
 
-    #we may have some lingering prefixes which we don't need and we want @id and @type instead of 'id' and 'type', cleanup:
+    # we may have some lingering prefixes which we don't need and we want @id and @type instead of 'id' and 'type', cleanup:
     data = cleanup(data, args.baseuri)
 
     assert isinstance(data, dict)
     return data
```

### Comparing `CodeMetaPy-2.4.1/codemeta/serializers/turtle.py` & `CodeMetaPy-2.5.0/codemeta/serializers/turtle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sys
 import json
 from codemeta.common import SDO, get_subgraph
 from typing import Union, IO, Sequence
 from rdflib import Graph, URIRef, BNode, Literal
 
 
-def serialize_to_turtle(g: Graph, res: Union[Sequence,URIRef,None]) -> str:
+def serialize_to_turtle(g: Graph, res: Union[Sequence, URIRef, None]) -> str:
     """Serializes the RDF graph to Turtle"""
     if res:
-        #Get the subgraph that focusses on this specific resource (may be multiple) 
-        #TODO: this may not work well with ordered lists yet!!
-        if isinstance(res, (list,tuple)):
+        # Get the subgraph that focusses on this specific resource (may be multiple)
+        # TODO: this may not work well with ordered lists yet!!
+        if isinstance(res, (list, tuple)):
             g = get_subgraph(g, res)
         else:
             g = get_subgraph(g, [res])
 
-    g.bind('sdo', SDO)
-    return g.serialize(format='turtle', auto_compact=True)
+    g.bind("sdo", SDO)
+    return g.serialize(format="turtle", auto_compact=True)
```

### Comparing `CodeMetaPy-2.4.1/codemeta/validation.py` & `CodeMetaPy-2.5.0/codemeta/validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,83 +1,164 @@
 import sys
 import os
 import datetime
-from rdflib import Graph, Namespace, URIRef, BNode, Literal
-from rdflib.namespace import RDF, SH
-from typing import Union, IO, Sequence, Optional, Tuple
-from codemeta.common import init_graph, init_context, CODEMETA, AttribDict,  SDO,  generate_uri
+from rdflib import Graph, URIRef, BNode, Literal
+from rdflib.namespace import RDF, SH # type: ignore
+from typing import Union, Sequence, Optional, Tuple
+from codemeta.common import (
+    AttribDict,
+    SDO,
+    generate_uri,
+)
 
 from pyshacl import validate as pyshacl_validate
 
-def validate(g: Graph, res: Union[URIRef,BNode], args: AttribDict, contextgraph: Union[Graph,None] = None) -> Tuple[bool, Graph]:
+
+def validate(
+    g: Graph,
+    res: Union[URIRef, BNode],
+    args: AttribDict,
+    contextgraph: Union[Graph, None] = None,
+) -> Tuple[bool, Graph]:
     """Validates software metadata using SHACL, generates a validation report and adds it to the SoftwareSourceCode metadata via the schema:review property"""
-    shacl_file: str = args.validate
+    shacl_file: str = args.validate #type: ignore
     if shacl_file.endswith("ttl"):
-        shacl_format="turtle"
-    elif shacl_file.endswith(("json","jsonld")):
-        shacl_format="json-ld"
+        shacl_format = "turtle"
+    elif shacl_file.endswith(("json", "jsonld")):
+        shacl_format = "json-ld"
     else:
-        raise ValueError(f"Expect ttl or json file for SHACL ({args.validate}), unable to determine from extension")
+        raise ValueError(
+            f"Expect ttl or json file for SHACL ({args.validate}), unable to determine from extension"
+        )
     shacl_graph = Graph()
     shacl_graph.parse(args.validate, format=shacl_format)
-    conforms, results_graph, _ = pyshacl_validate(data_graph=g, shacl_graph=shacl_graph, ont_graph=contextgraph, abort_on_first=False, allow_infos=True, allow_warnings=True)
+    conforms, results_graph, _ = pyshacl_validate(
+        data_graph=g,
+        shacl_graph=shacl_graph,
+        ont_graph=contextgraph,
+        abort_on_first=False,
+        allow_infos=True,
+        allow_warnings=True,
+    )
     counter = 0
-    review = URIRef(generate_uri(None, args.baseuri,prefix="validation"))
+    review = URIRef(generate_uri(None, args.baseuri, prefix="validation"))
     g.add((review, RDF.type, SDO.Review))
-    g.add((review, SDO.author, Literal(f"codemetapy validator using {os.path.basename(shacl_file)}")))
-    g.add((review, SDO.datePublished, Literal(datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"))))
-    name = g.value(res,SDO.name)
-    if not name: name = "unnamed software"
-    version = g.value(res,SDO.version)
-    if not version: version = "(unknown version)"
-    g.add((review, SDO.name, Literal(f"Automatic software metadata validation report for {name} {version}")))
+    g.add(
+        (
+            review,
+            SDO.author,
+            Literal(f"codemetapy validator using {os.path.basename(shacl_file)}"),
+        )
+    )
+    g.add(
+        (
+            review,
+            SDO.datePublished,
+            Literal(datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")),
+        )
+    )
+    name = g.value(res, SDO.name)
+    if not name:
+        name = "unnamed software"
+    version = g.value(res, SDO.version)
+    if not version:
+        version = "(unknown version)"
+    g.add(
+        (
+            review,
+            SDO.name,
+            Literal(
+                f"Automatic software metadata validation report for {name} {version}"
+            ),
+        )
+    )
     messages = []
     warnings = 0
     violations = 0
     info = 0
-    for node ,_,_ in results_graph.triples((None,SH.focusNode,res)):
+    for node, _, _ in results_graph.triples((None, SH.focusNode, res)):
         if (node, RDF.type, SH.ValidationResult) in results_graph:
             severity = ""
             if (node, SH.resultSeverity, SH.Violation) in results_graph:
                 severity = "Violation"
                 violations += 1
             elif (node, SH.resultSeverity, SH.Warning) in results_graph:
                 severity = "Warning"
                 warnings += 1
             elif (node, SH.resultSeverity, SH.Info) in results_graph:
                 severity = "Info"
                 info += 1
             else:
                 severity = "Unknown"
             cause = ""
-            if (node, SH.sourceConstraintComponent, SH.ClassConstraintComponent) in results_graph:
+            if (
+                node,
+                SH.sourceConstraintComponent,
+                SH.ClassConstraintComponent,
+            ) in results_graph:
                 cause = "The metadata does express this currently, but the wrong class is used."
-            elif (node, SH.sourceConstraintComponent, SH.DatatypeConstraintComponent) in results_graph:
+            elif (
+                node,
+                SH.sourceConstraintComponent,
+                SH.DatatypeConstraintComponent,
+            ) in results_graph:
                 cause = "The metadata does express this currently, but the wrong datatype is used"
-            elif (node, SH.sourceConstraintComponent, SH.NodeKindConstraintComponent) in results_graph:
+            elif (
+                node,
+                SH.sourceConstraintComponent,
+                SH.NodeKindConstraintComponent,
+            ) in results_graph:
                 cause = "The metadata does express this currently, but the wrong node kind is used (probably URI vs literal)"
-            elif (node, SH.sourceConstraintComponent, SH.OrConstraintComponent) in results_graph:
+            elif (
+                node,
+                SH.sourceConstraintComponent,
+                SH.OrConstraintComponent,
+            ) in results_graph:
                 cause = "The metadata does express this currently, but something is wrong in the way it is expressed. Is the type/class valid?"
-            elif (node, SH.sourceConstraintComponent, SH.QualifiedMinCountConstraintComponent) in results_graph:
+            elif (
+                node,
+                SH.sourceConstraintComponent,
+                SH.QualifiedMinCountConstraintComponent,
+            ) in results_graph:
                 cause = "This is missing in the metadata"
-            elif (node, SH.sourceConstraintComponent, SH.QualifiedMaxCountConstraintComponent) in results_graph:
-                cause = "The metadata expresses this multiple times and is too ambiguous"
-            elif (node, SH.sourceConstraintComponent, SH.MinCountConstraintComponent) in results_graph:
+            elif (
+                node,
+                SH.sourceConstraintComponent,
+                SH.QualifiedMaxCountConstraintComponent,
+            ) in results_graph:
+                cause = (
+                    "The metadata expresses this multiple times and is too ambiguous"
+                )
+            elif (
+                node,
+                SH.sourceConstraintComponent,
+                SH.MinCountConstraintComponent,
+            ) in results_graph:
                 cause = "This is missing in the metadata"
-            elif (node, SH.sourceConstraintComponent, SH.MaxCountConstraintComponent) in results_graph:
-                cause = "The metadata expresses this multiple times and is too ambiguous"
-            if cause: cause = f"({cause})"
+            elif (
+                node,
+                SH.sourceConstraintComponent,
+                SH.MaxCountConstraintComponent,
+            ) in results_graph:
+                cause = (
+                    "The metadata expresses this multiple times and is too ambiguous"
+                )
+            if cause:
+                cause = f"({cause})"
 
-            #path = results_graph.value(node, SH.resultPath)
+            # path = results_graph.value(node, SH.resultPath)
             msg = results_graph.value(node, SH.resultMessage)
             if msg:
-                counter +=1 
-                print(f"VALIDATION {str(res)} #{counter}: {severity}: {str(msg)} {cause}", file=sys.stderr)
+                counter += 1
+                print(
+                    f"VALIDATION {str(res)} #{counter}: {severity}: {str(msg)} {cause}",
+                    file=sys.stderr,
+                )
                 messages.append(f"{counter}. {severity}: {msg} {cause}")
-    head = args.textv  + "\n\n" if args.textv else ""
+    head = args.textv + "\n\n" if args.textv else ""
     if messages:
         if conforms:
             if warnings:
                 head += f"Validation of {name} {version} was successful (score=3/5), but there are some warnings which should be addressed:"
                 g.add((review, SDO.reviewRating, Literal(3)))
             else:
                 head += f"Validation of {name} {version} was successful (score=4/5), but there are some remarks which you may or may not want to address:"
@@ -91,23 +172,28 @@
                 score = "(score 1/5)"
             else:
                 g.add((review, SDO.reviewRating, Literal(2)))
                 score = "(score 2/5)"
             head += f"Validation of {name} {version} failed {score} due to one or more requirement violations:"
         g.add((review, SDO.reviewBody, Literal(head + "\n\n" + "\n".join(messages))))
     else:
-        g.add((review, SDO.reviewBody, Literal("Validates perfectly, no further remarks!")))
+        g.add(
+            (
+                review,
+                SDO.reviewBody,
+                Literal("Validates perfectly, no further remarks!"),
+            )
+        )
         g.add((review, SDO.reviewRating, Literal(5)))
     g.add((res, SDO.review, review))
     return conforms, results_graph
 
-def get_validation_report(g: Graph, res: Union[Sequence,URIRef,BNode]) -> Optional[str]:
+
+def get_validation_report(
+    g: Graph, res: Union[Sequence, URIRef, BNode]
+) -> Optional[str]:
     """Get the text of an existing validation report for the given resource"""
-    if (res,RDF.type,SDO.Review):
-        return g.value(res,SDO.reviewBody)
+    if (res, RDF.type, SDO.Review):
+        return g.value(res, SDO.reviewBody)
     else:
-        for _,_,review in g.triples((res,SDO.review,None)):
-            return g.value(review,SDO.reviewBody)
-
-            
-
-    
+        for _, _, review in g.triples((res, SDO.review, None)): #type: ignore
+            return g.value(review, SDO.reviewBody)
```

### Comparing `CodeMetaPy-2.4.1/setup.py` & `CodeMetaPy-2.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     cmdclass={}
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname),'r',encoding='utf-8').read()
 
 setup(
     name = "CodeMetaPy",
-    version = "2.4.1", #also adapt in codemeta.json
+    version = "2.5.0", #also adapt in codemeta.json
     author = "Maarten van Gompel",
     author_email = "proycon@anaproy.nl",
     description = ("Generate and manage CodeMeta software metadata"),
     license = "GPL-3.0-only",
     keywords = [ "software metadata", "codemeta", "schema.org", "rdf", "linked data"],
     url = "https://github.com/proycon/codemetapy",
     packages=['codemeta', 'codemeta.parsers','codemeta.serializers'],
@@ -37,11 +37,11 @@
         "Operating System :: POSIX",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
     zip_safe=False,
     include_package_data=True,
     package_data = { 'codemeta': ['schema/crosswalk.csv', 'schema/codemeta.jsonld', 'templates/*.html','resources/*.css', 'resources/fa-*' ] },
-    install_requires=[ 'nameparser','importlib_metadata','BeautifulSoup4', 'rdflib >= 6.1.1','pyshacl', 'requests','lxml','pyyaml','Jinja2','pep517','tomlkit','pyproject_parser'],
+    install_requires=[ 'nameparser','importlib_metadata','BeautifulSoup4', 'rdflib >= 6.1.1','pyshacl == 0.20.0', 'requests','lxml','pyyaml','pep517','tomlkit','pyproject_parser'],
     entry_points = {    'console_scripts': [ 'codemetapy = codemeta.codemeta:main' ] },
     cmdclass=cmdclass
 )
```

### Comparing `CodeMetaPy-2.4.1/tests/tests.py` & `CodeMetaPy-2.5.0/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,17 +160,14 @@
         self.assertEqual(data['softwareHelp']['url'], "https://frognlp.readthedocs.io", "Testing softwareHelp URL")
 
 
     def test100_serialisation_turtle(self):
         """Test json serialisation"""
         serialize(self.g, self.res, AttribDict({ "output": "ttl" }), self.contextgraph)
 
-    def test100_serialisation_html(self):
-        """Test html serialisation"""
-        serialize(self.g, self.res, AttribDict({ "output": "html" }), self.contextgraph)
 
 
 class BuildTest_SetupPy(unittest.TestCase):
 
     def setUp(self):
         #relies on automatically guessing the type based on the directory we are inputsources
         os.chdir("fusus")
@@ -221,17 +218,14 @@
         """Test json serialisation"""
         serialize(self.g, self.res, AttribDict({ "output": "json" }), self.contextgraph)
 
     def test100_serialisation_turtle(self):
         """Test json serialisation"""
         serialize(self.g, self.res, AttribDict({ "output": "ttl" }), self.contextgraph)
 
-    def test100_serialisation_html(self):
-        """Test html serialisation"""
-        serialize(self.g, self.res, AttribDict({ "output": "html" }), self.contextgraph)
 
 class BuildTest_GithubAPI(unittest.TestCase):
     """Build codemeta.json from existing codemeta.json (basically a parse, validation/reconciliation and reserialisation)"""
 
     def setUp(self):
         #relies on automatically guessing the type
         #deliberately picked software that is end-of-life and will not change much anymore
@@ -272,17 +266,14 @@
         """Test json serialisation"""
         serialize(self.g, self.res, AttribDict({ "output": "json" }), self.contextgraph)
 
     def test100_serialisation_turtle(self):
         """Test json serialisation"""
         serialize(self.g, self.res, AttribDict({ "output": "ttl" }), self.contextgraph)
 
-    def test100_serialisation_html(self):
-        """Test html serialisation"""
-        serialize(self.g, self.res, AttribDict({ "output": "html" }), self.contextgraph)
 
 class BuildTest_NpmPackageJSON(unittest.TestCase):
     """Build codemeta.json from npm package json"""
 
     def setUp(self):
         #relies on automatically guessing the type
         self.g, self.res, self.args, self.contextgraph = build(inputsources=["labirinto.package.json"])
@@ -311,17 +302,14 @@
         """Test json serialisation"""
         serialize(self.g, self.res, AttribDict({ "output": "json" }), self.contextgraph)
 
     def test100_serialisation_turtle(self):
         """Test json serialisation"""
         serialize(self.g, self.res, AttribDict({ "output": "ttl" }), self.contextgraph)
 
-    def test100_serialisation_html(self):
-        """Test html serialisation"""
-        serialize(self.g, self.res, AttribDict({ "output": "html" }), self.contextgraph)
 
 class BuildTest_Web_HTML(unittest.TestCase):
     """Build codemeta.json from webpage metadata"""
 
     def setUp(self):
         #relies on automatically guessing the type
         self.g, self.res, self.args, self.contextgraph = build(inputsources=["https://shebanq.ancient-data.org/"], with_stypes=True)
@@ -511,15 +499,12 @@
         """Test json serialisation"""
         serialize(self.g, self.res, AttribDict({ "output": "json" }), self.contextgraph)
 
     def test100_serialisation_turtle(self):
         """Test json serialisation"""
         serialize(self.g, self.res, AttribDict({ "output": "ttl" }), self.contextgraph)
 
-    def test100_serialisation_html(self):
-        """Test html serialisation"""
-        serialize(self.g, self.res, AttribDict({ "output": "html" }), self.contextgraph)
 
 
 if __name__ == '__main__':
     unittest.main()
```

