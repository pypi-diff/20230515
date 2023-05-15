# Comparing `tmp/statute_patterns-0.2.3.tar.gz` & `tmp/statute_patterns-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_patterns-0.2.3.tar", max compression
+gzip compressed data, was "statute_patterns-0.2.4.tar", max compression
```

## Comparing `statute_patterns-0.2.3.tar` & `statute_patterns-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      540 2023-01-24 05:16:45.918551 statute_patterns-0.2.3/README.md
--rw-r--r--   0        0        0     1597 2023-05-15 16:43:15.557380 statute_patterns-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      413 2023-05-15 16:43:31.621286 statute_patterns-0.2.3/statute_patterns/__init__.py
--rw-r--r--   0        0        0     2587 2023-03-06 01:38:57.132031 statute_patterns-0.2.3/statute_patterns/__main__.py
--rw-r--r--   0        0        0      347 2022-11-15 05:02:57.881610 statute_patterns-0.2.3/statute_patterns/components/__init__.py
--rw-r--r--   0        0        0     9606 2023-03-05 05:22:13.847839 statute_patterns-0.2.3/statute_patterns/components/category.py
--rw-r--r--   0        0        0     3232 2023-03-05 05:24:24.768020 statute_patterns-0.2.3/statute_patterns/components/details.py
--rw-r--r--   0        0        0     9174 2023-03-05 05:26:48.589297 statute_patterns-0.2.3/statute_patterns/components/rule.py
--rw-r--r--   0        0        0     2015 2022-12-30 06:17:42.944342 statute_patterns-0.2.3/statute_patterns/components/short.py
--rw-r--r--   0        0        0     2681 2023-03-05 05:24:31.413742 statute_patterns-0.2.3/statute_patterns/components/utils.py
--rw-r--r--   0        0        0     5369 2023-03-05 05:24:24.782830 statute_patterns-0.2.3/statute_patterns/models.py
--rw-r--r--   0        0        0     4617 2023-01-23 14:00:20.449616 statute_patterns-0.2.3/statute_patterns/names.py
--rw-r--r--   0        0        0      249 2022-11-15 04:58:03.940842 statute_patterns-0.2.3/statute_patterns/recipes/__init__.py
--rw-r--r--   0        0        0      380 2022-11-07 05:50:23.161499 statute_patterns-0.2.3/statute_patterns/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-03-05 05:24:53.354912 statute_patterns-0.2.3/statute_patterns/recipes/digits.py
--rw-r--r--   0        0        0      311 2022-11-07 05:50:23.161594 statute_patterns-0.2.3/statute_patterns/recipes/roc.py
--rw-r--r--   0        0        0      550 2022-11-07 05:50:23.161690 statute_patterns-0.2.3/statute_patterns/recipes/spain.py
--rw-r--r--   0        0        0     6553 2023-03-05 05:25:51.543676 statute_patterns-0.2.3/statute_patterns/serials.py
--rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 statute_patterns-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      540 2023-01-24 05:16:45.918551 statute_patterns-0.2.4/README.md
+-rw-r--r--   0        0        0     1558 2023-05-15 16:47:38.581464 statute_patterns-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      413 2023-05-15 16:46:04.262159 statute_patterns-0.2.4/statute_patterns/__init__.py
+-rw-r--r--   0        0        0     2587 2023-03-06 01:38:57.132031 statute_patterns-0.2.4/statute_patterns/__main__.py
+-rw-r--r--   0        0        0      347 2022-11-15 05:02:57.881610 statute_patterns-0.2.4/statute_patterns/components/__init__.py
+-rw-r--r--   0        0        0     9606 2023-03-05 05:22:13.847839 statute_patterns-0.2.4/statute_patterns/components/category.py
+-rw-r--r--   0        0        0     3232 2023-03-05 05:24:24.768020 statute_patterns-0.2.4/statute_patterns/components/details.py
+-rw-r--r--   0        0        0     9042 2023-05-15 16:46:07.217824 statute_patterns-0.2.4/statute_patterns/components/rule.py
+-rw-r--r--   0        0        0     2015 2022-12-30 06:17:42.944342 statute_patterns-0.2.4/statute_patterns/components/short.py
+-rw-r--r--   0        0        0     2673 2023-05-15 16:46:07.189845 statute_patterns-0.2.4/statute_patterns/components/utils.py
+-rw-r--r--   0        0        0     5339 2023-05-15 16:46:07.197213 statute_patterns-0.2.4/statute_patterns/models.py
+-rw-r--r--   0        0        0     4617 2023-01-23 14:00:20.449616 statute_patterns-0.2.4/statute_patterns/names.py
+-rw-r--r--   0        0        0      249 2022-11-15 04:58:03.940842 statute_patterns-0.2.4/statute_patterns/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2022-11-07 05:50:23.161499 statute_patterns-0.2.4/statute_patterns/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-03-05 05:24:53.354912 statute_patterns-0.2.4/statute_patterns/recipes/digits.py
+-rw-r--r--   0        0        0      311 2022-11-07 05:50:23.161594 statute_patterns-0.2.4/statute_patterns/recipes/roc.py
+-rw-r--r--   0        0        0      550 2022-11-07 05:50:23.161690 statute_patterns-0.2.4/statute_patterns/recipes/spain.py
+-rw-r--r--   0        0        0     6553 2023-03-05 05:25:51.543676 statute_patterns-0.2.4/statute_patterns/serials.py
+-rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 statute_patterns-0.2.4/PKG-INFO
```

### Comparing `statute_patterns-0.2.3/README.md` & `statute_patterns-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.3/pyproject.toml` & `statute_patterns-0.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-patterns"
-version = "0.2.3"
+version = "0.2.4"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-patterns"
 documentation = "https://justmars.github.io/statute-patterns"
