# Comparing `tmp/awswrangler-3.0.0rc3.tar.gz` & `tmp/awswrangler-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awswrangler-3.0.0rc3.tar", max compression
+gzip compressed data, was "awswrangler-3.1.0.tar", max compression
```

## Comparing `awswrangler-3.0.0rc3.tar` & `awswrangler-3.1.0.tar`

### file list

```diff
@@ -1,125 +1,145 @@
--rw-r--r--   0        0        0    10142 2021-01-13 17:42:05.000000 awswrangler-3.0.0rc3/LICENSE.txt
--rw-r--r--   0        0        0       92 2022-09-07 12:05:27.255553 awswrangler-3.0.0rc3/NOTICE.txt
--rw-r--r--   0        0        0    21748 2023-03-09 12:07:46.432839 awswrangler-3.0.0rc3/README.md
--rw-r--r--   0        0        0    17494 2021-01-13 17:42:05.000000 awswrangler-3.0.0rc3/THIRD_PARTY.txt
--rw-r--r--   0        0        0     1405 2023-03-08 12:15:27.591147 awswrangler-3.0.0rc3/awswrangler/__init__.py
--rw-r--r--   0        0        0      279 2023-03-09 12:07:49.987326 awswrangler-3.0.0rc3/awswrangler/__metadata__.py
--rw-r--r--   0        0        0     3909 2023-03-08 12:15:27.591821 awswrangler-3.0.0rc3/awswrangler/_arrow.py
--rw-r--r--   0        0        0    26860 2023-03-08 12:15:27.592854 awswrangler-3.0.0rc3/awswrangler/_config.py
--rw-r--r--   0        0        0    31114 2023-03-08 12:15:27.594375 awswrangler-3.0.0rc3/awswrangler/_data_types.py
--rw-r--r--   0        0        0    12621 2023-03-08 15:59:02.540573 awswrangler-3.0.0rc3/awswrangler/_databases.py
--rw-r--r--   0        0        0     5271 2023-03-08 12:15:27.595561 awswrangler-3.0.0rc3/awswrangler/_distributed.py
--rw-r--r--   0        0        0     6211 2023-03-08 12:15:27.595743 awswrangler-3.0.0rc3/awswrangler/_sql_formatter.py
--rw-r--r--   0        0        0     1657 2023-03-08 12:15:27.595951 awswrangler-3.0.0rc3/awswrangler/_threading.py
--rw-r--r--   0        0        0    27386 2023-03-08 15:59:02.541259 awswrangler-3.0.0rc3/awswrangler/_utils.py
--rw-r--r--   0        0        0     1700 2023-02-28 14:45:26.197772 awswrangler-3.0.0rc3/awswrangler/annotations.py
--rw-r--r--   0        0        0     1038 2023-02-06 14:01:33.949479 awswrangler-3.0.0rc3/awswrangler/athena/__init__.py
--rw-r--r--   0        0        0     9301 2023-03-08 12:15:27.597366 awswrangler-3.0.0rc3/awswrangler/athena/_cache.py
--rw-r--r--   0        0        0    65007 2023-03-09 12:07:51.643380 awswrangler-3.0.0rc3/awswrangler/athena/_read.py
--rw-r--r--   0        0        0    52218 2023-03-09 12:05:44.014718 awswrangler-3.0.0rc3/awswrangler/athena/_utils.py
--rw-r--r--   0        0        0     2414 2023-02-06 14:01:33.952737 awswrangler-3.0.0rc3/awswrangler/catalog/__init__.py
--rw-r--r--   0        0        0    14077 2023-03-08 12:15:27.600887 awswrangler-3.0.0rc3/awswrangler/catalog/_add.py
--rw-r--r--   0        0        0    49119 2023-03-08 12:15:27.601768 awswrangler-3.0.0rc3/awswrangler/catalog/_create.py
--rw-r--r--   0        0        0    11466 2023-03-08 12:15:27.602150 awswrangler-3.0.0rc3/awswrangler/catalog/_definitions.py
--rw-r--r--   0        0        0     8178 2023-03-08 12:15:27.602755 awswrangler-3.0.0rc3/awswrangler/catalog/_delete.py
--rw-r--r--   0        0        0    36005 2023-03-08 15:59:02.542310 awswrangler-3.0.0rc3/awswrangler/catalog/_get.py
--rw-r--r--   0        0        0    11221 2023-03-08 15:59:02.543175 awswrangler-3.0.0rc3/awswrangler/catalog/_utils.py
--rw-r--r--   0        0        0     1199 2022-10-08 10:37:42.800465 awswrangler-3.0.0rc3/awswrangler/chime.py
--rw-r--r--   0        0        0    16587 2023-03-08 15:59:02.543878 awswrangler-3.0.0rc3/awswrangler/cloudwatch.py
--rw-r--r--   0        0        0      141 2022-10-08 10:37:42.802168 awswrangler-3.0.0rc3/awswrangler/data_api/__init__.py
--rw-r--r--   0        0        0     2829 2023-03-08 15:59:02.545717 awswrangler-3.0.0rc3/awswrangler/data_api/_connector.py
--rw-r--r--   0        0        0     5711 2023-03-08 15:59:02.546277 awswrangler-3.0.0rc3/awswrangler/data_api/rds.py
--rw-r--r--   0        0        0     9535 2023-03-08 15:59:02.548007 awswrangler-3.0.0rc3/awswrangler/data_api/redshift.py
--rw-r--r--   0        0        0      377 2023-02-06 14:01:33.956385 awswrangler-3.0.0rc3/awswrangler/data_quality/__init__.py
--rw-r--r--   0        0        0    13575 2023-03-08 15:59:02.548811 awswrangler-3.0.0rc3/awswrangler/data_quality/_create.py
--rw-r--r--   0        0        0     1392 2023-03-08 15:59:02.549405 awswrangler-3.0.0rc3/awswrangler/data_quality/_get.py
--rw-r--r--   0        0        0     6531 2023-03-08 15:59:02.549879 awswrangler-3.0.0rc3/awswrangler/data_quality/_utils.py
--rw-r--r--   0        0        0       26 2023-03-08 12:15:27.608654 awswrangler-3.0.0rc3/awswrangler/distributed/__init__.py
--rw-r--r--   0        0        0      237 2023-03-08 12:15:27.608904 awswrangler-3.0.0rc3/awswrangler/distributed/ray/__init__.py
--rw-r--r--   0        0        0     6256 2023-03-08 12:15:27.609095 awswrangler-3.0.0rc3/awswrangler/distributed/ray/_core.py
--rw-r--r--   0        0        0      931 2023-03-08 12:15:27.609264 awswrangler-3.0.0rc3/awswrangler/distributed/ray/_core.pyi
--rw-r--r--   0        0        0      691 2023-03-08 12:15:27.609747 awswrangler-3.0.0rc3/awswrangler/distributed/ray/_pool.py
--rw-r--r--   0        0        0     3794 2023-03-08 15:59:02.550452 awswrangler-3.0.0rc3/awswrangler/distributed/ray/_register.py
--rw-r--r--   0        0        0     1013 2023-03-08 12:15:27.611382 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/__init__.py
--rw-r--r--   0        0        0     2191 2023-03-08 12:15:27.611592 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
--rw-r--r--   0        0        0     1273 2023-03-08 12:15:27.611744 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
--rw-r--r--   0        0        0     3323 2023-03-08 12:15:27.612380 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
--rw-r--r--   0        0        0    18550 2023-03-08 12:15:27.613073 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
--rw-r--r--   0        0        0     5880 2023-03-08 12:15:27.614125 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
--rw-r--r--   0        0        0     5896 2023-03-08 12:15:27.614332 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
--rw-r--r--   0        0        0      135 2023-03-08 12:15:27.614858 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/__init__.py
--rw-r--r--   0        0        0     2524 2023-03-08 12:15:27.615045 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_core.py
--rw-r--r--   0        0        0      929 2023-03-08 12:15:27.615199 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_data_types.py
--rw-r--r--   0        0        0     4116 2023-03-08 15:59:02.551878 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_utils.py
--rw-r--r--   0        0        0       27 2023-03-08 12:15:27.615513 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/__init__.py
--rw-r--r--   0        0        0     1861 2023-03-08 12:15:27.616193 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_read_parquet.py
--rw-r--r--   0        0        0     5507 2023-03-08 12:15:27.617730 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_read_text.py
--rw-r--r--   0        0        0     7368 2023-03-08 12:15:27.617987 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_dataset.py
--rw-r--r--   0        0        0     3065 2023-03-08 12:15:27.618180 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_parquet.py
--rw-r--r--   0        0        0     5500 2023-03-08 12:15:27.619168 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_text.py
--rw-r--r--   0        0        0       21 2023-03-08 12:15:27.619453 awswrangler-3.0.0rc3/awswrangler/distributed/ray/s3/__init__.py
--rw-r--r--   0        0        0     2413 2023-03-08 12:15:27.620925 awswrangler-3.0.0rc3/awswrangler/distributed/ray/s3/_list.py
--rw-r--r--   0        0        0      948 2023-03-08 12:15:27.621309 awswrangler-3.0.0rc3/awswrangler/distributed/ray/s3/_read_parquet.py
--rw-r--r--   0        0        0      484 2023-01-26 20:57:05.678884 awswrangler-3.0.0rc3/awswrangler/dynamodb/__init__.py
--rw-r--r--   0        0        0     1530 2023-02-03 14:21:04.504277 awswrangler-3.0.0rc3/awswrangler/dynamodb/_delete.py
--rw-r--r--   0        0        0    24682 2023-03-08 15:59:02.552497 awswrangler-3.0.0rc3/awswrangler/dynamodb/_read.py
--rw-r--r--   0        0        0     6951 2023-03-08 12:15:27.623772 awswrangler-3.0.0rc3/awswrangler/dynamodb/_utils.py
--rw-r--r--   0        0        0     5367 2023-03-08 15:59:02.553390 awswrangler-3.0.0rc3/awswrangler/dynamodb/_write.py
--rw-r--r--   0        0        0    43346 2023-03-08 12:15:27.625778 awswrangler-3.0.0rc3/awswrangler/emr.py
--rw-r--r--   0        0        0     2610 2023-03-08 12:15:27.626512 awswrangler-3.0.0rc3/awswrangler/exceptions.py
--rw-r--r--   0        0        0      682 2023-02-06 14:01:33.970611 awswrangler-3.0.0rc3/awswrangler/lakeformation/__init__.py
--rw-r--r--   0        0        0    10914 2023-03-08 12:15:27.627707 awswrangler-3.0.0rc3/awswrangler/lakeformation/_read.py
--rw-r--r--   0        0        0    13144 2023-03-08 12:15:27.629036 awswrangler-3.0.0rc3/awswrangler/lakeformation/_utils.py
--rw-r--r--   0        0        0    20092 2023-03-08 15:59:02.554140 awswrangler-3.0.0rc3/awswrangler/mysql.py
--rw-r--r--   0        0        0      484 2023-03-08 12:15:27.630640 awswrangler-3.0.0rc3/awswrangler/neptune/__init__.py
--rw-r--r--   0        0        0     9648 2023-03-08 12:15:27.631252 awswrangler-3.0.0rc3/awswrangler/neptune/_client.py
--rw-r--r--   0        0        0      923 2023-03-08 12:15:27.631448 awswrangler-3.0.0rc3/awswrangler/neptune/_gremlin_init.py
--rw-r--r--   0        0        0     2685 2023-03-08 12:15:27.631634 awswrangler-3.0.0rc3/awswrangler/neptune/_gremlin_parser.py
--rw-r--r--   0        0        0    15665 2023-03-08 15:59:02.555007 awswrangler-3.0.0rc3/awswrangler/neptune/_neptune.py
--rw-r--r--   0        0        0     3736 2023-03-08 15:59:02.555454 awswrangler-3.0.0rc3/awswrangler/neptune/_utils.py
--rw-r--r--   0        0        0      502 2023-02-06 14:01:33.975500 awswrangler-3.0.0rc3/awswrangler/opensearch/__init__.py
--rw-r--r--   0        0        0     6470 2023-03-08 15:59:02.555999 awswrangler-3.0.0rc3/awswrangler/opensearch/_read.py
--rw-r--r--   0        0        0    13684 2023-03-08 12:15:27.633906 awswrangler-3.0.0rc3/awswrangler/opensearch/_utils.py
--rw-r--r--   0        0        0    21497 2023-03-08 15:59:02.557225 awswrangler-3.0.0rc3/awswrangler/opensearch/_write.py
--rw-r--r--   0        0        0    18538 2023-03-08 15:59:02.557830 awswrangler-3.0.0rc3/awswrangler/oracle.py
--rw-r--r--   0        0        0    18557 2023-03-08 15:59:02.558527 awswrangler-3.0.0rc3/awswrangler/postgresql.py
--rw-r--r--   0        0        0       27 2022-10-08 10:37:42.809867 awswrangler-3.0.0rc3/awswrangler/py.typed
--rw-r--r--   0        0        0     2219 2023-02-06 14:01:33.981133 awswrangler-3.0.0rc3/awswrangler/quicksight/__init__.py
--rw-r--r--   0        0        0     1906 2023-03-08 12:15:27.637078 awswrangler-3.0.0rc3/awswrangler/quicksight/_cancel.py
--rw-r--r--   0        0        0    15485 2023-03-08 12:15:27.637832 awswrangler-3.0.0rc3/awswrangler/quicksight/_create.py
--rw-r--r--   0        0        0    11710 2023-03-08 12:15:27.638684 awswrangler-3.0.0rc3/awswrangler/quicksight/_delete.py
--rw-r--r--   0        0        0     8659 2023-03-08 12:15:27.639397 awswrangler-3.0.0rc3/awswrangler/quicksight/_describe.py
--rw-r--r--   0        0        0    23655 2023-03-08 12:15:27.640237 awswrangler-3.0.0rc3/awswrangler/quicksight/_get_list.py
--rw-r--r--   0        0        0     1929 2023-03-08 12:15:27.640749 awswrangler-3.0.0rc3/awswrangler/quicksight/_utils.py
--rw-r--r--   0        0        0    71162 2023-03-09 12:05:44.015919 awswrangler-3.0.0rc3/awswrangler/redshift.py
--rw-r--r--   0        0        0     1704 2023-03-08 12:15:27.644244 awswrangler-3.0.0rc3/awswrangler/s3/__init__.py
--rw-r--r--   0        0        0    10654 2023-03-08 12:15:27.646030 awswrangler-3.0.0rc3/awswrangler/s3/_copy.py
--rw-r--r--   0        0        0     5305 2023-03-08 12:15:27.647330 awswrangler-3.0.0rc3/awswrangler/s3/_delete.py
--rw-r--r--   0        0        0     9346 2023-03-08 12:15:27.648395 awswrangler-3.0.0rc3/awswrangler/s3/_describe.py
--rw-r--r--   0        0        0     2633 2023-01-26 18:51:25.209062 awswrangler-3.0.0rc3/awswrangler/s3/_download.py
--rw-r--r--   0        0        0    23119 2023-03-08 12:15:27.649704 awswrangler-3.0.0rc3/awswrangler/s3/_fs.py
--rw-r--r--   0        0        0    15630 2023-03-08 12:15:27.650507 awswrangler-3.0.0rc3/awswrangler/s3/_list.py
--rw-r--r--   0        0        0     3970 2023-03-08 12:15:27.651659 awswrangler-3.0.0rc3/awswrangler/s3/_list.pyi
--rw-r--r--   0        0        0     5342 2023-03-08 12:15:27.651979 awswrangler-3.0.0rc3/awswrangler/s3/_read.py
--rw-r--r--   0        0        0     3345 2023-03-08 12:15:27.652310 awswrangler-3.0.0rc3/awswrangler/s3/_read_deltalake.py
--rw-r--r--   0        0        0     3265 2023-03-08 12:15:27.652733 awswrangler-3.0.0rc3/awswrangler/s3/_read_excel.py
--rw-r--r--   0        0        0    43247 2023-03-09 12:07:53.865219 awswrangler-3.0.0rc3/awswrangler/s3/_read_parquet.py
--rw-r--r--   0        0        0    33704 2023-03-09 12:07:56.102213 awswrangler-3.0.0rc3/awswrangler/s3/_read_text.py
--rw-r--r--   0        0        0     4108 2023-03-08 12:15:27.655668 awswrangler-3.0.0rc3/awswrangler/s3/_read_text_core.py
--rw-r--r--   0        0        0    11642 2023-03-08 12:15:27.656418 awswrangler-3.0.0rc3/awswrangler/s3/_select.py
--rw-r--r--   0        0        0     2465 2023-03-08 12:15:27.656776 awswrangler-3.0.0rc3/awswrangler/s3/_upload.py
--rw-r--r--   0        0        0     6584 2023-03-08 12:15:27.658242 awswrangler-3.0.0rc3/awswrangler/s3/_wait.py
--rw-r--r--   0        0        0     4298 2023-03-08 12:15:27.658568 awswrangler-3.0.0rc3/awswrangler/s3/_write.py
--rw-r--r--   0        0        0     1840 2023-03-08 12:15:27.658883 awswrangler-3.0.0rc3/awswrangler/s3/_write_concurrent.py
--rw-r--r--   0        0        0    12676 2023-03-08 12:15:27.659239 awswrangler-3.0.0rc3/awswrangler/s3/_write_dataset.py
--rw-r--r--   0        0        0     3196 2023-03-08 12:15:27.659541 awswrangler-3.0.0rc3/awswrangler/s3/_write_excel.py
--rw-r--r--   0        0        0    43164 2023-03-09 12:07:57.600534 awswrangler-3.0.0rc3/awswrangler/s3/_write_parquet.py
--rw-r--r--   0        0        0    48770 2023-03-09 12:07:58.910296 awswrangler-3.0.0rc3/awswrangler/s3/_write_text.py
--rw-r--r--   0        0        0     2018 2023-03-08 12:15:27.662297 awswrangler-3.0.0rc3/awswrangler/secretsmanager.py
--rw-r--r--   0        0        0    17879 2023-03-08 15:59:02.559864 awswrangler-3.0.0rc3/awswrangler/sqlserver.py
--rw-r--r--   0        0        0     1853 2023-03-08 12:15:27.665913 awswrangler-3.0.0rc3/awswrangler/sts.py
--rw-r--r--   0        0        0    28314 2023-03-08 15:59:02.560527 awswrangler-3.0.0rc3/awswrangler/timestream.py
--rw-r--r--   0        0        0     8209 2023-03-08 12:15:27.667551 awswrangler-3.0.0rc3/awswrangler/typing.py
--rw-r--r--   0        0        0     4454 2023-03-09 12:07:41.676456 awswrangler-3.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0    24090 1970-01-01 00:00:00.000000 awswrangler-3.0.0rc3/setup.py
--rw-r--r--   0        0        0    24270 1970-01-01 00:00:00.000000 awswrangler-3.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    10142 2022-08-02 16:44:38.861100 awswrangler-3.1.0/LICENSE.txt
+-rw-r--r--   0        0        0       92 2022-09-01 20:50:36.683640 awswrangler-3.1.0/NOTICE.txt
+-rw-r--r--   0        0        0    19946 2023-05-15 16:32:46.970048 awswrangler-3.1.0/README.md
+-rw-r--r--   0        0        0    17494 2022-08-02 16:44:38.861401 awswrangler-3.1.0/THIRD_PARTY.txt
+-rw-r--r--   0        0        0     1405 2023-04-21 16:06:31.383067 awswrangler-3.1.0/awswrangler/__init__.py
+-rw-r--r--   0        0        0      276 2023-05-15 16:32:46.971384 awswrangler-3.1.0/awswrangler/__metadata__.py
+-rw-r--r--   0        0        0     4359 2023-04-25 15:43:59.617624 awswrangler-3.1.0/awswrangler/_arrow.py
+-rw-r--r--   0        0        0    27916 2023-05-02 21:22:41.635980 awswrangler-3.1.0/awswrangler/_config.py
+-rw-r--r--   0        0        0    31116 2023-04-25 15:43:59.618486 awswrangler-3.1.0/awswrangler/_data_types.py
+-rw-r--r--   0        0        0    13202 2023-05-02 20:57:29.199914 awswrangler-3.1.0/awswrangler/_databases.py
+-rw-r--r--   0        0        0     6169 2023-04-21 16:06:31.387129 awswrangler-3.1.0/awswrangler/_distributed.py
+-rw-r--r--   0        0        0     2063 2023-04-21 16:06:31.388005 awswrangler-3.1.0/awswrangler/_executor.py
+-rw-r--r--   0        0        0     6211 2023-04-21 16:06:31.388148 awswrangler-3.1.0/awswrangler/_sql_formatter.py
+-rw-r--r--   0        0        0    28878 2023-04-25 15:43:59.619218 awswrangler-3.1.0/awswrangler/_utils.py
+-rw-r--r--   0        0        0     1701 2023-04-21 16:06:31.390428 awswrangler-3.1.0/awswrangler/annotations.py
+-rw-r--r--   0        0        0     1190 2023-05-05 17:01:05.124627 awswrangler-3.1.0/awswrangler/athena/__init__.py
+-rw-r--r--   0        0        0     9301 2023-04-21 16:06:31.390689 awswrangler-3.1.0/awswrangler/athena/_cache.py
+-rw-r--r--   0        0        0     9681 2023-05-05 17:01:05.124758 awswrangler-3.1.0/awswrangler/athena/_executions.py
+-rw-r--r--   0        0        0     2148 2023-05-05 17:01:05.124846 awswrangler-3.1.0/awswrangler/athena/_executions.pyi
+-rw-r--r--   0        0        0    54600 2023-05-15 16:32:46.972287 awswrangler-3.1.0/awswrangler/athena/_read.py
+-rw-r--r--   0        0        0    11526 2023-05-05 17:01:05.125558 awswrangler-3.1.0/awswrangler/athena/_read.pyi
+-rw-r--r--   0        0        0    41939 2023-05-05 17:01:05.126045 awswrangler-3.1.0/awswrangler/athena/_utils.py
+-rw-r--r--   0        0        0     7073 2023-05-05 17:01:05.126400 awswrangler-3.1.0/awswrangler/athena/_write_iceberg.py
+-rw-r--r--   0        0        0     2414 2023-01-17 17:33:17.175478 awswrangler-3.1.0/awswrangler/catalog/__init__.py
+-rw-r--r--   0        0        0    14077 2023-04-21 16:06:31.392981 awswrangler-3.1.0/awswrangler/catalog/_add.py
+-rw-r--r--   0        0        0    50455 2023-04-21 16:06:31.393727 awswrangler-3.1.0/awswrangler/catalog/_create.py
+-rw-r--r--   0        0        0    11466 2023-04-21 16:06:31.393962 awswrangler-3.1.0/awswrangler/catalog/_definitions.py
+-rw-r--r--   0        0        0     8236 2023-04-21 16:06:31.394534 awswrangler-3.1.0/awswrangler/catalog/_delete.py
+-rw-r--r--   0        0        0    36053 2023-04-21 16:06:31.395286 awswrangler-3.1.0/awswrangler/catalog/_get.py
+-rw-r--r--   0        0        0    11233 2023-04-21 16:06:31.395700 awswrangler-3.1.0/awswrangler/catalog/_utils.py
+-rw-r--r--   0        0        0     1199 2022-08-02 16:44:38.863657 awswrangler-3.1.0/awswrangler/chime.py
+-rw-r--r--   0        0        0    16592 2023-04-21 16:06:31.396720 awswrangler-3.1.0/awswrangler/cloudwatch.py
+-rw-r--r--   0        0        0      141 2022-08-02 16:44:38.863831 awswrangler-3.1.0/awswrangler/data_api/__init__.py
+-rw-r--r--   0        0        0     2841 2023-04-21 16:06:31.396849 awswrangler-3.1.0/awswrangler/data_api/_connector.py
+-rw-r--r--   0        0        0     5723 2023-04-21 16:06:31.397250 awswrangler-3.1.0/awswrangler/data_api/rds.py
+-rw-r--r--   0        0        0     9547 2023-04-21 16:06:31.397699 awswrangler-3.1.0/awswrangler/data_api/redshift.py
+-rw-r--r--   0        0        0      377 2023-01-17 17:33:17.179381 awswrangler-3.1.0/awswrangler/data_quality/__init__.py
+-rw-r--r--   0        0        0    13403 2023-04-21 16:06:31.398627 awswrangler-3.1.0/awswrangler/data_quality/_create.py
+-rw-r--r--   0        0        0     1404 2023-04-21 16:06:31.398990 awswrangler-3.1.0/awswrangler/data_quality/_get.py
+-rw-r--r--   0        0        0     6550 2023-04-21 16:06:31.399880 awswrangler-3.1.0/awswrangler/data_quality/_utils.py
+-rw-r--r--   0        0        0       26 2023-04-21 16:06:31.399991 awswrangler-3.1.0/awswrangler/distributed/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-21 16:06:31.400247 awswrangler-3.1.0/awswrangler/distributed/ray/__init__.py
+-rw-r--r--   0        0        0     6256 2023-04-21 16:06:31.400358 awswrangler-3.1.0/awswrangler/distributed/ray/_core.py
+-rw-r--r--   0        0        0      931 2023-04-21 16:06:31.400648 awswrangler-3.1.0/awswrangler/distributed/ray/_core.pyi
+-rw-r--r--   0        0        0     2121 2023-04-21 16:06:31.400948 awswrangler-3.1.0/awswrangler/distributed/ray/_executor.py
+-rw-r--r--   0        0        0     4239 2023-05-10 17:40:59.248347 awswrangler-3.1.0/awswrangler/distributed/ray/_register.py
+-rw-r--r--   0        0        0     2443 2023-04-21 16:06:31.401571 awswrangler-3.1.0/awswrangler/distributed/ray/_utils.py
+-rw-r--r--   0        0        0     1013 2023-04-21 16:06:31.401685 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-21 16:06:31.401968 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
+-rw-r--r--   0        0        0     1273 2023-04-21 16:06:31.402074 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
+-rw-r--r--   0        0        0     3323 2023-05-05 18:06:21.358459 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
+-rw-r--r--   0        0        0    18476 2023-05-10 17:40:59.248836 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
+-rw-r--r--   0        0        0     8991 2023-05-15 14:41:37.788540 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
+-rw-r--r--   0        0        0     5896 2023-05-01 20:36:12.635110 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
+-rw-r--r--   0        0        0      135 2023-04-21 16:06:31.402995 awswrangler-3.1.0/awswrangler/distributed/ray/modin/__init__.py
+-rw-r--r--   0        0        0     2524 2023-04-21 16:06:31.403517 awswrangler-3.1.0/awswrangler/distributed/ray/modin/_core.py
+-rw-r--r--   0        0        0      929 2023-04-21 16:06:31.403611 awswrangler-3.1.0/awswrangler/distributed/ray/modin/_data_types.py
+-rw-r--r--   0        0        0     4126 2023-04-25 15:43:59.620007 awswrangler-3.1.0/awswrangler/distributed/ray/modin/_utils.py
+-rw-r--r--   0        0        0       27 2023-04-21 16:06:31.403997 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/__init__.py
+-rw-r--r--   0        0        0     1912 2023-05-15 16:16:27.394845 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py
+-rw-r--r--   0        0        0     5507 2023-04-21 16:06:31.404564 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_read_text.py
+-rw-r--r--   0        0        0     7306 2023-04-21 16:06:31.405287 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py
+-rw-r--r--   0        0        0     3065 2023-04-21 16:06:31.405385 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py
+-rw-r--r--   0        0        0     5479 2023-05-10 17:40:59.250548 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_text.py
+-rw-r--r--   0        0        0       21 2023-04-21 16:06:31.405975 awswrangler-3.1.0/awswrangler/distributed/ray/s3/__init__.py
+-rw-r--r--   0        0        0     2413 2023-04-21 16:06:31.406055 awswrangler-3.1.0/awswrangler/distributed/ray/s3/_list.py
+-rw-r--r--   0        0        0     1005 2023-04-21 16:06:31.406314 awswrangler-3.1.0/awswrangler/distributed/ray/s3/_read_parquet.py
+-rw-r--r--   0        0        0      484 2023-05-04 22:03:58.498637 awswrangler-3.1.0/awswrangler/dynamodb/__init__.py
+-rw-r--r--   0        0        0     1545 2023-04-21 16:06:31.406985 awswrangler-3.1.0/awswrangler/dynamodb/_delete.py
+-rw-r--r--   0        0        0    24958 2023-05-05 17:01:05.126808 awswrangler-3.1.0/awswrangler/dynamodb/_read.py
+-rw-r--r--   0        0        0     9045 2023-05-05 17:01:05.126904 awswrangler-3.1.0/awswrangler/dynamodb/_read.pyi
+-rw-r--r--   0        0        0     6978 2023-05-05 17:01:05.127213 awswrangler-3.1.0/awswrangler/dynamodb/_utils.py
+-rw-r--r--   0        0        0     8406 2023-04-21 16:06:31.408377 awswrangler-3.1.0/awswrangler/dynamodb/_write.py
+-rw-r--r--   0        0        0    44390 2023-05-05 17:01:05.127643 awswrangler-3.1.0/awswrangler/emr.py
+-rw-r--r--   0        0        0     2756 2023-05-02 21:22:41.637450 awswrangler-3.1.0/awswrangler/exceptions.py
+-rw-r--r--   0        0        0      682 2023-04-13 20:06:09.276287 awswrangler-3.1.0/awswrangler/lakeformation/__init__.py
+-rw-r--r--   0        0        0    10941 2023-04-21 16:06:31.410840 awswrangler-3.1.0/awswrangler/lakeformation/_read.py
+-rw-r--r--   0        0        0    13151 2023-04-21 16:06:31.411661 awswrangler-3.1.0/awswrangler/lakeformation/_utils.py
+-rw-r--r--   0        0        0    20293 2023-05-10 17:43:52.854565 awswrangler-3.1.0/awswrangler/mysql.py
+-rw-r--r--   0        0        0      570 2023-05-02 21:22:41.638164 awswrangler-3.1.0/awswrangler/neptune/__init__.py
+-rw-r--r--   0        0        0    12730 2023-05-10 17:40:54.870838 awswrangler-3.1.0/awswrangler/neptune/_client.py
+-rw-r--r--   0        0        0      923 2023-04-21 16:06:31.412767 awswrangler-3.1.0/awswrangler/neptune/_gremlin_init.py
+-rw-r--r--   0        0        0     2685 2023-05-10 17:40:54.871069 awswrangler-3.1.0/awswrangler/neptune/_gremlin_parser.py
+-rw-r--r--   0        0        0    22208 2023-05-10 17:40:54.871423 awswrangler-3.1.0/awswrangler/neptune/_neptune.py
+-rw-r--r--   0        0        0     3748 2023-04-21 16:06:31.413536 awswrangler-3.1.0/awswrangler/neptune/_utils.py
+-rw-r--r--   0        0        0      502 2023-01-30 20:05:15.832378 awswrangler-3.1.0/awswrangler/opensearch/__init__.py
+-rw-r--r--   0        0        0     6480 2023-05-10 17:40:54.871644 awswrangler-3.1.0/awswrangler/opensearch/_read.py
+-rw-r--r--   0        0        0    13764 2023-05-10 17:40:54.872112 awswrangler-3.1.0/awswrangler/opensearch/_utils.py
+-rw-r--r--   0        0        0    21509 2023-05-10 17:40:54.872409 awswrangler-3.1.0/awswrangler/opensearch/_write.py
+-rw-r--r--   0        0        0    20931 2023-05-10 17:43:52.855383 awswrangler-3.1.0/awswrangler/oracle.py
+-rw-r--r--   0        0        0     1595 2023-04-25 15:43:59.622719 awswrangler-3.1.0/awswrangler/pandas/__init__.py
+-rw-r--r--   0        0        0    20629 2023-05-10 17:43:52.856222 awswrangler-3.1.0/awswrangler/postgresql.py
+-rw-r--r--   0        0        0       27 2022-08-02 16:44:38.866284 awswrangler-3.1.0/awswrangler/py.typed
+-rw-r--r--   0        0        0     2219 2023-01-17 17:33:17.208660 awswrangler-3.1.0/awswrangler/quicksight/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-21 16:06:31.416913 awswrangler-3.1.0/awswrangler/quicksight/_cancel.py
+-rw-r--r--   0        0        0    15508 2023-05-15 16:16:15.071628 awswrangler-3.1.0/awswrangler/quicksight/_create.py
+-rw-r--r--   0        0        0    11710 2023-04-21 16:06:31.417954 awswrangler-3.1.0/awswrangler/quicksight/_delete.py
+-rw-r--r--   0        0        0     8660 2023-04-21 16:06:31.418387 awswrangler-3.1.0/awswrangler/quicksight/_describe.py
+-rw-r--r--   0        0        0    23657 2023-05-15 14:19:50.276077 awswrangler-3.1.0/awswrangler/quicksight/_get_list.py
+-rw-r--r--   0        0        0     1929 2023-05-15 15:20:02.815523 awswrangler-3.1.0/awswrangler/quicksight/_utils.py
+-rw-r--r--   0        0        0      440 2023-05-10 17:40:59.251591 awswrangler-3.1.0/awswrangler/redshift/__init__.py
+-rw-r--r--   0        0        0     8809 2023-05-10 17:40:59.251715 awswrangler-3.1.0/awswrangler/redshift/_connect.py
+-rw-r--r--   0        0        0    18905 2023-05-10 17:40:59.251876 awswrangler-3.1.0/awswrangler/redshift/_read.py
+-rw-r--r--   0        0        0     6086 2023-05-10 17:40:59.251990 awswrangler-3.1.0/awswrangler/redshift/_read.pyi
+-rw-r--r--   0        0        0    15681 2023-05-10 17:40:59.252145 awswrangler-3.1.0/awswrangler/redshift/_utils.py
+-rw-r--r--   0        0        0    28318 2023-05-10 17:40:59.252324 awswrangler-3.1.0/awswrangler/redshift/_write.py
+-rw-r--r--   0        0        0     1789 2023-05-02 21:22:41.642687 awswrangler-3.1.0/awswrangler/s3/__init__.py
+-rw-r--r--   0        0        0    10594 2023-04-21 16:06:31.421145 awswrangler-3.1.0/awswrangler/s3/_copy.py
+-rw-r--r--   0        0        0     5289 2023-04-21 16:06:31.421784 awswrangler-3.1.0/awswrangler/s3/_delete.py
+-rw-r--r--   0        0        0     9327 2023-04-21 16:06:31.422180 awswrangler-3.1.0/awswrangler/s3/_describe.py
+-rw-r--r--   0        0        0     2633 2023-01-30 20:05:15.841405 awswrangler-3.1.0/awswrangler/s3/_download.py
+-rw-r--r--   0        0        0    23146 2023-04-21 16:06:31.422841 awswrangler-3.1.0/awswrangler/s3/_fs.py
+-rw-r--r--   0        0        0    15683 2023-04-21 16:06:31.423159 awswrangler-3.1.0/awswrangler/s3/_list.py
+-rw-r--r--   0        0        0     3970 2023-04-21 16:06:31.423979 awswrangler-3.1.0/awswrangler/s3/_list.pyi
+-rw-r--r--   0        0        0     5342 2023-04-21 16:06:31.424139 awswrangler-3.1.0/awswrangler/s3/_read.py
+-rw-r--r--   0        0        0     3471 2023-05-02 21:22:41.643295 awswrangler-3.1.0/awswrangler/s3/_read_deltalake.py
+-rw-r--r--   0        0        0     3277 2023-05-10 17:40:54.875396 awswrangler-3.1.0/awswrangler/s3/_read_excel.py
+-rw-r--r--   0        0        0    36296 2023-05-15 16:32:46.973134 awswrangler-3.1.0/awswrangler/s3/_read_parquet.py
+-rw-r--r--   0        0        0     9380 2023-05-05 17:01:05.128332 awswrangler-3.1.0/awswrangler/s3/_read_parquet.pyi
+-rw-r--r--   0        0        0    26728 2023-05-15 16:32:46.973775 awswrangler-3.1.0/awswrangler/s3/_read_text.py
+-rw-r--r--   0        0        0     7577 2023-05-05 17:01:05.129193 awswrangler-3.1.0/awswrangler/s3/_read_text.pyi
+-rw-r--r--   0        0        0     4108 2023-04-21 16:06:31.426375 awswrangler-3.1.0/awswrangler/s3/_read_text_core.py
+-rw-r--r--   0        0        0    11991 2023-05-02 21:22:41.644182 awswrangler-3.1.0/awswrangler/s3/_select.py
+-rw-r--r--   0        0        0     2465 2023-04-21 16:06:31.426801 awswrangler-3.1.0/awswrangler/s3/_upload.py
+-rw-r--r--   0        0        0     6205 2023-04-21 16:06:31.427634 awswrangler-3.1.0/awswrangler/s3/_wait.py
+-rw-r--r--   0        0        0     4715 2023-04-21 16:06:31.428073 awswrangler-3.1.0/awswrangler/s3/_write.py
+-rw-r--r--   0        0        0     1840 2023-04-21 16:06:31.428436 awswrangler-3.1.0/awswrangler/s3/_write_concurrent.py
+-rw-r--r--   0        0        0    12694 2023-04-21 16:06:31.428881 awswrangler-3.1.0/awswrangler/s3/_write_dataset.py
+-rw-r--r--   0        0        0     4087 2023-05-02 21:22:41.644400 awswrangler-3.1.0/awswrangler/s3/_write_deltalake.py
+-rw-r--r--   0        0        0     3196 2023-05-10 17:40:54.875751 awswrangler-3.1.0/awswrangler/s3/_write_excel.py
+-rw-r--r--   0        0        0    43262 2023-05-15 16:32:46.974626 awswrangler-3.1.0/awswrangler/s3/_write_parquet.py
+-rw-r--r--   0        0        0    48588 2023-05-15 16:32:46.975422 awswrangler-3.1.0/awswrangler/s3/_write_text.py
+-rw-r--r--   0        0        0     2018 2023-04-21 16:06:31.431108 awswrangler-3.1.0/awswrangler/secretsmanager.py
+-rw-r--r--   0        0        0    17975 2023-05-10 17:43:52.856811 awswrangler-3.1.0/awswrangler/sqlserver.py
+-rw-r--r--   0        0        0     1853 2023-04-21 16:06:31.432014 awswrangler-3.1.0/awswrangler/sts.py
+-rw-r--r--   0        0        0      644 2023-05-10 17:40:59.253502 awswrangler-3.1.0/awswrangler/timestream/__init__.py
+-rw-r--r--   0        0        0     4512 2023-05-10 17:40:59.255448 awswrangler-3.1.0/awswrangler/timestream/_create.py
+-rw-r--r--   0        0        0     2491 2023-05-10 17:40:59.255770 awswrangler-3.1.0/awswrangler/timestream/_delete.py
+-rw-r--r--   0        0        0     2603 2023-05-15 14:41:20.785245 awswrangler-3.1.0/awswrangler/timestream/_list.py
+-rw-r--r--   0        0        0     5881 2023-05-10 17:40:59.256502 awswrangler-3.1.0/awswrangler/timestream/_read.py
+-rw-r--r--   0        0        0      722 2023-05-10 17:40:59.256775 awswrangler-3.1.0/awswrangler/timestream/_read.pyi
+-rw-r--r--   0        0        0    26397 2023-05-10 17:40:59.257401 awswrangler-3.1.0/awswrangler/timestream/_write.py
+-rw-r--r--   0        0        0     8983 2023-05-02 21:22:41.646552 awswrangler-3.1.0/awswrangler/typing.py
+-rw-r--r--   0        0        0     4786 2023-05-15 16:32:46.977245 awswrangler-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    22545 1970-01-01 00:00:00.000000 awswrangler-3.1.0/PKG-INFO
```

### Comparing `awswrangler-3.0.0rc3/LICENSE.txt` & `awswrangler-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/README.md` & `awswrangler-3.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/release-3.0.0rc3-brightgreen.svg)](https://pypi.org/project/awswrangler/)
-[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
+[![Release](https://img.shields.io/badge/3.1.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![Coverage](https://img.shields.io/badge/coverage-91%25-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
 
 | Source | Downloads | Installation Command |
 |--------|-----------|----------------------|
 | **[PyPi](https://pypi.org/project/awswrangler/)**  | [![PyPI Downloads](https://pepy.tech/badge/awswrangler)](https://pypi.org/project/awswrangler/) | `pip install awswrangler` |
 | **[Conda](https://anaconda.org/conda-forge/awswrangler)** | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/awswrangler.svg)](https://anaconda.org/conda-forge/awswrangler) | `conda install -c conda-forge awswrangler` |
@@ -35,15 +34,15 @@
 
 - [Quick Start](#quick-start)
 - [At Scale](#at-scale)
 - [Read The Docs](#read-the-docs)
 - [Getting Help](#getting-help)
 - [Community Resources](#community-resources)
 - [Logging](#logging)
-- [Who uses AWS SDK for pandas?](#who-uses-aws-sdk-pandas)
+- [Who uses AWS SDK for pandas?](#who-uses-aws-sdk-for-pandas)
 
 ## Quick Start
 
 Installation command: `pip install awswrangler`
 
 > ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>
 ➡️`pip install 'awswrangler[redshift]'`
@@ -96,73 +95,33 @@
 """)
 
 ```
 
 ## At scale
 AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
 
-The quickest way to get started is to use AWS Glue with Ray. Read our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/) to learn about it, then head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/release-3.0.0/tutorials) to discover even more features.
-
-### Installation
-```
-pip install "awswrangler[modin,ray]==3.0.0rc3"
-```
-
-As a result existing scripts can run on significantly larger datasets with no code rewrite. Supported APIs are parallelized across cores on a single machine or across multiple nodes on a cluster in the cloud.
-
-### Supported APIs
-
-<p align="center">
-
-| Service         | API                      | Implementation |
-|-----------------|--------------------------|:--------------:|
-| `S3`            | `read_parquet`           |       ✅        |
-|                 | `read_parquet_metadata`  |       ✅        |
-|                 | `read_parquet_table`     |       ✅        |
-|                 | `read_csv`               |       ✅        |
-|                 | `read_json`              |       ✅        |
-|                 | `read_fwf`               |       ✅        |
-|                 | `to_parquet`             |       ✅        |
-|                 | `to_csv`                 |       ✅        |
-|                 | `to_json`                |       ✅        |
-|                 | `select_query`           |       ✅        |
-|                 | `store_parquet_metadata` |       ✅        |
-|                 | `delete_objects`         |       ✅        |
-|                 | `describe_objects`       |       ✅        |
-|                 | `size_objects`           |       ✅        |
-|                 | `wait_objects_exist`     |       ✅        |
-|                 | `wait_objects_not_exist` |       ✅        |
-|                 | `merge_datasets`         |       ✅        |
-|                 | `copy_objects`           |       ✅        |
-| `Redshift`      | `copy`                   |       ✅        |
-|                 | `unload`                 |       ✅        |
-| `Athena`        | `read_sql_query`         |       ✅        |
-|                 | `read_sql_table`         |       ✅        |
-|                 | `describe_table`         |       ✅        |
-|                 | `get_query_results`      |       ✅        |
-|                 | `show_create_table`      |       ✅        |
-| `DynamoDB`      | `read_items`             |       ✅        |
-| `LakeFormation` | `read_sql_query`         |       ✅        |
-|                 | `read_sql_table`         |       ✅        |
-| `Timestream`    | `write`                  |       ✅        |
-</p>
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/what.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#from-source)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#resources)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -189,52 +148,56 @@
   - [027 - Amazon Timestream 2](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/027%20-%20Amazon%20Timestream%202.ipynb)
   - [028 - Amazon DynamoDB](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/028%20-%20DynamoDB.ipynb)
   - [029 - S3 Select](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/029%20-%20S3%20Select.ipynb)
   - [030 - Data Api](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/030%20-%20Data%20Api.ipynb)
   - [031 - OpenSearch](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/031%20-%20OpenSearch.ipynb)
   - [032 - Lake Formation Governed Tables](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/032%20-%20Lake%20Formation%20Governed%20Tables.ipynb)
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
-  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
-  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
-  - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
+  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
+  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
+  - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
   - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
   - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#opensearch)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#global-configurations)
+  - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#distributed-ray)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
 * The #aws-sdk-pandas Slack [channel](https://join.slack.com/t/aws-sdk-pandas/shared_invite/zt-sxdx38sl-E0coRfAds8WdpxXD2Nzfrg)
 * Ask a question on [Stack Overflow](https://stackoverflow.com/questions/tagged/awswrangler)
   and tag it with `awswrangler`
+* [Runbook](https://github.com/aws/aws-sdk-pandas/discussions/1815) for AWS SDK for pandas with Ray
 
 ## Community Resources
 
 Please [send a Pull Request](https://github.com/aws/aws-sdk-pandas/edit/main/README.md) with your resource reference and @githubhandle.
 
 - [Optimize Python ETL by extending Pandas with AWS SDK for pandas](https://aws.amazon.com/blogs/big-data/optimize-python-etl-by-extending-pandas-with-aws-data-wrangler/) [[@igorborgest](https://github.com/igorborgest)]
 - [Reading Parquet Files With AWS Lambda](https://aprakash.wordpress.com/2020/04/14/reading-parquet-files-with-aws-lambda/) [[@anand086](https://github.com/anand086)]
```

### Comparing `awswrangler-3.0.0rc3/THIRD_PARTY.txt` & `awswrangler-3.1.0/THIRD_PARTY.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/__init__.py` & `awswrangler-3.1.0/awswrangler/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/_arrow.py` & `awswrangler-3.1.0/awswrangler/_arrow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Arrow Utilities Module (PRIVATE)."""
 
 import datetime
 import json
 import logging
 from typing import Any, Dict, Optional, Tuple, cast
 
-import pandas as pd
 import pyarrow as pa
 
+import awswrangler.pandas as pd
 from awswrangler._data_types import athena2pyarrow
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _extract_partitions_from_path(path_root: str, path: str) -> Dict[str, str]:
     path_root = path_root if path_root.endswith("/") else f"{path_root}/"
@@ -43,14 +43,25 @@
                     table.schema.get_field_index(col),
                     col,
                     part_value,
                 )
     return table
 
 
+def ensure_df_is_mutable(df: pd.DataFrame) -> pd.DataFrame:
+    """Ensure that all columns has the writeable flag True."""
+    for column in df.columns.to_list():
+        if hasattr(df[column].values, "flags") is True:
+            if df[column].values.flags.writeable is False:
+                s: pd.Series = df[column]
+                df[column] = None
+                df[column] = s
+    return df
+
+
 def _apply_timezone(df: pd.DataFrame, metadata: Dict[str, Any]) -> pd.DataFrame:
     for c in metadata["columns"]:
         if "field_name" in c and c["field_name"] is not None:
             col_name = str(c["field_name"])
         elif "name" in c and c["name"] is not None:
             col_name = str(c["name"])
         else:
@@ -74,14 +85,15 @@
     """
     metadata: Dict[str, Any] = {}
     if table.schema.metadata is not None and b"pandas" in table.schema.metadata:
         metadata = json.loads(table.schema.metadata[b"pandas"])
 
     df = table.to_pandas(**kwargs)
 
+    df = ensure_df_is_mutable(df=df)
     if metadata:
         _logger.debug("metadata: %s", metadata)
         df = _apply_timezone(df=df, metadata=metadata)
     return df
 
 
 def _df_to_table(
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/_config.py` & `awswrangler-3.1.0/awswrangler/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Configuration file for AWS SDK for pandas."""
 
 import inspect
 import logging
 import os
+from functools import wraps
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Type, TypeVar, Union, cast
 
 import botocore.config
 import pandas as pd
 
 from awswrangler import exceptions
 from awswrangler.typing import AthenaCacheSettings
@@ -37,14 +38,16 @@
     "max_cache_query_inspections": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
     "max_cache_seconds": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
     "max_remote_cache_entries": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
     "max_local_cache_entries": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
     "athena_query_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
     "cloudwatch_query_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
     "lakeformation_query_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
+    "neptune_load_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
+    "timestream_batch_load_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
     "s3_block_size": _ConfigArg(dtype=int, nullable=False, enforced=True),
     "workgroup": _ConfigArg(dtype=str, nullable=False, enforced=True),
     "chunksize": _ConfigArg(dtype=int, nullable=False, enforced=True),
     "suppress_warnings": _ConfigArg(dtype=bool, nullable=False, default=False, loaded=True),
     # Endpoints URLs
     "s3_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "athena_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
@@ -351,14 +354,32 @@
         return cast(float, self["lakeformation_query_wait_polling_delay"])
 
     @lakeformation_query_wait_polling_delay.setter
     def lakeformation_query_wait_polling_delay(self, value: float) -> None:
         self._set_config_value(key="lakeformation_query_wait_polling_delay", value=value)
 
     @property
+    def neptune_load_wait_polling_delay(self) -> float:
+        """Property neptune_load_wait_polling_delay."""
+        return cast(float, self["neptune_load_wait_polling_delay"])
+
+    @neptune_load_wait_polling_delay.setter
+    def neptune_load_wait_polling_delay(self, value: float) -> None:
+        self._set_config_value(key="neptune_load_wait_polling_delay", value=value)
+
+    @property
+    def timestream_batch_load_wait_polling_delay(self) -> float:
+        """Property timestream_batch_load_wait_polling_delay."""
+        return cast(float, self["timestream_batch_load_wait_polling_delay"])
+
+    @timestream_batch_load_wait_polling_delay.setter
+    def timestream_batch_load_wait_polling_delay(self, value: float) -> None:
+        self._set_config_value(key="timestream_batch_load_wait_polling_delay", value=value)
+
+    @property
     def s3_block_size(self) -> int:
         """Property s3_block_size."""
         return cast(int, self["s3_block_size"])
 
     @s3_block_size.setter
     def s3_block_size(self, value: int) -> None:
         self._set_config_value(key="s3_block_size", value=value)
@@ -669,14 +690,15 @@
 
 def apply_configs(function: FunctionType) -> FunctionType:
     """Decorate some function with configs."""
     signature = inspect.signature(function)
     args_names: Tuple[str, ...] = tuple(signature.parameters.keys())
     available_configs: Tuple[str, ...] = tuple(x for x in _CONFIG_ARGS if x in args_names)
 
+    @wraps(function)
     def wrapper(*args_raw: Any, **kwargs: Any) -> Any:
         args: Dict[str, Any] = signature.bind_partial(*args_raw, **kwargs).arguments
         for name in available_configs:
             if hasattr(config, name) is True:
                 value = config[name]
                 _assign_args_value(args, name, value)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/_data_types.py` & `awswrangler-3.1.0/awswrangler/_data_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any, Callable, Dict, Iterator, List, Match, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet
 
-from awswrangler import _utils, exceptions
+from awswrangler import _arrow, exceptions
 from awswrangler._distributed import engine
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def pyarrow2athena(  # pylint: disable=too-many-branches,too-many-return-statements
     dtype: pa.DataType, ignore_null: bool = False
@@ -168,15 +168,15 @@
     if pa.types.is_date(dtype):
         return "DATE"
     if pa.types.is_decimal(dtype):
         return f"NUMBER({dtype.precision},{dtype.scale})"
     if pa.types.is_dictionary(dtype):
         return pyarrow2oracle(dtype=dtype.value_type, string_type=string_type)
     if pa.types.is_binary(dtype):
-        return "RAW"
+        return "BLOB"
     raise exceptions.UnsupportedType(f"Unsupported Oracle type: {dtype}")
 
 
 def pyarrow2postgresql(  # pylint: disable=too-many-branches,too-many-return-statements
     dtype: pa.DataType, string_type: str
 ) -> str:
     """Pyarrow to PostgreSQL data types conversion."""
@@ -239,15 +239,15 @@
         return "DATE"
     if pa.types.is_decimal(dtype):
         return f"DECIMAL({dtype.precision},{dtype.scale})"
     if pa.types.is_dictionary(dtype):
         return pyarrow2sqlserver(dtype=dtype.value_type, string_type=string_type)
     if pa.types.is_binary(dtype):
         return "VARBINARY"
-    raise exceptions.UnsupportedType(f"Unsupported PostgreSQL type: {dtype}")
+    raise exceptions.UnsupportedType(f"Unsupported SQL Server type: {dtype}")
 
 
 def pyarrow2timestream(dtype: pa.DataType) -> str:  # pylint: disable=too-many-branches,too-many-return-statements
     """Pyarrow to Amazon Timestream data types conversion."""
     if pa.types.is_int8(dtype):
         return "BIGINT"
     if pa.types.is_int16(dtype) or pa.types.is_uint8(dtype):
@@ -552,15 +552,15 @@
 
 def pyarrow2pandas_defaults(use_threads: Union[bool, int], kwargs: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
     """Return Pyarrow to Pandas default dictionary arguments."""
     default_kwargs = {
         "use_threads": use_threads,
         "split_blocks": True,
         "self_destruct": True,
-        "ignore_metadata": True,
+        "ignore_metadata": False,
         "types_mapper": pyarrow2pandas_extension,
     }
     if kwargs:
         default_kwargs.update(kwargs)
     return default_kwargs
 
 
@@ -696,15 +696,15 @@
             and (athena_type.startswith("map") is False)
         ):
             desired_type: str = athena2pandas(dtype=athena_type)
             current_type: str = _normalize_pandas_dtype_name(dtype=str(df[col].dtypes))
             if desired_type != current_type:  # Needs conversion
                 _logger.debug("current_type: %s -> desired_type: %s", current_type, desired_type)
                 if mutability_ensured is False:
-                    df = _utils.ensure_df_is_mutable(df=df)
+                    df = _arrow.ensure_df_is_mutable(df=df)
                     mutability_ensured = True
                 _cast_pandas_column(df=df, col=col, current_type=current_type, desired_type=desired_type)
     return df
 
 
 def _normalize_pandas_dtype_name(dtype: str) -> str:
     if dtype.startswith("datetime64") is True:
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/_databases.py` & `awswrangler-3.1.0/awswrangler/_databases.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import importlib.util
 import logging
 import ssl
 from typing import Any, Dict, Generator, Iterator, List, NamedTuple, Optional, Tuple, Union, cast, overload
 
 import boto3
-import pandas as pd
 import pyarrow as pa
 
+import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions, oracle, secretsmanager
 from awswrangler.catalog import get_connection
 
 _oracledb_found = importlib.util.find_spec("oracledb")
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
@@ -57,18 +57,28 @@
                 ssl_cadata = client_s3.get_object(Bucket=bucket_name, Key=key_path)["Body"].read().decode("utf-8")
             except client_s3.exceptions.NoSuchKey:
                 raise exceptions.NoFilesFound(  # pylint: disable=raise-missing-from
                     f"No CA certificate found at {ssl_cert_path}."
                 )
         ssl_context = ssl.create_default_context(cadata=ssl_cadata)
 
+    if "SECRET_ID" in details:
+        secret_value: Dict[str, Any] = secretsmanager.get_secret_json(
+            name=details["SECRET_ID"], boto3_session=boto3_session
+        )
+        username = secret_value["username"]
+        password = secret_value["password"]
+    else:
+        username = details["USERNAME"]
+        password = details["PASSWORD"]
+
     return ConnectionAttributes(
         kind=details["JDBC_CONNECTION_URL"].split(":")[1].lower(),
-        user=details["USERNAME"],
-        password=details["PASSWORD"],
+        user=username,
+        password=password,
         host=details["JDBC_CONNECTION_URL"].split(":")[-2].replace("/", "").replace("@", ""),
         port=int(port),
         database=dbname if dbname is not None else database,
         ssl_context=ssl_context,
     )
 
 
@@ -122,14 +132,24 @@
     if params is not None:
         if hasattr(params, "keys"):
             return args + [params]
         return args + [list(params)]
     return args
 
 
+def _should_handle_oracle_objects(dtype: pa.DataType) -> bool:
+    return (
+        dtype == pa.string()
+        or dtype == pa.large_string()
+        or isinstance(dtype, pa.Decimal128Type)
+        or dtype == pa.binary()
+        or dtype == pa.large_binary()
+    )
+
+
 def _records2df(
     records: List[Tuple[Any]],
     cols_names: List[str],
     index: Optional[Union[str, List[str]]],
     safe: bool,
     dtype: Optional[Dict[str, pa.DataType]],
     timestamp_as_object: bool,
@@ -142,15 +162,15 @@
             try:
                 array: pa.Array = pa.array(obj=col_values, safe=safe)  # Creating Arrow array
             except pa.ArrowInvalid as ex:
                 array = _data_types.process_not_inferred_array(ex, values=col_values)  # Creating Arrow array
         else:
             try:
                 if _oracledb_found:
-                    if dtype[col_name] == pa.string() or isinstance(dtype[col_name], pa.Decimal128Type):
+                    if _should_handle_oracle_objects(dtype[col_name]):
                         col_values = oracle.handle_oracle_objects(col_values, col_name, dtype)
                 array = pa.array(obj=col_values, type=dtype[col_name], safe=safe)  # Creating Arrow array with dtype
             except (pa.ArrowInvalid, pa.ArrowTypeError):
                 array = pa.array(obj=col_values, safe=safe)  # Creating Arrow array
                 array = array.cast(target_type=dtype[col_name], safe=safe)  # Casting
         arrays.append(array)
     if not arrays:
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/_sql_formatter.py` & `awswrangler-3.1.0/awswrangler/_sql_formatter.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/_threading.py` & `awswrangler-3.1.0/awswrangler/_executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,60 @@
-"""Threading Module (PRIVATE)."""
+"""Executor Module (PRIVATE)."""
 
 import concurrent.futures
 import itertools
 import logging
+from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Callable, List, Optional, TypeVar, Union
 
 from awswrangler import _utils
-from awswrangler._distributed import EngineEnum, engine
+from awswrangler._distributed import engine
 
 if TYPE_CHECKING:
     from botocore.client import BaseClient
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 MapOutputType = TypeVar("MapOutputType")
 
 
-class _ThreadPoolExecutor:
+class _BaseExecutor(ABC):
+    def __init__(self) -> None:
+        _logger.debug("Creating an %s executor: ", self.__class__)
+
+    @abstractmethod
+    def map(
+        self,
+        func: Callable[..., MapOutputType],
+        boto3_client: Optional["BaseClient"],
+        *args: Any,
+    ) -> List[MapOutputType]:
+        pass
+
+
+class _ThreadPoolExecutor(_BaseExecutor):
     def __init__(self, use_threads: Union[bool, int]):
         super().__init__()
         self._exec: Optional[concurrent.futures.ThreadPoolExecutor] = None
         self._cpus: int = _utils.ensure_cpu_count(use_threads=use_threads)
         if self._cpus > 1:
+            _logger.debug("Initializing ThreadPoolExecutor with %d workers", self._cpus)
             self._exec = concurrent.futures.ThreadPoolExecutor(max_workers=self._cpus)  # pylint: disable=R1732
 
     def map(
-        self, func: Callable[..., MapOutputType], boto3_client: Optional["BaseClient"], *iterables: Any
+        self, func: Callable[..., MapOutputType], boto3_client: Optional["BaseClient"], *args: Any
     ) -> List[MapOutputType]:
         """Map iterables to multi-threaded function."""
         _logger.debug("Map: %s", func)
         if self._exec is not None:
-            args = (itertools.repeat(boto3_client), *iterables)
-            return list(self._exec.map(func, *args))
+            iterables = (itertools.repeat(boto3_client), *args)
+            return list(self._exec.map(func, *iterables))
         # Single-threaded
-        return list(map(func, *(itertools.repeat(boto3_client), *iterables)))
-
+        return list(map(func, *(itertools.repeat(boto3_client), *args)))
 
-def _get_executor(use_threads: Union[bool, int]) -> _ThreadPoolExecutor:
-    if engine.get() == EngineEnum.RAY:
-        from awswrangler.distributed.ray._pool import _RayPoolExecutor  # pylint: disable=import-outside-toplevel
 
-        return _RayPoolExecutor()  # type: ignore[return-value]
+@engine.dispatch_on_engine
+def _get_executor(use_threads: Union[bool, int], **kwargs: Any) -> _BaseExecutor:
+    # kwargs allows for parameter that will be used by other variants of this function,
+    # such as `parallelism` for _get_ray_executor
     return _ThreadPoolExecutor(use_threads)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/_utils.py` & `awswrangler-3.1.0/awswrangler/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Internal (private) Utilities Module."""
 
 import importlib
+import inspect
 import itertools
 import logging
 import math
 import os
 import random
 import time
 from concurrent.futures import FIRST_COMPLETED, Future, wait
@@ -26,48 +27,70 @@
     cast,
     overload,
 )
 
 import boto3
 import botocore.credentials
 import numpy as np
-import pandas as pd
 import pyarrow as pa
 from botocore.config import Config
 
+import awswrangler.pandas as pd
 from awswrangler import _config, exceptions
 from awswrangler.__metadata__ import __version__
 from awswrangler._arrow import _table_to_df
 from awswrangler._config import _insert_str, apply_configs
 from awswrangler._distributed import EngineEnum, engine
 
 if TYPE_CHECKING:
     from boto3.resources.base import ServiceResource
     from botocore.client import BaseClient
     from mypy_boto3_athena import AthenaClient
-    from mypy_boto3_athena.literals import ServiceName
     from mypy_boto3_dynamodb import DynamoDBClient, DynamoDBServiceResource
     from mypy_boto3_ec2 import EC2Client
     from mypy_boto3_emr.client import EMRClient
     from mypy_boto3_glue import GlueClient
     from mypy_boto3_kms.client import KMSClient
     from mypy_boto3_lakeformation.client import LakeFormationClient
     from mypy_boto3_logs.client import CloudWatchLogsClient
     from mypy_boto3_opensearch.client import OpenSearchServiceClient
     from mypy_boto3_opensearchserverless.client import OpenSearchServiceServerlessClient
     from mypy_boto3_quicksight.client import QuickSightClient
+    from mypy_boto3_rds_data.client import RDSDataServiceClient
     from mypy_boto3_redshift.client import RedshiftClient
     from mypy_boto3_redshift_data.client import RedshiftDataAPIServiceClient
     from mypy_boto3_s3 import S3Client, S3ServiceResource
     from mypy_boto3_secretsmanager import SecretsManagerClient
     from mypy_boto3_sts.client import STSClient
     from mypy_boto3_timestream_query.client import TimestreamQueryClient
     from mypy_boto3_timestream_write.client import TimestreamWriteClient
     from typing_extensions import Literal
 
+    ServiceName = Literal[
+        "athena",
+        "dynamodb",
+        "ec2",
+        "emr",
+        "glue",
+        "kms",
+        "lakeformation",
+        "logs",
+        "opensearch",
+        "opensearchserverless",
+        "quicksight",
+        "rds-data",
+        "redshift-data",
+        "redshift",
+        "s3",
+        "secretsmanager",
+        "sts",
+        "timestream-query",
+        "timestream-write",
+    ]
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 Boto3PrimitivesType = Dict[str, Optional[str]]
 FunctionType = TypeVar("FunctionType", bound=Callable[..., Any])
 
 # A mapping from import name to package name (on PyPI) for packages where
 # these two names are different.
@@ -126,14 +149,16 @@
     condition_fn: Callable[..., bool] = lambda _: True,
     unsupported_kwargs: Optional[List[str]] = None,
     message: str = "Arguments not supported:",
 ) -> Callable[[FunctionType], FunctionType]:
     unsupported_kwargs = unsupported_kwargs if unsupported_kwargs else []
 
     def decorator(func: FunctionType) -> FunctionType:
+        signature = inspect.signature(func)
+
         @wraps(func)
         def inner(*args: Any, **kwargs: Any) -> Any:
             passed_unsupported_kwargs = set(unsupported_kwargs).intersection(  # type: ignore
                 set([key for key, value in kwargs.items() if value is not None])
             )
 
             if condition_fn() and len(passed_unsupported_kwargs) > 0:
@@ -142,14 +167,16 @@
             return func(*args, **kwargs)
 
         inner.__doc__ = _inject_kwargs_validation_doc(
             doc=func.__doc__,
             unsupported_kwargs=unsupported_kwargs,
             message=message,
         )
+        inner.__name__ = func.__name__
+        inner.__setattr__("__signature__", signature)  # pylint: disable=no-member
 
         return cast(FunctionType, inner)
 
     return decorator
 
 
 def _inject_kwargs_validation_doc(
@@ -164,15 +191,15 @@
     insertion: str = header + kwargs_block + "\n\n"
     return _insert_str(text=doc, token="\n    Parameters", insert=insertion)
 
 
 validate_distributed_kwargs = partial(
     validate_kwargs,
     condition_fn=lambda: engine.get() == EngineEnum.RAY,
-    message=f"Following arguments not supported in distributed mode with engine `{EngineEnum.RAY}`:",
+    message=f"Following arguments are not supported in distributed mode with engine `{EngineEnum.RAY}`:",
 )
 
 
 def ensure_session(session: Union[None, boto3.Session] = None) -> boto3.Session:
     """Ensure that a valid boto3.Session will be returned."""
     if session is not None:
         return session
@@ -350,14 +377,24 @@
     verify: Optional[Union[str, bool]] = None,
 ) -> "QuickSightClient":
     ...
 
 
 @overload
 def client(
+    service_name: 'Literal["rds-data"]',
+    session: Optional[boto3.Session] = None,
+    botocore_config: Optional[Config] = None,
+    verify: Optional[Union[str, bool]] = None,
+) -> "RDSDataServiceClient":
+    ...
+
+
+@overload
+def client(
     service_name: 'Literal["redshift"]',
     session: Optional[boto3.Session] = None,
     botocore_config: Optional[Config] = None,
     verify: Optional[Union[str, bool]] = None,
 ) -> "RedshiftClient":
     ...
 
@@ -558,21 +595,59 @@
     if use_threads is True:
         cpu_cnt: Optional[int] = os.cpu_count()
         if cpu_cnt is not None:
             cpus = cpu_cnt if cpu_cnt > cpus else cpus
     return cpus
 
 
-def chunkify(lst: List[Any], num_chunks: int = 1, max_length: Optional[int] = None) -> List[List[Any]]:
+@engine.dispatch_on_engine
+def ensure_worker_or_thread_count(use_threads: Union[bool, int] = True) -> int:
+    """Get the number of CPU cores or Ray workers to be used.
+
+    Note
+    ----
+    In case of `use_threads=True` the number of threads that could be spawned will be spawned from the OS
+    or the Ray cluster configuration.
+
+
+    Parameters
+    ----------
+    use_threads : Union[bool, int]
+            True to enable multi-core utilization, False to disable.
+            If given an int will simply return the input value.
+
+    Returns
+    -------
+    int
+        Number of workers of threads to be used.
+
+    Examples
+    --------
+    >>> from awswrangler._utils import ensure_worker_or_thread_count
+    >>> ensure_worker_or_thread_count(use_threads=True)
+    4
+    >>> ensure_worker_or_thread_count(use_threads=False)
+    1
+
+    """
+    return ensure_cpu_count(use_threads=use_threads)
+
+
+ChunkifyItemType = TypeVar("ChunkifyItemType")
+
+
+def chunkify(
+    lst: List[ChunkifyItemType], num_chunks: int = 1, max_length: Optional[int] = None
+) -> List[List[ChunkifyItemType]]:
     """Split a list in a List of List (chunks) with even sizes.
 
     Parameters
     ----------
     lst: List
-        List of anything to be splitted.
+        List of anything to be split up.
     num_chunks: int, optional
         Maximum number of chunks.
     max_length: int, optional
         Max length of each chunk. Has priority over num_chunks.
 
     Returns
     -------
@@ -587,15 +662,15 @@
     >>> chunkify(list(range(13)), max_length=4)
     [[0, 1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]]
 
     """
     if not lst:
         return []
     n: int = num_chunks if max_length is None else int(math.ceil((float(len(lst)) / float(max_length))))
-    np_chunks = np.array_split(lst, n)
+    np_chunks = np.array_split(lst, n)  # type: ignore[arg-type,var-annotated]
     return [arr.tolist() for arr in np_chunks if len(arr) > 0]
 
 
 def empty_generator() -> Generator[None, None, None]:
     """Empty Generator."""
     yield from ()
 
@@ -649,25 +724,14 @@
     _logger.debug("sampling: %s", sampling)
     _logger.debug("num_samples: %s", num_samples)
     random_lst: List[Any] = random.sample(population=lst, k=num_samples)
     random_lst.sort()
     return random_lst
 
 
-def ensure_df_is_mutable(df: pd.DataFrame) -> pd.DataFrame:
-    """Ensure that all columns has the writeable flag True."""
-    for column in df.columns.to_list():
-        if hasattr(df[column].values, "flags") is True:
-            if df[column].values.flags.writeable is False:
-                s: pd.Series = df[column]
-                df[column] = None
-                df[column] = s
-    return df
-
-
 def check_duplicated_columns(df: pd.DataFrame) -> Any:
     """Raise an exception if there are duplicated columns names."""
     duplicated: List[str] = df.loc[:, df.columns.duplicated()].columns.to_list()
     if duplicated:
         raise exceptions.InvalidDataFrame(
             f"There are duplicated column names in your DataFrame: {duplicated}. "
             f"Note that your columns may have been sanitized and it can be the cause of "
@@ -793,15 +857,15 @@
 def split_pandas_frame(df: pd.DataFrame, splits: int) -> List[pd.DataFrame]:
     """Split a DataFrame into n chunks."""
     return [sub_df for sub_df in np.array_split(df, splits) if not sub_df.empty]  # type: ignore[attr-defined]
 
 
 @engine.dispatch_on_engine
 def table_refs_to_df(tables: List[pa.Table], kwargs: Dict[str, Any]) -> pd.DataFrame:
-    """Build Pandas dataframe from list of PyArrow tables."""
+    """Build Pandas DataFrame from list of PyArrow tables."""
     return _table_to_df(pa.concat_tables(tables, promote=True), kwargs=kwargs)
 
 
 @engine.dispatch_on_engine
 def is_pandas_frame(obj: Any) -> bool:
     """Check if the passed objected is a Pandas DataFrame."""
     return isinstance(obj, pd.DataFrame)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/annotations.py` & `awswrangler-3.1.0/awswrangler/annotations.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class SDKPandasDeprecatedWarning(Warning):
     """Deprecated Warning."""
 
 
 class SDKPandasExperimentalWarning(Warning):
-    """Experiental Warning."""
+    """Experimental Warning."""
 
 
 def _inject_note(
     doc: Optional[str],
     message: str,
 ) -> Optional[str]:
     token: str = "\n    Parameters"
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/athena/__init__.py` & `awswrangler-3.1.0/awswrangler/athena/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 """Amazon Athena Module."""
 
-from awswrangler.athena._read import get_query_results, read_sql_query, read_sql_table, unload  # noqa
+from awswrangler.athena._executions import (  # noqa
+    get_query_execution,
+    stop_query_execution,
+    start_query_execution,
+    wait_query,
+)
+from awswrangler.athena._read import (  # noqa
+    get_query_results,
+    read_sql_query,
+    read_sql_table,
+    unload,
+)
 from awswrangler.athena._utils import (  # noqa
     create_athena_bucket,
     create_ctas_table,
     describe_table,
     generate_create_query,
     get_named_query_statement,
     get_query_columns_types,
-    get_query_execution,
     get_query_executions,
     get_work_group,
     list_query_executions,
     repair_table,
     show_create_table,
-    start_query_execution,
-    stop_query_execution,
-    wait_query,
 )
+from awswrangler.athena._write_iceberg import to_iceberg
+
 
 __all__ = [
     "read_sql_query",
     "read_sql_table",
     "create_athena_bucket",
     "describe_table",
     "get_query_columns_types",
@@ -35,8 +44,9 @@
     "repair_table",
     "create_ctas_table",
     "show_create_table",
     "start_query_execution",
     "stop_query_execution",
     "unload",
     "wait_query",
+    "to_iceberg",
 ]
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/athena/_cache.py` & `awswrangler-3.1.0/awswrangler/athena/_cache.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/athena/_read.py` & `awswrangler-3.1.0/awswrangler/athena/_read.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Amazon Athena Module gathering all read_sql_* function."""
 
 # pylint: disable=too-many-lines
 import csv
 import logging
 import sys
 import uuid
-from typing import Any, Dict, Iterator, List, Literal, Optional, Union, cast, overload
+from datetime import date
+from typing import Any, Dict, Iterator, List, Optional, Union, cast
 
 import boto3
 import botocore.exceptions
 import pandas as pd
 
 from awswrangler import _utils, catalog, exceptions, s3, typing
 from awswrangler._config import apply_configs
@@ -34,15 +35,17 @@
 
 
 def _extract_ctas_manifest_paths(path: str, boto3_session: Optional[boto3.Session] = None) -> List[str]:
     """Get the list of paths of the generated files."""
     bucket_name, key_path = _utils.parse_path(path)
     client_s3 = _utils.client(service_name="s3", session=boto3_session)
     body: bytes = client_s3.get_object(Bucket=bucket_name, Key=key_path)["Body"].read()
-    return [x for x in body.decode("utf-8").split("\n") if x != ""]
+    paths = [x for x in body.decode("utf-8").split("\n") if x != ""]
+    _logger.debug("Read %d paths from manifest file in: %s", len(paths), path)
+    return paths
 
 
 def _fix_csv_types_generator(
     dfs: Iterator[pd.DataFrame], parse_dates: List[str], binaries: List[str]
 ) -> Iterator[pd.DataFrame]:
     """Apply data types cast to a Pandas DataFrames Generator."""
     for df in dfs:
@@ -58,15 +61,20 @@
         yield df
 
 
 def _fix_csv_types(df: pd.DataFrame, parse_dates: List[str], binaries: List[str]) -> pd.DataFrame:
     """Apply data types cast to a Pandas DataFrames."""
     if len(df.index) > 0:
         for col in parse_dates:
-            df[col] = df[col].dt.date.replace(to_replace={pd.NaT: None})
+            if pd.api.types.is_datetime64_any_dtype(df[col]):
+                df[col] = df[col].dt.date.replace(to_replace={pd.NaT: None})
+            else:
+                df[col] = (
+                    df[col].replace(to_replace={pd.NaT: None}).apply(lambda x: date.fromisoformat(x) if x else None)
+                )
         for col in binaries:
             df[col] = df[col].str.encode(encoding="utf-8")
     return df
 
 
 def _delete_after_iterate(
     dfs: Iterator[pd.DataFrame],
@@ -91,59 +99,53 @@
     boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     temp_table_fqn: Optional[str] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ret: Union[pd.DataFrame, Iterator[pd.DataFrame]]
     chunked: Union[bool, int] = False if chunksize is None else chunksize
-    _logger.debug("chunked: %s", chunked)
+    _logger.debug("Chunked: %s", chunked)
     if query_metadata.manifest_location is None:
         return _empty_dataframe_response(bool(chunked), query_metadata)
     manifest_path: str = query_metadata.manifest_location
     metadata_path: str = manifest_path.replace("-manifest.csv", ".metadata")
-    _logger.debug("manifest_path: %s", manifest_path)
-    _logger.debug("metadata_path: %s", metadata_path)
+    _logger.debug("Manifest path: %s", manifest_path)
+    _logger.debug("Metadata path: %s", metadata_path)
     paths: List[str] = _extract_ctas_manifest_paths(path=manifest_path, boto3_session=boto3_session)
     if not paths:
         if not temp_table_fqn:
             raise exceptions.EmptyDataFrame("Query would return untyped, empty dataframe.")
-
         database, temp_table_name = map(lambda x: x.replace('"', ""), temp_table_fqn.split("."))
         dtype_dict = catalog.get_table_types(database=database, table=temp_table_name, boto3_session=boto3_session)
         if dtype_dict is None:
             raise exceptions.ResourceDoesNotExist(f"Temp table {temp_table_fqn} not found.")
-
         df = pd.DataFrame(columns=list(dtype_dict.keys()))
         df = cast_pandas_with_athena_types(df=df, dtype=dtype_dict)
         df = _apply_query_metadata(df=df, query_metadata=query_metadata)
-
         if chunked:
             return (df,)
-
         return df
-
     if not pyarrow_additional_kwargs:
         pyarrow_additional_kwargs = {}
         if categories:
             pyarrow_additional_kwargs["categories"] = categories
-
+    _logger.debug("Reading Parquet result from %d paths", len(paths))
     ret = s3.read_parquet(
         path=paths,
         use_threads=use_threads,
         boto3_session=boto3_session,
         chunked=chunked,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
 
     if chunked is False:
         ret = _apply_query_metadata(df=ret, query_metadata=query_metadata)
     else:
         ret = _add_query_metadata_generator(dfs=ret, query_metadata=query_metadata)
     paths_delete: List[str] = paths + [manifest_path, metadata_path]
-    _logger.debug("type(ret): %s", type(ret))
     if chunked is False:
         if keep_files is False:
             s3.delete_objects(
                 path=paths_delete,
                 use_threads=use_threads,
                 boto3_session=boto3_session,
                 s3_additional_kwargs=s3_additional_kwargs,
@@ -165,35 +167,34 @@
     keep_files: bool,
     chunksize: Optional[int],
     use_threads: Union[bool, int],
     boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, Any]],
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     _chunksize: Optional[int] = chunksize if isinstance(chunksize, int) else None
-    _logger.debug("_chunksize: %s", _chunksize)
+    _logger.debug("Chunksize: %s", _chunksize)
     if query_metadata.output_location is None or query_metadata.output_location.endswith(".csv") is False:
         chunked = _chunksize is not None
         return _empty_dataframe_response(chunked, query_metadata)
     path: str = query_metadata.output_location
-    _logger.debug("Start CSV reading from %s", path)
+    _logger.debug("Reading CSV result from %s", path)
     ret = s3.read_csv(
         path=[path],
         dtype=query_metadata.dtype,
         parse_dates=query_metadata.parse_timestamps,
         converters=query_metadata.converters,
         quoting=csv.QUOTE_ALL,
         keep_default_na=False,
         na_values=["", "NaN"],
         chunksize=_chunksize,
         skip_blank_lines=False,
         use_threads=False,
         boto3_session=boto3_session,
     )
     _logger.debug("Start type casting...")
-    _logger.debug(type(ret))
     if _chunksize is None:
         df = _fix_csv_types(df=ret, parse_dates=query_metadata.parse_dates, binaries=query_metadata.binaries)
         df = _apply_query_metadata(df=df, query_metadata=query_metadata)
         if keep_files is False:
             s3.delete_objects(
                 path=[path, f"{path}.metadata"],
                 use_threads=use_threads,
@@ -294,15 +295,15 @@
         kms_key=kms_key,
         wait=True,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         boto3_session=boto3_session,
     )
     fully_qualified_name: str = f'"{ctas_query_info["ctas_database"]}"."{ctas_query_info["ctas_table"]}"'
     ctas_query_metadata = cast(_QueryMetadata, ctas_query_info["ctas_query_metadata"])
-    _logger.debug("ctas_query_metadata: %s", ctas_query_metadata)
+    _logger.debug("CTAS query metadata: %s", ctas_query_metadata)
     return _fetch_parquet_result(
         query_metadata=ctas_query_metadata,
         keep_files=keep_files,
         categories=categories,
         chunksize=chunksize,
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
@@ -377,27 +378,27 @@
     athena_query_wait_polling_delay: float,
     s3_additional_kwargs: Optional[Dict[str, Any]],
     boto3_session: Optional[boto3.Session],
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     wg_config: _WorkGroupConfig = _get_workgroup_config(session=boto3_session, workgroup=workgroup)
     s3_output = _get_s3_output(s3_output=s3_output, wg_config=wg_config, boto3_session=boto3_session)
     s3_output = s3_output[:-1] if s3_output[-1] == "/" else s3_output
-    _logger.debug("sql: %s", sql)
+    _logger.debug("Executing sql: %s", sql)
     query_id: str = _start_query_execution(
         sql=sql,
         wg_config=wg_config,
         database=database,
         data_source=data_source,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
         boto3_session=boto3_session,
     )
-    _logger.debug("query_id: %s", query_id)
+    _logger.debug("Query id: %s", query_id)
     query_metadata: _QueryMetadata = _get_query_metadata(
         query_execution_id=query_id,
         boto3_session=boto3_session,
         categories=categories,
         metadata_cache_manager=_cache_manager,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
     )
@@ -541,15 +542,15 @@
         unload_parameters += f"  , compression='{compression}'"
     if field_delimiter:
         unload_parameters += f"  , field_delimiter='{field_delimiter}'"
     if partitioned_by:
         unload_parameters += f"  , partitioned_by=ARRAY{partitioned_by}"
 
     sql = f"UNLOAD ({sql}) " f"TO '{path}' " f"WITH ({unload_parameters})"
-    _logger.debug("sql: %s", sql)
+    _logger.debug("Executing unload query: %s", sql)
     try:
         query_id: str = _start_query_execution(
             sql=sql,
             workgroup=workgroup,
             wg_config=wg_config,
             database=database,
             data_source=data_source,
@@ -587,69 +588,14 @@
                 "Please, don't leave undefined columns types in your query. You can cast to ensure it. "
                 "(E.g. 'SELECT CAST(NULL AS INTEGER) AS MY_COL, ...')"
             )
         raise ex
     return query_metadata
 
 
-@overload
-def get_query_results(
-    query_execution_id: str,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: Union[None, Literal[False]] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> pd.DataFrame:
-    ...
-
-
-@overload
-def get_query_results(
-    query_execution_id: str,
-    *,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: Literal[True],
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def get_query_results(
-    query_execution_id: str,
-    *,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: bool,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
-@overload
-def get_query_results(
-    query_execution_id: str,
-    *,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: int,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def get_query_results(
     query_execution_id: str,
     use_threads: Union[bool, int] = True,
@@ -674,15 +620,15 @@
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     categories: List[str], optional
         List of columns names that should be returned as pandas.Categorical.
         Recommended for memory restricted environments.
     chunksize : Union[int, bool], optional
         If passed will split the data in a Iterable of DataFrames (Memory friendly).
         If `True` awswrangler iterates on the data by files in the most efficient way without guarantee of chunksize.
-        If an `INTEGER` is passed awswrangler will iterate on the data by number of rows igual the received INTEGER.
+        If an `INTEGER` is passed awswrangler will iterate on the data by number of rows equal the received INTEGER.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     pyarrow_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
         Valid values include "split_blocks", "self_destruct", "ignore_metadata".
         e.g. pyarrow_additional_kwargs={'split_blocks': True}.
@@ -705,16 +651,18 @@
     query_metadata: _QueryMetadata = _get_query_metadata(
         query_execution_id=query_execution_id,
         boto3_session=boto3_session,
         categories=categories,
         metadata_cache_manager=_cache_manager,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
     )
+    _logger.debug("Query metadata:\n%s", query_metadata)
     client_athena = _utils.client(service_name="athena", session=boto3_session)
     query_info = client_athena.get_query_execution(QueryExecutionId=query_execution_id)["QueryExecution"]
+    _logger.debug("Query info:\n%s", query_info)
     statement_type: Optional[str] = query_info.get("StatementType")
     if (statement_type == "DDL" and query_info["Query"].startswith("CREATE TABLE")) or (
         statement_type == "DML" and query_info["Query"].startswith("UNLOAD")
     ):
         return _fetch_parquet_result(
             query_metadata=query_metadata,
             keep_files=True,
@@ -733,153 +681,14 @@
             use_threads=use_threads,
             boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
         )
     raise exceptions.UndetectedType(f"""Unable to get results for: {query_info["Query"]}.""")
 
 
-@overload
-def read_sql_query(  # pylint: disable=too-many-arguments
-    sql: str,
-    database: str,
-    ctas_approach: bool = ...,
-    unload_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: Union[None, Literal[False]] = ...,
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> pd.DataFrame:
-    ...
-
-
-@overload
-def read_sql_query(
-    sql: str,
-    database: str,
-    *,
-    ctas_approach: bool = ...,
-    unload_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: Literal[True],
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_sql_query(
-    sql: str,
-    database: str,
-    *,
-    ctas_approach: bool = ...,
-    unload_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: bool,
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
-@overload
-def read_sql_query(
-    sql: str,
-    database: str,
-    *,
-    ctas_approach: bool = ...,
-    unload_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: int,
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_sql_query(
-    sql: str,
-    database: str,
-    *,
-    ctas_approach: bool = ...,
-    unload_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: Optional[Union[int, bool]],
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
 )
 def read_sql_query(  # pylint: disable=too-many-arguments,too-many-locals
     sql: str,
     database: str,
@@ -903,19 +712,19 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Execute any SQL query on AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -971,15 +780,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -1026,24 +835,24 @@
     ctas_approach: bool
         Wraps the query using a CTAS, and read the resulted parquet data on S3.
         If false, read the regular CSV on S3.
     unload_approach: bool
         Wraps the query using UNLOAD, and read the results from S3.
         Only PARQUET format is supported.
     ctas_parameters: typing.AthenaCTASSettings, optional
-        Params of the CTAS such as database, temp_table_name, bucketing_info, and compression.
+        Parameters of the CTAS such as database, temp_table_name, bucketing_info, and compression.
     unload_parameters : typing.AthenaUNLOADSettings, optional
-        Params of the UNLOAD such as format, compression, field_delimiter, and partitioned_by.
+        Parameters of the UNLOAD such as format, compression, field_delimiter, and partitioned_by.
     categories: List[str], optional
         List of columns names that should be returned as pandas.Categorical.
         Recommended for memory restricted environments.
     chunksize : Union[int, bool], optional
         If passed will split the data in a Iterable of DataFrames (Memory friendly).
         If `True` awswrangler iterates on the data by files in the most efficient way without guarantee of chunksize.
-        If an `INTEGER` is passed awswrangler will iterate on the data by number of rows igual the received INTEGER.
+        If an `INTEGER` is passed awswrangler will iterate on the data by number of rows equal the received INTEGER.
     s3_output : str, optional
         Amazon S3 path.
     workgroup : str, optional
         Athena workgroup.
     encryption : str, optional
         Valid values: [None, 'SSE_S3', 'SSE_KMS']. Notice: 'CSE_KMS' is not supported.
     kms_key : str, optional
@@ -1053,15 +862,15 @@
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     athena_cache_settings: typing.AthenaCacheSettings, optional
-        Params of the Athena cache settings such as max_cache_seconds, max_cache_query_inspections,
+        Parameters of the Athena cache settings such as max_cache_seconds, max_cache_query_inspections,
         max_remote_cache_entries, and max_local_cache_entries.
         AthenaCacheSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaCacheSettings or as a regular Python dict.
         If cached results are valid, awswrangler ignores the `ctas_approach`, `s3_output`, `encryption`, `kms_key`,
         `keep_files` and `ctas_temp_table_name` params.
         If reading cached data fails for any reason, execution falls back to the usual query run path.
     data_source : str, optional
@@ -1137,15 +946,15 @@
         sql=sql,
         boto3_session=boto3_session,
         workgroup=workgroup,
         max_cache_seconds=max_cache_seconds,
         max_cache_query_inspections=max_cache_query_inspections,
         max_remote_cache_entries=max_remote_cache_entries,
     )
-    _logger.debug("cache_info:\n%s", cache_info)
+    _logger.debug("Cache info:\n%s", cache_info)
     if cache_info.has_valid_cache is True:
         _logger.debug("Valid cache found. Retrieving...")
         try:
             return _resolve_query_with_cache(
                 cache_info=cache_info,
                 categories=categories,
                 chunksize=chunksize,
@@ -1187,144 +996,14 @@
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
 
 
-@overload
-def read_sql_table(
-    table: str,
-    database: str,
-    *,
-    unload_approach: bool = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    ctas_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: Union[None, Literal[False]] = ...,
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> pd.DataFrame:
-    ...
-
-
-@overload
-def read_sql_table(
-    table: str,
-    database: str,
-    *,
-    unload_approach: bool = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    ctas_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: Literal[True],
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_sql_table(
-    table: str,
-    database: str,
-    *,
-    unload_approach: bool = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    ctas_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: bool,
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
-@overload
-def read_sql_table(
-    table: str,
-    database: str,
-    *,
-    unload_approach: bool = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    ctas_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: int,
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_sql_table(
-    table: str,
-    database: str,
-    *,
-    unload_approach: bool = ...,
-    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
-    ctas_approach: bool = ...,
-    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
-    categories: Optional[List[str]] = ...,
-    chunksize: Optional[Union[int, bool]],
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    keep_files: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    data_source: Optional[str] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
 )
 def read_sql_table(
     table: str,
     database: str,
@@ -1346,19 +1025,19 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Extract the full table AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -1414,15 +1093,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -1467,24 +1146,24 @@
     ctas_approach: bool
         Wraps the query using a CTAS, and read the resulted parquet data on S3.
         If false, read the regular CSV on S3.
     unload_approach: bool
         Wraps the query using UNLOAD, and read the results from S3.
         Only PARQUET format is supported.
     ctas_parameters: typing.AthenaCTASSettings, optional
-        Params of the CTAS such as database, temp_table_name, bucketing_info, and compression.
+        Parameters of the CTAS such as database, temp_table_name, bucketing_info, and compression.
     unload_parameters : typing.AthenaUNLOADSettings, optional
-        Params of the UNLOAD such as format, compression, field_delimiter, and partitioned_by.
+        Parameters of the UNLOAD such as format, compression, field_delimiter, and partitioned_by.
     categories: List[str], optional
         List of columns names that should be returned as pandas.Categorical.
         Recommended for memory restricted environments.
     chunksize : Union[int, bool], optional
         If passed will split the data in a Iterable of DataFrames (Memory friendly).
         If `True` awswrangler iterates on the data by files in the most efficient way without guarantee of chunksize.
-        If an `INTEGER` is passed awswrangler will iterate on the data by number of rows igual the received INTEGER.
+        If an `INTEGER` is passed awswrangler will iterate on the data by number of rows equal the received INTEGER.
     s3_output : str, optional
         AWS S3 path.
     workgroup : str, optional
         Athena workgroup.
     encryption : str, optional
         Valid values: [None, 'SSE_S3', 'SSE_KMS']. Notice: 'CSE_KMS' is not supported.
     kms_key : str, optional
@@ -1494,15 +1173,15 @@
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     athena_cache_settings: typing.AthenaCacheSettings, optional
-        Params of the Athena cache settings such as max_cache_seconds, max_cache_query_inspections,
+        Parameters of the Athena cache settings such as max_cache_seconds, max_cache_query_inspections,
         max_remote_cache_entries, and max_local_cache_entries.
         AthenaCacheSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaCacheSettings or as a regular Python dict.
         If cached results are valid, awswrangler ignores the `ctas_approach`, `s3_output`, `encryption`, `kms_key`,
         `keep_files` and `ctas_temp_table_name` params.
         If reading cached data fails for any reason, execution falls back to the usual query run path.
     data_source : str, optional
@@ -1524,15 +1203,14 @@
     --------
     >>> import awswrangler as wr
     >>> df = wr.athena.read_sql_table(table="...", database="...")
     >>> scanned_bytes = df.query_metadata["Statistics"]["DataScannedInBytes"]
 
     """
     table = catalog.sanitize_table_name(table=table)
-
     return read_sql_query(
         sql=f'SELECT * FROM "{table}"',
         database=database,
         ctas_approach=ctas_approach,
         unload_approach=unload_approach,
         ctas_parameters=ctas_parameters,
         unload_parameters=unload_parameters,
@@ -1622,15 +1300,14 @@
     ...     sql="SELECT * FROM my_table WHERE name=:name AND city=:city",
     ...     params={"name": "filtered_name", "city": "filtered_city"}
     ... )
 
     """
     # Substitute query parameters
     sql = _process_sql_params(sql, params)
-
     return _unload(
         sql=sql,
         path=path,
         file_format=file_format,
         compression=compression,
         field_delimiter=field_delimiter,
         partitioned_by=partitioned_by,
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/athena/_utils.py` & `awswrangler-3.1.0/awswrangler/athena/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 """Utilities Module for Amazon Athena."""
 import base64
 import csv
 import json
 import logging
 import pprint
-import time
 import uuid
 import warnings
 from decimal import Decimal
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Generator,
     List,
-    Literal,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Union,
     cast,
-    overload,
 )
 
 import boto3
 import botocore.exceptions
 import pandas as pd
 
 from awswrangler import _data_types, _utils, catalog, exceptions, s3, sts, typing
 from awswrangler._config import apply_configs
-from awswrangler._sql_formatter import _process_sql_params
 from awswrangler.catalog._utils import _catalog_id, _transaction_id
 
-from ._cache import _cache_manager, _CacheInfo, _check_for_cached_results, _LocalMetadataCacheManager
+from . import _executions
+from ._cache import _cache_manager, _LocalMetadataCacheManager
 
 if TYPE_CHECKING:
     from mypy_boto3_glue.type_defs import ColumnTypeDef
 
 _QUERY_FINAL_STATES: List[str] = ["FAILED", "SUCCEEDED", "CANCELLED"]
 _QUERY_WAIT_POLLING_DELAY: float = 1.0  # SECONDS
 
@@ -112,22 +109,23 @@
             args["QueryExecutionContext"]["Catalog"] = data_source
 
     # workgroup
     if workgroup is not None:
         args["WorkGroup"] = workgroup
 
     client_athena = _utils.client(service_name="athena", session=boto3_session)
-    _logger.debug("args: \n%s", pprint.pformat(args))
+    _logger.debug("Starting query execution with args: \n%s", pprint.pformat(args))
     response = _utils.try_it(
         f=client_athena.start_query_execution,
         ex=botocore.exceptions.ClientError,
         ex_code="ThrottlingException",
         max_num_tries=5,
         **args,
     )
+    _logger.debug("Query response:\n%s", response)
     return response["QueryExecutionId"]
 
 
 def _get_workgroup_config(session: Optional[boto3.Session] = None, workgroup: Optional[str] = None) -> _WorkGroupConfig:
     enforced: bool
     wg_s3_output: Optional[str]
     wg_encryption: Optional[str]
@@ -142,28 +140,28 @@
             wg_s3_output = config.get("OutputLocation")
             encrypt_config: Optional[Dict[str, str]] = config.get("EncryptionConfiguration")
             wg_encryption = None if encrypt_config is None else encrypt_config.get("EncryptionOption")
             wg_kms_key = None if encrypt_config is None else encrypt_config.get("KmsKey")
     wg_config: _WorkGroupConfig = _WorkGroupConfig(
         enforced=enforced, s3_output=wg_s3_output, encryption=wg_encryption, kms_key=wg_kms_key
     )
-    _logger.debug("wg_config:\n%s", wg_config)
+    _logger.debug("Workgroup config:\n%s", wg_config)
     return wg_config
 
 
 def _fetch_txt_result(
     query_metadata: _QueryMetadata,
     keep_files: bool,
     boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, str]],
 ) -> pd.DataFrame:
     if query_metadata.output_location is None or query_metadata.output_location.endswith(".txt") is False:
         return pd.DataFrame()
     path: str = query_metadata.output_location
-    _logger.debug("Start TXT reading from %s", path)
+    _logger.debug("Reading TXT result from %s", path)
     df = s3.read_csv(
         path=[path],
         dtype=query_metadata.dtype,
         parse_dates=query_metadata.parse_timestamps,
         converters=query_metadata.converters,
         quoting=csv.QUOTE_ALL,
         keep_default_na=False,
@@ -213,23 +211,23 @@
     """Get query metadata."""
     if (query_execution_payload is not None) and (query_execution_payload["Status"]["State"] in _QUERY_FINAL_STATES):
         if query_execution_payload["Status"]["State"] != "SUCCEEDED":
             reason: str = query_execution_payload["Status"]["StateChangeReason"]
             raise exceptions.QueryFailed(f"Query error: {reason}")
         _query_execution_payload: Dict[str, Any] = query_execution_payload
     else:
-        _query_execution_payload = wait_query(
+        _query_execution_payload = _executions.wait_query(
             query_execution_id=query_execution_id,
             boto3_session=boto3_session,
             athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         )
     cols_types: Dict[str, str] = get_query_columns_types(
         query_execution_id=query_execution_id, boto3_session=boto3_session
     )
-    _logger.debug("cols_types: %s", cols_types)
+    _logger.debug("Casting query column types: %s", cols_types)
     dtype: Dict[str, str] = {}
     parse_timestamps: List[str] = []
     parse_dates: List[str] = []
     converters: Dict[str, Any] = {}
     binaries: List[str] = []
     col_name: str
     col_type: str
@@ -265,22 +263,22 @@
         parse_dates=parse_dates,
         converters=converters,
         binaries=binaries,
         output_location=output_location,
         manifest_location=manifest_location,
         raw_payload=_query_execution_payload,
     )
-    _logger.debug("query_metadata:\n%s", query_metadata)
+    _logger.debug("Query metadata:\n%s", query_metadata)
     return query_metadata
 
 
 def _empty_dataframe_response(
     chunked: bool, query_metadata: _QueryMetadata
 ) -> Union[pd.DataFrame, Generator[None, None, None]]:
-    """Generate an empty dataframe response."""
+    """Generate an empty DataFrame response."""
     if chunked is False:
         df = pd.DataFrame()
         df = _apply_query_metadata(df=df, query_metadata=query_metadata)
         return df
     return _utils.empty_generator()
 
 
@@ -383,192 +381,14 @@
     except botocore.exceptions.ClientError as err:
         if err.response["Error"]["Code"] == "OperationAborted":
             _logger.debug("A conflicting conditional operation is currently in progress against this resource.")
     client_s3.get_waiter("bucket_exists").wait(Bucket=bucket_name)
     return path
 
 
-@overload
-def start_query_execution(
-    sql: str,
-    database: Optional[str] = ...,
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    params: Optional[Dict[str, Any]] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    athena_query_wait_polling_delay: float = ...,
-    data_source: Optional[str] = ...,
-    wait: Literal[False] = ...,
-) -> str:
-    ...
-
-
-@overload
-def start_query_execution(
-    sql: str,
-    *,
-    database: Optional[str] = ...,
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    params: Optional[Dict[str, Any]] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    athena_query_wait_polling_delay: float = ...,
-    data_source: Optional[str] = ...,
-    wait: Literal[True],
-) -> Dict[str, Any]:
-    ...
-
-
-@overload
-def start_query_execution(
-    sql: str,
-    *,
-    database: Optional[str] = ...,
-    s3_output: Optional[str] = ...,
-    workgroup: Optional[str] = ...,
-    encryption: Optional[str] = ...,
-    kms_key: Optional[str] = ...,
-    params: Optional[Dict[str, Any]] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
-    athena_query_wait_polling_delay: float = ...,
-    data_source: Optional[str] = ...,
-    wait: bool,
-) -> Union[str, Dict[str, Any]]:
-    ...
-
-
-@apply_configs
-def start_query_execution(
-    sql: str,
-    database: Optional[str] = None,
-    s3_output: Optional[str] = None,
-    workgroup: Optional[str] = None,
-    encryption: Optional[str] = None,
-    kms_key: Optional[str] = None,
-    params: Optional[Dict[str, Any]] = None,
-    boto3_session: Optional[boto3.Session] = None,
-    athena_cache_settings: Optional[typing.AthenaCacheSettings] = None,
-    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
-    data_source: Optional[str] = None,
-    wait: bool = False,
-) -> Union[str, Dict[str, Any]]:
-    """Start a SQL Query against AWS Athena.
-
-    Note
-    ----
-    Create the default Athena bucket if it doesn't exist and s3_output is None.
-    (E.g. s3://aws-athena-query-results-ACCOUNT-REGION/)
-
-    Parameters
-    ----------
-    sql : str
-        SQL query.
-    database : str, optional
-        AWS Glue/Athena database name.
-    s3_output : str, optional
-        AWS S3 path.
-    workgroup : str, optional
-        Athena workgroup.
-    encryption : str, optional
-        None, 'SSE_S3', 'SSE_KMS', 'CSE_KMS'.
-    kms_key : str, optional
-        For SSE-KMS and CSE-KMS , this is the KMS key ARN or ID.
-    params: Dict[str, any], optional
-        Dict of parameters that will be used for constructing the SQL query. Only named parameters are supported.
-        The dict needs to contain the information in the form {'name': 'value'} and the SQL query needs to contain
-        `:name`. Note that for varchar columns and similar, you must surround the value in single quotes.
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    athena_cache_settings: typing.AthenaCacheSettings, optional
-        Params of the Athena cache settings such as max_cache_seconds, max_cache_query_inspections,
-        max_remote_cache_entries, and max_local_cache_entries.
-        AthenaCacheSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
-        instance of AthenaCacheSettings or as a regular Python dict.
-        If cached results are valid, awswrangler ignores the `ctas_approach`, `s3_output`, `encryption`, `kms_key`,
-        `keep_files` and `ctas_temp_table_name` params.
-        If reading cached data fails for any reason, execution falls back to the usual query run path.
-    athena_query_wait_polling_delay: float, default: 0.25 seconds
-        Interval in seconds for how often the function will check if the Athena query has completed.
-    data_source : str, optional
-        Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
-    wait : bool, default False
-        Indicates whether to wait for the query to finish and return a dictionary with the query execution response.
-
-    Returns
-    -------
-    Union[str, Dict[str, Any]]
-        Query execution ID if `wait` is set to `False`, dictionary with the get_query_execution response otherwise.
-
-    Examples
-    --------
-    Querying into the default data source (Amazon s3 - 'AwsDataCatalog')
-
-    >>> import awswrangler as wr
-    >>> query_exec_id = wr.athena.start_query_execution(sql='...', database='...')
-
-    Querying into another data source (PostgreSQL, Redshift, etc)
-
-    >>> import awswrangler as wr
-    >>> query_exec_id = wr.athena.start_query_execution(sql='...', database='...', data_source='...')
-
-    """
-    sql = _process_sql_params(sql, params)
-
-    athena_cache_settings = athena_cache_settings if athena_cache_settings else {}
-    max_cache_seconds = athena_cache_settings.get("max_cache_seconds", 0)
-    max_cache_query_inspections = athena_cache_settings.get("max_cache_query_inspections", 50)
-    max_remote_cache_entries = athena_cache_settings.get("max_remote_cache_entries", 50)
-    max_local_cache_entries = athena_cache_settings.get("max_local_cache_entries", 100)
-
-    max_remote_cache_entries = min(max_remote_cache_entries, max_local_cache_entries)
-
-    _cache_manager.max_cache_size = max_local_cache_entries
-    cache_info: _CacheInfo = _check_for_cached_results(
-        sql=sql,
-        boto3_session=boto3_session,
-        workgroup=workgroup,
-        max_cache_seconds=max_cache_seconds,
-        max_cache_query_inspections=max_cache_query_inspections,
-        max_remote_cache_entries=max_remote_cache_entries,
-    )
-    _logger.debug("cache_info:\n%s", cache_info)
-
-    if cache_info.has_valid_cache and cache_info.query_execution_id is not None:
-        query_execution_id = cache_info.query_execution_id
-        _logger.debug("Valid cache found. Retrieving...")
-    else:
-        wg_config: _WorkGroupConfig = _get_workgroup_config(session=boto3_session, workgroup=workgroup)
-        query_execution_id = _start_query_execution(
-            sql=sql,
-            wg_config=wg_config,
-            database=database,
-            data_source=data_source,
-            s3_output=s3_output,
-            workgroup=workgroup,
-            encryption=encryption,
-            kms_key=kms_key,
-            boto3_session=boto3_session,
-        )
-    if wait:
-        return wait_query(
-            query_execution_id=query_execution_id,
-            boto3_session=boto3_session,
-            athena_query_wait_polling_delay=athena_query_wait_polling_delay,
-        )
-
-    return query_execution_id
-
-
 @apply_configs
 def repair_table(
     table: str,
     database: Optional[str] = None,
     data_source: Optional[str] = None,
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
@@ -621,25 +441,25 @@
     >>> import awswrangler as wr
     >>> query_final_state = wr.athena.repair_table(table='...', database='...')
 
     """
     query = f"MSCK REPAIR TABLE `{table}`;"
     if (database is not None) and (not database.startswith("`")):
         database = f"`{database}`"
-    query_id = start_query_execution(
+    query_id = _executions.start_query_execution(
         sql=query,
         database=database,
         data_source=data_source,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
         boto3_session=boto3_session,
     )
-    response: Dict[str, Any] = wait_query(
+    response: Dict[str, Any] = _executions.wait_query(
         query_execution_id=query_id,
         boto3_session=boto3_session,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
     )
     return cast(str, response["Status"]["State"])
 
 
@@ -689,26 +509,26 @@
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     pandas.DataFrame
-        Pandas DataFrame filled by formatted infos.
+        Pandas DataFrame filled by formatted table information.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> df_table = wr.athena.describe_table(table='my_table', database='default')
 
     """
     query = f"DESCRIBE `{table}`;"
     if (database is not None) and (not database.startswith("`")):
         database = f"`{database}`"
-    query_id = start_query_execution(
+    query_id = _executions.start_query_execution(
         sql=query,
         database=database,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
         boto3_session=boto3_session,
@@ -937,14 +757,15 @@
                 raise exceptions.InvalidArgumentValue(
                     "Please, don't leave undefined columns types in your query. You can cast to ensure it. "
                     "(E.g. 'SELECT CAST(NULL AS INTEGER) AS MY_COL, ...')"
                 )
             raise ex
     else:
         response["ctas_query_id"] = query_execution_id
+    _logger.info("Created CTAS table %s", fully_qualified_name)
     return response
 
 
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
@@ -1000,15 +821,15 @@
     >>> import awswrangler as wr
     >>> df_table = wr.athena.show_create_table(table='my_table', database='default')
 
     """
     query = f"SHOW CREATE TABLE `{table}`;"
     if (database is not None) and (not database.startswith("`")):
         database = f"`{database}`"
-    query_id = start_query_execution(
+    query_id = _executions.start_query_execution(
         sql=query,
         database=database,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
         boto3_session=boto3_session,
@@ -1115,15 +936,17 @@
             f"""  '{table_detail['StorageDescriptor']['InputFormat']}' """,
             """OUTPUTFORMAT """,
             f"""  '{table_detail['StorageDescriptor']['OutputFormat']}'""",
             """LOCATION""",
             f"""  '{table_detail['StorageDescriptor']['Location']}'""",
             f"""TBLPROPERTIES (\n{tblproperties})""",
         ]
-        return "\n".join(query_parts)
+        sql = "\n".join(query_parts)
+        _logger.debug("Generated create query:\n%s", sql)
+        return sql
     raise NotImplementedError()
 
 
 def get_work_group(workgroup: str, boto3_session: Optional[boto3.Session] = None) -> Dict[str, Any]:
     """Return information about the workgroup with the specified name.
 
     Parameters
@@ -1153,118 +976,14 @@
             ex_code="ThrottlingException",
             max_num_tries=5,
             WorkGroup=workgroup,
         ),
     )
 
 
-def stop_query_execution(query_execution_id: str, boto3_session: Optional[boto3.Session] = None) -> None:
-    """Stop a query execution.
-
-    Requires you to have access to the workgroup in which the query ran.
-
-    Parameters
-    ----------
-    query_execution_id : str
-        Athena query execution ID.
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-
-    Returns
-    -------
-    None
-        None.
-
-    Examples
-    --------
-    >>> import awswrangler as wr
-    >>> wr.athena.stop_query_execution(query_execution_id='query-execution-id')
-
-    """
-    client_athena = _utils.client(service_name="athena", session=boto3_session)
-    client_athena.stop_query_execution(QueryExecutionId=query_execution_id)
-
-
-@apply_configs
-def wait_query(
-    query_execution_id: str,
-    boto3_session: Optional[boto3.Session] = None,
-    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
-) -> Dict[str, Any]:
-    """Wait for the query end.
-
-    Parameters
-    ----------
-    query_execution_id : str
-        Athena query execution ID.
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    athena_query_wait_polling_delay: float, default: 0.25 seconds
-        Interval in seconds for how often the function will check if the Athena query has completed.
-
-    Returns
-    -------
-    Dict[str, Any]
-        Dictionary with the get_query_execution response.
-
-    Examples
-    --------
-    >>> import awswrangler as wr
-    >>> res = wr.athena.wait_query(query_execution_id='query-execution-id')
-
-    """
-    response: Dict[str, Any] = get_query_execution(query_execution_id=query_execution_id, boto3_session=boto3_session)
-    state: str = response["Status"]["State"]
-    while state not in _QUERY_FINAL_STATES:
-        time.sleep(athena_query_wait_polling_delay)
-        response = get_query_execution(query_execution_id=query_execution_id, boto3_session=boto3_session)
-        state = response["Status"]["State"]
-    _logger.debug("state: %s", state)
-    _logger.debug("StateChangeReason: %s", response["Status"].get("StateChangeReason"))
-    if state == "FAILED":
-        raise exceptions.QueryFailed(response["Status"].get("StateChangeReason"))
-    if state == "CANCELLED":
-        raise exceptions.QueryCancelled(response["Status"].get("StateChangeReason"))
-    return response
-
-
-def get_query_execution(query_execution_id: str, boto3_session: Optional[boto3.Session] = None) -> Dict[str, Any]:
-    """Fetch query execution details.
-
-    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_query_execution
-
-    Parameters
-    ----------
-    query_execution_id : str
-        Athena query execution ID.
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-
-    Returns
-    -------
-    Dict[str, Any]
-        Dictionary with the get_query_execution response.
-
-    Examples
-    --------
-    >>> import awswrangler as wr
-    >>> res = wr.athena.get_query_execution(query_execution_id='query-execution-id')
-
-    """
-    client_athena = _utils.client(service_name="athena", session=boto3_session)
-    response = _utils.try_it(
-        f=client_athena.get_query_execution,
-        ex=botocore.exceptions.ClientError,
-        ex_code="ThrottlingException",
-        max_num_tries=5,
-        QueryExecutionId=query_execution_id,
-    )
-    return cast(Dict[str, Any], response["QueryExecution"])
-
-
 def get_query_executions(
     query_execution_ids: List[str], return_unprocessed: bool = False, boto3_session: Optional[boto3.Session] = None
 ) -> Union[Tuple[pd.DataFrame, pd.DataFrame], pd.DataFrame]:
     """From specified query execution IDs, return a DataFrame of query execution details.
 
     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.batch_get_query_execution
 
@@ -1355,8 +1074,9 @@
             f=client_athena.list_query_executions,
             ex=botocore.exceptions.ClientError,
             ex_code="ThrottlingException",
             max_num_tries=5,
             **kwargs,
         )
         query_list += response["QueryExecutionIds"]
+    _logger.debug("Running %d query executions", len(query_list))
     return query_list
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/catalog/__init__.py` & `awswrangler-3.1.0/awswrangler/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/catalog/_add.py` & `awswrangler-3.1.0/awswrangler/catalog/_add.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/catalog/_create.py` & `awswrangler-3.1.0/awswrangler/catalog/_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """AWS Glue Catalog Module."""
 
 import logging
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, Literal, Optional
 
 import boto3
 
 from awswrangler import _utils, exceptions, typing
 from awswrangler._config import apply_configs
 from awswrangler.catalog._definitions import _csv_table_definition, _json_table_definition, _parquet_table_definition
 from awswrangler.catalog._delete import delete_all_partitions, delete_table_if_exists
@@ -246,14 +246,37 @@
                 transaction_id=transaction_id, DatabaseName=database, TableInput=table_input, SkipArchive=skip_archive
             ),
         )
     )
     return parameters
 
 
+def _update_table_input(table_input: Dict[str, Any], columns_types: Dict[str, str], allow_reorder: bool = True) -> bool:
+    column_updated = False
+
+    catalog_cols: Dict[str, str] = {x["Name"]: x["Type"] for x in table_input["StorageDescriptor"]["Columns"]}
+
+    if not allow_reorder:
+        for catalog_key, frame_key in zip(catalog_cols, columns_types):
+            if catalog_key != frame_key:
+                raise exceptions.InvalidArgumentValue(f"Column {frame_key} is out of order.")
+
+    for c, t in columns_types.items():
+        if c not in catalog_cols:
+            _logger.debug("New column %s with type %s.", c, t)
+            table_input["StorageDescriptor"]["Columns"].append({"Name": c, "Type": t})
+            column_updated = True
+        elif t != catalog_cols[c]:  # Data type change detected!
+            raise exceptions.InvalidArgumentValue(
+                f"Data type change detected on column {c} (Old type: {catalog_cols[c]} / New type {t})."
+            )
+
+    return column_updated
+
+
 def _create_parquet_table(
     database: str,
     table: str,
     path: str,
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Optional[Dict[str, str]],
@@ -269,27 +292,22 @@
     athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings],
     boto3_session: Optional[boto3.Session],
     catalog_table_input: Optional[Dict[str, Any]],
 ) -> None:
     table = sanitize_table_name(table=table)
     partitions_types = {} if partitions_types is None else partitions_types
     _logger.debug("catalog_table_input: %s", catalog_table_input)
+
     table_input: Dict[str, Any]
     if (catalog_table_input is not None) and (mode in ("append", "overwrite_partitions")):
         table_input = catalog_table_input
-        catalog_cols: Dict[str, str] = {x["Name"]: x["Type"] for x in table_input["StorageDescriptor"]["Columns"]}
-        for c, t in columns_types.items():
-            if c not in catalog_cols:
-                _logger.debug("New column %s with type %s.", c, t)
-                table_input["StorageDescriptor"]["Columns"].append({"Name": c, "Type": t})
-                mode = "update"
-            elif t != catalog_cols[c]:  # Data type change detected!
-                raise exceptions.InvalidArgumentValue(
-                    f"Data type change detected on column {c} (Old type: {catalog_cols[c]} / New type {t})."
-                )
+
+        is_table_updated = _update_table_input(table_input, columns_types)
+        if is_table_updated:
+            mode = "update"
     else:
         table_input = _parquet_table_definition(
             table=table,
             path=path,
             columns_types=columns_types,
             table_type=table_type,
             partitions_types=partitions_types,
@@ -341,19 +359,26 @@
     athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings],
     catalog_table_input: Optional[Dict[str, Any]],
     catalog_id: Optional[str],
 ) -> None:
     table = sanitize_table_name(table=table)
     partitions_types = {} if partitions_types is None else partitions_types
     _logger.debug("catalog_table_input: %s", catalog_table_input)
-    table_input: Dict[str, Any]
+
     if schema_evolution is False:
         _utils.check_schema_changes(columns_types=columns_types, table_input=catalog_table_input, mode=mode)
+
+    table_input: Dict[str, Any]
     if (catalog_table_input is not None) and (mode in ("append", "overwrite_partitions")):
         table_input = catalog_table_input
+
+        is_table_updated = _update_table_input(table_input, columns_types, allow_reorder=False)
+        if is_table_updated:
+            mode = "update"
+
     else:
         table_input = _csv_table_definition(
             table=table,
             path=path,
             columns_types=columns_types,
             table_type=table_type,
             partitions_types=partitions_types,
@@ -381,15 +406,15 @@
         partitions_types=partitions_types,
         transaction_id=transaction_id,
         athena_partition_projection_settings=athena_partition_projection_settings,
         catalog_id=catalog_id,
     )
 
 
-def _create_json_table(  # pylint: disable=too-many-arguments
+def _create_json_table(  # pylint: disable=too-many-arguments,too-many-locals
     database: str,
     table: str,
     path: str,
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Optional[Dict[str, str]],
     bucketing_info: Optional[typing.BucketingInfoTuple],
@@ -412,14 +437,19 @@
     partitions_types = {} if partitions_types is None else partitions_types
     _logger.debug("catalog_table_input: %s", catalog_table_input)
     table_input: Dict[str, Any]
     if schema_evolution is False:
         _utils.check_schema_changes(columns_types=columns_types, table_input=catalog_table_input, mode=mode)
     if (catalog_table_input is not None) and (mode in ("append", "overwrite_partitions")):
         table_input = catalog_table_input
+
+        is_table_updated = _update_table_input(table_input, columns_types)
+        if is_table_updated:
+            mode = "update"
+
     else:
         table_input = _json_table_definition(
             table=table,
             path=path,
             columns_types=columns_types,
             table_type=table_type,
             partitions_types=partitions_types,
@@ -579,30 +609,34 @@
 
 @apply_configs
 def create_database(
     name: str,
     description: Optional[str] = None,
     catalog_id: Optional[str] = None,
     exist_ok: bool = False,
+    database_input_args: Optional[Dict[str, Any]] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> None:
     """Create a database in AWS Glue Catalog.
 
     Parameters
     ----------
     name : str
         Database name.
     description : str, optional
-        A Descrption for the Database.
+        A description for the Database.
     catalog_id : str, optional
         The ID of the Data Catalog from which to retrieve Databases.
         If none is provided, the AWS account ID is used by default.
     exist_ok : bool
         If set to True will not raise an Exception if a Database with the same already exists.
         In this case the description will be updated if it is different from the current one.
+    database_input_args : dict[str, Any], optional
+        Additional metadata to pass to database creation. Supported arguments listed here:
+        https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_database
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     None
         None.
@@ -611,24 +645,26 @@
     --------
     >>> import awswrangler as wr
     >>> wr.catalog.create_database(
     ...     name='awswrangler_test'
     ... )
     """
     client_glue = _utils.client(service_name="glue", session=boto3_session)
-    args: Dict[str, str] = {"Name": name}
+    args: Dict[str, Any] = {"Name": name, **database_input_args} if database_input_args else {"Name": name}
     if description is not None:
         args["Description"] = description
 
     try:
         r = client_glue.get_database(**_catalog_id(catalog_id=catalog_id, Name=name))
         if not exist_ok:
             raise exceptions.AlreadyExists(f"Database {name} already exists and <exist_ok> is set to False.")
-        if description and description != r["Database"].get("Description", ""):
-            client_glue.update_database(**_catalog_id(catalog_id=catalog_id, Name=name, DatabaseInput=args))
+        for k, v in args.items():
+            if v != r["Database"].get(k, ""):
+                client_glue.update_database(**_catalog_id(catalog_id=catalog_id, Name=name, DatabaseInput=args))
+                break
     except client_glue.exceptions.EntityNotFoundException:
         client_glue.create_database(**_catalog_id(catalog_id=catalog_id, DatabaseInput=args))
 
 
 @apply_configs
 def create_parquet_table(
     database: str,
@@ -639,15 +675,15 @@
     partitions_types: Optional[Dict[str, str]] = None,
     bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     catalog_id: Optional[str] = None,
     compression: Optional[str] = None,
     description: Optional[str] = None,
     parameters: Optional[Dict[str, str]] = None,
     columns_comments: Optional[Dict[str, str]] = None,
-    mode: str = "overwrite",
+    mode: Literal["overwrite", "append"] = "overwrite",
     catalog_versioning: bool = False,
     transaction_id: Optional[str] = None,
     athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> None:
     """Create a Parquet Table (Metadata Only) in the AWS Glue Catalog.
 
@@ -685,15 +721,15 @@
     mode: str
         'overwrite' to recreate any possible existing table or 'append' to keep any possible existing table.
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     transaction_id: str, optional
         The ID of the transaction (i.e. used with GOVERNED tables).
     athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
-        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        Parameters of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
         AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaPartitionProjectionSettings or as a regular Python dict.
 
         Following projection parameters are supported:
 
         .. list-table:: Projection Parameters
            :header-rows: 1
@@ -800,15 +836,15 @@
     table_type: Optional[str] = None,
     partitions_types: Optional[Dict[str, str]] = None,
     bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     compression: Optional[str] = None,
     description: Optional[str] = None,
     parameters: Optional[Dict[str, str]] = None,
     columns_comments: Optional[Dict[str, str]] = None,
-    mode: str = "overwrite",
+    mode: Literal["overwrite", "append"] = "overwrite",
     catalog_versioning: bool = False,
     schema_evolution: bool = False,
     sep: str = ",",
     skip_header_line_count: Optional[int] = None,
     serde_library: Optional[str] = None,
     serde_parameters: Optional[Dict[str, str]] = None,
     transaction_id: Optional[str] = None,
@@ -848,15 +884,15 @@
     description : str, optional
         Table description
     parameters : Dict[str, str], optional
         Key/value pairs to tag the table.
     columns_comments: Dict[str, str], optional
         Columns names and the related comments (e.g. {'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}).
     mode : str
-        'overwrite' to recreate any possible axisting table or 'append' to keep any possible axisting table.
+        'overwrite' to recreate any possible existing table or 'append' to keep any possible existing table.
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
         https://aws-sdk-pandas.readthedocs.io/en/2.11.0/tutorials/014%20-%20Schema%20Evolution.html
@@ -870,15 +906,15 @@
         If no library is provided the default is `org.apache.hadoop.hive.serde2.lazy.LazySimpleSerDe`.
     serde_parameters : Optional[str]
         Dictionary of initialization parameters for the SerDe.
         The default is `{"field.delim": sep, "escape.delim": "\\"}`.
     transaction_id: str, optional
         The ID of the transaction (i.e. used with GOVERNED tables).
     athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
-        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        Parameters of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
         AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaPartitionProjectionSettings or as a regular Python dict.
 
         Following projection parameters are supported:
 
         .. list-table:: Projection Parameters
            :header-rows: 1
@@ -993,15 +1029,15 @@
     table_type: Optional[str] = None,
     partitions_types: Optional[Dict[str, str]] = None,
     bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     compression: Optional[str] = None,
     description: Optional[str] = None,
     parameters: Optional[Dict[str, str]] = None,
     columns_comments: Optional[Dict[str, str]] = None,
-    mode: str = "overwrite",
+    mode: Literal["overwrite", "append"] = "overwrite",
     catalog_versioning: bool = False,
     schema_evolution: bool = False,
     serde_library: Optional[str] = None,
     serde_parameters: Optional[Dict[str, str]] = None,
     transaction_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
@@ -1034,15 +1070,15 @@
     description : str, optional
         Table description
     parameters : Dict[str, str], optional
         Key/value pairs to tag the table.
     columns_comments: Dict[str, str], optional
         Columns names and the related comments (e.g. {'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}).
     mode : str
-        'overwrite' to recreate any possible axisting table or 'append' to keep any possible axisting table.
+        'overwrite' to recreate any possible existing table or 'append' to keep any possible existing table.
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
         https://aws-sdk-pandas.readthedocs.io/en/2.11.0/tutorials/014%20-%20Schema%20Evolution.html
@@ -1052,15 +1088,15 @@
         If no library is provided the default is `org.openx.data.jsonserde.JsonSerDe`.
     serde_parameters : Optional[str]
         Dictionary of initialization parameters for the SerDe.
         The default is `{"field.delim": sep, "escape.delim": "\\"}`.
     transaction_id: str, optional
         The ID of the transaction (i.e. used with GOVERNED tables).
     athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
-        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        Parameters of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
         AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaPartitionProjectionSettings or as a regular Python dict.
 
         Following projection parameters are supported:
 
         .. list-table:: Projection Parameters
            :header-rows: 1
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/catalog/_definitions.py` & `awswrangler-3.1.0/awswrangler/catalog/_definitions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/catalog/_delete.py` & `awswrangler-3.1.0/awswrangler/catalog/_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         client_glue.delete_table(
             **_catalog_id(
                 **_transaction_id(
                     transaction_id=transaction_id, DatabaseName=database, Name=table, catalog_id=catalog_id
                 )
             )
         )
+        _logger.debug("Deleted catalog table: %s", table)
         return True
     except client_glue.exceptions.EntityNotFoundException:
         return False
 
 
 @apply_configs
 def delete_partitions(
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/catalog/_get.py` & `awswrangler-3.1.0/awswrangler/catalog/_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import base64
 import itertools
 import logging
 from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Union, cast
 
 import boto3
 import botocore.exceptions
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler import _utils, exceptions
 from awswrangler._config import apply_configs
 from awswrangler.catalog._utils import _catalog_id, _extract_dtypes_from_table_details, _transaction_id
 
 if TYPE_CHECKING:
     from mypy_boto3_glue.type_defs import GetPartitionsResponseTypeDef
 
@@ -212,15 +212,15 @@
         If none is provided, the AWS account ID is used by default.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     pandas.DataFrame
-        Pandas DataFrame filled by formatted infos.
+        Pandas DataFrame filled by formatted table information.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> df_dbs = wr.catalog.databases()
 
     """
@@ -352,15 +352,15 @@
         Select by a specific suffix on table name
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     pandas.DataFrame
-        Pandas Dataframe filled by formatted infos.
+        Pandas DataFrame filled by formatted table information.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> df_tables = wr.catalog.tables()
 
     """
@@ -485,15 +485,15 @@
         If none is provided, the AWS account ID is used by default.
     boto3_session: boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     pandas.DataFrame
-        Pandas DataFrame filled by formatted infos.
+        Pandas DataFrame filled by formatted table information.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> df_table = wr.catalog.table(database='default', table='my_table')
 
     """
@@ -1054,15 +1054,15 @@
     return versions
 
 
 @apply_configs
 def get_table_number_of_versions(
     database: str, table: str, catalog_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None
 ) -> int:
-    """Get tatal number of versions.
+    """Get total number of versions.
 
     Parameters
     ----------
     database : str
         Database name.
     table : str
         Table name.
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/catalog/_utils.py` & `awswrangler-3.1.0/awswrangler/catalog/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import logging
 import re
 import unicodedata
 import warnings
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 import boto3
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._config import apply_configs
 
 if TYPE_CHECKING:
     from mypy_boto3_glue.type_defs import GetTableResponseTypeDef
 
 _logger: logging.Logger = logging.getLogger(__name__)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/chime.py` & `awswrangler-3.1.0/awswrangler/chime.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/cloudwatch.py` & `awswrangler-3.1.0/awswrangler/cloudwatch.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import datetime
 import logging
 import time
 from typing import Any, Dict, List, Optional, cast
 
 import boto3
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler import _utils, exceptions
 from awswrangler._config import apply_configs
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 _QUERY_WAIT_POLLING_DELAY: float = 1.0  # SECONDS
 
@@ -25,16 +25,16 @@
     if start_timestamp >= end_timestamp:
         raise exceptions.InvalidArgumentCombination("`start_time` must be inferior to `end_time`.")
 
 
 def start_query(
     query: str,
     log_group_names: List[str],
-    start_time: datetime.datetime = datetime.datetime(year=1970, month=1, day=1, tzinfo=datetime.timezone.utc),
-    end_time: datetime.datetime = datetime.datetime.utcnow(),
+    start_time: Optional[datetime.datetime] = None,
+    end_time: Optional[datetime.datetime] = None,
     limit: Optional[int] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> str:
     """Run a query against AWS CloudWatchLogs Insights.
 
     https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_QuerySyntax.html
 
@@ -64,18 +64,25 @@
     >>> query_id = wr.cloudwatch.start_query(
     ...     log_group_names=["loggroup"],
     ...     query="fields @timestamp, @message | sort @timestamp desc | limit 5",
     ... )
 
     """
     _logger.debug("log_group_names: %s", log_group_names)
+
+    start_time = (
+        start_time if start_time else datetime.datetime(year=1970, month=1, day=1, tzinfo=datetime.timezone.utc)
+    )
+    end_time = end_time if end_time else datetime.datetime.utcnow()
+
     start_timestamp: int = int(1000 * start_time.timestamp())
     end_timestamp: int = int(1000 * end_time.timestamp())
     _logger.debug("start_timestamp: %s", start_timestamp)
     _logger.debug("end_timestamp: %s", end_timestamp)
+
     _validate_args(start_timestamp=start_timestamp, end_timestamp=end_timestamp)
     args: Dict[str, Any] = {
         "logGroupNames": log_group_names,
         "startTime": start_timestamp,
         "endTime": end_timestamp,
         "queryString": query,
     }
@@ -135,16 +142,16 @@
         raise exceptions.QueryCancelled(f"query ID: {query_id}")
     return cast(Dict[str, Any], response)
 
 
 def run_query(
     query: str,
     log_group_names: List[str],
-    start_time: datetime.datetime = datetime.datetime(year=1970, month=1, day=1, tzinfo=datetime.timezone.utc),
-    end_time: datetime.datetime = datetime.datetime.utcnow(),
+    start_time: Optional[datetime.datetime] = None,
+    end_time: Optional[datetime.datetime] = None,
     limit: Optional[int] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> List[List[Dict[str, str]]]:
     """Run a query against AWS CloudWatchLogs Insights and wait the results.
 
     https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_QuerySyntax.html
 
@@ -188,16 +195,16 @@
     response: Dict[str, Any] = wait_query(query_id=query_id, boto3_session=boto3_session)
     return cast(List[List[Dict[str, str]]], response["results"])
 
 
 def read_logs(
     query: str,
     log_group_names: List[str],
-    start_time: datetime.datetime = datetime.datetime(year=1970, month=1, day=1, tzinfo=datetime.timezone.utc),
-    end_time: datetime.datetime = datetime.datetime.utcnow(),
+    start_time: Optional[datetime.datetime] = None,
+    end_time: Optional[datetime.datetime] = None,
     limit: Optional[int] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> pd.DataFrame:
     """Run a query against AWS CloudWatchLogs Insights and convert the results to Pandas DataFrame.
 
     https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_QuerySyntax.html
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/data_api/_connector.py` & `awswrangler-3.1.0/awswrangler/data_api/_connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Data API Connector base class."""
 import logging
 from typing import Any, Dict, Optional
 
-import pandas as pd
+import awswrangler.pandas as pd
 
 
 class DataApiConnector:
     """Base class for Data API (RDS, Redshift, etc.) connectors."""
 
     def __init__(self, client: Any, logger: logging.Logger):
         self.client = client
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/data_api/rds.py` & `awswrangler-3.1.0/awswrangler/data_api/rds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """RDS Data API Connector."""
 import logging
 import time
 import uuid
 from typing import Any, Dict, List, Optional
 
 import boto3
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler import _utils
 from awswrangler.data_api import _connector
 
 
 class RdsDataApi(_connector.DataApiConnector):
     """Provides access to the RDS Data API.
 
@@ -138,23 +138,23 @@
     -------
     A RdsDataApi connection instance that can be used with `wr.rds.data_api.read_sql_query`.
     """
     return RdsDataApi(resource_arn, database, secret_arn=secret_arn, boto3_session=boto3_session, **kwargs)
 
 
 def read_sql_query(sql: str, con: RdsDataApi, database: Optional[str] = None) -> pd.DataFrame:
-    """Run an SQL query on an RdsDataApi connection and return the result as a dataframe.
+    """Run an SQL query on an RdsDataApi connection and return the result as a DataFrame.
 
     Parameters
     ----------
     sql: str
         SQL query to run.
     con: RdsDataApi
         A RdsDataApi connection instance
     database: str
         Database to run query on - defaults to the database specified by `con`.
 
     Returns
     -------
-    A Pandas dataframe containing the query results.
+    A Pandas DataFrame containing the query results.
     """
     return con.execute(sql, database=database)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/data_api/redshift.py` & `awswrangler-3.1.0/awswrangler/data_api/redshift.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Redshift Data API Connector."""
 import logging
 import time
 from typing import Any, Dict, List, Optional
 
 import boto3
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler import _utils
 from awswrangler.data_api import _connector
 
 
 class RedshiftDataApi(_connector.DataApiConnector):
     """Provides access to a Redshift cluster via the Data API.
 
@@ -234,23 +234,23 @@
         db_user=db_user,
         boto3_session=boto3_session,
         **kwargs,
     )
 
 
 def read_sql_query(sql: str, con: RedshiftDataApi, database: Optional[str] = None) -> pd.DataFrame:
-    """Run an SQL query on a RedshiftDataApi connection and return the result as a dataframe.
+    """Run an SQL query on a RedshiftDataApi connection and return the result as a DataFrame.
 
     Parameters
     ----------
     sql: str
         SQL query to run.
     con: RedshiftDataApi
         A RedshiftDataApi connection instance
     database: str
         Database to run query on - defaults to the database specified by `con`.
 
     Returns
     -------
-    A Pandas dataframe containing the query results.
+    A Pandas DataFrame containing the query results.
     """
     return con.execute(sql, database=database)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/data_quality/_create.py` & `awswrangler-3.1.0/awswrangler/data_quality/_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """AWS Glue Data Quality Create module."""
 
 import logging
 import pprint
 import uuid
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Dict, List, Literal, Optional, Union, cast
 
 import boto3
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler import _utils, exceptions
 from awswrangler._config import apply_configs
 from awswrangler.data_quality._get import get_ruleset
 from awswrangler.data_quality._utils import (
     _create_datasource,
     _get_data_quality_results,
     _rules_to_df,
@@ -117,29 +117,26 @@
     except client_glue.exceptions.AlreadyExistsException as not_found:
         raise exceptions.AlreadyExists(f"Ruleset {name} already exists.") from not_found
 
 
 @apply_configs
 def update_ruleset(
     name: str,
-    updated_name: Optional[str] = None,
-    mode: str = "overwrite",
+    mode: Literal["overwrite", "upsert"] = "overwrite",
     df_rules: Optional[pd.DataFrame] = None,
     dqdl_rules: Optional[str] = None,
     description: str = "",
     boto3_session: Optional[boto3.Session] = None,
 ) -> None:
     """Update Data Quality ruleset.
 
     Parameters
     ----------
     name : str
         Ruleset name.
-    updated_name : str
-        New ruleset name if renaming an existing ruleset.
     mode : str
         overwrite (default) or upsert.
     df_rules : str, optional
         Data frame with `rule_type`, `parameter`, and `expression` columns.
     dqdl_rules : str, optional
         Data Quality Definition Language definition.
     description : str
@@ -148,15 +145,14 @@
         Boto3 Session. If none, the default boto3 session is used.
 
     Examples
     --------
     Overwrite rules in the existing ruleset.
     >>> wr.data_quality.update_ruleset(
     >>>     name="ruleset",
-    >>>     new_name="my_ruleset",
     >>>     dqdl_rules="Rules = [ RowCount between 1 and 3 ]",
     >>>)
 
     Update or insert rules in the existing ruleset.
     >>> wr.data_quality.update_ruleset(
     >>>     name="ruleset",
     >>>     mode="insert",
@@ -179,16 +175,14 @@
         dqdl_rules = _create_dqdl(df_rules) if df_rules is not None else dqdl_rules
 
     args = {
         "Name": name,
         "Description": description,
         "Ruleset": dqdl_rules,
     }
-    if updated_name:
-        args["UpdatedName"] = updated_name
 
     client_glue = _utils.client(service_name="glue", session=boto3_session)
     try:
         client_glue.update_data_quality_ruleset(**args)  # type: ignore[arg-type]
     except client_glue.exceptions.EntityNotFoundException as not_found:
         raise exceptions.ResourceDoesNotExist(f"Ruleset {name} does not exist.") from not_found
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/data_quality/_get.py` & `awswrangler-3.1.0/awswrangler/data_quality/_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """AWS Glue Data Quality Get Module."""
 
 from typing import List, Optional, Union, cast
 
 import boto3
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler.data_quality._utils import _get_ruleset, _rules_to_df
 
 
 def get_ruleset(
     name: Union[str, List[str]],
     boto3_session: Optional[boto3.Session] = None,
 ) -> pd.DataFrame:
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/data_quality/_utils.py` & `awswrangler-3.1.0/awswrangler/data_quality/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import pprint
 import re
 import time
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 import boto3
 import botocore.exceptions
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler import _utils, exceptions
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 _RULESET_EVALUATION_FINAL_STATUSES: List[str] = ["STOPPED", "SUCCEEDED", "FAILED", "TIMEOUT"]
 _RULESET_EVALUATION_WAIT_POLLING_DELAY: float = 1.0  # SECONDS
 
@@ -173,10 +173,10 @@
     results = client_glue.batch_get_data_quality_result(
         ResultIds=result_ids,
     )["Results"]
     rule_results: List[Dict[str, Any]] = []
     for result in results:
         rules = result["RuleResults"]
         for rule in rules:
-            rule["ResultId"] = result["ResultId"]  # type: ignore[typeddict-item]
+            rule["ResultId"] = result["ResultId"]  # type: ignore[typeddict-unknown-key]
         rule_results.extend(cast(List[Dict[str, Any]], rules))
     return pd.json_normalize(rule_results)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/_core.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/_core.pyi` & `awswrangler-3.1.0/awswrangler/distributed/ray/_core.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/_register.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/_register.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 """Ray and Modin registered methods (PRIVATE)."""
 # pylint: disable=import-outside-toplevel
 from awswrangler._data_types import pyarrow_types_from_pandas
 from awswrangler._distributed import MemoryFormatEnum, engine, memory_format
-from awswrangler._utils import copy_df_shallow, is_pandas_frame, split_pandas_frame, table_refs_to_df
+from awswrangler._executor import _get_executor
+from awswrangler._utils import (
+    copy_df_shallow,
+    ensure_worker_or_thread_count,
+    is_pandas_frame,
+    split_pandas_frame,
+    table_refs_to_df,
+)
 from awswrangler.distributed.ray import ray_remote
+from awswrangler.distributed.ray._executor import _get_ray_executor
+from awswrangler.distributed.ray._utils import ensure_worker_count
 from awswrangler.distributed.ray.s3._list import _list_objects_s3fs
 from awswrangler.distributed.ray.s3._read_parquet import _read_parquet_metadata_file_distributed
 from awswrangler.dynamodb._read import _read_scan
+from awswrangler.dynamodb._write import _put_df, _put_items
 from awswrangler.lakeformation._read import _get_work_unit_results
 from awswrangler.s3._copy import _copy_objects
 from awswrangler.s3._delete import _delete_objects
 from awswrangler.s3._describe import _describe_object
 from awswrangler.s3._list import _list_objects_paginate
 from awswrangler.s3._read_parquet import _read_parquet, _read_parquet_metadata_file
 from awswrangler.s3._read_text import _read_text
 from awswrangler.s3._select import _select_object_content, _select_query
 from awswrangler.s3._wait import _wait_object_batch
 from awswrangler.s3._write_dataset import _to_buckets, _to_partitions
 from awswrangler.s3._write_parquet import _to_parquet
 from awswrangler.s3._write_text import _to_text
-from awswrangler.timestream import _write_batch, _write_df
+from awswrangler.timestream._write import _write_batch, _write_df
 
 
 def register_ray() -> None:
     """Register dispatched Ray and Modin (on Ray) methods."""
     for func in [
         _get_work_unit_results,
         _copy_objects,
@@ -34,22 +44,26 @@
         _select_object_content,
         _wait_object_batch,
     ]:
         # Schedule for maximum concurrency
         engine.register_func(func, ray_remote(scheduling_strategy="SPREAD")(func))
 
     for func in [
+        _put_df,
+        _put_items,
         _write_batch,
         _write_df,
     ]:
         engine.register_func(func, ray_remote()(func))
 
     for o_f, d_f in {
+        _get_executor: _get_ray_executor,
         _list_objects_paginate: _list_objects_s3fs,
         _read_parquet_metadata_file: ray_remote()(_read_parquet_metadata_file_distributed),
+        ensure_worker_or_thread_count: ensure_worker_count,
     }.items():
         engine.register_func(o_f, d_f)  # type: ignore[arg-type]
 
     if memory_format.get() == MemoryFormatEnum.MODIN:
         from awswrangler.distributed.ray.modin._data_types import pyarrow_types_from_pandas_distributed
         from awswrangler.distributed.ray.modin._utils import (
             _arrow_refs_to_df,
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/__init__.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_json_datasource.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,16 @@
 ) -> List[ParquetFileFragment]:
     return [p.deserialize() for p in serialized_pieces]
 
 
 # This retry helps when the upstream datasource is not able to handle
 # overloaded read request or failed with some retriable failures.
 # For example when reading data from HA hdfs service, hdfs might
-# lose connection for some unknown reason expecially when
-# simutaneously running many hyper parameter tuning jobs
+# lose connection for some unknown reason especially when
+# simultaneously running many hyper parameter tuning jobs
 # with ray.data parallelism setting at high value like the default 200
 # Such connection failure can be restored with some waiting and retry.
 def _deserialize_pieces_with_retry(
     serialized_pieces: List[_SerializedPiece],
 ) -> List[ParquetFileFragment]:
     min_interval: float = 0
     final_exception: Optional[Exception] = None
@@ -251,16 +251,15 @@
                 total_size += row_group_metadata.total_byte_size
         return total_size * self._encoding_ratio  # type: ignore[return-value]
 
     def get_read_tasks(self, parallelism: int) -> List[ReadTask]:
         """Override the base class FileBasedDatasource.get_read_tasks().
 
         Required in order to leverage pyarrow's ParquetDataset abstraction,
-        which simplifies partitioning logic. We still use
-        FileBasedDatasource's write side (do_write), however.
+        which simplifies partitioning logic.
         """
         read_tasks = []
         block_udf, reader_args, columns, schema = (
             self._block_udf,
             self._reader_args,
             self._columns,
             self._schema,
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Ray PandasFileBasedDatasource Module."""
 import logging
-from typing import Any, Callable, Dict, List, Optional
+from dataclasses import dataclass
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 import pandas as pd
 import pyarrow
+import ray
+from ray.data._internal.delegating_block_builder import DelegatingBlockBuilder
 from ray.data.block import Block, BlockAccessor, BlockMetadata
 from ray.data.datasource.datasource import WriteResult
 from ray.data.datasource.file_based_datasource import (
     BlockWritePathProvider,
     DefaultBlockWritePathProvider,
     FileBasedDatasource,
 )
 from ray.types import ObjectRef
 
-from awswrangler.distributed.ray import ray_remote
+from awswrangler.distributed.ray import ray_get, ray_remote
 from awswrangler.s3._fs import open_s3_object
 from awswrangler.s3._write import _COMPRESSION_2_EXT
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 class UserProvidedKeyBlockWritePathProvider(BlockWritePathProvider):
@@ -28,35 +31,44 @@
 
     def _get_write_path_for_block(
         self,
         base_path: str,
         *,
         filesystem: Optional["pyarrow.fs.FileSystem"] = None,
         dataset_uuid: Optional[str] = None,
-        block: Optional[ObjectRef[Block[Any]]] = None,
+        block: Optional[Block[Any]] = None,
         block_index: Optional[int] = None,
         file_format: Optional[str] = None,
     ) -> str:
         return base_path
 
 
+@dataclass
+class TaskContext:
+    """Describes the information of a task running block transform."""
+
+    # The index of task. Each task has a unique task index within the same
+    # operator.
+    task_idx: int
+
+
 class PandasFileBasedDatasource(FileBasedDatasource):  # pylint: disable=abstract-method
     """Pandas file based datasource, for reading and writing Pandas blocks."""
 
     _FILE_EXTENSION: str
 
     def __init__(self) -> None:
         super().__init__()
 
         self._write_paths: List[str] = []
 
     def _read_file(self, f: pyarrow.NativeFile, path: str, **reader_args: Any) -> pd.DataFrame:
         raise NotImplementedError()
 
-    def do_write(  # type: ignore[override]  # pylint: disable=arguments-differ
+    def do_write(  # pylint: disable=arguments-differ
         self,
         blocks: List[ObjectRef[pd.DataFrame]],
         metadata: List[BlockMetadata],
         path: str,
         dataset_uuid: str,
         filesystem: Optional[pyarrow.fs.FileSystem] = None,
         try_create_dir: bool = True,
@@ -67,15 +79,21 @@
         ray_remote_args: Optional[Dict[str, Any]] = None,
         s3_additional_kwargs: Optional[Dict[str, str]] = None,
         pandas_kwargs: Optional[Dict[str, Any]] = None,
         compression: Optional[str] = None,
         mode: str = "wb",
         **write_args: Any,
     ) -> List[ObjectRef[WriteResult]]:
-        """Create and return write tasks for a file-based datasource."""
+        """Create and return write tasks for a file-based datasource.
+
+        Note: In Ray 2.4+ write semantics has changed. datasource.do_write() was deprecated in favour of
+        datasource.write() that represents a single write task and enables it to be captured by execution
+        plan allowing query optimisation ("fuse" with other operations). The change is not backward-compatible
+        with earlier versions still attempting to call do_write().
+        """
         _write_block_to_file = self._write_block
 
         if ray_remote_args is None:
             ray_remote_args = {}
 
         if pandas_kwargs is None:
             pandas_kwargs = {}
@@ -119,14 +137,78 @@
                 file_format=file_suffix,
             )
             write_task = write_block_fn(write_path, block)
             write_tasks.append(write_task)
 
         return write_tasks
 
+    def write(  # type: ignore[override]
+        self,
+        blocks: Iterable[Union[Block[pd.DataFrame], ObjectRef[pd.DataFrame]]],
+        ctx: TaskContext,
+        path: str,
+        dataset_uuid: str,
+        filesystem: Optional[pyarrow.fs.FileSystem] = None,
+        block_path_provider: BlockWritePathProvider = DefaultBlockWritePathProvider(),
+        _block_udf: Optional[Callable[[pd.DataFrame], pd.DataFrame]] = None,
+        s3_additional_kwargs: Optional[Dict[str, str]] = None,
+        pandas_kwargs: Optional[Dict[str, Any]] = None,
+        compression: Optional[str] = None,
+        mode: str = "wb",
+        **write_args: Any,
+    ) -> WriteResult:
+        """Write blocks for a file-based datasource."""
+        _write_block_to_file = self._write_block
+
+        if pandas_kwargs is None:
+            pandas_kwargs = {}
+
+        if not compression:
+            compression = pandas_kwargs.get("compression")
+
+        def write_block(write_path: str, block: pd.DataFrame) -> str:
+            if _block_udf is not None:
+                block = _block_udf(block)
+
+            with open_s3_object(
+                path=write_path,
+                mode=mode,
+                use_threads=False,
+                s3_additional_kwargs=s3_additional_kwargs,
+                encoding=write_args.get("encoding"),
+                newline=write_args.get("newline"),
+            ) as f:
+                _write_block_to_file(
+                    f,
+                    BlockAccessor.for_block(block),
+                    pandas_kwargs=pandas_kwargs,
+                    compression=compression,
+                    **write_args,
+                )
+                return write_path
+
+        file_suffix = self._get_file_suffix(self._FILE_EXTENSION, compression)
+
+        builder = DelegatingBlockBuilder()  # type: ignore[no-untyped-call,var-annotated]
+        for block in blocks:
+            # Dereference the block if ObjectRef is passed
+            builder.add_block(ray_get(block) if isinstance(block, ray.ObjectRef) else block)  # type: ignore[arg-type]
+        block = builder.build()
+
+        write_path = block_path_provider(
+            path,
+            filesystem=filesystem,
+            dataset_uuid=dataset_uuid,
+            block=block,
+            block_index=ctx.task_idx,
+            file_format=file_suffix,
+        )
+
+        return write_block(write_path, block)
+
     def _get_file_suffix(self, file_format: str, compression: Optional[str]) -> str:
         return f"{file_format}{_COMPRESSION_2_EXT.get(compression)}"
 
     def _write_block(
         self,
         f: "pyarrow.NativeFile",
         block: BlockAccessor[Any],
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/pandas_text_datasource.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_core.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/modin/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     ) -> Any:
         # Validate partitions and repartition Modin data frame along row (axis=0) axis
         # to avoid a situation where columns are split along multiple blocks
         if isinstance(df, ModinDataFrame):
             if validate_partitions and not _validate_partition_shape(df):
                 _logger.warning(
                     "Partitions of this data frame are detected to be split along column axis. "
-                    "The dataframe will be automatically repartitioned along row axis to ensure "
+                    "The DataFrame will be automatically repartitioned along row axis to ensure "
                     "each partition can be processed independently."
                 )
                 axis = 0
             if axis is not None:
                 df = from_partitions(unwrap_partitions(df, axis=axis), axis=axis, row_lengths=row_lengths)
         return function(df, *args, **kwargs)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_data_types.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/modin/_data_types.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_utils.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/modin/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return from_pandas(df)  # type: ignore[no-any-return]
     raise ValueError(f"Unknown DataFrame type: {type(df)}")
 
 
 def _to_modin(
     dataset: Union[ray.data.Dataset[Any], ray.data.Dataset[pd.DataFrame]],
     to_pandas_kwargs: Optional[Dict[str, Any]] = None,
-    ignore_index: bool = True,
+    ignore_index: Optional[bool] = True,
 ) -> modin_pd.DataFrame:
     index = modin_pd.RangeIndex(start=0, stop=dataset.count()) if ignore_index else None
     _to_pandas_kwargs = {} if to_pandas_kwargs is None else to_pandas_kwargs
 
     return from_partitions(
         partitions=[
             _block_to_df(block=block, to_pandas_kwargs=_to_pandas_kwargs) for block in dataset.get_internal_block_refs()
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_read_parquet.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,8 +48,12 @@
         use_threads=use_threads,
         paths=paths,
         schema=schema,
         columns=columns,
         path_root=path_root,
         dataset_kwargs=dataset_kwargs,
     )
-    return _to_modin(dataset=dataset, to_pandas_kwargs=arrow_kwargs, ignore_index=bool(path_root))
+    return _to_modin(
+        dataset=dataset,
+        to_pandas_kwargs=arrow_kwargs,
+        ignore_index=arrow_kwargs.get("ignore_metadata"),
+    )
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_read_text.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_read_text.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_dataset.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Modin on Ray S3 write dataset module (PRIVATE)."""
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
 import boto3
 import modin.pandas as pd
 import numpy as np
-from pandas import DataFrame as PandasDataFrame
 
 from awswrangler import _utils, typing
 from awswrangler._distributed import engine
 from awswrangler.distributed.ray import ray_get, ray_remote
 from awswrangler.distributed.ray.modin import modin_repartition
 from awswrangler.distributed.ray.modin._utils import _ray_dataset_from_df
 from awswrangler.s3._write_concurrent import _WriteProxy
@@ -135,16 +134,16 @@
 ) -> Tuple[List[str], Dict[str, List[str]]]:
     paths: List[str]
     partitions_values: Dict[str, List[str]]
 
     if not bucketing_info:
         # If only partitioning (without bucketing), avoid expensive modin groupby
         # by partitioning and writing each block as an ordinary Pandas DataFrame
-        _to_partitions_func = engine.dispatch_func(_to_partitions, PandasDataFrame)
-        func = engine.dispatch_func(func, PandasDataFrame)
+        _to_partitions_func = engine.dispatch_func(_to_partitions, "python")
+        func = engine.dispatch_func(func, "python")
 
         @ray_remote()
         def write_partitions(df: pd.DataFrame, block_index: int) -> Tuple[List[str], Dict[str, List[str]]]:
             paths, partitions_values = _to_partitions_func(
                 # Passing a copy of the data frame because data in ray object store is immutable
                 # and that leads to "ValueError: buffer source array is read-only" during df.groupby()
                 df.copy(),
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_parquet.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_text.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     path: Optional[str] = None,
     path_root: Optional[str] = None,
     filename_prefix: Optional[str] = None,
     bucketing: bool = False,
     **pandas_kwargs: Any,
 ) -> List[str]:
     if df.empty is True:
-        raise exceptions.EmptyDataFrame("DataFrame cannot be empty.")
+        _logger.warning("Empty DataFrame will be written.")
 
     if bucketing:
         # Add bucket id to the prefix
         prefix = f"{filename_prefix}_bucket-{df.name:05d}"
         extension = f"{file_format}{_COMPRESSION_2_EXT.get(pandas_kwargs.get('compression'))}"
 
         file_path = f"{path_root}{prefix}.{extension}"
@@ -127,15 +127,15 @@
         write_options = None
         can_use_arrow = False
 
     datasource = _datasource_for_format(file_format, can_use_arrow)
 
     mode, encoding, newline = _get_write_details(path=file_path, pandas_kwargs=pandas_kwargs)
     ds.write_datasource(
-        datasource=datasource,
+        datasource,
         path=file_path,
         block_path_provider=(
             UserProvidedKeyBlockWritePathProvider()
             if path and not path.endswith("/")
             else DefaultBlockWritePathProvider()
         ),
         file_path=file_path,
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/s3/_list.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/s3/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/distributed/ray/s3/_read_parquet.py` & `awswrangler-3.1.0/awswrangler/distributed/ray/s3/_read_parquet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 import pyarrow as pa
 from pyarrow.fs import _resolve_filesystem_and_path
 
+from awswrangler import _utils
 from awswrangler.s3._read_parquet import _pyarrow_parquet_file_wrapper
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
 
 
+@_utils.retry(ex=OSError)
 def _read_parquet_metadata_file_distributed(
     s3_client: Optional["S3Client"],
     path: str,
     s3_additional_kwargs: Optional[Dict[str, str]],
     use_threads: Union[bool, int],
     version_id: Optional[str] = None,
     coerce_int96_timestamp_unit: Optional[str] = None,
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/dynamodb/_delete.py` & `awswrangler-3.1.0/awswrangler/dynamodb/_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     >>> import awswrangler as wr
     >>> wr.dynamodb.delete_items(
     ...     items=[{'key': 1}, {'key': 2, 'value': 'Hello'}],
     ...     table_name='table'
     ... )
     """
-    _logger.debug("Deleting items from DynamoDB table")
+    _logger.debug("Deleting items from DynamoDB table %s", table_name)
 
     dynamodb_table = get_table(table_name=table_name, boto3_session=boto3_session)
     _validate_items(items=items, dynamodb_table=dynamodb_table)
     table_keys = [schema["AttributeName"] for schema in dynamodb_table.key_schema]
     with dynamodb_table.batch_writer() as writer:
         for item in items:
             writer.delete_item(Key={key: item[key] for key in table_keys})
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/dynamodb/_read.py` & `awswrangler-3.1.0/awswrangler/dynamodb/_read.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,79 +6,48 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterator,
     List,
-    Literal,
     Optional,
     Sequence,
     TypeVar,
     Union,
     cast,
-    overload,
 )
 
 import boto3
-import pandas as pd
 import pyarrow as pa
 from boto3.dynamodb.conditions import ConditionBase
 from boto3.dynamodb.types import Binary
 from botocore.exceptions import ClientError
 
+import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor
+from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.distributed.ray import ray_get
 from awswrangler.dynamodb._utils import _serialize_kwargs, execute_statement, get_table
 
 if TYPE_CHECKING:
     from mypy_boto3_dynamodb.client import DynamoDBClient
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
+_ItemsListType = List[Dict[str, Any]]
+
+
 def _read_chunked(iterator: Iterator[Dict[str, Any]]) -> Iterator[pd.DataFrame]:
     for item in iterator:
         yield pd.DataFrame(item)
 
 
-@overload
-def read_partiql_query(
-    query: str,
-    parameters: Optional[List[Any]] = ...,
-    chunked: Literal[False] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-) -> pd.DataFrame:
-    ...
-
-
-@overload
-def read_partiql_query(
-    query: str,
-    *,
-    parameters: Optional[List[Any]] = ...,
-    chunked: Literal[True],
-    boto3_session: Optional[boto3.Session] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_partiql_query(
-    query: str,
-    *,
-    parameters: Optional[List[Any]] = ...,
-    chunked: bool,
-    boto3_session: Optional[boto3.Session] = ...,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
 def read_partiql_query(
     query: str,
     parameters: Optional[List[Any]] = None,
     chunked: bool = False,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Read data from a DynamoDB table via a PartiQL query.
@@ -121,45 +90,46 @@
     )
     if chunked:
         return _read_chunked(iterator=iterator)
     return pd.DataFrame([item for sublist in iterator for item in sublist])
 
 
 def _get_invalid_kwarg(msg: str) -> Optional[str]:
-    """Detect which kwarg contains reserved keywords based on given error message.
+    """Detect which keyword argument contains reserved keywords based on given error message.
 
     Parameters
     ----------
     msg : str
         Botocore client error message.
 
     Returns
     -------
     str, optional
-        Detected invalid kwarg if any, None otherwise.
+        Detected invalid keyword argument if any, None otherwise.
     """
     for kwarg in ("ProjectionExpression", "KeyConditionExpression", "FilterExpression"):
         if msg.startswith(f"Invalid {kwarg}: Attribute name is a reserved keyword; reserved keyword: "):
             return kwarg
     return None
 
 
 # SEE: https://stackoverflow.com/a/72295070
-CustomCallable = TypeVar("CustomCallable", bound=Callable[[Any], List[Dict[str, Any]]])
+# CustomCallable = TypeVar("CustomCallable", bound=Callable[[Any], Union[_ItemsListType, Iterator[_ItemsListType]]])
+CustomCallable = TypeVar("CustomCallable", bound=Callable[..., Any])
 
 
 def _handle_reserved_keyword_error(func: CustomCallable) -> CustomCallable:
     """Handle automatic replacement of DynamoDB reserved keywords.
 
     For reserved keywords reference:
     https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/ReservedWords.html.
     """
 
     @wraps(func)
-    def wrapper(*args: Any, **kwargs: Any) -> List[Dict[str, Any]]:
+    def wrapper(*args: Any, **kwargs: Any) -> Any:
         try:
             return func(*args, **kwargs)
         except ClientError as e:
             error_code, error_message = (e.response["Error"]["Code"], e.response["Error"]["Message"])
             # Check caught error to verify its message
             kwarg = _get_invalid_kwarg(error_message)
             if (error_code == "ValidationException") and kwarg:
@@ -177,21 +147,18 @@
             raise e
 
     # SEE: https://github.com/python/mypy/issues/3157#issue-221120895
     return cast(CustomCallable, wrapper)
 
 
 def _convert_items(
-    items: List[Dict[str, Any]],
-    use_scan: bool,
+    items: _ItemsListType,
     as_dataframe: bool,
     arrow_kwargs: Dict[str, Any],
-) -> Union[pd.DataFrame, List[Dict[str, Any]]]:
-    if use_scan:
-        return _utils.table_refs_to_df(items, arrow_kwargs) if as_dataframe else list(itertools.chain(*ray_get(items)))
+) -> Union[pd.DataFrame, _ItemsListType]:
     return (
         _utils.table_refs_to_df(
             [
                 _utils.list_to_arrow_table(
                     # Convert DynamoDB "Binary" type to native Python data type
                     mapping=[
                         {k: v.value if isinstance(v, Binary) else v for k, v in d.items()}  # type: ignore[attr-defined]
@@ -202,207 +169,237 @@
             arrow_kwargs,
         )
         if as_dataframe
         else items
     )
 
 
-@engine.dispatch_on_engine
-@_utils.retry(
-    ex=ClientError,
-    ex_code="ProvisionedThroughputExceededException",
-)
-def _read_scan(
+def _convert_items_chunked(
+    items_iterator: Iterator[_ItemsListType],
+    as_dataframe: bool,
+    arrow_kwargs: Dict[str, Any],
+) -> Union[Iterator[pd.DataFrame], Iterator[_ItemsListType]]:
+    for items in items_iterator:
+        yield _convert_items(items, as_dataframe, arrow_kwargs)
+
+
+def _read_scan_chunked(
     dynamodb_client: Optional["DynamoDBClient"],
     as_dataframe: bool,
     kwargs: Dict[str, Any],
-    segment: int,
-) -> Union[pa.Table, List[Dict[str, Any]]]:
+    segment: Optional[int] = None,
+) -> Union[Iterator[pa.Table], Iterator[_ItemsListType]]:
     # SEE: https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Scan.html#Scan.ParallelScan
     client_dynamodb = dynamodb_client if dynamodb_client else _utils.client(service_name="dynamodb")
 
     deserializer = boto3.dynamodb.types.TypeDeserializer()
     next_token = "init_token"  # Dummy token
-    items: List[Dict[str, Any]] = []
+
+    kwargs = dict(kwargs)
+    if segment is not None:
+        kwargs["Segment"] = segment
 
     while next_token:
-        response = _handle_reserved_keyword_error(client_dynamodb.scan)(**kwargs, Segment=segment)  # type: ignore[type-var]
+        response = _handle_reserved_keyword_error(client_dynamodb.scan)(**kwargs)
         # Unlike a resource, the DynamoDB client returns serialized results, so they must be deserialized
         # Additionally, the DynamoDB "Binary" type is converted to a native Python data type
         # SEE: https://boto3.amazonaws.com/v1/documentation/api/latest/_modules/boto3/dynamodb/types.html
-        items.extend(
-            [
-                {k: v["B"] if list(v.keys())[0] == "B" else deserializer.deserialize(v) for k, v in d.items()}
-                for d in response.get("Items", [])
-            ]
-        )
+        items = [
+            {k: v["B"] if list(v.keys())[0] == "B" else deserializer.deserialize(v) for k, v in d.items()}
+            for d in response.get("Items", [])
+        ]
+        yield _utils.list_to_arrow_table(mapping=items) if as_dataframe else items
+
         next_token = response.get("LastEvaluatedKey", None)  # type: ignore[assignment]
-        kwargs["ExclusiveStartKey"] = next_token
+        if next_token:
+            kwargs["ExclusiveStartKey"] = next_token
+
+
+@engine.dispatch_on_engine
+@_utils.retry(
+    ex=ClientError,
+    ex_code="ProvisionedThroughputExceededException",
+)
+def _read_scan(
+    dynamodb_client: Optional["DynamoDBClient"],
+    as_dataframe: bool,
+    kwargs: Dict[str, Any],
+    segment: int,
+) -> Union[pa.Table, _ItemsListType]:
+    items_iterator: Iterator[_ItemsListType] = _read_scan_chunked(dynamodb_client, False, kwargs, segment)
+
+    items = list(itertools.chain.from_iterable(items_iterator))
+
     return _utils.list_to_arrow_table(mapping=items) if as_dataframe else items
 
 
-@_handle_reserved_keyword_error
-def _read_query(table_name: str, boto3_session: Optional[boto3.Session] = None, **kwargs: Any) -> List[Dict[str, Any]]:
+def _read_query_chunked(
+    table_name: str, boto3_session: Optional[boto3.Session] = None, **kwargs: Any
+) -> Iterator[_ItemsListType]:
     table = get_table(table_name=table_name, boto3_session=boto3_session)
     response = table.query(**kwargs)
-    items = response.get("Items", [])
+    yield response.get("Items", [])
 
     # Handle pagination
     while "LastEvaluatedKey" in response:
         kwargs["ExclusiveStartKey"] = response["LastEvaluatedKey"]
         response = table.query(**kwargs)
-        items.extend(response.get("Items", []))
-    return items
+        yield response.get("Items", [])
 
 
 @_handle_reserved_keyword_error
-def _read_batch_items(
+def _read_query(
+    table_name: str, chunked: bool, boto3_session: Optional[boto3.Session] = None, **kwargs: Any
+) -> Union[_ItemsListType, Iterator[_ItemsListType]]:
+    items_iterator = _read_query_chunked(table_name, boto3_session, **kwargs)
+
+    if chunked:
+        return items_iterator
+    else:
+        return list(itertools.chain.from_iterable(items_iterator))
+
+
+def _read_batch_items_chunked(
     table_name: str, boto3_session: Optional[boto3.Session] = None, **kwargs: Any
-) -> List[Dict[str, Any]]:
+) -> Iterator[_ItemsListType]:
     resource = _utils.resource(service_name="dynamodb", session=boto3_session)
+
     response = resource.batch_get_item(RequestItems={table_name: kwargs})  # type: ignore[dict-item]
-    items = response.get("Responses", {table_name: []}).get(table_name, [])
+    yield response.get("Responses", {table_name: []}).get(table_name, [])  # type: ignore[arg-type]
 
     # SEE: handle possible unprocessed keys. As suggested in Boto3 docs,
     # this approach should involve exponential backoff, but this should be
     # already managed by AWS SDK itself, as stated
     # [here](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Programming.Errors.html)
     while response["UnprocessedKeys"]:
         kwargs["Keys"] = response["UnprocessedKeys"][table_name]["Keys"]
+
         response = resource.batch_get_item(RequestItems={table_name: kwargs})  # type: ignore[dict-item]
-        items.extend(response.get("Responses", {table_name: []}).get(table_name, []))
-    return items
+        yield response.get("Responses", {table_name: []}).get(table_name, [])  # type: ignore[arg-type]
+
+
+@_handle_reserved_keyword_error
+def _read_batch_items(
+    table_name: str, chunked: bool, boto3_session: Optional[boto3.Session] = None, **kwargs: Any
+) -> Union[_ItemsListType, Iterator[_ItemsListType]]:
+    items_iterator = _read_batch_items_chunked(table_name, boto3_session, **kwargs)
+
+    if chunked:
+        return items_iterator
+    else:
+        return list(itertools.chain.from_iterable(items_iterator))
 
 
 @_handle_reserved_keyword_error
-def _read_item(table_name: str, boto3_session: Optional[boto3.Session] = None, **kwargs: Any) -> List[Dict[str, Any]]:
+def _read_item(
+    table_name: str, chunked: bool = False, boto3_session: Optional[boto3.Session] = None, **kwargs: Any
+) -> Union[_ItemsListType, Iterator[_ItemsListType]]:
     table = get_table(table_name=table_name, boto3_session=boto3_session)
-    return [table.get_item(**kwargs).get("Item", {})]
+    item_list: _ItemsListType = [table.get_item(**kwargs).get("Item", {})]
+
+    return [item_list] if chunked else item_list
+
+
+def _read_items_scan(
+    table_name: str,
+    as_dataframe: bool,
+    arrow_kwargs: Dict[str, Any],
+    use_threads: Union[bool, int],
+    chunked: bool,
+    boto3_session: Optional[boto3.Session] = None,
+    **kwargs: Any,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame], _ItemsListType, Iterator[_ItemsListType]]:
+    dynamodb_client = _utils.client(service_name="dynamodb", session=boto3_session)
+
+    kwargs = _serialize_kwargs(kwargs)
+    kwargs["TableName"] = table_name
+
+    if chunked:
+        _logger.debug("Scanning DynamoDB table %s and returning results in an iterator", table_name)
+        scan_iterator = _read_scan_chunked(dynamodb_client, as_dataframe, kwargs)
+        if as_dataframe:
+            return (_utils.table_refs_to_df([items], arrow_kwargs) for items in scan_iterator)
+
+        return scan_iterator
+
+    # Use Parallel Scan
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
+    total_segments = _utils.ensure_worker_or_thread_count(use_threads=use_threads)
+    kwargs["TotalSegments"] = total_segments
+
+    _logger.debug("Scanning DynamoDB table %s with %d segments", table_name, total_segments)
+
+    items = executor.map(
+        _read_scan,
+        dynamodb_client,
+        itertools.repeat(as_dataframe),
+        itertools.repeat(kwargs),
+        range(total_segments),
+    )
+
+    if as_dataframe:
+        return _utils.table_refs_to_df(items, arrow_kwargs)
+
+    return list(itertools.chain(*ray_get(items)))
 
 
 def _read_items(
     table_name: str,
     as_dataframe: bool,
     arrow_kwargs: Dict[str, Any],
     use_threads: Union[bool, int],
+    chunked: bool,
     boto3_session: Optional[boto3.Session] = None,
     **kwargs: Any,
-) -> Union[pd.DataFrame, List[Dict[str, Any]]]:
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame], _ItemsListType, Iterator[_ItemsListType]]:
     # Extract 'Keys' and 'IndexName' from provided kwargs: if needed, will be reinserted later on
     keys = kwargs.pop("Keys", None)
     index = kwargs.pop("IndexName", None)
 
     # Conditionally define optimal reading strategy
     use_get_item = (keys is not None) and (len(keys) == 1)
     use_batch_get_item = (keys is not None) and (len(keys) > 1)
     use_query = (keys is None) and ("KeyConditionExpression" in kwargs)
-    use_scan = (keys is None) and ("KeyConditionExpression" not in kwargs)
 
     # Single Item
     if use_get_item:
         kwargs["Key"] = keys[0]
-        items = _read_item(table_name, boto3_session, **kwargs)
+        items = _read_item(table_name, chunked, boto3_session, **kwargs)
 
     # Batch of Items
     elif use_batch_get_item:
         kwargs["Keys"] = keys
-        items = _read_batch_items(table_name, boto3_session, **kwargs)
+        items = _read_batch_items(table_name, chunked, boto3_session, **kwargs)
 
-    elif use_query or use_scan:
+    else:
         if index:
             kwargs["IndexName"] = index
 
         if use_query:
             # Query
-            items = _read_query(table_name, boto3_session, **kwargs)
+            _logger.debug("Query DynamoDB table %s", table_name)
+            items = _read_query(table_name, chunked, boto3_session, **kwargs)
         else:
-            # Last resort use Parallel Scan
-            executor = _get_executor(use_threads=use_threads)
-            dynamodb_client = _utils.client(service_name="dynamodb", session=boto3_session)
-            total_segments = _utils.ensure_cpu_count(use_threads=use_threads)
-            kwargs = _serialize_kwargs(kwargs)
-            kwargs["TableName"] = table_name
-            kwargs["TotalSegments"] = total_segments
-
-            items = executor.map(
-                _read_scan,
-                dynamodb_client,
-                itertools.repeat(as_dataframe),
-                itertools.repeat(kwargs),
-                range(total_segments),
+            # Last resort use Scan
+            return _read_items_scan(
+                table_name=table_name,
+                as_dataframe=as_dataframe,
+                arrow_kwargs=arrow_kwargs,
+                use_threads=use_threads,
+                chunked=chunked,
+                boto3_session=boto3_session,
+                **kwargs,
             )
-    return _convert_items(items=items, use_scan=use_scan, as_dataframe=as_dataframe, arrow_kwargs=arrow_kwargs)
-
-
-@overload
-def read_items(
-    table_name: str,
-    index_name: Optional[str] = ...,
-    partition_values: Optional[Sequence[Any]] = ...,
-    sort_values: Optional[Sequence[Any]] = ...,
-    filter_expression: Optional[Union[ConditionBase, str]] = ...,
-    key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
-    expression_attribute_names: Optional[Dict[str, str]] = ...,
-    expression_attribute_values: Optional[Dict[str, Any]] = ...,
-    consistent: bool = ...,
-    columns: Optional[Sequence[str]] = ...,
-    allow_full_scan: bool = ...,
-    max_items_evaluated: Optional[int] = ...,
-    as_dataframe: Literal[True] = ...,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> pd.DataFrame:
-    ...
 
-
-@overload
-def read_items(
-    table_name: str,
-    *,
-    index_name: Optional[str] = ...,
-    partition_values: Optional[Sequence[Any]] = ...,
-    sort_values: Optional[Sequence[Any]] = ...,
-    filter_expression: Optional[Union[ConditionBase, str]] = ...,
-    key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
-    expression_attribute_names: Optional[Dict[str, str]] = ...,
-    expression_attribute_values: Optional[Dict[str, Any]] = ...,
-    consistent: bool = ...,
-    columns: Optional[Sequence[str]] = ...,
-    allow_full_scan: bool = ...,
-    max_items_evaluated: Optional[int] = ...,
-    as_dataframe: Literal[False],
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> List[Dict[str, Any]]:
-    ...
-
-
-@overload
-def read_items(
-    table_name: str,
-    *,
-    index_name: Optional[str] = ...,
-    partition_values: Optional[Sequence[Any]] = ...,
-    sort_values: Optional[Sequence[Any]] = ...,
-    filter_expression: Optional[Union[ConditionBase, str]] = ...,
-    key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
-    expression_attribute_names: Optional[Dict[str, str]] = ...,
-    expression_attribute_values: Optional[Dict[str, Any]] = ...,
-    consistent: bool = ...,
-    columns: Optional[Sequence[str]] = ...,
-    allow_full_scan: bool = ...,
-    max_items_evaluated: Optional[int] = ...,
-    as_dataframe: bool,
-    use_threads: Union[bool, int] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Union[pd.DataFrame, List[Dict[str, Any]]]:
-    ...
+    if chunked:
+        return _convert_items_chunked(
+            items_iterator=cast(Iterator[_ItemsListType], items), as_dataframe=as_dataframe, arrow_kwargs=arrow_kwargs
+        )
+    else:
+        return _convert_items(items=cast(_ItemsListType, items), as_dataframe=as_dataframe, arrow_kwargs=arrow_kwargs)
 
 
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def read_items(  # pylint: disable=too-many-branches
     table_name: str,
@@ -414,26 +411,27 @@
     expression_attribute_names: Optional[Dict[str, str]] = None,
     expression_attribute_values: Optional[Dict[str, Any]] = None,
     consistent: bool = False,
     columns: Optional[Sequence[str]] = None,
     allow_full_scan: bool = False,
     max_items_evaluated: Optional[int] = None,
     as_dataframe: bool = True,
+    chunked: bool = False,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Union[pd.DataFrame, List[Dict[str, Any]]]:
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame], _ItemsListType, Iterator[_ItemsListType]]:
     """Read items from given DynamoDB table.
 
     This function aims to gracefully handle (some of) the complexity of read actions
     available in Boto3 towards a DynamoDB table, abstracting it away while providing
-    a single, unified entrypoint.
+    a single, unified entry point.
 
-    Under the hood, it wraps all the four available read actions: get_item, batch_get_item,
-    query and scan.
+    Under the hood, it wraps all the four available read actions: `get_item`, `batch_get_item`,
+    `query` and `scan`.
 
     Note
     ----
     Number of Parallel Scan segments is based on the `use_threads` argument.
     A parallel scan with a large number of workers could consume all the provisioned throughput
     of the table or index.
     See: https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Scan.html#Scan.ParallelScan
@@ -464,37 +462,40 @@
         Attributes to retain in the returned items. Defaults to None (all attributes).
     allow_full_scan : bool
         If True, allow full table scan without any filtering. Defaults to False.
     max_items_evaluated : int, optional
         Limit the number of items evaluated in case of query or scan operations. Defaults to None (all matching items).
     as_dataframe : bool
         If True, return items as pd.DataFrame, otherwise as list/dict. Defaults to True.
+    chunked : bool
+        If `True` an iterable of DataFrames/lists is returned. False by default.
     use_threads : Union[bool, int]
         Used for Parallel Scan requests. True (default) to enable concurrency, False to disable multiple threads.
         If enabled os.cpu_count() is used as the max number of threads.
         If integer is provided, specified number is used.
     boto3_session : boto3.Session, optional
         Boto3 Session. Defaults to None (the default boto3 Session will be used).
     pyarrow_additional_kwargs : Dict[str, Any], optional
-        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas dataframe.
+        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
         Valid values include "split_blocks", "self_destruct", "ignore_metadata".
         e.g. pyarrow_additional_kwargs={'split_blocks': True}.
 
     Raises
     ------
     exceptions.InvalidArgumentType
         When the specified table has also a sort key but only the partition values are specified.
     exceptions.InvalidArgumentCombination
         When both partition and sort values sequences are specified but they have different lengths,
         or when provided parameters are not enough informative to proceed with a read operation.
 
     Returns
     -------
-    Union[pd.DataFrame, List[Mapping[str, Any]]]
+    pd.DataFrame | list[dict[str, Any]] | Iterable[pd.DataFrame] | Iterable[list[dict[str, Any]]]
         A Data frame containing the retrieved items, or a dictionary of returned items.
+        Alternatively, the return type can be an iterable of either type when `chunked=True`.
 
     Examples
     --------
     Reading 5 random items from a table
 
     >>> import awswrangler as wr
     >>> df = wr.dynamodb.read_items(table_name='my-table', max_items_evaluated=5)
@@ -614,23 +615,24 @@
     if expression_attribute_names:
         kwargs["ExpressionAttributeNames"] = expression_attribute_names
     if expression_attribute_values:
         kwargs["ExpressionAttributeValues"] = expression_attribute_values
     if max_items_evaluated:
         kwargs["Limit"] = max_items_evaluated
 
-    _logger.debug("kwargs: %s", kwargs)
+    _logger.debug("DynamoDB scan/query kwargs: %s", kwargs)
     # If kwargs are sufficiently informative, proceed with actual read op
     if any((partition_values, key_condition_expression, filter_expression, allow_full_scan, max_items_evaluated)):
         return _read_items(
             table_name=table_name,
             as_dataframe=as_dataframe,
             arrow_kwargs=arrow_kwargs,
             use_threads=use_threads,
             boto3_session=boto3_session,
+            chunked=chunked,
             **kwargs,
         )
     # Raise otherwise
     _args = (
         "partition_values",
         "key_condition_expression",
         "filter_expression",
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/dynamodb/_utils.py` & `awswrangler-3.1.0/awswrangler/dynamodb/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Amazon DynamoDB Utils Module (PRIVATE)."""
 
 import logging
 from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Mapping, Optional, Union
 
 import boto3
 from boto3.dynamodb.conditions import ConditionExpressionBuilder
+from boto3.dynamodb.types import TypeSerializer
 from botocore.exceptions import ClientError
 
 from awswrangler import _utils, exceptions
 from awswrangler._config import apply_configs
 
 if TYPE_CHECKING:
     from mypy_boto3_dynamodb.service_resource import Table
@@ -151,15 +152,15 @@
     Returns
     -------
     Dict[str, Any]
         Serialized dictionary.
     """
     names: Dict[str, Any] = {}
     values: Dict[str, Any] = {}
-    serializer = boto3.dynamodb.types.TypeSerializer()
+    serializer = TypeSerializer()
 
     if "FilterExpression" in kwargs and not isinstance(kwargs["FilterExpression"], str):
         builder = ConditionExpressionBuilder()
         exp_string, names, values = builder.build_expression(kwargs["FilterExpression"], False)  # type: ignore[assignment]
         kwargs["FilterExpression"] = exp_string
 
     if "ExpressionAttributeNames" in kwargs:
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/emr.py` & `awswrangler-3.1.0/awswrangler/emr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """EMR (Elastic Map Reduce) module."""
 # pylint: disable=line-too-long
 
 import logging
 import pprint
-from typing import Any, Dict, List, Optional, Union, cast
+import re
+from typing import Any, Dict, List, Literal, Optional, Union, cast
 
 import boto3
 
 from awswrangler import _utils, exceptions, sts
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
+_ActionOnFailureLiteral = Literal["TERMINATE_JOB_FLOW", "TERMINATE_CLUSTER", "CANCEL_AND_WAIT", "CONTINUE"]
+
+
 def _get_ecr_credentials_refresh_content(region: str) -> str:
     return f"""
 import subprocess
 from pyspark.sql import SparkSession
 spark = SparkSession.builder.appName("ECR Setup Job").getOrCreate()
 
 COMMANDS = [
@@ -73,14 +77,36 @@
     elif (region is None) and (subnet_id is None):
         raise exceptions.InvalidArgumentCombination("You must pass region or subnet_id or both.")
     else:
         _region = cast(str, region)
     return f"s3://aws-logs-{_account_id}-{_region}/elasticmapreduce/"
 
 
+def _get_emr_classification_lib(emr_version: str) -> str:
+    """Parse emr release string.
+
+    Parse emr release string and return its corresponding Classification
+    configuration string. i.e. log4j or log4j2.
+
+    Parameters
+    ----------
+        emr_version: emr release string
+
+    Returns
+    -------
+        A string mentioning the appropriate classification lib based on the emr release.
+    """
+    matches = re.findall(r"(\d.\d.\d)", emr_version)
+    number = 670
+    if matches:
+        number = int(matches[0].replace(".", ""))
+
+    return "spark-log4j2" if number > 670 else "spark-log4j"
+
+
 def _build_cluster_args(**pars: Any) -> Dict[str, Any]:  # pylint: disable=too-many-branches,too-many-statements
     account_id: str = sts.get_account_id(boto3_session=pars["boto3_session"])
     region: str = _utils.get_region_from_session(boto3_session=pars["boto3_session"])
 
     # S3 Logging path
     if pars.get("logging_s3_path") is None:
         pars["logging_s3_path"] = _get_default_logging_path(
@@ -153,15 +179,15 @@
     if pars["security_group_service_access"] is not None:
         args["Instances"]["ServiceAccessSecurityGroup"] = pars["security_group_service_access"]
 
     # Configurations
     args["Configurations"] = (
         [
             {
-                "Classification": "spark-log4j",
+                "Classification": _get_emr_classification_lib(pars["emr_release"]),
                 "Properties": {"log4j.rootCategory": f"{pars['spark_log_level']}, console"},
             }
         ]
         if not pars["configurations"]
         else pars["configurations"]
     )
     if pars["docker"] is True:
@@ -391,14 +417,17 @@
                 "SpotSpecification": {
                     "TimeoutDurationMinutes": pars["spot_provisioning_timeout_task"],
                     "TimeoutAction": timeout_action_task,
                 }
             }
         args["Instances"]["InstanceFleets"].append(fleet_task)
 
+    if pars["security_configuration"]:
+        args["SecurityConfiguration"] = pars["security_configuration"]
+
     # Tags
     if pars["tags"] is not None:
         args["Tags"] = [{"Key": k, "Value": v} for k, v in pars["tags"].items()]
 
     _logger.debug("args: \n%s", pprint.pformat(args))
     return args
 
@@ -811,15 +840,15 @@
     return response["StepIds"]
 
 
 def submit_step(
     cluster_id: str,
     command: str,
     name: str = "my-step",
-    action_on_failure: str = "CONTINUE",
+    action_on_failure: _ActionOnFailureLiteral = "CONTINUE",
     script: bool = False,
     boto3_session: Optional[boto3.Session] = None,
 ) -> str:
     """Submit new job in the EMR Cluster.
 
     Parameters
     ----------
@@ -861,15 +890,15 @@
     _logger.debug("response: \n%s", pprint.pformat(response))
     return response["StepIds"][0]
 
 
 def build_step(
     command: str,
     name: str = "my-step",
-    action_on_failure: str = "CONTINUE",
+    action_on_failure: _ActionOnFailureLiteral = "CONTINUE",
     script: bool = False,
     region: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Dict[str, Any]:
     """Build the Step structure (dictionary).
 
     Parameters
@@ -947,15 +976,18 @@
     client_emr = _utils.client(service_name="emr", session=boto3_session)
     response = client_emr.describe_step(ClusterId=cluster_id, StepId=step_id)
     _logger.debug("response: \n%s", pprint.pformat(response))
     return response["Step"]["Status"]["State"]
 
 
 def submit_ecr_credentials_refresh(
-    cluster_id: str, path: str, action_on_failure: str = "CONTINUE", boto3_session: Optional[boto3.Session] = None
+    cluster_id: str,
+    path: str,
+    action_on_failure: _ActionOnFailureLiteral = "CONTINUE",
+    boto3_session: Optional[boto3.Session] = None,
 ) -> str:
     """Update internal ECR credentials.
 
     Parameters
     ----------
     cluster_id : str
         Cluster ID.
@@ -995,18 +1027,18 @@
     _logger.debug("response: \n%s", pprint.pformat(response))
     return response["StepIds"][0]
 
 
 def build_spark_step(
     path: str,
     args: Optional[List[str]] = None,
-    deploy_mode: str = "cluster",
+    deploy_mode: Literal["cluster", "client"] = "cluster",
     docker_image: Optional[str] = None,
     name: str = "my-step",
-    action_on_failure: str = "CONTINUE",
+    action_on_failure: _ActionOnFailureLiteral = "CONTINUE",
     region: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Dict[str, Any]:
     """Build the Step structure (dictionary).
 
     Parameters
     ----------
@@ -1070,18 +1102,18 @@
     )
 
 
 def submit_spark_step(
     cluster_id: str,
     path: str,
     args: Optional[List[str]] = None,
-    deploy_mode: str = "cluster",
+    deploy_mode: Literal["cluster", "client"] = "cluster",
     docker_image: Optional[str] = None,
     name: str = "my-step",
-    action_on_failure: str = "CONTINUE",
+    action_on_failure: _ActionOnFailureLiteral = "CONTINUE",
     region: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> str:
     """Submit Spark Step.
 
     Parameters
     ----------
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/exceptions.py` & `awswrangler-3.1.0/awswrangler/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -131,7 +131,15 @@
 
 class PolicyResourceConflict(Exception):
     """PolicyResourceConflict."""
 
 
 class NotSupported(Exception):
     """NotSupported."""
+
+
+class TimestreamLoadError(Exception):
+    """TimestreamLoadError exception."""
+
+
+class NeptuneLoadError(Exception):
+    """NeptuneLoadError."""
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/lakeformation/__init__.py` & `awswrangler-3.1.0/awswrangler/lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/lakeformation/_read.py` & `awswrangler-3.1.0/awswrangler/lakeformation/_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import boto3
 import pandas as pd
 from pyarrow import NativeFile, RecordBatchStreamReader, Table
 
 from awswrangler import _data_types, _utils, catalog
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
+from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler._sql_formatter import _EngineType, _process_sql_params
-from awswrangler._threading import _get_executor
 from awswrangler.catalog._utils import _catalog_id, _transaction_id
 from awswrangler.lakeformation._utils import commit_transaction, start_transaction, wait_query
 
 if TYPE_CHECKING:
     from mypy_boto3_lakeformation.client import LakeFormationClient
 
 _logger: logging.Logger = logging.getLogger(__name__)
@@ -60,15 +60,15 @@
                 for unit in response["WorkUnitRanges"]
                 for unit_id in range(unit["WorkUnitIdMin"], unit["WorkUnitIdMax"] + 1)  # Max is inclusive
             ]
         )
         next_token = response.get("NextToken", None)
         scan_kwargs["NextToken"] = next_token  # type: ignore[assignment]
 
-    executor = _get_executor(use_threads=use_threads)
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
 
     tables = executor.map(
         _get_work_unit_results,
         client_lakeformation,
         itertools.repeat(query_id),
         token_work_units,
     )
@@ -90,15 +90,15 @@
     params: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> pd.DataFrame:
     """Execute PartiQL query on AWS Glue Table (Transaction ID or time travel timestamp). Return Pandas DataFrame.
 
     Note
     ----
-    ORDER BY operations are not honoured.
+    ORDER BY operations are not honored.
     i.e. sql="SELECT * FROM my_table ORDER BY my_column" is NOT valid
 
     Note
     ----
     The database must NOT be explicitly defined in the PartiQL statement.
     i.e. sql="SELECT * FROM my_table" is valid
     but sql="SELECT * FROM my_db.my_table" is NOT valid
@@ -128,15 +128,15 @@
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session is used if boto3_session receives None.
     params : Dict[str, any], optional
         Dict of parameters used to format the partiQL query. Only named parameters are supported.
         The dict must contain the information in the form {"name": "value"} and the SQL query must contain
         `:name`.
     pyarrow_additional_kwargs : Dict[str, Any], optional
-        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas dataframe.
+        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
         Valid values include "split_blocks", "self_destruct", "ignore_metadata".
         e.g. pyarrow_additional_kwargs={'split_blocks': True}.
 
     Returns
     -------
     pd.DataFrame
         Pandas DataFrame.
@@ -210,15 +210,15 @@
     boto3_session: Optional[boto3.Session] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> pd.DataFrame:
     """Extract all rows from AWS Glue Table (Transaction ID or time travel timestamp). Return Pandas DataFrame.
 
     Note
     ----
-    ORDER BY operations are not honoured.
+    ORDER BY operations are not honored.
     i.e. sql="SELECT * FROM my_table ORDER BY my_column" is NOT valid
 
     Note
     ----
     Pass one of `transaction_id` or `query_as_of_time`, not both.
 
     Parameters
@@ -238,15 +238,15 @@
         If none is provided, the AWS account ID is used by default.
     use_threads : bool
         True to enable concurrent requests, False to disable multiple threads.
         When enabled, os.cpu_count() is used as the max number of threads.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session is used if boto3_session receives None.
     pyarrow_additional_kwargs : Dict[str, Any], optional
-        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas dataframe.
+        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
         Valid values include "split_blocks", "self_destruct", "ignore_metadata".
         e.g. pyarrow_additional_kwargs={'split_blocks': True}.
 
     Returns
     -------
     pd.DataFrame
         Pandas DataFrame.
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/lakeformation/_utils.py` & `awswrangler-3.1.0/awswrangler/lakeformation/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             base=1.0,
             max_num_tries=5,
             **scan_kwargs,
         )
         for objects in response["Objects"]:
             for table_object in objects["Objects"]:
                 if objects["PartitionValues"]:
-                    table_object["PartitionValues"] = objects["PartitionValues"]  # type: ignore[typeddict-item]
+                    table_object["PartitionValues"] = objects["PartitionValues"]  # type: ignore[typeddict-unknown-key]
                 table_objects.append(table_object)  # type: ignore[arg-type]
         next_token = response.get("NextToken", None)
         scan_kwargs["NextToken"] = next_token
     return table_objects
 
 
 def _update_table_objects(
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/mysql.py` & `awswrangler-3.1.0/awswrangler/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # mypy: disable-error-code=name-defined
 """Amazon MySQL Module."""
 
 import logging
 import uuid
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Type, Union, overload
+from typing import Any, Dict, Iterator, List, Literal, Optional, Tuple, Type, Union, cast, overload
 
 import boto3
-import pandas as pd
 import pyarrow as pa
 
+import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler import _databases as _db_utils
 from awswrangler._config import apply_configs
 
 pymysql = _utils.import_optional_dependency("pymysql")
 
 _logger: logging.Logger = logging.getLogger(__name__)
@@ -398,22 +398,27 @@
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
+_ToSqlModeLiteral = Literal[
+    "append", "overwrite", "upsert_replace_into", "upsert_duplicate_key", "upsert_distinct", "ignore"
+]
+
+
 @_utils.check_optional_dependency(pymysql, "pymysql")
 @apply_configs
 def to_sql(
     df: pd.DataFrame,
     con: "pymysql.connections.Connection[Any]",
     table: str,
     schema: str,
-    mode: str = "append",
+    mode: _ToSqlModeLiteral = "append",
     index: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     varchar_lengths: Optional[Dict[str, int]] = None,
     use_column_names: bool = False,
     chunksize: int = 200,
     cursorclass: Optional[Type["pymysql.cursors.Cursor"]] = None,
 ) -> None:
@@ -426,15 +431,15 @@
     con : pymysql.connections.Connection
         Use pymysql.connect() to use credentials directly or wr.mysql.connect() to fetch it from the Glue Catalog.
     table : str
         Table name
     schema : str
         Schema name
     mode : str
-        Append, overwrite, upsert_duplicate_key, upsert_replace_into, upsert_distinct, ignore.
+        append, overwrite, upsert_duplicate_key, upsert_replace_into, upsert_distinct, ignore.
             append: Inserts new records into table.
             overwrite: Drops table and recreates.
             upsert_duplicate_key: Performs an upsert using `ON DUPLICATE KEY` clause. Requires table schema to have
             defined keys, otherwise duplicate records will be inserted.
             upsert_replace_into: Performs upsert using `REPLACE INTO` clause. Less efficient and still requires the
             table schema to have keys or else duplicate records will be inserted
             upsert_distinct: Inserts new records, including duplicates, then recreates the table and inserts `DISTINCT`
@@ -480,15 +485,15 @@
     ... )
     >>> con.close()
 
     """
     if df.empty is True:
         raise exceptions.EmptyDataFrame("DataFrame cannot be empty.")
 
-    mode = mode.strip().lower()
+    mode = cast(_ToSqlModeLiteral, mode.strip().lower())
     allowed_modes = [
         "append",
         "overwrite",
         "upsert_replace_into",
         "upsert_duplicate_key",
         "upsert_distinct",
         "ignore",
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/neptune/_gremlin_init.py` & `awswrangler-3.1.0/awswrangler/neptune/_gremlin_init.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/neptune/_gremlin_parser.py` & `awswrangler-3.1.0/awswrangler/neptune/_gremlin_parser.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/neptune/_utils.py` & `awswrangler-3.1.0/awswrangler/neptune/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """Amazon Neptune Utils Module (PRIVATE)."""
 
 import logging
 from enum import Enum
 from typing import Any
 
-import pandas as pd
 from gremlin_python.process.graph_traversal import GraphTraversalSource, __
 from gremlin_python.process.translator import Translator
 from gremlin_python.process.traversal import Cardinality, T
 from gremlin_python.structure.graph import Graph
 
+import awswrangler.pandas as pd
 from awswrangler import exceptions
 from awswrangler.neptune._client import NeptuneClient
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 class WriteDFType(Enum):
-    """Dataframe type enum."""
+    """DataFrame type enum."""
 
     VERTEX = 1
     EDGE = 2
     UPDATE = 3
 
 
 def write_gremlin_df(client: NeptuneClient, df: pd.DataFrame, mode: WriteDFType, batch_size: int) -> bool:
-    """Write the provided dataframe using Gremlin.
+    """Write the provided DataFrame using Gremlin.
 
     Parameters
     ----------
     client : NeptuneClient
-        The Neptune client to write the dataframe
+        The Neptune client to write the DataFrame
     df : pd.DataFrame
-        The dataframe to write
+        The DataFrame to write
     mode : WriteDFType
-        The type of dataframe to write
+        The type of DataFrame to write
     batch_size : int
         The size of the batch to write
 
     Returns
     -------
     bool
         True if the write operation succeeded
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/opensearch/_read.py` & `awswrangler-3.1.0/awswrangler/opensearch/_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # mypy: disable-error-code=name-defined
 """Amazon OpenSearch Read Module (PRIVATE)."""
 
 from typing import Any, Collection, Dict, List, Mapping, Optional, Union
 
-import pandas as pd
-
+import awswrangler.pandas as pd
 from awswrangler import _utils, exceptions
 from awswrangler.opensearch._utils import _get_distribution, _is_serverless
 
 opensearchpy = _utils.import_optional_dependency("opensearchpy")
 
 
 def _resolve_fields(row: Mapping[str, Any]) -> Mapping[str, Any]:
@@ -48,15 +47,15 @@
     index: Optional[str] = "_all",
     search_body: Optional[Dict[str, Any]] = None,
     doc_type: Optional[str] = None,
     is_scroll: Optional[bool] = False,
     filter_path: Optional[Union[str, Collection[str]]] = None,
     **kwargs: Any,
 ) -> pd.DataFrame:
-    """Return results matching query DSL as pandas dataframe.
+    """Return results matching query DSL as pandas DataFrame.
 
     Parameters
     ----------
     client : OpenSearch
         instance of opensearchpy.OpenSearch to use.
     index : str, optional
         A comma-separated list of index names to search.
@@ -74,15 +73,15 @@
     filter_path : Union[str, Collection[str]], optional
         Use the filter_path parameter to reduce the size of the OpenSearch Service response \
 (default: ['hits.hits._id','hits.hits._source'])
     **kwargs :
         KEYWORD arguments forwarded to `opensearchpy.OpenSearch.search \
 <https://opensearch-py.readthedocs.io/en/latest/api.html#opensearchpy.OpenSearch.search>`_
         and also to `opensearchpy.helpers.scan <https://opensearch-py.readthedocs.io/en/master/helpers.html#scan>`_
-         if `is_scroll=True`
+        if `is_scroll=True`
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Results as Pandas DataFrame
 
     Examples
@@ -127,15 +126,15 @@
         response = client.search(index=index, body=search_body, filter_path=filter_path, **kwargs)
         df = _search_response_to_df(response)
     return df
 
 
 @_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def search_by_sql(client: "opensearchpy.OpenSearch", sql_query: str, **kwargs: Any) -> pd.DataFrame:
-    """Return results matching `SQL query <https://opensearch.org/docs/search-plugins/sql/index/>`_ as pandas dataframe.
+    """Return results matching `SQL query <https://opensearch.org/docs/search-plugins/sql/index/>`_ as pandas DataFrame.
 
     Parameters
     ----------
     client : OpenSearch
         instance of opensearchpy.OpenSearch to use.
     sql_query : str
         SQL query
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/opensearch/_utils.py` & `awswrangler-3.1.0/awswrangler/opensearch/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,16 @@
         while status not in _CREATE_COLLECTION_FINAL_STATUSES:
             time.sleep(_CREATE_COLLECTION_WAIT_POLLING_DELAY)
             response = client.batch_get_collection(names=[name])
             status = response["collectionDetails"][0]["status"]
 
         response = cast("BatchGetCollectionResponseTypeDef", response)
         if status == "FAILED":
-            error_details = response["collectionErrorDetails"][0]
+            errors = response["collectionErrorDetails"]
+            error_details = errors[0] if len(errors) > 0 else "No error details provided"
             raise exceptions.QueryFailed(f"Failed to create collection `{name}`: {error_details}.")
 
         return response["collectionDetails"][0]  # type: ignore[return-value]
     except botocore.exceptions.ClientError as error:
         if error.response["Error"]["Code"] == "ConflictException":
             raise exceptions.AlreadyExists(f"A collection with name `{name}` already exists.") from error
         raise error
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/opensearch/_write.py` & `awswrangler-3.1.0/awswrangler/opensearch/_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import json
 import logging
 import uuid
 from typing import Any, Dict, Generator, Iterable, List, Mapping, Optional, Tuple, Union
 
 import boto3
 import numpy as np
-import pandas as pd
 from pandas import notna
 
+import awswrangler.pandas as pd
 from awswrangler import _utils, exceptions
 from awswrangler._utils import parse_path
 from awswrangler.opensearch._utils import _get_distribution, _get_version_major, _is_serverless
 
 progressbar = _utils.import_optional_dependency("progressbar")
 opensearchpy = _utils.import_optional_dependency("opensearchpy")
 if opensearchpy:
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/oracle.py` & `awswrangler-3.1.0/awswrangler/oracle.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 # mypy: disable-error-code=name-defined
 """Amazon Oracle Database Module."""
 
 import logging
 from decimal import Decimal
-from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, TypeVar, Union, overload
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+    overload,
+)
 
 import boto3
-import pandas as pd
 import pyarrow as pa
 
+import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler import _databases as _db_utils
 from awswrangler._config import apply_configs
 
 __all__ = ["connect", "read_sql_query", "read_sql_table", "to_sql"]
 
 oracledb = _utils.import_optional_dependency("oracledb")
@@ -63,30 +75,41 @@
     cursor: "oracledb.Cursor",
     table: str,
     schema: str,
     mode: str,
     index: bool,
     dtype: Optional[Dict[str, str]],
     varchar_lengths: Optional[Dict[str, int]],
+    primary_keys: Optional[List[str]],
 ) -> None:
     if mode == "overwrite":
         _drop_table(cursor=cursor, schema=schema, table=table)
     elif _does_table_exist(cursor=cursor, schema=schema, table=table):
         return
     oracle_types: Dict[str, str] = _data_types.database_types_from_pandas(
         df=df,
         index=index,
         dtype=dtype,
         varchar_lengths_default="CLOB",
         varchar_lengths=varchar_lengths,
         converter_func=_data_types.pyarrow2oracle,
     )
     cols_str: str = "".join([f'"{k}" {v},\n' for k, v in oracle_types.items()])[:-2]
+
+    if primary_keys:
+        primary_keys_str = ", ".join([f'"{k}"' for k in primary_keys])
+    else:
+        primary_keys_str = None
+
     table_identifier = _get_table_identifier(schema, table)
-    sql = f"CREATE TABLE {table_identifier} (\n{cols_str})"
+    create_table_params: str = f"\n{cols_str}"
+    if primary_keys_str:
+        create_table_params += f",\nPRIMARY KEY ({primary_keys_str})"
+
+    sql = f"CREATE TABLE {table_identifier} ({create_table_params})"
     _logger.debug("Create table query:\n%s", sql)
     cursor.execute(sql)
 
 
 @_utils.check_optional_dependency(oracledb, "oracledb")
 def connect(
     connection: Optional[str] = None,
@@ -393,55 +416,109 @@
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
+def _generate_insert_statement(
+    table_identifier: str,
+    df: pd.DataFrame,
+    use_column_names: bool,
+) -> str:
+    column_placeholders: str = f"({', '.join([':' + str(i + 1) for i in range(len(df.columns))])})"
+
+    if use_column_names:
+        insertion_columns = "(" + ", ".join('"' + column + '"' for column in df.columns) + ")"
+    else:
+        insertion_columns = ""
+
+    return f"INSERT INTO {table_identifier} {insertion_columns} VALUES {column_placeholders}"
+
+
+def _generate_upsert_statement(
+    table_identifier: str,
+    df: pd.DataFrame,
+    use_column_names: bool,
+    primary_keys: Optional[List[str]],
+) -> str:
+    if use_column_names is False:
+        raise exceptions.InvalidArgumentCombination('`use_column_names` has to be True when `mode="upsert"`')
+    if not primary_keys:
+        raise exceptions.InvalidArgumentCombination('`primary_keys` need to be defined when `mode="upsert"`')
+
+    non_primary_key_columns = [key for key in df.columns if key not in set(primary_keys)]
+
+    primary_keys_str = ", ".join([f'"{key}"' for key in primary_keys])
+    columns_str = ", ".join([f'"{key}"' for key in non_primary_key_columns])
+
+    column_placeholders: str = f"({', '.join([':' + str(i + 1) for i in range(len(df.columns))])})"
+
+    primary_key_condition_str = " AND ".join([f'"{key}" = :{i+1}' for i, key in enumerate(primary_keys)])
+    assignment_str = ", ".join(
+        [f'"{col}" = :{i + len(primary_keys) + 1}' for i, col in enumerate(non_primary_key_columns)]
+    )
+
+    return f"""
+    BEGIN
+        INSERT INTO {table_identifier} ({primary_keys_str}, {columns_str})
+            VALUES {column_placeholders};
+        EXCEPTION
+        WHEN dup_val_on_index THEN
+            UPDATE {table_identifier}
+            SET    {assignment_str}
+            WHERE  {primary_key_condition_str};
+    END;
+    """
+
+
 @_utils.check_optional_dependency(oracledb, "oracledb")
 @apply_configs
 def to_sql(
     df: pd.DataFrame,
     con: "oracledb.Connection",
     table: str,
     schema: str,
-    mode: str = "append",
+    mode: Literal["append", "overwrite", "upsert"] = "append",
     index: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     varchar_lengths: Optional[Dict[str, int]] = None,
     use_column_names: bool = False,
+    primary_keys: Optional[List[str]] = None,
     chunksize: int = 200,
 ) -> None:
     """Write records stored in a DataFrame into Oracle Database.
 
     Parameters
     ----------
-    df : pandas.DataFrame
+    df: pandas.DataFrame
         Pandas DataFrame https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
-    con : oracledb.Connection
+    con: oracledb.Connection
         Use oracledb.connect() to use credentials directly or wr.oracle.connect() to fetch it from the Glue Catalog.
-    table : str
+    table: str
         Table name
-    schema : str
+    schema: str
         Schema name
-    mode : str
-        Append or overwrite.
-    index : bool
+    mode: str
+        Append, overwrite or upsert.
+    index: bool
         True to store the DataFrame index as a column in the table,
         otherwise False to ignore it.
     dtype: Dict[str, str], optional
         Dictionary of columns names and Oracle types to be casted.
         Useful when you have columns with undetermined or mixed data types.
         (e.g. {'col name': 'TEXT', 'col2 name': 'FLOAT'})
-    varchar_lengths : Dict[str, int], optional
+    varchar_lengths: Dict[str, int], optional
         Dict of VARCHAR length by columns. (e.g. {"col1": 10, "col5": 200}).
     use_column_names: bool
         If set to True, will use the column names of the DataFrame for generating the INSERT SQL Query.
         E.g. If the DataFrame has two columns `col1` and `col3` and `use_column_names` is True, data will only be
         inserted into the database columns `col1` and `col3`.
+    primary_keys : List[str], optional
+        Primary keys.
     chunksize: int
         Number of rows which are inserted with each SQL query. Defaults to inserting 200 rows per query.
 
     Returns
     -------
     None
         None.
@@ -471,31 +548,35 @@
                 cursor=cursor,
                 table=table,
                 schema=schema,
                 mode=mode,
                 index=index,
                 dtype=dtype,
                 varchar_lengths=varchar_lengths,
+                primary_keys=primary_keys,
             )
             if index:
                 df.reset_index(level=df.index.names, inplace=True)
+
             column_placeholders: str = f"({', '.join([':' + str(i + 1) for i in range(len(df.columns))])})"
             table_identifier = _get_table_identifier(schema, table)
-            insertion_columns = ""
-            if use_column_names:
-                insertion_columns = "(" + ", ".join('"' + column + '"' for column in df.columns) + ")"
+
+            if mode == "upsert":
+                sql = _generate_upsert_statement(table_identifier, df, use_column_names, primary_keys)
+            else:
+                sql = _generate_insert_statement(table_identifier, df, use_column_names)
 
             placeholder_parameter_pair_generator = _db_utils.generate_placeholder_parameter_pairs(
                 df=df, column_placeholders=column_placeholders, chunksize=chunksize
             )
             for _, parameters in placeholder_parameter_pair_generator:
                 parameters = list(zip(*[iter(parameters)] * len(df.columns)))
-                sql: str = f"INSERT INTO {table_identifier} {insertion_columns} VALUES {column_placeholders}"
                 _logger.debug("sql: %s", sql)
                 cursor.executemany(sql, parameters)
+
             con.commit()
     except Exception as ex:
         con.rollback()
         _logger.error(ex)
         raise
 
 
@@ -512,15 +593,15 @@
     _logger.debug("decimal dtypes: %s", dtype)
     return dtype
 
 
 def handle_oracle_objects(
     col_values: List[Any], col_name: str, dtype: Optional[Dict[str, pa.DataType]] = None
 ) -> List[Any]:
-    """Get the string representation of an Oracle LOB value, and convert float to decimal."""
+    """Retrieve Oracle LOB values which may be string or bytes, and convert float to decimal."""
     if any(isinstance(col_value, oracledb.LOB) for col_value in col_values):
         col_values = [
             col_value.read() if isinstance(col_value, oracledb.LOB) else col_value for col_value in col_values
         ]
 
     if dtype is not None:
         if isinstance(dtype[col_name], pa.Decimal128Type):
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/postgresql.py` & `awswrangler-3.1.0/awswrangler/postgresql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # mypy: disable-error-code=name-defined
 """Amazon PostgreSQL Module."""
 
 import logging
+import uuid
 from ssl import SSLContext
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union, overload
+from typing import Any, Dict, Iterator, List, Literal, Optional, Tuple, Union, cast, overload
 
 import boto3
-import pandas as pd
 import pyarrow as pa
 
+import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler import _databases as _db_utils
 from awswrangler._config import apply_configs
 
 pg8000 = _utils.import_optional_dependency("pg8000")
 
 _logger: logging.Logger = logging.getLogger(__name__)
@@ -69,14 +70,56 @@
     )
     cols_str: str = "".join([f'"{k}" {v},\n' for k, v in postgresql_types.items()])[:-2]
     sql = f'CREATE TABLE IF NOT EXISTS "{schema}"."{table}" (\n{cols_str})'
     _logger.debug("Create table query:\n%s", sql)
     cursor.execute(sql)
 
 
+def _iterate_server_side_cursor(
+    sql: str,
+    con: Any,
+    chunksize: int,
+    index_col: Optional[Union[str, List[str]]],
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]],
+    safe: bool,
+    dtype: Optional[Dict[str, pa.DataType]],
+    timestamp_as_object: bool,
+) -> Iterator[pd.DataFrame]:
+    """
+    Iterate through the results using server-side cursor.
+
+    Note: Pg8000 is not fully DB API 2.0 - compliant with fetchmany() fetching all result set. Using server-side cursor
+    allows fetching only specific amount of results reducing memory impact. Ultimately we'd like pg8000 to add full
+    support for fetchmany() or add SSCursor implementation similar to MySQL and revise this implementation in the future.
+    """
+    with con.cursor() as cursor:
+        sscursor_name: str = f"c_{uuid.uuid4().hex}"
+        cursor_args = _db_utils._convert_params(f"DECLARE {sscursor_name} CURSOR FOR {sql}", params)
+        cursor.execute(*cursor_args)
+
+        try:
+            while True:
+                cursor.execute(f"FETCH FORWARD {chunksize} FROM {sscursor_name}")
+                records = cursor.fetchall()
+
+                if not records:
+                    break
+
+                yield _db_utils._records2df(
+                    records=records,
+                    cols_names=_db_utils._get_cols_names(cursor.description),
+                    index=index_col,
+                    safe=safe,
+                    dtype=dtype,
+                    timestamp_as_object=timestamp_as_object,
+                )
+        finally:
+            cursor.execute(f"CLOSE {sscursor_name}")
+
+
 @_utils.check_optional_dependency(pg8000, "pg8000")
 def connect(
     connection: Optional[str] = None,
     secret_id: Optional[str] = None,
     catalog_id: Optional[str] = None,
     dbname: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
@@ -258,20 +301,31 @@
     ...     sql="SELECT * FROM public.my_table",
     ...     con=con
     ... )
     >>> con.close()
 
     """
     _validate_connection(con=con)
+    if chunksize is not None:
+        return _iterate_server_side_cursor(
+            sql=sql,
+            con=con,
+            chunksize=chunksize,
+            index_col=index_col,
+            params=params,
+            safe=safe,
+            dtype=dtype,
+            timestamp_as_object=timestamp_as_object,
+        )
     return _db_utils.read_sql_query(
         sql=sql,
         con=con,
         index_col=index_col,
         params=params,
-        chunksize=chunksize,
+        chunksize=None,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
 @overload
@@ -389,22 +443,25 @@
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
+_ToSqlModeLiteral = Literal["append", "overwrite", "upsert"]
+
+
 @_utils.check_optional_dependency(pg8000, "pg8000")
 @apply_configs
 def to_sql(
     df: pd.DataFrame,
     con: "pg8000.Connection",
     table: str,
     schema: str,
-    mode: str = "append",
+    mode: _ToSqlModeLiteral = "append",
     index: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     varchar_lengths: Optional[Dict[str, int]] = None,
     use_column_names: bool = False,
     chunksize: int = 200,
     upsert_conflict_columns: Optional[List[str]] = None,
     insert_conflict_columns: Optional[List[str]] = None,
@@ -468,15 +525,15 @@
     ... )
     >>> con.close()
 
     """
     if df.empty is True:
         raise exceptions.EmptyDataFrame("DataFrame cannot be empty.")
 
-    mode = mode.strip().lower()
+    mode = cast(_ToSqlModeLiteral, mode.strip().lower())
     allowed_modes = ["append", "overwrite", "upsert"]
     _db_utils.validate_mode(mode=mode, allowed_modes=allowed_modes)
     if mode == "upsert" and not upsert_conflict_columns:
         raise exceptions.InvalidArgumentValue("<upsert_conflict_columns> needs to be set when using upsert mode.")
     _validate_connection(con=con)
     try:
         with con.cursor() as cursor:
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/quicksight/__init__.py` & `awswrangler-3.1.0/awswrangler/quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/quicksight/_cancel.py` & `awswrangler-3.1.0/awswrangler/quicksight/_cancel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/quicksight/_create.py` & `awswrangler-3.1.0/awswrangler/quicksight/_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Amazon QuickSight Create Module."""
 
 import logging
 import uuid
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Dict, List, Literal, Optional, Union, cast
 
 import boto3
 
 from awswrangler import _utils, exceptions, sts
 from awswrangler.quicksight._get_list import get_data_source_arn, get_dataset_id, list_users
 from awswrangler.quicksight._utils import extract_athena_query_columns, extract_athena_table_columns
 
@@ -198,15 +198,15 @@
     name: str,
     database: Optional[str] = None,
     table: Optional[str] = None,
     sql: Optional[str] = None,
     sql_name: Optional[str] = None,
     data_source_name: Optional[str] = None,
     data_source_arn: Optional[str] = None,
-    import_mode: str = "DIRECT_QUERY",
+    import_mode: Literal["SPICE", "DIRECT_QUERY"] = "DIRECT_QUERY",
     allowed_to_use: Optional[List[str]] = None,
     allowed_to_manage: Optional[List[str]] = None,
     logical_table_alias: str = "LogicalTable",
     rename_columns: Optional[Dict[str, str]] = None,
     cast_columns_types: Optional[Dict[str, str]] = None,
     tag_columns: Optional[Dict[str, List[Dict[str, Any]]]] = None,
     tags: Optional[Dict[str, str]] = None,
@@ -262,16 +262,15 @@
     rename_columns : Dict[str, str], optional
         Dictionary to map column renames. e.g. {"old_name": "new_name", "old_name2": "new_name2"}
     cast_columns_types : Dict[str, str], optional
         Dictionary to map column casts. e.g. {"col_name": "STRING", "col_name2": "DECIMAL"}
         Valid types: 'STRING'|'INTEGER'|'DECIMAL'|'DATETIME'
     tag_columns : Dict[str, List[Dict[str, Any]]], optional
         Dictionary to map column tags.
-        e.g. {"col_name": [{ "ColumnGeographicRole": "CITY" }],
-              "col_name2": [{ "ColumnDescription": { "Text": "description" }}]}
+        e.g. {"col_name": [{ "ColumnGeographicRole": "CITY" }],"col_name2": [{ "ColumnDescription": { "Text": "description" }}]}
         Valid geospatial roles: 'COUNTRY'|'STATE'|'COUNTY'|'CITY'|'POSTCODE'|'LONGITUDE'|'LATITUDE'
     account_id : str, optional
         If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     namespace : str
         The namespace. Currently, you should set this to default.
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/quicksight/_delete.py` & `awswrangler-3.1.0/awswrangler/quicksight/_delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 def delete_template(
     name: Optional[str] = None,
     template_id: Optional[str] = None,
     version_number: Optional[int] = None,
     account_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> None:
-    """Delete a tamplate.
+    """Delete a template.
 
     Note
     ----
     You must pass a not None ``name`` or ``template_id`` argument.
 
     Parameters
     ----------
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/quicksight/_describe.py` & `awswrangler-3.1.0/awswrangler/quicksight/_describe.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     Dict[str, Any]
-        Dashboad Description.
+        Dashboard Description.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> description = wr.quicksight.describe_dashboard(name="my-dashboard")
     """
     if (name is None) and (dashboard_id is None):
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/quicksight/_get_list.py` & `awswrangler-3.1.0/awswrangler/quicksight/_get_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,15 @@
         If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     List[str]
-        Dashboad IDs.
+        Dashboard IDs.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> ids = wr.quicksight.get_dashboard_ids(name="...")
     """
     return _get_ids(
@@ -498,15 +498,15 @@
         If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     str
-        Dashboad ID.
+        Dashboard ID.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> my_id = wr.quicksight.get_dashboard_id(name="...")
     """
     return _get_id(
@@ -656,15 +656,15 @@
         If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     List[str]
-        Tamplate IDs.
+        Template IDs.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> ids = wr.quicksight.get_template_ids(name="...")
     """
     return _get_ids(
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/quicksight/_utils.py` & `awswrangler-3.1.0/awswrangler/quicksight/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/__init__.py` & `awswrangler-3.1.0/awswrangler/s3/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from awswrangler.s3._read_deltalake import read_deltalake  # noqa
 from awswrangler.s3._read_excel import read_excel  # noqa
 from awswrangler.s3._read_parquet import read_parquet, read_parquet_metadata, read_parquet_table  # noqa
 from awswrangler.s3._read_text import read_csv, read_fwf, read_json  # noqa
 from awswrangler.s3._select import select_query
 from awswrangler.s3._upload import upload  # noqa
 from awswrangler.s3._wait import wait_objects_exist, wait_objects_not_exist  # noqa
+from awswrangler.s3._write_deltalake import to_deltalake  # noqa
 from awswrangler.s3._write_excel import to_excel  # noqa
 from awswrangler.s3._write_parquet import store_parquet_metadata, to_parquet  # noqa
 from awswrangler.s3._write_text import to_csv, to_json  # noqa
 
 __all__ = [
     "copy_objects",
     "merge_datasets",
@@ -37,12 +38,13 @@
     "wait_objects_exist",
     "wait_objects_not_exist",
     "select_query",
     "store_parquet_metadata",
     "to_parquet",
     "to_csv",
     "to_json",
+    "to_deltalake",
     "to_excel",
     "read_excel",
     "download",
     "upload",
 ]
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_copy.py` & `awswrangler-3.1.0/awswrangler/s3/_copy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Amazon S3 Copy Module (PRIVATE)."""
 
 import itertools
 import logging
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Tuple, Union
 
 import boto3
 from boto3.s3.transfer import TransferConfig
 
 from awswrangler import _utils, exceptions
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor
+from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.distributed.ray import ray_get
 from awswrangler.s3._delete import delete_objects
 from awswrangler.s3._fs import get_botocore_valid_kwargs
 from awswrangler.s3._list import list_objects
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
@@ -25,15 +25,15 @@
 @engine.dispatch_on_engine
 def _copy_objects(
     s3_client: Optional["S3Client"],
     batch: List[Tuple[str, str]],
     use_threads: Union[bool, int],
     s3_additional_kwargs: Optional[Dict[str, Any]],
 ) -> None:
-    _logger.debug("len(batch): %s", len(batch))
+    _logger.debug("Copying %s objects", len(batch))
     s3_client = s3_client if s3_client else _utils.client(service_name="s3")
     for source, target in batch:
         source_bucket, source_key = _utils.parse_path(path=source)
         copy_source: CopySourceTypeDef = {"Bucket": source_bucket, "Key": source_key}
         target_bucket, target_key = _utils.parse_path(path=target)
         s3_client.copy(
             CopySource=copy_source,
@@ -51,15 +51,15 @@
     s3_additional_kwargs: Optional[Dict[str, Any]],
 ) -> None:
     s3_client = _utils.client(service_name="s3", session=boto3_session)
     if s3_additional_kwargs is None:
         boto3_kwargs: Optional[Dict[str, Any]] = None
     else:
         boto3_kwargs = get_botocore_valid_kwargs(function_name="copy_object", s3_additional_kwargs=s3_additional_kwargs)
-    executor = _get_executor(use_threads=use_threads)
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     ray_get(
         executor.map(
             _copy_objects,
             s3_client,
             batches,
             itertools.repeat(use_threads),
             itertools.repeat(boto3_kwargs),
@@ -69,15 +69,15 @@
 
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def merge_datasets(
     source_path: str,
     target_path: str,
-    mode: str = "append",
+    mode: Literal["append", "overwrite", "overwrite_partitions"] = "append",
     ignore_empty: bool = False,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> List[str]:
     """Merge a source dataset into a target dataset.
 
@@ -150,15 +150,14 @@
     ["s3://bucket1/dir1/key0", "s3://bucket1/dir1/key1"]
 
     """
     source_path = source_path[:-1] if source_path[-1] == "/" else source_path
     target_path = target_path[:-1] if target_path[-1] == "/" else target_path
 
     paths: List[str] = list_objects(path=f"{source_path}/", ignore_empty=ignore_empty, boto3_session=boto3_session)
-    _logger.debug("len(paths): %s", len(paths))
     if len(paths) < 1:
         return []
 
     if mode == "overwrite":
         _logger.debug("Deleting to overwrite: %s/", target_path)
         delete_objects(path=f"{target_path}/", use_threads=use_threads, boto3_session=boto3_session)
     elif mode == "overwrite_partitions":
@@ -176,15 +175,14 @@
         paths=paths,
         source_path=source_path,
         target_path=target_path,
         use_threads=use_threads,
         boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
     )
-    _logger.debug("len(new_objects): %s", len(new_objects))
     return new_objects
 
 
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def copy_objects(
@@ -251,15 +249,14 @@
     ...         'ServerSideEncryption': 'aws:kms',
     ...         'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'
     ...     }
     ... )
     ["s3://bucket1/dir1/key0", "s3://bucket1/dir1/key1"]
 
     """
-    _logger.debug("len(paths): %s", len(paths))
     if len(paths) < 1:
         return []
     source_path = source_path[:-1] if source_path[-1] == "/" else source_path
     target_path = target_path[:-1] if target_path[-1] == "/" else target_path
     batch: List[Tuple[str, str]] = []
     new_objects: List[str] = []
     for path in paths:
@@ -272,15 +269,15 @@
                 filename: str = parts[1]
                 if filename in replace_filenames:
                     new_filename: str = replace_filenames[filename]
                     _logger.debug("Replacing filename: %s -> %s", filename, new_filename)
                     path_final = f"{path_wo_filename}/{new_filename}"
         new_objects.append(path_final)
         batch.append((path, path_final))
-    _logger.debug("len(new_objects): %s", len(new_objects))
+    _logger.debug("Creating %s new objects", len(new_objects))
     _copy(
         batches=_utils.chunkify(lst=batch, max_length=1_000),
         use_threads=use_threads,
         boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
     )
     return new_objects
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_delete.py` & `awswrangler-3.1.0/awswrangler/s3/_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import boto3
 
 from awswrangler import _utils, exceptions
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor
+from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.distributed.ray import ray_get
 from awswrangler.s3._fs import get_botocore_valid_kwargs
 from awswrangler.s3._list import _path2list
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
 
@@ -34,30 +34,30 @@
 @engine.dispatch_on_engine
 def _delete_objects(
     s3_client: Optional["S3Client"],
     paths: List[str],
     s3_additional_kwargs: Optional[Dict[str, Any]],
 ) -> None:
     s3_client = s3_client if s3_client else _utils.client(service_name="s3")
-    _logger.debug("len(paths): %s", len(paths))
+
     if s3_additional_kwargs:
         extra_kwargs: Dict[str, Any] = get_botocore_valid_kwargs(
             function_name="list_objects_v2", s3_additional_kwargs=s3_additional_kwargs
         )
     else:
         extra_kwargs = {}
     bucket = _utils.parse_path(path=paths[0])[0]
     batch: List[Dict[str, str]] = [{"Key": _utils.parse_path(path)[1]} for path in paths]
     res = s3_client.delete_objects(
         Bucket=bucket,
         Delete={"Objects": batch},  # type: ignore[typeddict-item]
         **extra_kwargs,
     )
     deleted = res.get("Deleted", [])
-    _logger.debug("len(deleted): %s", len(deleted))
+    _logger.debug("Deleted %s objects", len(deleted))
     errors = res.get("Errors", [])
     for error in errors:
         _logger.debug("error: %s", error)
         if "Code" not in error or error["Code"] != "InternalError":
             raise exceptions.ServiceApiError(errors)
 
 
@@ -132,15 +132,15 @@
     )
     paths_by_bucket: Dict[str, List[str]] = _split_paths_by_bucket(paths)
 
     chunks = []
     for _, paths in paths_by_bucket.items():
         chunks += _utils.chunkify(lst=paths, max_length=1_000)
 
-    executor = _get_executor(use_threads=use_threads)
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     ray_get(
         executor.map(
             _delete_objects,
             s3_client,
             chunks,
             itertools.repeat(s3_additional_kwargs),
         )
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_describe.py` & `awswrangler-3.1.0/awswrangler/s3/_describe.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 
 import boto3
 
 from awswrangler import _utils
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor
+from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.distributed.ray import ray_get
 from awswrangler.s3 import _fs
 from awswrangler.s3._list import _path2list
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
 
@@ -120,19 +120,18 @@
     paths = _path2list(
         path=path,
         s3_client=s3_client,
         last_modified_begin=last_modified_begin,
         last_modified_end=last_modified_end,
         s3_additional_kwargs=s3_additional_kwargs,
     )
-    _logger.debug("len(paths): %s", len(paths))
     if len(paths) < 1:
         return {}
 
-    executor = _get_executor(use_threads=use_threads)
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     resp_list = ray_get(
         executor.map(
             _describe_object,
             s3_client,
             paths,
             itertools.repeat(s3_additional_kwargs),
             [version_id.get(p) if isinstance(version_id, dict) else version_id for p in paths],
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_download.py` & `awswrangler-3.1.0/awswrangler/s3/_download.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_fs.py` & `awswrangler-3.1.0/awswrangler/s3/_fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def _snake_to_camel_case(s: str) -> str:
     return "".join(c.title() for c in s.split("_"))
 
 
 def get_botocore_valid_kwargs(function_name: str, s3_additional_kwargs: Dict[str, Any]) -> Dict[str, Any]:
     """Filter and keep only the valid botocore key arguments."""
     s3_operation_model = _S3_SERVICE_MODEL.operation_model(_snake_to_camel_case(function_name))
-    allowed_kwargs = s3_operation_model.input_shape.members.keys()  # pylint: disable=E1101
+    allowed_kwargs = s3_operation_model.input_shape.members.keys()  # type: ignore[union-attr] # pylint: disable=E1101
     return {k: v for k, v in s3_additional_kwargs.items() if k in allowed_kwargs}
 
 
 def _fetch_range(
     range_values: Tuple[int, int],
     bucket: str,
     key: str,
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_list.py` & `awswrangler-3.1.0/awswrangler/s3/_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                 last_modified_begin=last_modified_begin,
                 last_modified_end=last_modified_end,
                 ignore_empty=ignore_empty,
                 s3_additional_kwargs=s3_additional_kwargs,
             )
             for path in paths
         ]
+        _logger.debug("Listed %s paths", len(paths))
     elif isinstance(path, list):
         if last_modified_begin or last_modified_end:
             raise exceptions.InvalidArgumentCombination(
                 "Specify a list of files or (last_modified_begin and last_modified_end)"
             )
         paths = path if _suffix is None else [x for x in path if x.endswith(tuple(_suffix))]
         paths = path if _ignore_suffix is None else [x for x in paths if x.endswith(tuple(_ignore_suffix)) is False]
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_list.pyi` & `awswrangler-3.1.0/awswrangler/s3/_list.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_read.py` & `awswrangler-3.1.0/awswrangler/s3/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_read_deltalake.py` & `awswrangler-3.1.0/awswrangler/s3/_read_deltalake.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 """Amazon S3 Read Delta Lake Module (PRIVATE)."""
 
-from typing import Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 import boto3
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils
 
-deltalake = _utils.import_optional_dependency("deltalake")
+if TYPE_CHECKING:
+    try:
+        import deltalake
+    except ImportError:
+        pass
+else:
+    deltalake = _utils.import_optional_dependency("deltalake")
 
 
 def _set_default_storage_options_kwargs(
     boto3_session: Optional[boto3.Session], s3_additional_kwargs: Optional[Dict[str, Any]]
 ) -> Dict[str, Any]:
     defaults = {key.upper(): value for key, value in _utils.boto3_to_primitives(boto3_session=boto3_session).items()}
     s3_additional_kwargs = s3_additional_kwargs or {}
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_read_excel.py` & `awswrangler-3.1.0/awswrangler/s3/_read_excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Amazon S3 Excel Read Module (PRIVATE)."""
 
 import logging
 from typing import Any, Dict, Optional, Union
 
 import boto3
-import pandas as pd
 
+import awswrangler.pandas as pd
 from awswrangler import _utils, exceptions
 from awswrangler.s3._fs import open_s3_object
 
 openpyxl = _utils.import_optional_dependency("openpyxl")
 
 _logger: logging.Logger = logging.getLogger(__name__)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_read_parquet.py` & `awswrangler-3.1.0/awswrangler/s3/_read_parquet.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,32 +8,30 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Iterator,
     List,
-    Literal,
     Optional,
     Tuple,
     Union,
-    overload,
 )
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 import pyarrow.dataset
 import pyarrow.parquet
 
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._arrow import _add_table_partitions, _table_to_df
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor
+from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.catalog._get import _get_partitions
 from awswrangler.catalog._utils import _catalog_id
 from awswrangler.distributed.ray import ray_get
 from awswrangler.s3._fs import open_s3_object
 from awswrangler.s3._list import _path2list
 from awswrangler.s3._read import (
     _apply_partition_filter,
@@ -111,15 +109,15 @@
     s3_client: "S3Client",
     s3_additional_kwargs: Optional[Dict[str, str]],
     version_ids: Optional[Dict[str, str]] = None,
     coerce_int96_timestamp_unit: Optional[str] = None,
 ) -> List[pa.schema]:
     paths = _utils.list_sampling(lst=paths, sampling=sampling)
 
-    executor = _get_executor(use_threads=use_threads)
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     schemas = ray_get(
         executor.map(
             _read_parquet_metadata_file,
             s3_client,
             paths,
             itertools.repeat(s3_additional_kwargs),
             itertools.repeat(use_threads),
@@ -165,15 +163,15 @@
     )
     return _validate_schemas(schemas, validate_schema)
 
 
 def _read_parquet_metadata(
     path: Union[str, List[str]],
     path_suffix: Optional[str],
-    path_ignore_suffix: Optional[str],
+    path_ignore_suffix: Union[str, List[str], None],
     ignore_empty: bool,
     ignore_null: bool,
     dtype: Optional[Dict[str, str]],
     sampling: float,
     dataset: bool,
     use_threads: Union[bool, int],
     boto3_session: Optional[boto3.Session],
@@ -329,132 +327,29 @@
     parallelism: int,
     version_ids: Optional[Dict[str, str]],
     s3_client: Optional["S3Client"],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     arrow_kwargs: Dict[str, Any],
     bulk_read: bool,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    executor = _get_executor(use_threads=use_threads)
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     tables = executor.map(
         _read_parquet_file,
         s3_client,
         paths,
         itertools.repeat(path_root),
         itertools.repeat(columns),
         itertools.repeat(coerce_int96_timestamp_unit),
         itertools.repeat(s3_additional_kwargs),
         itertools.repeat(use_threads),
         [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths],
     )
     return _utils.table_refs_to_df(tables, kwargs=arrow_kwargs)
 
 
-@overload
-def read_parquet(
-    path: Union[str, List[str]],
-    path_root: Optional[str] = ...,
-    dataset: bool = ...,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    ignore_empty: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    columns: Optional[List[str]] = ...,
-    validate_schema: bool = ...,
-    coerce_int96_timestamp_unit: Optional[str] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    chunked: Literal[False] = ...,
-    use_threads: Union[bool, int] = ...,
-    ray_args: Optional[RayReadParquetSettings] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> pd.DataFrame:
-    ...
-
-
-@overload
-def read_parquet(
-    path: Union[str, List[str]],
-    *,
-    path_root: Optional[str] = ...,
-    dataset: bool = ...,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    ignore_empty: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    columns: Optional[List[str]] = ...,
-    validate_schema: bool = ...,
-    coerce_int96_timestamp_unit: Optional[str] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    chunked: Literal[True],
-    use_threads: Union[bool, int] = ...,
-    ray_args: Optional[RayReadParquetSettings] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_parquet(
-    path: Union[str, List[str]],
-    *,
-    path_root: Optional[str] = ...,
-    dataset: bool = ...,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    ignore_empty: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    columns: Optional[List[str]] = ...,
-    validate_schema: bool = ...,
-    coerce_int96_timestamp_unit: Optional[str] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    chunked: bool,
-    use_threads: Union[bool, int] = ...,
-    ray_args: Optional[RayReadParquetSettings] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
-@overload
-def read_parquet(
-    path: Union[str, List[str]],
-    *,
-    path_root: Optional[str] = ...,
-    dataset: bool = ...,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    ignore_empty: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    columns: Optional[List[str]] = ...,
-    validate_schema: bool = ...,
-    coerce_int96_timestamp_unit: Optional[str] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    chunked: int,
-    use_threads: Union[bool, int] = ...,
-    ray_args: Optional[RayReadParquetSettings] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session", "version_id", "s3_additional_kwargs"],
 )
 def read_parquet(
     path: Union[str, List[str]],
     path_root: Optional[str] = None,
     dataset: bool = False,
@@ -530,15 +425,15 @@
     partition_filter : Callable[[Dict[str, str]], bool], optional
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-data-wrangler.readthedocs.io/en/3.0.0rc3/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-data-wrangler.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
@@ -557,15 +452,15 @@
         If an `INTEGER` is passed, an iterable of DataFrames is returned with maximum rows
         equal to the received INTEGER.
     use_threads : Union[bool, int], default True
         True to enable concurrent requests, False to disable multiple threads.
         If enabled, os.cpu_count() is used as the max number of threads.
         If integer is provided, specified number is used.
     ray_args: typing.RayReadParquetSettings, optional
-        Params of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
+        Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session is used if None is received.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forward to S3 botocore requests.
     pyarrow_additional_kwargs : Dict[str, Any], optional
         Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
         Valid values include "split_blocks", "self_destruct", "ignore_metadata".
@@ -631,15 +526,14 @@
     )
     if not path_root:
         path_root = _get_path_root(path=path, dataset=dataset)
     if path_root and partition_filter:
         paths = _apply_partition_filter(path_root=path_root, paths=paths, filter_func=partition_filter)
     if len(paths) < 1:
         raise exceptions.NoFilesFound(f"No files Found on: {path}.")
-    _logger.debug("len(paths): %s", len(paths))
 
     version_ids = _check_version_id(paths=paths, version_id=version_id)
 
     # Create PyArrow schema based on file metadata, columns filter, and partitions
     schema: Optional[pa.schema] = None
     if validate_schema and not bulk_read:
         schema = _validate_schemas_from_files(
@@ -657,15 +551,15 @@
             if partition_types:
                 partition_schema = pa.schema(
                     fields={k: _data_types.athena2pyarrow(dtype=v) for k, v in partition_types.items()}
                 )
                 schema = pa.unify_schemas([schema, partition_schema])
         if columns:
             schema = pa.schema([schema.field(column) for column in columns], schema.metadata)
-        _logger.debug("schema:\n%s", schema)
+        _logger.debug("Resolved pyarrow schema:\n%s", schema)
 
     arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
 
     if chunked:
         return _read_parquet_chunked(
             s3_client=s3_client,
             paths=paths,
@@ -691,102 +585,14 @@
         s3_additional_kwargs=s3_additional_kwargs,
         arrow_kwargs=arrow_kwargs,
         version_ids=version_ids,
         bulk_read=bulk_read,
     )
 
 
-@overload
-def read_parquet_table(
-    table: str,
-    database: str,
-    *,
-    filename_suffix: Union[str, List[str], None] = ...,
-    filename_ignore_suffix: Union[str, List[str], None] = ...,
-    catalog_id: Optional[str] = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    columns: Optional[List[str]] = ...,
-    validate_schema: bool = ...,
-    coerce_int96_timestamp_unit: Optional[str] = ...,
-    chunked: Literal[False] = ...,
-    use_threads: Union[bool, int] = ...,
-    ray_args: Optional[RayReadParquetSettings] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> pd.DataFrame:
-    ...
-
-
-@overload
-def read_parquet_table(
-    table: str,
-    database: str,
-    *,
-    filename_suffix: Union[str, List[str], None] = ...,
-    filename_ignore_suffix: Union[str, List[str], None] = ...,
-    catalog_id: Optional[str] = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    columns: Optional[List[str]] = ...,
-    validate_schema: bool = ...,
-    coerce_int96_timestamp_unit: Optional[str] = ...,
-    chunked: Literal[True],
-    use_threads: Union[bool, int] = ...,
-    ray_args: Optional[RayReadParquetSettings] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_parquet_table(
-    table: str,
-    database: str,
-    *,
-    filename_suffix: Union[str, List[str], None] = ...,
-    filename_ignore_suffix: Union[str, List[str], None] = ...,
-    catalog_id: Optional[str] = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    columns: Optional[List[str]] = ...,
-    validate_schema: bool = ...,
-    coerce_int96_timestamp_unit: Optional[str] = ...,
-    chunked: bool,
-    use_threads: Union[bool, int] = ...,
-    ray_args: Optional[RayReadParquetSettings] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
-@overload
-def read_parquet_table(
-    table: str,
-    database: str,
-    *,
-    filename_suffix: Union[str, List[str], None] = ...,
-    filename_ignore_suffix: Union[str, List[str], None] = ...,
-    catalog_id: Optional[str] = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    columns: Optional[List[str]] = ...,
-    validate_schema: bool = ...,
-    coerce_int96_timestamp_unit: Optional[str] = ...,
-    chunked: int,
-    use_threads: Union[bool, int] = ...,
-    ray_args: Optional[RayReadParquetSettings] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
 )
 def read_parquet_table(
     table: str,
     database: str,
@@ -844,15 +650,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
@@ -862,15 +668,15 @@
         If an `INTEGER` is passed, an iterable of DataFrames is returned with maximum rows
         equal to the received INTEGER.
     use_threads : Union[bool, int], default True
         True to enable concurrent requests, False to disable multiple threads.
         If enabled, os.cpu_count() is used as the max number of threads.
         If integer is provided, specified number is used.
     ray_args: typing.RayReadParquetSettings, optional
-        Params of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
+        Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session is used if None is received.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forward to S3 botocore requests.
     pyarrow_additional_kwargs : Dict[str, Any], optional
         Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
         Valid values include "split_blocks", "self_destruct", "ignore_metadata".
@@ -968,15 +774,15 @@
     unsupported_kwargs=["boto3_session"],
 )
 def read_parquet_metadata(
     path: Union[str, List[str]],
     dataset: bool = False,
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     path_suffix: Optional[str] = None,
-    path_ignore_suffix: Optional[str] = None,
+    path_ignore_suffix: Union[str, List[str], None] = None,
     ignore_empty: bool = True,
     ignore_null: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     sampling: float = 1.0,
     coerce_int96_timestamp_unit: Optional[str] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_read_text.py` & `awswrangler-3.1.0/awswrangler/s3/_read_text.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Amazon S3 Read Module (PRIVATE)."""
 import datetime
 import itertools
 import logging
 import pprint
-from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Optional, Union, overload
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Optional, Union
 
 import boto3
 import pandas as pd
 
 from awswrangler import _utils, exceptions
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor
+from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.s3._list import _path2list
 from awswrangler.s3._read import (
     _apply_partition_filter,
     _check_version_id,
     _get_path_ignore_suffix,
     _get_path_root,
     _union,
@@ -49,15 +49,15 @@
     dataset: bool,
     ignore_index: bool,
     parallelism: int,
     version_ids: Optional[Dict[str, str]],
     pandas_kwargs: Dict[str, Any],
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     parser_func = _resolve_format(read_format)
-    executor = _get_executor(use_threads=use_threads)
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     tables = executor.map(
         _read_text_file,
         s3_client,
         paths,
         [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths],
         itertools.repeat(parser_func),
         itertools.repeat(path_root),
@@ -101,28 +101,27 @@
     )
 
     path_root: Optional[str] = _get_path_root(path=path, dataset=dataset)
     if path_root is not None:
         paths = _apply_partition_filter(path_root=path_root, paths=paths, filter_func=partition_filter)
     if len(paths) < 1:
         raise exceptions.NoFilesFound(f"No files Found on: {path}.")
-    _logger.debug("len(paths): %s", len(paths))
 
     version_ids = _check_version_id(paths=paths, version_id=version_id)
 
     args: Dict[str, Any] = {
         "parser_func": _resolve_format(read_format),
         "s3_client": s3_client,
         "dataset": dataset,
         "path_root": path_root,
         "pandas_kwargs": pandas_kwargs,
         "s3_additional_kwargs": s3_additional_kwargs,
         "use_threads": use_threads,
     }
-    _logger.debug("args:\n%s", pprint.pformat(args))
+    _logger.debug("Read args:\n%s", pprint.pformat(args))
 
     if chunksize is not None:
         return _read_text_files_chunked(
             paths=paths,
             version_ids=version_ids,
             chunksize=chunksize,
             **args,
@@ -140,80 +139,14 @@
         ignore_index=ignore_index,
         parallelism=ray_args.get("parallelism", -1),
         version_ids=version_ids,
         pandas_kwargs=pandas_kwargs,
     )
 
 
-@overload
-def read_csv(
-    path: Union[str, List[str]],
-    *,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    ignore_empty: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    chunksize: None = ...,
-    dataset: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    ray_args: Optional[RaySettings] = ...,
-    **pandas_kwargs: Any,
-) -> pd.DataFrame:
-    ...
-
-
-@overload
-def read_csv(
-    path: Union[str, List[str]],
-    *,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    ignore_empty: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    chunksize: int,
-    dataset: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    ray_args: Optional[RaySettings] = ...,
-    **pandas_kwargs: Any,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_csv(
-    path: Union[str, List[str]],
-    *,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    ignore_empty: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    chunksize: Optional[int],
-    dataset: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    ray_args: Optional[RaySettings] = ...,
-    **pandas_kwargs: Any,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def read_csv(
     path: Union[str, List[str]],
     path_suffix: Union[str, List[str], None] = None,
     path_ignore_suffix: Union[str, List[str], None] = None,
@@ -288,17 +221,17 @@
     partition_filter : Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
-        Params of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
+        Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs :
         KEYWORD arguments forwarded to pandas.read_csv(). You can NOT pass `pandas_kwargs` explicitly, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_csv('s3://bucket/prefix/', sep='|', na_values=['null', 'none'], skip_blank_lines=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
 
     Returns
@@ -362,79 +295,14 @@
         last_modified_end=last_modified_end,
         ignore_index=ignore_index,
         ray_args=ray_args,
         **pandas_kwargs,
     )
 
 
-@overload
-def read_fwf(
-    path: Union[str, List[str]],
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    ignore_empty: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    chunksize: None = ...,
-    dataset: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    ray_args: Optional[RaySettings] = ...,
-    **pandas_kwargs: Any,
-) -> pd.DataFrame:
-    ...
-
-
-@overload
-def read_fwf(
-    path: Union[str, List[str]],
-    *,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    ignore_empty: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    chunksize: int,
-    dataset: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    ray_args: Optional[RaySettings] = ...,
-    **pandas_kwargs: Any,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_fwf(
-    path: Union[str, List[str]],
-    *,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    ignore_empty: bool = ...,
-    use_threads: Union[bool, int] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    chunksize: Optional[int],
-    dataset: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    ray_args: Optional[RaySettings] = ...,
-    **pandas_kwargs: Any,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def read_fwf(
     path: Union[str, List[str]],
     path_suffix: Union[str, List[str], None] = None,
     path_ignore_suffix: Union[str, List[str], None] = None,
@@ -509,17 +377,17 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
-        Params of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
+        Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_fwf(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_fwf(path='s3://bucket/prefix/', widths=[1, 3], names=["c0", "c1"])
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_fwf.html
 
     Returns
@@ -583,82 +451,14 @@
         ignore_index=True,
         sort_index=False,
         ray_args=ray_args,
         **pandas_kwargs,
     )
 
 
-@overload
-def read_json(
-    path: Union[str, List[str]],
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    ignore_empty: bool = ...,
-    orient: str = ...,
-    use_threads: Union[bool, int] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    chunksize: None = ...,
-    dataset: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    ray_args: Optional[RaySettings] = ...,
-    **pandas_kwargs: Any,
-) -> pd.DataFrame:
-    ...
-
-
-@overload
-def read_json(
-    path: Union[str, List[str]],
-    *,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    ignore_empty: bool = ...,
-    orient: str = ...,
-    use_threads: Union[bool, int] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    chunksize: int,
-    dataset: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    ray_args: Optional[RaySettings] = ...,
-    **pandas_kwargs: Any,
-) -> Iterator[pd.DataFrame]:
-    ...
-
-
-@overload
-def read_json(
-    path: Union[str, List[str]],
-    *,
-    path_suffix: Union[str, List[str], None] = ...,
-    path_ignore_suffix: Union[str, List[str], None] = ...,
-    version_id: Optional[Union[str, Dict[str, str]]] = ...,
-    ignore_empty: bool = ...,
-    orient: str = ...,
-    use_threads: Union[bool, int] = ...,
-    last_modified_begin: Optional[datetime.datetime] = ...,
-    last_modified_end: Optional[datetime.datetime] = ...,
-    boto3_session: Optional[boto3.Session] = ...,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
-    chunksize: Optional[int],
-    dataset: bool = ...,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
-    ray_args: Optional[RaySettings] = ...,
-    **pandas_kwargs: Any,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    ...
-
-
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def read_json(
     path: Union[str, List[str]],
     path_suffix: Union[str, List[str], None] = None,
     path_ignore_suffix: Union[str, List[str], None] = None,
@@ -737,17 +537,17 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
-        Params of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
+        Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_json(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_json('s3://bucket/prefix/', lines=True, keep_default_dates=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_json.html
 
     Returns
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_read_text_core.py` & `awswrangler-3.1.0/awswrangler/s3/_read_text_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_select.py` & `awswrangler-3.1.0/awswrangler/s3/_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor, _ThreadPoolExecutor
+from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.distributed.ray import ray_get
 from awswrangler.s3._describe import size_objects
 from awswrangler.s3._list import _path2list
 from awswrangler.s3._read import _get_path_ignore_suffix
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
@@ -37,14 +37,15 @@
 @_utils.retry(
     ex=exceptions.S3SelectRequestIncomplete,
 )
 def _select_object_content(
     s3_client: Optional["S3Client"],
     args: Dict[str, Any],
     scan_range: Optional[Tuple[int, int]] = None,
+    schema: Optional[pa.Schema] = None,
 ) -> pa.Table:
     client_s3: "S3Client" = s3_client if s3_client else _utils.client(service_name="s3")
     if scan_range:
         response = client_s3.select_object_content(**args, ScanRange={"Start": scan_range[0], "End": scan_range[1]})
     else:
         response = client_s3.select_object_content(**args)
 
@@ -63,32 +64,37 @@
             )
             records[0] = partial_record + records[0]
             # Record end can either be a partial record or a return char
             partial_record = records.pop()
             payload_records.extend([json.loads(record) for record in records])
         elif "End" in event:
             # End Event signals the request was successful
-            _logger.debug("Received End Event. Result is complete")
+            _logger.debug(
+                "Received End Event. Result is complete for S3 key: %s, Scan Range: %s",
+                args["Key"],
+                scan_range if scan_range else 0,
+            )
             request_complete = True
     # If the End Event is not received, the results may be incomplete
     if not request_complete:
         raise exceptions.S3SelectRequestIncomplete(
             f"S3 Select request for path {args['Key']} is incomplete as End Event was not received"
         )
 
-    return _utils.list_to_arrow_table(mapping=payload_records)
+    return _utils.list_to_arrow_table(mapping=payload_records, schema=schema)
 
 
 @engine.dispatch_on_engine
 def _select_query(
     path: str,
-    executor: _ThreadPoolExecutor,
+    executor: _BaseExecutor,
     sql: str,
     input_serialization: str,
     input_serialization_params: Dict[str, Union[bool, str]],
+    schema: Optional[pa.Schema] = None,
     compression: Optional[str] = None,
     scan_range_chunk_size: Optional[int] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> List[pa.Table]:
     bucket, key = _utils.parse_path(path)
     s3_client = _utils.client(service_name="s3", session=boto3_session)
@@ -126,15 +132,21 @@
             input_serialization_params.get("AllowQuotedRecordDelimiter"),
             input_serialization_params.get("Type") == "Document",
         ]
     ):  # Scan range is only supported for uncompressed CSV/JSON, CSV (without quoted delimiters)
         # and JSON objects (in LINES mode only)
         scan_ranges = [None]  # type: ignore[assignment]
 
-    return executor.map(_select_object_content, s3_client, itertools.repeat(args), scan_ranges)
+    return executor.map(
+        _select_object_content,
+        s3_client,
+        itertools.repeat(args),
+        scan_ranges,
+        itertools.repeat(schema),
+    )
 
 
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def select_query(
     sql: str,
@@ -197,15 +209,15 @@
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session is used if none is provided.
     s3_additional_kwargs : Dict[str, Any], optional
         Forwarded to botocore requests.
         Valid values: "SSECustomerAlgorithm", "SSECustomerKey", "ExpectedBucketOwner".
         e.g. s3_additional_kwargs={'SSECustomerAlgorithm': 'md5'}.
     pyarrow_additional_kwargs : Dict[str, Any], optional
-        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas dataframe.
+        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
         Valid values include "split_blocks", "self_destruct", "ignore_metadata".
         e.g. pyarrow_additional_kwargs={'split_blocks': True}.
 
     Returns
     -------
     pandas.DataFrame
         Pandas DataFrame with results from query.
@@ -264,26 +276,27 @@
         ignore_empty=ignore_empty,
         last_modified_begin=last_modified_begin,
         last_modified_end=last_modified_end,
         s3_additional_kwargs=s3_additional_kwargs,
     )
     if len(paths) < 1:
         raise exceptions.NoFilesFound(f"No files Found: {path}.")
-    _logger.debug("len(paths): %s", len(paths))
 
     select_kwargs: Dict[str, Any] = {
         "sql": sql,
         "input_serialization": input_serialization,
         "input_serialization_params": input_serialization_params,
         "compression": compression,
         "scan_range_chunk_size": scan_range_chunk_size,
         "boto3_session": boto3_session,
         "s3_additional_kwargs": s3_additional_kwargs,
     }
-    _logger.debug("kwargs:\n%s", pprint.pformat(select_kwargs))
+
+    if pyarrow_additional_kwargs and "schema" in pyarrow_additional_kwargs:
+        select_kwargs["schema"] = pyarrow_additional_kwargs.pop("schema")
 
     arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
-    executor = _get_executor(use_threads=use_threads)
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     tables = list(
         itertools.chain(*ray_get([_select_query(path=path, executor=executor, **select_kwargs) for path in paths]))
     )
     return _utils.table_refs_to_df(tables, kwargs=arrow_kwargs)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_upload.py` & `awswrangler-3.1.0/awswrangler/s3/_upload.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_wait.py` & `awswrangler-3.1.0/awswrangler/s3/_wait.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,91 @@
 """Amazon S3 Wait Module (PRIVATE)."""
 
 import itertools
 import logging
 from typing import TYPE_CHECKING, List, Optional, Union
 
 import boto3
+import botocore.exceptions
 
-from awswrangler import _utils
+from awswrangler import _utils, exceptions
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor
+from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.distributed.ray import ray_get
 
 if TYPE_CHECKING:
-    from mypy_boto3_s3 import S3Client
+    from mypy_boto3_s3 import ObjectExistsWaiter, ObjectNotExistsWaiter, S3Client
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _wait_object(s3_client: "S3Client", path: str, waiter_name: str, delay: int, max_attempts: int) -> None:
-    waiter = s3_client.get_waiter(waiter_name)  # type: ignore[call-overload]
-
+def _wait_object(
+    waiter: Union["ObjectExistsWaiter", "ObjectNotExistsWaiter"], path: str, delay: int, max_attempts: int
+) -> None:
     bucket, key = _utils.parse_path(path=path)
-    waiter.wait(Bucket=bucket, Key=key, WaiterConfig={"Delay": delay, "MaxAttempts": max_attempts})
+    try:
+        waiter.wait(Bucket=bucket, Key=key, WaiterConfig={"Delay": delay, "MaxAttempts": max_attempts})
+    except botocore.exceptions.WaiterError:
+        raise exceptions.NoFilesFound(f"No files found: {key}.")
 
 
 @engine.dispatch_on_engine
 def _wait_object_batch(
     s3_client: Optional["S3Client"], paths: List[str], waiter_name: str, delay: int, max_attempts: int
 ) -> None:
     s3_client = s3_client if s3_client else _utils.client(service_name="s3")
+    waiter = s3_client.get_waiter(waiter_name)  # type: ignore[call-overload]
     for path in paths:
-        _wait_object(s3_client, path, waiter_name, delay, max_attempts)
+        _wait_object(waiter, path, delay, max_attempts)
 
 
 def _wait_objects(
     waiter_name: str,
     paths: List[str],
     delay: Optional[float],
     max_attempts: Optional[int],
     use_threads: Union[bool, int],
-    parallelism: Optional[int],
     s3_client: "S3Client",
 ) -> None:
     delay = 5 if delay is None else delay
     max_attempts = 20 if max_attempts is None else max_attempts
-    parallelism = 100 if parallelism is None else parallelism
+
+    concurrency = _utils.ensure_worker_or_thread_count(use_threads)
 
     if len(paths) < 1:
         return None
 
     path_batches = (
-        _utils.chunkify(paths, num_chunks=parallelism)
-        if len(paths) > parallelism
+        _utils.chunkify(paths, num_chunks=concurrency)
+        if len(paths) > concurrency
         else _utils.chunkify(paths, max_length=1)
     )
 
-    executor = _get_executor(use_threads=use_threads)
+    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     ray_get(
         executor.map(
             _wait_object_batch,
             s3_client,
             path_batches,
             itertools.repeat(waiter_name),
             itertools.repeat(int(delay)),
             itertools.repeat(max_attempts),
         )
     )
 
-    return None
-
 
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def wait_objects_exist(
     paths: List[str],
     delay: Optional[float] = None,
     max_attempts: Optional[int] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
-    parallelism: Optional[int] = None,
 ) -> None:
     """Wait Amazon S3 objects exist.
 
     Polls S3.Client.head_object() every 5 seconds (default) until a successful
     state is reached. An error is returned after 20 (default) failed checks.
     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.ObjectExists
 
@@ -100,17 +102,14 @@
         The amount of time in seconds to wait between attempts. Default: 5
     max_attempts : int, optional
         The maximum number of attempts to be made. Default: 20
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
-    parallelism: int, optional
-        The requested parallelism of the wait. Only used when `distributed` add-on is installed.
-        Parallelism may be limited by the number of files of the dataset. 100 by default.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     None
         None.
@@ -124,29 +123,27 @@
     s3_client = _utils.client(service_name="s3", session=boto3_session)
     return _wait_objects(
         waiter_name="object_exists",
         paths=paths,
         delay=delay,
         max_attempts=max_attempts,
         use_threads=use_threads,
-        parallelism=parallelism,
         s3_client=s3_client,
     )
 
 
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def wait_objects_not_exist(
     paths: List[str],
     delay: Optional[float] = None,
     max_attempts: Optional[int] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
-    parallelism: Optional[int] = None,
 ) -> None:
     """Wait Amazon S3 objects not exist.
 
     Polls S3.Client.head_object() every 5 seconds (default) until a successful
     state is reached. An error is returned after 20 (default) failed checks.
     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.ObjectNotExists
 
@@ -163,17 +160,14 @@
         The amount of time in seconds to wait between attempts. Default: 5
     max_attempts : int, optional
         The maximum number of attempts to be made. Default: 20
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
-    parallelism: int, optional
-        The requested parallelism of the wait. Only used when `distributed` add-on is installed.
-        Parallelism may be limited by the number of files of the dataset. 100 by default.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     None
         None.
@@ -187,10 +181,9 @@
     s3_client = _utils.client(service_name="s3", session=boto3_session)
     return _wait_objects(
         waiter_name="object_not_exists",
         paths=paths,
         delay=delay,
         max_attempts=max_attempts,
         use_threads=use_threads,
-        parallelism=parallelism,
         s3_client=s3_client,
     )
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_write.py` & `awswrangler-3.1.0/awswrangler/s3/_write.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Amazon CSV S3 Write Module (PRIVATE)."""
 
 import logging
 from enum import Enum
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, NamedTuple, Optional
 
 import pandas as pd
 
 from awswrangler import _data_types, _utils, catalog, exceptions, typing
 from awswrangler._distributed import EngineEnum
 
 _logger: logging.Logger = logging.getLogger(__name__)
@@ -56,15 +56,15 @@
     mode: Optional[str],
     description: Optional[str],
     parameters: Optional[Dict[str, str]],
     columns_comments: Optional[Dict[str, str]],
     execution_engine: Enum,
 ) -> None:
     if df.empty is True:
-        raise exceptions.EmptyDataFrame("DataFrame cannot be empty.")
+        _logger.warning("Empty DataFrame will be written.")
     if dataset is False:
         if path is None:
             raise exceptions.InvalidArgumentValue("If dataset is False, the `path` argument must be passed.")
         if execution_engine == EngineEnum.PYTHON and path.endswith("/"):
             raise exceptions.InvalidArgumentValue(
                 "If <dataset=False>, the argument <path> should be a key, not a prefix."
             )
@@ -91,15 +91,29 @@
         )
     elif bucketing_info and bucketing_info[1] <= 0:
         raise exceptions.InvalidArgumentValue(
             "Please pass a value greater than 1 for the number of buckets for bucketing."
         )
 
 
+class _SanitizeResult(NamedTuple):
+    frame: pd.DataFrame
+    dtype: Dict[str, str]
+    partition_cols: List[str]
+    bucketing_info: Optional[typing.BucketingInfoTuple]
+
+
 def _sanitize(
-    df: pd.DataFrame, dtype: Dict[str, str], partition_cols: List[str]
-) -> Tuple[pd.DataFrame, Dict[str, str], List[str]]:
+    df: pd.DataFrame,
+    dtype: Dict[str, str],
+    partition_cols: List[str],
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
+) -> _SanitizeResult:
     df = catalog.sanitize_dataframe_columns_names(df=df)
     partition_cols = [catalog.sanitize_column_name(p) for p in partition_cols]
+    if bucketing_info:
+        bucketing_info = [
+            catalog.sanitize_column_name(bucketing_col) for bucketing_col in bucketing_info[0]
+        ], bucketing_info[1]
     dtype = {catalog.sanitize_column_name(k): v.lower() for k, v in dtype.items()}
     _utils.check_duplicated_columns(df=df)
-    return df, dtype, partition_cols
+    return _SanitizeResult(df, dtype, partition_cols, bucketing_info)
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_write_concurrent.py` & `awswrangler-3.1.0/awswrangler/s3/_write_concurrent.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_write_dataset.py` & `awswrangler-3.1.0/awswrangler/s3/_write_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -314,16 +314,16 @@
             path_root=path_root,
             filename_prefix=filename_prefix,
             use_threads=use_threads,
             index=index,
             s3_client=s3_client,
             **func_kwargs,
         )
-    _logger.debug("paths: %s", paths)
-    _logger.debug("partitions_values: %s", partitions_values)
+    _logger.debug("Wrote %s paths", len(paths))
+    _logger.debug("Created partitions_values: %s", partitions_values)
     if (table_type == "GOVERNED") and (table is not None) and (database is not None):
         list_add_objects: List[
             List[Dict[str, Any]]
         ] = lakeformation._build_table_objects(  # pylint: disable=protected-access
             paths, partitions_values, use_threads=use_threads, boto3_session=boto3_session
         )
         try:
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_write_excel.py` & `awswrangler-3.1.0/awswrangler/s3/_write_excel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_write_parquet.py` & `awswrangler-3.1.0/awswrangler/s3/_write_parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Amazon PARQUET S3 Parquet Write Module (PRIVATE)."""
 
 import logging
 import math
 import uuid
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Literal, Optional, Tuple, Union, cast
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 import pyarrow.lib
 import pyarrow.parquet
 
@@ -237,15 +237,15 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     sanitize_columns: bool = False,
     dataset: bool = False,
     filename_prefix: Optional[str] = None,
     partition_cols: Optional[List[str]] = None,
     bucketing_info: Optional[BucketingInfoTuple] = None,
     concurrent_partitioning: bool = False,
-    mode: Optional[str] = None,
+    mode: Optional[Literal["append", "overwrite", "overwrite_partitions"]] = None,
     catalog_versioning: bool = False,
     schema_evolution: bool = True,
     database: Optional[str] = None,
     table: Optional[str] = None,
     glue_table_settings: Optional[GlueTableSettings] = None,
     dtype: Optional[Dict[str, str]] = None,
     athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
@@ -254,15 +254,15 @@
     """Write Parquet file or dataset on Amazon S3.
 
     The concept of Dataset goes beyond the simple idea of ordinary files and enable more
     complex features like partitioning and catalog integration (Amazon Athena/AWS Glue Catalog).
 
     Note
     ----
-    This operation may mutate the original pandas dataframe in-place. To avoid this behaviour
+    This operation may mutate the original pandas DataFrame in-place. To avoid this behaviour
     please pass in a deep copy instead (i.e. `df.copy()`)
 
     Note
     ----
     If `database` and `table` arguments are passed, the table name and all column names
     will be automatically sanitized using `wr.catalog.sanitize_table_name` and `wr.catalog.sanitize_column_name`.
     Please, pass `sanitize_columns=True` to enforce this behaviour always.
@@ -286,17 +286,17 @@
         Compression style (``None``, ``snappy``, ``gzip``, ``zstd``).
     pyarrow_additional_kwargs : Optional[Dict[str, Any]]
         Additional parameters forwarded to pyarrow.
         e.g. pyarrow_additional_kwargs={'coerce_timestamps': 'ns', 'use_deprecated_int96_timestamps': False,
         'allow_truncated_timestamps'=False}
     max_rows_by_file : int
         Max number of rows in each file.
-        Default is None i.e. dont split the files.
+        Default is None i.e. don't split the files.
         (e.g. 33554432, 268435456)
-        Is not supported in conjuction with `index=True` when running the library with Ray/Modin.
+        Is not supported in conjunction with `index=True` when running the library with Ray/Modin.
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     s3_additional_kwargs : Optional[Dict[str, Any]]
@@ -318,38 +318,38 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode: str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/004%20-%20Parquet%20Datasets.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/004%20-%20Parquet%20Datasets.html
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised. True by default.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
         Dictionary of columns names and Athena/Glue types to be casted.
         Useful when you have columns with undetermined or mixed data types.
         (e.g. {'col name': 'bigint', 'col2 name': 'int'})
     athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
-        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        Parameters of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
         AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaPartitionProjectionSettings or as a regular Python dict.
 
         Following projection parameters are supported:
 
         .. list-table:: Projection Parameters
            :header-rows: 1
@@ -634,18 +634,19 @@
     if not pyarrow_additional_kwargs.get("coerce_timestamps"):
         pyarrow_additional_kwargs["coerce_timestamps"] = "ms"
     if "flavor" not in pyarrow_additional_kwargs:
         pyarrow_additional_kwargs["flavor"] = "spark"
 
     # Sanitize table to respect Athena's standards
     if (sanitize_columns is True) or (database is not None and table is not None):
-        df, dtype, partition_cols = _sanitize(
+        df, dtype, partition_cols, bucketing_info = _sanitize(
             df=copy_df_shallow(df),
             dtype=dtype,
             partition_cols=partition_cols,
+            bucketing_info=bucketing_info,
         )
 
     # Evaluating dtype
     catalog_table_input: Optional[Dict[str, Any]] = None
     if database is not None and table is not None:
         catalog_table_input = catalog._get_table_input(  # pylint: disable=protected-access
             database=database,
@@ -678,15 +679,15 @@
             )
             commit_trans = True
 
     df = _apply_dtype(df=df, dtype=dtype, catalog_table_input=catalog_table_input, mode=mode)
     schema: pa.Schema = _data_types.pyarrow_schema_from_pandas(
         df=df, index=index, ignore_cols=partition_cols, dtype=dtype
     )
-    _logger.debug("schema: \n%s", schema)
+    _logger.debug("Resolved pyarrow schema: \n%s", schema)
 
     if dataset is False:
         paths = _to_parquet(
             df,
             path=path,
             filename_prefix=filename_prefix,
             schema=schema,
@@ -765,19 +766,18 @@
             dtype=dtype,
             mode=mode,
             boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
             schema=schema,
             max_rows_by_file=max_rows_by_file,
         )
-        if (database is not None) and (table is not None):
+        if database and table:
             try:
                 catalog._create_parquet_table(**create_table_args)  # pylint: disable=protected-access
                 if partitions_values and (regular_partitions is True) and (table_type != "GOVERNED"):
-                    _logger.debug("partitions_values:\n%s", partitions_values)
                     catalog.add_parquet_partitions(
                         database=database,
                         table=table,
                         partitions_values=partitions_values,
                         bucketing_info=bucketing_info,
                         compression=compression,
                         boto3_session=boto3_session,
@@ -807,25 +807,25 @@
 )
 def store_parquet_metadata(  # pylint: disable=too-many-arguments,too-many-locals
     path: str,
     database: str,
     table: str,
     catalog_id: Optional[str] = None,
     path_suffix: Optional[str] = None,
-    path_ignore_suffix: Optional[str] = None,
+    path_ignore_suffix: Union[str, List[str], None] = None,
     ignore_empty: bool = True,
     dtype: Optional[Dict[str, str]] = None,
     sampling: float = 1.0,
     dataset: bool = False,
     use_threads: Union[bool, int] = True,
     description: Optional[str] = None,
     parameters: Optional[Dict[str, str]] = None,
     columns_comments: Optional[Dict[str, str]] = None,
     compression: Optional[str] = None,
-    mode: str = "overwrite",
+    mode: Literal["append", "overwrite"] = "overwrite",
     catalog_versioning: bool = False,
     regular_partitions: bool = True,
     athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Tuple[Dict[str, str], Optional[Dict[str, str]], Optional[Dict[str, List[str]]]]:
     """Infer and store parquet metadata on AWS Glue Catalog.
@@ -895,15 +895,15 @@
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     regular_partitions : bool
         Create regular partitions (Non projected partitions) on Glue Catalog.
         Disable when you will work only with Partition Projection.
         Keep enabled even when working with projections is useful to keep
         Redshift Spectrum working with the regular partitions.
     athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
-        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        Parameters of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
         AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaPartitionProjectionSettings or as a regular Python dict.
 
         Following projection parameters are supported:
 
         .. list-table:: Projection Parameters
            :header-rows: 1
@@ -990,17 +990,17 @@
         path_ignore_suffix=path_ignore_suffix,
         ignore_empty=ignore_empty,
         ignore_null=False,
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
     )
-    _logger.debug("columns_types: %s", columns_types)
-    _logger.debug("partitions_types: %s", partitions_types)
-    _logger.debug("partitions_values: %s", partitions_values)
+    _logger.debug("Resolved columns_types: %s", columns_types)
+    _logger.debug("Resolved partitions_types: %s", partitions_types)
+    _logger.debug("Resolved partitions_values: %s", partitions_values)
     catalog.create_parquet_table(
         database=database,
         table=table,
         path=path,
         columns_types=columns_types,
         partitions_types=partitions_types,
         description=description,
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/s3/_write_text.py` & `awswrangler-3.1.0/awswrangler/s3/_write_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Amazon S3 Text Write Module (PRIVATE)."""
 
 import csv
 import logging
 import uuid
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Tuple, Union, cast
 
 import boto3
 import pandas as pd
 from pandas.io.common import infer_compression
 
 from awswrangler import _data_types, _utils, catalog, exceptions, lakeformation, typing
 from awswrangler._config import apply_configs
@@ -45,15 +45,15 @@
     path_root: Optional[str] = None,
     filename_prefix: Optional[str] = None,
     bucketing: bool = False,
     **pandas_kwargs: Any,
 ) -> List[str]:
     s3_client = s3_client if s3_client else _utils.client(service_name="s3")
     if df.empty is True:
-        raise exceptions.EmptyDataFrame("DataFrame cannot be empty.")
+        _logger.warning("Empty DataFrame will be written.")
     if path is None and path_root is not None:
         file_path: str = (
             f"{path_root}{filename_prefix}.{file_format}{_COMPRESSION_2_EXT.get(pandas_kwargs.get('compression'))}"
         )
     elif path is not None and path_root is None:
         file_path = path
     else:
@@ -92,15 +92,15 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     sanitize_columns: bool = False,
     dataset: bool = False,
     filename_prefix: Optional[str] = None,
     partition_cols: Optional[List[str]] = None,
     bucketing_info: Optional[BucketingInfoTuple] = None,
     concurrent_partitioning: bool = False,
-    mode: Optional[str] = None,
+    mode: Optional[Literal["append", "overwrite", "overwrite_partitions"]] = None,
     catalog_versioning: bool = False,
     schema_evolution: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     database: Optional[str] = None,
     table: Optional[str] = None,
     glue_table_settings: Optional[GlueTableSettings] = None,
     athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
@@ -121,18 +121,14 @@
     Note
     ----
     If `table` and `database` arguments are passed, `pandas_kwargs` will be ignored due
     restrictive quoting, date_format, escapechar and encoding required by Athena/Glue Catalog.
 
     Note
     ----
-    Compression: The minimum acceptable version to achieve it is Pandas 1.2.0 that requires Python >= 3.7.1.
-
-    Note
-    ----
     In case of `use_threads=True` the number of threads
     that will be spawned will be gotten from os.cpu_count().
 
     Parameters
     ----------
     df: pandas.DataFrame
         Pandas DataFrame https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
@@ -169,38 +165,38 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions")). False by default.
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
         Dictionary of columns names and Athena/Glue types to be casted.
         Useful when you have columns with undetermined or mixed data types.
         (e.g. {'col name': 'bigint', 'col2 name': 'int'})
     athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
-        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        Parameters of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
         AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaPartitionProjectionSettings or as a regular Python dict.
 
         Following projection parameters are supported:
 
         .. list-table:: Projection Parameters
            :header-rows: 1
@@ -500,18 +496,19 @@
         table_type = "GOVERNED"
 
     filename_prefix = filename_prefix + uuid.uuid4().hex if filename_prefix else uuid.uuid4().hex
     s3_client = _utils.client(service_name="s3", session=boto3_session)
 
     # Sanitize table to respect Athena's standards
     if (sanitize_columns is True) or (database is not None and table is not None):
-        df, dtype, partition_cols = _sanitize(
+        df, dtype, partition_cols, bucketing_info = _sanitize(
             df=copy_df_shallow(df),
             dtype=dtype,
             partition_cols=partition_cols,
+            bucketing_info=bucketing_info,
         )
 
     # Evaluating dtype
     catalog_table_input: Optional[Dict[str, Any]] = None
     if database and table:
         catalog_table_input = catalog._get_table_input(  # pylint: disable=protected-access
             database=database,
@@ -668,15 +665,14 @@
                 serde_info: Dict[str, Any] = {}
                 if catalog_table_input:
                     serde_info = catalog_table_input["StorageDescriptor"]["SerdeInfo"]
                 create_table_args["serde_library"] = serde_info.get("SerializationLibrary", None)
                 create_table_args["serde_parameters"] = serde_info.get("Parameters", None)
                 catalog._create_csv_table(**create_table_args)  # pylint: disable=protected-access
                 if partitions_values and (regular_partitions is True) and (table_type != "GOVERNED"):
-                    _logger.debug("partitions_values:\n%s", partitions_values)
                     catalog.add_csv_partitions(
                         database=database,
                         table=table,
                         partitions_values=partitions_values,
                         bucketing_info=bucketing_info,
                         boto3_session=boto3_session,
                         sep=sep,
@@ -717,15 +713,15 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     sanitize_columns: bool = False,
     dataset: bool = False,
     filename_prefix: Optional[str] = None,
     partition_cols: Optional[List[str]] = None,
     bucketing_info: Optional[BucketingInfoTuple] = None,
     concurrent_partitioning: bool = False,
-    mode: Optional[str] = None,
+    mode: Optional[Literal["append", "overwrite", "overwrite_partitions"]] = None,
     catalog_versioning: bool = False,
     schema_evolution: bool = True,
     dtype: Optional[Dict[str, str]] = None,
     database: Optional[str] = None,
     table: Optional[str] = None,
     glue_table_settings: Optional[GlueTableSettings] = None,
     athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
@@ -735,18 +731,14 @@
     """Write JSON file on Amazon S3.
 
     Note
     ----
     In case of `use_threads=True` the number of threads
     that will be spawned will be gotten from os.cpu_count().
 
-    Note
-    ----
-    Compression: The minimum acceptable version to achive it is Pandas 1.2.0 that requires Python >= 3.7.1.
-
     Parameters
     ----------
     df: pandas.DataFrame
         Pandas DataFrame https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
     path : str
         Amazon S3 path (e.g. s3://bucket/filename.json).
     index : bool
@@ -777,38 +769,38 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
         Dictionary of columns names and Athena/Glue types to be casted.
         Useful when you have columns with undetermined or mixed data types.
         (e.g. {'col name': 'bigint', 'col2 name': 'int'})
     athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
-        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        Parameters of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
         AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaPartitionProjectionSettings or as a regular Python dict.
 
         Following projection parameters are supported:
 
         .. list-table:: Projection Parameters
            :header-rows: 1
@@ -988,18 +980,19 @@
         table_type = "GOVERNED"
 
     filename_prefix = filename_prefix + uuid.uuid4().hex if filename_prefix else uuid.uuid4().hex
     s3_client = _utils.client(service_name="s3", session=boto3_session)
 
     # Sanitize table to respect Athena's standards
     if (sanitize_columns is True) or (database is not None and table is not None):
-        df, dtype, partition_cols = _sanitize(
+        df, dtype, partition_cols, bucketing_info = _sanitize(
             df=copy_df_shallow(df),
             dtype=dtype,
             partition_cols=partition_cols,
+            bucketing_info=bucketing_info,
         )
 
     # Evaluating dtype
     catalog_table_input: Optional[Dict[str, Any]] = None
 
     if database and table:
         catalog_table_input = catalog._get_table_input(  # pylint: disable=protected-access
@@ -1127,15 +1120,14 @@
             serde_info: Dict[str, Any] = {}
             if catalog_table_input:
                 serde_info = catalog_table_input["StorageDescriptor"]["SerdeInfo"]
             create_table_args["serde_library"] = serde_info.get("SerializationLibrary", None)
             create_table_args["serde_parameters"] = serde_info.get("Parameters", None)
             catalog._create_json_table(**create_table_args)  # pylint: disable=protected-access
             if partitions_values and (regular_partitions is True) and (table_type != "GOVERNED"):
-                _logger.debug("partitions_values:\n%s", partitions_values)
                 catalog.add_json_partitions(
                     database=database,
                     table=table,
                     partitions_values=partitions_values,
                     bucketing_info=bucketing_info,
                     boto3_session=boto3_session,
                     serde_library=create_table_args["serde_library"],
@@ -1146,15 +1138,15 @@
                 )
                 if commit_trans:
                     lakeformation.commit_transaction(
                         transaction_id=transaction_id,  # type: ignore[arg-type]
                         boto3_session=boto3_session,
                     )
         except Exception:
-            _logger.debug("Catalog write failed, cleaning up S3 (paths: %s).", paths)
+            _logger.debug("Catalog write failed, cleaning up S3 objects (len(paths): %s).", len(paths))
             delete_objects(
                 path=paths,
                 use_threads=use_threads,
                 boto3_session=boto3_session,
                 s3_additional_kwargs=s3_additional_kwargs,
             )
             raise
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/secretsmanager.py` & `awswrangler-3.1.0/awswrangler/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/sqlserver.py` & `awswrangler-3.1.0/awswrangler/sqlserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 # mypy: disable-error-code=name-defined
 """Amazon Microsoft SQL Server Module."""
 
 import logging
-from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, TypeVar, Union, overload
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+    overload,
+)
 
 import boto3
-import pandas as pd
 import pyarrow as pa
 
+import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler import _databases as _db_utils
 from awswrangler._config import apply_configs
 
 __all__ = ["connect", "read_sql_query", "read_sql_table", "to_sql"]
 
 pyodbc = _utils.import_optional_dependency("pyodbc")
@@ -393,15 +405,15 @@
 @_utils.check_optional_dependency(pyodbc, "pyodbc")
 @apply_configs
 def to_sql(
     df: pd.DataFrame,
     con: "pyodbc.Connection",
     table: str,
     schema: str,
-    mode: str = "append",
+    mode: Literal["append", "overwrite"] = "append",
     index: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     varchar_lengths: Optional[Dict[str, int]] = None,
     use_column_names: bool = False,
     chunksize: int = 200,
     fast_executemany: bool = False,
 ) -> None:
@@ -438,15 +450,15 @@
         Mode of execution which greatly reduces round trips for a DBAPI executemany() call when using
         Microsoft ODBC drivers, for limited size batches that fit in memory. `False` by default.
 
         https://github.com/mkleehammer/pyodbc/wiki/Cursor#executemanysql-params-with-fast_executemanytrue
 
         Note: when using this mode, pyodbc converts the Python parameter values to their ODBC "C" equivalents,
         based on the target column types in the database which may lead to subtle data type conversion
-        diffferences depending on whether fast_executemany is True or False.
+        differences depending on whether fast_executemany is True or False.
 
     Returns
     -------
     None
         None.
 
     Examples
```

### Comparing `awswrangler-3.0.0rc3/awswrangler/sts.py` & `awswrangler-3.1.0/awswrangler/sts.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc3/awswrangler/typing.py` & `awswrangler-3.1.0/awswrangler/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 class AthenaPartitionProjectionSettings(TypedDict):
     """
     Typed dictionary defining the settings for Athena Partition Projection.
 
     https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html
     """
 
-    projection_types: NotRequired[Dict[str, str]]
+    projection_types: NotRequired[Dict[str, Literal["enum", "integer", "date", "injected"]]]
     """
     Dictionary of partitions names and Athena projections types.
     Valid types: "enum", "integer", "date", "injected"
     https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
     (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
     """
     projection_ranges: NotRequired[Dict[str, str]]
@@ -161,14 +161,39 @@
     Value which is allows Athena to properly map partition values if the S3 file locations do not follow
     a typical `.../column=value/...` pattern.
     https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
     (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
     """
 
 
+class TimestreamBatchLoadReportS3Configuration(TypedDict):
+    """
+    Report configuration for a batch load task. This contains details about where error reports are stored.
+
+    https://docs.aws.amazon.com/timestream/latest/developerguide/API_ReportS3Configuration.html
+    """
+
+    BucketName: Required[str]
+    """
+    The name of the bucket where the error reports are stored.
+    """
+    ObjectKeyPrefix: NotRequired[str]
+    """
+    Optional S3 prefix for the error reports.
+    """
+    Encryption: NotRequired[Literal["SSE_S3", "SSE_KMS"]]
+    """
+    Optional encryption type for the error reports. SSE_S3 by default.
+    """
+    KmsKeyId: NotRequired[str]
+    """
+    Optional KMS key ID for the error reports.
+    """
+
+
 class RaySettings(TypedDict):
     """Typed dictionary defining the settings for distributing calls using Ray."""
 
     parallelism: NotRequired[int]
     """
     The requested parallelism of the read.
     Parallelism may be limited by the number of files of the dataset.
```

### Comparing `awswrangler-3.0.0rc3/pyproject.toml` & `awswrangler-3.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awswrangler"
-version = "3.0.0rc3"
+version = "3.1.0"
 description = "Pandas on AWS."
 authors = ["Amazon Web Services"]
 license = "Apache License 2.0"
 
 readme = "README.md"
 
 include = ["README.md", "LICENSE.txt", "NOTICE.txt", "THIRD_PARTY.txt", "awswrangler/py.typed"]
@@ -17,52 +17,53 @@
 
 keywords = ["pandas", "aws"]
 
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
 
 # Required
 boto3 = "^1.20.32"
 botocore = "^1.23.32"
-pandas = "^1.0"
+pandas = ">=1.2.0,!=1.5.0,<3.0.0" # Exclusion per: https://github.com/aws/aws-sdk-pandas/issues/1678
 numpy = "^1.18"
 pyarrow = ">=7.0.0"
 typing-extensions = "^4.4.0"
 
 # Databases
 redshift-connector = { version = "^2.0.0", optional = true }
 pymysql = { version = "^1.0.0", optional = true }
 pg8000 = { version = "^1.29.0", optional = true }
 pyodbc = { version = "^4.0.0", optional = true }
 oracledb = { version = "^1.0.0", optional = true }
 
 # Graph
-gremlinpython = { version = "^3.5.2", optional = true }
+gremlinpython = { version = "^3.6.2", optional = true }
 SPARQLWrapper = { version = "^2.0.0", optional = true }
 requests = { version = "^2.0.0", optional = true }
 
 # OpenSearch
 opensearch-py = { version = "^2.0.0", optional = true }
 requests-aws4auth = { version = "^1.1.1", optional = true }
 jsonpath-ng = { version = "^1.5.3", optional = true }
 
 # Other
 openpyxl = { version = "^3.0.0", optional = true }
 progressbar2 = { version = "^4.0.0", optional = true }
-deltalake = { version = "^0.6.4", optional = true }
+deltalake = { version = ">=0.6.4,<0.10.0", optional = true }
 
 # Distributed
-modin = { version = "~0.18.0", optional = true }
-ray = { version = ">=2.0.0,<2.4.0", extras = ["default", "data"], optional = true}
+modin = { version = "^0.20.1", optional = true }
+ray = { version = ">=2.0.0,<2.5.0", extras = ["default", "data"], optional = true }
 
 [tool.poetry.extras]
 redshift = ["redshift-connector"]
 mysql = ["pymysql"]
 postgres = ["pg8000"]
 sqlserver = ["pyodbc"]
 oracle = ["oracledb"]
@@ -79,41 +80,46 @@
 [tool.poetry.dev-dependencies]
 # Build
 setuptools = "*"
 wheel = "^0.38.1"
 
 # Lint
 black = "^23.1.0"
-boto3-stubs = {version = "1.26.47", extras = ["athena", "chime", "cloudwatch", "dynamodb", "ec2", "emr", "glue", "kms", "lakeformation", "logs", "neptune", "opensearch", "opensearchserverless", "quicksight", "rds", "redshift", "redshift-data", "s3", "secretsmanager", "ssm", "sts", "timestream-query", "timestream-write"]}
+boto3-stubs = {version = "1.26.47", extras = ["athena", "chime", "cloudwatch", "dynamodb", "ec2", "emr", "glue", "kms", "lakeformation", "logs", "neptune", "opensearch", "opensearchserverless", "quicksight", "rds", "rds-data", "redshift", "redshift-data", "s3", "secretsmanager", "ssm", "sts", "timestream-query", "timestream-write"]}
 doc8 = "^1.0"
-mypy = "^0.991"
-pylint = "^2.0"
+mypy = "^1.0"
+pylint = "^2.17"
 ruff = "^0.0.240"
+isort = "^5.9.2"
+flake8 = "^5.0.1"
+pydocstyle = "^6.1.1"
 
 # Test
-moto = "^4.0"
+moto = "^4.1"
 openpyxl = "^3.0"
 pyparsing = "^3.0.7"
-pytest = "^7.0"
+pytest = "^7.1.2"
 pytest-cov = "^4.0"
-pytest-rerunfailures = "^10.0"
+pytest-rerunfailures = "^11.1"
 pytest-timeout = "^2.1.0"
-pytest-xdist = "^3.0"
+pytest-xdist = "^3.0.2"
 s3fs = "0.4.2"  # Must be pinned to 0.4.2
-tox = "^3.25.1"
+tox = "^4.5.0"
 
 # Docs
 bump2version = "^1.0.1"
-IPython = "^7.34.0"
+IPython = "^8.10.0"
 jupyterlab = "^3.0"
-nbsphinx = "^0.8"
+nbsphinx = "^0.8.8"
 nbsphinx-link = "^1.3.0"
 sphinx = "^6.0"
 sphinx-bootstrap-theme = "^0.8"
-sphinx-copybutton = "^0.5"
+sphinx-copybutton = "^0.5.1"
+pydot = "^1.4.2"
+myst-parser = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -172,11 +178,16 @@
 addopts = "--log-cli-format \"[%(name)s][%(funcName)s] %(message)s\" --verbose --capture=sys"
 markers = [
     "distributed: tests againsts methods with distributed functionality",
 ]
 
 [tool.coverage.run]
 branch = true
-omit = ["awswrangler/distributed/*", "awswrangler/neptune/_utils.py"]
+omit = [
+    "awswrangler/distributed/*",
+    "awswrangler/neptune/_utils.py",
+    "awswrangler/opensearch/_utils.py",
+    "awswrangler/chime.py",
+]
 
 [tool.coverage.report]
 show_missing = true
```

### Comparing `awswrangler-3.0.0rc3/setup.py` & `awswrangler-3.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,318 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: awswrangler
+Version: 3.1.0
+Summary: Pandas on AWS.
+Home-page: https://aws-sdk-pandas.readthedocs.io/
+License: Apache-2.0
+Keywords: pandas,aws
+Author: Amazon Web Services
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: deltalake
+Provides-Extra: gremlin
+Provides-Extra: modin
+Provides-Extra: mysql
+Provides-Extra: opencypher
+Provides-Extra: openpyxl
+Provides-Extra: opensearch
+Provides-Extra: oracle
+Provides-Extra: postgres
+Provides-Extra: progressbar
+Provides-Extra: ray
+Provides-Extra: redshift
+Provides-Extra: sparql
+Provides-Extra: sqlserver
+Requires-Dist: SPARQLWrapper (>=2.0.0,<3.0.0) ; extra == "sparql"
+Requires-Dist: boto3 (>=1.20.32,<2.0.0)
+Requires-Dist: botocore (>=1.23.32,<2.0.0)
+Requires-Dist: deltalake (>=0.6.4,<0.10.0) ; extra == "deltalake"
+Requires-Dist: gremlinpython (>=3.6.2,<4.0.0) ; extra == "gremlin"
+Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0) ; extra == "opensearch"
+Requires-Dist: modin (>=0.20.1,<0.21.0) ; extra == "modin"
+Requires-Dist: numpy (>=1.18,<2.0)
+Requires-Dist: openpyxl (>=3.0.0,<4.0.0) ; extra == "openpyxl"
+Requires-Dist: opensearch-py (>=2.0.0,<3.0.0) ; extra == "opensearch"
+Requires-Dist: oracledb (>=1.0.0,<2.0.0) ; extra == "oracle"
+Requires-Dist: pandas (>=1.2.0,!=1.5.0,<3.0.0)
+Requires-Dist: pg8000 (>=1.29.0,<2.0.0) ; extra == "postgres"
+Requires-Dist: progressbar2 (>=4.0.0,<5.0.0) ; extra == "progressbar"
+Requires-Dist: pyarrow (>=7.0.0)
+Requires-Dist: pymysql (>=1.0.0,<2.0.0) ; extra == "mysql"
+Requires-Dist: pyodbc (>=4.0.0,<5.0.0) ; extra == "sqlserver"
+Requires-Dist: ray[data,default] (>=2.0.0,<2.5.0) ; extra == "ray"
+Requires-Dist: redshift-connector (>=2.0.0,<3.0.0) ; extra == "redshift"
+Requires-Dist: requests (>=2.0.0,<3.0.0) ; extra == "gremlin" or extra == "sparql" or extra == "opencypher"
+Requires-Dist: requests-aws4auth (>=1.1.1,<2.0.0) ; extra == "opensearch"
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Project-URL: Documentation, https://aws-sdk-pandas.readthedocs.io/
+Project-URL: Repository, https://github.com/aws/aws-sdk-pandas
+Description-Content-Type: text/markdown
 
-packages = \
-['awswrangler',
- 'awswrangler.athena',
- 'awswrangler.catalog',
- 'awswrangler.data_api',
- 'awswrangler.data_quality',
- 'awswrangler.distributed',
- 'awswrangler.distributed.ray',
- 'awswrangler.distributed.ray.datasources',
- 'awswrangler.distributed.ray.modin',
- 'awswrangler.distributed.ray.modin.s3',
- 'awswrangler.distributed.ray.s3',
- 'awswrangler.dynamodb',
- 'awswrangler.lakeformation',
- 'awswrangler.neptune',
- 'awswrangler.opensearch',
- 'awswrangler.quicksight',
- 'awswrangler.s3']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['boto3>=1.20.32,<2.0.0',
- 'botocore>=1.23.32,<2.0.0',
- 'numpy>=1.18,<2.0',
- 'pandas>=1.0,<2.0',
- 'pyarrow>=7.0.0',
- 'typing-extensions>=4.4.0,<5.0.0']
-
-extras_require = \
-{'deltalake': ['deltalake>=0.6.4,<0.7.0'],
- 'gremlin': ['gremlinpython>=3.5.2,<4.0.0', 'requests>=2.0.0,<3.0.0'],
- 'modin': ['modin>=0.18.0,<0.19.0'],
- 'mysql': ['pymysql>=1.0.0,<2.0.0'],
- 'opencypher': ['requests>=2.0.0,<3.0.0'],
- 'openpyxl': ['openpyxl>=3.0.0,<4.0.0'],
- 'opensearch': ['opensearch-py>=2.0.0,<3.0.0',
-                'requests-aws4auth>=1.1.1,<2.0.0',
-                'jsonpath-ng>=1.5.3,<2.0.0'],
- 'oracle': ['oracledb>=1.0.0,<2.0.0'],
- 'postgres': ['pg8000>=1.29.0,<2.0.0'],
- 'progressbar': ['progressbar2>=4.0.0,<5.0.0'],
- 'ray': ['ray[data,default]>=2.0.0,<2.4.0'],
- 'redshift': ['redshift-connector>=2.0.0,<3.0.0'],
- 'sparql': ['SPARQLWrapper>=2.0.0,<3.0.0', 'requests>=2.0.0,<3.0.0'],
- 'sqlserver': ['pyodbc>=4.0.0,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'awswrangler',
-    'version': '3.0.0rc3',
-    'description': 'Pandas on AWS.',
-    'long_description': '# AWS SDK for pandas (awswrangler)\n\nAWS Data Wrangler is now **AWS SDK for pandas (awswrangler)**.  We’re changing the name we use when we talk about the library, but everything else will stay the same.  You’ll still be able to install using `pip install awswrangler` and you won’t need to change any of your code.  As part of this change, we’ve moved the library from AWS Labs to the main AWS GitHub organisation but, thanks to the GitHub’s redirect feature, you’ll still be able to access the project by its old URLs until you update your bookmarks.  Our documentation has also moved to [aws-sdk-pandas.readthedocs.io](https://aws-sdk-pandas.readthedocs.io), but old bookmarks will redirect to the new site.\n\n*Pandas on AWS*\n\nEasy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).\n\n![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")\n![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)\n\n> An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com\n\n[![Release](https://img.shields.io/badge/release-3.0.0rc3-brightgreen.svg)](https://pypi.org/project/awswrangler/)\n[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Coverage](https://img.shields.io/badge/coverage-91%25-brightgreen.svg)](https://pypi.org/project/awswrangler/)\n![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)\n[![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)\n\n| Source | Downloads | Installation Command |\n|--------|-----------|----------------------|\n| **[PyPi](https://pypi.org/project/awswrangler/)**  | [![PyPI Downloads](https://pepy.tech/badge/awswrangler)](https://pypi.org/project/awswrangler/) | `pip install awswrangler` |\n| **[Conda](https://anaconda.org/conda-forge/awswrangler)** | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/awswrangler.svg)](https://anaconda.org/conda-forge/awswrangler) | `conda install -c conda-forge awswrangler` |\n\n> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>\n➡️`pip install \'awswrangler[redshift]\'`\n\nPowered By [<img src="https://arrow.apache.org/img/arrow.png" width="200">](https://arrow.apache.org/powered_by/)\n\n## Table of contents\n\n- [Quick Start](#quick-start)\n- [At Scale](#at-scale)\n- [Read The Docs](#read-the-docs)\n- [Getting Help](#getting-help)\n- [Community Resources](#community-resources)\n- [Logging](#logging)\n- [Who uses AWS SDK for pandas?](#who-uses-aws-sdk-pandas)\n\n## Quick Start\n\nInstallation command: `pip install awswrangler`\n\n> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>\n➡️`pip install \'awswrangler[redshift]\'`\n\n```py3\nimport awswrangler as wr\nimport pandas as pd\nfrom datetime import datetime\n\ndf = pd.DataFrame({"id": [1, 2], "value": ["foo", "boo"]})\n\n# Storing data on Data Lake\nwr.s3.to_parquet(\n    df=df,\n    path="s3://bucket/dataset/",\n    dataset=True,\n    database="my_db",\n    table="my_table"\n)\n\n# Retrieving the data directly from Amazon S3\ndf = wr.s3.read_parquet("s3://bucket/dataset/", dataset=True)\n\n# Retrieving the data from Amazon Athena\ndf = wr.athena.read_sql_query("SELECT * FROM my_table", database="my_db")\n\n# Get a Redshift connection from Glue Catalog and retrieving data from Redshift Spectrum\ncon = wr.redshift.connect("my-glue-connection")\ndf = wr.redshift.read_sql_query("SELECT * FROM external_schema.my_table", con=con)\ncon.close()\n\n# Amazon Timestream Write\ndf = pd.DataFrame({\n    "time": [datetime.now(), datetime.now()],   \n    "my_dimension": ["foo", "boo"],\n    "measure": [1.0, 1.1],\n})\nrejected_records = wr.timestream.write(df,\n    database="sampleDB",\n    table="sampleTable",\n    time_col="time",\n    measure_col="measure",\n    dimensions_cols=["my_dimension"],\n)\n\n# Amazon Timestream Query\nwr.timestream.query("""\nSELECT time, measure_value::double, my_dimension\nFROM "sampleDB"."sampleTable" ORDER BY time DESC LIMIT 3\n""")\n\n```\n\n## At scale\nAWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.\n\nThe quickest way to get started is to use AWS Glue with Ray. Read our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/) to learn about it, then head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/release-3.0.0/tutorials) to discover even more features.\n\n### Installation\n```\npip install "awswrangler[modin,ray]==3.0.0rc3"\n```\n\nAs a result existing scripts can run on significantly larger datasets with no code rewrite. Supported APIs are parallelized across cores on a single machine or across multiple nodes on a cluster in the cloud.\n\n### Supported APIs\n\n<p align="center">\n\n| Service         | API                      | Implementation |\n|-----------------|--------------------------|:--------------:|\n| `S3`            | `read_parquet`           |       ✅        |\n|                 | `read_parquet_metadata`  |       ✅        |\n|                 | `read_parquet_table`     |       ✅        |\n|                 | `read_csv`               |       ✅        |\n|                 | `read_json`              |       ✅        |\n|                 | `read_fwf`               |       ✅        |\n|                 | `to_parquet`             |       ✅        |\n|                 | `to_csv`                 |       ✅        |\n|                 | `to_json`                |       ✅        |\n|                 | `select_query`           |       ✅        |\n|                 | `store_parquet_metadata` |       ✅        |\n|                 | `delete_objects`         |       ✅        |\n|                 | `describe_objects`       |       ✅        |\n|                 | `size_objects`           |       ✅        |\n|                 | `wait_objects_exist`     |       ✅        |\n|                 | `wait_objects_not_exist` |       ✅        |\n|                 | `merge_datasets`         |       ✅        |\n|                 | `copy_objects`           |       ✅        |\n| `Redshift`      | `copy`                   |       ✅        |\n|                 | `unload`                 |       ✅        |\n| `Athena`        | `read_sql_query`         |       ✅        |\n|                 | `read_sql_table`         |       ✅        |\n|                 | `describe_table`         |       ✅        |\n|                 | `get_query_results`      |       ✅        |\n|                 | `show_create_table`      |       ✅        |\n| `DynamoDB`      | `read_items`             |       ✅        |\n| `LakeFormation` | `read_sql_query`         |       ✅        |\n|                 | `read_sql_table`         |       ✅        |\n| `Timestream`    | `write`                  |       ✅        |\n</p>\n\n## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)\n\n- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/what.html)\n- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html)\n  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#pypi-pip)\n  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#conda)\n  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-lambda-layer)\n  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-python-shell-jobs)\n  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-pyspark-jobs)\n  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook)\n  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook-lifecycle)\n  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#emr)\n  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#from-source)\n- [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)\n  - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)\n  - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)\n  - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)\n  - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)\n  - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)\n  - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)\n  - [007 - Databases (Redshift, MySQL, PostgreSQL, SQL Server and Oracle)](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/007%20-%20Redshift%2C%20MySQL%2C%20PostgreSQL%2C%20SQL%20Server%2C%20Oracle.ipynb)\n  - [008 - Redshift - Copy & Unload.ipynb](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/008%20-%20Redshift%20-%20Copy%20%26%20Unload.ipynb)\n  - [009 - Redshift - Append, Overwrite and Upsert](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/009%20-%20Redshift%20-%20Append%2C%20Overwrite%2C%20Upsert.ipynb)\n  - [010 - Parquet Crawler](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/010%20-%20Parquet%20Crawler.ipynb)\n  - [011 - CSV Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/011%20-%20CSV%20Datasets.ipynb)\n  - [012 - CSV Crawler](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/012%20-%20CSV%20Crawler.ipynb)\n  - [013 - Merging Datasets on S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/013%20-%20Merging%20Datasets%20on%20S3.ipynb)\n  - [014 - Schema Evolution](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/014%20-%20Schema%20Evolution.ipynb)\n  - [015 - EMR](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/015%20-%20EMR.ipynb)\n  - [016 - EMR & Docker](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/016%20-%20EMR%20%26%20Docker.ipynb)\n  - [017 - Partition Projection](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/017%20-%20Partition%20Projection.ipynb)\n  - [018 - QuickSight](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/018%20-%20QuickSight.ipynb)\n  - [019 - Athena Cache](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/019%20-%20Athena%20Cache.ipynb)\n  - [020 - Spark Table Interoperability](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/020%20-%20Spark%20Table%20Interoperability.ipynb)\n  - [021 - Global Configurations](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/021%20-%20Global%20Configurations.ipynb)\n  - [022 - Writing Partitions Concurrently](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/022%20-%20Writing%20Partitions%20Concurrently.ipynb)\n  - [023 - Flexible Partitions Filter](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/023%20-%20Flexible%20Partitions%20Filter.ipynb)\n  - [024 - Athena Query Metadata](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/024%20-%20Athena%20Query%20Metadata.ipynb)\n  - [025 - Redshift - Loading Parquet files with Spectrum](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/025%20-%20Redshift%20-%20Loading%20Parquet%20files%20with%20Spectrum.ipynb)\n  - [026 - Amazon Timestream](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/026%20-%20Amazon%20Timestream.ipynb)\n  - [027 - Amazon Timestream 2](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/027%20-%20Amazon%20Timestream%202.ipynb)\n  - [028 - Amazon DynamoDB](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/028%20-%20DynamoDB.ipynb)\n  - [029 - S3 Select](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/029%20-%20S3%20Select.ipynb)\n  - [030 - Data Api](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/030%20-%20Data%20Api.ipynb)\n  - [031 - OpenSearch](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/031%20-%20OpenSearch.ipynb)\n  - [032 - Lake Formation Governed Tables](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/032%20-%20Lake%20Formation%20Governed%20Tables.ipynb)\n  - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)\n  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)\n  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)\n  - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)\n  - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)\n  - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)\n- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html)\n  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-s3)\n  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-glue-catalog)\n  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-athena)\n  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-lake-formation)\n  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-redshift)\n  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#postgresql)\n  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#mysql)\n  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#sqlserver)\n  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#oracle)\n  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-redshift)\n  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-rds)\n  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#opensearch)\n  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-neptune)\n  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#dynamodb)\n  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-timestream)\n  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-emr)\n  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-cloudwatch-logs)\n  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-chime)\n  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-quicksight)\n  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-sts)\n  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-secrets-manager)\n  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#global-configurations)\n- [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)\n- [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)\n\n## Getting Help\n\nThe best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...\nYou may also find help on these community resources:\n* The #aws-sdk-pandas Slack [channel](https://join.slack.com/t/aws-sdk-pandas/shared_invite/zt-sxdx38sl-E0coRfAds8WdpxXD2Nzfrg)\n* Ask a question on [Stack Overflow](https://stackoverflow.com/questions/tagged/awswrangler)\n  and tag it with `awswrangler`\n\n## Community Resources\n\nPlease [send a Pull Request](https://github.com/aws/aws-sdk-pandas/edit/main/README.md) with your resource reference and @githubhandle.\n\n- [Optimize Python ETL by extending Pandas with AWS SDK for pandas](https://aws.amazon.com/blogs/big-data/optimize-python-etl-by-extending-pandas-with-aws-data-wrangler/) [[@igorborgest](https://github.com/igorborgest)]\n- [Reading Parquet Files With AWS Lambda](https://aprakash.wordpress.com/2020/04/14/reading-parquet-files-with-aws-lambda/) [[@anand086](https://github.com/anand086)]\n- [Transform AWS CloudTrail data using AWS SDK for pandas](https://aprakash.wordpress.com/2020/09/17/transform-aws-cloudtrail-data-using-aws-data-wrangler/) [[@anand086](https://github.com/anand086)]\n- [Rename Glue Tables using AWS SDK for pandas](https://ananddatastories.com/rename-glue-tables-using-aws-sdk-pandas/) [[@anand086](https://github.com/anand086)]\n- [Getting started on AWS SDK for pandas and Athena](https://medium.com/@dheerajsharmainampudi/getting-started-on-aws-sdk-pandas-and-athena-7b446c834076) [[@dheerajsharma21](https://github.com/dheerajsharma21)]\n- [Simplifying Pandas integration with AWS data related services](https://medium.com/@bv_subhash/aws-sdk-pandas-simplifying-pandas-integration-with-aws-data-related-services-2b3325c12188) [[@bvsubhash](https://github.com/bvsubhash)]\n- [Build an ETL pipeline using AWS S3, Glue and Athena](https://www.linkedin.com/pulse/build-etl-pipeline-using-aws-s3-glue-athena-data-wrangler-tom-reid/) [[@taupirho](https://github.com/taupirho)]\n\n## Logging\n\nEnabling internal logging examples:\n\n```py3\nimport logging\nlogging.basicConfig(level=logging.INFO, format="[%(name)s][%(funcName)s] %(message)s")\nlogging.getLogger("awswrangler").setLevel(logging.DEBUG)\nlogging.getLogger("botocore.credentials").setLevel(logging.CRITICAL)\n```\n\nInto AWS lambda:\n\n```py3\nimport logging\nlogging.getLogger("awswrangler").setLevel(logging.DEBUG)\n```\n\n## Who uses AWS SDK for pandas?\n\nKnowing which companies are using this library is important to help prioritize the project internally.\nIf you would like us to include your company’s name and/or logo in the README file to indicate that your company is using the AWS SDK for pandas, please raise a "Support Us" issue. If you would like us to display your company’s logo, please raise a linked pull request to provide an image file for the logo. Note that by raising a Support Us issue (and related pull request), you are granting AWS permission to use your company’s name (and logo) for the limited purpose described here and you are confirming that you have authority to grant such permission.\n\n- [Amazon](https://www.amazon.com/)\n- [AWS](https://aws.amazon.com/)\n- [Cepsa](https://cepsa.com) [[@alvaropc](https://github.com/alvaropc)]\n- [Cognitivo](https://www.cognitivo.ai/) [[@msantino](https://github.com/msantino)]\n- [Digio](https://www.digio.com.br/) [[@afonsomy](https://github.com/afonsomy)]\n- [DNX](https://www.dnx.solutions/) [[@DNXLabs](https://github.com/DNXLabs)]\n- [Fortescue Future Industries](https://ffi.com.au/) [[@spencervoorend](https://github.com/spencervoorend)]\n- [Funcional Health Tech](https://www.funcionalcorp.com.br/) [[@webysther](https://github.com/webysther)]\n- [Funding Circle](https://www.fundingcircle.com/) [[@pfig](https://github.com/pfig)]\n- [Infomach](https://www.infomach.com.br/)\n- [Informa Markets](https://www.informamarkets.com/en/home.html) [[@mateusmorato]](http://github.com/mateusmorato)\n- [LINE TV](https://www.linetv.tw/) [[@bryanyang0528](https://github.com/bryanyang0528)]\n- [Magnataur](https://magnataur.com) [[@brianmingus2](https://github.com/brianmingus2)]\n- [M4U](https://www.m4u.com.br/) [[@Thiago-Dantas](https://github.com/Thiago-Dantas)]\n- [NBCUniversal](https://www.nbcuniversal.com/) [[@vibe](https://github.com/vibe)]\n- [nrd.io](https://nrd.io/) [[@mrtns](https://github.com/mrtns)]\n- [OKRA Technologies](https://okra.ai) [[@JPFrancoia](https://github.com/JPFrancoia), [@schot](https://github.com/schot)]\n- [Pier](https://www.pier.digital/) [[@flaviomax](https://github.com/flaviomax)]\n- [Pismo](https://www.pismo.io/) [[@msantino](https://github.com/msantino)]\n- [ringDNA](https://www.ringdna.com/) [[@msropp](https://github.com/msropp)]\n- [Serasa Experian](https://www.serasaexperian.com.br/) [[@andre-marcos-perez](https://github.com/andre-marcos-perez)]\n- [Shipwell](https://shipwell.com/) [[@zacharycarter](https://github.com/zacharycarter)]\n- [strongDM](https://www.strongdm.com/) [[@mrtns](https://github.com/mrtns)]\n- [Thinkbumblebee](https://www.thinkbumblebee.com/) [[@dheerajsharma21]](https://github.com/dheerajsharma21)\n- [VTEX](https://vtex.com/us-en/) [[@igorborgest]](https://github.com/igorborgest)\n- [Zillow](https://www.zillow.com/) [[@nicholas-miles]](https://github.com/nicholas-miles)\n',
-    'author': 'Amazon Web Services',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://aws-sdk-pandas.readthedocs.io/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
+# AWS SDK for pandas (awswrangler)
 
+AWS Data Wrangler is now **AWS SDK for pandas (awswrangler)**.  We’re changing the name we use when we talk about the library, but everything else will stay the same.  You’ll still be able to install using `pip install awswrangler` and you won’t need to change any of your code.  As part of this change, we’ve moved the library from AWS Labs to the main AWS GitHub organisation but, thanks to the GitHub’s redirect feature, you’ll still be able to access the project by its old URLs until you update your bookmarks.  Our documentation has also moved to [aws-sdk-pandas.readthedocs.io](https://aws-sdk-pandas.readthedocs.io), but old bookmarks will redirect to the new site.
+
+*Pandas on AWS*
+
+Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
+
+![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
+![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
+
+> An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
+
+[![Release](https://img.shields.io/badge/3.1.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
+[![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
+
+| Source | Downloads | Installation Command |
+|--------|-----------|----------------------|
+| **[PyPi](https://pypi.org/project/awswrangler/)**  | [![PyPI Downloads](https://pepy.tech/badge/awswrangler)](https://pypi.org/project/awswrangler/) | `pip install awswrangler` |
+| **[Conda](https://anaconda.org/conda-forge/awswrangler)** | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/awswrangler.svg)](https://anaconda.org/conda-forge/awswrangler) | `conda install -c conda-forge awswrangler` |
+
+> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>
+➡️`pip install 'awswrangler[redshift]'`
+
+Powered By [<img src="https://arrow.apache.org/img/arrow.png" width="200">](https://arrow.apache.org/powered_by/)
+
+## Table of contents
+
+- [Quick Start](#quick-start)
+- [At Scale](#at-scale)
+- [Read The Docs](#read-the-docs)
+- [Getting Help](#getting-help)
+- [Community Resources](#community-resources)
+- [Logging](#logging)
+- [Who uses AWS SDK for pandas?](#who-uses-aws-sdk-for-pandas)
+
+## Quick Start
+
+Installation command: `pip install awswrangler`
+
+> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>
+➡️`pip install 'awswrangler[redshift]'`
+
+```py3
+import awswrangler as wr
+import pandas as pd
+from datetime import datetime
+
+df = pd.DataFrame({"id": [1, 2], "value": ["foo", "boo"]})
+
+# Storing data on Data Lake
+wr.s3.to_parquet(
+    df=df,
+    path="s3://bucket/dataset/",
+    dataset=True,
+    database="my_db",
+    table="my_table"
+)
+
+# Retrieving the data directly from Amazon S3
+df = wr.s3.read_parquet("s3://bucket/dataset/", dataset=True)
+
+# Retrieving the data from Amazon Athena
+df = wr.athena.read_sql_query("SELECT * FROM my_table", database="my_db")
+
+# Get a Redshift connection from Glue Catalog and retrieving data from Redshift Spectrum
+con = wr.redshift.connect("my-glue-connection")
+df = wr.redshift.read_sql_query("SELECT * FROM external_schema.my_table", con=con)
+con.close()
+
+# Amazon Timestream Write
+df = pd.DataFrame({
+    "time": [datetime.now(), datetime.now()],   
+    "my_dimension": ["foo", "boo"],
+    "measure": [1.0, 1.1],
+})
+rejected_records = wr.timestream.write(df,
+    database="sampleDB",
+    table="sampleTable",
+    time_col="time",
+    measure_col="measure",
+    dimensions_cols=["my_dimension"],
+)
+
+# Amazon Timestream Query
+wr.timestream.query("""
+SELECT time, measure_value::double, my_dimension
+FROM "sampleDB"."sampleTable" ORDER BY time DESC LIMIT 3
+""")
+
+```
+
+## At scale
+AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
+
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
+
+## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
+
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#resources)
+- [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
+  - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
+  - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
+  - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
+  - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
+  - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
+  - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
+  - [007 - Databases (Redshift, MySQL, PostgreSQL, SQL Server and Oracle)](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/007%20-%20Redshift%2C%20MySQL%2C%20PostgreSQL%2C%20SQL%20Server%2C%20Oracle.ipynb)
+  - [008 - Redshift - Copy & Unload.ipynb](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/008%20-%20Redshift%20-%20Copy%20%26%20Unload.ipynb)
+  - [009 - Redshift - Append, Overwrite and Upsert](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/009%20-%20Redshift%20-%20Append%2C%20Overwrite%2C%20Upsert.ipynb)
+  - [010 - Parquet Crawler](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/010%20-%20Parquet%20Crawler.ipynb)
+  - [011 - CSV Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/011%20-%20CSV%20Datasets.ipynb)
+  - [012 - CSV Crawler](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/012%20-%20CSV%20Crawler.ipynb)
+  - [013 - Merging Datasets on S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/013%20-%20Merging%20Datasets%20on%20S3.ipynb)
+  - [014 - Schema Evolution](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/014%20-%20Schema%20Evolution.ipynb)
+  - [015 - EMR](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/015%20-%20EMR.ipynb)
+  - [016 - EMR & Docker](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/016%20-%20EMR%20%26%20Docker.ipynb)
+  - [017 - Partition Projection](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/017%20-%20Partition%20Projection.ipynb)
+  - [018 - QuickSight](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/018%20-%20QuickSight.ipynb)
+  - [019 - Athena Cache](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/019%20-%20Athena%20Cache.ipynb)
+  - [020 - Spark Table Interoperability](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/020%20-%20Spark%20Table%20Interoperability.ipynb)
+  - [021 - Global Configurations](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/021%20-%20Global%20Configurations.ipynb)
+  - [022 - Writing Partitions Concurrently](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/022%20-%20Writing%20Partitions%20Concurrently.ipynb)
+  - [023 - Flexible Partitions Filter](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/023%20-%20Flexible%20Partitions%20Filter.ipynb)
+  - [024 - Athena Query Metadata](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/024%20-%20Athena%20Query%20Metadata.ipynb)
+  - [025 - Redshift - Loading Parquet files with Spectrum](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/025%20-%20Redshift%20-%20Loading%20Parquet%20files%20with%20Spectrum.ipynb)
+  - [026 - Amazon Timestream](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/026%20-%20Amazon%20Timestream.ipynb)
+  - [027 - Amazon Timestream 2](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/027%20-%20Amazon%20Timestream%202.ipynb)
+  - [028 - Amazon DynamoDB](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/028%20-%20DynamoDB.ipynb)
+  - [029 - S3 Select](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/029%20-%20S3%20Select.ipynb)
+  - [030 - Data Api](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/030%20-%20Data%20Api.ipynb)
+  - [031 - OpenSearch](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/031%20-%20OpenSearch.ipynb)
+  - [032 - Lake Formation Governed Tables](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/032%20-%20Lake%20Formation%20Governed%20Tables.ipynb)
+  - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
+  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
+  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
+  - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
+  - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
+  - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
+  - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#distributed-ray)
+- [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
+- [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
+
+## Getting Help
+
+The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
+You may also find help on these community resources:
+* The #aws-sdk-pandas Slack [channel](https://join.slack.com/t/aws-sdk-pandas/shared_invite/zt-sxdx38sl-E0coRfAds8WdpxXD2Nzfrg)
+* Ask a question on [Stack Overflow](https://stackoverflow.com/questions/tagged/awswrangler)
+  and tag it with `awswrangler`
+* [Runbook](https://github.com/aws/aws-sdk-pandas/discussions/1815) for AWS SDK for pandas with Ray
+
+## Community Resources
+
+Please [send a Pull Request](https://github.com/aws/aws-sdk-pandas/edit/main/README.md) with your resource reference and @githubhandle.
+
+- [Optimize Python ETL by extending Pandas with AWS SDK for pandas](https://aws.amazon.com/blogs/big-data/optimize-python-etl-by-extending-pandas-with-aws-data-wrangler/) [[@igorborgest](https://github.com/igorborgest)]
+- [Reading Parquet Files With AWS Lambda](https://aprakash.wordpress.com/2020/04/14/reading-parquet-files-with-aws-lambda/) [[@anand086](https://github.com/anand086)]
+- [Transform AWS CloudTrail data using AWS SDK for pandas](https://aprakash.wordpress.com/2020/09/17/transform-aws-cloudtrail-data-using-aws-data-wrangler/) [[@anand086](https://github.com/anand086)]
+- [Rename Glue Tables using AWS SDK for pandas](https://ananddatastories.com/rename-glue-tables-using-aws-sdk-pandas/) [[@anand086](https://github.com/anand086)]
+- [Getting started on AWS SDK for pandas and Athena](https://medium.com/@dheerajsharmainampudi/getting-started-on-aws-sdk-pandas-and-athena-7b446c834076) [[@dheerajsharma21](https://github.com/dheerajsharma21)]
+- [Simplifying Pandas integration with AWS data related services](https://medium.com/@bv_subhash/aws-sdk-pandas-simplifying-pandas-integration-with-aws-data-related-services-2b3325c12188) [[@bvsubhash](https://github.com/bvsubhash)]
+- [Build an ETL pipeline using AWS S3, Glue and Athena](https://www.linkedin.com/pulse/build-etl-pipeline-using-aws-s3-glue-athena-data-wrangler-tom-reid/) [[@taupirho](https://github.com/taupirho)]
+
+## Logging
+
+Enabling internal logging examples:
+
+```py3
+import logging
+logging.basicConfig(level=logging.INFO, format="[%(name)s][%(funcName)s] %(message)s")
+logging.getLogger("awswrangler").setLevel(logging.DEBUG)
+logging.getLogger("botocore.credentials").setLevel(logging.CRITICAL)
+```
+
+Into AWS lambda:
+
+```py3
+import logging
+logging.getLogger("awswrangler").setLevel(logging.DEBUG)
+```
+
+## Who uses AWS SDK for pandas?
+
+Knowing which companies are using this library is important to help prioritize the project internally.
+If you would like us to include your company’s name and/or logo in the README file to indicate that your company is using the AWS SDK for pandas, please raise a "Support Us" issue. If you would like us to display your company’s logo, please raise a linked pull request to provide an image file for the logo. Note that by raising a Support Us issue (and related pull request), you are granting AWS permission to use your company’s name (and logo) for the limited purpose described here and you are confirming that you have authority to grant such permission.
+
+- [Amazon](https://www.amazon.com/)
+- [AWS](https://aws.amazon.com/)
+- [Cepsa](https://cepsa.com) [[@alvaropc](https://github.com/alvaropc)]
+- [Cognitivo](https://www.cognitivo.ai/) [[@msantino](https://github.com/msantino)]
+- [Digio](https://www.digio.com.br/) [[@afonsomy](https://github.com/afonsomy)]
+- [DNX](https://www.dnx.solutions/) [[@DNXLabs](https://github.com/DNXLabs)]
+- [Fortescue Future Industries](https://ffi.com.au/) [[@spencervoorend](https://github.com/spencervoorend)]
+- [Funcional Health Tech](https://www.funcionalcorp.com.br/) [[@webysther](https://github.com/webysther)]
+- [Funding Circle](https://www.fundingcircle.com/) [[@pfig](https://github.com/pfig)]
+- [Infomach](https://www.infomach.com.br/)
+- [Informa Markets](https://www.informamarkets.com/en/home.html) [[@mateusmorato]](http://github.com/mateusmorato)
+- [LINE TV](https://www.linetv.tw/) [[@bryanyang0528](https://github.com/bryanyang0528)]
+- [Magnataur](https://magnataur.com) [[@brianmingus2](https://github.com/brianmingus2)]
+- [M4U](https://www.m4u.com.br/) [[@Thiago-Dantas](https://github.com/Thiago-Dantas)]
+- [NBCUniversal](https://www.nbcuniversal.com/) [[@vibe](https://github.com/vibe)]
+- [nrd.io](https://nrd.io/) [[@mrtns](https://github.com/mrtns)]
+- [OKRA Technologies](https://okra.ai) [[@JPFrancoia](https://github.com/JPFrancoia), [@schot](https://github.com/schot)]
+- [Pier](https://www.pier.digital/) [[@flaviomax](https://github.com/flaviomax)]
+- [Pismo](https://www.pismo.io/) [[@msantino](https://github.com/msantino)]
+- [ringDNA](https://www.ringdna.com/) [[@msropp](https://github.com/msropp)]
+- [Serasa Experian](https://www.serasaexperian.com.br/) [[@andre-marcos-perez](https://github.com/andre-marcos-perez)]
+- [Shipwell](https://shipwell.com/) [[@zacharycarter](https://github.com/zacharycarter)]
+- [strongDM](https://www.strongdm.com/) [[@mrtns](https://github.com/mrtns)]
+- [Thinkbumblebee](https://www.thinkbumblebee.com/) [[@dheerajsharma21]](https://github.com/dheerajsharma21)
+- [VTEX](https://vtex.com/us-en/) [[@igorborgest]](https://github.com/igorborgest)
+- [Zillow](https://www.zillow.com/) [[@nicholas-miles]](https://github.com/nicholas-miles)
 
-setup(**setup_kwargs)
```

