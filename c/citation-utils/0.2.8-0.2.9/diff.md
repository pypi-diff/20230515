# Comparing `tmp/citation_utils-0.2.8.tar.gz` & `tmp/citation_utils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_utils-0.2.8.tar", max compression
+gzip compressed data, was "citation_utils-0.2.9.tar", max compression
```

## Comparing `citation_utils-0.2.8.tar` & `citation_utils-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       70 2023-03-07 12:44:35.024460 citation_utils-0.2.8/citation_utils/__init__.py
--rw-r--r--   0        0        0     2566 2023-03-06 01:26:55.330877 citation_utils-0.2.8/citation_utils/db.py
--rw-r--r--   0        0        0     1580 2023-02-25 08:59:18.991399 citation_utils-0.2.8/citation_utils/helpers.py
--rw-r--r--   0        0        0    17343 2023-03-07 13:21:42.478886 citation_utils-0.2.8/citation_utils/main.py
--rw-r--r--   0        0        0      541 2022-11-20 00:05:42.227549 citation_utils-0.2.8/citation_utils/sql/legacy/multiple_cat_idx.sql
--rw-r--r--   0        0        0     1653 2023-03-07 12:44:28.354815 citation_utils-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 citation_utils-0.2.8/setup.py
--rw-r--r--   0        0        0     1039 1970-01-01 00:00:00.000000 citation_utils-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-05-15 16:32:51.983670 citation_utils-0.2.9/citation_utils/__init__.py
+-rw-r--r--   0        0        0     2566 2023-03-06 01:26:55.330877 citation_utils-0.2.9/citation_utils/db.py
+-rw-r--r--   0        0        0     1580 2023-02-25 08:59:18.991399 citation_utils-0.2.9/citation_utils/helpers.py
+-rw-r--r--   0        0        0    17514 2023-05-15 16:39:38.638376 citation_utils-0.2.9/citation_utils/main.py
+-rw-r--r--   0        0        0      541 2022-11-20 00:05:42.227549 citation_utils-0.2.9/citation_utils/sql/legacy/multiple_cat_idx.sql
+-rw-r--r--   0        0        0     1443 2023-05-15 16:32:42.500144 citation_utils-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1039 1970-01-01 00:00:00.000000 citation_utils-0.2.9/PKG-INFO
```

### Comparing `citation_utils-0.2.8/citation_utils/db.py` & `citation_utils-0.2.9/citation_utils/db.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.2.8/citation_utils/helpers.py` & `citation_utils-0.2.9/citation_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.2.8/citation_utils/main.py` & `citation_utils-0.2.9/citation_utils/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,18 @@
     None | `phil` | optional (str) | combined `volume` Phil. `page`
     342 SCRA 449 | `scra` | optional (str) | combined `volume` SCRA `page`
     None | `offg` | optional (str) | combined `volume` O.G. `page`
 
     Examples:
         >>> text1 = "GR Nos. L-15756; L-15818;  L-16200 and L-16201, Dec. 29, 1962"
         >>> cite1 = next(Citation.extract_citations(text1))
-        Citation(docket_category='GR', docket_serial='L-15756', docket_date=datetime.date(1962, 12, 29), docket='GR L-15756, Dec. 29, 1962', phil=None, scra=None, offg=None)
+        >>> cite1 == Citation(docket_category='GR', docket_serial='L-15756', docket_date=datetime.date(1962, 12, 29), docket='GR L-15756, Dec. 29, 1962', phil=None, scra=None, offg=None)
+        True
         >>> cite1.storage_prefix
