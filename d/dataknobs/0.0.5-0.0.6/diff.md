# Comparing `tmp/dataknobs-0.0.5.tar.gz` & `tmp/dataknobs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataknobs-0.0.5.tar", max compression
+gzip compressed data, was "dataknobs-0.0.6.tar", max compression
```

## Comparing `dataknobs-0.0.5.tar` & `dataknobs-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1065 2023-02-10 14:57:51.288106 dataknobs-0.0.5/LICENSE
--rw-r--r--   0        0        0     2189 2023-04-07 02:48:31.052502 dataknobs-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.454505 dataknobs-0.0.5/dataknobs/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.448758 dataknobs-0.0.5/dataknobs/structures/__init__.py
--rw-r--r--   0        0        0     1984 2023-02-10 14:59:17.453600 dataknobs-0.0.5/dataknobs/structures/conditional_dict.py
--rw-r--r--   0        0        0     2244 2023-04-07 02:48:31.054139 dataknobs-0.0.5/dataknobs/structures/document.py
--rw-r--r--   0        0        0     2109 2023-04-29 20:37:59.841029 dataknobs-0.0.5/dataknobs/structures/record_store.py
--rw-r--r--   0        0        0    16152 2023-04-07 02:48:31.055468 dataknobs-0.0.5/dataknobs/structures/tree.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.460301 dataknobs-0.0.5/dataknobs/utils/__init__.py
--rw-r--r--   0        0        0    10016 2023-04-07 02:48:31.055899 dataknobs-0.0.5/dataknobs/utils/elasticsearch_utils.py
--rw-r--r--   0        0        0     8677 2023-02-10 14:59:17.470241 dataknobs-0.0.5/dataknobs/utils/emoji_utils.py
--rw-r--r--   0        0        0     2317 2023-04-19 15:41:48.056711 dataknobs-0.0.5/dataknobs/utils/file_utils.py
--rw-r--r--   0        0        0    17695 2023-03-10 01:33:33.971598 dataknobs-0.0.5/dataknobs/utils/json_paths.py.002
--rw-r--r--   0        0        0    17767 2023-03-11 21:00:19.316119 dataknobs-0.0.5/dataknobs/utils/json_paths.py.del
--rw-r--r--   0        0        0    40729 2023-04-29 20:00:19.391504 dataknobs-0.0.5/dataknobs/utils/json_utils.py
--rw-r--r--   0        0        0    20296 2023-02-18 17:25:48.681883 dataknobs-0.0.5/dataknobs/utils/json_utils.py.000
--rw-r--r--   0        0        0    56727 2023-03-08 20:22:00.908582 dataknobs-0.0.5/dataknobs/utils/json_utils.py.001
--rw-r--r--   0        0        0    56710 2023-03-09 18:53:43.696089 dataknobs-0.0.5/dataknobs/utils/json_utils.py.002
--rw-r--r--   0        0        0    38844 2023-03-12 02:44:32.369267 dataknobs-0.0.5/dataknobs/utils/json_utils.py.003
--rw-r--r--   0        0        0    39879 2023-03-22 16:43:44.020177 dataknobs-0.0.5/dataknobs/utils/json_utils.py.004
--rw-r--r--   0        0        0    14351 2023-02-10 14:59:17.456062 dataknobs-0.0.5/dataknobs/utils/pandas_utils.py
--rw-r--r--   0        0        0     9134 2023-03-13 17:34:48.816244 dataknobs-0.0.5/dataknobs/utils/path_group.py.no-add
--rw-r--r--   0        0        0    11853 2023-03-11 22:32:17.644075 dataknobs-0.0.5/dataknobs/utils/path_sorter.py.del
--rw-r--r--   0        0        0    13283 2023-02-10 14:59:17.466209 dataknobs-0.0.5/dataknobs/utils/requests_utils.py
--rw-r--r--   0        0        0     3782 2023-02-10 14:59:17.458516 dataknobs-0.0.5/dataknobs/utils/resource_utils.py
--rw-r--r--   0        0        0    13186 2023-02-10 14:59:17.469429 dataknobs-0.0.5/dataknobs/utils/sql_utils.py
--rw-r--r--   0        0        0    24066 2023-05-08 19:59:02.942710 dataknobs-0.0.5/dataknobs/utils/stats_utils.py
--rw-r--r--   0        0        0     1425 2023-04-07 02:48:31.057298 dataknobs-0.0.5/dataknobs/utils/subprocess_utils.py
--rw-r--r--   0        0        0     3104 2023-02-10 14:59:17.468140 dataknobs-0.0.5/dataknobs/utils/xml_utils.py
--rw-r--r--   0        0        0     2878 2023-02-10 14:59:17.477011 dataknobs-0.0.5/dataknobs/xization/0.readme.txt
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.477662 dataknobs-0.0.5/dataknobs/xization/__init__.py
--rw-r--r--   0        0        0    23741 2023-04-07 02:48:31.058125 dataknobs-0.0.5/dataknobs/xization/annotations.py
--rw-r--r--   0        0        0    32223 2023-04-07 02:48:31.059013 dataknobs-0.0.5/dataknobs/xization/authorities.py
--rw-r--r--   0        0        0    24670 2023-04-07 02:48:31.059440 dataknobs-0.0.5/dataknobs/xization/lexicon.py
--rw-r--r--   0        0        0    27391 2023-04-07 02:48:31.060348 dataknobs-0.0.5/dataknobs/xization/masking_tokenizer.py
--rw-r--r--   0        0        0    14226 2023-02-10 14:59:17.476141 dataknobs-0.0.5/dataknobs/xization/normalize.py
--rw-r--r--   0        0        0      834 2023-05-08 19:59:02.943066 dataknobs-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 dataknobs-0.0.5/setup.py
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dataknobs-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-10 14:57:51.288106 dataknobs-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2189 2023-04-07 02:48:31.052502 dataknobs-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.454505 dataknobs-0.0.6/dataknobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.448758 dataknobs-0.0.6/dataknobs/structures/__init__.py
+-rw-r--r--   0        0        0     1984 2023-02-10 14:59:17.453600 dataknobs-0.0.6/dataknobs/structures/conditional_dict.py
+-rw-r--r--   0        0        0     2244 2023-04-07 02:48:31.054139 dataknobs-0.0.6/dataknobs/structures/document.py
+-rw-r--r--   0        0        0     2846 2023-05-15 16:49:57.176743 dataknobs-0.0.6/dataknobs/structures/record_store.py
+-rw-r--r--   0        0        0    16152 2023-04-07 02:48:31.055468 dataknobs-0.0.6/dataknobs/structures/tree.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.460301 dataknobs-0.0.6/dataknobs/utils/__init__.py
+-rw-r--r--   0        0        0    10016 2023-04-07 02:48:31.055899 dataknobs-0.0.6/dataknobs/utils/elasticsearch_utils.py
+-rw-r--r--   0        0        0     8677 2023-02-10 14:59:17.470241 dataknobs-0.0.6/dataknobs/utils/emoji_utils.py
+-rw-r--r--   0        0        0     2317 2023-04-19 15:41:48.056711 dataknobs-0.0.6/dataknobs/utils/file_utils.py
+-rw-r--r--   0        0        0    17695 2023-03-10 01:33:33.971598 dataknobs-0.0.6/dataknobs/utils/json_paths.py.002
+-rw-r--r--   0        0        0    17767 2023-03-11 21:00:19.316119 dataknobs-0.0.6/dataknobs/utils/json_paths.py.del
+-rw-r--r--   0        0        0    40729 2023-04-29 20:00:19.391504 dataknobs-0.0.6/dataknobs/utils/json_utils.py
+-rw-r--r--   0        0        0    20296 2023-02-18 17:25:48.681883 dataknobs-0.0.6/dataknobs/utils/json_utils.py.000
+-rw-r--r--   0        0        0    56727 2023-03-08 20:22:00.908582 dataknobs-0.0.6/dataknobs/utils/json_utils.py.001
+-rw-r--r--   0        0        0    56710 2023-03-09 18:53:43.696089 dataknobs-0.0.6/dataknobs/utils/json_utils.py.002
+-rw-r--r--   0        0        0    38844 2023-03-12 02:44:32.369267 dataknobs-0.0.6/dataknobs/utils/json_utils.py.003
+-rw-r--r--   0        0        0    39879 2023-03-22 16:43:44.020177 dataknobs-0.0.6/dataknobs/utils/json_utils.py.004
+-rw-r--r--   0        0        0    14351 2023-02-10 14:59:17.456062 dataknobs-0.0.6/dataknobs/utils/pandas_utils.py
+-rw-r--r--   0        0        0     9134 2023-03-13 17:34:48.816244 dataknobs-0.0.6/dataknobs/utils/path_group.py.no-add
+-rw-r--r--   0        0        0    11853 2023-03-11 22:32:17.644075 dataknobs-0.0.6/dataknobs/utils/path_sorter.py.del
+-rw-r--r--   0        0        0    13283 2023-02-10 14:59:17.466209 dataknobs-0.0.6/dataknobs/utils/requests_utils.py
+-rw-r--r--   0        0        0     3782 2023-02-10 14:59:17.458516 dataknobs-0.0.6/dataknobs/utils/resource_utils.py
+-rw-r--r--   0        0        0    13186 2023-02-10 14:59:17.469429 dataknobs-0.0.6/dataknobs/utils/sql_utils.py
+-rw-r--r--   0        0        0    24066 2023-05-08 19:59:02.942710 dataknobs-0.0.6/dataknobs/utils/stats_utils.py
+-rw-r--r--   0        0        0     1425 2023-04-07 02:48:31.057298 dataknobs-0.0.6/dataknobs/utils/subprocess_utils.py
+-rw-r--r--   0        0        0     3104 2023-02-10 14:59:17.468140 dataknobs-0.0.6/dataknobs/utils/xml_utils.py
+-rw-r--r--   0        0        0     2878 2023-02-10 14:59:17.477011 dataknobs-0.0.6/dataknobs/xization/0.readme.txt
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.477662 dataknobs-0.0.6/dataknobs/xization/__init__.py
+-rw-r--r--   0        0        0    23741 2023-04-07 02:48:31.058125 dataknobs-0.0.6/dataknobs/xization/annotations.py
+-rw-r--r--   0        0        0    32223 2023-04-07 02:48:31.059013 dataknobs-0.0.6/dataknobs/xization/authorities.py
+-rw-r--r--   0        0        0    24670 2023-04-07 02:48:31.059440 dataknobs-0.0.6/dataknobs/xization/lexicon.py
+-rw-r--r--   0        0        0    27391 2023-04-07 02:48:31.060348 dataknobs-0.0.6/dataknobs/xization/masking_tokenizer.py
+-rw-r--r--   0        0        0    14226 2023-02-10 14:59:17.476141 dataknobs-0.0.6/dataknobs/xization/normalize.py
+-rw-r--r--   0        0        0      834 2023-05-15 16:49:57.177027 dataknobs-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 dataknobs-0.0.6/setup.py
+-rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dataknobs-0.0.6/PKG-INFO
```

### Comparing `dataknobs-0.0.5/LICENSE` & `dataknobs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/README.md` & `dataknobs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/structures/conditional_dict.py` & `dataknobs-0.0.6/dataknobs/structures/conditional_dict.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/structures/document.py` & `dataknobs-0.0.6/dataknobs/structures/document.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/structures/record_store.py` & `dataknobs-0.0.6/dataknobs/structures/record_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,32 +10,37 @@
     dictionaries and/or as a dataframe and as a tsv file on disk.
     '''
 
     def __init__(
             self,
             tsv_fpath: str,
             df: pd.DataFrame = None,
+            sep: str = '\t',
     ):
         '''
         :param tsv_fpath: The path to the tsv file on disk. If None or
             empty, then data will not be persisted.
