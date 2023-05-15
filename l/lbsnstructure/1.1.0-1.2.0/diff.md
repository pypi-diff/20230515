# Comparing `tmp/lbsnstructure-1.1.0.tar.gz` & `tmp/lbsnstructure-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbsnstructure-1.1.0.tar", last modified: Fri May 12 10:28:26 2023, max compression
+gzip compressed data, was "lbsnstructure-1.2.0.tar", last modified: Mon May 15 11:14:09 2023, max compression
```

## Comparing `lbsnstructure-1.1.0.tar` & `lbsnstructure-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.895713 lbsnstructure-1.1.0/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1227 2019-07-11 09:18:07.000000 lbsnstructure-1.1.0/.gitignore
--rwxrwxrwx   0 alex      (1000) alex      (1000)      807 2023-05-04 10:44:19.000000 lbsnstructure-1.1.0/.gitlab-ci.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1655 2023-05-12 10:28:17.000000 lbsnstructure-1.1.0/CHANGELOG.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.1.0/LICENSE.md
--rw-r--r--   0 alex      (1000) alex      (1000)     3115 2023-05-12 10:28:26.896134 lbsnstructure-1.1.0/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)     2778 2023-05-10 06:12:09.000000 lbsnstructure-1.1.0/README.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)     4124 2019-07-11 09:18:07.000000 lbsnstructure-1.1.0/StructureTest.ipynb
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.644081 lbsnstructure-1.1.0/google/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.744611 lbsnstructure-1.1.0/google/protobuf/
--rw-r--r--   0 alex      (1000) alex      (1000)     1625 2023-05-12 09:14:33.000000 lbsnstructure-1.1.0/google/protobuf/duration_pb2.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1641 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/google/protobuf/timestamp_pb2.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.870633 lbsnstructure-1.1.0/lbsnstructure/
--rw-rw-rw-   0 alex      (1000) alex      (1000)      425 2023-05-04 09:00:50.000000 lbsnstructure-1.1.0/lbsnstructure/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2703 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/interlinkage_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5527 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/social_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4172 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/spatial_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2693 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/temporal_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5116 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/topical_pb2.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)       22 2023-05-12 10:28:17.000000 lbsnstructure-1.1.0/lbsnstructure/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.893125 lbsnstructure-1.1.0/lbsnstructure.egg-info/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     3115 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/PKG-INFO
--rw-rw-rw-   0 alex      (1000) alex      (1000)      584 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/SOURCES.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/dependency_links.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2019-07-11 11:04:14.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/not-zip-safe
--rw-rw-rw-   0 alex      (1000) alex      (1000)        9 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/requires.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)       14 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/top_level.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2023-05-12 10:28:26.898553 lbsnstructure-1.1.0/setup.cfg
--rw-rw-rw-   0 alex      (1000) alex      (1000)      909 2019-07-11 09:18:07.000000 lbsnstructure-1.1.0/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-15 11:14:09.634899 lbsnstructure-1.2.0/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.2.0/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     3119 2023-05-15 11:14:09.632896 lbsnstructure-1.2.0/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     2778 2023-05-10 06:12:09.000000 lbsnstructure-1.2.0/README.md
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     1115 2023-05-15 11:13:22.000000 lbsnstructure-1.2.0/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-15 11:14:09.635274 lbsnstructure-1.2.0/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-15 11:14:09.439451 lbsnstructure-1.2.0/src/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-15 11:14:09.609557 lbsnstructure-1.2.0/src/lbsnstructure/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      647 2023-05-15 11:05:47.000000 lbsnstructure-1.2.0/src/lbsnstructure/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2703 2023-05-15 10:25:53.000000 lbsnstructure-1.2.0/src/lbsnstructure/interlinkage_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       27 2023-05-15 10:55:05.000000 lbsnstructure-1.2.0/src/lbsnstructure/py.typed
+-rw-r--r--   0 alex      (1000) alex      (1000)     5527 2023-05-15 10:25:53.000000 lbsnstructure-1.2.0/src/lbsnstructure/social_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16339 2023-05-15 10:25:53.000000 lbsnstructure-1.2.0/src/lbsnstructure/social_pb2.pyi
+-rw-r--r--   0 alex      (1000) alex      (1000)     4172 2023-05-15 10:25:53.000000 lbsnstructure-1.2.0/src/lbsnstructure/spatial_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10723 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/spatial_pb2.pyi
+-rw-r--r--   0 alex      (1000) alex      (1000)     2693 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/temporal_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6292 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/temporal_pb2.pyi
+-rw-r--r--   0 alex      (1000) alex      (1000)     5119 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/topical_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    22233 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/topical_pb2.pyi
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       22 2023-05-15 11:13:40.000000 lbsnstructure-1.2.0/src/lbsnstructure/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-15 11:14:09.631063 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3119 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      671 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-15 10:48:01.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/not-zip-safe
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       14 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/top_level.txt
```

### Comparing `lbsnstructure-1.1.0/LICENSE.md` & `lbsnstructure-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.1.0/PKG-INFO` & `lbsnstructure-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.1.0
+Version: 1.2.0
 Summary: A common language independent and cross-network social-media data scheme.
