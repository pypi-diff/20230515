# Comparing `tmp/qualtrics_utils-0.5.0.tar.gz` & `tmp/qualtrics_utils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualtrics_utils-0.5.0.tar", max compression
+gzip compressed data, was "qualtrics_utils-0.5.1.tar", max compression
```

## Comparing `qualtrics_utils-0.5.0.tar` & `qualtrics_utils-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1263 2023-05-15 17:45:49.414448 qualtrics_utils-0.5.0/README.md
--rw-r--r--   0        0        0      612 2023-05-15 17:49:13.610727 qualtrics_utils-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-05-15 17:24:27.114345 qualtrics_utils-0.5.0/qualtrics_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 17:42:52.914230 qualtrics_utils-0.5.0/qualtrics_utils/codebook/__init__.py
--rw-r--r--   0        0        0     6983 2023-05-15 17:30:20.944642 qualtrics_utils-0.5.0/qualtrics_utils/codebook/generate.py
--rw-r--r--   0        0        0     3498 2023-05-15 14:49:13.310183 qualtrics_utils-0.5.0/qualtrics_utils/codebook/map_columns.py
--rw-r--r--   0        0        0     9221 2023-05-15 17:37:33.348189 qualtrics_utils-0.5.0/qualtrics_utils/surveys.py
--rw-r--r--   0        0        0      494 2023-05-15 17:46:11.216385 qualtrics_utils-0.5.0/qualtrics_utils/utils.py
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.0/setup.py
--rw-r--r--   0        0        0     2027 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1310 2023-05-15 17:51:41.207011 qualtrics_utils-0.5.1/README.md
+-rw-r--r--   0        0        0      593 2023-05-15 17:52:05.400239 qualtrics_utils-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-05-15 17:24:27.114345 qualtrics_utils-0.5.1/qualtrics_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 17:42:52.914230 qualtrics_utils-0.5.1/qualtrics_utils/codebook/__init__.py
+-rw-r--r--   0        0        0     6983 2023-05-15 17:30:20.944642 qualtrics_utils-0.5.1/qualtrics_utils/codebook/generate.py
+-rw-r--r--   0        0        0     3498 2023-05-15 14:49:13.310183 qualtrics_utils-0.5.1/qualtrics_utils/codebook/map_columns.py
+-rw-r--r--   0        0        0     9221 2023-05-15 17:37:33.348189 qualtrics_utils-0.5.1/qualtrics_utils/surveys.py
+-rw-r--r--   0        0        0      494 2023-05-15 17:46:11.216385 qualtrics_utils-0.5.1/qualtrics_utils/utils.py
+-rw-r--r--   0        0        0     2140 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.1/setup.py
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 qualtrics_utils-0.5.1/PKG-INFO
```

### Comparing `qualtrics_utils-0.5.0/README.md` & `qualtrics_utils-0.5.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # qualtrics-utils
 
-A collection of utility scripts for Qualtrics surveys.
+Utilities for qualtrics surveys. Get survey responses, generate codebooks, & c.
 
