# Comparing `tmp/corpus_pax-0.1.8.tar.gz` & `tmp/corpus_pax-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus_pax-0.1.8.tar", max compression
+gzip compressed data, was "corpus_pax-0.1.9.tar", max compression
```

## Comparing `corpus_pax-0.1.8.tar` & `corpus_pax-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2893 2023-01-11 15:53:40.624099 corpus_pax-0.1.8/README.md
--rw-r--r--   0        0        0      298 2023-01-11 15:53:40.624361 corpus_pax-0.1.8/corpus_pax/__init__.py
--rw-r--r--   0        0        0     2383 2023-01-11 15:53:40.624487 corpus_pax-0.1.8/corpus_pax/__main__.py
--rw-r--r--   0        0        0     4380 2023-01-11 13:15:14.422364 corpus_pax-0.1.8/corpus_pax/_api.py
--rw-r--r--   0        0        0     3273 2023-01-11 15:53:40.624680 corpus_pax-0.1.8/corpus_pax/articles.py
--rw-r--r--   0        0        0     6731 2023-01-11 15:53:40.624890 corpus_pax-0.1.8/corpus_pax/entities.py
--rw-r--r--   0        0        0     6265 2023-01-11 13:15:14.423551 corpus_pax-0.1.8/corpus_pax/resources.py
--rw-r--r--   0        0        0      402 2022-10-31 04:17:42.220338 corpus_pax-0.1.8/corpus_pax/templates/update_member_id_on_insert_email.sql
--rw-r--r--   0        0        0     1531 2023-01-11 15:53:40.625100 corpus_pax-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3869 1970-01-01 00:00:00.000000 corpus_pax-0.1.8/setup.py
--rw-r--r--   0        0        0     3747 1970-01-01 00:00:00.000000 corpus_pax-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2556 2023-01-12 04:14:31.067322 corpus_pax-0.1.9/README.md
+-rw-r--r--   0        0        0      302 2023-01-12 03:54:45.747005 corpus_pax-0.1.9/corpus_pax/__init__.py
+-rw-r--r--   0        0        0     2328 2023-01-12 03:54:18.218097 corpus_pax-0.1.9/corpus_pax/__main__.py
+-rw-r--r--   0        0        0     4380 2023-01-11 13:15:14.422364 corpus_pax-0.1.9/corpus_pax/_api.py
+-rw-r--r--   0        0        0     3273 2023-01-11 15:53:40.624680 corpus_pax-0.1.9/corpus_pax/articles.py
+-rw-r--r--   0        0        0     6731 2023-01-11 15:53:40.624890 corpus_pax-0.1.9/corpus_pax/entities.py
+-rw-r--r--   0        0        0     6265 2023-01-11 13:15:14.423551 corpus_pax-0.1.9/corpus_pax/resources.py
+-rw-r--r--   0        0        0      402 2022-10-31 04:17:42.220338 corpus_pax-0.1.9/corpus_pax/templates/update_member_id_on_insert_email.sql
+-rw-r--r--   0        0        0     1547 2023-01-12 04:15:57.533613 corpus_pax-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 corpus_pax-0.1.9/setup.py
+-rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 corpus_pax-0.1.9/PKG-INFO
```

### Comparing `corpus_pax-0.1.8/README.md` & `corpus_pax-0.1.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 # corpus-pax
 