-Home-page: https://gitlab.vgiscience.de/lbsn/concept
-Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
-Author-email: alexander.dunkel@tu-dresden.de
+Author: Filip Krumpe, Marc Löchner
+Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://lbsn.vgiscience.org/
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![pypi version](https://lbsn.vgiscience.org/structure/python/version.svg) ![pipeline status](https://gitlab.vgiscience.de/lbsn/structure/python/badges/master/pipeline.svg) from protobuf: ![version](https://lbsn.vgiscience.org/structure/protobuf/version.svg) 
 
 # LBSNSTRUCTURE
 
@@ -61,8 +61,7 @@
 The versioning (major.minor.patch) is automated using [python-semantic-release](https://github.com/relekang/python-semantic-release).
 Commit messages that follow the [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) will be automatically interpreted, 
 followed by version bumps if necessary. 
 
 ## License
 
 This project is licensed under the  MIT License.
-
```

### Comparing `lbsnstructure-1.1.0/README.md` & `lbsnstructure-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.1.0/lbsnstructure/interlinkage_pb2.py` & `lbsnstructure-1.2.0/src/lbsnstructure/interlinkage_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.1.0/lbsnstructure/social_pb2.py` & `lbsnstructure-1.2.0/src/lbsnstructure/social_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.1.0/lbsnstructure/spatial_pb2.py` & `lbsnstructure-1.2.0/src/lbsnstructure/spatial_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.1.0/lbsnstructure/temporal_pb2.py` & `lbsnstructure-1.2.0/src/lbsnstructure/temporal_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.1.0/lbsnstructure/topical_pb2.py` & `lbsnstructure-1.2.0/src/lbsnstructure/topical_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from lbsnstructure import social_pb2 as lbsnstructure_dot_social__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1blbsnstructure/topical.proto\x12\x0elbsn.structure\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1albsnstructure/social.proto\"\xd6\x08\n\x04Post\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x13\n\x0bpost_latlng\x18\x02 \x01(\t\x12\x30\n\nplace_pkey\x18\x03 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tcity_pkey\x18\x04 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x32\n\x0c\x63ountry_pkey\x18\x05 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tuser_pkey\x18\x06 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x35\n\x11post_publish_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tpost_body\x18\x08 \x01(\t\x12>\n\x10post_geoaccuracy\x18\t \x01(\x0e\x32$.lbsn.structure.Post.PostGeoaccuracy\x12\x38\n\x12user_mentions_pkey\x18\n \x03(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x10\n\x08hashtags\x18\x0b \x03(\t\x12\r\n\x05\x65moji\x18\x0c \x03(\t\x12\x17\n\x0fpost_like_count\x18\r \x01(\x03\x12\x1a\n\x12post_comment_count\x18\x0e \x01(\x03\x12\x18\n\x10post_views_count\x18\x0f \x01(\x03\x12\x12\n\npost_title\x18\x10 \x01(\t\x12\x34\n\x10post_create_date\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12post_thumbnail_url\x18\x12 \x01(\t\x12\x10\n\x08post_url\x18\x13 \x01(\t\x12\x30\n\tpost_type\x18\x14 \x01(\x0e\x32\x1d.lbsn.structure.Post.PostType\x12\x13\n\x0bpost_filter\x18\x15 \x01(\t\x12\x18\n\x10post_quote_count\x18\x16 \x01(\x03\x12\x18\n\x10post_share_count\x18\x17 \x01(\x03\x12\x14\n\x0cinput_source\x18\x18 \x01(\t\x12/\n\rpost_language\x18\x19 \x01(\x0b\x32\x18.lbsn.structure.Language\x12\x1c\n\x14post_content_license\x18\x1a \x01(\x05\x12\x12\n\npost_topic\x18\x1b \x03(\t\x12\x16\n\x0epost_downvotes\x18\x1c \x01(\x03\"L\n\x0fPostGeoaccuracy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LATLNG\x10\x01\x12\t\n\x05PLACE\x10\x02\x12\x08\n\x04\x43ITY\x10\x03\x12\x0b\n\x07\x43OUNTRY\x10\x04\"?\n\x08PostType\x12\x08\n\x04TEXT\x10\x00\x12\t\n\x05IMAGE\x10\x01\x12\t\n\x05VIDEO\x10\x02\x12\x08\n\x04LINK\x10\x03\x12\t\n\x05OTHER\x10\x04\"\xc8\x04\n\x0cPostReaction\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tuser_pkey\x18\x02 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x39\n\x13referencedPost_pkey\x18\x03 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x41\n\x1breferencedPostreaction_pkey\x18\x04 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x17\n\x0freaction_latlng\x18\x05 \x01(\t\x12@\n\rreaction_type\x18\x06 \x01(\x0e\x32).lbsn.structure.PostReaction.ReactionType\x12\x31\n\rreaction_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10reaction_content\x18\x08 \x01(\t\x12\x1b\n\x13reaction_like_count\x18\t \x01(\x03\x12\x38\n\x12user_mentions_pkey\x18\n \x03(\x0b\x32\x1c.lbsn.structure.CompositeKey\"^\n\x0cReactionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05SHARE\x10\x01\x12\x0b\n\x07\x43OMMENT\x10\x02\x12\t\n\x05QUOTE\x10\x03\x12\x08\n\x04LIKE\x10\x04\x12\t\n\x05\x45MOJI\x10\x05\x12\t\n\x05OTHER\x10\x06\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1blbsnstructure/topical.proto\x12\x0elbsn.structure\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1albsnstructure/social.proto\"\xd7\x08\n\x04Post\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x13\n\x0bpost_latlng\x18\x02 \x01(\t\x12\x30\n\nplace_pkey\x18\x03 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tcity_pkey\x18\x04 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x32\n\x0c\x63ountry_pkey\x18\x05 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tuser_pkey\x18\x06 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x35\n\x11post_publish_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tpost_body\x18\x08 \x01(\t\x12>\n\x10post_geoaccuracy\x18\t \x01(\x0e\x32$.lbsn.structure.Post.PostGeoaccuracy\x12\x38\n\x12user_mentions_pkey\x18\n \x03(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x10\n\x08hashtags\x18\x0b \x03(\t\x12\r\n\x05\x65moji\x18\x0c \x03(\t\x12\x17\n\x0fpost_like_count\x18\r \x01(\x03\x12\x1a\n\x12post_comment_count\x18\x0e \x01(\x03\x12\x18\n\x10post_views_count\x18\x0f \x01(\x03\x12\x12\n\npost_title\x18\x10 \x01(\t\x12\x34\n\x10post_create_date\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12post_thumbnail_url\x18\x12 \x01(\t\x12\x10\n\x08post_url\x18\x13 \x01(\t\x12\x30\n\tpost_type\x18\x14 \x01(\x0e\x32\x1d.lbsn.structure.Post.PostType\x12\x13\n\x0bpost_filter\x18\x15 \x01(\t\x12\x18\n\x10post_quote_count\x18\x16 \x01(\x03\x12\x18\n\x10post_share_count\x18\x17 \x01(\x03\x12\x14\n\x0cinput_source\x18\x18 \x01(\t\x12/\n\rpost_language\x18\x19 \x01(\x0b\x32\x18.lbsn.structure.Language\x12\x1c\n\x14post_content_license\x18\x1a \x01(\x05\x12\x13\n\x0btopic_group\x18\x1b \x03(\t\x12\x16\n\x0epost_downvotes\x18\x1c \x01(\x03\"L\n\x0fPostGeoaccuracy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LATLNG\x10\x01\x12\t\n\x05PLACE\x10\x02\x12\x08\n\x04\x43ITY\x10\x03\x12\x0b\n\x07\x43OUNTRY\x10\x04\"?\n\x08PostType\x12\x08\n\x04TEXT\x10\x00\x12\t\n\x05IMAGE\x10\x01\x12\t\n\x05VIDEO\x10\x02\x12\x08\n\x04LINK\x10\x03\x12\t\n\x05OTHER\x10\x04\"\xc8\x04\n\x0cPostReaction\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tuser_pkey\x18\x02 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x39\n\x13referencedPost_pkey\x18\x03 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x41\n\x1breferencedPostreaction_pkey\x18\x04 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x17\n\x0freaction_latlng\x18\x05 \x01(\t\x12@\n\rreaction_type\x18\x06 \x01(\x0e\x32).lbsn.structure.PostReaction.ReactionType\x12\x31\n\rreaction_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10reaction_content\x18\x08 \x01(\t\x12\x1b\n\x13reaction_like_count\x18\t \x01(\x03\x12\x38\n\x12user_mentions_pkey\x18\n \x03(\x0b\x32\x1c.lbsn.structure.CompositeKey\"^\n\x0cReactionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05SHARE\x10\x01\x12\x0b\n\x07\x43OMMENT\x10\x02\x12\t\n\x05QUOTE\x10\x03\x12\x08\n\x04LIKE\x10\x04\x12\t\n\x05\x45MOJI\x10\x05\x12\t\n\x05OTHER\x10\x06\x62\x06proto3')
 
 
 
 _POST = DESCRIPTOR.message_types_by_name['Post']
 _POSTREACTION = DESCRIPTOR.message_types_by_name['PostReaction']
 _POST_POSTGEOACCURACY = _POST.enum_types_by_name['PostGeoaccuracy']
 _POST_POSTTYPE = _POST.enum_types_by_name['PostType']
@@ -39,17 +39,17 @@
   })
 _sym_db.RegisterMessage(PostReaction)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _POST._serialized_start=109