-## [Surveys](qualtrics_utils/surveys.py)
+## [`surveys`](qualtrics_utils/surveys.py)
 
 Module to interact with Qualtrics surveys.
 
 Example (get a survey's responses, convert to a pandas DataFrame):
 
 ```python
 from qualtrics_utils import Surveys
 
 qs = Surveys(api_token=QUALTRICS_API_TOKEN)
 
 exported_file = qs.get_responses_df(
     surveyId=SURVEY_ID, parse_dates=["StartDate", "EndDate"]
 )
-...
+df = exported_file.data
 ```
 
 ## Codebook mapping
 
 ### [`generate.py`](qualtrics_utils/codebook/generate_codebook.py)
 
 Takes the exported `.qsf` file from Qualtrics and generates a codebook mapping question
```

### Comparing `qualtrics_utils-0.5.0/pyproject.toml` & `qualtrics_utils-0.5.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "qualtrics-utils"
-version = "0.5.0"
-description = "A set of utilities for working with Qualtrics data."
+version = "0.5.1"
+description = "Utilities for qualtrics surveys."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 readme = "README.md"
 keywords = ["qualtrics"]
 license = "MIT"
 repository = "https://github.com/mkbabb/qualtrics-utils"
```

### Comparing `qualtrics_utils-0.5.0/qualtrics_utils/codebook/generate.py` & `qualtrics_utils-0.5.1/qualtrics_utils/codebook/generate.py`

 * *Files identical despite different names*

### Comparing `qualtrics_utils-0.5.0/qualtrics_utils/codebook/map_columns.py` & `qualtrics_utils-0.5.1/qualtrics_utils/codebook/map_columns.py`

 * *Files identical despite different names*

### Comparing `qualtrics_utils-0.5.0/qualtrics_utils/surveys.py` & `qualtrics_utils-0.5.1/qualtrics_utils/surveys.py`

 * *Files identical despite different names*

### Comparing `qualtrics_utils-0.5.0/setup.py` & `qualtrics_utils-0.5.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['googleapiutils2>=0.5.8,<0.6.0',
  'numpy>=1.24.3,<2.0.0',
  'pandas>=2.0.1,<3.0.0',
  'requests>=2.30.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'qualtrics-utils',
-    'version': '0.5.0',
-    'description': 'A set of utilities for working with Qualtrics data.',
-    'long_description': '# qualtrics-utils\n\nA collection of utility scripts for Qualtrics surveys.\n\n## [Surveys](qualtrics_utils/surveys.py)\n\nModule to interact with Qualtrics surveys.\n\nExample (get a survey\'s responses, convert to a pandas DataFrame):\n\n```python\nfrom qualtrics_utils import Surveys\n\nqs = Surveys(api_token=QUALTRICS_API_TOKEN)\n\nexported_file = qs.get_responses_df(\n    surveyId=SURVEY_ID, parse_dates=["StartDate", "EndDate"]\n)\n...\n```\n\n## Codebook mapping\n\n### [`generate.py`](qualtrics_utils/codebook/generate_codebook.py)\n\nTakes the exported `.qsf` file from Qualtrics and generates a codebook mapping question\nIDs to question text and answer choices. The output is a JSON file containing a list of\ndictionaries.\n\nExample row:\n\n```json\n{\n        "question_number": "Q5.10",\n        "question_string": "What is your role at this school?"\n        "answer_choices": ...\n},\n```\n\n### [`map_columns.py`](qualtrics_utils/codebook/map_codebook_columns.py)\n\nTakes a codebook mapping (generated by the above function) and creates conditional\nstatements to map the question columns into valid Tableau or SQL code. Used to create a\nsingular question column in the above formats when there are multiple questions in a\nsingle question block (e.g. multiple Likert scale questions).\n',
+    'version': '0.5.1',
+    'description': 'Utilities for qualtrics surveys.',
+    'long_description': '# qualtrics-utils\n\nUtilities for qualtrics surveys. Get survey responses, generate codebooks, & c.\n\n## [`surveys`](qualtrics_utils/surveys.py)\n\nModule to interact with Qualtrics surveys.\n\nExample (get a survey\'s responses, convert to a pandas DataFrame):\n\n```python\nfrom qualtrics_utils import Surveys\n\nqs = Surveys(api_token=QUALTRICS_API_TOKEN)\n\nexported_file = qs.get_responses_df(\n    surveyId=SURVEY_ID, parse_dates=["StartDate", "EndDate"]\n)\ndf = exported_file.data\n```\n\n## Codebook mapping\n\n### [`generate.py`](qualtrics_utils/codebook/generate_codebook.py)\n\nTakes the exported `.qsf` file from Qualtrics and generates a codebook mapping question\nIDs to question text and answer choices. The output is a JSON file containing a list of\ndictionaries.\n\nExample row:\n\n```json\n{\n        "question_number": "Q5.10",\n        "question_string": "What is your role at this school?"\n        "answer_choices": ...\n},\n```\n\n### [`map_columns.py`](qualtrics_utils/codebook/map_codebook_columns.py)\n\nTakes a codebook mapping (generated by the above function) and creates conditional\nstatements to map the question columns into valid Tableau or SQL code. Used to create a\nsingular question column in the above formats when there are multiple questions in a\nsingle question block (e.g. multiple Likert scale questions).\n',
     'author': 'Mike Babb',
     'author_email': 'mike7400@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mkbabb/qualtrics-utils',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `qualtrics_utils-0.5.0/PKG-INFO` & `qualtrics_utils-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qualtrics-utils
-Version: 0.5.0
-Summary: A set of utilities for working with Qualtrics data.
+Version: 0.5.1
+Summary: Utilities for qualtrics surveys.
 Home-page: https://github.com/mkbabb/qualtrics-utils
 License: MIT
 Keywords: qualtrics
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,31 +17,31 @@
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Project-URL: Repository, https://github.com/mkbabb/qualtrics-utils
 Description-Content-Type: text/markdown
 
 # qualtrics-utils
 
-A collection of utility scripts for Qualtrics surveys.
+Utilities for qualtrics surveys. Get survey responses, generate codebooks, & c.
 
-## [Surveys](qualtrics_utils/surveys.py)
+## [`surveys`](qualtrics_utils/surveys.py)
 
 Module to interact with Qualtrics surveys.
 
 Example (get a survey's responses, convert to a pandas DataFrame):
 
 ```python
 from qualtrics_utils import Surveys
 
 qs = Surveys(api_token=QUALTRICS_API_TOKEN)
 
 exported_file = qs.get_responses_df(
     surveyId=SURVEY_ID, parse_dates=["StartDate", "EndDate"]
 )
-...
+df = exported_file.data
 ```
 
 ## Codebook mapping
 
 ### [`generate.py`](qualtrics_utils/codebook/generate_codebook.py)
 
 Takes the exported `.qsf` file from Qualtrics and generates a codebook mapping question
```

