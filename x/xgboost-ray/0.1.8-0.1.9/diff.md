# Comparing `tmp/xgboost_ray-0.1.8-py3-none-any.whl.zip` & `tmp/xgboost_ray-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,79 +1,106 @@
-Zip file size: 138434 bytes, number of entries: 77
--rw-r--r--  2.0 unx        0 b- defN 21-Jul-16 22:31 examples/__init__.py
--rw-r--r--  2.0 unx      255 b- defN 21-Jul-16 22:31 examples/create_test_data.py
--rw-r--r--  2.0 unx     2124 b- defN 22-Feb-24 02:28 examples/higgs.py
--rw-r--r--  2.0 unx     3304 b- defN 22-Feb-24 02:28 examples/higgs_parquet.py
--rw-r--r--  2.0 unx     2793 b- defN 21-Jul-16 22:31 examples/readme.py
--rw-r--r--  2.0 unx     1278 b- defN 21-Jul-16 22:31 examples/readme_sklearn_api.py
--rw-r--r--  2.0 unx     2298 b- defN 21-Jul-16 22:31 examples/simple.py
--rw-r--r--  2.0 unx     2806 b- defN 21-Jul-16 22:31 examples/simple_dask.py
--rw-r--r--  2.0 unx     2882 b- defN 21-Jul-16 22:31 examples/simple_modin.py
--rw-r--r--  2.0 unx     2458 b- defN 21-Sep-08 01:21 examples/simple_objectstore.py
--rw-r--r--  2.0 unx     3849 b- defN 22-Feb-24 02:28 examples/simple_partitioned.py
--rw-r--r--  2.0 unx      820 b- defN 21-Sep-08 01:21 examples/simple_predict.py
--rw-r--r--  2.0 unx     2904 b- defN 22-Feb-24 02:28 examples/simple_ray_dataset.py
--rw-r--r--  2.0 unx     3357 b- defN 21-Jul-16 22:31 examples/simple_tune.py
--rw-r--r--  2.0 unx     1837 b- defN 21-Jul-16 22:31 examples/train_on_test_data.py
--rw-r--r--  2.0 unx     1917 b- defN 21-Jul-16 22:31 examples/train_with_ml_dataset.py
--rw-r--r--  2.0 unx      689 b- defN 22-Feb-24 02:28 xgboost_ray/__init__.py
--rw-r--r--  2.0 unx     3671 b- defN 21-Sep-24 04:24 xgboost_ray/callback.py
--rw-r--r--  2.0 unx     5871 b- defN 22-Feb-24 02:28 xgboost_ray/elastic.py
--rw-r--r--  2.0 unx    62730 b- defN 22-Feb-24 02:28 xgboost_ray/main.py
--rw-r--r--  2.0 unx    38910 b- defN 22-Feb-24 02:28 xgboost_ray/matrix.py
--rw-r--r--  2.0 unx     1902 b- defN 21-Sep-24 04:24 xgboost_ray/session.py
--rw-r--r--  2.0 unx    39699 b- defN 22-Feb-24 02:28 xgboost_ray/sklearn.py
--rw-r--r--  2.0 unx    10270 b- defN 21-Sep-24 04:24 xgboost_ray/tune.py
--rw-r--r--  2.0 unx     5586 b- defN 21-Sep-24 04:24 xgboost_ray/util.py
--rw-r--r--  2.0 unx      179 b- defN 21-Sep-24 04:24 xgboost_ray/xgb.py
--rw-r--r--  2.0 unx     1576 b- defN 21-Sep-24 04:24 xgboost_ray/compat/__init__.py
--rw-r--r--  2.0 unx    12396 b- defN 21-Jul-16 22:31 xgboost_ray/compat/tracker.py
--rw-r--r--  2.0 unx      973 b- defN 22-Feb-24 02:28 xgboost_ray/data_sources/__init__.py
--rw-r--r--  2.0 unx     4788 b- defN 21-Jul-16 22:31 xgboost_ray/data_sources/_distributed.py
--rw-r--r--  2.0 unx     1515 b- defN 21-Jul-16 22:31 xgboost_ray/data_sources/csv.py
--rw-r--r--  2.0 unx     5592 b- defN 22-Feb-24 02:28 xgboost_ray/data_sources/dask.py
--rw-r--r--  2.0 unx     4902 b- defN 21-Sep-24 04:24 xgboost_ray/data_sources/data_source.py
--rw-r--r--  2.0 unx     2687 b- defN 22-Feb-24 02:28 xgboost_ray/data_sources/ml_dataset.py
--rw-r--r--  2.0 unx     4284 b- defN 21-Jul-16 22:31 xgboost_ray/data_sources/modin.py
--rw-r--r--  2.0 unx     1136 b- defN 21-Sep-24 04:24 xgboost_ray/data_sources/numpy.py
--rw-r--r--  2.0 unx     1275 b- defN 21-Sep-08 01:21 xgboost_ray/data_sources/object_store.py
--rw-r--r--  2.0 unx      807 b- defN 21-Jul-16 22:31 xgboost_ray/data_sources/pandas.py
--rw-r--r--  2.0 unx     1533 b- defN 21-Jul-16 22:31 xgboost_ray/data_sources/parquet.py
--rw-r--r--  2.0 unx     3779 b- defN 22-Feb-24 02:28 xgboost_ray/data_sources/partitioned.py
--rw-r--r--  2.0 unx     2720 b- defN 21-Jul-16 22:31 xgboost_ray/data_sources/petastorm.py
--rw-r--r--  2.0 unx     3868 b- defN 22-Feb-24 02:28 xgboost_ray/data_sources/ray_dataset.py
--rw-r--r--  2.0 unx        0 b- defN 21-Jul-16 22:31 xgboost_ray/examples/__init__.py
--rw-r--r--  2.0 unx      255 b- defN 21-Jul-16 22:31 xgboost_ray/examples/create_test_data.py
--rw-r--r--  2.0 unx     2124 b- defN 22-Feb-24 02:28 xgboost_ray/examples/higgs.py
--rw-r--r--  2.0 unx     3304 b- defN 22-Feb-24 02:28 xgboost_ray/examples/higgs_parquet.py
--rw-r--r--  2.0 unx     2793 b- defN 21-Jul-16 22:31 xgboost_ray/examples/readme.py
--rw-r--r--  2.0 unx     1278 b- defN 21-Jul-16 22:31 xgboost_ray/examples/readme_sklearn_api.py
--rw-r--r--  2.0 unx     2298 b- defN 21-Jul-16 22:31 xgboost_ray/examples/simple.py
--rw-r--r--  2.0 unx     2806 b- defN 21-Jul-16 22:31 xgboost_ray/examples/simple_dask.py
--rw-r--r--  2.0 unx     2882 b- defN 21-Jul-16 22:31 xgboost_ray/examples/simple_modin.py
--rw-r--r--  2.0 unx     2458 b- defN 21-Sep-08 01:21 xgboost_ray/examples/simple_objectstore.py
--rw-r--r--  2.0 unx     3849 b- defN 22-Feb-24 02:28 xgboost_ray/examples/simple_partitioned.py
--rw-r--r--  2.0 unx      820 b- defN 21-Sep-08 01:21 xgboost_ray/examples/simple_predict.py
--rw-r--r--  2.0 unx     2904 b- defN 22-Feb-24 02:28 xgboost_ray/examples/simple_ray_dataset.py
--rw-r--r--  2.0 unx     3357 b- defN 21-Jul-16 22:31 xgboost_ray/examples/simple_tune.py
--rw-r--r--  2.0 unx     1837 b- defN 21-Jul-16 22:31 xgboost_ray/examples/train_on_test_data.py
--rw-r--r--  2.0 unx     1917 b- defN 21-Jul-16 22:31 xgboost_ray/examples/train_with_ml_dataset.py
--rw-r--r--  2.0 unx        0 b- defN 21-Jul-16 22:31 xgboost_ray/tests/__init__.py
--rw-r--r--  2.0 unx     2123 b- defN 21-Jul-16 22:31 xgboost_ray/tests/conftest.py
--rw-r--r--  2.0 unx     4215 b- defN 21-Jul-16 22:31 xgboost_ray/tests/fault_tolerance.py
--rw-r--r--  2.0 unx     1789 b- defN 21-Sep-08 01:21 xgboost_ray/tests/test_client.py
--rw-r--r--  2.0 unx     7403 b- defN 22-Feb-24 02:28 xgboost_ray/tests/test_colocation.py
--rw-r--r--  2.0 unx    26926 b- defN 22-Feb-24 02:28 xgboost_ray/tests/test_data_source.py
--rw-r--r--  2.0 unx    13826 b- defN 22-Feb-24 02:28 xgboost_ray/tests/test_end_to_end.py
--rw-r--r--  2.0 unx    21810 b- defN 22-Feb-24 02:28 xgboost_ray/tests/test_fault_tolerance.py
--rw-r--r--  2.0 unx    13772 b- defN 22-Feb-24 02:28 xgboost_ray/tests/test_matrix.py
--rw-r--r--  2.0 unx    45758 b- defN 22-Feb-24 02:28 xgboost_ray/tests/test_sklearn.py
--rw-r--r--  2.0 unx     5535 b- defN 22-Feb-24 02:28 xgboost_ray/tests/test_sklearn_matrix.py
--rw-r--r--  2.0 unx     5894 b- defN 21-Jul-16 22:31 xgboost_ray/tests/test_tune.py
--rw-r--r--  2.0 unx     5499 b- defN 21-Jul-16 22:31 xgboost_ray/tests/test_xgboost_api.py
--rw-r--r--  2.0 unx     6969 b- defN 21-Jul-16 22:31 xgboost_ray/tests/utils.py
--rw-r--r--  2.0 unx    15673 b- defN 22-Feb-24 23:27 xgboost_ray-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      463 b- defN 22-Feb-24 23:27 xgboost_ray-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Feb-24 23:27 xgboost_ray-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 22-Feb-24 23:27 xgboost_ray-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6752 b- defN 22-Feb-24 23:27 xgboost_ray-0.1.8.dist-info/RECORD
-77 files, 477622 bytes uncompressed, 127704 bytes compressed:  73.3%
+Zip file size: 230633 bytes, number of entries: 104
+-rw-rw-r--  2.0 unx        0 b- defN 21-Jun-17 12:56 examples/__init__.py
+-rw-rw-r--  2.0 unx      255 b- defN 21-Oct-07 15:16 examples/create_test_data.py
+-rw-rw-r--  2.0 unx     2124 b- defN 22-Jan-20 17:43 examples/higgs.py
+-rw-rw-r--  2.0 unx     3304 b- defN 22-Feb-02 21:01 examples/higgs_parquet.py
+-rw-rw-r--  2.0 unx     2793 b- defN 21-Oct-07 15:16 examples/readme.py
+-rw-rw-r--  2.0 unx     1278 b- defN 21-Jun-25 13:49 examples/readme_sklearn_api.py
+-rw-rw-r--  2.0 unx     2298 b- defN 21-Jun-17 12:56 examples/simple.py
+-rw-rw-r--  2.0 unx     2806 b- defN 21-Jun-17 12:56 examples/simple_dask.py
+-rw-rw-r--  2.0 unx     2882 b- defN 21-Jun-17 12:56 examples/simple_modin.py
+-rw-rw-r--  2.0 unx     2458 b- defN 21-Jul-26 14:57 examples/simple_objectstore.py
+-rw-rw-r--  2.0 unx     3849 b- defN 21-Oct-14 15:00 examples/simple_partitioned.py
+-rw-rw-r--  2.0 unx      820 b- defN 21-Aug-29 23:55 examples/simple_predict.py
+-rw-rw-r--  2.0 unx     2904 b- defN 22-Feb-08 16:58 examples/simple_ray_dataset.py
+-rw-rw-r--  2.0 unx     3357 b- defN 22-Mar-17 17:19 examples/simple_tune.py
+-rw-rw-r--  2.0 unx     1837 b- defN 21-Jun-17 12:56 examples/train_on_test_data.py
+-rw-rw-r--  2.0 unx     1917 b- defN 21-Jun-17 12:56 examples/train_with_ml_dataset.py
+-rw-rw-r--  2.0 unx      689 b- defN 22-Mar-02 21:00 xgboost_ray/__init__.py
+-rw-rw-r--  2.0 unx     3671 b- defN 21-Oct-13 14:37 xgboost_ray/callback.py
+-rw-rw-r--  2.0 unx     5871 b- defN 21-Oct-29 11:43 xgboost_ray/elastic.py
+-rw-rw-r--  2.0 unx    63072 b- defN 22-May-23 18:36 xgboost_ray/main.py
+-rw-rw-r--  2.0 unx    38468 b- defN 22-May-23 18:36 xgboost_ray/matrix.py
+-rw-rw-r--  2.0 unx     1902 b- defN 21-Oct-13 14:37 xgboost_ray/session.py
+-rw-rw-r--  2.0 unx    40321 b- defN 22-May-23 18:36 xgboost_ray/sklearn.py
+-rw-rw-r--  2.0 unx     5874 b- defN 22-May-23 18:36 xgboost_ray/tune.py
+-rw-rw-r--  2.0 unx     3045 b- defN 22-May-23 18:36 xgboost_ray/util.py
+-rw-rw-r--  2.0 unx      179 b- defN 21-Oct-13 14:37 xgboost_ray/xgb.py
+-rw-rw-r--  2.0 unx      794 b- defN 22-Feb-16 18:30 xgboost_ray/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     4930 b- defN 22-Feb-16 18:30 xgboost_ray/__pycache__/callback.cpython-38.pyc
+-rw-rw-r--  2.0 unx    45444 b- defN 22-Feb-16 18:30 xgboost_ray/__pycache__/main.cpython-38.pyc
+-rw-rw-r--  2.0 unx    29525 b- defN 22-Feb-16 18:30 xgboost_ray/__pycache__/matrix.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2604 b- defN 22-Feb-16 18:30 xgboost_ray/__pycache__/session.cpython-38.pyc
+-rw-rw-r--  2.0 unx    23303 b- defN 22-Feb-16 18:30 xgboost_ray/__pycache__/sklearn.cpython-38.pyc
+-rw-rw-r--  2.0 unx     8277 b- defN 22-Feb-16 18:30 xgboost_ray/__pycache__/tune.cpython-38.pyc
+-rw-rw-r--  2.0 unx     7320 b- defN 22-Feb-16 18:30 xgboost_ray/__pycache__/util.cpython-38.pyc
+-rw-rw-r--  2.0 unx      296 b- defN 22-Feb-16 18:30 xgboost_ray/__pycache__/xgb.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1576 b- defN 21-Oct-13 14:37 xgboost_ray/compat/__init__.py
+-rw-rw-r--  2.0 unx    12396 b- defN 21-Aug-29 23:39 xgboost_ray/compat/tracker.py
+-rw-rw-r--  2.0 unx     1538 b- defN 22-Feb-16 18:30 xgboost_ray/compat/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     9713 b- defN 22-Feb-16 18:32 xgboost_ray/compat/__pycache__/tracker.cpython-38.pyc
+-rw-rw-r--  2.0 unx      887 b- defN 22-May-23 18:36 xgboost_ray/data_sources/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 21-Jun-03 17:18 xgboost_ray/data_sources/_distributed.py
+-rw-rw-r--  2.0 unx     1515 b- defN 21-Oct-07 15:16 xgboost_ray/data_sources/csv.py
+-rw-rw-r--  2.0 unx     5592 b- defN 21-Oct-14 15:00 xgboost_ray/data_sources/dask.py
+-rw-rw-r--  2.0 unx     4887 b- defN 22-May-23 18:36 xgboost_ray/data_sources/data_source.py
+-rw-rw-r--  2.0 unx     4284 b- defN 21-Oct-07 15:16 xgboost_ray/data_sources/modin.py
+-rw-rw-r--  2.0 unx     1136 b- defN 21-Oct-13 14:37 xgboost_ray/data_sources/numpy.py
+-rw-rw-r--  2.0 unx     1275 b- defN 21-Oct-07 15:16 xgboost_ray/data_sources/object_store.py
+-rw-rw-r--  2.0 unx      807 b- defN 21-Oct-07 15:16 xgboost_ray/data_sources/pandas.py
+-rw-rw-r--  2.0 unx     1533 b- defN 21-Oct-07 15:16 xgboost_ray/data_sources/parquet.py
+-rw-rw-r--  2.0 unx     3779 b- defN 21-Oct-14 15:00 xgboost_ray/data_sources/partitioned.py
+-rw-rw-r--  2.0 unx     2720 b- defN 21-Oct-07 15:16 xgboost_ray/data_sources/petastorm.py
+-rw-rw-r--  2.0 unx     3868 b- defN 22-Feb-01 16:44 xgboost_ray/data_sources/ray_dataset.py
+-rw-rw-r--  2.0 unx     1164 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3685 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/_distributed.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1805 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/csv.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5258 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/dask.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5598 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/data_source.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3080 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/ml_dataset.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3925 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/modin.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1722 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/numpy.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1955 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/object_store.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1156 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/pandas.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1854 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/parquet.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3756 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/partitioned.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3222 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/petastorm.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3674 b- defN 22-Feb-16 18:30 xgboost_ray/data_sources/__pycache__/ray_dataset.cpython-38.pyc
+-rw-rw-r--  2.0 unx        0 b- defN 21-Jun-17 12:56 xgboost_ray/examples/__init__.py
+-rw-rw-r--  2.0 unx      255 b- defN 21-Oct-07 15:16 xgboost_ray/examples/create_test_data.py
+-rw-rw-r--  2.0 unx     2124 b- defN 22-Jan-20 17:43 xgboost_ray/examples/higgs.py
+-rw-rw-r--  2.0 unx     3304 b- defN 22-Feb-02 21:01 xgboost_ray/examples/higgs_parquet.py
+-rw-rw-r--  2.0 unx     2793 b- defN 21-Oct-07 15:16 xgboost_ray/examples/readme.py
+-rw-rw-r--  2.0 unx     1278 b- defN 21-Jun-25 13:49 xgboost_ray/examples/readme_sklearn_api.py
+-rw-rw-r--  2.0 unx     2298 b- defN 21-Jun-17 12:56 xgboost_ray/examples/simple.py
+-rw-rw-r--  2.0 unx     2806 b- defN 21-Jun-17 12:56 xgboost_ray/examples/simple_dask.py
+-rw-rw-r--  2.0 unx     2882 b- defN 21-Jun-17 12:56 xgboost_ray/examples/simple_modin.py
+-rw-rw-r--  2.0 unx     2458 b- defN 21-Jul-26 14:57 xgboost_ray/examples/simple_objectstore.py
+-rw-rw-r--  2.0 unx     3849 b- defN 21-Oct-14 15:00 xgboost_ray/examples/simple_partitioned.py
+-rw-rw-r--  2.0 unx      820 b- defN 21-Aug-29 23:55 xgboost_ray/examples/simple_predict.py
+-rw-rw-r--  2.0 unx     2904 b- defN 22-Feb-08 16:58 xgboost_ray/examples/simple_ray_dataset.py
+-rw-rw-r--  2.0 unx     3357 b- defN 22-Mar-17 17:19 xgboost_ray/examples/simple_tune.py
+-rw-rw-r--  2.0 unx     1837 b- defN 21-Jun-17 12:56 xgboost_ray/examples/train_on_test_data.py
+-rw-rw-r--  2.0 unx     1917 b- defN 21-Jun-17 12:56 xgboost_ray/examples/train_with_ml_dataset.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Jun-03 17:18 xgboost_ray/tests/__init__.py
+-rw-rw-r--  2.0 unx     2123 b- defN 21-Jun-03 17:18 xgboost_ray/tests/conftest.py
+-rw-rw-r--  2.0 unx     4215 b- defN 21-Jun-17 12:56 xgboost_ray/tests/fault_tolerance.py
+-rw-rw-r--  2.0 unx     1789 b- defN 21-Aug-09 20:51 xgboost_ray/tests/test_client.py
+-rw-rw-r--  2.0 unx     7427 b- defN 22-May-23 18:36 xgboost_ray/tests/test_colocation.py
+-rw-rw-r--  2.0 unx    26926 b- defN 22-Feb-08 16:58 xgboost_ray/tests/test_data_source.py
+-rw-rw-r--  2.0 unx    13826 b- defN 22-Feb-08 16:58 xgboost_ray/tests/test_end_to_end.py
+-rw-rw-r--  2.0 unx    21810 b- defN 21-Oct-29 11:43 xgboost_ray/tests/test_fault_tolerance.py
+-rw-rw-r--  2.0 unx    12415 b- defN 22-May-23 18:36 xgboost_ray/tests/test_matrix.py
+-rw-rw-r--  2.0 unx    46288 b- defN 22-Apr-19 19:42 xgboost_ray/tests/test_sklearn.py
+-rw-rw-r--  2.0 unx     5602 b- defN 22-Apr-19 12:14 xgboost_ray/tests/test_sklearn_matrix.py
+-rw-rw-r--  2.0 unx     5991 b- defN 22-Apr-08 20:03 xgboost_ray/tests/test_tune.py
+-rw-rw-r--  2.0 unx     5499 b- defN 21-Jun-03 17:18 xgboost_ray/tests/test_xgboost_api.py
+-rw-rw-r--  2.0 unx     6969 b- defN 21-Oct-07 15:16 xgboost_ray/tests/utils.py
+-rw-rw-r--  2.0 unx      155 b- defN 22-Feb-16 18:30 xgboost_ray/tests/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1820 b- defN 22-Feb-16 18:30 xgboost_ray/tests/__pycache__/conftest.cpython-38-pytest-6.2.4.pyc
+-rw-rw-r--  2.0 unx    13218 b- defN 22-Feb-16 18:31 xgboost_ray/tests/__pycache__/test_matrix.cpython-38-pytest-6.2.4.pyc
+-rw-rw-r--  2.0 unx    15673 b- defN 22-May-23 18:38 xgboost_ray-0.1.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      464 b- defN 22-May-23 18:38 xgboost_ray-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-May-23 18:38 xgboost_ray-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       21 b- defN 22-May-23 18:38 xgboost_ray-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9792 b- defN 22-May-23 18:38 xgboost_ray-0.1.9.dist-info/RECORD
+104 files, 661612 bytes uncompressed, 214849 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -72,20 +72,53 @@
 
 Filename: xgboost_ray/util.py
 Comment: 
 
 Filename: xgboost_ray/xgb.py
 Comment: 
 
