# Comparing `tmp/qualtrics_utils-0.5.2.tar.gz` & `tmp/qualtrics_utils-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualtrics_utils-0.5.2.tar", max compression
+gzip compressed data, was "qualtrics_utils-0.5.3.tar", max compression
```

## Comparing `qualtrics_utils-0.5.2.tar` & `qualtrics_utils-0.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1317 2023-05-15 17:53:52.951555 qualtrics_utils-0.5.2/README.md
--rw-r--r--   0        0        0      593 2023-05-15 17:54:36.098240 qualtrics_utils-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 17:54:25.042235 qualtrics_utils-0.5.2/qualtrics_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 17:42:52.914230 qualtrics_utils-0.5.2/qualtrics_utils/codebook/__init__.py
--rw-r--r--   0        0        0     6983 2023-05-15 17:30:20.944642 qualtrics_utils-0.5.2/qualtrics_utils/codebook/generate.py
--rw-r--r--   0        0        0     3498 2023-05-15 14:49:13.310183 qualtrics_utils-0.5.2/qualtrics_utils/codebook/map_columns.py
--rw-r--r--   0        0        0     9221 2023-05-15 17:37:33.348189 qualtrics_utils-0.5.2/qualtrics_utils/survey.py
--rw-r--r--   0        0        0      494 2023-05-15 17:46:11.216385 qualtrics_utils-0.5.2/qualtrics_utils/utils.py
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.2/setup.py
--rw-r--r--   0        0        0     2062 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1317 2023-05-15 17:53:52.951555 qualtrics_utils-0.5.3/README.md
+-rw-r--r--   0        0        0      593 2023-05-15 18:05:16.795064 qualtrics_utils-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 17:54:25.042235 qualtrics_utils-0.5.3/qualtrics_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 17:42:52.914230 qualtrics_utils-0.5.3/qualtrics_utils/codebook/__init__.py
+-rw-r--r--   0        0        0     6989 2023-05-15 17:56:40.451923 qualtrics_utils-0.5.3/qualtrics_utils/codebook/generate.py
+-rw-r--r--   0        0        0     3538 2023-05-15 18:03:33.886523 qualtrics_utils-0.5.3/qualtrics_utils/codebook/map_columns.py
+-rw-r--r--   0        0        0     9221 2023-05-15 17:37:33.348189 qualtrics_utils-0.5.3/qualtrics_utils/survey.py
+-rw-r--r--   0        0        0      494 2023-05-15 17:46:11.216385 qualtrics_utils-0.5.3/qualtrics_utils/utils.py
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.3/setup.py
+-rw-r--r--   0        0        0     2062 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.3/PKG-INFO
```

### Comparing `qualtrics_utils-0.5.2/README.md` & `qualtrics_utils-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `qualtrics_utils-0.5.2/pyproject.toml` & `qualtrics_utils-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qualtrics-utils"
-version = "0.5.2"
+version = "0.5.3"
 description = "Utilities for qualtrics surveys."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 readme = "README.md"
 keywords = ["qualtrics"]
 license = "MIT"
 repository = "https://github.com/mkbabb/qualtrics-utils"
```

### Comparing `qualtrics_utils-0.5.2/qualtrics_utils/codebook/generate.py` & `qualtrics_utils-0.5.3/qualtrics_utils/codebook/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,16 +188,16 @@
                 key: normalize_html_string(value) for key, value in a_choices.items()
             }
             question["answer_choices"] = a_choices
 
     return codebook
 
 
-def create_codebook(filepath: pathlib.Path) -> list[dict]:
-    """Create a codebook from a Qualtrics .qsf file."""
+def generate_codebook(filepath: pathlib.Path) -> list[dict]:
+    """Generate a codebook from a Qualtrics .qsf file."""
     codebook: list[dict] = []
 
     with open(filepath, "r") as file:
         qsf_json = json.load(file)
 
         SurveyElements = qsf_json["SurveyElements"]
 