-        'GR/1962/L-15756/12/29'
+        'gr/l-15756/1962/12/29'
 
     Note that the fields contain a `col` and `index`. These are populated as extra
     Pydantic fields in anticipation of [sqlpyd](https://github.com/justmars/sqlpyd) for
     database processing. Relatedly, the `@slug` can be used as primary key based on
     the consolidated fields.
     """  # noqa: E501
 
@@ -77,17 +78,15 @@
         description="Serialized identifier of docket category.",
         col=str,
         index=True,
     )
     docket_date: datetime.date | None = Field(
         None,
         title="Docket Date",
-        description=(
-            "Distinguishes same category and serial decisions by issuance."
-        ),
+        description="Distinguishes same category and serial decisions by issuance.",
         col=datetime.date,
         index=True,
     )
     docket: str | None = Field(
         None,
         title="Docket Reference",
         description="Clean parts: category, a single serial id, and date.",
@@ -169,16 +168,16 @@
         Examples:
             >>> text = "AM 07-115-CA-J and CA-08-46-J, Aug. 19, 2008"
             >>> cite = next(Citation.extract_citations(text))
             >>> cite.slug
             'am-07-115-ca-j-aug-19-2008'
             >>> data = {"date_prom": "1985-04-24", "docket": "General Register L-63915, April 24, 1985", "orig_idx": "GR No. L-63915", "phil": "220 Phil. 422", "scra": "136 SCRA 27", "offg": None}
             >>> other_cite = Citation.extract_citation_from_data(data)
-            >>> other_cite
-            'gr-l-63915-apr-24-1985-136-scra-27-220-phil-422'
+            >>> other_cite == Citation(docket_category='GR', docket_serial='L-63915', docket_date=datetime.date(1985, 4, 24), docket='GR L-63915, Apr. 24, 1985', phil='220 Phil. 422', scra='136 SCRA 27', offg=None)
+            True
 
         """  # noqa: E501
         if self.has_citation:
             return slugify(" ".join(self.has_citation)).strip()
         return None
 
     def join_elements(self, separator: str) -> str | None:
@@ -245,15 +244,15 @@
         and `slug` is `prefix_db_key` only relates to citations which
         have dockets.
 
         Examples:
             >>> text = "AM 07-115-CA-J and CA-08-46-J, Aug. 19, 2008"
             >>> cite = next(Citation.extract_citations(text))
             >>> cite.storage_prefix
-            'am.07-115-ca-j.2008.8.19'
+            'am/07-115-ca-j/2008/8/19'
 
         Returns:
             str | None: Should only work if the docket citation is available.
 
         """
         return self.join_elements(separator=".")
 
@@ -292,18 +291,16 @@
         cls, data: dict
     ) -> tuple[str, str, Self] | None:
         """Shortcut to determine viability of unique identifiers for a decision
         based on the same dictionary passed to `extract_citation_from_data()`
 
         Examples:
             >>> data = {"date_prom": "1985-04-24", "docket": "General Register L-63915, April 24, 1985", "orig_idx": "GR No. L-63915", "phil": "220 Phil. 422", "scra": "136 SCRA 27", "offg": None}
-            >>> Citation.extract_id_prefix_citation_from_data(data)
-            ('gr.l-63915.1985.4.24',
-            'gr/l-63915/1985/4/24',
-            Citation(docket_category='GR', docket_serial='L-63915', docket_date=datetime.date(1985, 4, 24), docket='GR L-63915, Apr. 24, 1985', phil='220 Phil. 422', scra='136 SCRA 27', offg=None))
+            >>> Citation.extract_id_prefix_citation_from_data(data) == ('gr.l-63915.1985.4.24', 'gr/l-63915/1985/4/24', Citation(docket_category='GR', docket_serial='L-63915', docket_date=datetime.date(1985, 4, 24), docket='GR L-63915, Apr. 24, 1985', phil='220 Phil. 422', scra='136 SCRA 27', offg=None))
+            True
 
         Args:
             data (dict): Dict loaded from a details.yaml file with relevant fields. See
                 `extract_citation_from_data()`
 
         Returns:
             tuple[str, str, Self] | None: Docket-based identifiers of the decision based on data dict.
@@ -327,16 +324,17 @@
     @classmethod
     def extract_citations(cls, text: str) -> Iterator[Self]:
         """Combine `Docket`s (which have `Reports`), and filtered `Report` models,
         if they exist.
 
         Examples:
             >>> text = "<em>Gatchalian Promotions Talent Pool, Inc. v. Atty. Naldoza</em>, 374 Phil 1, 10-11 (1999), citing: <em>In re Almacen</em>, 31 SCRA 562, 600 (1970).; People v. Umayam, G.R. No. 147033, April 30, 2003; <i>Bagong Alyansang Makabayan v. Zamora,</i> G.R. Nos. 138570, 138572, 138587, 138680, 138698, October 10, 2000, 342 SCRA 449; Villegas <em>v.</em> Subido, G.R. No. 31711, Sept. 30, 1971, 41 SCRA 190;"
-            >>> [c.dict(exclude_none=True) for c in Citation.extract_citations(text)]
-            [{'docket_category': 'GR', 'docket_serial': '147033', 'docket_date': datetime.date(2003, 4, 30), 'docket': 'GR 147033, Apr. 30, 2003'}, {'docket_category': 'GR', 'docket_serial': '138570', 'docket_date': datetime.date(2000, 10, 10), 'docket': 'GR 138570, Oct. 10, 2000', 'scra': '342 SCRA 449'}, {'docket_category': 'GR', 'docket_serial': '31711', 'docket_date': datetime.date(1971, 9, 30), 'docket': 'GR 31711, Sep. 30, 1971', 'scra': '41 SCRA 190'}, {'scra': '31 SCRA 562'}, {'phil': '374 Phil 1'}]
+            >>> results = [c.dict(exclude_none=True) for c in Citation.extract_citations(text)]
+            >>> results == [{'docket_category': 'GR', 'docket_serial': '147033', 'docket_date': datetime.date(2003, 4, 30), 'docket': 'GR 147033, Apr. 30, 2003'}, {'docket_category': 'GR', 'docket_serial': '138570', 'docket_date': datetime.date(2000, 10, 10), 'docket': 'GR 138570, Oct. 10, 2000', 'scra': '342 SCRA 449'}, {'docket_category': 'GR', 'docket_serial': '31711', 'docket_date': datetime.date(1971, 9, 30), 'docket': 'GR 31711, Sep. 30, 1971', 'scra': '41 SCRA 190'}, {'scra': '31 SCRA 562'}, {'phil': '374 Phil 1'}]
+            True
 
         Yields:
             Iterator[Self]: Matching Citations found in the text.
         """  # noqa: E501
         from .helpers import filtered_reports
 
         def extract_report(obj):
```

### Comparing `citation_utils-0.2.8/citation_utils/sql/legacy/multiple_cat_idx.sql` & `citation_utils-0.2.9/citation_utils/sql/legacy/multiple_cat_idx.sql`

 * *Files identical despite different names*

### Comparing `citation_utils-0.2.8/pyproject.toml` & `citation_utils-0.2.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation-utils"
-version = "0.2.8"
+version = "0.2.9"
 description = "Regex-based docket- and report- styled citations based on Philippine Supreme Court decisions."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-utils"
 documentation = "https://justmars.github.io/citation-utils"
 classifiers = [
@@ -15,57 +15,38 @@
   "Intended Audience :: Legal Industry",
   "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-citation-docket = "^0.1.2"
+citation-docket = "^0.1.3"
 python-slugify = "^8.0"
-sqlite-utils = "^3.30"
+sqlite-utils = "^3.31"
 loguru = "^0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3"
 pytest = "^7.2"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 types-Markdown = "^3.4.0"
 types-PyYAML = "^6.0.7"
 types-python-slugify = "^5.0.4"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.1"
-ipython = "^8.11.0"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 filterwarnings = ['ignore::DeprecationWarning']
-addopts = "-ra -q --doctest-modules --cov=citation_utils tests/"
-testpaths = ["tests"]
+addopts = "-ra -q --doctest-modules --cov"
+testpaths = ["tests", "citation_utils"]
 
 [tool.ruff]
 ignore = ["F401"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
 
-[tool.black]
-line-length = 79
-include = '.pyi?$'
-exclude = '''
-/(
-    .git
-    | .hg
-    | .mypy_cache
-    | .tox
-    | .venv
-    | _build
-    | buck-out
-    | build
-    | dist
-)/
-'''
-
-
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `citation_utils-0.2.8/PKG-INFO` & `citation_utils-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Regex-based docket- and report- styled citations based on Philippine Supreme Court decisions.
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,13 +13,13 @@
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
-Requires-Dist: citation-docket (>=0.1.2,<0.2.0)
+Requires-Dist: citation-docket (>=0.1.3,<0.2.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: python-slugify (>=8.0,<9.0)
-Requires-Dist: sqlite-utils (>=3.30,<4.0)
+Requires-Dist: sqlite-utils (>=3.31,<4.0)
 Project-URL: Documentation, https://justmars.github.io/citation-utils
 Project-URL: Repository, https://github.com/justmars/citation-utils
```