+        :param df: An initial dataframe
+        :param sep: The file separator to use (if not a tab)
         '''
         self.tsv_fpath = tsv_fpath
+        self.init_df = df
+        self.sep = sep
         self._df = None
         self._recs = None  # List[Dict[str, Any]]
         self._init_data(df)
 
     def _init_data(self, df: pd.DataFrame = None):
         '''
         Initialize store data from the tsv file.
         '''
-        if os.path.exists(self.tsv_fpath):
-            self._df = pd.read_csv(self.tsv_fpath, sep='\t')
+        if self.tsv_fpath is not None and os.path.exists(self.tsv_fpath):
+            self._df = pd.read_csv(self.tsv_fpath, sep=self.sep)
         else:
-            self._df = df
+            self._df = df.copy() if df is not None else None
         self._recs = self._build_recs_from_df()
 
     def _build_recs_from_df(self) -> List[Dict[str, Any]]:
         ''' Build records from the dataframe '''
         if self._df is not None:
             recs = [
                 json.loads(rec)
@@ -55,19 +60,32 @@
         return self._df
 
     @property
     def records(self) -> List[Dict[str, Any]]:
         ''' Get the records as a list of dictionaries '''
         return self._recs
 
+    def clear(self):
+        '''
+        Clear the contents, starting from empty, but don't auto-"save".
+        '''
+        self._recs.clear()
+        self._df = None
+
     def add_rec(self, rec: Dict[str, Any]):
         ''' Add the record '''
         self._recs.append(rec)
         self._df = None
 
     def save(self):
         ''' Save the records to disk as a tsv '''
-        self.df.to_csv(self.tsv_fpath, sep='\t', index=False)
+        if self.tsv_fpath is not None:
+            self.df.to_csv(self.tsv_fpath, sep=self.sep, index=False)
 
-    def restore(self):
-        ''' Restore records from the version on disk, discarding any changes '''
-        self._init_data()
+    def restore(self, df: pd.DataFrame = None):
+        '''
+        Restore records from the version on disk, discarding any changes.
+        NOTE: If there is no backing file (e.g., tsv_fpath is None), then
+        restore will discard all data and restart with the given df (if not
+        None,) the init df or start anew.
+        '''
+        self._init_data(df if df is not None else self.init_df)
```

### Comparing `dataknobs-0.0.5/dataknobs/structures/tree.py` & `dataknobs-0.0.6/dataknobs/structures/tree.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/elasticsearch_utils.py` & `dataknobs-0.0.6/dataknobs/utils/elasticsearch_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/emoji_utils.py` & `dataknobs-0.0.6/dataknobs/utils/emoji_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/file_utils.py` & `dataknobs-0.0.6/dataknobs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/json_paths.py.002` & `dataknobs-0.0.6/dataknobs/utils/json_paths.py.002`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/json_paths.py.del` & `dataknobs-0.0.6/dataknobs/utils/json_paths.py.del`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/json_utils.py` & `dataknobs-0.0.6/dataknobs/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/json_utils.py.000` & `dataknobs-0.0.6/dataknobs/utils/json_utils.py.000`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/json_utils.py.001` & `dataknobs-0.0.6/dataknobs/utils/json_utils.py.001`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/json_utils.py.002` & `dataknobs-0.0.6/dataknobs/utils/json_utils.py.002`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/json_utils.py.003` & `dataknobs-0.0.6/dataknobs/utils/json_utils.py.003`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/json_utils.py.004` & `dataknobs-0.0.6/dataknobs/utils/json_utils.py.004`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/pandas_utils.py` & `dataknobs-0.0.6/dataknobs/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/path_group.py.no-add` & `dataknobs-0.0.6/dataknobs/utils/path_group.py.no-add`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/path_sorter.py.del` & `dataknobs-0.0.6/dataknobs/utils/path_sorter.py.del`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/requests_utils.py` & `dataknobs-0.0.6/dataknobs/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/resource_utils.py` & `dataknobs-0.0.6/dataknobs/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/sql_utils.py` & `dataknobs-0.0.6/dataknobs/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/stats_utils.py` & `dataknobs-0.0.6/dataknobs/utils/stats_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/subprocess_utils.py` & `dataknobs-0.0.6/dataknobs/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/utils/xml_utils.py` & `dataknobs-0.0.6/dataknobs/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/xization/0.readme.txt` & `dataknobs-0.0.6/dataknobs/xization/0.readme.txt`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/xization/annotations.py` & `dataknobs-0.0.6/dataknobs/xization/annotations.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/xization/authorities.py` & `dataknobs-0.0.6/dataknobs/xization/authorities.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/xization/lexicon.py` & `dataknobs-0.0.6/dataknobs/xization/lexicon.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/xization/masking_tokenizer.py` & `dataknobs-0.0.6/dataknobs/xization/masking_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/dataknobs/xization/normalize.py` & `dataknobs-0.0.6/dataknobs/xization/normalize.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.5/pyproject.toml` & `dataknobs-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataknobs"
-version = "0.0.5"
+version = "0.0.6"
 description = "Useful implementations of data structures and design patterns for AI knowledge bases."
 authors = ["Spence Koehler <KoehlerSB747@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dataknobs"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dataknobs-0.0.5/setup.py` & `dataknobs-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'psycopg2-binary>=2.9.3,<3.0.0',
  'python-dotenv>=0.21.0,<0.22.0',
  'requests>=2.28.1,<3.0.0',
  'scikit-learn>=1.2.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'dataknobs',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'Useful implementations of data structures and design patterns for AI knowledge bases.',
     'long_description': 'DataKnobs\n=============================\n\n## Description\n\nUseful implementations of data structures and design patterns for knowledge bases and AI, or the knobs and levers for fine-tuning and leveraging your data.\n\nThis repo also serves as a template or sandbox for development, experimentation, and testing of general data structures, algorithms, and utilities for DS, AI, ML, and NLP.\n\nProvides connectors for other popular text and data processing packages like:\n  * numpy and pandas\n  * nltk\n  * wordnet\n  * postgres\n  * elasticsearch\n\n## General project information\n\nThe purpose of this project is:\n\n  * To provide dependable implementations of useful data structures.\n  * To show examples of design patterns and ways to apply AI concepts.\n  * To prototype tools for delivering a robust DS/AI/ML/NLP utilities library package.\n  * To facilitate interactive development, demonstration, visualization, and testing of the library components via jupter notebooks and/or scripts.\n\n## Installation and Usage\n\n```bash/python\n% pip install dataknobs\n% python\n>>> import dataknobs as dk\n>>> ...\n```\n\n\n## Development\n\n### Development machine prerequisites\n\nThe following minimum configuration should exist for development:\n\n  * tox\n  * pyenv\n     * pyenv install 3.9\n  * poetry\n\nWith optional:\n\n  * docker\n  * bash\n\nBy convention, a data directory can be leveraged for development that is mounted as a shared volumne in Docker as /data. This has the default of $HOME/data, but can be overridden with the DATADIR environment variable.\n\n\n### Development quickstart guide\n\n  * In a terminal, clone the repo and cd into the project directory.\n\n#### Testing\n\n  * Tests and Lint: "tox"\n  * Just unit tests: "tox -e tests"\n  * Just lint: "tox -e lint"\n\n#### Using docker\n\n  * Development:\n```\n% tox -e dev\n# poetry shell\n# python\n```\n\n  * Notebook:\n    * execute "tox -e nb"\n      * copy/paste url into browser\n\n#### Using virtual environments\n\n  * Development:\n    * Manual: source ".project_vars", poetry install, poetry shell\n    * Automated: execute "bin/start_dev.sh"  (requires "/bin/bash" on your machine)\n\n  * Notebook:\n    * execute "bin/start_notebook.sh"\n      * copy/paste url into browser\n',
     'author': 'Spence Koehler',
     'author_email': 'KoehlerSB747@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dataknobs-0.0.5/PKG-INFO` & `dataknobs-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataknobs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Useful implementations of data structures and design patterns for AI knowledge bases.
 Author: Spence Koehler
 Author-email: KoehlerSB747@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

