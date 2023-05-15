# Comparing `tmp/somerandomapi.py-0.0.3.tar.gz` & `tmp/somerandomapi.py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somerandomapi.py-0.0.3.tar", last modified: Sat May  6 16:38:39 2023, max compression
+gzip compressed data, was "somerandomapi.py-0.0.4.tar", last modified: Mon May 15 03:50:27 2023, max compression
```

## Comparing `somerandomapi.py-0.0.3.tar` & `somerandomapi.py-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.701849 somerandomapi.py-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-05-06 16:38:39.701849 somerandomapi.py-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:38:39.701849 somerandomapi.py-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.693849 somerandomapi.py-0.0.3/somerandomapi/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.693849 somerandomapi.py-0.0.3/somerandomapi/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/animal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/animu.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.693849 somerandomapi.py-0.0.3/somerandomapi/internals/
--rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/internals/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/internals/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.697849 somerandomapi.py-0.0.3/somerandomapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/animal_fact.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/animu_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/lyrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/namecard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/rankcard.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/tweet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.697849 somerandomapi.py-0.0.3/somerandomapi/models/welcome/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/welcome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/welcome/free.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/welcome/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/youtube_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.697849 somerandomapi.py-0.0.3/somerandomapi/types/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/animal.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/animu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.701849 somerandomapi.py-0.0.3/somerandomapi/types/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/canvas/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/canvas/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/canvas/overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/img.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/others.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.693849 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:50:27.567345 somerandomapi.py-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-05-15 03:50:27.567345 somerandomapi.py-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 03:50:27.567345 somerandomapi.py-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:50:27.559344 somerandomapi.py-0.0.4/somerandomapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:50:27.563345 somerandomapi.py-0.0.4/somerandomapi/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/clients/animal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/clients/animu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/clients/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/clients/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/clients/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/clients/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:50:27.563345 somerandomapi.py-0.0.4/somerandomapi/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/internals/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/internals/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:50:27.567345 somerandomapi.py-0.0.4/somerandomapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/animal_fact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/animu_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/namecard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/rankcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/tweet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:50:27.567345 somerandomapi.py-0.0.4/somerandomapi/models/welcome/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/welcome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/welcome/free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/welcome/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/models/youtube_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:50:27.567345 somerandomapi.py-0.0.4/somerandomapi/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/animal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/animu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:50:27.567345 somerandomapi.py-0.0.4/somerandomapi/types/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/canvas/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/canvas/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/canvas/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/img.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/others.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/types/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-15 03:50:19.000000 somerandomapi.py-0.0.4/somerandomapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:50:27.563345 somerandomapi.py-0.0.4/somerandomapi.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-05-15 03:50:27.000000 somerandomapi.py-0.0.4/somerandomapi.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-15 03:50:27.000000 somerandomapi.py-0.0.4/somerandomapi.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 03:50:27.000000 somerandomapi.py-0.0.4/somerandomapi.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-15 03:50:27.000000 somerandomapi.py-0.0.4/somerandomapi.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 03:50:27.000000 somerandomapi.py-0.0.4/somerandomapi.py.egg-info/top_level.txt
```

### Comparing `somerandomapi.py-0.0.3/LICENSE` & `somerandomapi.py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/PKG-INFO` & `somerandomapi.py-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somerandomapi.py
-Version: 0.0.3
+Version: 0.0.4
 Summary: A maintained wrapper for the somerandomapi API.
 Author: Soheab_
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `somerandomapi.py-0.0.3/pyproject.toml` & `somerandomapi.py-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/clients/__init__.py` & `somerandomapi.py-0.0.4/somerandomapi/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/clients/animal.py` & `somerandomapi.py-0.0.4/somerandomapi/clients/animal.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/clients/animu.py` & `somerandomapi.py-0.0.4/somerandomapi/clients/animu.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/clients/canvas.py` & `somerandomapi.py-0.0.4/somerandomapi/clients/canvas.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/clients/chatbot.py` & `somerandomapi.py-0.0.4/somerandomapi/clients/chatbot.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/clients/client.py` & `somerandomapi.py-0.0.4/somerandomapi/clients/client.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/clients/pokemon.py` & `somerandomapi.py-0.0.4/somerandomapi/clients/pokemon.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/clients/premium.py` & `somerandomapi.py-0.0.4/somerandomapi/clients/premium.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/enums.py` & `somerandomapi.py-0.0.4/somerandomapi/enums.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/errors.py` & `somerandomapi.py-0.0.4/somerandomapi/errors.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/internals/endpoints.py` & `somerandomapi.py-0.0.4/somerandomapi/internals/endpoints.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/internals/http.py` & `somerandomapi.py-0.0.4/somerandomapi/internals/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 class APIKey(NamedTuple):
     tier: Literal[0, 1, 2, 3]
     value: str
 
 
 class HTTPClient:
-    BASE_URL: ClassVar[str] = "https://some-random-api.ml"
+    BASE_URL: ClassVar[str] = "https://some-random-api.com"
 
     __slots__ = ("_animal", "_animu", "_canvas", "_pokemon", "_premium", "_key", "_session", "__chatbot")
 
     def __init__(
         self,
         key: Optional[tuple[Literal[0, 1, 2, 3], str]],
         session: Optional[aiohttp.ClientSession] = None,
```

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/abc.py` & `somerandomapi.py-0.0.4/somerandomapi/models/abc.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/dictionary.py` & `somerandomapi.py-0.0.4/somerandomapi/models/dictionary.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/encoding.py` & `somerandomapi.py-0.0.4/somerandomapi/models/encoding.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/image.py` & `somerandomapi.py-0.0.4/somerandomapi/models/image.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/lyrics.py` & `somerandomapi.py-0.0.4/somerandomapi/models/lyrics.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/namecard.py` & `somerandomapi.py-0.0.4/somerandomapi/models/namecard.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/pokemon.py` & `somerandomapi.py-0.0.4/somerandomapi/models/pokemon.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/rankcard.py` & `somerandomapi.py-0.0.4/somerandomapi/models/rankcard.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/rgb.py` & `somerandomapi.py-0.0.4/somerandomapi/models/rgb.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/tweet.py` & `somerandomapi.py-0.0.4/somerandomapi/models/tweet.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/welcome/free.py` & `somerandomapi.py-0.0.4/somerandomapi/models/welcome/free.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/welcome/premium.py` & `somerandomapi.py-0.0.4/somerandomapi/models/welcome/premium.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/models/youtube_comment.py` & `somerandomapi.py-0.0.4/somerandomapi/models/youtube_comment.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/types/pokemon.py` & `somerandomapi.py-0.0.4/somerandomapi/types/pokemon.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi/utils.py` & `somerandomapi.py-0.0.4/somerandomapi/utils.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.3/somerandomapi.py.egg-info/PKG-INFO` & `somerandomapi.py-0.0.4/somerandomapi.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somerandomapi.py
-Version: 0.0.3
+Version: 0.0.4
 Summary: A maintained wrapper for the somerandomapi API.
 Author: Soheab_
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `somerandomapi.py-0.0.3/somerandomapi.py.egg-info/SOURCES.txt` & `somerandomapi.py-0.0.4/somerandomapi.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

