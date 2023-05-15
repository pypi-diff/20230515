# Comparing `tmp/pypi-search-1.2.1.tar.gz` & `tmp/pypi-search-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi-search-1.2.1.tar", last modified: Fri Jul  2 21:38:20 2021, max compression
+gzip compressed data, was "pypi-search-1.2.2.tar", last modified: Mon May 15 17:55:33 2023, max compression
```

## Comparing `pypi-search-1.2.1.tar` & `pypi-search-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 asad      (1000) asad      (1000)        0 2021-07-02 21:38:20.054271 pypi-search-1.2.1/
--rw-rw-r--   0 asad      (1000) asad      (1000)     1068 2021-07-02 21:06:59.000000 pypi-search-1.2.1/LICENSE
--rw-rw-r--   0 asad      (1000) asad      (1000)       25 2021-07-02 21:35:23.000000 pypi-search-1.2.1/MANIFEST.in
--rw-rw-r--   0 asad      (1000) asad      (1000)     1790 2021-07-02 21:38:20.054271 pypi-search-1.2.1/PKG-INFO
--rw-rw-r--   0 asad      (1000) asad      (1000)     1307 2021-07-02 21:11:41.000000 pypi-search-1.2.1/README.md
-drwxrwxr-x   0 asad      (1000) asad      (1000)        0 2021-07-02 21:38:20.054271 pypi-search-1.2.1/pypi_search/
--rw-rw-r--   0 asad      (1000) asad      (1000)       22 2021-07-02 21:36:41.000000 pypi-search-1.2.1/pypi_search/__init__.py
--rw-rw-r--   0 asad      (1000) asad      (1000)       80 2021-07-02 21:06:59.000000 pypi-search-1.2.1/pypi_search/__main__.py
--rw-rw-r--   0 asad      (1000) asad      (1000)      701 2021-07-02 21:11:41.000000 pypi-search-1.2.1/pypi_search/arg_parser.py
--rw-rw-r--   0 asad      (1000) asad      (1000)      377 2021-07-02 21:06:59.000000 pypi-search-1.2.1/pypi_search/log.py
--rw-rw-r--   0 asad      (1000) asad      (1000)     2782 2021-07-02 21:11:41.000000 pypi-search-1.2.1/pypi_search/main.py
--rw-rw-r--   0 asad      (1000) asad      (1000)      994 2021-07-02 21:06:59.000000 pypi-search-1.2.1/pypi_search/search.py
--rw-rw-r--   0 asad      (1000) asad      (1000)     4433 2021-07-02 21:11:41.000000 pypi-search-1.2.1/pypi_search/utils.py
-drwxrwxr-x   0 asad      (1000) asad      (1000)        0 2021-07-02 21:38:20.054271 pypi-search-1.2.1/pypi_search.egg-info/
--rw-rw-r--   0 asad      (1000) asad      (1000)     1790 2021-07-02 21:38:20.000000 pypi-search-1.2.1/pypi_search.egg-info/PKG-INFO
--rw-rw-r--   0 asad      (1000) asad      (1000)      423 2021-07-02 21:38:20.000000 pypi-search-1.2.1/pypi_search.egg-info/SOURCES.txt
--rw-rw-r--   0 asad      (1000) asad      (1000)        1 2021-07-02 21:38:20.000000 pypi-search-1.2.1/pypi_search.egg-info/dependency_links.txt
--rw-rw-r--   0 asad      (1000) asad      (1000)       54 2021-07-02 21:38:20.000000 pypi-search-1.2.1/pypi_search.egg-info/entry_points.txt
--rw-rw-r--   0 asad      (1000) asad      (1000)       60 2021-07-02 21:38:20.000000 pypi-search-1.2.1/pypi_search.egg-info/requires.txt
--rw-rw-r--   0 asad      (1000) asad      (1000)       12 2021-07-02 21:38:20.000000 pypi-search-1.2.1/pypi_search.egg-info/top_level.txt
--rw-rw-r--   0 asad      (1000) asad      (1000)       60 2021-07-02 21:06:59.000000 pypi-search-1.2.1/requirements.txt
--rw-rw-r--   0 asad      (1000) asad      (1000)       38 2021-07-02 21:38:20.054271 pypi-search-1.2.1/setup.cfg
--rw-rw-r--   0 asad      (1000) asad      (1000)      891 2021-07-02 21:36:50.000000 pypi-search-1.2.1/setup.py
+drwxrwxr-x   0 asad      (1000) asad      (1000)        0 2023-05-15 17:55:33.771723 pypi-search-1.2.2/
+-rw-rw-r--   0 asad      (1000) asad      (1000)     1068 2023-05-14 00:32:40.000000 pypi-search-1.2.2/LICENSE
+-rw-rw-r--   0 asad      (1000) asad      (1000)       25 2023-05-14 00:32:40.000000 pypi-search-1.2.2/MANIFEST.in
+-rw-rw-r--   0 asad      (1000) asad      (1000)     1770 2023-05-15 17:55:33.771723 pypi-search-1.2.2/PKG-INFO
+-rw-rw-r--   0 asad      (1000) asad      (1000)     1307 2023-05-14 00:32:40.000000 pypi-search-1.2.2/README.md
+drwxrwxr-x   0 asad      (1000) asad      (1000)        0 2023-05-15 17:55:33.771723 pypi-search-1.2.2/pypi_search/
+-rw-rw-r--   0 asad      (1000) asad      (1000)       22 2023-05-15 17:54:30.000000 pypi-search-1.2.2/pypi_search/__init__.py
+-rw-rw-r--   0 asad      (1000) asad      (1000)       80 2023-05-14 00:32:40.000000 pypi-search-1.2.2/pypi_search/__main__.py
+-rw-rw-r--   0 asad      (1000) asad      (1000)      701 2023-05-14 00:32:40.000000 pypi-search-1.2.2/pypi_search/arg_parser.py
+-rw-rw-r--   0 asad      (1000) asad      (1000)      377 2023-05-14 00:32:40.000000 pypi-search-1.2.2/pypi_search/log.py
+-rw-rw-r--   0 asad      (1000) asad      (1000)     2782 2023-05-14 00:32:40.000000 pypi-search-1.2.2/pypi_search/main.py
+-rw-rw-r--   0 asad      (1000) asad      (1000)      994 2023-05-14 00:32:40.000000 pypi-search-1.2.2/pypi_search/search.py
+-rw-rw-r--   0 asad      (1000) asad      (1000)     4350 2023-05-15 17:45:38.000000 pypi-search-1.2.2/pypi_search/utils.py
+drwxrwxr-x   0 asad      (1000) asad      (1000)        0 2023-05-15 17:55:33.771723 pypi-search-1.2.2/pypi_search.egg-info/
+-rw-rw-r--   0 asad      (1000) asad      (1000)     1770 2023-05-15 17:55:33.000000 pypi-search-1.2.2/pypi_search.egg-info/PKG-INFO
+-rw-rw-r--   0 asad      (1000) asad      (1000)      423 2023-05-15 17:55:33.000000 pypi-search-1.2.2/pypi_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 asad      (1000) asad      (1000)        1 2023-05-15 17:55:33.000000 pypi-search-1.2.2/pypi_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 asad      (1000) asad      (1000)       53 2023-05-15 17:55:33.000000 pypi-search-1.2.2/pypi_search.egg-info/entry_points.txt
+-rw-rw-r--   0 asad      (1000) asad      (1000)       60 2023-05-15 17:55:33.000000 pypi-search-1.2.2/pypi_search.egg-info/requires.txt
+-rw-rw-r--   0 asad      (1000) asad      (1000)       12 2023-05-15 17:55:33.000000 pypi-search-1.2.2/pypi_search.egg-info/top_level.txt
+-rw-rw-r--   0 asad      (1000) asad      (1000)       60 2023-05-14 00:32:40.000000 pypi-search-1.2.2/requirements.txt
+-rw-rw-r--   0 asad      (1000) asad      (1000)       38 2023-05-15 17:55:33.771723 pypi-search-1.2.2/setup.cfg
+-rw-rw-r--   0 asad      (1000) asad      (1000)      891 2023-05-15 17:54:36.000000 pypi-search-1.2.2/setup.py
```

### Comparing `pypi-search-1.2.1/LICENSE` & `pypi-search-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi-search-1.2.1/PKG-INFO` & `pypi-search-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pypi-search
-Version: 1.2.1
+Version: 1.2.2
 Summary: Get Information on Python Packages From PyPI
 Home-page: https://github.com/asadmoosvi/pypi-search
 Author: Asad Moosvi
 Author-email: moosvi.asad@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -64,9 +63,7 @@
 ```
 
 
 # todo
 
 - [x] In order to make this easier to use I will be making a package out of this
 so it can easily be installed via `pip`.
-
-
```

