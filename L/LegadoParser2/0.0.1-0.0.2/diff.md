# Comparing `tmp/LegadoParser2-0.0.1.tar.gz` & `tmp/LegadoParser2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LegadoParser2-0.0.1.tar", last modified: Mon May 15 16:53:29 2023, max compression
+gzip compressed data, was "LegadoParser2-0.0.2.tar", last modified: Mon May 15 17:07:48 2023, max compression
```

## Comparing `LegadoParser2-0.0.1.tar` & `LegadoParser2-0.0.2.tar`

### file list

```diff
@@ -1,67 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.840055 LegadoParser2-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-05-15 16:10:54.000000 LegadoParser2-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      550 2023-05-15 16:53:29.840055 LegadoParser2-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-05-15 16:12:00.000000 LegadoParser2-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-15 16:12:52.000000 LegadoParser2-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 16:53:29.840055 LegadoParser2-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      892 2023-05-15 16:52:16.000000 LegadoParser2-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.803470 LegadoParser2-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.821055 LegadoParser2-0.0.1/src/LegadoParser2/
--rw-rw-rw-   0        0        0     3415 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/BookInfo.py
--rw-rw-rw-   0        0        0     4508 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/Chapter.py
--rw-rw-rw-   0        0        0     4651 2023-05-02 14:05:57.000000 LegadoParser2-0.0.1/src/LegadoParser2/ChapterList.py
--rw-rw-rw-   0        0        0     3800 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/Debug.py
--rw-rw-rw-   0        0        0     1962 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/FormatUtils.py
--rw-rw-rw-   0        0        0     1367 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/GSON.py
--rw-rw-rw-   0        0        0     4993 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/HttpRequset2.py
--rw-rw-rw-   0        0        0    15949 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleCompile.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.829056 LegadoParser2-0.0.1/src/LegadoParser2/RuleDefault/
--rw-rw-rw-   0        0        0      421 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleDefault/EndRule.py
--rw-rw-rw-   0        0        0    11652 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleDefault/RuleDefaultEfficient2.py
--rw-rw-rw-   0        0        0       65 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleDefault/__init__.py
--rw-rw-rw-   0        0        0     8707 2023-05-02 06:17:05.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleEval.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.831057 LegadoParser2-0.0.1/src/LegadoParser2/RuleJs/
--rw-rw-rw-   0        0        0     2920 2023-05-15 16:40:05.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleJs/JS.py
--rw-rw-rw-   0        0        0       41 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleJs/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleJs/jsExtension.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.832055 LegadoParser2-0.0.1/src/LegadoParser2/RuleJsonPath/
--rw-rw-rw-   0        0        0     3962 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleJsonPath/RuleJsonPath.py
--rw-rw-rw-   0        0        0       57 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleJsonPath/__init__.py
--rw-rw-rw-   0        0        0      657 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleObjectEncoder.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.833055 LegadoParser2-0.0.1/src/LegadoParser2/RuleRegex/
--rw-rw-rw-   0        0        0     2081 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleRegex/RuleRegex.py
--rw-rw-rw-   0        0        0       51 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleRegex/__init__.py
--rw-rw-rw-   0        0        0     6237 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleType.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.835055 LegadoParser2-0.0.1/src/LegadoParser2/RuleUrl/
--rw-rw-rw-   0        0        0      110 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleUrl/BodyType.py
--rw-rw-rw-   0        0        0     6511 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleUrl/Url.py
--rw-rw-rw-   0        0        0      264 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleUrl/UrlEval.py
--rw-rw-rw-   0        0        0      138 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleUrl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.836055 LegadoParser2-0.0.1/src/LegadoParser2/RuleXpath/
--rw-rw-rw-   0        0        0     2491 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleXpath/RuleXpath.py
--rw-rw-rw-   0        0        0       51 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/RuleXpath/__init__.py
--rw-rw-rw-   0        0        0     5585 2023-04-30 07:42:52.000000 LegadoParser2-0.0.1/src/LegadoParser2/Search.py
--rw-rw-rw-   0        0        0      602 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/StrOperate.py
--rw-rw-rw-   0        0        0    20933 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/Tokenize2.py
--rw-rw-rw-   0        0        0       70 2023-05-15 16:09:50.000000 LegadoParser2-0.0.1/src/LegadoParser2/__init__.py
--rw-rw-rw-   0        0        0      601 2023-04-12 16:33:21.000000 LegadoParser2-0.0.1/src/LegadoParser2/config.py
--rw-rw-rw-   0        0        0     5206 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/entities.py
--rw-rw-rw-   0        0        0      335 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/exceptions.py
--rw-rw-rw-   0        0        0     8259 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/fontutils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.839055 LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/
--rw-rw-rw-   0        0        0     9493 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/__init__.py
--rw-rw-rw-   0        0        0     2714 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/dom.py
--rw-rw-rw-   0        0        0     6549 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/encoding_names.py
--rw-rw-rw-   0        0        0    11970 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/encoding_parser.py
--rw-rw-rw-   0        0        0     4358 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/soup.py
--rw-rw-rw-   0        0        0     1569 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/stdlib_etree.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.839055 LegadoParser2-0.0.1/src/LegadoParser2/quickjs/
--rw-rw-rw-   0        0        0     3512 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/quickjs/__init__.py
--rw-rw-rw-   0        0        0       70 2023-05-15 16:10:28.000000 LegadoParser2-0.0.1/src/LegadoParser2/test.py
--rw-rw-rw-   0        0        0      319 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/utils.py
--rw-rw-rw-   0        0        0     8391 2023-04-12 14:32:46.000000 LegadoParser2-0.0.1/src/LegadoParser2/webview.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:53:29.827062 LegadoParser2-0.0.1/src/LegadoParser2.egg-info/
--rw-rw-rw-   0        0        0      550 2023-05-15 16:53:29.000000 LegadoParser2-0.0.1/src/LegadoParser2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2023-05-15 16:53:29.000000 LegadoParser2-0.0.1/src/LegadoParser2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 16:53:29.000000 LegadoParser2-0.0.1/src/LegadoParser2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 16:53:29.000000 LegadoParser2-0.0.1/src/LegadoParser2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.166531 LegadoParser2-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-05-15 16:10:54.000000 LegadoParser2-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-15 17:06:49.000000 LegadoParser2-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      550 2023-05-15 17:07:48.165445 LegadoParser2-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-05-15 16:12:00.000000 LegadoParser2-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-15 16:12:52.000000 LegadoParser2-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 17:07:48.166531 LegadoParser2-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-05-15 17:07:29.000000 LegadoParser2-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.112953 LegadoParser2-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.134360 LegadoParser2-0.0.2/src/LegadoParser2/
+-rw-rw-rw-   0        0        0     3415 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/BookInfo.py
+-rw-rw-rw-   0        0        0     4508 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/Chapter.py
+-rw-rw-rw-   0        0        0     4651 2023-05-02 14:05:57.000000 LegadoParser2-0.0.2/src/LegadoParser2/ChapterList.py
+-rw-rw-rw-   0        0        0     3800 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/Debug.py
+-rw-rw-rw-   0        0        0     1962 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/FormatUtils.py
+-rw-rw-rw-   0        0        0     1367 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/GSON.py
+-rw-rw-rw-   0        0        0     4993 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/HttpRequset2.py
+-rw-rw-rw-   0        0        0    15949 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleCompile.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.152376 LegadoParser2-0.0.2/src/LegadoParser2/RuleDefault/
+-rw-rw-rw-   0        0        0      421 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleDefault/EndRule.py
+-rw-rw-rw-   0        0        0    11652 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleDefault/RuleDefaultEfficient2.py
+-rw-rw-rw-   0        0        0       65 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleDefault/__init__.py
+-rw-rw-rw-   0        0        0     8707 2023-05-02 06:17:05.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleEval.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.153380 LegadoParser2-0.0.2/src/LegadoParser2/RuleJs/
+-rw-rw-rw-   0        0        0     2920 2023-05-15 16:40:05.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleJs/JS.py
+-rw-rw-rw-   0        0        0       41 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleJs/__init__.py
+-rw-rw-rw-   0        0        0    59277 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleJs/jsExtension.js
+-rw-rw-rw-   0        0        0     2226 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleJs/jsExtension.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.154387 LegadoParser2-0.0.2/src/LegadoParser2/RuleJsonPath/
+-rw-rw-rw-   0        0        0     3962 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleJsonPath/RuleJsonPath.py
+-rw-rw-rw-   0        0        0       57 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleJsonPath/__init__.py
+-rw-rw-rw-   0        0        0      657 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleObjectEncoder.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.155395 LegadoParser2-0.0.2/src/LegadoParser2/RuleRegex/
+-rw-rw-rw-   0        0        0     2081 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleRegex/RuleRegex.py
+-rw-rw-rw-   0        0        0       51 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleRegex/__init__.py
+-rw-rw-rw-   0        0        0     6237 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleType.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.157432 LegadoParser2-0.0.2/src/LegadoParser2/RuleUrl/
+-rw-rw-rw-   0        0        0      110 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleUrl/BodyType.py
+-rw-rw-rw-   0        0        0     6511 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleUrl/Url.py
+-rw-rw-rw-   0        0        0      264 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleUrl/UrlEval.py
+-rw-rw-rw-   0        0        0      138 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleUrl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.158490 LegadoParser2-0.0.2/src/LegadoParser2/RuleXpath/
+-rw-rw-rw-   0        0        0     2491 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleXpath/RuleXpath.py
+-rw-rw-rw-   0        0        0       51 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/RuleXpath/__init__.py
+-rw-rw-rw-   0        0        0     5585 2023-04-30 07:42:52.000000 LegadoParser2-0.0.2/src/LegadoParser2/Search.py
+-rw-rw-rw-   0        0        0      602 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/StrOperate.py
+-rw-rw-rw-   0        0        0    20933 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/Tokenize2.py
+-rw-rw-rw-   0        0        0       70 2023-05-15 16:09:50.000000 LegadoParser2-0.0.2/src/LegadoParser2/__init__.py
+-rw-rw-rw-   0        0        0      601 2023-04-12 16:33:21.000000 LegadoParser2-0.0.2/src/LegadoParser2/config.py
+-rw-rw-rw-   0        0        0     5206 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/entities.py
+-rw-rw-rw-   0        0        0      335 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/exceptions.py
+-rw-rw-rw-   0        0        0     8259 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/fontutils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.164440 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/
+-rw-rw-rw-   0        0        0     9493 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/__init__.py
+-rw-rw-rw-   0        0        0     2714 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/dom.py
+-rw-rw-rw-   0        0        0     6549 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/encoding_names.py
+-rw-rw-rw-   0        0        0    11970 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/encoding_parser.py
+-rw-rw-rw-   0        0        0    83456 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/libexslt.dll
+-rw-rw-rw-   0        0        0  1515520 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/libxml2.dll
+-rw-rw-rw-   0        0        0   221696 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/libxslt.dll
+-rw-rw-rw-   0        0        0     4358 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/soup.py
+-rw-rw-rw-   0        0        0     1569 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/stdlib_etree.py
+-rw-rw-rw-   0        0        0    88064 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/zlib1.dll
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.165445 LegadoParser2-0.0.2/src/LegadoParser2/quickjs/
+-rw-rw-rw-   0        0        0     3512 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/quickjs/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-05-15 16:10:28.000000 LegadoParser2-0.0.2/src/LegadoParser2/test.py
+-rw-rw-rw-   0        0        0      319 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/utils.py
+-rw-rw-rw-   0        0        0     8391 2023-04-12 14:32:46.000000 LegadoParser2-0.0.2/src/LegadoParser2/webview.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:07:48.150278 LegadoParser2-0.0.2/src/LegadoParser2.egg-info/
+-rw-rw-rw-   0        0        0      550 2023-05-15 17:07:48.000000 LegadoParser2-0.0.2/src/LegadoParser2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2265 2023-05-15 17:07:48.000000 LegadoParser2-0.0.2/src/LegadoParser2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 17:07:48.000000 LegadoParser2-0.0.2/src/LegadoParser2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 17:07:48.000000 LegadoParser2-0.0.2/src/LegadoParser2.egg-info/top_level.txt
```

### Comparing `LegadoParser2-0.0.1/PKG-INFO` & `LegadoParser2-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LegadoParser2
-Version: 0.0.1
+Version: 0.0.2
 Summary: parse legado rule package
 Home-page: https://github.com/pypa/sampleproject
 Author: Legado
 Author-email: 843019417@qq.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LegadoParser2-0.0.1/setup.py` & `LegadoParser2-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="LegadoParser2",
