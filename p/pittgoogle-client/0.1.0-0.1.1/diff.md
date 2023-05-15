# Comparing `tmp/pittgoogle-client-0.1.0.tar.gz` & `tmp/pittgoogle_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/troyraen/Documents/broker/pittgoogle-client/pubsub/dist/tmpzlzz4p1a/pittgoogle-client-0.1.0.tar", last modified: Fri Jun 17 10:29:02 2022, max compression
+gzip compressed data, was "pittgoogle_client-0.1.1.tar", max compression
```

## Comparing `pittgoogle-client-0.1.0.tar` & `pittgoogle_client-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,9 @@
-drwxr-xr-x   0 troyraen   (501) staff       (20)        0 2022-06-17 10:29:02.000000 pittgoogle-client-0.1.0/
--rw-r--r--   0 troyraen   (501) staff       (20)     1516 2022-06-17 07:48:51.000000 pittgoogle-client-0.1.0/LICENSE.txt
--rw-r--r--   0 troyraen   (501) staff       (20)       25 2022-06-17 07:48:51.000000 pittgoogle-client-0.1.0/MANIFEST.in
--rw-r--r--   0 troyraen   (501) staff       (20)     1054 2022-06-17 10:29:02.000000 pittgoogle-client-0.1.0/PKG-INFO
--rw-r--r--   0 troyraen   (501) staff       (20)      317 2022-06-17 08:40:36.000000 pittgoogle-client-0.1.0/README.md
-drwxr-xr-x   0 troyraen   (501) staff       (20)        0 2022-06-17 10:29:02.000000 pittgoogle-client-0.1.0/pittgoogle/
--rw-r--r--   0 troyraen   (501) staff       (20)      721 2022-06-17 09:37:29.000000 pittgoogle-client-0.1.0/pittgoogle/__init__.py
--rw-r--r--   0 troyraen   (501) staff       (20)    24166 2022-06-17 10:19:48.000000 pittgoogle-client-0.1.0/pittgoogle/bigquery.py
--rw-r--r--   0 troyraen   (501) staff       (20)     4278 2022-06-17 07:48:51.000000 pittgoogle-client-0.1.0/pittgoogle/figures.py
--rw-r--r--   0 troyraen   (501) staff       (20)    12444 2022-06-17 07:48:51.000000 pittgoogle-client-0.1.0/pittgoogle/pubsub.py
--rw-r--r--   0 troyraen   (501) staff       (20)     2221 2022-06-17 07:48:51.000000 pittgoogle-client-0.1.0/pittgoogle/utils.py
-drwxr-xr-x   0 troyraen   (501) staff       (20)        0 2022-06-17 10:29:02.000000 pittgoogle-client-0.1.0/pittgoogle_client.egg-info/
--rw-r--r--   0 troyraen   (501) staff       (20)     1054 2022-06-17 10:29:01.000000 pittgoogle-client-0.1.0/pittgoogle_client.egg-info/PKG-INFO
--rw-r--r--   0 troyraen   (501) staff       (20)      397 2022-06-17 10:29:02.000000 pittgoogle-client-0.1.0/pittgoogle_client.egg-info/SOURCES.txt
--rw-r--r--   0 troyraen   (501) staff       (20)        1 2022-06-17 10:29:01.000000 pittgoogle-client-0.1.0/pittgoogle_client.egg-info/dependency_links.txt
--rw-r--r--   0 troyraen   (501) staff       (20)      138 2022-06-17 10:29:02.000000 pittgoogle-client-0.1.0/pittgoogle_client.egg-info/requires.txt
--rw-r--r--   0 troyraen   (501) staff       (20)       11 2022-06-17 10:29:02.000000 pittgoogle-client-0.1.0/pittgoogle_client.egg-info/top_level.txt
--rw-r--r--   0 troyraen   (501) staff       (20)      104 2022-06-17 07:48:51.000000 pittgoogle-client-0.1.0/pyproject.toml
--rw-r--r--   0 troyraen   (501) staff       (20)      238 2022-06-17 07:48:51.000000 pittgoogle-client-0.1.0/requirements.txt
--rw-r--r--   0 troyraen   (501) staff       (20)       78 2022-06-17 10:29:02.000000 pittgoogle-client-0.1.0/setup.cfg
--rw-r--r--   0 troyraen   (501) staff       (20)     2636 2022-06-17 08:53:48.000000 pittgoogle-client-0.1.0/setup.py
+-rw-r--r--   0        0        0     1516 2023-05-15 15:45:17.853955 pittgoogle_client-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      615 2023-05-15 15:45:17.853955 pittgoogle_client-0.1.1/README.md
+-rw-r--r--   0        0        0      680 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/__init__.py
+-rw-r--r--   0        0        0    23547 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/bigquery.py
+-rw-r--r--   0        0        0     4287 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/figures.py
+-rw-r--r--   0        0        0    12389 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/pubsub.py
+-rw-r--r--   0        0        0     2177 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/utils.py
+-rw-r--r--   0        0        0     1358 2023-05-15 15:45:39.595834 pittgoogle_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 pittgoogle_client-0.1.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pittgoogle-client-0.1.0/LICENSE.txt` & `pittgoogle_client-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pittgoogle-client-0.1.0/pittgoogle/__init__.py` & `pittgoogle_client-0.1.1/pittgoogle/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
 """Tools for interacting with Pitt-Google Broker data resources."""
 
-import pkg_resources  # part of setuptools
-import os as _os
-# from warnings import warn as _warn
-import logging
-
+try:
+    from importlib import metadata
 
-logger = logging.getLogger(__name__)
+except ImportError:  # for Python<3.8
+    import importlib_metadata as metadata
 
+import logging
+import os as os
 
 from . import bigquery, figures, pubsub, utils
 
+__version__ = metadata.version('pittgoogle-client')
 
-__version__ = pkg_resources.require("pittgoogle-client")[0].version
-
-
-env_vars = ['GOOGLE_CLOUD_PROJECT', 'GOOGLE_APPLICATION_CREDENTIALS']
-for var in env_vars:
-    if var not in _os.environ:
+for var in ["GOOGLE_CLOUD_PROJECT", "GOOGLE_APPLICATION_CREDENTIALS"]:
+    if var not in os.environ:
+        logger = logging.getLogger(__name__)
         logger.warning(
-            f'Warning: The environment variable {var} is not set. '
-            'This may impact your ability to connect to your '
-            'Google Cloud Platform project.'
+            f"Warning: The environment variable {var} is not set. "
+            "This may impact your ability to connect to your "
+            "Google Cloud Platform project."
         )
