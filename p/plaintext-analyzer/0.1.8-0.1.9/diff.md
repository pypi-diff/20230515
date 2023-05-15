# Comparing `tmp/plaintext-analyzer-0.1.8.tar.gz` & `tmp/plaintext-analyzer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plaintext-analyzer-0.1.8.tar", max compression
+gzip compressed data, was "plaintext-analyzer-0.1.9.tar", max compression
```

## Comparing `plaintext-analyzer-0.1.8.tar` & `plaintext-analyzer-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     5362 2021-11-17 06:40:58.414258 plaintext-analyzer-0.1.8/README.md
--rw-r--r--   0        0        0      944 2021-11-17 06:40:58.474259 plaintext-analyzer-0.1.8/plaintext_analyzer/__init__.py
--rw-r--r--   0        0        0     3805 2021-11-17 06:40:58.474259 plaintext-analyzer-0.1.8/plaintext_analyzer/entry.py
--rw-r--r--   0        0        0     1018 2021-11-17 06:40:58.474259 plaintext-analyzer-0.1.8/plaintext_analyzer/file_reader.py
--rw-r--r--   0        0        0     1767 2021-11-17 06:40:58.474259 plaintext-analyzer-0.1.8/plaintext_analyzer/file_writer.py
--rw-r--r--   0        0        0     1679 2021-11-17 06:40:58.474259 plaintext-analyzer-0.1.8/plaintext_analyzer/phrase_analyzer.py
--rw-r--r--   0        0        0     2453 2021-11-17 06:40:58.474259 plaintext-analyzer-0.1.8/plaintext_analyzer/structure_kg_analyzer.py
--rw-r--r--   0        0        0     1356 2021-11-17 06:40:58.474259 plaintext-analyzer-0.1.8/plaintext_analyzer/vocab_analyzer.py
--rw-r--r--   0        0        0      820 2021-11-17 06:40:58.478259 plaintext-analyzer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6535 2021-11-17 06:53:38.216176 plaintext-analyzer-0.1.8/setup.py
--rw-r--r--   0        0        0     6131 2021-11-17 06:53:38.216566 plaintext-analyzer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5362 2022-01-09 07:12:43.804798 plaintext-analyzer-0.1.9/README.md
+-rw-r--r--   0        0        0      944 2022-01-09 07:12:43.884805 plaintext-analyzer-0.1.9/plaintext_analyzer/__init__.py
+-rw-r--r--   0        0        0     3805 2022-01-09 07:12:43.884805 plaintext-analyzer-0.1.9/plaintext_analyzer/entry.py
+-rw-r--r--   0        0        0     1018 2022-01-09 07:12:43.884805 plaintext-analyzer-0.1.9/plaintext_analyzer/file_reader.py
+-rw-r--r--   0        0        0     1767 2022-01-09 07:12:43.884805 plaintext-analyzer-0.1.9/plaintext_analyzer/file_writer.py
+-rw-r--r--   0        0        0     1679 2022-01-09 07:12:43.884805 plaintext-analyzer-0.1.9/plaintext_analyzer/phrase_analyzer.py
+-rw-r--r--   0        0        0     2453 2022-01-09 07:12:43.884805 plaintext-analyzer-0.1.9/plaintext_analyzer/structure_kg_analyzer.py
+-rw-r--r--   0        0        0     1356 2022-01-09 07:12:43.884805 plaintext-analyzer-0.1.9/plaintext_analyzer/vocab_analyzer.py
+-rw-r--r--   0        0        0      820 2022-01-09 07:12:43.884805 plaintext-analyzer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6535 2022-01-09 07:13:25.292229 plaintext-analyzer-0.1.9/setup.py
+-rw-r--r--   0        0        0     6131 2022-01-09 07:13:25.292694 plaintext-analyzer-0.1.9/PKG-INFO
```

### Comparing `plaintext-analyzer-0.1.8/README.md` & `plaintext-analyzer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `plaintext-analyzer-0.1.8/plaintext_analyzer/__init__.py` & `plaintext-analyzer-0.1.9/plaintext_analyzer/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,14 @@
     print(sens)
 
     analyzer = PhraseAnalyzer(lang)
     exs = analyzer.overview_phrases(sens, google)
     print(exs)
 """
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 from .file_reader import PlaintextReader
 from .file_writer import CSVWriter, write_to_json
 from .vocab_analyzer import VocabAnalyzer
 from .phrase_analyzer import PhraseAnalyzer
 from .structure_kg_analyzer import StructureKGAnalyzer
```

### Comparing `plaintext-analyzer-0.1.8/plaintext_analyzer/entry.py` & `plaintext-analyzer-0.1.9/plaintext_analyzer/entry.py`

 * *Files identical despite different names*