+Filename: xgboost_ray/__pycache__/__init__.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/__pycache__/callback.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/__pycache__/main.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/__pycache__/matrix.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/__pycache__/session.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/__pycache__/sklearn.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/__pycache__/tune.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/__pycache__/util.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/__pycache__/xgb.cpython-38.pyc
+Comment: 
+
 Filename: xgboost_ray/compat/__init__.py
 Comment: 
 
 Filename: xgboost_ray/compat/tracker.py
 Comment: 
 
+Filename: xgboost_ray/compat/__pycache__/__init__.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/compat/__pycache__/tracker.cpython-38.pyc
+Comment: 
+
 Filename: xgboost_ray/data_sources/__init__.py
 Comment: 
 
 Filename: xgboost_ray/data_sources/_distributed.py
 Comment: 
 
 Filename: xgboost_ray/data_sources/csv.py
@@ -93,17 +126,14 @@
 
 Filename: xgboost_ray/data_sources/dask.py
 Comment: 
 
 Filename: xgboost_ray/data_sources/data_source.py
 Comment: 
 
-Filename: xgboost_ray/data_sources/ml_dataset.py
-Comment: 
-
 Filename: xgboost_ray/data_sources/modin.py
 Comment: 
 
 Filename: xgboost_ray/data_sources/numpy.py
 Comment: 
 
 Filename: xgboost_ray/data_sources/object_store.py