@@ -222,15 +222,15 @@
     filepath = args.input
 
     if filepath.suffix != ".qsf":
         raise ValueError("Please input a valid .qsf file.")
 
     out_path = filepath.parent / f"{filepath.stem}-codebook"
 
-    codebook = create_codebook(filepath)
+    codebook = generate_codebook(filepath)
 
     with open(out_path, "w") as file:
         json.dump(codebook, file, indent=4)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `qualtrics_utils-0.5.2/qualtrics_utils/codebook/map_columns.py` & `qualtrics_utils-0.5.3/qualtrics_utils/codebook/map_columns.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import argparse
 import json
 import pathlib
 from typing import *
 
+from qualtrics_utils.codebook.generate import generate_codebook
 from qualtrics_utils.utils import normalize_whitespace, quote_value
 
+GENERATOR_TYPES = ["tableau", "sql"]
+
 
 def sql_qualtrics_map_func(mapping: dict) -> dict:
     question_number, question_string, answer_choices = (
         mapping["question_number"],
         mapping["question_string"],
         mapping.get("answer_choices", {}),
     )
@@ -16,25 +19,14 @@
     return {
         "key": question_number,
         "alias": question_string,
         "mapping": answer_choices,
     }
 
 
-def tableau_qualtrics_map_func(mapping: dict) -> dict:
-    question_number, answer_choices = (
-        mapping["question_number"],
-        mapping.get("answer_choices", {}),
-    )
-    return {
-        "key": question_number,
-        "mapping": answer_choices,
-    }
-
-
 def generate_sql(table_name: str, key_mapping: dict) -> Tuple[str, str]:
     key = key_mapping.get("key", "")
     alias = key_mapping.get("alias", key)
     mapping = key_mapping.get("mapping", {})
 
     s = "CASE\n"
 
@@ -45,14 +37,25 @@
         )
         s += f"\tWHEN {key} = {sub_key} THEN {sub_value}\n"
 
     s += f"END AS {alias}"
     return key, s
 
 
+def tableau_qualtrics_map_func(mapping: dict) -> dict:
+    question_number, answer_choices = (
+        mapping["question_number"],
+        mapping.get("answer_choices", {}),
+    )
+    return {
+        "key": question_number,
+        "mapping": answer_choices,
+    }
+
+
 def generate_tableau(key_mapping: dict) -> Tuple[str, str]:
     key = key_mapping.get("key", "")
     mapping = key_mapping.get("mapping", {})
 
     s = ""
     for n, (sub_key, sub_value) in enumerate(mapping.items()):
         sub_key = sub_key if str(sub_key).isnumeric() else quote_value(sub_key, "'")
@@ -62,65 +65,68 @@
         s += f"IF [{key}] == {sub_key} THEN "
         s += f"{sub_value} "
 
     s += f"END"
     return key, s
 
 
+def get_map_and_generator_funcs(kind: str) -> tuple[Callable, Callable]:
+    if kind == "sql":
+        map_func = sql_qualtrics_map_func
+        generator_func = lambda key_mapping: generate_sql("$$TABLE_NAME$$", key_mapping)
+        return map_func, generator_func
+    elif kind == "tableau":
+        return tableau_qualtrics_map_func, generate_tableau
+
+    raise ValueError(f"Invalid kind: {kind}")
+
+
 def map_columns(
-    map_filepath: pathlib.Path,
-    map_func: Callable[[dict], dict],
-    generator_func: Callable[[dict], Tuple[str, str]],
+    input_filepath: pathlib.Path,
+    kind: str,
 ) -> dict:
-    with open(map_filepath, "r") as file:
-        mapping_list = json.load(file)
-        commands = {}
+    map_func, generator_func = get_map_and_generator_funcs(kind)
+
+    with open(input_filepath, "r") as file:
+        mapping_list = (
+            json.load(file)
+            if input_filepath.suffix == ".json"
+            else generate_codebook(input_filepath)
+        )
 
+        commands = {}
         for mapping in mapping_list:
             key_mapping = map_func(mapping)
 
-            if key_mapping is not None:
-                key, command = generator_func(key_mapping)
-                commands[key] = command
+            if key_mapping is None:
+                continue
+
+            key, command = generator_func(key_mapping)
+            commands[key] = command
 
         return commands
 
 
 def main() -> None:
-    generator_types = ["tableau", "sql"]
-
     parser = argparse.ArgumentParser()
     parser.add_argument("input", help="Input file path.", type=pathlib.Path)
     parser.add_argument(
         "--kind",
         help="Generated output kind.",
-        choices=generator_types,
-        required=True,
+        choices=GENERATOR_TYPES,
+        default=GENERATOR_TYPES[0],
     )
 
     args = parser.parse_args()
 
     filepath = args.input
     kind = args.kind
     out_path = filepath.parent / f"{filepath.name}-{kind}-map.json"
 
-    def get_map_and_generator_funcs(kind: str) -> Tuple[Callable, Callable]:
-        if kind == "sql":
-            # TODO: add proper table name retrieval?
-            map_func = sql_qualtrics_map_func
-            generator_func = lambda key_mapping: generate_sql("table_name", key_mapping)
-            return map_func, generator_func
-        elif kind == "tableau":
-            return tableau_qualtrics_map_func, generate_tableau
-        else:
-            return None, None
-
-    map_func, generator_func = get_map_and_generator_funcs(args.kind)
-
-    command = map_columns(filepath, map_func, generator_func)
+    commands = map_columns(filepath, kind)
 
     with open(out_path, "w") as file:
-        json.dump(command, file, indent=4)
+        json.dump(commands, file, indent=4)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `qualtrics_utils-0.5.2/qualtrics_utils/survey.py` & `qualtrics_utils-0.5.3/qualtrics_utils/survey.py`

 * *Files identical despite different names*

### Comparing `qualtrics_utils-0.5.2/setup.py` & `qualtrics_utils-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['googleapiutils2>=0.5.8,<0.6.0',
  'numpy>=1.24.3,<2.0.0',
  'pandas>=2.0.1,<3.0.0',
  'requests>=2.30.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'qualtrics-utils',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': 'Utilities for qualtrics surveys.',
     'long_description': '# qualtrics-utils\n\nUtilities for qualtrics surveys. Get survey responses, generate codebooks, & c.\n\n## [`surveys`](qualtrics_utils/surveys.py)\n\nModule to interact with Qualtrics surveys.\n\nExample (get a survey\'s responses, convert to a pandas DataFrame):\n\n```python\nfrom qualtrics_utils.survey import Surveys\n\nqs = Surveys(api_token=QUALTRICS_API_TOKEN)\n\nexported_file = qs.get_responses_df(\n    surveyId=SURVEY_ID, parse_dates=["StartDate", "EndDate"]\n)\ndf = exported_file.data\n```\n\n## Codebook mapping\n\n### [`generate.py`](qualtrics_utils/codebook/generate_codebook.py)\n\nTakes the exported `.qsf` file from Qualtrics and generates a codebook mapping question\nIDs to question text and answer choices. The output is a JSON file containing a list of\ndictionaries.\n\nExample row:\n\n```json\n{\n        "question_number": "Q5.10",\n        "question_string": "What is your role at this school?"\n        "answer_choices": ...\n},\n```\n\n### [`map_columns.py`](qualtrics_utils/codebook/map_codebook_columns.py)\n\nTakes a codebook mapping (generated by the above function) and creates conditional\nstatements to map the question columns into valid Tableau or SQL code. Used to create a\nsingular question column in the above formats when there are multiple questions in a\nsingle question block (e.g. multiple Likert scale questions).\n',
     'author': 'Mike Babb',
     'author_email': 'mike7400@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mkbabb/qualtrics-utils',
```

### Comparing `qualtrics_utils-0.5.2/PKG-INFO` & `qualtrics_utils-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualtrics-utils
-Version: 0.5.2
+Version: 0.5.3
 Summary: Utilities for qualtrics surveys.
 Home-page: https://github.com/mkbabb/qualtrics-utils
 License: MIT
 Keywords: qualtrics
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