### Comparing `plaintext-analyzer-0.1.8/plaintext_analyzer/file_reader.py` & `plaintext-analyzer-0.1.9/plaintext_analyzer/file_reader.py`

 * *Files identical despite different names*

### Comparing `plaintext-analyzer-0.1.8/plaintext_analyzer/file_writer.py` & `plaintext-analyzer-0.1.9/plaintext_analyzer/file_writer.py`

 * *Files identical despite different names*

### Comparing `plaintext-analyzer-0.1.8/plaintext_analyzer/phrase_analyzer.py` & `plaintext-analyzer-0.1.9/plaintext_analyzer/phrase_analyzer.py`

 * *Files identical despite different names*

### Comparing `plaintext-analyzer-0.1.8/plaintext_analyzer/structure_kg_analyzer.py` & `plaintext-analyzer-0.1.9/plaintext_analyzer/structure_kg_analyzer.py`

 * *Files identical despite different names*

### Comparing `plaintext-analyzer-0.1.8/plaintext_analyzer/vocab_analyzer.py` & `plaintext-analyzer-0.1.9/plaintext_analyzer/vocab_analyzer.py`

 * *Files identical despite different names*

### Comparing `plaintext-analyzer-0.1.8/pyproject.toml` & `plaintext-analyzer-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "plaintext-analyzer"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Phoenix Grey <phoenix.grey0108@gmail.com>"]
 repository = "https://github.com/qishe-nlp/plaintext-analyzer"
 readme = "README.md"
 documentation = "https://qishe-nlp.github.io/plaintext-analyzer/"
 keywords = ["vocabulary", "phrases", "text", "nlp"] 
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^7.1.2"
-x2cdict = "^0.1.42"
-sencore = "^0.1.30"
+sencore = "^0.1.35"
+x2cdict = "^0.1.44"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 Sphinx = "^3.5.3"
 sphinx-rtd-theme = "^0.5.1"
 
 [tool.poetry.scripts]