@@ -37,35 +37,21 @@
 types-python-dateutil = "^2.8.19.2"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.1.0"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
-addopts = "--doctest-modules"
-testpaths = ["tests"]
+addopts = "-ra -q --doctest-modules --cov"
+filterwarnings = [
+  "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
+]
+testpaths = ["tests", "statute_patterns"]
 
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
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `statute_patterns-0.2.3/statute_patterns/__main__.py` & `statute_patterns-0.2.4/statute_patterns/__main__.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.3/statute_patterns/components/category.py` & `statute_patterns-0.2.4/statute_patterns/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.3/statute_patterns/components/details.py` & `statute_patterns-0.2.4/statute_patterns/components/details.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.3/statute_patterns/components/rule.py` & `statute_patterns-0.2.4/statute_patterns/components/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     4. Serial title generated by [`StatuteSerialCategory.serialize()`][statute_patterns.components.category.StatuteSerialCategory.serialize]
     5. Countability via a `collection.Counter` built-in
     """  # noqa: E501
 
     cat: StatuteSerialCategory = Field(
         ...,
         title="Statute Category",
-        description=(
-            "Classification under the limited StatuteSerialCategory taxonomy."
-        ),
+        description="Classification under the limited StatuteSerialCategory taxonomy.",
     )
     id: constr(to_lower=True) = Field(  # type: ignore
         ...,
         title="Serial Identifier",
         description=(
             "Limited inclusion of identifiers, e.g. only a subset of Executive"
             " Orders, Letters of Instruction, Spanish Codes will be permitted."
@@ -150,17 +148,15 @@
         target = base_path / self.cat
         paths = target.glob(f"{self.id}-*/{DETAILS_FILE}")
         for variant_path in paths:
             if variant_path.exists():
                 targets.append(variant_path.parent)
         return targets
 
-    def extract_folders(
-        self, base_path: Path = STATUTE_PATH
-    ) -> Iterator[Path]:
+    def extract_folders(self, base_path: Path = STATUTE_PATH) -> Iterator[Path]:
         """Using the `category` and `id` of the object,
         get the possible folder paths."""
         if folder := self.get_path(base_path):
             yield folder
         else:
             if folders := self.get_paths(base_path):
                 yield from folders
@@ -183,23 +179,19 @@
 
         return None
 
 
 class BasePattern(BaseModel, abc.ABC):
     matches: list[str] = Field(
         default_factory=list,
-        description=(
-            "When supplied, text included _should_ match regex property."
-        ),
+        description="When supplied, text included _should_ match regex property.",
     )
     excludes: list[str] = Field(
         default_factory=list,
-        description=(
-            "When supplied, text included _should not_ match regex property."
-        ),
+        description="When supplied, text included _should not_ match regex property.",
     )
 
     class Config:
         use_enum_values = True
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
@@ -226,24 +218,22 @@
         regardless of it being a SerialPattern or a NamedPattern."""
         return re.compile(self.regex, re.X)
 
     def validate_matches(self) -> None:
         for example_text in self.matches:
             if not self.pattern.fullmatch(example_text):
                 raise ValueError(
-                    "Missing match but intended to be included:"
-                    f" {example_text}"
+                    f"Missing match but intended to be included: {example_text}"
                 )
 
     def validate_excludes(self) -> None:
         for example_text in self.excludes:
             if self.pattern.fullmatch(example_text):
                 raise ValueError(
-                    "Match found even if intended to be excluded:"
-                    f" {example_text}."
+                    f"Match found even if intended to be excluded: {example_text}."
                 )
 
 
 class BaseCollection(BaseModel, abc.ABC):
     """Whether a collection of Named or Serial patterns are instantiated,
     a `combined_regex` property and a `pattern` propery will be automatically
     created based on the collection of objects declared on instantiation
```

