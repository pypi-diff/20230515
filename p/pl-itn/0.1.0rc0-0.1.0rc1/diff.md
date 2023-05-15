# Comparing `tmp/pl_itn-0.1.0rc0.tar.gz` & `tmp/pl_itn-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pl_itn-0.1.0rc0.tar", last modified: Sat Apr  8 19:11:31 2023, max compression
+gzip compressed data, was "pl_itn-0.1.0rc1.tar", last modified: Mon May 15 08:24:30 2023, max compression
```

## Comparing `pl_itn-0.1.0rc0.tar` & `pl_itn-0.1.0rc1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      162 2023-02-19 12:25:07.227843 pl_itn-0.1.0rc0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-02-19 11:26:57.797584 pl_itn-0.1.0rc0/LICENSE
--rw-r--r--   0        0        0    11357 2023-02-19 11:26:57.797584 pl_itn-0.1.0rc0/LICENSE
--rw-r--r--   0        0        0     2504 2023-04-08 17:29:01.946988 pl_itn-0.1.0rc0/README.md
--rw-r--r--   0        0        0     2504 2023-04-08 17:29:01.946988 pl_itn-0.1.0rc0/README.md
--rw-r--r--   0        0        0       92 2023-03-25 22:22:05.615323 pl_itn-0.1.0rc0/pl_itn/__init__.py
--rw-r--r--   0        0        0     2602 2023-04-08 09:44:45.039041 pl_itn-0.1.0rc0/pl_itn/__main__.py
--rw-r--r--   0        0        0      126 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-19 13:35:28.311455 pl_itn-0.1.0rc0/pl_itn/grammars/__init__.py
--rw-r--r--   0        0        0  1217770 2023-02-19 13:34:04.504228 pl_itn-0.1.0rc0/pl_itn/grammars/tagger.fst
--rw-r--r--   0        0        0   104302 2023-02-19 13:34:04.596228 pl_itn-0.1.0rc0/pl_itn/grammars/verbalizer.fst
--rw-r--r--   0        0        0      685 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/logging.py
--rw-r--r--   0        0        0       34 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/src/__init__.py
--rw-r--r--   0        0        0     2486 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/src/normalize.py
--rw-r--r--   0        0        0     1571 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/src/parse.py
--rw-r--r--   0        0        0     2408 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/src/permute.py
--rw-r--r--   0        0        0     1609 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/src/restore_uppercase.py
--rw-r--r--   0        0        0     3877 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/src/restore_whitespace.py
--rw-r--r--   0        0        0      276 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/src/tag.py
--rw-r--r--   0        0        0      424 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/src/utils.py
--rw-r--r--   0        0        0      646 2023-03-25 22:22:05.619323 pl_itn-0.1.0rc0/pl_itn/src/verbalize.py
--rw-r--r--   0        0        0     3811 2023-04-08 19:11:31.048508 pl_itn-0.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 pl_itn-0.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      162 2023-05-05 16:10:37.295418 pl_itn-0.1.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-02-19 11:26:57.797584 pl_itn-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0    11357 2023-02-19 11:26:57.797584 pl_itn-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     4810 2023-05-13 10:04:31.433713 pl_itn-0.1.0rc1/README.md
+-rw-r--r--   0        0        0     4810 2023-05-13 10:04:31.433713 pl_itn-0.1.0rc1/README.md
+-rw-r--r--   0        0        0      130 2023-05-13 07:09:30.399348 pl_itn-0.1.0rc1/pl_itn/__init__.py
+-rw-r--r--   0        0        0     2374 2023-05-13 07:17:32.876934 pl_itn-0.1.0rc1/pl_itn/__main__.py
+-rw-r--r--   0        0        0      126 2023-05-05 16:10:37.295418 pl_itn-0.1.0rc1/pl_itn/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:10:37.295418 pl_itn-0.1.0rc1/pl_itn/grammars/__init__.py
+-rw-r--r--   0        0        0  4083774 2023-05-15 08:21:25.977626 pl_itn-0.1.0rc1/pl_itn/grammars/tagger.fst
+-rw-r--r--   0        0        0   104302 2023-05-15 08:21:26.081626 pl_itn-0.1.0rc1/pl_itn/grammars/verbalizer.fst
+-rw-r--r--   0        0        0      685 2023-05-05 16:10:37.303418 pl_itn-0.1.0rc1/pl_itn/logging.py
+-rw-r--r--   0        0        0       76 2023-05-13 07:09:30.399348 pl_itn-0.1.0rc1/pl_itn/src/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-13 07:09:30.399348 pl_itn-0.1.0rc1/pl_itn/src/grammar.py
+-rw-r--r--   0        0        0     2944 2023-05-13 07:09:30.399348 pl_itn-0.1.0rc1/pl_itn/src/normalize.py
+-rw-r--r--   0        0        0     1520 2023-05-13 07:09:30.399348 pl_itn-0.1.0rc1/pl_itn/src/parse.py
+-rw-r--r--   0        0        0     2408 2023-05-13 07:09:30.399348 pl_itn-0.1.0rc1/pl_itn/src/permute.py
+-rw-r--r--   0        0        0     1548 2023-05-13 07:09:30.399348 pl_itn-0.1.0rc1/pl_itn/src/restore_uppercase.py
+-rw-r--r--   0        0        0     3738 2023-05-13 07:09:30.399348 pl_itn-0.1.0rc1/pl_itn/src/restore_whitespace.py
+-rw-r--r--   0        0        0      276 2023-05-05 16:10:37.303418 pl_itn-0.1.0rc1/pl_itn/src/tag.py
+-rw-r--r--   0        0        0      572 2023-05-13 07:09:30.399348 pl_itn-0.1.0rc1/pl_itn/src/utils.py
+-rw-r--r--   0        0        0      818 2023-05-13 10:04:31.457712 pl_itn-0.1.0rc1/pl_itn/src/verbalize.py
+-rw-r--r--   0        0        0     2980 2023-05-15 08:24:30.461214 pl_itn-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5781 1970-01-01 00:00:00.000000 pl_itn-0.1.0rc1/PKG-INFO
```

### Comparing `pl_itn-0.1.0rc0/LICENSE` & `pl_itn-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pl_itn-0.1.0rc0/pl_itn/__main__.py` & `pl_itn-0.1.0rc1/pl_itn/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import argparse
+import yaml
 from pathlib import Path
 from signal import signal, SIGINT, SIGTERM
 