@@ -120,14 +150,56 @@
 
 Filename: xgboost_ray/data_sources/petastorm.py
 Comment: 
 
 Filename: xgboost_ray/data_sources/ray_dataset.py
 Comment: 
 
+Filename: xgboost_ray/data_sources/__pycache__/__init__.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/_distributed.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/csv.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/dask.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/data_source.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/ml_dataset.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/modin.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/numpy.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/object_store.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/pandas.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/parquet.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/partitioned.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/petastorm.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/data_sources/__pycache__/ray_dataset.cpython-38.pyc
+Comment: 
+
 Filename: xgboost_ray/examples/__init__.py
 Comment: 
 
 Filename: xgboost_ray/examples/create_test_data.py
 Comment: 
 
 Filename: xgboost_ray/examples/higgs.py
@@ -210,23 +282,32 @@
 
 Filename: xgboost_ray/tests/test_xgboost_api.py
 Comment: 
 
 Filename: xgboost_ray/tests/utils.py
 Comment: 
 
-Filename: xgboost_ray-0.1.8.dist-info/LICENSE
+Filename: xgboost_ray/tests/__pycache__/__init__.cpython-38.pyc
+Comment: 
+
+Filename: xgboost_ray/tests/__pycache__/conftest.cpython-38-pytest-6.2.4.pyc
+Comment: 
+
+Filename: xgboost_ray/tests/__pycache__/test_matrix.cpython-38-pytest-6.2.4.pyc
+Comment: 
+
+Filename: xgboost_ray-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: xgboost_ray-0.1.8.dist-info/METADATA
+Filename: xgboost_ray-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xgboost_ray-0.1.8.dist-info/WHEEL
+Filename: xgboost_ray-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xgboost_ray-0.1.8.dist-info/top_level.txt
+Filename: xgboost_ray-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xgboost_ray-0.1.8.dist-info/RECORD
+Filename: xgboost_ray-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xgboost_ray/__init__.py

```diff
@@ -5,15 +5,15 @@
 # workaround for legacy xgboost==0.9.0
 try:
     from xgboost_ray.sklearn import RayXGBClassifier, RayXGBRegressor, \
         RayXGBRFClassifier, RayXGBRFRegressor, RayXGBRanker
 except ImportError:
     pass
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 __all__ = [
     "__version__", "RayParams", "RayDMatrix", "RayDeviceQuantileDMatrix",
     "RayFileType", "RayShardingMode", "Data", "combine_data", "train",
     "predict", "RayXGBClassifier", "RayXGBRegressor", "RayXGBRFClassifier",
     "RayXGBRFRegressor", "RayXGBRanker"
 ]
```

## xgboost_ray/main.py