-    version="0.0.1",
+    version="0.0.2",
     author="Legado",
     author_email="843019417@qq.com",
     description="parse legado rule package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     project_urls={
         "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_data={"pipmodule": ["*.js","*.dll","*.pyd"]},
+    package_data={"": ["*.js", "*.dll"]},
     package_dir={"": "src"},
+    include_package_data=True,
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
```

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/BookInfo.py` & `LegadoParser2-0.0.2/src/LegadoParser2/BookInfo.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/Chapter.py` & `LegadoParser2-0.0.2/src/LegadoParser2/Chapter.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/ChapterList.py` & `LegadoParser2-0.0.2/src/LegadoParser2/ChapterList.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/Debug.py` & `LegadoParser2-0.0.2/src/LegadoParser2/Debug.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/FormatUtils.py` & `LegadoParser2-0.0.2/src/LegadoParser2/FormatUtils.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/GSON.py` & `LegadoParser2-0.0.2/src/LegadoParser2/GSON.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/HttpRequset2.py` & `LegadoParser2-0.0.2/src/LegadoParser2/HttpRequset2.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleCompile.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleCompile.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleDefault/RuleDefaultEfficient2.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleDefault/RuleDefaultEfficient2.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleEval.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleEval.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleJs/JS.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleJs/JS.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleJs/jsExtension.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleJs/jsExtension.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleJsonPath/RuleJsonPath.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleJsonPath/RuleJsonPath.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleObjectEncoder.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleObjectEncoder.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleRegex/RuleRegex.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleRegex/RuleRegex.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleType.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleType.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleUrl/Url.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleUrl/Url.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/RuleXpath/RuleXpath.py` & `LegadoParser2-0.0.2/src/LegadoParser2/RuleXpath/RuleXpath.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/Search.py` & `LegadoParser2-0.0.2/src/LegadoParser2/Search.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/StrOperate.py` & `LegadoParser2-0.0.2/src/LegadoParser2/StrOperate.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/Tokenize2.py` & `LegadoParser2-0.0.2/src/LegadoParser2/Tokenize2.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/config.py` & `LegadoParser2-0.0.2/src/LegadoParser2/config.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/entities.py` & `LegadoParser2-0.0.2/src/LegadoParser2/entities.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/fontutils.py` & `LegadoParser2-0.0.2/src/LegadoParser2/fontutils.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/__init__.py` & `LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/dom.py` & `LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/dom.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/encoding_names.py` & `LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/encoding_names.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/encoding_parser.py` & `LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/encoding_parser.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/soup.py` & `LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/soup.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/html5_parser/stdlib_etree.py` & `LegadoParser2-0.0.2/src/LegadoParser2/html5_parser/stdlib_etree.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/quickjs/__init__.py` & `LegadoParser2-0.0.2/src/LegadoParser2/quickjs/__init__.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2/webview.py` & `LegadoParser2-0.0.2/src/LegadoParser2/webview.py`

 * *Files identical despite different names*

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2.egg-info/PKG-INFO` & `LegadoParser2-0.0.2/src/LegadoParser2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LegadoParser2
-Version: 0.0.1
+Version: 0.0.2
 Summary: parse legado rule package
 Home-page: https://github.com/pypa/sampleproject
 Author: Legado
 Author-email: 843019417@qq.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LegadoParser2-0.0.1/src/LegadoParser2.egg-info/SOURCES.txt` & `LegadoParser2-0.0.2/src/LegadoParser2.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+./src/LegadoParser2/RuleJs/jsExtension.js