```

### Comparing `pittgoogle-client-0.1.0/pittgoogle/bigquery.py` & `pittgoogle_client-0.1.1/pittgoogle/bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,351 +1,387 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
 """The ``bigquery`` module facilitates querying Pitt-Google Broker's
 BigQuery databases and reading the results.
 """
 
+from typing import Generator, List, Optional, Tuple, Union
+
 import astropy
+import pandas as pd
 from astropy import coordinates as coord
 from google.cloud import bigquery
-import pandas as pd
 from tabulate import tabulate
-from typing import List, Tuple, Optional, Union, Generator
-
 
-pgb_project_id = 'ardent-cycling-243415'
+pgb_project_id = "ardent-cycling-243415"
 
-#--- BigQuery Client
+# --- BigQuery Client
 user_bq_client, user_project_id = None, None  # module's global Client, related id
 
+
 def create_client(project_id: str):
     """Open a BigQuery Client.
 
     Args:
         project_id: User's Google Cloud Platform project ID
     """
+
     global user_bq_client
     global user_project_id
 
     # instantiate the client
-    print(f'\nInstantiating a BigQuery client with project_id: {project_id}\n')
+    print(f"\nInstantiating a BigQuery client with project_id: {project_id}\n")
     user_bq_client = bigquery.Client(project=project_id)
 
     # if the user passed a bad project_id, we won't know it yet. Let's check
     _create_client_raise_exception_if_not_connected(project_id)
 
     # client is connected. set the global user_project_id
     user_project_id = project_id
 
+
 def _create_client_raise_exception_if_not_connected(project_id: str):
     """Checks that the user's client can successfully connect to our tables
     by executing a dry run query.
     """
+
     global user_bq_client
 
-    query = f'SELECT candid FROM `{pgb_project_id}.ztf_alerts.salt2`'
+    query = f"SELECT candid FROM `{pgb_project_id}.ztf_alerts.salt2`"
     try:
         dry_run(query, notify=False)
     except:
         user_bq_client = None  # reset so the user can try again
         msg = (
-            'You have tried to create a BigQuery Client with the project_id:\n'
-            f'\t{project_id}\n'
-            'But the Client cannot connect to the Pitt-Google Broker.\n'
-            'Check that your project_id is valid '
-            '(e.g., it should not be wrapped in quotes).'
+            "You have tried to create a BigQuery Client with the project_id:\n"
+            f"\t{project_id}\n"
+            "But the Client cannot connect to the Pitt-Google Broker.\n"
+            "Check that your project_id is valid "
+            "(e.g., it should not be wrapped in quotes)."
         )
         raise ValueError(msg)
 
+
 def _check_client_isinstance():
-    msg = ("You must create a BigQuery client first. "
-           "Run `pittgoogle.bigquery.create_client('your_project_id')`")
+    msg = (
+        "You must create a BigQuery client first. "
+        "Run `pittgoogle.bigquery.create_client('your_project_id')`"
+    )
     assert isinstance(user_bq_client, bigquery.client.Client), msg
 
+
 def _create_client_if_needed():
     stop = False  # will be set to True if the user chooses to exit
 
     try:
         _check_client_isinstance()
 
     except AssertionError:
         # help the user open a bigquery client