```diff
@@ -1,19 +1,19 @@
+import platform
 from typing import Tuple, Dict, Any, List, Optional, Callable, Union, Sequence
 from dataclasses import dataclass, field
 from distutils.version import LooseVersion
 
 import functools
 import multiprocessing
 import os
 import pickle
 import time
 import threading
 import warnings
-import re
 import inspect
 
 import numpy as np
 import pandas as pd
 
 from xgboost_ray.xgb import xgboost as xgb
 from xgboost.core import XGBoostError
@@ -34,23 +34,19 @@
     from ray import logger
     from ray.exceptions import RayActorError, RayTaskError
     from ray.actor import ActorHandle
     from ray.util import get_node_ip_address, placement_group
     from ray.util.annotations import PublicAPI, DeveloperAPI
     from ray.util.placement_group import PlacementGroup, \
         remove_placement_group, get_current_placement_group
+    from ray.util.queue import Queue
 
-    from xgboost_ray.util import Event, Queue, MultiActorTask, \
-        force_on_current_node
+    from xgboost_ray.util import Event, MultiActorTask, force_on_current_node
 
-    if LooseVersion(ray.__version__) >= LooseVersion("1.5.0"):
-        # https://github.com/ray-project/ray/pull/16437
-        DEFAULT_PG = "default"
-    else:
-        DEFAULT_PG = None
+    DEFAULT_PG = "default"
 
     RAY_INSTALLED = True
 except ImportError:
     ray = get_node_ip_address = Queue = Event = ActorHandle = logger = None
 
     def PublicAPI(f):
         @functools.wraps(f)
@@ -59,15 +55,15 @@
 
         return inner_f
 
     DeveloperAPI = PublicAPI
     RAY_INSTALLED = False
 
 from xgboost_ray.tune import _try_add_tune_callback, _get_tune_resources, \
-    TUNE_USING_PG, is_session_enabled
+    is_session_enabled
 
 from xgboost_ray.matrix import RayDMatrix, combine_data, \
     RayDeviceQuantileDMatrix, RayDataIter, concat_dataframes, \
     LEGACY_MATRIX
 from xgboost_ray.session import init_session, put_queue, \
     set_session_queue
 
@@ -127,17 +123,16 @@
 LEGACY_WARNING = (
     f"You are using `xgboost_ray` with a legacy XGBoost version "
     f"(version {xgboost_version}). While we try to support "
     f"older XGBoost versions, please note that this library is only "
     f"fully tested and supported for XGBoost >= 1.4. Please consider "
     f"upgrading your XGBoost version (`pip install -U xgboost`).")
 
-# XGBoost version as an int tuple for comparisions
-XGBOOST_VERSION_TUPLE = tuple(
-    int(x) for x in re.sub(r"[^\.0-9]", "", xgboost_version).split("."))
+# XGBoost LooseVersion for comparisions
+XGBOOST_LOOSE_VERSION = LooseVersion(xgboost_version)
 
 
 class RayXGBoostTrainingError(RuntimeError):
     """Raised from RayXGBoostActor.train() when the local xgb.train function
     did not complete."""
     pass
 
@@ -846,15 +841,15 @@
 
 
 def _create_communication_processes(added_tune_callback: bool = False):
     # Create Queue and Event actors and make sure to colocate with driver node.
     node_ip = get_node_ip_address()
     # Have to explicitly set num_cpus to 0.
     placement_option = {"num_cpus": 0}
-    if added_tune_callback and TUNE_USING_PG:
+    if added_tune_callback:
         # If Tune is using placement groups, then we force Queue and
         # StopEvent onto same bundle as the Trainable.
         # This forces all 3 to be on the same node.
         current_pg = get_current_placement_group()
         if current_pg is None:
             # This means the user is not using Tune PGs after all -
             # e.g. via setting an environment variable.
@@ -1074,18 +1069,27 @@
 
     # Failure handling loop. Here we wait until all training tasks finished.
     # If a training task fails, we stop training on the remaining actors,
     # check which ones are still alive, and raise the error.
     # The train() wrapper function will then handle the error.
     start_wait = time.time()
     last_status = start_wait
+
+    # When the number of trees/dataset size is very small,
+    # training can be too fast and finish before the queue Actor
+    # gets to process the calls it has recieved. This is a very rare edge
+    # case, but it can show up in CI.
+    # In order to mitigate, if the queue has not been handled before,
+    # we simply wait a moment before checking it one last time.
+    has_queue_been_handled = False
     try:
         not_ready = training_futures
         while not_ready:
             if _training_state.queue:
+                has_queue_been_handled = True
                 _handle_queue(
                     queue=_training_state.queue,
                     checkpoint=_training_state.checkpoint,
                     callback_returns=callback_returns)
 
             if ray_params.elastic_training \
                     and not ENV.ELASTIC_RESTART_DISABLED:
@@ -1107,14 +1111,16 @@
                 last_status = time.time()
 
             ready, not_ready = ray.wait(
                 not_ready, num_returns=len(not_ready), timeout=1)
             ray.get(ready)
 
         # Get items from queue one last time
+        if not has_queue_been_handled:
+            time.sleep(1)
         if _training_state.queue:
             _handle_queue(
                 queue=_training_state.queue,
                 checkpoint=_training_state.checkpoint,
                 callback_returns=callback_returns)
 
     # The inner loop should catch all exceptions
@@ -1215,14 +1221,18 @@
         **kwargs: Keyword arguments will be passed to the local
             `xgb.train()` calls.
 
     Returns: An ``xgboost.Booster`` object.
     """
     os.environ.setdefault("RAY_IGNORE_UNHANDLED_ERRORS", "1")
 
+    if platform.system() == "Windows":
+        raise RuntimeError("xgboost-ray training currently does not support "
+                           "Windows.")
+
     if xgb is None:
         raise ImportError(
             "xgboost package is not installed. XGBoost-Ray WILL NOT WORK. "
             "FIX THIS by running `pip install \"xgboost-ray\"`.")
 
     if _remote is None:
         _remote = _is_client_connected() and \
@@ -1370,20 +1380,17 @@
 
     # Create the Queue and Event actors.
     queue, stop_event = _create_communication_processes(added_tune_callback)
 
     placement_strategy = None
     if not ray_params.elastic_training:
         if added_tune_callback:
-            if TUNE_USING_PG:
-                # If Tune is using placement groups, then strategy has already
-                # been set. Don't create an additional placement_group here.
-                placement_strategy = None
-            else:
-                placement_strategy = "PACK"
+            # Tune is using placement groups, so the strategy has already
+            # been set. Don't create an additional placement_group here.
+            placement_strategy = None
         elif bool(ENV.USE_SPREAD_STRATEGY):
             placement_strategy = "SPREAD"
 
     if placement_strategy is not None:
         pg = _create_placement_group(cpus_per_actor, gpus_per_actor,
                                      ray_params.resources_per_actor,
                                      ray_params.num_actors, placement_strategy)
```

## xgboost_ray/matrix.py

```diff
@@ -16,23 +16,17 @@
 
 import os
 
 import ray
 from ray import logger
 from ray.util.annotations import PublicAPI, DeveloperAPI
 
-from xgboost_ray.util import Unavailable
 from xgboost_ray.data_sources import DataSource, data_sources, RayFileType
 
 try:
-    from ray.util.data import MLDataset
-except ImportError:
-    MLDataset = Unavailable
-
-try:
     from ray.data.dataset import Dataset as RayDataset
 except (ImportError, ModuleNotFoundError):
 
     class RayDataset:
         pass
 
 
@@ -42,15 +36,15 @@
 except ImportError:
     DataIter = object
     LEGACY_MATRIX = True
 
 if TYPE_CHECKING:
     from xgboost_ray.xgb import xgboost as xgb
 
-Data = Union[str, List[str], np.ndarray, pd.DataFrame, pd.Series, MLDataset]
+Data = Union[str, List[str], np.ndarray, pd.DataFrame, pd.Series]
 
 
 def concat_dataframes(dfs: List[Optional[pd.DataFrame]]):
     filtered = [df for df in dfs if df is not None]
     return pd.concat(filtered, ignore_index=True, copy=False)
 
 
@@ -400,15 +394,15 @@
             elif os.path.exists(self.data):
                 self.data = [self.data]
             else:
                 invalid_data = True
 
         # Todo (krfricke): It would be good to have a more general way to
         # check for compatibility here. Combine with test below?
