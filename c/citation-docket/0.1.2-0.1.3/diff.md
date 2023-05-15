# Comparing `tmp/citation_docket-0.1.2.tar.gz` & `tmp/citation_docket-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_docket-0.1.2.tar", max compression
+gzip compressed data, was "citation_docket-0.1.3.tar", max compression
```

## Comparing `citation_docket-0.1.2.tar` & `citation_docket-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0      681 2023-02-25 08:52:20.504305 citation_docket-0.1.2/citation_docket/__init__.py
--rw-r--r--   0        0        0     2428 2023-02-25 08:47:01.299013 citation_docket-0.1.2/citation_docket/main.py
--rw-r--r--   0        0        0      813 2023-02-25 08:31:23.194919 citation_docket-0.1.2/citation_docket/regexes/__init__.py
--rw-r--r--   0        0        0     3123 2023-02-25 08:29:02.278789 citation_docket-0.1.2/citation_docket/regexes/constructed_ac.py
--rw-r--r--   0        0        0     3164 2023-02-25 08:28:27.409030 citation_docket-0.1.2/citation_docket/regexes/constructed_am.py
--rw-r--r--   0        0        0     2485 2023-02-25 08:28:13.070495 citation_docket-0.1.2/citation_docket/regexes/constructed_bm.py
--rw-r--r--   0        0        0     2858 2023-02-25 08:28:39.943312 citation_docket-0.1.2/citation_docket/regexes/constructed_gr.py
--rw-r--r--   0        0        0     2438 2023-02-25 08:27:53.317404 citation_docket-0.1.2/citation_docket/regexes/constructed_oca.py
--rw-r--r--   0        0        0     1647 2023-02-25 08:31:23.194872 citation_docket-0.1.2/citation_docket/regexes/constructed_pet.py
--rw-r--r--   0        0        0      318 2023-01-22 05:43:38.806076 citation_docket-0.1.2/citation_docket/regexes/models/__init__.py
--rw-r--r--   0        0        0     4824 2023-02-25 08:00:22.655943 citation_docket-0.1.2/citation_docket/regexes/models/constructor.py
--rw-r--r--   0        0        0     1233 2023-02-25 06:10:48.723073 citation_docket-0.1.2/citation_docket/regexes/models/docket_category.py
--rw-r--r--   0        0        0      806 2023-01-23 14:56:36.287341 citation_docket-0.1.2/citation_docket/regexes/models/docket_citation.py
--rw-r--r--   0        0        0     3615 2023-02-25 06:04:26.946543 citation_docket-0.1.2/citation_docket/regexes/models/docket_model.py
--rw-r--r--   0        0        0     2911 2023-01-22 07:02:08.786981 citation_docket-0.1.2/citation_docket/regexes/models/gr_clean.py
--rw-r--r--   0        0        0       81 2023-02-25 07:24:24.112930 citation_docket-0.1.2/citation_docket/regexes/models/misc/__init__.py
--rw-r--r--   0        0        0      746 2022-12-30 05:16:22.648456 citation_docket-0.1.2/citation_docket/regexes/models/misc/extra.py
--rw-r--r--   0        0        0     1514 2022-12-30 05:27:34.939026 citation_docket-0.1.2/citation_docket/regexes/models/misc/num.py
--rw-r--r--   0        0        0      242 2022-11-20 04:25:09.137225 citation_docket-0.1.2/citation_docket/regexes/models/misc/x.py
--rw-r--r--   0        0        0     2607 2023-02-25 08:51:06.796290 citation_docket-0.1.2/citation_docket/sc_website_2023.py
--rw-r--r--   0        0        0     7002 2023-01-22 06:56:13.992705 citation_docket-0.1.2/citation_docket/simple_matcher.py
--rw-r--r--   0        0        0      489 2022-11-20 04:19:09.072188 citation_docket-0.1.2/citation_docket/specials.py
--rw-r--r--   0        0        0     1350 2023-02-25 08:52:03.472625 citation_docket-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 citation_docket-0.1.2/setup.py
--rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 citation_docket-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      681 2023-05-15 16:29:06.515132 citation_docket-0.1.3/citation_docket/__init__.py
+-rw-r--r--   0        0        0     2428 2023-02-25 08:47:01.299013 citation_docket-0.1.3/citation_docket/main.py
+-rw-r--r--   0        0        0      813 2023-02-25 08:31:23.194919 citation_docket-0.1.3/citation_docket/regexes/__init__.py
+-rw-r--r--   0        0        0     3123 2023-02-25 08:29:02.278789 citation_docket-0.1.3/citation_docket/regexes/constructed_ac.py
+-rw-r--r--   0        0        0     3164 2023-02-25 08:28:27.409030 citation_docket-0.1.3/citation_docket/regexes/constructed_am.py
+-rw-r--r--   0        0        0     2485 2023-02-25 08:28:13.070495 citation_docket-0.1.3/citation_docket/regexes/constructed_bm.py
+-rw-r--r--   0        0        0     2858 2023-02-25 08:28:39.943312 citation_docket-0.1.3/citation_docket/regexes/constructed_gr.py
+-rw-r--r--   0        0        0     2436 2023-05-15 16:29:12.052715 citation_docket-0.1.3/citation_docket/regexes/constructed_oca.py
+-rw-r--r--   0        0        0     1647 2023-02-25 08:31:23.194872 citation_docket-0.1.3/citation_docket/regexes/constructed_pet.py
+-rw-r--r--   0        0        0      318 2023-01-22 05:43:38.806076 citation_docket-0.1.3/citation_docket/regexes/models/__init__.py
+-rw-r--r--   0        0        0     4824 2023-02-25 08:00:22.655943 citation_docket-0.1.3/citation_docket/regexes/models/constructor.py
+-rw-r--r--   0        0        0     1233 2023-02-25 06:10:48.723073 citation_docket-0.1.3/citation_docket/regexes/models/docket_category.py
+-rw-r--r--   0        0        0      806 2023-01-23 14:56:36.287341 citation_docket-0.1.3/citation_docket/regexes/models/docket_citation.py
+-rw-r--r--   0        0        0     3615 2023-02-25 06:04:26.946543 citation_docket-0.1.3/citation_docket/regexes/models/docket_model.py
+-rw-r--r--   0        0        0     2911 2023-01-22 07:02:08.786981 citation_docket-0.1.3/citation_docket/regexes/models/gr_clean.py
+-rw-r--r--   0        0        0       81 2023-02-25 07:24:24.112930 citation_docket-0.1.3/citation_docket/regexes/models/misc/__init__.py
+-rw-r--r--   0        0        0      746 2022-12-30 05:16:22.648456 citation_docket-0.1.3/citation_docket/regexes/models/misc/extra.py
+-rw-r--r--   0        0        0     1514 2022-12-30 05:27:34.939026 citation_docket-0.1.3/citation_docket/regexes/models/misc/num.py
+-rw-r--r--   0        0        0      242 2022-11-20 04:25:09.137225 citation_docket-0.1.3/citation_docket/regexes/models/misc/x.py
+-rw-r--r--   0        0        0     2607 2023-02-25 08:51:06.796290 citation_docket-0.1.3/citation_docket/sc_website_2023.py
+-rw-r--r--   0        0        0     7002 2023-01-22 06:56:13.992705 citation_docket-0.1.3/citation_docket/simple_matcher.py
+-rw-r--r--   0        0        0      489 2022-11-20 04:19:09.072188 citation_docket-0.1.3/citation_docket/specials.py
+-rw-r--r--   0        0        0     1466 2023-05-15 16:27:39.511078 citation_docket-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 citation_docket-0.1.3/PKG-INFO
```

### Comparing `citation_docket-0.1.2/citation_docket/__init__.py` & `citation_docket-0.1.3/citation_docket/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 from .sc_website_2023 import extract_docket_meta
 from .main import (
     CITATIONS,
     DocketReportCitationType,
     extract_docket_from_data,
     extract_dockets,
 )