-import yaml
-
 from pl_itn import Normalizer, package_root
-from pl_itn.logging import ITN_logger
 from pl_itn.exceptions import InterruptException, gentle_interrupt_handler
-
+from pl_itn.logging import ITN_logger
 
 def main():
     args = parser()
 
     itn_logger = ITN_logger("pl_itn")
     itn_logger.set_level(args.log_level)
 
     if args.config:
-        with args.config.open() as f:
-            config = yaml.safe_load(f)
+        with args.config.open() as config_file:
+            config = yaml.safe_load(config_file)
         args.tagger = Path(config.get("out_dir")) / config.get("tagger_fname")
         args.verbalizer = Path(config.get("out_dir")) / config.get("verbalizer_fname")
 
     normalizer = Normalizer(
         tagger_fst_path=args.tagger,
         verbalizer_fst_path=args.verbalizer,
-        debug_mode=args.debug_mode,
     )
 
     if args.interactive:
         run_interactive(normalizer)
     else:
         run_single(normalizer, args.text)
 
@@ -54,22 +51,15 @@
         "--verbalizer", type=Path, default=(package_root / "grammars/verbalizer.fst")
     )
     parser.add_argument(
         "--config",
         type=Path,
         help="Optionally provide yaml config with tagger and verbalizer paths.",
     )
-
     parser.add_argument("--log-level", choices=["debug", "info"], default="info")
-    parser.add_argument(
-        "-d",
-        "--debug-mode",
-        action="store_true",
-        help="If used, process will be interrupted on runtime errors, else it will return a step back value.",
-    )
 
     return parser.parse_args()
 
 
 def run_interactive(normalizer: Normalizer):
     signal(SIGINT, gentle_interrupt_handler)  # keyboard interrupt
     signal(SIGTERM, gentle_interrupt_handler)  # terminal interrupt
```

### Comparing `pl_itn-0.1.0rc0/pl_itn/grammars/verbalizer.fst` & `pl_itn-0.1.0rc1/pl_itn/grammars/verbalizer.fst`

 * *Files identical despite different names*

### Comparing `pl_itn-0.1.0rc0/pl_itn/logging.py` & `pl_itn-0.1.0rc1/pl_itn/logging.py`

 * *Files identical despite different names*

### Comparing `pl_itn-0.1.0rc0/pl_itn/src/normalize.py` & `pl_itn-0.1.0rc1/pl_itn/src/normalize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,91 @@
 import logging