-        if not (isinstance(self.data, (Iterable, MLDataset, RayDataset))
+        if not (isinstance(self.data, (Iterable, RayDataset))
                 or hasattr(self.data, "__partitioned__")) or invalid_data:
             raise ValueError(
                 f"Distributed data loading only works with already "
                 f"distributed datasets. These should be specified through a "
                 f"list of locations (or a single string). "
                 f"Got: {type(self.data)}."
                 f"\nFIX THIS by passing a list of files (e.g. on S3) to the "
@@ -440,15 +434,15 @@
 
         if not data_source:
             raise ValueError(
                 f"Invalid data source type: {type(self.data)} "
                 f"with FileType: {self.filetype} for a distributed dataset."
                 "\nFIX THIS by passing a supported data type. Supported "
                 "data types for distributed datasets are a list of "
-                "CSV or Parquet sources as well as Ray MLDatasets. If using "
+                "CSV or Parquet sources. If using "
                 "Modin, Dask, or Petastorm, make sure the library is "
                 "installed.")
 
         self.data_source = data_source
         self._cached_n = data_source.get_n(self.data)
         return self.data_source
 
@@ -582,15 +576,15 @@
     dataframes according to the actor rank.
 
     The total number of actors has to remain constant and cannot be changed
     once it has been set.
 
     Args:
         data: Data object. Can be a pandas dataframe, pandas series,
-            numpy array, Ray MLDataset, modin dataframe, string pointing to
+            numpy array, modin dataframe, string pointing to
             a csv or parquet file, or list of strings pointing to csv or
             parquet files.
         label: Optional label object. Can be a pandas series, numpy array,
             modin series, string pointing to a csv or parquet file, or
             a string indicating the column of the data dataframe that
             contains the label. If this is not a string it must be of the
             same type as the data argument.
@@ -870,21 +864,18 @@
         data_dict.pop("label_lower_bound", None)
         data_dict.pop("label_upper_bound", None)
         return data_dict
 
 
 def _can_load_distributed(source: Data) -> bool:
     """Returns True if it might be possible to use distributed data loading"""
-    from xgboost_ray.data_sources.ml_dataset import MLDataset
     from xgboost_ray.data_sources.modin import Modin
 
     if isinstance(source, (int, float, bool)):
         return False
-    elif MLDataset.is_data_type(source):
-        return True
     elif Modin.is_data_type(source):
         return True
     elif isinstance(source, str):
         # Strings should point to files or URLs
         # Usually parquet files point to directories
         return source.endswith(".parquet")
     elif isinstance(source, Sequence):
@@ -898,20 +889,17 @@
 
     # Per default, allow distributed loading.
     return True
 
 
 def _detect_distributed(source: Data) -> bool:
     """Returns True if we should try to use distributed data loading"""
-    from xgboost_ray.data_sources.ml_dataset import MLDataset
     from xgboost_ray.data_sources.modin import Modin
     if not _can_load_distributed(source):
         return False
-    if MLDataset.is_data_type(source):
-        return True
     if Modin.is_data_type(source):
         return True
     if isinstance(source, Iterable) and not isinstance(source, str) and \
        not (isinstance(source, Sequence) and isinstance(source[0], str)):
         # This is an iterable but not a Sequence of strings, and not a
         # pandas dataframe, series, or numpy array.
         # Detect False per default, can be overridden by passing
```

## xgboost_ray/sklearn.py

```diff
@@ -21,24 +21,25 @@
 # File based on:
 # https://github.com/dmlc/xgboost/blob/c6a0bdbb5a68232cd59ea556c981c633cc0646ca/python-package/xgboost/sklearn.py
 
 # License:
 # https://github.com/dmlc/xgboost/blob/c6a0bdbb5a68232cd59ea556c981c633cc0646ca/LICENSE
 
 from typing import Callable, Tuple, Dict, Optional, Union, Any, List
+from distutils.version import LooseVersion
 
 import numpy as np
 
 import warnings
 import functools
 import inspect
 
 from ray.util.annotations import PublicAPI, DeveloperAPI
 
-from xgboost_ray.main import (RayParams, train, predict, XGBOOST_VERSION_TUPLE,
+from xgboost_ray.main import (RayParams, train, predict, XGBOOST_LOOSE_VERSION,
                               LEGACY_WARNING)
 from xgboost_ray.matrix import RayDMatrix
 
 from xgboost import Booster, __version__ as xgboost_version
 from xgboost.sklearn import (XGBModel, XGBClassifier, XGBRegressor,
                              XGBRFClassifier, XGBRFRegressor, XGBRanker,
                              _objective_decorator)
@@ -54,14 +55,16 @@
         @functools.wraps(f)
         def inner_f(*args, **kwargs):
             return f(*args, **kwargs)
 
         return inner_f
 
 
+# If _wrap_evaluation_matrices has new arguments added in xgboost, update
+# RayXGBMixin._ray_get_wrap_evaluation_matrices_compat_kwargs
 try:
     from xgboost.sklearn import _wrap_evaluation_matrices
 except ImportError:
     # copied from the file in the top comment
     def _wrap_evaluation_matrices(
             missing: float,
             X: Any,
@@ -209,15 +212,16 @@
 )
 
 
 def _treat_estimator_doc(doc: str) -> str:
     """Helper function to make nececssary changes in estimator docstrings"""
     doc = doc.replace(*_N_JOBS_DOC_REPLACE).replace(
         "scikit-learn API for XGBoost",
-        "scikit-learn API for Ray-distributed XGBoost")
+        "scikit-learn API for Ray-distributed XGBoost").replace(
+            ":doc:`tree method\n        </treemethod>`", "tree method")
     return doc
 
 
 def _treat_X_doc(doc: str) -> str:
     doc = doc.replace("Data to predict with.",
                       "Data to predict with. Can also be a ``RayDMatrix``.")
     doc = doc.replace("Feature matrix.",
@@ -228,15 +232,15 @@
 
 
 def _xgboost_version_warn(f):
     """Decorator to warn when xgboost version is < 1.4.0"""
 
     @functools.wraps(f)
     def inner_f(*args, **kwargs):
-        if XGBOOST_VERSION_TUPLE < (1, 4, 0):
+        if XGBOOST_LOOSE_VERSION < LooseVersion("1.4.0"):
             warnings.warn(LEGACY_WARNING)
         return f(*args, **kwargs)
 
     return inner_f
 
 
 def _check_if_params_are_ray_dmatrix(X,
@@ -352,21 +356,28 @@
             _remote=_remote,
             **compat_predict_kwargs,
         )
 
     def _ray_get_wrap_evaluation_matrices_compat_kwargs(
             self, label_transform=None) -> dict:
         ret = {}
-        if "label_transform" in inspect.signature(
-                _wrap_evaluation_matrices).parameters:
+        wrap_evaluation_matrices_parameters = inspect.signature(
+            _wrap_evaluation_matrices).parameters
+        if "label_transform" in wrap_evaluation_matrices_parameters:
             # XGBoost < 1.6.0
             identity_func = lambda x: x  # noqa
             ret["label_transform"] = label_transform or identity_func
-        if hasattr(self, "enable_categorical"):
+        if hasattr(
+                self, "enable_categorical"
+        ) and "enable_categorical" in wrap_evaluation_matrices_parameters:
             ret["enable_categorical"] = self.enable_categorical
+        if hasattr(
+                self, "feature_types"
+        ) and "feature_types" in wrap_evaluation_matrices_parameters:
+            ret["feature_types"] = self.feature_types
         return ret
 
     # copied from the file in the top comment
     # provided here for compatibility with legacy xgboost versions
     # will be overwritten by vanilla xgboost if possible
     def _configure_fit(
             self,
```

## xgboost_ray/tune.py

```diff
@@ -1,25 +1,18 @@
 # Tune imports.
-import os
-from typing import Dict, Union, List, Optional
+from typing import Dict, Optional
 
 import ray
 
-try:
-    from typing import OrderedDict
-except ImportError:
-    from collections import OrderedDict
-
 import logging
 
 from ray.util.annotations import PublicAPI
 
 from xgboost_ray.xgb import xgboost as xgb
 
-from xgboost_ray.compat import TrainingCallback
 from xgboost_ray.session import put_queue, get_rabit_rank
 from xgboost_ray.util import Unavailable, force_on_current_node
 
 try:
     from ray import tune
     from ray.tune import is_session_enabled
     from ray.tune.utils import flatten_dict
@@ -38,98 +31,15 @@
 
     def is_session_enabled():
         return False
 
     flatten_dict = is_session_enabled
     TUNE_INSTALLED = False
 
-# Todo(krfricke): Remove after next ray core release
-if not hasattr(OrigTuneReportCallback, "_get_report_dict") or not issubclass(
-        OrigTuneReportCallback, TrainingCallback):
-    TUNE_LEGACY = True
-else:
-    TUNE_LEGACY = False
-
-# Todo(amogkam): Remove after Ray 1.3 release.
-try:
-    from ray.tune import PlacementGroupFactory
-
-    TUNE_USING_PG = True
-except ImportError:
-    TUNE_USING_PG = False
-    PlacementGroupFactory = Unavailable
-
-if TUNE_LEGACY and TUNE_INSTALLED:
-    # Until the next release, keep compatible callbacks here.
-    class TuneReportCallback(OrigTuneReportCallback, TrainingCallback):
-        def _get_report_dict(self, evals_log):
-            if isinstance(evals_log, OrderedDict):
-                # xgboost>=1.3
-                result_dict = flatten_dict(evals_log, delimiter="-")
-                for k in list(result_dict):
-                    result_dict[k] = result_dict[k][0]
-            else:
-                # xgboost<1.3
-                result_dict = dict(evals_log)
-            if not self._metrics:
-                report_dict = result_dict
-            else:
-                report_dict = {}
-                for key in self._metrics:
-                    if isinstance(self._metrics, dict):
-                        metric = self._metrics[key]
-                    else:
-                        metric = key
-                    report_dict[key] = result_dict[metric]
-            return report_dict
-
-        def after_iteration(self, model, epoch: int, evals_log: Dict):
-            if get_rabit_rank() == 0:
-                report_dict = self._get_report_dict(evals_log)
-                put_queue(lambda: tune.report(**report_dict))
-
-    class _TuneCheckpointCallback(_OrigTuneCheckpointCallback,
-                                  TrainingCallback):
-        def __init__(self, filename: str, frequency: int):
-            super(_TuneCheckpointCallback, self).__init__(filename)
-            self._frequency = frequency
-
-        @staticmethod
-        def _create_checkpoint(model, epoch: int, filename: str,
-                               frequency: int):
-            if epoch % frequency > 0:
-                return
-            with tune.checkpoint_dir(step=epoch) as checkpoint_dir:
-                model.save_model(os.path.join(checkpoint_dir, filename))
-
-        def after_iteration(self, model, epoch: int, evals_log: Dict):
-            if get_rabit_rank() == 0:
-                put_queue(lambda: self._create_checkpoint(
-                    model, epoch, self._filename, self._frequency))
-
-    class TuneReportCheckpointCallback(OrigTuneReportCheckpointCallback,
-                                       TrainingCallback):
-        _checkpoint_callback_cls = _TuneCheckpointCallback
-        _report_callbacks_cls = TuneReportCallback
-
-        def __init__(
-                self,
-                metrics: Union[None, str, List[str], Dict[str, str]] = None,
-                filename: str = "checkpoint",
-                frequency: int = 5):
-            self._checkpoint = self._checkpoint_callback_cls(
-                filename, frequency)
-            self._report = self._report_callbacks_cls(metrics)
-
-        def after_iteration(self, model, epoch: int, evals_log: Dict):
-            if get_rabit_rank() == 0:
-                self._checkpoint.after_iteration(model, epoch, evals_log)
-                self._report.after_iteration(model, epoch, evals_log)
-
-elif TUNE_INSTALLED:
+if TUNE_INSTALLED:
     # New style callbacks.
     class TuneReportCallback(OrigTuneReportCallback):
         def after_iteration(self, model, epoch: int, evals_log: Dict):
             if get_rabit_rank() == 0:
                 report_dict = self._get_report_dict(evals_log)
                 put_queue(lambda: tune.report(**report_dict))
 
@@ -164,23 +74,18 @@
                 new_callbacks.append(replace_cb)
                 logging.warning(
                     REPLACE_MSG.format(
                         orig="ray.tune.integration.xgboost.TuneReportCallback",
                         target="xgboost_ray.tune.TuneReportCallback"))
                 has_tune_callback = True
             elif isinstance(cb, OrigTuneReportCheckpointCallback):
-                if TUNE_LEGACY:
-                    replace_cb = TuneReportCheckpointCallback(
-                        metrics=cb._report._metrics,
-                        filename=cb._checkpoint._filename)
-                else:
-                    replace_cb = TuneReportCheckpointCallback(
-                        metrics=cb._report._metrics,
-                        filename=cb._checkpoint._filename,
-                        frequency=cb._checkpoint._frequency)
+                replace_cb = TuneReportCheckpointCallback(
+                    metrics=cb._report._metrics,
+                    filename=cb._checkpoint._filename,
+                    frequency=cb._checkpoint._frequency)
                 new_callbacks.append(replace_cb)
                 logging.warning(
                     REPLACE_MSG.format(
                         orig="ray.tune.integration.xgboost."
                         "TuneReportCheckpointCallback",
                         target="xgboost_ray.tune.TuneReportCheckpointCallback")
                 )
@@ -199,43 +104,29 @@
 
 
 def _get_tune_resources(num_actors: int, cpus_per_actor: int,
                         gpus_per_actor: int,
                         resources_per_actor: Optional[Dict]):
     """Returns object to use for ``resources_per_trial`` with Ray Tune."""
     if TUNE_INSTALLED:
-        if not TUNE_USING_PG:
-            resources_per_actor = {} if not resources_per_actor \
-                else resources_per_actor
-            extra_custom_resources = {
-                k: v * num_actors
-                for k, v in resources_per_actor.items()
-            }
-            return dict(
-                cpu=1,
-                extra_cpu=cpus_per_actor * num_actors,
-                extra_gpu=gpus_per_actor * num_actors,
-                extra_custom_resources=extra_custom_resources,
-            )
-        else:
-            from ray.tune import PlacementGroupFactory
-
-            head_bundle = {"CPU": 1}
-            child_bundle = {"CPU": cpus_per_actor, "GPU": gpus_per_actor}
-            child_bundle_extra = {} if resources_per_actor is None else \
-                resources_per_actor
-            child_bundles = [{
-                **child_bundle,
-                **child_bundle_extra
-            } for _ in range(num_actors)]
-            bundles = [head_bundle] + child_bundles
-            placement_group_factory = PlacementGroupFactory(
-                bundles, strategy="PACK")
+        from ray.tune import PlacementGroupFactory
+
+        head_bundle = {"CPU": 1}
+        child_bundle = {"CPU": cpus_per_actor, "GPU": gpus_per_actor}
+        child_bundle_extra = {} if resources_per_actor is None else \
+            resources_per_actor
+        child_bundles = [{
+            **child_bundle,
+            **child_bundle_extra
+        } for _ in range(num_actors)]
+        bundles = [head_bundle] + child_bundles
+        placement_group_factory = PlacementGroupFactory(
+            bundles, strategy="PACK")
 
-            return placement_group_factory
+        return placement_group_factory
     else:
         raise RuntimeError("Tune is not installed, so `get_tune_resources` is "
                            "not supported. You can install Ray Tune via `pip "
                            "install ray[tune]`.")
 
 
 @PublicAPI(stability="beta")
```

## xgboost_ray/util.py

```diff
@@ -1,14 +1,13 @@
 from typing import Dict, Optional, List
 
 import asyncio
 
 import ray
 from ray.util.annotations import DeveloperAPI
-from ray.util.queue import Queue as RayQueue, Empty, Full
 
 
 @DeveloperAPI
 class Unavailable:
     """No object should be instance of this class"""
 
     def __init__(self):
@@ -46,86 +45,14 @@
 
     def shutdown(self):
         if self.actor:
             ray.kill(self.actor)
         self.actor = None
 
 
-# Remove after Ray 1.2 release.
-if getattr(RayQueue, "shutdown", None) is not None:
-    from ray.util.queue import _QueueActor
-else:
-    # Have to copy the class here so that we can subclass this for mocking.
-    # If we have the @ray.remote decorator, then we can't subclass it.
-    class _QueueActor:
-        def __init__(self, maxsize):
-            self.maxsize = maxsize
-            self.queue = asyncio.Queue(self.maxsize)
-
-        def qsize(self):
-            return self.queue.qsize()
-
-        def empty(self):
-            return self.queue.empty()
-
-        def full(self):
-            return self.queue.full()
-
-        async def put(self, item, timeout=None):
-            try:
-                await asyncio.wait_for(self.queue.put(item), timeout)
-            except asyncio.TimeoutError:
-                raise Full
-
-        async def get(self, timeout=None):
-            try:
-                return await asyncio.wait_for(self.queue.get(), timeout)
-            except asyncio.TimeoutError:
-                raise Empty
-
-        def put_nowait(self, item):
-            self.queue.put_nowait(item)
-
-        def put_nowait_batch(self, items):
-            # If maxsize is 0, queue is unbounded, so no need to check size.
-            if self.maxsize > 0 and len(items) + self.qsize() > self.maxsize:
-                raise Full(f"Cannot add {len(items)} items to queue of size "
-                           f"{self.qsize()} and maxsize {self.maxsize}.")
-            for item in items:
-                self.queue.put_nowait(item)
-
-        def get_nowait(self):
-            return self.queue.get_nowait()
-
-        def get_nowait_batch(self, num_items):
-            if num_items > self.qsize():
-                raise Empty(f"Cannot get {num_items} items from queue of size "
-                            f"{self.qsize()}.")
-            return [self.queue.get_nowait() for _ in range(num_items)]
-
-
-# Remove after Ray 1.2 release.
-@DeveloperAPI
-class Queue(RayQueue):
-    def __init__(self, maxsize: int = 0,
-                 actor_options: Optional[Dict] = None) -> None:
-        actor_options = actor_options or {}
-        self.maxsize = maxsize
-        self.actor = ray.remote(_QueueActor).options(**actor_options).remote(
-            self.maxsize)
-
-    def shutdown(self):
-        if getattr(RayQueue, "shutdown", None) is not None:
-            super(Queue, self).shutdown()
-        else:
-            if self.actor:
-                ray.kill(self.actor)
-            self.actor = None
-
-
 @DeveloperAPI
 class MultiActorTask:
     """Utility class to hold multiple futures.
 
     The `is_ready()` method will return True once all futures are ready.
 
     Args:
```

## xgboost_ray/data_sources/__init__.py

```diff
@@ -1,23 +1,21 @@
 from xgboost_ray.data_sources.data_source import DataSource, RayFileType
 from xgboost_ray.data_sources.numpy import Numpy
 from xgboost_ray.data_sources.pandas import Pandas
 from xgboost_ray.data_sources.modin import Modin
 from xgboost_ray.data_sources.dask import Dask
-from xgboost_ray.data_sources.ml_dataset import MLDataset
 from xgboost_ray.data_sources.petastorm import Petastorm
 from xgboost_ray.data_sources.csv import CSV
 from xgboost_ray.data_sources.parquet import Parquet
 from xgboost_ray.data_sources.object_store import ObjectStore
 from xgboost_ray.data_sources.ray_dataset import RayDataset
 from xgboost_ray.data_sources.partitioned import Partitioned
 
 data_sources = [
-    Numpy, Pandas, Partitioned, Modin, Dask, MLDataset, Petastorm, CSV,
-    Parquet, ObjectStore, RayDataset
+    Numpy, Pandas, Partitioned, Modin, Dask, Petastorm, CSV, Parquet,
+    ObjectStore, RayDataset
 ]
 
 __all__ = [
     "DataSource", "RayFileType", "Numpy", "Pandas", "Modin", "Dask",
-    "MLDataset", "Petastorm", "CSV", "Parquet", "ObjectStore", "RayDataset",
-    "Partitioned"
+    "Petastorm", "CSV", "Parquet", "ObjectStore", "RayDataset", "Partitioned"
 ]
```

## xgboost_ray/data_sources/data_source.py

```diff
@@ -20,15 +20,15 @@
 
 
 @PublicAPI(stability="beta")
 class DataSource:
     """Abstract class for data sources.
 
     xgboost_ray supports reading from various sources, such as files
-    (e.g. CSV, Parquet) or distributed datasets (Ray MLDataset, Modin).
+    (e.g. CSV, Parquet) or distributed datasets (Modin).
 
     This abstract class defines an interface to read from these sources.
     New data sources can be added by implementing this interface.
 
     ``DataSource`` classes are not instantiated. Instead, static and
     class methods are called directly.
     """
```

## xgboost_ray/tests/test_colocation.py

```diff
@@ -4,17 +4,18 @@
 import unittest
 from unittest.mock import patch
 import pytest
 
 import numpy as np
 
 import ray
+from ray.util.queue import _QueueActor
 from xgboost_ray import train, RayDMatrix, RayParams
 from xgboost_ray.main import _train
-from xgboost_ray.util import _EventActor, _QueueActor
+from xgboost_ray.util import _EventActor
 
 
 class _MockQueueActor(_QueueActor):
     def get_node_id(self):
         return ray.state.current_node_id()
 
 
@@ -53,15 +54,15 @@
             os.remove(self.die_lock_file)
 
     def tearDown(self) -> None:
         if os.path.exists(self.tmpdir):
             shutil.rmtree(self.tmpdir)
         ray.shutdown()
 
-    @patch("xgboost_ray.util._QueueActor", _MockQueueActor)
+    @patch("ray.util.queue._QueueActor", _MockQueueActor)
     @patch("xgboost_ray.util._EventActor", _MockEventActor)
     def test_communication_colocation(self):
         """Checks that Queue and Event actors are colocated with the driver."""
         with self.ray_start_cluster() as cluster:
             cluster.add_node(num_cpus=3)
             cluster.add_node(num_cpus=3)
             cluster.wait_for_nodes()
```

## xgboost_ray/tests/test_matrix.py

```diff
@@ -285,40 +285,14 @@
             df_2.to_parquet(data_file_2)
 
             self._testMatrixCreation(
                 [data_file_1, data_file_2], "label", distributed=False)
             self._testMatrixCreation(
                 [data_file_1, data_file_2], "label", distributed=True)
 
-    def testFromMLDataset(self):
-        try:
-            from ray.util import data as ml_data
-        except ImportError:
-            self.skipTest("MLDataset not available in current Ray version.")
-            return
-
-        with tempfile.TemporaryDirectory() as dir:
-            data_file_1 = os.path.join(dir, "data_1.parquet")
-            data_file_2 = os.path.join(dir, "data_2.parquet")
-
-            data_df = pd.DataFrame(self.x, columns=["a", "b", "c", "d"])
-            data_df["label"] = pd.Series(self.y)
-
-            df_1 = data_df[0:len(data_df) // 2]
-            df_2 = data_df[len(data_df) // 2:]
-
-            df_1.to_parquet(data_file_1)
-            df_2.to_parquet(data_file_2)
-
-            dataset = ml_data.read_parquet(
-                [data_file_1, data_file_2], num_shards=2)
-
-            self._testMatrixCreation(dataset, "label", distributed=False)
-            self._testMatrixCreation(dataset, "label", distributed=True)
-
     def testDetectDistributed(self):
         with tempfile.TemporaryDirectory() as dir:
             parquet_file = os.path.join(dir, "file.parquet")
             csv_file = os.path.join(dir, "file.csv")
 
             data_df = pd.DataFrame(self.x, columns=["a", "b", "c", "d"])
             data_df["label"] = pd.Series(self.y)
@@ -335,24 +309,14 @@
 
             mat = RayDMatrix([parquet_file] * 3, lazy=True)
             self.assertTrue(mat.distributed)
 
             mat = RayDMatrix([csv_file] * 3, lazy=True)
             self.assertTrue(mat.distributed)
 
-            try:
-                from ray.util import data as ml_data
-                mat = RayDMatrix(
-                    ml_data.read_parquet(parquet_file, num_shards=1),
-                    lazy=True)
-                self.assertTrue(mat.distributed)
-            except ImportError:
-                print("MLDataset not available in current Ray version. "
-                      "Skipping part of test.")
-
     def testTooManyActorsDistributed(self):
         """Test error when too many actors are passed"""
         with self.assertRaises(RuntimeError):
             dtrain = RayDMatrix(["foo.csv"], num_actors=4, distributed=True)
             dtrain.assert_enough_shards_for_actors(4)
 
     def testTooManyActorsCentral(self):
```

## xgboost_ray/tests/test_sklearn.py

```diff
@@ -24,29 +24,30 @@
 # https://github.com/dmlc/xgboost/blob/a5c852660b1056204aa2e0cbfcd5b4ecfbf31adf/LICENSE
 
 # import collections
 # import importlib.util
 import numpy as np
 import xgboost as xgb
 import unittest
+from distutils.version import LooseVersion
 
 # import io
 # from contextlib import redirect_stdout, redirect_stderr
 import tempfile
 import os
 import shutil
 import json
 
 import ray
 
 from xgboost_ray.sklearn import (RayXGBClassifier, RayXGBRegressor,
                                  RayXGBRFClassifier, RayXGBRFRegressor,
                                  RayXGBRanker)
 
-from xgboost_ray.main import (XGBOOST_VERSION_TUPLE, RayDMatrix, RayParams,
+from xgboost_ray.main import (XGBOOST_LOOSE_VERSION, RayDMatrix, RayParams,
                               train, predict)
 from xgboost_ray.matrix import RayShardingMode
 
 
 def softmax(x):
     e = np.exp(x)
     return e / np.sum(e)
@@ -130,15 +131,15 @@
 
     def test_binary_classification_dmatrix_params(self):
         self.run_binary_classification(
             RayXGBClassifier,
             ray_dmatrix_params={"sharding": RayShardingMode.BATCH})
 
     # ray: added for legacy CI test
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 0, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.0.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_binary_rf_classification(self):
         self.run_binary_classification(RayXGBRFClassifier)
 
     def test_multiclass_classification(self):
         self._init_ray()
 
@@ -189,15 +190,15 @@
         # so no transformation is required.
         cls = RayXGBClassifier(
             n_estimators=4, objective=softprob_obj(3)).fit(X, y)
         proba = cls.predict_proba(X)
         assert proba.shape[0] == X.shape[0]
         assert proba.shape[1] == cls.n_classes_
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 4, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.4.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_best_ntree_limit(self):
         self._init_ray()
 
         from sklearn.datasets import load_iris
 
         X, y = load_iris(return_X_y=True)
@@ -302,23 +303,28 @@
         reg = RayXGBRegressor(
             n_estimators=4, num_parallel_tree=4, tree_method="hist")
         boston = load_boston()
         bst = reg.fit(X=boston["data"], y=boston["target"])
         dump = bst.get_booster().get_dump(dump_format="json")
         assert len(dump) == 16
 
-        if xgb.__version__ != "0.90":
+        if XGBOOST_LOOSE_VERSION != LooseVersion("0.90"):
             reg = RayXGBRFRegressor(n_estimators=4)
             bst = reg.fit(X=boston["data"], y=boston["target"])
             dump = bst.get_booster().get_dump(dump_format="json")
             assert len(dump) == 4
 
-            config = json.loads(bst.get_booster().save_config())
-            assert (int(config["learner"]["gradient_booster"][
-                "gbtree_train_param"]["num_parallel_tree"]) == 4)
+            if XGBOOST_LOOSE_VERSION >= LooseVersion("1.6.0"):
+                config = json.loads(bst.get_booster().save_config())
+                assert (int(config["learner"]["gradient_booster"][
+                    "gbtree_model_param"]["num_parallel_tree"]) == 4)
+            else:
+                config = json.loads(bst.get_booster().save_config())
+                assert (int(config["learner"]["gradient_booster"][
+                    "gbtree_train_param"]["num_parallel_tree"]) == 4)
 
     def test_boston_housing_regression(self):
         self._init_ray()
 
         from sklearn.metrics import mean_squared_error
         from sklearn.datasets import load_boston
         from sklearn.model_selection import KFold
@@ -341,15 +347,15 @@
             labels = y[test_index]
 
             assert mean_squared_error(preds, labels) < 25
             assert mean_squared_error(preds2, labels) < 350
             assert mean_squared_error(preds3, labels) < 25
             assert mean_squared_error(preds4, labels) < 350
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 0, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.0.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def run_boston_housing_rf_regression(self, tree_method):
         from sklearn.metrics import mean_squared_error
         from sklearn.datasets import load_boston
         from sklearn.model_selection import KFold
 
         X, y = load_boston(return_X_y=True)
@@ -513,41 +519,41 @@
 
         preds = classifier.predict(te_d)
         labels = te_l
         err = (sum([1 for p, l in zip(preds, labels)
                     if p != l]) * 1.0 / len(te_l))
         assert err < 0.5
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 0, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.0.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_sklearn_random_state(self):
         self._init_ray()
 
         clf = RayXGBClassifier(random_state=402)
         assert clf.get_xgb_params()["random_state"] == 402
 
         clf = RayXGBClassifier(random_state=401)
         assert clf.get_xgb_params()["random_state"] == 401
 
         random_state = np.random.RandomState(seed=403)
         clf = RayXGBClassifier(random_state=random_state)
         assert isinstance(clf.get_xgb_params()["random_state"], int)
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 0, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.0.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_sklearn_n_jobs(self):
         self._init_ray()
 
         clf = RayXGBClassifier(n_jobs=1)
         assert clf.get_xgb_params()["n_jobs"] == 1
 
         clf = RayXGBClassifier(n_jobs=2)
         assert clf.get_xgb_params()["n_jobs"] == 2
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 3, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.3.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_parameters_access(self):
         self._init_ray()
 
         from sklearn import datasets
 
         params = {"updater": "grow_gpu_hist", "subsample": 0.5, "n_jobs": -1}
@@ -605,30 +611,30 @@
 
         from sklearn.base import clone
 
         clf = RayXGBClassifier(n_jobs=2)
         clf.n_jobs = -1
         clone(clf)
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 0, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.0.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_sklearn_get_default_params(self):
         self._init_ray()
 
         from sklearn.datasets import load_digits
 
         digits_2class = load_digits(n_class=2)
         X = digits_2class["data"]
         y = digits_2class["target"]
         cls = RayXGBClassifier()
         assert cls.get_params()["base_score"] is None
         cls.fit(X[:4, ...], y[:4, ...])
         assert cls.get_params()["base_score"] is not None
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 1, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.1.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_validation_weights_xgbmodel(self):
         self._init_ray()
 
         from sklearn.datasets import make_hastie_10_2
 
         # prepare training and test data
@@ -792,15 +798,15 @@
                 xgb.DMatrix(X[test_index]), output_margin=True)
             assert np.allclose(preds, predt_1)
 
             with self.assertRaises(TypeError):
                 xgb_model = xgb.XGBModel()
                 xgb_model.load_model(model_path)
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 3, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.3.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_save_load_model(self):
         self._init_ray()
 
         with TemporaryDirectory() as tempdir:
             model_path = os.path.join(tempdir, "digits.model")
             self.save_load_model(model_path)
@@ -946,26 +952,26 @@
 
             pred2 = model2.predict(X)
             log_loss2 = log_loss(pred2, Y)
 
             assert np.any(pred1 != pred2)
             assert log_loss1 > log_loss2
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 0, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.0.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_constraint_parameters(self):
         self._init_ray()
 
         reg = RayXGBRegressor(interaction_constraints="[[0, 1], [2, 3, 4]]")
         X = np.random.randn(10, 10)
         y = np.random.randn(10)
         reg.fit(X, y)
 
         config = json.loads(reg.get_booster().save_config())
-        if XGBOOST_VERSION_TUPLE >= (1, 6, 0):
+        if XGBOOST_LOOSE_VERSION >= LooseVersion("1.6.0"):
             assert (config["learner"]["gradient_booster"]["updater"][
                 "grow_histmaker"]["train_param"]["interaction_constraints"] ==
                     "[[0, 1], [2, 3, 4]]")
         else:
             assert (config["learner"]["gradient_booster"]["updater"]["prune"][
                 "train_param"]["interaction_constraints"] ==
                     "[[0, 1], [2, 3, 4]]")
@@ -1166,31 +1172,31 @@
         assert np.all(predictions_1 == predictions_2)
 
     def boost_from_prediction(self, tree_method):
         self._init_ray()
 
         self.run_boost_from_prediction(tree_method)
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 0, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.0.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_boost_from_prediction_hist(self):
         self.run_boost_from_prediction("hist")
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 2, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.2.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_boost_from_prediction_approx(self):
         self.run_boost_from_prediction("approx")
 
     # Updater `grow_colmaker` or `exact` tree method doesn't support
     # distributed training
     def test_boost_from_prediction_exact(self):
         with self.assertRaises(ValueError):
             self.run_boost_from_prediction("exact")
 
-    @unittest.skipIf(XGBOOST_VERSION_TUPLE < (1, 4, 0),
+    @unittest.skipIf(XGBOOST_LOOSE_VERSION < LooseVersion("1.4.0"),
                      f"not supported in xgb version {xgb.__version__}")
     def test_estimator_type(self):
         self._init_ray()
 
         assert RayXGBClassifier._estimator_type == "classifier"
         assert RayXGBRFClassifier._estimator_type == "classifier"
         assert RayXGBRegressor._estimator_type == "regressor"
```

## xgboost_ray/tests/test_sklearn_matrix.py

```diff
@@ -1,22 +1,23 @@
+from distutils.version import LooseVersion
 import numpy as np
 import unittest
 
 import ray
 import xgboost as xgb
 
 from sklearn.model_selection import train_test_split
 
 from xgboost_ray.sklearn import (RayXGBClassifier, RayXGBRegressor)
 from xgboost_ray.main import RayDMatrix
 
-from xgboost_ray.main import XGBOOST_VERSION_TUPLE
+from xgboost_ray.main import XGBOOST_LOOSE_VERSION
 
-has_label_encoder = (XGBOOST_VERSION_TUPLE >= (1, 0, 0)
-                     and XGBOOST_VERSION_TUPLE < (1, 6, 0))
+has_label_encoder = (XGBOOST_LOOSE_VERSION >= LooseVersion("1.0.0")
+                     and XGBOOST_LOOSE_VERSION < LooseVersion("1.6.0"))
 
 
 class XGBoostRaySklearnMatrixTest(unittest.TestCase):
     def setUp(self):
         self.seed = 1994
         self.rng = np.random.RandomState(self.seed)
         self.params = {"n_estimators": 10}
```

## xgboost_ray/tests/test_tune.py

```diff
@@ -63,19 +63,21 @@
         ray.shutdown()
         shutil.rmtree(self.experiment_dir)
 
     # noinspection PyTypeChecker
     def testNumIters(self):
         """Test that the number of reported tune results is correct"""
         ray_params = RayParams(cpus_per_actor=1, num_actors=2)
+        params = self.params.copy()
+        params["num_boost_round"] = tune.grid_search([1, 3])
         analysis = tune.run(
             self.train_func(ray_params),
             config=self.params,
             resources_per_trial=ray_params.get_tune_resources(),
-            num_samples=2)
+            num_samples=1)
 
         self.assertSequenceEqual(
             list(analysis.results_df["training_iteration"]),
             list(analysis.results_df["config.num_boost_round"]))
 
     def testNumItersClient(self):
         """Test ray client mode"""
```

## Comparing `xgboost_ray-0.1.8.dist-info/LICENSE` & `xgboost_ray-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