### Comparing `pypi-search-1.2.1/README.md` & `pypi-search-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pypi-search-1.2.1/pypi_search/arg_parser.py` & `pypi-search-1.2.2/pypi_search/arg_parser.py`

 * *Files identical despite different names*

### Comparing `pypi-search-1.2.1/pypi_search/main.py` & `pypi-search-1.2.2/pypi_search/main.py`

 * *Files identical despite different names*

### Comparing `pypi-search-1.2.1/pypi_search/search.py` & `pypi-search-1.2.2/pypi_search/search.py`

 * *Files identical despite different names*

### Comparing `pypi-search-1.2.1/pypi_search/utils.py` & `pypi-search-1.2.2/pypi_search/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,19 @@
         links = {
             link.text.strip(): link['href'] for
             link in links
         }
         return links
 
     def get_github_stats(self) -> Optional[Dict[str, int]]:
-        # github stats are in the third sidebar section
-        sidebar_sections = self._get_sidebar_sections()
-        github_stats = sidebar_sections[2].find('div', class_='github-repo-info')
+        github_stats = self.soup.find('div', {'data-controller': 'github-repo-stats'})
         if not github_stats:
             return None
 
-        github_data_url = github_stats['data-url']
+        github_data_url = github_stats['data-github-repo-stats-url-value']
         github_stats_json = requests.get(github_data_url).json()
 
         stars = github_stats_json.get('stargazers_count')
         forks = github_stats_json.get('forks_count')
         issues = github_stats_json.get('open_issues_count')
         if stars is None or forks is None or issues is None:
             return None
```

### Comparing `pypi-search-1.2.1/pypi_search.egg-info/PKG-INFO` & `pypi-search-1.2.2/pypi_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pypi-search
-Version: 1.2.1
+Version: 1.2.2
 Summary: Get Information on Python Packages From PyPI
 Home-page: https://github.com/asadmoosvi/pypi-search
 Author: Asad Moosvi
 Author-email: moosvi.asad@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -64,9 +63,7 @@
 ```
 
 
 # todo
 
 - [x] In order to make this easier to use I will be making a package out of this
 so it can easily be installed via `pip`.
-
-
```

### Comparing `pypi-search-1.2.1/setup.py` & `pypi-search-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as req_f:
     install_requires=req_f.read().split()
 
 setuptools.setup(
     name="pypi-search",
-    version="1.2.1",
+    version="1.2.2",
     author="Asad Moosvi",
     author_email="moosvi.asad@gmail.com",
     description="Get Information on Python Packages From PyPI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/asadmoosvi/pypi-search",
     packages=setuptools.find_packages(),
```