```

### Comparing `citation_docket-0.1.2/citation_docket/main.py` & `citation_docket-0.1.3/citation_docket/main.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/__init__.py` & `citation_docket-0.1.3/citation_docket/regexes/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/constructed_ac.py` & `citation_docket-0.1.3/citation_docket/regexes/constructed_ac.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/constructed_am.py` & `citation_docket-0.1.3/citation_docket/regexes/constructed_am.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/constructed_bm.py` & `citation_docket-0.1.3/citation_docket/regexes/constructed_bm.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/constructed_gr.py` & `citation_docket-0.1.3/citation_docket/regexes/constructed_gr.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/constructed_oca.py` & `citation_docket-0.1.3/citation_docket/regexes/constructed_oca.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,14 @@
     init_name="oca_init",
     docket_regex=oca_phrases,
     key_regex=oca_key,
     num_regex=NUMBER_KEYWORD,
 )
 
 
-
-
 class CitationOCA(DocketReportCitation):
     ...
 
     @classmethod
     def search(cls, text: str) -> Iterator[Self]:
         """Get all dockets matching the `OCA` docket pattern, inclusive of their optional Report object.
```

### Comparing `citation_docket-0.1.2/citation_docket/regexes/constructed_pet.py` & `citation_docket-0.1.3/citation_docket/regexes/constructed_pet.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/models/constructor.py` & `citation_docket-0.1.3/citation_docket/regexes/models/constructor.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/models/docket_category.py` & `citation_docket-0.1.3/citation_docket/regexes/models/docket_category.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/models/docket_citation.py` & `citation_docket-0.1.3/citation_docket/regexes/models/docket_citation.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/models/docket_model.py` & `citation_docket-0.1.3/citation_docket/regexes/models/docket_model.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/models/gr_clean.py` & `citation_docket-0.1.3/citation_docket/regexes/models/gr_clean.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/models/misc/extra.py` & `citation_docket-0.1.3/citation_docket/regexes/models/misc/extra.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/regexes/models/misc/num.py` & `citation_docket-0.1.3/citation_docket/regexes/models/misc/num.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/sc_website_2023.py` & `citation_docket-0.1.3/citation_docket/sc_website_2023.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/citation_docket/simple_matcher.py` & `citation_docket-0.1.3/citation_docket/simple_matcher.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.2/pyproject.toml` & `citation_docket-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation_docket"
-version = "0.1.2"
+version = "0.1.3"
 description = "Regex formula of Philippine Supreme Court citations in docket format, i.e. GR, AM, AC, BM."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-docket"
 documentation = "https://justmars.github.io/citation-docket"
 classifiers = [
@@ -15,29 +15,31 @@
   "Intended Audience :: Legal Industry",
   "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-citation_report = "^0.1.2"
+citation_report = "^0.1.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
-mkdocs-material = "^9.0.14"
-ipython = "^8.10.0"
+mkdocs-material = "^9.1"
 
-[tool.pytest]
-minversion = "7.2"
-addopts = "-ra -q --cov=citation_docket tests/"
-testpaths = ["tests"]
+[tool.pytest.ini_options]
+minversion = "7.3"
+addopts = "-ra -q --doctest-modules --cov"
+filterwarnings = [
+  "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
+]
+testpaths = ["tests", "citation_docket"]
 
 [tool.ruff]
 ignore = ["F401"]
 
 [tool.black]
 line-length = 79
 include = '.pyi?$'
```

### Comparing `citation_docket-0.1.2/PKG-INFO` & `citation_docket-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-docket
-Version: 0.1.2
+Version: 0.1.3
 Summary: Regex formula of Philippine Supreme Court citations in docket format, i.e. GR, AM, AC, BM.
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,10 +13,10 @@
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
-Requires-Dist: citation_report (>=0.1.2,<0.2.0)
+Requires-Dist: citation_report (>=0.1.3,<0.2.0)
 Project-URL: Documentation, https://justmars.github.io/citation-docket
 Project-URL: Repository, https://github.com/justmars/citation-docket
```