+./src/LegadoParser2/html5_parser/libexslt.dll
+./src/LegadoParser2/html5_parser/libxml2.dll
+./src/LegadoParser2/html5_parser/libxslt.dll
+./src/LegadoParser2/html5_parser/zlib1.dll
 src/LegadoParser2/BookInfo.py
 src/LegadoParser2/Chapter.py
 src/LegadoParser2/ChapterList.py
 src/LegadoParser2/Debug.py
 src/LegadoParser2/FormatUtils.py
 src/LegadoParser2/GSON.py
 src/LegadoParser2/HttpRequset2.py
@@ -29,14 +35,15 @@
 src/LegadoParser2.egg-info/dependency_links.txt
 src/LegadoParser2.egg-info/top_level.txt
 src/LegadoParser2/RuleDefault/EndRule.py
 src/LegadoParser2/RuleDefault/RuleDefaultEfficient2.py
 src/LegadoParser2/RuleDefault/__init__.py
 src/LegadoParser2/RuleJs/JS.py
 src/LegadoParser2/RuleJs/__init__.py
+src/LegadoParser2/RuleJs/jsExtension.js
 src/LegadoParser2/RuleJs/jsExtension.py
 src/LegadoParser2/RuleJsonPath/RuleJsonPath.py
 src/LegadoParser2/RuleJsonPath/__init__.py
 src/LegadoParser2/RuleRegex/RuleRegex.py
 src/LegadoParser2/RuleRegex/__init__.py
 src/LegadoParser2/RuleUrl/BodyType.py
 src/LegadoParser2/RuleUrl/Url.py
@@ -44,10 +51,14 @@
 src/LegadoParser2/RuleUrl/__init__.py
 src/LegadoParser2/RuleXpath/RuleXpath.py
 src/LegadoParser2/RuleXpath/__init__.py
 src/LegadoParser2/html5_parser/__init__.py
 src/LegadoParser2/html5_parser/dom.py
 src/LegadoParser2/html5_parser/encoding_names.py
 src/LegadoParser2/html5_parser/encoding_parser.py
+src/LegadoParser2/html5_parser/libexslt.dll
+src/LegadoParser2/html5_parser/libxml2.dll
+src/LegadoParser2/html5_parser/libxslt.dll
 src/LegadoParser2/html5_parser/soup.py
 src/LegadoParser2/html5_parser/stdlib_etree.py
+src/LegadoParser2/html5_parser/zlib1.dll
 src/LegadoParser2/quickjs/__init__.py
```