-Initial, foundational sqlite tables with generic users, organizations, and articles.
+[sqlpyd](https://github.com/justmars/sqlpyd) tables: generic users, organizations, and articles.
 
 ```mermaid
 flowchart TB
 subgraph dev env
   pax[corpus-pax]
-  pax--run setup--->db[(sqlite.db)]
+  pax--run setup_pax--->db[(sqlite.db)]
 end
 subgraph /corpus-entities
   1(members)--github api---pax
   2(orgs)--github api---pax
 end
 subgraph /lawsql-articles
   3(articles)--github api---pax
 end
 pax--cloudflare api-->cf(cloudflare images)
 ```
 
+## Run
+
+```sh
+from corpus_pax import setup_pax
+setup_pax("x.db")
+```
+
+`setup_pax()` is a collection of 3 functions:
+
+1. `add_individuals_from_api()`
+2. `add_organizations_from_api()`
+3. `add_articles_from_api()`
+
+Since it's hard to correct the m2m tables, `setup_pax()` drops all the tables first, before adding content.
+
 ## Prerequisites
 
 Repository | Description
 --:|:--
 [corpus-entities](https://github.com/justmars/corpus-entities) | yaml-formatted member and org files
 [lawsql-articles](https://github.com/justmars/lawsql-articles) | markdown-styled articles with frontmatter
 
@@ -56,25 +71,7 @@
 #### Why Cloudflare Images
 
 Individuals and organizations have images stored in Github. To persist and optimize images for the web, I use [Cloudflare Images](https://www.cloudflare.com/products/cloudflare-images/) to take advantage of modern image formats and customizable variants.
 
 #### Why sqlite
 
 The initial data is simple. This database however will be the foundation for a more complicated schema. Sqlite seems a better fit for experimentation and future app use (Android and iOS rely on sqlite).
-
-## Steps
-
-Need to specify filename, e.g. ex.db, for this to created in the root directory of the project folder.
-
-Without the filename, the `Connection` (sqlite-utils' Database() under the hood) used is the path declared in $env.DB_FILE
-
-```python
-from sqlpyd import Connection  # this is sqlite-utils' Database() under the hood
-from corpus_pax import setup
-
-c = Connection(DatabasePath="ex.db", WALMode=False)
-setup_pax_db("x.db")
-```
-
-## Gotcha
-
-The m2m tables are not corrected when an update is made via `add_individuals_from_api()`, `add_organizations_from_api()` and `add_articles_from_api()`. To alleviate, simply reset the tables and recreate the same from scratch.
```

### Comparing `corpus_pax-0.1.8/corpus_pax/__main__.py` & `corpus_pax-0.1.9/corpus_pax/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from sqlpyd import Connection
 
 from .articles import Article
 from .entities import Individual, Org, OrgMember
 
-
-def reset_tables(c: Connection):
-    table_collection = [
-        # delete all area related tables
-        "pax_tbl_areas_pax_tbl_individuals",
-        "pax_tbl_areas_pax_tbl_orgs",
-        "pax_tbl_areas",
-        # delete all category related tables
-        "pax_tbl_categories_pax_tbl_individuals",
-        "pax_tbl_categories_pax_tbl_orgs",
-        "pax_tbl_categories",
-        # delete all org related tables
-        "pax_tbl_org_members",
-        "pax_tbl_orgs",
-        # delete all article related tables
-        "pax_tbl_articles_pax_tbl_individuals",
-        "pax_tbl_articles_pax_tbl_tags",
-        "pax_tbl_articles",
-        # finally, delete the individual table
-        "pax_tbl_individuals",
-    ]
-    for tbl in table_collection:
-        c.db.execute(f"drop table if exists {tbl}")
+TABLE_LIST = [
+    # delete all area related tables
+    "pax_tbl_areas_pax_tbl_individuals",
+    "pax_tbl_areas_pax_tbl_orgs",
+    "pax_tbl_areas",
+    # delete all category related tables
+    "pax_tbl_categories_pax_tbl_individuals",
+    "pax_tbl_categories_pax_tbl_orgs",
+    "pax_tbl_categories",
+    # delete all org related tables
+    "pax_tbl_org_members",
+    "pax_tbl_orgs_fts",
+    "pax_tbl_orgs",
+    # delete all article related tables
+    "pax_tbl_articles_pax_tbl_individuals",
+    "pax_tbl_articles_pax_tbl_tags",
+    "pax_tbl_articles_fts",
+    "pax_tbl_articles",
+    # finally, delete the individual table
+    "pax_tbl_individuals_fts",
+    "pax_tbl_individuals",
+]
 
 
 def init_person_tables(c: Connection) -> Connection:
     """Create tables related to persons, i.e. individuals, organizations, articles."""
 
     c.create_table(Individual)
     c.create_table(Org)
@@ -54,16 +53,17 @@
 
 def add_articles_from_api(c: Connection):
     """Add/replace records of articles from an API call."""
     for extracted_data in Article.extract_articles():
         Article.make_or_replace(c, extracted_data)
 
 
-def setup(db_path: str, replace_img: bool = False) -> Connection:
+def setup_pax(db_path: str, replace_img: bool = False) -> Connection:
     """Recreates tables and populates the same."""
     c = Connection(DatabasePath=db_path, WAL=True)
-    reset_tables(c)
+    for tbl in TABLE_LIST:
+        c.db.execute(f"drop table if exists {tbl}")
     init_person_tables(c)
     add_individuals_from_api(c, replace_img)
     add_organizations_from_api(c, replace_img)
     add_articles_from_api(c)
     return c
```

### Comparing `corpus_pax-0.1.8/corpus_pax/_api.py` & `corpus_pax-0.1.9/corpus_pax/_api.py`

 * *Files identical despite different names*

### Comparing `corpus_pax-0.1.8/corpus_pax/articles.py` & `corpus_pax-0.1.9/corpus_pax/articles.py`

 * *Files identical despite different names*

### Comparing `corpus_pax-0.1.8/corpus_pax/entities.py` & `corpus_pax-0.1.9/corpus_pax/entities.py`

 * *Files identical despite different names*

### Comparing `corpus_pax-0.1.8/corpus_pax/resources.py` & `corpus_pax-0.1.9/corpus_pax/resources.py`

 * *Files identical despite different names*

### Comparing `corpus_pax-0.1.8/pyproject.toml` & `corpus_pax-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "corpus-pax"
-version = "0.1.8"
+version = "0.1.9"
 description = "Using Github API (to pull individuals, orgs, and article content), setup a local sqlite database, syncing images to Cloudflare."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
+license = "MIT"
 homepage = "https://lawdata.xyz"
 repository = "https://github.com/justmars/corpus-pax"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
 ]
```

### Comparing `corpus_pax-0.1.8/setup.py` & `corpus_pax-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'httpx>=0.23.0,<0.24.0',
  'jinja2>=3.1.2,<4.0.0',
  'python-frontmatter>=1.0.0,<2.0.0',
  'sqlpyd>=0.1.1,<0.2.0']
 
 setup_kwargs = {
     'name': 'corpus-pax',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Using Github API (to pull individuals, orgs, and article content), setup a local sqlite database, syncing images to Cloudflare.',
-    'long_description': '# corpus-pax\n\nInitial, foundational sqlite tables with generic users, organizations, and articles.\n\n```mermaid\nflowchart TB\nsubgraph dev env\n  pax[corpus-pax]\n  pax--run setup--->db[(sqlite.db)]\nend\nsubgraph /corpus-entities\n  1(members)--github api---pax\n  2(orgs)--github api---pax\nend\nsubgraph /lawsql-articles\n  3(articles)--github api---pax\nend\npax--cloudflare api-->cf(cloudflare images)\n```\n\n## Prerequisites\n\nRepository | Description\n--:|:--\n[corpus-entities](https://github.com/justmars/corpus-entities) | yaml-formatted member and org files\n[lawsql-articles](https://github.com/justmars/lawsql-articles) | markdown-styled articles with frontmatter\n\nSince data concerning members will be pulled from such repositories, make sure the individual / org fields in [resources.py](corpus_pax/resources.py) match the data pulled from `corpus-entities`.\n\nEach avatar image should be named `avatar.jpeg` so that these can be uploaded to Cloudflare.\n\n## Install\n\n```zsh\npoetry add corpus-pax\npoetry update\n```\n\n## Supply .env\n\nCreate an .env file to create/populate the database. See [sample .env](.env.example) highlighting the following variables:\n\n1. Cloudflare `CF_ACCT`\n2. Cloudflare `CF_TOKEN`\n3. Github `GH_TOKEN`\n4. `DB_FILE` (sqlite)\n\nNote the [workflow](.github/workflows/main.yml) where the secrets are included for Github actions. Ensure these are set in the repository\'s `<url-to-repo>/settings/secrets/actions`, making the proper replacements when the tokens for Cloudflare and Github expire.\n\n### Notes\n\n#### Why Github\n\nThe names and profiles of individuals and organizations are stored in Github. These are pulled into the application via an API call requiring the use of a personal access token.\n\n#### Why Cloudflare Images\n\nIndividuals and organizations have images stored in Github. To persist and optimize images for the web, I use [Cloudflare Images](https://www.cloudflare.com/products/cloudflare-images/) to take advantage of modern image formats and customizable variants.\n\n#### Why sqlite\n\nThe initial data is simple. This database however will be the foundation for a more complicated schema. Sqlite seems a better fit for experimentation and future app use (Android and iOS rely on sqlite).\n\n## Steps\n\nNeed to specify filename, e.g. ex.db, for this to created in the root directory of the project folder.\n\nWithout the filename, the `Connection` (sqlite-utils\' Database() under the hood) used is the path declared in $env.DB_FILE\n\n```python\nfrom sqlpyd import Connection  # this is sqlite-utils\' Database() under the hood\nfrom corpus_pax import setup\n\nc = Connection(DatabasePath="ex.db", WALMode=False)\nsetup_pax_db("x.db")\n```\n\n## Gotcha\n\nThe m2m tables are not corrected when an update is made via `add_individuals_from_api()`, `add_organizations_from_api()` and `add_articles_from_api()`. To alleviate, simply reset the tables and recreate the same from scratch.\n',
+    'long_description': '# corpus-pax\n\n[sqlpyd](https://github.com/justmars/sqlpyd) tables: generic users, organizations, and articles.\n\n```mermaid\nflowchart TB\nsubgraph dev env\n  pax[corpus-pax]\n  pax--run setup_pax--->db[(sqlite.db)]\nend\nsubgraph /corpus-entities\n  1(members)--github api---pax\n  2(orgs)--github api---pax\nend\nsubgraph /lawsql-articles\n  3(articles)--github api---pax\nend\npax--cloudflare api-->cf(cloudflare images)\n```\n\n## Run\n\n```sh\nfrom corpus_pax import setup_pax\nsetup_pax("x.db")\n```\n\n`setup_pax()` is a collection of 3 functions:\n\n1. `add_individuals_from_api()`\n2. `add_organizations_from_api()`\n3. `add_articles_from_api()`\n\nSince it\'s hard to correct the m2m tables, `setup_pax()` drops all the tables first, before adding content.\n\n## Prerequisites\n\nRepository | Description\n--:|:--\n[corpus-entities](https://github.com/justmars/corpus-entities) | yaml-formatted member and org files\n[lawsql-articles](https://github.com/justmars/lawsql-articles) | markdown-styled articles with frontmatter\n\nSince data concerning members will be pulled from such repositories, make sure the individual / org fields in [resources.py](corpus_pax/resources.py) match the data pulled from `corpus-entities`.\n\nEach avatar image should be named `avatar.jpeg` so that these can be uploaded to Cloudflare.\n\n## Install\n\n```zsh\npoetry add corpus-pax\npoetry update\n```\n\n## Supply .env\n\nCreate an .env file to create/populate the database. See [sample .env](.env.example) highlighting the following variables:\n\n1. Cloudflare `CF_ACCT`\n2. Cloudflare `CF_TOKEN`\n3. Github `GH_TOKEN`\n4. `DB_FILE` (sqlite)\n\nNote the [workflow](.github/workflows/main.yml) where the secrets are included for Github actions. Ensure these are set in the repository\'s `<url-to-repo>/settings/secrets/actions`, making the proper replacements when the tokens for Cloudflare and Github expire.\n\n### Notes\n\n#### Why Github\n\nThe names and profiles of individuals and organizations are stored in Github. These are pulled into the application via an API call requiring the use of a personal access token.\n\n#### Why Cloudflare Images\n\nIndividuals and organizations have images stored in Github. To persist and optimize images for the web, I use [Cloudflare Images](https://www.cloudflare.com/products/cloudflare-images/) to take advantage of modern image formats and customizable variants.\n\n#### Why sqlite\n\nThe initial data is simple. This database however will be the foundation for a more complicated schema. Sqlite seems a better fit for experimentation and future app use (Android and iOS rely on sqlite).\n',
     'author': 'Marcelino G. Veloso III',
     'author_email': 'mars@veloso.one',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://lawdata.xyz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `corpus_pax-0.1.8/PKG-INFO` & `corpus_pax-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,65 @@
 Metadata-Version: 2.1
 Name: corpus-pax
-Version: 0.1.8
+Version: 0.1.9
 Summary: Using Github API (to pull individuals, orgs, and article content), setup a local sqlite database, syncing images to Cloudflare.
 Home-page: https://lawdata.xyz
+License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: ==3.11.0
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: email-validator (>=1.3.0,<2.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: python-frontmatter (>=1.0.0,<2.0.0)
 Requires-Dist: sqlpyd (>=0.1.1,<0.2.0)
 Project-URL: Repository, https://github.com/justmars/corpus-pax
 Description-Content-Type: text/markdown
 
 # corpus-pax
 
-Initial, foundational sqlite tables with generic users, organizations, and articles.
+[sqlpyd](https://github.com/justmars/sqlpyd) tables: generic users, organizations, and articles.
 
 ```mermaid
 flowchart TB
 subgraph dev env
   pax[corpus-pax]
-  pax--run setup--->db[(sqlite.db)]
+  pax--run setup_pax--->db[(sqlite.db)]
 end
 subgraph /corpus-entities
   1(members)--github api---pax
   2(orgs)--github api---pax
 end
 subgraph /lawsql-articles
   3(articles)--github api---pax
 end
 pax--cloudflare api-->cf(cloudflare images)
 ```
 
+## Run
+
+```sh
+from corpus_pax import setup_pax
+setup_pax("x.db")
+```
+
+`setup_pax()` is a collection of 3 functions:
+
+1. `add_individuals_from_api()`
+2. `add_organizations_from_api()`
+3. `add_articles_from_api()`
+
+Since it's hard to correct the m2m tables, `setup_pax()` drops all the tables first, before adding content.
+
 ## Prerequisites
 
 Repository | Description
 --:|:--
 [corpus-entities](https://github.com/justmars/corpus-entities) | yaml-formatted member and org files
 [lawsql-articles](https://github.com/justmars/lawsql-articles) | markdown-styled articles with frontmatter
 
@@ -78,25 +95,7 @@
 
 Individuals and organizations have images stored in Github. To persist and optimize images for the web, I use [Cloudflare Images](https://www.cloudflare.com/products/cloudflare-images/) to take advantage of modern image formats and customizable variants.
 
 #### Why sqlite
 
 The initial data is simple. This database however will be the foundation for a more complicated schema. Sqlite seems a better fit for experimentation and future app use (Android and iOS rely on sqlite).
 
-## Steps
-
-Need to specify filename, e.g. ex.db, for this to created in the root directory of the project folder.
-
-Without the filename, the `Connection` (sqlite-utils' Database() under the hood) used is the path declared in $env.DB_FILE
-
-```python
-from sqlpyd import Connection  # this is sqlite-utils' Database() under the hood
-from corpus_pax import setup
-
-c = Connection(DatabasePath="ex.db", WALMode=False)
-setup_pax_db("x.db")
-```
-
-## Gotcha
-
-The m2m tables are not corrected when an update is made via `add_individuals_from_api()`, `add_organizations_from_api()` and `add_articles_from_api()`. To alleviate, simply reset the tables and recreate the same from scratch.
-
```