-  _POST._serialized_end=1219
-  _POST_POSTGEOACCURACY._serialized_start=1078
-  _POST_POSTGEOACCURACY._serialized_end=1154
-  _POST_POSTTYPE._serialized_start=1156
-  _POST_POSTTYPE._serialized_end=1219
-  _POSTREACTION._serialized_start=1222
-  _POSTREACTION._serialized_end=1806
-  _POSTREACTION_REACTIONTYPE._serialized_start=1712
-  _POSTREACTION_REACTIONTYPE._serialized_end=1806
+  _POST._serialized_end=1220
+  _POST_POSTGEOACCURACY._serialized_start=1079
+  _POST_POSTGEOACCURACY._serialized_end=1155
+  _POST_POSTTYPE._serialized_start=1157
+  _POST_POSTTYPE._serialized_end=1220
+  _POSTREACTION._serialized_start=1223
+  _POSTREACTION._serialized_end=1807
+  _POSTREACTION_REACTIONTYPE._serialized_start=1713
+  _POSTREACTION_REACTIONTYPE._serialized_end=1807
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lbsnstructure-1.1.0/lbsnstructure.egg-info/PKG-INFO` & `lbsnstructure-1.2.0/src/lbsnstructure.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.1.0
+Version: 1.2.0
 Summary: A common language independent and cross-network social-media data scheme.
-Home-page: https://gitlab.vgiscience.de/lbsn/concept
-Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
-Author-email: alexander.dunkel@tu-dresden.de
+Author: Filip Krumpe, Marc Löchner
+Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://lbsn.vgiscience.org/
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![pypi version](https://lbsn.vgiscience.org/structure/python/version.svg) ![pipeline status](https://gitlab.vgiscience.de/lbsn/structure/python/badges/master/pipeline.svg) from protobuf: ![version](https://lbsn.vgiscience.org/structure/protobuf/version.svg) 
 
 # LBSNSTRUCTURE
 
@@ -61,8 +61,7 @@
 The versioning (major.minor.patch) is automated using [python-semantic-release](https://github.com/relekang/python-semantic-release).
 Commit messages that follow the [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) will be automatically interpreted, 
 followed by version bumps if necessary. 
 
 ## License
 
 This project is licensed under the  MIT License.
-
```