```

### Comparing `plaintext-analyzer-0.1.8/setup.py` & `plaintext-analyzer-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['plaintext_analyzer']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>=7.1.2,<8.0.0', 'sencore>=0.1.30,<0.2.0', 'x2cdict>=0.1.42,<0.2.0']
+['click>=7.1.2,<8.0.0', 'sencore>=0.1.35,<0.2.0', 'x2cdict>=0.1.44,<0.2.0']
 
 entry_points = \
 {'console_scripts': ['pta_phrase = plaintext_analyzer.entry:parser_phrase',
                      'pta_structure_kg = '
                      'plaintext_analyzer.entry:parser_structure_kg',
                      'pta_vocab = plaintext_analyzer.entry:parser_vocab']}
 
 setup_kwargs = {
     'name': 'plaintext-analyzer',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '# Installation from pip3\n\n```shell\npip3 install --verbose plaintext_analyzer \npython -m spacy download en_core_web_trf\npython -m spacy download es_dep_news_trf\n```\n\n# Usage\n\nPlease refer to [api docs](https://qishe-nlp.github.io/plaintext-analyzer/).\n\n### Excutable usage\n\n* Get vocabularies from plaintext file \n\n```shell\npta_vocab --source en_plaintext.txt --stype FILE --lang en  \n``` \n\n* Get vocabularies from text \n\n```shell\npta_vocab --source "The typical Bangladeshi breakfast consists of flour-based flatbreads such as chapati, roti or paratha, served with a curry. Usually the curry can be vegetable, home-fried potatoes, or scrambled eggs. The breakfast varies according to location and the eater\'s income. In villages and rural areas, rice with curry (potato mash, dal ) is mostly preferred by day laborers. In the city, sliced bread with jam or jelly is chosen due to time efficiency. In Bangladesh tea is preferred to coffee and is an essential part of most breakfasts. Having toasted biscuits, bread or puffed rice with tea is also very popular." --stype RAW --lang en  \n``` \n\n* Get vocabularies from plaintext file, and write to csv files \n\n```shell\npta_vocab --source en_plaintext.txt --stype FILE --lang en --dstname en_vocab\n``` \n\n* Get vocabularies from text, and write to csv file \n\n```shell\npta_vocab --source "The typical Bangladeshi breakfast consists of flour-based flatbreads such as chapati, roti or paratha, served with a curry. Usually the curry can be vegetable, home-fried potatoes, or scrambled eggs. The breakfast varies according to location and the eater\'s income. In villages and rural areas, rice with curry (potato mash, dal ) is mostly preferred by day laborers. In the city, sliced bread with jam or jelly is chosen due to time efficiency. In Bangladesh tea is preferred to coffee and is an essential part of most breakfasts. Having toasted biscuits, bread or puffed rice with tea is also very popular." --stype RAW --lang en --dstname en_vocab \n``` \n\n* Get phrases from plaintext file \n\n```shell\npta_phrase --source en_plaintext.txt --stype FILE --lang en  \n``` \n\n* Get phrases from text \n\n```shell\npta_phrase --source "The typical Bangladeshi breakfast consists of flour-based flatbreads such as chapati, roti or paratha, served with a curry. Usually the curry can be vegetable, home-fried potatoes, or scrambled eggs. The breakfast varies according to location and the eater\'s income. In villages and rural areas, rice with curry (potato mash, dal ) is mostly preferred by day laborers. In the city, sliced bread with jam or jelly is chosen due to time efficiency. In Bangladesh tea is preferred to coffee and is an essential part of most breakfasts. Having toasted biscuits, bread or puffed rice with tea is also very popular." --stype RAW --lang en  \n``` \n\n* Get phrases from plaintext file, and write to csv files \n\n```shell\npta_phrase --source en_plaintext.txt --stype FILE --lang en --dstname en_phrase\n``` \n\n* Get phrases from text, and write to csv file \n\n```shell\npta_phrase --source "The typical Bangladeshi breakfast consists of flour-based flatbreads such as chapati, roti or paratha, served with a curry. Usually the curry can be vegetable, home-fried potatoes, or scrambled eggs. The breakfast varies according to location and the eater\'s income. In villages and rural areas, rice with curry (potato mash, dal ) is mostly preferred by day laborers. In the city, sliced bread with jam or jelly is chosen due to time efficiency. In Bangladesh tea is preferred to coffee and is an essential part of most breakfasts. Having toasted biscuits, bread or puffed rice with tea is also very popular." --stype RAW --lang en --dstname en_phrase \n``` \n\n### Package usage\n```\ndef parser_vocab(source, stype, lang):\n\n  sf = PlaintextReader(source, stype, lang)\n  sens = sf.sentences\n\n  analyzer = VocabAnalyzer(lang)\n  exs = analyzer.overview_vocabs(sens)\n\n  print(exs)\n\ndef parser_phrase(source, stype, lang):\n\n  sf = PlaintextReader(source, stype, lang)\n  sens = sf.sentences\n\n  analyzer = PhraseAnalyzer(lang)\n  exs = analyzer.overview_phrases(sens)\n\n  print(exs)\n\n```\n\n# Development\n\n### Clone project\n```\ngit clone https://github.com/qishe-nlp/plaintext-analyzer.git\n```\n\n### Install [poetry](https://python-poetry.org/docs/)\n\n### Install dependencies\n```\npoetry update\n```\n\n### Test\n```\npoetry run pytest -rP\n```\nwhich run tests under `tests/*`\n\n### Execute\n```\npoetry run pta_vocab --help\npoetry run pta_phrase --help\n```\n\n### Create sphinx docs\n```\npoetry shell\ncd apidocs\nsphinx-apidoc -f -o source ../plaintext_analyzer\nmake html\npython -m http.server -d build/html\n```\n\n### Host docs on github pages\n```\ncp -rf apidocs/build/html/* docs/\n```\n\n### Build\n* Change `version` in `pyproject.toml` and `plaintext_analyzer/__init__.py`\n* Build python package by `poetry build`\n\n### Git commit and push\n\n### Publish from local dev env\n\n* Set pypi test environment variables in poetry, refer to [poetry doc](https://python-poetry.org/docs/repositories/)\n* Publish to pypi test by `poetry publish -r test`\n\n### Publish through CI \n\n* Github action build and publish package to [test pypi repo](https://test.pypi.org/)\n\n```\ngit tag [x.x.x]\ngit push origin master\n```\n\n* Manually publish to [pypi repo](https://pypi.org/) through [github action](https://github.com/qishe-nlp/plaintext-analyzer/actions/workflows/pypi.yml)\n\n',
     'author': 'Phoenix Grey',
     'author_email': 'phoenix.grey0108@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/qishe-nlp/plaintext-analyzer',
```

### Comparing `plaintext-analyzer-0.1.8/PKG-INFO` & `plaintext-analyzer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: plaintext-analyzer
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/qishe-nlp/plaintext-analyzer
 Keywords: vocabulary,phrases,text,nlp
 Author: Phoenix Grey
 Author-email: phoenix.grey0108@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: sencore (>=0.1.30,<0.2.0)
-Requires-Dist: x2cdict (>=0.1.42,<0.2.0)
+Requires-Dist: sencore (>=0.1.35,<0.2.0)
+Requires-Dist: x2cdict (>=0.1.44,<0.2.0)
 Project-URL: Documentation, https://qishe-nlp.github.io/plaintext-analyzer/
 Project-URL: Repository, https://github.com/qishe-nlp/plaintext-analyzer
 Description-Content-Type: text/markdown
 
 # Installation from pip3
 
 ```shell
```