-        msg = ('\nTo run queries, you must first open a BigQuery Client.\n'
-               'Enter your Google Cloud Platform project ID now '
-               'or exit (just press Enter) and run\n'
-               '`pittgoogle.bigquery.create_client(my_project_id)`\n'
-               '\nProject ID: '
+        msg = (
+            "\nTo run queries, you must first open a BigQuery Client.\n"
+            "Enter your Google Cloud Platform project ID now "
+            "or exit (just press Enter) and run\n"
+            "`pittgoogle.bigquery.create_client(my_project_id)`\n"
+            "\nProject ID: "
         )
-        project_id = input(msg) or ''
+        project_id = input(msg) or ""
 
-        if project_id == '':
+        if project_id == "":
             stop = True  # user wants to exit rather than creating a client
         else:
             create_client(project_id)
 
     return stop
 
 
-#--- Get information about PGB datasets and tables
-def get_table_info(table: Union[str,list] = 'all', dataset: str ='ztf_alerts'):
+# --- Get information about PGB datasets and tables
+def get_table_info(table: Union[str, list] = "all", dataset: str = "ztf_alerts"):
     """Retrieves and prints BigQuery table schemas.
 
     Args:
 
         table: Name of the BigQuery table or list of the same.
                'all' will print the info for all tables in the dataset.
 
         dataset: Name of BigQuery dataset that the table(s) belong to.
     """
+
     # if a bigquery Client does not exist, help the user instantiate one
     stop = _create_client_if_needed()
     if stop:  # the user has chosen to exit rather than create a client
         return
 
     # get the table names in a list
-    if table == 'all':
+    if table == "all":
         tables = get_dataset_table_names(dataset=dataset)
     elif type(table) == str:
         tables = [table]
     else:
         tables = table
 
     # get and print info about each table
     for t in tables:
         df = get_table_schema(table=t, dataset=dataset)
 
         # print the metadata and column info
         print(df.table_name)
-        print(tabulate(df, headers='keys', tablefmt='grid'))  # psql
-        print(f'\n{df.table_name} has {df.num_rows} rows.\n')
+        print(tabulate(df, headers="keys", tablefmt="grid"))  # psql
+        print(f"\n{df.table_name} has {df.num_rows} rows.\n")
 
-def get_table_schema(table: str, dataset: str ='ztf_alerts') -> pd.DataFrame:
+
+def get_table_schema(table: str, dataset: str = "ztf_alerts") -> pd.DataFrame:
     """Retrieves information about the columns in a BigQuery table and returns
     it as a DataFrame.
 
     Args:
         table: Name of the BigQuery table
         dataset: Name of BigQuery dataset that the table(s) belong to.
     Returns
-        df: Column information from the BigQuery table schema.
+        Column information from the BigQuery table schema.
     """
+
     # if a bigquery Client does not exist, help the user instantiate one
     stop = _create_client_if_needed()
     if stop:  # the user has chosen to exit rather than create a client
         return
 
-    bqtable = user_bq_client.get_table(f'{pgb_project_id}.{dataset}.{table}')
+    bqtable = user_bq_client.get_table(f"{pgb_project_id}.{dataset}.{table}")
     cols = []
     for field in bqtable.schema:
         cols.append((field.name, field.description, field.field_type))
 
-        if field.field_type == 'RECORD':
+        if field.field_type == "RECORD":
             for subfield in field.fields:
-                cols.append((f'{field.name}.{subfield.name}', subfield.description, subfield.field_type))
+                cols.append(
+                    (
+                        f"{field.name}.{subfield.name}",
+                        subfield.description,
+                        subfield.field_type,
+                    )
+                )
 
     # cols = [(s.name, s.description, s.field_type, s.mode) for s in bqtable.schema]
-    colnames = ['column_name', 'description', 'type']
+    colnames = ["column_name", "description", "type"]
     df = pd.DataFrame(cols, columns=colnames)
 
     # add some metadata
-    df.table_name = f'{bqtable.project}.{bqtable.dataset_id}.{bqtable.table_id}'
+    df.table_name = f"{bqtable.project}.{bqtable.dataset_id}.{bqtable.table_id}"
     df.num_rows = bqtable.num_rows
 
     return df
 
-def get_dataset_table_names(dataset: str ='ztf_alerts') -> List[str]:
+
+def get_dataset_table_names(dataset: str = "ztf_alerts") -> List[str]:
     """
     Args:
         dataset: Name of the BigQuery dataset.
 
     Returns:
-        tables: List of table names in the dataset.
+        List of table names in the dataset.
     """
+
     # if a bigquery Client does not exist, help the user instantiate one
     stop = _create_client_if_needed()
     if stop:  # the user has chosen to exit rather than create a client
         return
 
-    print(f'Getting table names for dataset: {dataset}')
+    print(f"Getting table names for dataset: {dataset}")
 
-    query = (
-        'SELECT * '
-        f'FROM {pgb_project_id}.{dataset}.INFORMATION_SCHEMA.TABLES'
-    )
+    query = "SELECT * " f"FROM {pgb_project_id}.{dataset}.INFORMATION_SCHEMA.TABLES"
     query_job = user_bq_client.query(query)
-    tables = [row['table_name'] for row in query_job]
+    tables = [row["table_name"] for row in query_job]
     tables.sort(key=str.lower)
     return tables
 
 
-#--- Setup to query for object histories
+# --- Setup to query for object histories
 def get_history_column_names() -> List[str]:
     """
+    It would be convenient to also return the column descriptions, but
+    that is more complicated, and this function will be completely
+    obsolete if we change the database structure to store only the
+    "candidate" observation and metadata.
+
     Returns:
-        historycols: Column names appropriate for querying object histories.
+        Column names appropriate for querying object histories.
+    """
 
-    Note: It would be convenient to also return the column descriptions, but
-         that is more complicated, and this function will be completely
-         obsolete if we change the database structure to store only the
-         "candidate" observation and metadata.
-    """
-    objectcols = ['objectId',]
-    flatcols = ['schemavsn','publisher','candid',]
-    dropcols = ['prv_candidates', 'cutoutScience', 'cutoutDifference', 'cutoutTemplate']
+    dropcols = ["prv_candidates", "cutoutScience", "cutoutDifference", "cutoutTemplate"]
 
-    sdf = get_table_schema('alerts')
-    schemacols = list(sdf['column_name'])
+    sdf = get_table_schema("alerts")
+    schemacols = list(sdf["column_name"])
 
     # drop the prv_candidates and cutout columns
-    historycols = [c for c in schemacols if c.split('.')[0] not in dropcols]
+    historycols = [c for c in schemacols if c.split(".")[0] not in dropcols]
 
     # drop the full "candidate" RECORD column
-    historycols.remove('candidate')
+    historycols.remove("candidate")
 
     # drop "candidate.candid" as it is simply a repeat of "candid"
-    historycols.remove('candidate.candid')
+    historycols.remove("candidate.candid")
 
     # strip out "candidate." from nested columns
     # query_objects() uses only the base names
-    historycols = [c.replace('candidate.','') for c in historycols]
+    historycols = [c.replace("candidate.", "") for c in historycols]
 
     return historycols
 
-def check_history_column_names(columns: List[str]) -> Union[List[str],bool]:
-    """Make sure user-submitted column names are appropriate to query object histories.
-    """
 
-def _split_good_bad_history_column_names(columns: List[str]) -> Tuple[List[str],List[str]]:
+def check_history_column_names(columns: List[str]) -> Union[List[str], bool]:
+    """Make sure user-submitted column names are appropriate to query object histories."""
+
+
+def _split_good_bad_history_column_names(
+    columns: List[str],
+) -> Tuple[List[str], List[str]]:
     """Split columns list into "good" and "bad" according to whether they are
     suitable for querying an object's history.
     """
+
     badcols = list(set(columns) - set(get_history_column_names()))
     goodcols = columns.copy()
     for bc in badcols:
         goodcols.remove(bc)
     return (goodcols, badcols)
 
-def object_history_sql_statement(columns: List[str],
-                                 objectIds: Optional[list] = None,
-                                 limit: Optional[int] = None
-                                 ) -> str:
-    """Convience function that generates the SQL string needed to
+
+def object_history_sql_statement(
+    columns: List[str], objectIds: Optional[list] = None, limit: Optional[int] = None
+) -> str:
+    """Convince function that generates the SQL string needed to
     query the alerts table and aggregate data by objectId.
     When the resulting SQL query is executed, the query job will contain
     one row for each objectId, with the object's data aggregated into
     arrays (one array per column in columns) ordered by the observation date.
 
     Note: Arrays may contain duplicated observations; it is the user's
-    responsiblity to clean them.
+    responsibility to clean them.
 
     Args:
         columns: Names of columns to select from the alerts table.
                  The 'objectId' and 'candid' columns are automatically included
                  and do not need to be in this list.
         objectIds: IDs of ZTF objects to include in the query.
         limit: Maximum number of rows to be returned.
 
     Returns:
-        query: SQL statement to query the alerts table and aggregate data by objectId.
+        SQL statement to query the alerts table and aggregate data by objectId.
     """
-    dataset = 'ztf_alerts'
-    table = 'alerts'
-    objectcols = ['objectId',]  # columns unique to an object
+
+    dataset = "ztf_alerts"
+    table = "alerts"
+    objectcols = [
+        "objectId",
+    ]  # columns unique to an object
     # make sure 'candid' is in columns. (objectcols handled separately)
-    columns = list(set(columns).union(set(['candid'])))
+    columns = list(set(columns).union(set(["candid"])))
 
     # SELECT statement
     # create a list of strings that will aggregate columns into arrays
     aggcols = _list_aggcols_sql_statements(columns)
     selects = f'SELECT {", ".join(objectcols + aggcols)}'
 
     # FROM statement
-    froms = f'FROM `{pgb_project_id}.{dataset}.{table}`'
+    froms = f"FROM `{pgb_project_id}.{dataset}.{table}`"
     # concat the statements into the beginning of a SQL query statement
-    sqlquery = ' '.join([selects, froms])
+    sqlquery = " ".join([selects, froms])
 
     # WHERE statement
     if objectIds is not None:
         # wrap each objectId in quotes and join to single string
-        oids = ','.join([f'"{o}"' for o in objectIds])
-        wheres = f'WHERE objectId IN ({oids})'
+        oids = ",".join([f'"{o}"' for o in objectIds])
+        wheres = f"WHERE objectId IN ({oids})"
         # concat the statements into a SQL query statement
-        sqlquery = ' '.join([sqlquery, wheres])
+        sqlquery = " ".join([sqlquery, wheres])
 
     # GROUP BY statement
-    groupbys = f'GROUP BY objectId'
-    sqlquery = ' '.join([sqlquery, groupbys])
+    groupbys = f"GROUP BY objectId"
+    sqlquery = " ".join([sqlquery, groupbys])
 
     # LIMIT statement
     if limit is not None:
-        limits = f'LIMIT {limit}'
-        sqlquery = ' '.join([sqlquery, limits])
+        limits = f"LIMIT {limit}"
+        sqlquery = " ".join([sqlquery, limits])
 
     return sqlquery
 
+
 def _list_aggcols_sql_statements(columns: List[str]) -> List[str]:
     """Create a list of SQL string query segments that will aggregate
     all columns not in objectcols.
     """
-    objectcols = ['objectId',]
-    flatcols = ['schemavsn','publisher','candid',]
+
+    objectcols = [
+        "objectId",
+    ]
+    flatcols = [
+        "schemavsn",
+        "publisher",
+        "candid",
+    ]
 
     # list of requested flatcols
     fcols = list(set(columns) & set(flatcols))
     # list of requested columns nested under 'candidate'
     ncols = list(set(columns) - set(objectcols) - set(flatcols))
-    ncols = [f'candidate.{c}' for c in ncols]
+    ncols = [f"candidate.{c}" for c in ncols]
     # complete list of columns to be aggregated (group by) objectId
     aggcols = fcols + ncols
     # attach the ARRAY_AGG, ORDER By, and AS statements to the aggcols
-    aggcols = [f'ARRAY_AGG({c} ORDER BY candidate.jd) AS {c.split(".")[-1]}' for c in aggcols]
+    aggcols = [
+        f'ARRAY_AGG({c} ORDER BY candidate.jd) AS {c.split(".")[-1]}' for c in aggcols
+    ]
 
     return aggcols
 
 
-#--- Dry runs
+# --- Dry runs
 def dry_run(query: str, notify: bool = True):
     """Perform a dry run to find out how many bytes the query will process.
     Args:
         query: SQL query statement
     """
+
     global user_project_id
     _check_client_isinstance()  # make sure we have a bigquery.client
 
     job_config = bigquery.QueryJobConfig(dry_run=True, use_query_cache=False)
     query_job = user_bq_client.query(query, job_config=job_config)
 
     if notify:
-        nbytes, TiB = query_job.total_bytes_processed, 2**40
-        pTiB = nbytes/TiB*100  # nbytes as a percent of 1 TiB
-        print(f'\nQuery statement:')
+        nbytes, TiB = query_job.total_bytes_processed, 2 ** 40
+        pTiB = nbytes / TiB * 100  # nbytes as a percent of 1 TiB
+        print(f"\nQuery statement:")
         print(f'\n"{query}"\n')
-        print(f'will process {nbytes} bytes of data.')
-        print(f'({pTiB:.3}% of your 1 TiB Free Tier monthly allotment.)')
+        print(f"will process {nbytes} bytes of data.")
+        print(f"({pTiB:.3}% of your 1 TiB Free Tier monthly allotment.)")
+
 
 def _dry_run_and_confirm(query: str) -> bool:
     # print dry run info
     dry_run(query)
     # ask user if they want to proceed
-    cont = input('Continue? [y/N]: ') or 'N'
-    do_the_query = cont in ['y','Y']
+    cont = input("Continue? [y/N]: ") or "N"
+    do_the_query = cont in ["y", "Y"]
     return do_the_query
 
 
-#--- Query for object histories
-def query_objects(columns: List[str],
-                  objectIds: Optional[list] = None,
-                  limit: Optional[int] = None,
-                  format: str = 'pandas',
-                  iterator: bool = False,
-                  dry_run: bool = True
-                  ) -> Union[str,
-                             pd.DataFrame,
-                             bigquery.job.QueryJob,
-                             Generator[Union[str, pd.DataFrame], None, None]]:
+# --- Query for object histories
+def query_objects(
+    columns: List[str],
+    objectIds: Optional[list] = None,
+    limit: Optional[int] = None,
+    format: str = "pandas",
+    iterator: bool = False,
+    dry_run: bool = True,
+) -> Union[
+    str,
+    pd.DataFrame,
+    bigquery.job.QueryJob,
+    Generator[Union[str, pd.DataFrame], None, None],
+]:
     """Query the alerts database for object histories.
 
     Args:
         columns: Names of columns to select from the alerts table.
                  The 'objectId' and 'candid' columns are automatically included
                  and do not need to be in this list.
         objectIds: IDs of ZTF objects to include in the query.
@@ -355,16 +391,16 @@
                 contain duplicate observations; else duplicates are dropped.
         iterator: If True, iterate over the objects and return one at a time.
                   Else return the full query results together.
                   This parameter is ignored if `format` == 'query_job'.
         dry_run: If True, `pittgoogle.bigquery.dry_run` will be called first and the
                  user will be asked to confirm before continuing.
 
-    Returns: Query results in the requested format. If `iterator` is True,
-             yields one object at a time; else all results are returned together.
+    Returns:
+        Query results in the requested format.
     """
 
     # make sure we have appropriate column names
     goodcols = _query_objects_check_history_column_names(columns)
     if len(goodcols) == 0:  # user submitted bad columns and wants to abort
         return
 
@@ -382,49 +418,58 @@
         if not do_the_query:  # user has chosen to abort the query
             return
 
     # make the API call
     query_job = user_bq_client.query(query)
 
     # return the results
-    if format == 'query_job':
+    if format == "query_job":
         return query_job
     elif iterator:  # return a generator that cycles through the objects/rows
-        return (format_history_query_results(row=row, format=format) for row in query_job)
+        return (
+            format_history_query_results(row=row, format=format) for row in query_job
+        )
     else:  # format and return all rows at once
         return format_history_query_results(query_job=query_job, format=format)
 
+
 def _query_objects_check_history_column_names(columns: List[str]) -> List[str]:
     """Make sure user-submitted column names are appropriate for `query_objects()`.
+
     Returns one of:
         Columns stripped of bad column names.
         Empty list if there were bad columns and the user wants to abort the query.
     """
+
     goodcols, badcols = _split_good_bad_history_column_names(columns)
 
     try:
         assert len(badcols) == 0
     except AssertionError:
         msg = (
-            '\nYou have requested columns that are not available to `query_objects()`.\n'
-            '(To view available columns, use `pittgoogle.bigquery.get_history_column_names()`)\n'
-            f'\nRequested columns:\n\t{columns}\n'
-            f'Unavailable columns:\n\t{badcols}\n'
-            '\nProceed without the unavailable columns? [y/N] '
+            "\nYou have requested columns that are not available to `query_objects()`.\n"
+            "(To view available columns, use `pittgoogle.bigquery.get_history_column_names()`)\n"
+            f"\nRequested columns:\n\t{columns}\n"
+            f"Unavailable columns:\n\t{badcols}\n"
+            "\nProceed without the unavailable columns? [y/N] "
         )
-        proceed = input(msg) or 'N'
+        proceed = input(msg) or "N"
 
-        if proceed not in ['y','Y']:  # user wants to exit; return an empty list
+        if proceed not in ["y", "Y"]:  # user wants to exit; return an empty list
             return []
 
     return goodcols
 
 
-#--- Format query results
-def format_history_query_results(query_job: Optional[bigquery.job.QueryJob] = None, row: Optional[bigquery.table.Row] = None, format: str = 'pandas') -> Union[pd.DataFrame,str]:
+# --- Format query results
+def format_history_query_results(
+    query_job: Optional[bigquery.job.QueryJob] = None,
+    row: Optional[bigquery.table.Row] = None,
+    format: str = "pandas",
+) -> Union[pd.DataFrame, str]:
     """Converts the results of a BigQuery query to the desired format.
     Must pass either query_job or row.
     Any duplicate observations will be dropped.
 
     Args:
         query_job: Results from a object history query job. SQL statement needed
                    to create the job can be obtained with object_history_sql_statement().
@@ -434,77 +479,81 @@
 
         format: One of 'pandas' or 'json'. Input query results will be returned
                 in this format.
 
     Returns:
         histories: Input query results converted to requested format
     """
+
     # make sure we have an appropriate param combination
     do_job, do_row = query_job is not None, row is not None
-    good_format = format in ['pandas','json']
+    good_format = format in ["pandas", "json"]
     good_combo = (do_job != do_row) and good_format
     if not good_combo:
-        raise ValueError('Must pass one of query_job or row.')
+        raise ValueError("Must pass one of query_job or row.")
 
     # convert query_job
     if do_job:
         histories = _format_history_query_results_to_df(query_job)  # df
-        if format == 'json':
+        if format == "json":
             histories = histories.reset_index().to_json()  # str
 
     # convert row
     if do_row:
         histories = _format_history_row_to_df(row)  # df
-        if format == 'json':
-            histories['objectId'] = histories.objectId  # persist metadata
+        if format == "json":
+            histories["objectId"] = histories.objectId  # persist metadata
             histories = histories.reset_index().to_json()  # str
 
     return histories
 
+
 def _format_history_query_results_to_df(query_job: bigquery.job.QueryJob):
     """Convert a query_job (containing multiple rows of object history data)
     to a DataFrame.
     Any duplicate observations will be dropped.
     """
+
     dflist = []
     for r, row in enumerate(query_job):
         # convert to DataFrame
         df = _format_history_row_to_df(row)
         # add the objectId so we can use it to multi-index
-        df['objectId'] = df.objectId
+        df["objectId"] = df.objectId
         # set the multi-index and append to the list
-        dflist.append(df.reset_index().set_index(['objectId','candid']))
+        dflist.append(df.reset_index().set_index(["objectId", "candid"]))
 
     histories = pd.concat(dflist)
 
     return histories
 
-def _format_history_row_to_df(row: Union[dict,bigquery.table.Row]):
+
+def _format_history_row_to_df(row: Union[dict, bigquery.table.Row]):
     """Convert a single object's history from a query row to a DataFrame.
     Any duplicate observations will be dropped.
     """
+
     d = dict(row.items())
-    oid, cid = d.pop('objectId'), d.pop('candid')
-    df = pd.DataFrame(data=d, index=pd.Index(cid, name='candid'))
+    oid, cid = d.pop("objectId"), d.pop("candid")
+    df = pd.DataFrame(data=d, index=pd.Index(cid, name="candid"))
     df.drop_duplicates(inplace=True)
     df.objectId = oid
     return df
 
 
-#--- Cone Search
-def cone_search(center: astropy.coordinates.SkyCoord,
-                radius: astropy.coordinates.Angle,
-                columns: List[str],
-                objectIds: Optional[list] = None,
-                format: str = 'pandas',
-                iterator: bool = False,
-                dry_run: bool = True,
-                ) -> Union[str,
-                           pd.DataFrame,
-                           Generator[Union[str, pd.DataFrame], None, None]]:
+# --- Cone Search
+def cone_search(
+    center: astropy.coordinates.SkyCoord,
+    radius: astropy.coordinates.Angle,
+    columns: List[str],
+    objectIds: Optional[list] = None,
+    format: str = "pandas",
+    iterator: bool = False,
+    dry_run: bool = True,
+) -> Union[str, pd.DataFrame, Generator[Union[str, pd.DataFrame], None, None]]:
     """Perform a cone search on the alerts database and return object histories.
     This uses the coordinates of the most recent observation to determine
     whether an object is within the cone.
 
     Args:
         center: Center of the cone to search within.
         radius: Radius of the cone to search within.
@@ -515,106 +564,129 @@
         format: One of 'pandas', or 'json'. Query results will be
                 returned in this format. Duplicate observations are dropped.
         iterator: If True, iterate over the objects and return one at a time.
                   Else return the full query results together.
         dry_run: If True, `pittgoogle.bigquery.dry_run` will be called first and the
                  user will be asked to confirm before continuing.
 
-    Returns: Query results in the requested format. If `iterator` is True,
-             returns a generator; else all results are returned together.
+    Returns:
+        Query results in the requested format.
     """
+
     # make sure we have required columns
-    for c in ['jd', 'ra', 'dec']:
-        if c not in columns: columns.append(c)
+    for c in ["jd", "ra", "dec"]:
+        if c not in columns:
+            columns.append(c)
 
     # Performing a dry run prints the SQL query statement, which does not account
     # for the cone search. We'll print some things to reduce user confusion.
-    if dry_run: print('\nInitiating a cone search.')
+    if dry_run:
+        print("\nInitiating a cone search.")
 
     # Query the database for object histories.
-    objects = query_objects(columns,
-                            objectIds = objectIds,
-                            format = 'pandas',
-                            iterator=iterator,
-                            dry_run=dry_run
-                            )
+    objects = query_objects(
+        columns,
+        objectIds=objectIds,
+        format="pandas",
+        iterator=iterator,
+        dry_run=dry_run,
+    )
     # == None if user chose to abort; else DataFrame or generator of same
     if objects is None:
         return
 
-    if dry_run: print('\nFiltering for objects within the given cone.')
+    if dry_run:
+        print("\nFiltering for objects within the given cone.")
 
     # filter out objects not in the cone and return the rest
     objects_in_cone = _do_cone_search(objects, center, radius, format, iterator)
     return objects_in_cone
 
 
-def _do_cone_search(objects: Union[pd.DataFrame,Generator[pd.DataFrame, None, None]],
-                    center: astropy.coordinates.SkyCoord,
-                    radius: astropy.coordinates.Angle,
-                    format: str = 'pandas',
-                    iterator: bool = False,
-                    ) -> Union[str,
-                               pd.DataFrame,
-                               Generator[Union[str, pd.DataFrame], None, None]]:
-    """Apply the cone search filter and return appropriate objects.
-    """
+def _do_cone_search(
+    objects: Union[pd.DataFrame, Generator[pd.DataFrame, None, None]],
+    center: astropy.coordinates.SkyCoord,
+    radius: astropy.coordinates.Angle,
+    format: str = "pandas",
+    iterator: bool = False,
+) -> Union[str, pd.DataFrame, Generator[Union[str, pd.DataFrame], None, None]]:
+    """Apply the cone search filter and return appropriate objects."""
 
     if iterator:  # objects is a generator, return a generator
         return _do_cone_search_iterator(objects, center, radius, format)
 
     else:  # objects is single df
         return _do_cone_search_all(objects, center, radius, format)
 
-def _do_cone_search_iterator(objects: pd.DataFrame, center: astropy.coordinates.SkyCoord, radius: astropy.coordinates.Angle, format):
+
+def _do_cone_search_iterator(
+    objects: pd.DataFrame,
+    center: astropy.coordinates.SkyCoord,
+    radius: astropy.coordinates.Angle,
+    format,
+):
     """Iterate objects, format and yield those that are in the cone.
 
     Args:
         objects: DataFrame containing histories of multiple objectIds.
     """
+
     for df in objects:
         in_cone = object_is_in_cone(df, center, radius)
 
         if in_cone:  # format and yield
-            if format == 'json':
-                df['objectId'] = df.objectId  # else metadata is lost
+            if format == "json":
+                df["objectId"] = df.objectId  # else metadata is lost
                 object = df.reset_index().to_json()  # str
             else:
                 object = df
             yield object
 
-def _do_cone_search_all(objects: pd.DataFrame, center: astropy.coordinates.SkyCoord, radius: astropy.coordinates.Angle, format):
+
+def _do_cone_search_all(
+    objects: pd.DataFrame,
+    center: astropy.coordinates.SkyCoord,
+    radius: astropy.coordinates.Angle,
+    format,
+):
     """Filter out objects not in the cone, format, and return.
 
     Args:
         objects: DataFrame containing histories of multiple objectIds.
     """
-    gb = objects.groupby(level='objectId')
-    objects_in_cone = gb.filter(lambda df: object_is_in_cone(df,center,radius))
-    if format == 'json':
+
+    gb = objects.groupby(level="objectId")
+    objects_in_cone = gb.filter(lambda df: object_is_in_cone(df, center, radius))
+    if format == "json":
         objects_in_cone = objects_in_cone.reset_index().to_json()  # str
     return objects_in_cone
 
-def object_is_in_cone(object: pd.DataFrame, center: astropy.coordinates.SkyCoord, radius: astropy.coordinates.Angle):
+
+def object_is_in_cone(
+    object: pd.DataFrame,
+    center: astropy.coordinates.SkyCoord,
+    radius: astropy.coordinates.Angle,
+):
     """Checks whether the object's most recent observation has a position that
     is within a cone defined by center and radius.
 
     Args:
         object: DataFrame containing the history of a single objectId.
                 Required columns: ['jd','ra','dec']
         center: Center of the cone to search within.
         radius: Radius of the cone to search within.
 
     Returns:
-        in_cone: True if object is within radius of center, else False
+        True if object is within radius of center, else False
     """
+
     # get the SkyCoords of the most recent observation
     # to do: use the epoch with highest S/N instead
-    obs = object.loc[object['jd']==object['jd'].max(),:]
-    obs_coords = coord.SkyCoord(obs['ra'], obs['dec'], frame='icrs', unit='deg')
+    obs = object.loc[object["jd"] == object["jd"].max(), :]
+    obs_coords = coord.SkyCoord(obs["ra"], obs["dec"], frame="icrs", unit="deg")
 
     # check whether obs_coords are within the cone
     dist = center.separation(obs_coords)
     in_cone = dist < radius  # array with a single bool
     in_cone = in_cone[0]
 
     return in_cone
```

### Comparing `pittgoogle-client-0.1.0/pittgoogle/figures.py` & `pittgoogle_client-0.1.1/pittgoogle/figures.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,127 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
 """``figures`` contains functions for plotting alert and history data.
 """
 
-import aplpy
-from astropy.io import fits
-from astropy.time import Time
 import gzip
 import io
+from typing import Optional
+
+import aplpy
 import matplotlib as mpl
-from matplotlib import pyplot as plt
 import numpy as np
 import pandas as pd
-from typing import Optional
+from astropy.io import fits
+from astropy.time import Time
+from matplotlib import pyplot as plt
 
 from . import utils as pgbu
 
 
-#--- Plot object history
-def plot_lightcurve(dflc: pd.DataFrame,
-                    objectId: Optional[str] = None,
-                    ax: Optional[mpl.axes.Axes] = None,
-                    days_ago: bool = True,
-                    ):
+# --- Plot object history
+def plot_lightcurve(
+    dflc: pd.DataFrame,
+    objectId: Optional[str] = None,
+    ax: Optional[mpl.axes.Axes] = None,
+    days_ago: bool = True,
+):
     """Plot the lighcurve (per band) of a single ZTF object.
     Adapted from:
     https://github.com/ZwickyTransientFacility/ztf-avro-alert/blob/master/notebooks/Filtering_alerts.ipynb
 
     Args:
         dflc: Lightcurve history of a unique objectId. Must contain columns
               ['jd','fid','magpsf','sigmapsf','diffmaglim']
         objectId: objectId identifying dflc. Used for plot title.
         ax: matplotlib axes for the figure. If None, a new figure will be created
         days_ago: If True, x-axis will be number of days in the past.
                   Else x-axis will be Julian date.
     """
 
     filter_code = pgbu.ztf_fid_names()  # dict
-    filter_color = {1:'green', 2:'red', 3:'pink'}
+    filter_color = {1: "green", 2: "red", 3: "pink"}
 
     # set the x-axis (time) details
     if days_ago:
         now = Time.now().jd
         t = dflc.jd - now
-        xlabel = 'Days Ago'
+        xlabel = "Days Ago"
     else:
         t = dflc.jd
-        xlabel = 'Time (JD)'
+        xlabel = "Time (JD)"
 
     if ax is None:
         plt.figure()
 
     # plot lightcurves by band
     for fid, color in filter_color.items():
         # plot detections in this filter:
         w = (dflc.fid == fid) & ~dflc.magpsf.isnull()
         if np.sum(w):
-            label = f'{fid}: {filter_code[fid]}'
-            kwargs = {'fmt':'.', 'color':color, 'label':label}
-            plt.errorbar(t[w],dflc.loc[w,'magpsf'], dflc.loc[w,'sigmapsf'], **kwargs)
+            label = f"{fid}: {filter_code[fid]}"
+            kwargs = {"fmt": ".", "color": color, "label": label}
+            plt.errorbar(t[w], dflc.loc[w, "magpsf"], dflc.loc[w, "sigmapsf"], **kwargs)
         # plot nondetections in this filter
         wnodet = (dflc.fid == fid) & dflc.magpsf.isnull()
         if np.sum(wnodet):
-            plt.scatter(t[wnodet],dflc.loc[wnodet,'diffmaglim'], marker='v',color=color,alpha=0.25)
+            plt.scatter(
+                t[wnodet],
+                dflc.loc[wnodet, "diffmaglim"],
+                marker="v",
+                color=color,
+                alpha=0.25,
+            )
 
     plt.gca().invert_yaxis()
     plt.xlabel(xlabel)
-    plt.ylabel('Magnitude')
+    plt.ylabel("Magnitude")
     plt.legend()
-    plt.title(f'objectId: {objectId}')
+    plt.title(f"objectId: {objectId}")
 
 
-#--- Plot cutouts
+# --- Plot cutouts
 def plot_stamp(stamp, fig=None, subplot=None, **kwargs):
     """Adapted from:
     https://github.com/ZwickyTransientFacility/ztf-avro-alert/blob/master/notebooks/Filtering_alerts.ipynb
     """
-    with gzip.open(io.BytesIO(stamp), 'rb') as f:
+
+    with gzip.open(io.BytesIO(stamp), "rb") as f:
         with fits.open(io.BytesIO(f.read())) as hdul:
             if fig is None:
-                fig = plt.figure(figsize=(4,4))
+                fig = plt.figure(figsize=(4, 4))
             if subplot is None:
-                subplot = (1,1,1)
-            ffig = aplpy.FITSFigure(hdul[0],figure=fig, subplot=subplot, **kwargs)
-            
+                subplot = (1, 1, 1)
+            ffig = aplpy.FITSFigure(hdul[0], figure=fig, subplot=subplot, **kwargs)
+
             # the following has been throwing: `ValueError: a must be > 0 and <= 1`
             # this is fixed by requiring astropy==3.2.1
             # Note: I see this related thing: https://github.com/aplpy/aplpy/issues/420
             # but I am using the latest APLpy version (2.0.3).
-            ffig.show_grayscale(stretch='arcsinh')
+            ffig.show_grayscale(stretch="arcsinh")
     return ffig
 
+
 def plot_cutouts(alert_dict):
     """Adapted from:
     https://github.com/ZwickyTransientFacility/ztf-avro-alert/blob/master/notebooks/Filtering_alerts.ipynb
     """
-    #fig, axes = plt.subplots(1,3, figsize=(12,4))
-    fig = plt.figure(figsize=(12,4))
-    for i, cutout in enumerate(['Science','Template','Difference']):
-        stamp = alert_dict['cutout{}'.format(cutout)]['stampData']
-        ffig = plot_stamp(stamp, fig=fig, subplot = (1,3,i+1))
+
+    # fig, axes = plt.subplots(1,3, figsize=(12,4))
+    fig = plt.figure(figsize=(12, 4))
+    for i, cutout in enumerate(["Science", "Template", "Difference"]):
+        stamp = alert_dict["cutout{}".format(cutout)]["stampData"]
+        ffig = plot_stamp(stamp, fig=fig, subplot=(1, 3, i + 1))
         ffig.set_title(cutout)
 
 
-#--- Plot all
+# --- Plot all
 def plot_lightcurve_cutouts(alert_dict):
     """Adapted from:
     https://github.com/ZwickyTransientFacility/ztf-avro-alert/blob/master/notebooks/Filtering_alerts.ipynb
     """
-    fig = plt.figure(figsize=(16,4))
+
+    fig = plt.figure(figsize=(16, 4))
     dflc = pgbu.alert_dict_to_dataframe(alert_dict)
-    plot_lightcurve(dflc,ax = plt.subplot(1,4,1))
-    for i, cutout in enumerate(['Science','Template','Difference']):
-        stamp = alert_dict['cutout{}'.format(cutout)]['stampData']
-        ffig = plot_stamp(stamp, fig=fig, subplot = (1,4,i+2))
+    plot_lightcurve(dflc, ax=plt.subplot(1, 4, 1))
+    for i, cutout in enumerate(["Science", "Template", "Difference"]):
+        stamp = alert_dict["cutout{}".format(cutout)]["stampData"]
+        ffig = plot_stamp(stamp, fig=fig, subplot=(1, 4, i + 2))
         ffig.set_title(cutout)
```

### Comparing `pittgoogle-client-0.1.0/pittgoogle/pubsub.py` & `pittgoogle_client-0.1.1/pittgoogle/pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
 """The `pubsub` module facilitates access to Pitt-Google Pub/Sub streams."""
 
+import json
+import os
+from io import BytesIO
+from typing import Callable, List, Optional, Tuple, Union
+
+import pandas as pd
 from astropy.table import Table
 from fastavro import reader
 from google.cloud import pubsub_v1
 # note: the 'v1' refers to the underlying API, not the google.cloud.pubsub version
 from google.cloud.pubsub_v1.subscriber.futures import StreamingPullFuture
 from google.cloud.pubsub_v1.types import PubsubMessage, ReceivedMessage, Subscription
-from io import BytesIO
-import json
-import os
-import pandas as pd
-from typing import Callable, List, Optional, Tuple, Union
 
 from . import utils as pgbu
 
-
 pgb_project_id = "ardent-cycling-243415"
 
 
 # --- Pull messages --- #
 def pull(
     subscription_name: str,
     max_messages: int = 1,
@@ -47,14 +44,15 @@
 
         msg_only: Whether to return the message contents only or the full packet.
 
     Returns:
         A list of messages. If `msg_only` is True, the messages are bytes containing
         the message data only. Otherwise the messages are the full message packets.
     """
+
     if project_id is None:
         project_id = os.getenv("GOOGLE_CLOUD_PROJECT")
 
     # setup for pull
     subscriber = pubsub_v1.SubscriberClient()
     subscription_path = subscriber.subscription_path(project_id, subscription_name)
     request = {
@@ -89,15 +87,15 @@
     return message_list
 
 
 def streamingPull(
     subscription_name: str,
     callback: Callable[[PubsubMessage], None],
     project_id: str = None,
-    block: bool = True
+    block: bool = True,
 ) -> Union[None, StreamingPullFuture]:
     """Pull and process Pub/Sub messages continuously in streaming mode.
 
     Wrapper for the asynchronous
     `google.cloud.pubsub_v1.SubscriberClient().subscribe()`
     documented at
     https://googleapis.dev/python/pubsub/latest/subscriber/api/client.html.
@@ -121,14 +119,15 @@
         manages the background thread that is pulling and processing messages.
         Call its `cancel()` method to stop streaming messages.
 
         If `block` is True, the user's thread is blocked until the streaming encounters
         an error.
         Use Control+C to stop streaming.
     """
+
     if project_id is None:
         project_id = os.getenv("GOOGLE_CLOUD_PROJECT")
 
     subscriber = pubsub_v1.SubscriberClient()
     subscription_path = subscriber.subscription_path(project_id, subscription_name)
 
     # start receiving and processing messages in a background thread
@@ -170,14 +169,15 @@
                     If None, the environment variable GOOGLE_CLOUD_PROJECT will be used.
 
         attrs: Message attributes to be published.
 
     Returns:
         published message ID
     """
+
     if project_id is None:
         project_id = os.getenv("GOOGLE_CLOUD_PROJECT")
 
     publisher = pubsub_v1.PublisherClient()
 
     topic_path = publisher.topic_path(project_id, topic_name)
 
@@ -207,14 +207,15 @@
                     created in this account.
         subscription_name: Name for the user's Pub/Sub subscription. If None,
                            `topic_name` will be used.
 
     Returns:
         A Pub/Sub `Subscription` instance
     """
+
     if project_id is None:
         project_id = os.getenv("GOOGLE_CLOUD_PROJECT")
     if subscription_name is None:
         subscription_name = topic_name
 
     subscriber = pubsub_v1.SubscriberClient()
     publisher = pubsub_v1.PublisherClient()
@@ -247,14 +248,15 @@
     Args:
         subscription_name: Name for the user's Pub/Sub subscription. If None,
                            `topic_name` will be used.
         project_id: User's GCP project ID. If None, the environment variable
                     GOOGLE_CLOUD_PROJECT will be used. The subscription will be
                     created in this account.
     """
+
     if project_id is None:
         project_id = os.getenv("GOOGLE_CLOUD_PROJECT")
 
     subscriber = pubsub_v1.SubscriberClient()
     subscription_path = subscriber.subscription_path(project_id, subscription_name)
     request = {"subscription": subscription_path}
 
@@ -287,14 +289,15 @@
         If the message contains an alert packet only, it is returned in the requested
         format.
 
         If the message contains an alert packet plus value added products, it is
         returned as a tuple where the first element is the alert packet in the
         requested format, and the second element is the value added products as a dict.
     """
+
     # decode the message
     try:
         # decode message with avro encoding
         # may come from topic ztf-alerts or ztf-loop
         alert_dict, va_dict = _decode_avro_alert(msg_bytes)
     except ValueError:
         try:
@@ -338,17 +341,15 @@
 
     # these streams do not have value added products
     va_dict = None
 
     return alert_dict, va_dict
 
 
-def _decode_json_msg(
-    msg_bytes: bytes
-) -> Union[Tuple[dict, dict], Tuple[dict, None]]:
+def _decode_json_msg(msg_bytes: bytes) -> Union[Tuple[dict, dict], Tuple[dict, None]]:
     # decode to a dict
     dict_str = msg_bytes.decode("UTF-8")
     dic = json.loads(dict_str)
 
     # separate alert from value added
     if "alert" in dic.keys():  # value added products are included in the msg
         alert_dict = dic.pop("alert")
@@ -359,11 +360,10 @@
         va_dict = None
 
     return alert_dict, va_dict
 
 
 def _raise_decode_error():
     errmsg = (
-        "Unable to decode the message. "
-        "It does not seem to be of an expected type."
+        "Unable to decode the message. " "It does not seem to be of an expected type."
     )
     raise ValueError(errmsg)
```

### Comparing `pittgoogle-client-0.1.0/pittgoogle/utils.py` & `pittgoogle_client-0.1.1/pittgoogle/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
 """``utils`` contains functions that facilitate interacting with
 Pitt-Google Broker's data and services.
 """
 
-
-from astropy.table import Table
 from collections import OrderedDict
+
 import pandas as pd
+from astropy.table import Table
 
 
 def ztf_fid_names() -> dict:
     """Return a dictionary mapping the ZTF `fid` (filter ID) to the common name."""
+
     return {1: "g", 2: "r", 3: "i"}
 
 
 # --- Work with alert dictionaries
 def alert_dict_to_dataframe(alert_dict: dict) -> pd.DataFrame:
     """Package a ZTF alert dictionary into a dataframe.
 
@@ -31,15 +29,16 @@
     # we'll attach some metadata--note this may not be preserved after all operations
     # https://stackoverflow.com/questions/14688306/adding-meta-information-metadata-to-pandas-dataframe
     df.objectId = alert_dict["objectId"]
     return df
 
 
 def alert_dict_to_table(alert_dict: dict) -> Table:
-    """Package a ZTF alert dictionary into an Astopy Table."""
+    """Package a ZTF alert dictionary into an Astropy Table."""
+
     # collect rows for the table
     candidate = OrderedDict(alert_dict["candidate"])
     rows = [candidate]
     for prv_cand in alert_dict["prv_candidates"]:
         # astropy 3.2.1 cannot handle dicts with different keys (fixed by 4.1)
         prv_cand_tmp = {key: prv_cand.get(key, None) for key in candidate.keys()}
         rows.append(prv_cand_tmp)
@@ -54,10 +53,11 @@
     """Drop the cutouts from the alert dictionary.
 
     Args:
         alert_dict: ZTF alert formated as a dict
     Returns:
         `alert_data` with the cutouts (postage stamps) removed
     """
+
     cutouts = ["cutoutScience", "cutoutTemplate", "cutoutDifference"]
     alert_stripped = {k: v for k, v in alert_dict.items() if k not in cutouts}
     return alert_stripped
```