-from pathlib import Path
 import pynini
+from pathlib import Path
 
+from pl_itn.src.grammar import Grammar, GrammarType
 from pl_itn.src.tag import tag
 from pl_itn.src.parse import parse_tokens
 from pl_itn.src.permute import generate_permutations
-from pl_itn.src.verbalize import verbalize
-from pl_itn.src.restore_whitespace import restore_whitespaces
 from pl_itn.src.restore_uppercase import restore_uppercase
+from pl_itn.src.restore_whitespace import restore_whitespaces
+from pl_itn.src.tag import tag
 from pl_itn.src.utils import pre_process, post_process
+from pl_itn.src.verbalize import verbalize
 
 logger = logging.getLogger(__name__)
 
 package_root = Path(__file__).parents[1]
 
 
+class NormalizationError(Exception):
+    ...
+
+
 class Normalizer:
     def __init__(
         self,
         tagger_fst_path: Path = package_root / "grammars/tagger.fst",
         verbalizer_fst_path: Path = package_root / "grammars/verbalizer.fst",
-        debug_mode: bool = False,
     ):
-        self._tagger_fst = pynini.Fst.read(str(tagger_fst_path))
-        self._verbalizer_fst = pynini.Fst.read(str(verbalizer_fst_path))
-        self.debug_mode = debug_mode
+        self._tagger = Grammar(tagger_fst_path, GrammarType.TAGGER)
+        self._verbalizer = Grammar(verbalizer_fst_path, GrammarType.VERBALIZER)
 
     @property
-    def tagger_fst(self):
-        return self._tagger_fst
+    def tagger(self):
+        return self._tagger
 
     @property
-    def verbalizer_fst(self):
-        return self._verbalizer_fst
+    def verbalizer(self):
+        return self._verbalizer
+
+    def set_grammar(
+        self, grammar_fst_path: Path, grammar_type: GrammarType, description: str = ""
+    ):
+        if grammar_type == GrammarType.TAGGER:
+            self._tagger = Grammar(grammar_fst_path, GrammarType.TAGGER, description)
+        else:
+            self._verbalizer = Grammar(
+                grammar_fst_path, GrammarType.VERBALIZER, description
+            )
+
+    def __call__(self, text: str) -> str:
+        return self.normalize(text)
 
     def normalize(self, text: str) -> str:
         logger.debug(f"input: {text}")
 
         preprocessed_text = pre_process(text)
 
         if not preprocessed_text:
             logger.info("Empty input string")
             return text
 
         logger.debug(f"pre_process(): {preprocessed_text}")
 
         try:
-            tagged_text = tag(self.tagger_fst, preprocessed_text)
+            tagged_text = tag(self.tagger.fst, preprocessed_text)
             logger.debug(f"tag(): {tagged_text}")
 
             tokens = parse_tokens(tagged_text)
             logger.debug(f"parse(): {tokens}")
 
             tags_reordered = generate_permutations(tokens)
             logger.debug(f"generate_permutations(): {tags_reordered}")
 
-            verbalized_text = verbalize(self.verbalizer_fst, tags_reordered)
+            verbalized_text = verbalize(self.verbalizer.fst, tags_reordered)
             logger.debug(f"verbalize(): {verbalized_text}")
 
             postprocessed_text = post_process(verbalized_text)
             logger.debug(f"post_process(): {postprocessed_text}")
 
             uppercase_restored = restore_uppercase(text, postprocessed_text)
             logger.debug(f"restore_uppercase(): {uppercase_restored}")
 
             whitespaces_restored = restore_whitespaces(text, uppercase_restored, tokens)
             logger.debug(f"restore_whitespaces(): {whitespaces_restored}")
 
             return whitespaces_restored
 
-        except ValueError as e:
+        except Exception as e:
             logger.error(e)
-            if self.debug_mode:
-                raise
-            else:
-                return text
+            raise NormalizationError(e)
```

### Comparing `pl_itn-0.1.0rc0/pl_itn/src/parse.py` & `pl_itn-0.1.0rc1/pl_itn/src/parse.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from collections import OrderedDict
 import re