### Comparing `statute_patterns-0.2.3/statute_patterns/components/short.py` & `statute_patterns-0.2.4/statute_patterns/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.3/statute_patterns/components/utils.py` & `statute_patterns-0.2.4/statute_patterns/components/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 import yaml
 from dotenv import find_dotenv, load_dotenv
 
 load_dotenv(find_dotenv())
 
 
-STATUTE_PATH = (
-    Path().home().joinpath(os.getenv("STATUTE_PATH", "code/corpus/statutes"))
-)
+STATUTE_PATH = Path().home().joinpath(os.getenv("STATUTE_PATH", "code/corpus/statutes"))
 
 DETAILS_FILE = "details.yaml"
 
 UNITS_MONEY = [
     {
         "item": "Container 1",
         "content": "Appropriation laws are excluded.",
```

### Comparing `statute_patterns-0.2.3/statute_patterns/models.py` & `statute_patterns-0.2.4/statute_patterns/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,15 @@
     `excludes` | Usable in parametized tests to determine that the full pattern will not match | ["Republic Act No. 7160:", "RA 9337-"]
     """  # noqa: E501
 
     cat: StatuteSerialCategory = Field(
         ...,
         title="Statute Serial Category",
         description=(
-            "A type of rule from the taxonomy enumerated under"
-            " StatuteSerialCategory."
+            "A type of rule from the taxonomy enumerated under StatuteSerialCategory."
         ),
     )
     regex_bases: list[str] = Field(
         ...,
         title="Prefix Label in Regex",
         description=(
             "There are too many ways to express a category name. There is a"
@@ -86,16 +85,15 @@
             " the serial, can qualify for a serial rule."
         ),
     )
     regex_serials: list[str] = Field(
         ...,
         title="Serial Identifiers in Regex",
         description=(
-            "The possible values of serial numbers to be matched with the"
-            " regex_bases."
+            "The possible values of serial numbers to be matched with the regex_bases."
         ),
     )
 
     @property
     def lines(self) -> Iterator[str]:
         """Each regex string produced matches the serial rule. Note the line break
         needs to be retained so that when printing `@regex`, the result is organized.
```

### Comparing `statute_patterns-0.2.3/statute_patterns/names.py` & `statute_patterns-0.2.4/statute_patterns/names.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.3/statute_patterns/recipes/digits.py` & `statute_patterns-0.2.4/statute_patterns/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.3/statute_patterns/recipes/spain.py` & `statute_patterns-0.2.4/statute_patterns/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.3/statute_patterns/serials.py` & `statute_patterns-0.2.4/statute_patterns/serials.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.3/PKG-INFO` & `statute_patterns-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-patterns
-Version: 0.2.3
+Version: 0.2.4
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