+from collections import OrderedDict
 from typing import List
 
 """
 Parses tokenized/classified text, e.g. 
 'tokens { money { integer: "20" currency: "$" } } tokens { name: "left"}'
 
 Args
@@ -37,16 +37,15 @@
     text = _strip_braces_and_whitespaces(text)
     keywords = re.findall(r"(\S+): ", text)
     values = re.findall(r"\"([^\"]+)\"", text)
 
     if len(keywords) != len(values):
         raise ValueError("Parsing tagged text into tokens failed.")
 
-    for index, keyword in enumerate(keywords):
-        yield ((keyword, values[index]))
+    yield from zip(keywords, values)
 
 
 def _parse_recursively(text):
     text = _strip_braces_and_whitespaces(text)
     current_level_dict = OrderedDict()
 
     if "{" not in text:  # no nested dict
```

### Comparing `pl_itn-0.1.0rc0/pl_itn/src/permute.py` & `pl_itn-0.1.0rc1/pl_itn/src/permute.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from collections import OrderedDict
 import itertools
+from collections import OrderedDict
 from typing import List
 
 
 def generate_permutations(tokens: List[dict]):
     """
     Initiate generate_permutations_recursive() on tokens
     with no processed_left_string.
```

### Comparing `pl_itn-0.1.0rc0/pl_itn/src/restore_uppercase.py` & `pl_itn-0.1.0rc1/pl_itn/src/restore_uppercase.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         nonlocal original_index
         original_index += 1
         return not finished()  # False if index out of range
 
     def next_normalized_index():
         nonlocal normalized_index
         normalized_index += 1
-        return not finished()  # False if index out of range
 
     def restore():
         restored[normalized_index] = original[original_index]
         next_original_index()
         next_normalized_index()
 
     while not finished():
```

### Comparing `pl_itn-0.1.0rc0/pl_itn/src/restore_whitespace.py` & `pl_itn-0.1.0rc1/pl_itn/src/restore_whitespace.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,19 +69,15 @@
 
             if maybe_get_whitespace(original, index_original + 1):
                 # Include trailing whitespace to the processed part
                 index_original += 1
 
             # Remove processed input
             def slice_head(input_list, index):
-                try:
-                    output_list = input_list[index + 1 :]
-                except IndexError:
-                    output_list = []
-                return output_list
+                return input_list[index + 1 :]
 
             normalized = slice_head(normalized, index_normalized)
             normalized_lower = slice_head(normalized_lower, index_normalized)
             original = slice_head(original, index_original)
             original_lower = slice_head(original_lower, index_original)
 
     restored += " ".join(normalized)
```

### Comparing `pl_itn-0.1.0rc0/pyproject.toml` & `pl_itn-0.1.0rc1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "setuptools>=62.3.3",
     "markdown-exec>=0.7.0",
     "mkdocs-redirects>=1.2.0",
 ]
 workflow = [
     "pdm-pep517>=1.0.0,<2.0.0",
     "parver>=0.3.1",
-    "towncrier>=20",
     "pycomplete~=0.3",
 ]
 
 [tool.black]
 line-length = 120
 target-version = [
     "py37",
@@ -92,32 +91,14 @@
 max-complexity = 10
 
 [tool.ruff.isort]
 known-first-party = [
     "pdm",
 ]
 
-[tool.towncrier]
-package = "pl_itn"
-filename = "CHANGELOG.md"
-issue_format = "[#{issue}](https://github.com/mstopa/pl_itn/issues/{issue})"
-directory = "news/"
-title_format = "Release v{version} ({project_date})"
-template = "news/towncrier_template.md"
-underlines = "-~^"
-type = [
-    { directory = "break", name = "Breaking Changes", showcontent = true },
-    { directory = "feature", name = "Features & Improvements", showcontent = true },
-    { directory = "bugfix", name = "Bug Fixes", showcontent = true },
-    { directory = "doc", name = "Documentation", showcontent = true },
-    { directory = "dep", name = "Dependencies", showcontent = true },
-    { directory = "removal", name = "Removals and Deprecations", showcontent = true },
-    { directory = "misc", name = "Miscellany", showcontent = true },
-]
-
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning",
 ]
 markers = [
     "network: Tests that require network",
     "integration: Run with all Python versions",
@@ -132,15 +113,15 @@
 [project]
 name = "pl_itn"
 description = "Polish FST Inverse Text Normalization"
 authors = [
     { name = "mstopa" },
     { name = "cansubmarinesswim" },
 ]
-version = "0.1.0rc0"
+version = "0.1.0-rc1"
 requires-python = ">=3.7"
 dependencies = [
     "pynini>=2.1.4",
     "pyyaml>=6.0",
 ]
 readme = "README.md"
 keywords = [
```

