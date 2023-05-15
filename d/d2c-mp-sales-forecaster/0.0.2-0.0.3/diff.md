# Comparing `tmp/d2c_mp_sales_forecaster-0.0.2.tar.gz` & `tmp/d2c_mp_sales_forecaster-0.0.3.tar.gz`

## Comparing `d2c_mp_sales_forecaster-0.0.2.tar` & `d2c_mp_sales_forecaster-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/.dockerignore
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/Dockerfile
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/compose.yaml
--rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/environment.yml
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/requirements.txt
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/.vscode/launch.json
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/.vscode/tasks.json
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/D2CMPForecaster.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/config.toml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/config/db_ddl.sql
--rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_1_Load_Data.py
--rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_2_Product_Selection.py
--rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_3_Tune_and_Train.py
--rw-r--r--   0        0        0    12702 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_4_Forecast_Product.py
--rw-r--r--   0        0        0    10073 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_5_Distribute_Size_Forecast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/utils/__init__.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/utils/db_manager.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_1_Load_Data.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_2_Product_Selection.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_3_Tune_and_Train.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_4_Forecast_Product.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_5_Distribute_Size_forecast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_D2CMPForecaster.py
--rwxr-xr-x   0        0        0    41114 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/select_product/lag_data.csv
--rwxr-xr-x   0        0        0    31393 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/select_product/master_data_enc.csv
--rwxr-xr-x   0        0        0   918353 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/select_product/sales_data.csv
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/.gitignore
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/LICENSE
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/README.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/.dockerignore
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/Dockerfile
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/compose.yaml
+-rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/environment.yml
+-rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/.vscode/launch.json
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/.vscode/tasks.json
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/D2CMPForecaster.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/config.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/config/db_ddl.sql
+-rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_1_Load_Data.py
+-rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_2_Product_Selection.py
+-rw-r--r--   0        0        0    18370 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_3_Tune_and_Train.py
+-rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_4_Forecast_Product.py
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_5_Distribute_Size_Forecast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/utils/__init__.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/utils/db_manager.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/tests/test_1_Load_Data.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/tests/test_2_Product_Selection.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/tests/test_3_Tune_and_Train.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/tests/test_4_Forecast_Product.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/tests/test_5_Distribute_Size_forecast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/tests/test_D2CMPForecaster.py
+-rwxr-xr-x   0        0        0    41114 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/tests/select_product/lag_data.csv
+-rwxr-xr-x   0        0        0    31393 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/tests/select_product/master_data_enc.csv
+-rwxr-xr-x   0        0        0   918353 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/tests/select_product/sales_data.csv
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/README.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.3/PKG-INFO
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/Dockerfile` & `d2c_mp_sales_forecaster-0.0.3/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -6,23 +6,19 @@
 RUN apt-get update && apt-get install -y \
     build-essential \
     curl \
     software-properties-common \
     git \
     && rm -rf /var/lib/apt/lists/*
 
-#RUN git clone https://github.com/rhanderh/d2c_mp_forecast_tool.git .
+RUN git clone https://github.com/rhanderh/d2c_mp_forecast_tool.git .
 
-COPY . .
-
-# Create the environment from environment.yml and make sure conda is in the PATH
+# Create the environment from environment.yml 
 ADD environment.yml /tmp/environment.yml
 RUN conda env create -f /tmp/environment.yml
-
-# Pull the environment name out of the environment.yml
 RUN echo "source activate d2c_mp_sales_fcst" > ~/.bashrc
 ENV PATH /opt/conda/envs/d2c_mp_sales_fcst/bin:$PATH
 
 EXPOSE 8501
 
 HEALTHCHECK CMD curl --fail http://localhost:8501/_stcore/health
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/environment.yml` & `d2c_mp_sales_forecaster-0.0.3/environment.yml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
   - blinker=1.4=py39h06a4308_0
   - boltons=23.0.0=py39h06a4308_0
   - boost-cpp=1.73.0=h7f8727e_12
   - bottleneck=1.3.5=py39h7deecbd_0
   - brotli=1.0.9=h5eee18b_7
   - brotli-bin=1.0.9=h5eee18b_7
   - brotlipy=0.7.0=py39h27cfd23_1003
-  - build=0.7.0=pyhd8ed1ab_0
   - bzip2=1.0.8=h7b6447c_0
   - c-ares=1.19.0=h5eee18b_0
   - ca-certificates=2023.01.10=h06a4308_0
   - cachetools=4.2.2=pyhd3eb1b0_0
   - certifi=2022.12.7=py39h06a4308_0
   - cffi=1.15.1=py39h5eee18b_3
   - chardet=4.0.0=py39h06a4308_1003
@@ -109,14 +108,15 @@
   - libgfortran-ng=11.2.0=h00389a5_1
   - libgfortran5=11.2.0=h1234567_1
   - libgomp=11.2.0=h1234567_1
   - liblief=0.12.3=h6a678d5_0
   - libllvm11=11.1.0=h9e868ea_6
   - libnghttp2=1.46.0=hce63b2e_0
   - libpng=1.6.39=h5eee18b_0
+  - libpq=12.9=h16c4e8d_3
   - libprotobuf=3.20.3=he621ea3_0
   - libsodium=1.0.18=h7b6447c_0
   - libssh2=1.10.0=h8f2d780_0
   - libstdcxx-ng=11.2.0=h1234567_1
   - libthrift=0.15.0=hcc01f38_0
   - libtiff=4.5.0=h6a678d5_2
   - libwebp=1.2.4=h11a3e52_1
@@ -160,14 +160,15 @@
   - platformdirs=2.5.2=py39h06a4308_0
   - plotly=5.9.0=py39h06a4308_0
   - pluggy=1.0.0=py39h06a4308_1
   - pooch=1.4.0=pyhd3eb1b0_0
   - prompt-toolkit=3.0.36=py39h06a4308_0
   - protobuf=3.20.3=py39h6a678d5_0
   - psutil=5.9.0=py39h5eee18b_0
+  - psycopg2=2.9.3=py39h37d81fd_0
   - ptyprocess=0.7.0=pyhd3eb1b0_2
   - pure_eval=0.2.2=pyhd3eb1b0_0
   - py=1.11.0=pyhd3eb1b0_0
   - py-lief=0.12.3=py39h6a678d5_0
   - pyarrow=11.0.0=py39h992f0b0_0
   - pycodestyle=2.10.0=py39h06a4308_0
   - pycosat=0.6.4=py39h5eee18b_0
@@ -238,20 +239,22 @@
   - zeromq=4.3.4=h2531618_0
   - zipp=3.11.0=py39h06a4308_0
   - zlib=1.2.13=h5eee18b_0
   - zstandard=0.19.0=py39h5eee18b_0
   - zstd=1.5.5=hc292b87_0
   - pip:
       - bleach==6.0.0
-      - d2c-mp-sales-forecaster==0.0.1
+      - build==0.10.0
+      - d2c-mp-sales-forecaster==0.0.2
       - docutils==0.19
       - jaraco-classes==3.2.3
       - jeepney==0.8.0
       - keyring==23.13.1
       - more-itertools==9.1.0
+      - pyproject-hooks==1.0.0
       - readme-renderer==37.3
       - requests-toolbelt==0.10.1
       - rfc3986==2.0.0
       - secretstorage==3.3.3
       - twine==4.0.2
       - webencodings==0.5.1
 prefix: /home/rhanderh/miniconda3/envs/d2c_mp_sales_fcst
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/D2CMPForecaster.py` & `d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/D2CMPForecaster.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,12 +19,7 @@
 #from d2c_mp_sales_forecast_streamlit.libraries.similar_products import *
 
 # Page config
 st.set_page_config(page_title="D2C, Dropship, Marketplace Time-Series Forecasting")
 
 #Title
 st.title("D2C, Dropship, Marketplace Sales Time-Series Forecasting")
-
-
-
-
-
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/config/db_ddl.sql` & `d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/config/db_ddl.sql`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_1_Load_Data.py` & `d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_1_Load_Data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,261 +1,215 @@
 # Imports
 import streamlit as st
-import itertools
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from datetime import date
 from datetime import timedelta
 
-# Page config
-st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
+class LoadData:
 
-st.header("Step 1: Upload datasets for forcasting.")
-
-
-def upload_sales_size_data(uploaded_file) -> tuple:
-    """
-    Upload, format, and cleanse product sales data by size and day.
-
-    Args:
-        uploaded_file: A CSV file containing product sales data by size and day.
-
-    Returns:
-        A tuple of two DataFrames:
-            1. all_sales_data: Aggregated product sales data.
-            2. all_sales_size_data: Product sales data with proper typing and formatting.
-    """
-    with st.spinner("Uploading file..."):
-        all_sales_size_data = pd.read_csv(uploaded_file,
-                                          header=0,
-                                          names=['product', 'size', 'ds', 'y'],
-                                          dtype={
-                                              'product': 'object', 'size': 'object', 'date': 'object', 'y': 'object'},
-                                          parse_dates=['ds'],
-                                          infer_datetime_format=True
-                                          )
-        all_sales_size_data = all_sales_size_data[all_sales_size_data['size'] != 'Result']
-        all_sales_size_data['y'] = all_sales_size_data['y'].str.replace(
-            ',', '')
-        all_sales_size_data['y'] = all_sales_size_data['y'].astype('int64')
+    def __init__(self):
+        #Initialize state-dependent streamlit variables
         if 'all_sales_size_data' not in st.session_state:
-            st.session_state['all_sales_size_data'] = all_sales_size_data
-        else:
-            st.session_state['all_sales_size_data'] = all_sales_size_data
-        # Group and save a version of the dataframe aggregated to the product level
-        all_sales_data = all_sales_size_data.groupby(
-            ['product', 'ds']).agg({'y': 'sum'})
-        all_sales_data.reset_index(inplace=True)
+            st.session_state['all_sales_size_data'] = pd.DataFrame()
         if 'all_sales_data' not in st.session_state:
+            st.session_state['all_sales_data'] = pd.DataFrame()
+        if 'master_data' not in st.session_state:
+            st.session_state['master_data'] = pd.DataFrame()
+        if 'master_data_enc' not in st.session_state:
+            st.session_state['master_data_enc'] = pd.DataFrame()
+        if 'events_df' not in st.session_state:
+            st.session_state['events_df'] = pd.DataFrame()
+        if 'lag_data' not in st.session_state:
+            st.session_state['lag_data'] = pd.DataFrame()
+        #Layout the streamlit page 
+        st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
+        st.header("Step 1: Upload datasets for forecasting.")
+        self.upload_sales_size_data()
+        self.upload_master_data()
+        self.upload_events_data()
+        if not st.session_state['all_sales_data'].empty:
+            self.upload_lag_data()
+
+    def upload_sales_size_data(self):
+        st.subheader("a. Upload historical sales by product and size.")
+        uploaded_file = st.file_uploader(
+            "Select Sales History by Product and Size for Upload")
+        st.write(uploaded_file)
+        if uploaded_file is not None:
+            all_sales_data, lag_data = self.upload_sales_size_data_func(uploaded_file)
+        if not st.session_state['all_sales_data'].empty:
+            st.write("You currently have uploaded the following data:")
+            cola, colb = st.columns(2)
+            with cola:
+                st.subheader('Product Sales History')
+                st.write(st.session_state['all_sales_data'])
+            with colb:
+                st.subheader('Product-Size Sales History')
+                st.write(st.session_state['all_sales_size_data'])
+
+    def upload_sales_size_data_func(self, uploaded_file) -> tuple:
+        """
+        Upload, format, and cleanse product sales data by size and day.
+
+        Args:
+            uploaded_file: A CSV file containing product sales data by size and day.
+
+        Returns:
+            A tuple of two DataFrames:
+                1. all_sales_data: Aggregated product sales data.
+                2. all_sales_size_data: Product sales data with proper typing and formatting.
+        """
+        with st.spinner("Uploading file..."):
+            all_sales_size_data = pd.read_csv(uploaded_file,
+                                            header=0,
+                                            names=['product', 'size', 'ds', 'y'],
+                                            dtype={
+                                                'product': 'object', 'size': 'object', 'date': 'object', 'y': 'object'},
+                                            parse_dates=['ds'],
+                                            infer_datetime_format=True
+                                            )
+            all_sales_size_data = all_sales_size_data[all_sales_size_data['size'] != 'Result']
+            all_sales_size_data['y'] = all_sales_size_data['y'].str.replace(
+                ',', '')
+            all_sales_size_data['y'] = all_sales_size_data['y'].astype('int64')
+            st.session_state['all_sales_size_data'] = all_sales_size_data
+            # Group and save a version of the dataframe aggregated to the product level
+            all_sales_data = all_sales_size_data.groupby(
+                ['product', 'ds']).agg({'y': 'sum'})
+            all_sales_data.reset_index(inplace=True)
             st.session_state['all_sales_data'] = all_sales_data
-        else:
-            st.session_state['all_sales_data'] = all_sales_data
-    st.success("File upload complete!")
-    return all_sales_data, all_sales_size_data
-
+        st.success("File upload complete!")
+        return all_sales_data, all_sales_size_data
 
-def upload_master_data(uploaded_md_file) -> tuple:
-    """
-    Upload product master data.
-
-    Args:
-        uploaded_md_file: A CSV file containing product master data. The first column should be the unique product key.
-
-    Returns:
-        A tuple of two DataFrames:
-            1. master_data: The uploaded product master data.
-            2. master_data_enc: The encoded product master data.
-    """
-    with st.spinner("Uploading file..."):
-        master_data = pd.read_csv(uploaded_md_file, index_col=0)
-        master_data.index.rename('product', inplace=True)
-        master_data.index = master_data.index.map(str)
-        # Econde the master data --> break this into a separate optional function later.
-        master_data_enc = pd.get_dummies(master_data)
-        master_data_enc = master_data_enc.fillna(0)
-        if 'master_data' not in st.session_state:
+    def upload_master_data(self):
+        st.subheader("b. Upload product attributes for augmenting historicals with similar product sales.")
+        uploaded_md_file = st.file_uploader("Select product master data to upload.")
+        st.write(uploaded_md_file)
+        if uploaded_md_file is not None:
+            master_data, master_data_enc = self.upload_master_data_func(uploaded_md_file)
+        if not st.session_state['master_data'].empty:
+            st.write("You currently have uploaded the following data:")
+            st.subheader('Product Master Data')
+            st.write(st.session_state['master_data'])
+            st.download_button(label="Download Encoded Master Data",
+                            data=self.convert_df(st.session_state['master_data_enc']),
+                            file_name='master_data_enc.csv',
+                            mime='text/csv'
+                            )
+
+    def upload_master_data_func(self, uploaded_md_file) -> tuple:
+        """
+        Upload product master data.
+
+        Args:
+            uploaded_md_file: A CSV file containing product master data. The first column should be the unique product key.
+
+        Returns:
+            A tuple of two DataFrames:
+                1. master_data: The uploaded product master data.
+                2. master_data_enc: The encoded product master data.
+        """
+        with st.spinner("Uploading file..."):
+            master_data = pd.read_csv(uploaded_md_file, index_col=0)
+            master_data.index.rename('product', inplace=True)
+            master_data.index = master_data.index.map(str)
+            # Econde the master data --> break this into a separate optional function later.
+            master_data_enc = pd.get_dummies(master_data)
+            master_data_enc = master_data_enc.fillna(0)
             st.session_state['master_data'] = master_data
-        else:
-            st.session_state['master_data'] = master_data
-        if 'master_data_enc' not in st.session_state:
-            st.session_state['master_data_enc'] = master_data_enc
-        else:
             st.session_state['master_data_enc'] = master_data_enc
-    st.success("File upload complete!")
-    return master_data, master_data_enc
+        st.success("File upload complete!")
+        return master_data, master_data_enc
 
+    def upload_events_data(self):
+        st.subheader("c. Upload holidays and special events.  (Optional)")
+        uploaded_ev_file = st.file_uploader(
+            "Select holidays and events file to upload.")
+        st.write(uploaded_ev_file)
+        if uploaded_ev_file is not None:
+            events_df = self.upload_events_data_func(uploaded_ev_file)
+        if not st.session_state['events_df'].empty:
+            st.write("You currently have uploaded the following data:")
+            st.subheader('Events')
+            st.write(st.session_state['events_df'])
+
+    def upload_events_data_func(self, uploaded_ev_file) -> pd.DataFrame:
+        """
+        Upload holidays and events data.
+
+        Args:
+            uploaded_ev_file: A CSV file containing holidays and events data.
+
+        Returns:
+            events_df: A DataFrame containing the uploaded holidays and events data.
+        """
+        with st.spinner("Uploading file..."):
+            events_df = pd.read_csv(uploaded_ev_file,
+                                    header=0,
+                                    names=['event', 'ds',
+                                        'lower_window', 'upper_window'],
+                                    dtype={'event': 'object', 'ds': 'object',
+                                        'lower_window': 'int64', 'upper_window': 'int64'},
+                                    parse_dates=['ds'],
+                                    infer_datetime_format=True)
+            st.session_state['events_df'] = events_df
+        st.success("File upload complete!")
+        return events_df
 
-def upload_events_data(uploaded_ev_file) -> pd.DataFrame:
-    """
-    Upload holidays and events data.
-
-    Args:
-        uploaded_ev_file: A CSV file containing holidays and events data.
-
-    Returns:
-        events_df: A DataFrame containing the uploaded holidays and events data.
-    """
-    with st.spinner("Uploading file..."):
-        events_df = pd.read_csv(uploaded_ev_file,
+    def upload_lag_data(self):
+        st.subheader("d. Upload lag regressors.  (Optional)")
+        uploaded_lag_file = st.file_uploader(
+            "Select lag regressor data to upload.")
+        st.write(uploaded_lag_file)
+        if uploaded_lag_file is not None:
+            lag_data = self.upload_lag_data_func(uploaded_lag_file)
+        if not st.session_state['lag_data'].empty:
+            st.write("You currently have uploaded the following data:")
+            st.subheader('Lag Regressor Data')
+            st.write(st.session_state['lag_data'])
+
+    def upload_lag_data_func(self, uploaded_lag_file) -> tuple:
+        """
+        Upload and preprocess lag regressors data.
+
+        Args:
+            uploaded_lag_file: A CSV file containing lag regressors data.
+
+        Returns:
+            lag_data: A DataFrame containing the preprocessed lag regressors data.
+        """
+        with st.spinner("Uploading file..."):
+            lag_data = pd.read_csv(uploaded_lag_file,
                                 header=0,
-                                names=['event', 'ds',
-                                       'lower_window', 'upper_window'],
-                                dtype={'event': 'object', 'ds': 'object',
-                                       'lower_window': 'int64', 'upper_window': 'int64'},
                                 parse_dates=['ds'],
-                                infer_datetime_format=True)
-        if 'events_df' not in st.session_state:
-            st.session_state['events_df'] = events_df
-        else:
-            st.session_state['events_df'] = events_df
-    st.success("File upload complete!")
-    return events_df
-
-
-def upload_lag_data(uploaded_lag_file) -> tuple:
-    """
-    Upload and preprocess lag regressors data.
-
-    Args:
-        uploaded_lag_file: A CSV file containing lag regressors data.
-
-    Returns:
-        lag_data: A DataFrame containing the preprocessed lag regressors data.
-    """
-    with st.spinner("Uploading file..."):
-        lag_data = pd.read_csv(uploaded_lag_file,
-                               header=0,
-                               parse_dates=['ds'],
-                               infer_datetime_format=True
-                               )
-        # Set datetime interval to day and ensure timeseries complete by day
-        lag_data['ds'] = pd.to_datetime(lag_data['ds'])
-        lag_data = lag_data.set_index('ds')
-        lag_data = lag_data.resample('1D').ffill().reset_index()
-        # Remove commas and cast all other columns as float64 data type
-        for col in lag_data.columns:
-            if col != 'ds':
-                if lag_data[col].dtype == 'object':
-                    lag_data[col] = lag_data[col].str.replace(',', '')
-                lag_data[col] = lag_data[col].astype('float64')
-        if 'lag_data' not in st.session_state:
-            st.session_state['lag_data'] = lag_data
-        else:
+                                infer_datetime_format=True
+                                )
+            # Set datetime interval to day and ensure timeseries complete by day
+            lag_data['ds'] = pd.to_datetime(lag_data['ds'])
+            lag_data = lag_data.set_index('ds')
+            lag_data = lag_data.resample('1D').ffill().reset_index()
+            # Remove commas and cast all other columns as float64 data type
+            for col in lag_data.columns:
+                if col != 'ds':
+                    if lag_data[col].dtype == 'object':
+                        lag_data[col] = lag_data[col].str.replace(',', '')
+                    lag_data[col] = lag_data[col].astype('float64')
             st.session_state['lag_data'] = lag_data
-    st.success("File upload complete!")
-    return lag_data
+        st.success("File upload complete!")
+        return lag_data
 
+    def convert_df(self, df):
+        """
+        Convert a DataFrame to a CSV string and encode it as utf-8 bytes.
+
+        Args:
+            df: A DataFrame to be converted.
+
+        Returns:
+            A CSV string of the DataFrame encoded as utf-8 bytes.
+        """
+        return df.to_csv().encode('utf-8')
 
-def upload_future_data(uploaded_future_file) -> tuple:
-    """
-    Upload and preprocess future regressors data.
-
-    Args:
-        uploaded_future_file: A CSV file containing future regressors data.
-
-    Returns:
-        future_data: A DataFrame containing the preprocessed future regressors data.
-    """
-    with st.spinner("Uploading file..."):
-        future_data = pd.read_csv(uploaded_future_file,
-                                  header=0,
-                                  parse_dates=['ds'],
-                                  infer_datetime_format=True
-                                  )
-        # set datetime interval to day and ensure timeseries completeness
-        future_data['ds'] = pd.to_datetime(future_data['ds'])
-        future_data = future_data.set_index('ds')
-        future_data = future_data.resample('1D').ffill().reset_index()
-        # Remove commas and cast all other columns as float64 data type
-        for col in future_data.columns:
-            if col != 'ds':
-                if future_data[col].dtype == 'object':
-                    future_data[col] = future_data[col].str.replace(',', '')
-                future_data[col] = future_data[col].astype('float64')
-        if 'future_data' not in st.session_state:
-            st.session_state['future_data'] = future_data
-        else:
-            st.session_state['future_data'] = future_data
-    st.success("File upload complete!")
-    return future_data
-
-
-@st.cache_resource
-def convert_df(df):
-    """
-    Convert a DataFrame to a CSV string and encode it as utf-8 bytes.
-
-    Args:
-        df: A DataFrame to be converted.
-
-    Returns:
-        A CSV string of the DataFrame encoded as utf-8 bytes.
-    """
-    return df.to_csv().encode('utf-8')
-
-
-# File Uploaders
-st.subheader("a. Upload historical sales by product and size.")
-uploaded_file = st.file_uploader(
-    "Select Sales History by Product and Size for Upload")
-st.write(uploaded_file)
-if uploaded_file is not None:
-    all_sales_data, lag_data = upload_sales_size_data(uploaded_file)
-if 'all_sales_data' in st.session_state:
-    st.write("You currently have uploaded the following data:")
-    cola, colb = st.columns(2)
-    with cola:
-        st.subheader('Product Sales History')
-        st.write(st.session_state['all_sales_data'])
-    with colb:
-        st.subheader('Product-Size Sales History')
-        st.write(st.session_state['all_sales_size_data'])
-
-st.subheader(
-    "b. Upload product attributes for augmenting historicals with similar product sales.")
-uploaded_md_file = st.file_uploader("Select product master data to upload.")
-st.write(uploaded_md_file)
-if uploaded_md_file is not None:
-    master_data, master_data_enc = upload_master_data(uploaded_md_file)
-if 'master_data' in st.session_state:
-    st.write("You currently have uploaded the following data:")
-    st.subheader('Product Master Data')
-    st.write(st.session_state['master_data'])
-    st.download_button(label="Download Encoded Master Data",
-                       data=convert_df(st.session_state['master_data_enc']),
-                       file_name='master_data_enc.csv',
-                       mime='text/csv'
-                       )
-
-st.subheader("c. Upload holidays and special events.  (Optional)")
-uploaded_ev_file = st.file_uploader(
-    "Select holidays and events file to upload.")
-st.write(uploaded_ev_file)
-if uploaded_ev_file is not None:
-    events_df = upload_events_data(uploaded_ev_file)
-if 'events_df' in st.session_state:
-    st.write("You currently have uploaded the following data:")
-    st.subheader('Events')
-    st.write(st.session_state['events_df'])
-
-if 'all_sales_data' in st.session_state and 'all_sales_size_data' in st.session_state:
-    st.subheader("d. Upload lag regressors.  (Optional)")
-    uploaded_lag_file = st.file_uploader(
-        "Select lag regressor data to upload.")
-    st.write(uploaded_lag_file)
-    if uploaded_lag_file is not None:
-        lag_data = upload_lag_data(uploaded_lag_file)
-    if 'lag_data' in st.session_state:
-        st.write("You currently have uploaded the following data:")
-        st.subheader('Lag Regressor Data')
-        st.write(st.session_state['lag_data'])
-
-    # st.subheader("e. Upload future regressors.")
-    # uploaded_future_file = st.file_uploader("Select future regressor data to upload.")
-    # st.write(uploaded_future_file)
-    # if uploaded_future_file is not None:
-    #    future_data = upload_future_data(uploaded_future_file)
-    # if 'lag_data' in st.session_state:
-    #    st.write("You currently have uploaded the following data:")
-    #    st.subheader('Future Regressor Data')
-    #    st.write(st.session_state['future_data'])
+if __name__ == '__main__':
+    ld = LoadData()
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_2_Product_Selection.py` & `d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_2_Product_Selection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,349 +1,354 @@
 import streamlit as st
 import pandas as pd
 import numpy as np
 from sklearn.metrics.pairwise import cosine_similarity
 from datetime import date
 from datetime import timedelta
 
-# Page config
-st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
 
+class ProductSelection:
 
-def get_len_history(all_sales_data: pd.DataFrame) -> pd.DataFrame:
-    """
-    Calculate the length of sales history for each product.
-
-    Args:
-        all_sales_data: A DataFrame containing aggregated product sales data.
-
-    Returns:
-        sales_minmax_dates: A DataFrame containing the length of sales history for each product.
-    """
-    sorted_sales = all_sales_data.sort_values(
-        by=['product', 'ds'], ascending=True)
-    sales_minmax_dates = sorted_sales.groupby(
-        'product').agg({'ds': ['min', 'max'], 'y': 'sum'})
-    sales_minmax_dates['len_hist'] = (sales_minmax_dates.loc[:, (
-        'ds', 'max')] - sales_minmax_dates.loc[:, ('ds', 'min')]) / np.timedelta64(1, 'D')
-    return sales_minmax_dates
-
-
-@st.cache_data
-def get_similarities(master_data_enc: pd.DataFrame) -> pd.DataFrame:
-    """
-    Calculate cosine similarity between products based on encoded master data.
-
-    Args:
-        master_data_enc: A DataFrame containing encoded product master data.
-
-    Returns:
-        similarity_df: A DataFrame containing the cosine similarity scores between products.
-    """
-    similarity = cosine_similarity(master_data_enc)
-    similarity_df = pd.DataFrame(similarity,
-                                 index=master_data_enc.index.values,
-                                 columns=master_data_enc.index.values)
-    return similarity_df
-
-
-def check_history_needed(sales_minmax_dates: pd.DataFrame, product_fcst: str, min_req_hist: float = 366.0):
-    """
-    Check for the minimum history needed for forecasting a specific product.
-
-    Args:
-        sales_minmax_dates: A DataFrame containing the length of sales history for each product.
-        product_fcst: The product to be forecasted.
-        min_req_hist: The minimum required history for forecasting (default: 366 days).
-
-    Returns:
-        min_append_hist_req: The minimum required history to append.
-        cutoff_date: The cutoff date for adding history.
-    """
-    # lookup length of history for that product
-    len_avail_hist = sales_minmax_dates.loc[sales_minmax_dates.index ==
-                                            product_fcst]['len_hist'].values[0]
-    # difference with minimum required history to identify days gap aka minimum required length of history to append
-    min_append_hist_req = int(min_req_hist - len_avail_hist)
-    # identify the cutoff to add the length of history to
-    cutoff_date = sales_minmax_dates.loc[sales_minmax_dates.index == product_fcst][(
-        'ds', 'min')] - timedelta(min_append_hist_req)
-    return min_append_hist_req, cutoff_date.values[0]
-
-
-def match_product(similarity_df: pd.DataFrame, sales_minmax_dates: pd.DataFrame, product_fcst: str, cutoff_date: np.datetime64,  top_n: int = 1):
-    """
-    Match a product to similar products based on a similarity DataFrame.
-
-    Args:
-        similarity_df: A DataFrame containing the cosine similarity scores between products.
-        sales_minmax_dates: A DataFrame containing the length of sales history for each product.
-        product_fcst: The product to be forecasted.
-        cutoff_date: The cutoff date for adding history.
-        top_n: The number of top similar products desired (default: 1).
-
-    Returns:
-        matched: A list of matched similar products.
-    """
-    # product list of only products that meet minimum length requirements in addition to available history
-    product_list = sales_minmax_dates.loc[sales_minmax_dates[(
-        'ds', 'min')] < cutoff_date].index.values
-    # slice similarity dataframe by the product being forecasted on row-index, and the product list on the column-index
-    product_sim = similarity_df.loc[similarity_df.index ==
-                                    product_fcst, product_list].values[0]
-    # get products sorted by similarity
-    sorted_products = np.argsort(product_sim)[::-1]
-    # get matched product id
-    matched = product_list[sorted_products[1:top_n+1]]
-    return matched
-
-
-def fill_missing(sales_history: pd.DataFrame) -> pd.DataFrame:
-    """
-    Fill missing values in a sales history DataFrame.
-
-    Args:
-        sales_history: A DataFrame containing sales history data.
-
-    Returns:
-        sales_history: A DataFrame with missing values filled.
-    """
-    sales_history = sales_history.sort_values(by='ds')
-    sales_history.index = pd.to_datetime(sales_history['ds'])
-    sales_history.drop(columns=['ds'], inplace=True)
-    sales_history = sales_history.asfreq('D')
-    # fill all non quantities with forward-fill
-    for col in sales_history.columns:
-        if col != 'y':
-            sales_history[col].fillna(method='ffill', inplace=True)
-    # assume a 0 means no sale for that day
-    sales_history['y'].fillna(0, inplace=True)
-    sales_history.reset_index(inplace=True)
-    return sales_history
-
-
-def merge_regressors(sales_data, lag_data, future_data=None) -> pd.DataFrame:
-    """
-    Merge sales data with lag and future regressor data.
-
-    Args:
-        sales_data: A DataFrame containing sales data.
-        lag_data: A DataFrame containing lag regressor data.
-        future_data: A DataFrame containing future regressor data (optional).
-
-    Returns:
-        all_sales_data_lag: A DataFrame with sales data merged with lag and future regressor data.
-    """
-    all_sales_data_lag = pd.merge(sales_data, lag_data, on='ds', how='inner')
-    return all_sales_data_lag
-
-
-def append_history(all_sales_data: pd.DataFrame, matched: list, product_fcst: str, lag_data: pd.DataFrame = None) -> pd.DataFrame:
-    """
-    Append sales history for a product with the history of a similar product.
-
-    Args:
-        all_sales_data: A DataFrame containing aggregated product sales data.
-        matched: A list of matched similar products.
-        product_fcst: The product to be forecasted.
-        lag_data: A DataFrame containing lag regressor data (optional).
-
-    Returns:
-        A tuple of two DataFrames:
-            1. appended_history: The appended sales history.
-            2. appended_history_product: The appended sales history with the product column.
-    """
-    product_history = all_sales_data.loc[all_sales_data['product']
-                                         == product_fcst]
-    min_date = product_history['ds'].min()
-    extra_history = all_sales_data.loc[all_sales_data['product'] == matched[0]]
-    extra_history = extra_history.loc[extra_history['ds'] < min_date]
-    appended_history_product = fill_missing(
-        pd.concat([product_history, extra_history]))
-    if lag_data is not None:
-        appended_history_product = merge_regressors(
-            appended_history_product, lag_data)
-    appended_history = appended_history_product.drop(
-        columns='product').copy(deep=True)
-    return appended_history, appended_history_product
-
-
-def prepare_non_appended(sales_history: pd.DataFrame, forecast_product: str, all_sales_regressors: pd.DataFrame = None):
-    """
-    Prepare sales history for a product without appending additional history from similar products.
-
-    Args:
-        sales_history: A DataFrame containing sales history data.
-        forecast_product: The product to be forecasted.
-        all_sales_regressors: A DataFrame containing sales data with additional regressors (optional).
-
-    Returns:
-        A tuple of two DataFrames:
-            1. forecast_df: The prepared sales history without the product column.
-            2. forecast_df_product: The prepared sales history with the product column.
-    """
-    if all_sales_regressors is None:
-        forecast_df_product = fill_missing(
-            sales_history.loc[sales_history['product'] == forecast_product])
-        forecast_df = forecast_df_product.loc[:, ['ds', 'y']].copy(deep=True)
-    else:
-        forecast_df_product = fill_missing(
-            all_sales_regressors.loc[all_sales_regressors['product'] == forecast_product])
-        forecast_df = forecast_df_product.drop(
+    def __init__(self):
+        st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
+        # initialize session_state vars
+        if 'forecast_df' not in st.session_state:
+            st.session_state['forecast_df'] = pd.DataFrame
+        if 'forecast_df_product' not in st.session_state:
+            st.session_state['forecast_df_product'] = pd.DataFrame
+        if 'matched' not in st.session_state:
+            st.session_state['matched'] = None
+        if 'forecast_product' not in st.session_state:
+            st.session_state['forecast_product'] = None
+        if 'all_sales_regressors' not in st.session_state:
+            st.session_state['all_sales_regressors'] = pd.DataFrame
+        # layout page
+        st.title("D2C, Dropship, Marketplace Forecasting")
+        st.header("2. Select product for forecasting.")
+        if 'master_data' not in st.session_state:
+            st.write(
+                "Please go to Load Data and upload a product attribute file to be able to choose a product for forecasting.")
+        else:
+            st.session_state['forecast_product'] = self.select_product(st.session_state['forecast_product'])
+            cola, colb = st.columns(2)
+            self.diplay_product_selected(cola,colb)
+            # Section for identifying similar products
+            st.subheader(
+                "Optional - Match most similar product for sufficient historical data for forecasting. ")
+            st.write("It is necessary to have at minimum one year of sales history for the NeuralPropeht algorithm to pick up on seasonal affects effectively.  For products with not enough sales history, or for new products, we will use Cosine Similarity on the encoded product master to identify a product that is most-similar, and append that to the desired product history to be able to come up with a better forecast. \
+                    For reference on the meaning of Cosine Similarity: https://www.geeksforgeeks.org/cosine-similarity/")
+            st.write("If you loaded additional regressors on the previous page, these will be automatically inner-joined to the forecast product dataset.")
+            # Select if we want to use cosine similarity to extend product history?
+            use_similarity = st.checkbox(
+                "Identify most-similar product to extend historical data for forecasting?", help="Uses cosine similarity to match most-similar product and appends similar product sales to forecast product sales data to be at least one year in length. "
+            )
+            colc, cold = st.columns(2)
+            if use_similarity:
+                self.use_similar(colc, cold)
+            else:
+                self.single_product_setup(colc)
+
+    def get_len_history(self, all_sales_data: pd.DataFrame) -> pd.DataFrame:
+        """
+        Calculate the length of sales history for each product.
+
+        Args:
+            all_sales_data: A DataFrame containing aggregated product sales data.
+
+        Returns:
+            sales_minmax_dates: A DataFrame containing the length of sales history for each product.
+        """
+        sorted_sales = all_sales_data.sort_values(
+            by=['product', 'ds'], ascending=True)
+        sales_minmax_dates = sorted_sales.groupby(
+            'product').agg({'ds': ['min', 'max'], 'y': 'sum'})
+        sales_minmax_dates['len_hist'] = (sales_minmax_dates.loc[:, (
+            'ds', 'max')] - sales_minmax_dates.loc[:, ('ds', 'min')]) / np.timedelta64(1, 'D')
+        return sales_minmax_dates
+
+    @st.cache_data
+    def get_similarities(_self, master_data_enc: pd.DataFrame) -> pd.DataFrame:
+        """
+        Calculate cosine similarity between products based on encoded master data.
+
+        Args:
+            master_data_enc: A DataFrame containing encoded product master data.
+
+        Returns:
+            similarity_df: A DataFrame containing the cosine similarity scores between products.
+        """
+        similarity = cosine_similarity(master_data_enc)
+        similarity_df = pd.DataFrame(similarity,
+                                     index=master_data_enc.index.values,
+                                     columns=master_data_enc.index.values)
+        return similarity_df
+
+    def check_history_needed(self, sales_minmax_dates: pd.DataFrame, product_fcst: str, min_req_hist: float = 366.0):
+        """
+        Check for the minimum history needed for forecasting a specific product.
+
+        Args:
+            sales_minmax_dates: A DataFrame containing the length of sales history for each product.
+            product_fcst: The product to be forecasted.
+            min_req_hist: The minimum required history for forecasting (default: 366 days).
+
+        Returns:
+            min_append_hist_req: The minimum required history to append.
+            cutoff_date: The cutoff date for adding history.
+        """
+        # lookup length of history for that product
+        len_avail_hist = sales_minmax_dates.loc[sales_minmax_dates.index ==
+                                                product_fcst]['len_hist'].values[0]
+        # difference with minimum required history to identify days gap aka minimum required length of history to append
+        min_append_hist_req = int(min_req_hist - len_avail_hist)
+        # identify the cutoff to add the length of history to
+        cutoff_date = sales_minmax_dates.loc[sales_minmax_dates.index == product_fcst][(
+            'ds', 'min')] - timedelta(min_append_hist_req)
+        return min_append_hist_req, cutoff_date.values[0]
+
+    def match_product(self, similarity_df: pd.DataFrame, sales_minmax_dates: pd.DataFrame, product_fcst: str, cutoff_date: np.datetime64,  top_n: int = 1):
+        """
+        Match a product to similar products based on a similarity DataFrame.
+
+        Args:
+            similarity_df: A DataFrame containing the cosine similarity scores between products.
+            sales_minmax_dates: A DataFrame containing the length of sales history for each product.
+            product_fcst: The product to be forecasted.
+            cutoff_date: The cutoff date for adding history.
+            top_n: The number of top similar products desired (default: 1).
+
+        Returns:
+            matched: A list of matched similar products.
+        """
+        # product list of only products that meet minimum length requirements in addition to available history
+        product_list = sales_minmax_dates.loc[sales_minmax_dates[(
+            'ds', 'min')] < cutoff_date].index.values
+        # slice similarity dataframe by the product being forecasted on row-index, and the product list on the column-index
+        product_sim = similarity_df.loc[similarity_df.index ==
+                                        product_fcst, product_list].values[0]
+        # get products sorted by similarity
+        sorted_products = np.argsort(product_sim)[::-1]
+        # get matched product id
+        matched = product_list[sorted_products[1:top_n+1]]
+        return matched
+
+    def fill_missing(self, sales_history: pd.DataFrame) -> pd.DataFrame:
+        """
+        Fill missing values in a sales history DataFrame.
+
+        Args:
+            sales_history: A DataFrame containing sales history data.
+
+        Returns:
+            sales_history: A DataFrame with missing values filled.
+        """
+        sales_history = sales_history.sort_values(by='ds')
+        sales_history.index = pd.to_datetime(sales_history['ds'])
+        sales_history.drop(columns=['ds'], inplace=True)
+        sales_history = sales_history.asfreq('D')
+        # fill all non quantities with forward-fill
+        for col in sales_history.columns:
+            if col != 'y':
+                sales_history[col].fillna(method='ffill', inplace=True)
+        # assume a 0 means no sale for that day
+        sales_history['y'].fillna(0, inplace=True)
+        sales_history.reset_index(inplace=True)
+        return sales_history
+
+    def merge_regressors(self, sales_data, lag_data, future_data=None) -> pd.DataFrame:
+        """
+        Merge sales data with lag and future regressor data.
+
+        Args:
+            sales_data: A DataFrame containing sales data.
+            lag_data: A DataFrame containing lag regressor data.
+            future_data: A DataFrame containing future regressor data (optional).
+
+        Returns:
+            all_sales_data_lag: A DataFrame with sales data merged with lag and future regressor data.
+        """
+        all_sales_data_lag = pd.merge(
+            sales_data, lag_data, on='ds', how='inner')
+        return all_sales_data_lag
+
+    def append_history(self, all_sales_data: pd.DataFrame, matched: list, product_fcst: str, lag_data: pd.DataFrame = None) -> pd.DataFrame:
+        """
+        Append sales history for a product with the history of a similar product.
+
+        Args:
+            all_sales_data: A DataFrame containing aggregated product sales data.
+            matched: A list of matched similar products.
+            product_fcst: The product to be forecasted.
+            lag_data: A DataFrame containing lag regressor data (optional).
+
+        Returns:
+            A tuple of two DataFrames:
+                1. appended_history: The appended sales history.
+                2. appended_history_product: The appended sales history with the product column.
+        """
+        product_history = all_sales_data.loc[all_sales_data['product']
+                                             == product_fcst]
+        min_date = product_history['ds'].min()
+        extra_history = all_sales_data.loc[all_sales_data['product'] == matched[0]]
+        extra_history = extra_history.loc[extra_history['ds'] < min_date]
+        appended_history_product = self.fill_missing(
+            pd.concat([product_history, extra_history]))
+        if lag_data is not None:
+            appended_history_product = self.merge_regressors(
+                appended_history_product, lag_data)
+        appended_history = appended_history_product.drop(
             columns='product').copy(deep=True)
-    return forecast_df, forecast_df_product
+        return appended_history, appended_history_product
 
+    def prepare_non_appended(self, sales_history: pd.DataFrame, forecast_product: str, all_sales_regressors: pd.DataFrame = None):
+        """
+        Prepare sales history for a product without appending additional history from similar products.
+
+        Args:
+            sales_history: A DataFrame containing sales history data.
+            forecast_product: The product to be forecasted.
+            all_sales_regressors: A DataFrame containing sales data with additional regressors (optional).
+
+        Returns:
+            A tuple of two DataFrames:
+                1. forecast_df: The prepared sales history without the product column.
+                2. forecast_df_product: The prepared sales history with the product column.
+        """
+        if all_sales_regressors is None:
+            forecast_df_product = self.fill_missing(
+                sales_history.loc[sales_history['product'] == forecast_product])
+            forecast_df = forecast_df_product.loc[:, [
+                'ds', 'y']].copy(deep=True)
+        else:
+            forecast_df_product = self.fill_missing(
+                all_sales_regressors.loc[all_sales_regressors['product'] == forecast_product])
+            forecast_df = forecast_df_product.drop(
+                columns='product').copy(deep=True)
+        return forecast_df, forecast_df_product
+
+    def clear_state(self, key: str):
+        """
+        Clear the session state for a specified key.
+
+        Args:
+            key: The key to be cleared from the session state.
+        """
+        if key in st.session_state:
+            st.session_state[key] = None
+
+    def select_product(self, selected_product):
+        if selected_product is not None:
+            forecast_product = st.table(st.session_state['master_data']).selectbox('Select a product ID',
+                                                                                   st.session_state[
+                                                                                       'master_data'].index,
+                                                                                   index=st.session_state['master_data'].index.get_loc(
+                                                                                       st.session_state['forecast_product']),
+                                                                                   on_change=self.clear_state('matched'))
+        else:
+            forecast_product = st.table(st.session_state['master_data']).selectbox('Select a product ID',
+                                                                                   st.session_state[
+                                                                                       'master_data'].index,
+                                                                                   index=0,
+                                                                                   on_change=self.clear_state('matched'))
+        return forecast_product
+
+    def diplay_product_selected(self, cola, colb):
+        with cola:
+            st.write("You selected:", st.session_state['forecast_product'])
+            st.write(
+                st.session_state['master_data'].loc[st.session_state['forecast_product']])
+        with colb:
+            if not st.session_state['all_sales_data'].empty:
+                if not st.session_state['lag_data'].empty:
+                    st.session_state['all_sales_regressors'] = pd.DataFrame
+                    st.session_state['all_sales_regressors'] = self.merge_regressors(
+                        st.session_state['all_sales_data'], st.session_state['lag_data'])
+                    st.write("Sales history:")
+                    st.write(st.session_state['all_sales_regressors'].loc[st.session_state['all_sales_regressors']['product'] == st.session_state['forecast_product'], :]
+                             .sort_values(by='ds'))
+                else:
+                    st.write("Sales history:")
+                    st.write(st.session_state['all_sales_data'].loc[st.session_state['all_sales_data']
+                                                                    ['product'] == st.session_state['forecast_product'], :])
+            else:
+                st.write("Please load sales history data for the product ",
+                         st.session_state['forecast_product'], " before proceeding further.")
 
-def clear_state(key: str):
-    """
-    Clear the session state for a specified key.
-
-    Args:
-        key: The key to be cleared from the session state.
-    """
-    if key in st.session_state:
-        st.session_state[key] = None
-
-
-if 'forecast_df' not in st.session_state:
-    st.session_state['forecast_df'] = pd.DataFrame
-
-if 'forecast_df_product' not in st.session_state:
-    st.session_state['forecast_df_product'] = pd.DataFrame
-
-if 'matched' not in st.session_state:
-    st.session_state['matched'] = None
-
-if 'forecast_product' not in st.session_state:
-    st.session_state['forecast_product'] = None
-
-
-# Title
-st.title("D2C, Dropship, Marketplace Forecasting")
-
-# Select the product that will be used for forecasting.
-st.header("2. Select product for forecasting.")
-
-if 'master_data' not in st.session_state:
-    st.write("Please go to Load Data and upload a product attribute file to be able to choose a product for forecasting.")
-else:
-    if st.session_state['forecast_product'] is not None:
-        st.session_state['forecast_product'] = forecast_product = st.table(st.session_state['master_data']).selectbox('Select a product ID',
-                                                                                                                      st.session_state[
-                                                                                                                          'master_data'].index,
-                                                                                                                      index=st.session_state['master_data'].index.get_loc(
-                                                                                                                          st.session_state['forecast_product']),
-                                                                                                                      on_change=clear_state('matched'))
-    else:
-        st.session_state['forecast_product'] = forecast_product = st.table(st.session_state['master_data']).selectbox('Select a product ID',
-                                                                                                                      st.session_state[
-                                                                                                                          'master_data'].index,
-                                                                                                                      index=0,
-                                                                                                                      on_change=clear_state('matched'))
-    cola, colb = st.columns(2)
-    with cola:
-        st.write("You selected:", st.session_state['forecast_product'])
-        st.write(
-            st.session_state['master_data'].loc[st.session_state['forecast_product']])
-    with colb:
+    def use_similar(self, colc, cold):
         if 'all_sales_data' in st.session_state:
-            if 'lag_data' in st.session_state:
-                st.session_state['all_sales_regressors'] = pd.DataFrame
-                st.session_state['all_sales_regressors'] = merge_regressors(
-                    st.session_state['all_sales_data'], st.session_state['lag_data'])
-                st.write("Sales history:")
-                st.write(st.session_state['all_sales_regressors'].loc[st.session_state['all_sales_regressors']['product'] == st.session_state['forecast_product'], :]
-                         .sort_values(by='ds'))
+            # This sets up base values for calculating and appending history based on the uploaded data
+            sales_minmax_dates = self.get_len_history(
+                st.session_state['all_sales_data'])
+            top_n = 1  # Only find one most-similar product to matach and append history
+            similarity_df = self.get_similarities(
+                st.session_state['master_data_enc'])
+            min_append_hist_req, cutoff_date = self.check_history_needed(
+                sales_minmax_dates, st.session_state['forecast_product'])
+
+            # Determine if history appendage is required, and if so, append history of the most-similar identified product
+            if min_append_hist_req > 0:
+                st.session_state['matched'] = self.match_product(
+                    similarity_df, sales_minmax_dates, st.session_state['forecast_product'], cutoff_date, top_n)
+                if not st.session_state['lag_data'].empty:
+                    st.session_state['forecast_df'], st.session_state['forecast_df_product'] = self.append_history(st.session_state['all_sales_data'],
+                                                                                                                   st.session_state[
+                                                                                                                       'matched'],
+                                                                                                                   st.session_state[
+                        'forecast_product'],
+                        st.session_state['lag_data'])
+                else:
+                    st.session_state['forecast_df'], st.session_state['forecast_df_product'] = self.append_history(st.session_state['all_sales_data'],
+                                                                                                                   st.session_state[
+                                                                                                                       'matched'],
+                                                                                                                   st.session_state[
+                        'forecast_product']
+                    )
             else:
-                st.write("Sales history:")
-                st.write(st.session_state['all_sales_data'].loc[st.session_state['all_sales_data']
-                         ['product'] == st.session_state['forecast_product'], :])
+                if not st.session_state['all_sales_regressors'].empty:
+                    st.session_state['forecast_df'], st.session_state['forecast_df_product'] = self.prepare_non_appended(st.session_state['all_sales_data'],
+                                                                                                                         st.session_state[
+                        'forecast_product'],
+                        st.session_state['all_sales_regressors'])
+                else:
+                    st.session_state['forecast_df'], st.session_state['forecast_df_product'] = self.prepare_non_appended(st.session_state['all_sales_data'],
+                                                                                                                         st.session_state['forecast_product'])
+
+            if 'forecast_df_product' in st.session_state:
+                with colc:
+                    st.write(
+                        "This is the data-set that will be used for forecasting:")
+                    st.write(st.session_state['forecast_df_product'])
+                with cold:
+                    if st.session_state['matched'] is not None:
+                        st.write(
+                            'Identified most-similar product based on uploaded attributes using cosine similarity:')
+                        st.write(
+                            st.session_state['master_data'].loc[st.session_state['matched']])
+                    else:
+                        st.write(
+                            'Sufficient historical data identified, there is no need to append similar product history.')
         else:
-            st.write("Please load sales history data for the product ",
-                     st.session_state['forecast_product'], " before proceeding further.")
+            st.write(
+                "Please upload sales history from the Load Data page to proceed.")
 
+    def single_product_setup(self, colc):
+        # If the user does not select to append historicals, set up the forecast dataframe with just the chosen product
 
-# Section for identifying similar products
-st.subheader(
-    "Optional - Match most similar product for sufficient historical data for forecasting. ")
-
-
-st.write("It is necessary to have at minimum one year of sales history for the NeuralPropeht algorithm to pick up on seasonal affects effectively.  For products with not enough sales history, or for new products, we will use Cosine Similarity on the encoded product master to identify a product that is most-similar, and append that to the desired product history to be able to come up with a better forecast. \
-        For reference on the meaning of Cosine Similarity: https://www.geeksforgeeks.org/cosine-similarity/")
-st.write("If you loaded additional regressors on the previous page, these will be automatically inner-joined to the forecast product dataset.")
-
-# Select if we want to use cosine similarity to extend product history?
-use_similarity = st.checkbox(
-    "Identify most-similar product to extend historical data for forecasting?", help="Uses cosine similarity to match most-similar product and appends similar product sales to forecast product sales data to be at least one year in length. "
-)
-
-
-colc, cold = st.columns(2)
-if use_similarity:
-    if 'all_sales_data' in st.session_state:
-        # This sets up base values for calculating and appending history based on the uploaded data
-        sales_minmax_dates = get_len_history(
-            st.session_state['all_sales_data'])
-        top_n = 1  # Only find one most-similar product to matach and append history
-        similarity_df = get_similarities(st.session_state['master_data_enc'])
-        min_append_hist_req, cutoff_date = check_history_needed(
-            sales_minmax_dates, st.session_state['forecast_product'])
-
-        # Determine if history appendage is required, and if so, append history of the most-similar identified product
-        if min_append_hist_req > 0:
-            st.session_state['matched'] = match_product(
-                similarity_df, sales_minmax_dates, st.session_state['forecast_product'], cutoff_date, top_n)
-            if 'lag_data' in st.session_state:
-                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = append_history(st.session_state['all_sales_data'],
-                                                                                                          st.session_state['matched'],
-                                                                                                          st.session_state[
-                    'forecast_product'],
-                    st.session_state['lag_data'])
-            else:
-                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = append_history(st.session_state['all_sales_data'],
-                                                                                                          st.session_state['matched'],
-                                                                                                          st.session_state[
-                    'forecast_product']
-                )
-        else:
-            if 'all_sales_regressors' in st.session_state:
-                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = prepare_non_appended(st.session_state['all_sales_data'],
-                                                                                                                st.session_state[
-                    'forecast_product'],
-                    st.session_state['all_sales_regressors'])
+        if not st.session_state['all_sales_data'].empty:
+            if not st.session_state['all_sales_regressors'].empty:
+                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = self.prepare_non_appended(st.session_state['all_sales_data'],
+                                                                                                                     st.session_state[
+                                                                                                                         'forecast_product'],
+                                                                                                                     st.session_state['all_sales_regressors'])
             else:
-                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = prepare_non_appended(st.session_state['all_sales_data'],
-                                                                                                                st.session_state['forecast_product'])
-
-        if 'forecast_df_product' in st.session_state:
+                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = self.prepare_non_appended(st.session_state['all_sales_data'],
+                                                                                                                     st.session_state['forecast_product'])
             with colc:
                 st.write("This is the data-set that will be used for forecasting:")
                 st.write(st.session_state['forecast_df_product'])
-            with cold:
-                if st.session_state['matched'] is not None:
-                    st.write(
-                        'Identified most-similar product based on uploaded attributes using cosine similarity:')
-                    st.write(
-                        st.session_state['master_data'].loc[st.session_state['matched']])
-                else:
-                    st.write(
-                        'Sufficient historical data identified, there is no need to append similar product history.')
-    else:
-        st.write("Please upload sales history from the Load Data page to proceed.")
-
-else:
-    # If the user does not select to append historicals, set up the forecast dataframe with just the chosen product
-
-    if 'all_sales_data' in st.session_state:
-        if 'all_sales_regressors' in st.session_state:
-            st.session_state['forecast_df'], st.session_state['forecast_df_product'] = prepare_non_appended(st.session_state['all_sales_data'],
-                                                                                                            st.session_state[
-                'forecast_product'],
-                st.session_state['all_sales_regressors'])
         else:
-            st.session_state['forecast_df'], st.session_state['forecast_df_product'] = prepare_non_appended(st.session_state['all_sales_data'],
-                                                                                                            st.session_state['forecast_product'])
-        with colc:
-            st.write("This is the data-set that will be used for forecasting:")
-            st.write(st.session_state['forecast_df_product'])
-    else:
-        st.write("Please upload sales history from the Load Data page to proceed.")
+            st.write(
+                "Please upload sales history from the Load Data page to proceed.")
+
+
+if __name__ == '__main__':
+    ps = ProductSelection()
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_3_Tune_and_Train.py` & `d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_3_Tune_and_Train.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,328 +6,329 @@
 from datetime import date
 from datetime import timedelta
 from neuralprophet import NeuralProphet, set_log_level, set_random_seed, utils
 from sklearn.metrics import mean_squared_error
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_absolute_percentage_error
 
-# Page config
-st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
 
-
-@st.cache_resource(show_spinner=False)
-def fit_complete(params: dict, df: pd.DataFrame, events_df: pd.DataFrame = None, fit_spinner_text="Fitting the model for product") -> NeuralProphet:
-    """
-    Fit a NeuralProphet model to the complete dataset using the selected params or the best parameters obtained from cross-validation.
-
-    Args:
-        params: A dictionary containing the best hyperparameters.
-        df: A DataFrame containing the dataset to be fit.
-        events_df: A DataFrame containing events data (optional).
-
-    Returns:
-        A fitted NeuralProphet model.
-    """
-    # Fit the whole training set with best params
-    with st.spinner(fit_spinner_text):
+class TuneTrain:
+    def __init__(self):
+        # Initialize state-dependent streamlit variables
+        if 'hyperparam_options' not in st.session_state:
+            st.session_state['hyperparam_options'] = {}
+        if 'selected_options' not in st.session_state:
+            st.session_state['selected_options'] = {}
+        if 'iter_selections' not in st.session_state:
+            st.session_state['iter_selections'] = None
+        if 'best_params' not in st.session_state:
+            st.session_state["best_params"] = {}
+        if 'metrics_test' not in st.session_state:
+            st.session_state["metrics_test"] = pd.DataFrame()
+        if 'm' not in st.session_state:
+            st.session_state['m'] = None
+        if 'forecast_df' not in st.session_state:
+            st.session_state['forecast_df'] = pd.DataFrame()
+        if 'forecast_product' not in st.session_state:
+            st.session_state['forecast_product'] = None
+        if 'fit_flag' not in st.session_state:
+            st.session_state['fit_flag'] = False
+        if 'events_df' not in st.session_state:
+            st.session_state['events_df'] = pd.DataFrame()
+        normalize_list = ['soft', 'minmax', 'soft1', 'standardize', 'off']
+        # Layout page
+        st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
+        st.header("3. Select, tune, and train the forecasting model.")
+        if st.session_state['forecast_df'].empty:
+            st.write(
+                "Please first load sales data and select a product to forecast to be able to setup and train a forecasting model.")
+        else:
+            fit_spinner_text = "Fitting the model for product " + \
+                st.session_state['forecast_product'] + \
+                " with selected hyperparameters..."
+            tab_auto, tab_select = st.tabs(
+                ["Automatic Hyperparameter Tuning", "Manual Hyperparameter Selection"])
+            with tab_select:
+                st.subheader("Select hyperparamters to tune a forecasting model for the selected product: ",
+                             st.session_state['forecast_product'])
+                self.tab_select_form(normalize_list)
+                # Print selected options from form
+                st.write("Selected options:")
+                st.write(st.session_state['selected_options'])
+                if st.session_state['selected_options']:
+                    # Cross-Validation Option
+                    with st.expander("Cross-Validation"):
+                        if st.button("Cross-Validate"):
+                            with st.spinner("Performing cross-validation... (Please do not refresh or close this tab while running to complete this task.)"):
+                                st.session_state['metrics_test'], st.session_state['selected_options'] = self.cross_validate(
+                                    st.session_state['forecast_df'],
+                                    st.session_state['forecast_product'],
+                                    st.session_state['selected_options'],
+                                    st.session_state['events_df'])
+                            st.success("Cross-validation complete!", icon="✅")
+                        else:
+                            st.write(
+                                "Push \"Cross-Validate\" to perform 5-fold backtesting cross-validation with your selected hyperparameters.")
+                    # Fit complete dataset (required step for forecasting)
+                    with st.expander("Fit Model to Complete Dataset"):
+                        st.write("Current Identified Best Parameters: ")
+                        st.write(st.session_state['selected_options'])
+                        if st.button("Fit Model", key='fit_select'):
+                            with st.spinner(fit_spinner_text):
+                                st.session_state["m"], fit_metrics = self.fit_complete(params=st.session_state['selected_options'],
+                                                                          df=st.session_state['forecast_df'],
+                                                                          events_df=st.session_state['events_df'])
+                                st.write("Metrics from model fit:", fit_metrics)
+                                st.session_state['fit_flag'] = True
+                            st.success("Model fit complete!", icon="✅")
+                        else:
+                            st.write(
+                                "Fit the model with the full data-set for the selected product.  This is required for moving to forecast prediction.")
+            with tab_auto:
+                st.subheader("Select options and ranges for an automated grid-search to find the best hyperparameters: ",
+                             st.session_state['forecast_product'])
+                self.tab_auto_form(normalize_list)
+                st.write("Selected options:")
+                st.write(st.session_state['hyperparam_options'])
+                if st.session_state['hyperparam_options']:
+                    # Grid Search for Hyperparameter option
+                    with st.expander("Hyperparameter Search"):
+                        if st.button("Grid Search"):
+                            with st.spinner("Performing cross-validation... (Please do not refresh or close this tab while running to complete this task.)"):
+                                st.session_state['metrics_test'], st.session_state['best_params'] = self.cross_validate(
+                                    st.session_state['forecast_df'],
+                                    st.session_state['forecast_product'],
+                                    st.session_state['hyperparam_options'],
+                                    st.session_state['events_df'])
+                            st.success("Cross-validation complete!", icon="✅")
+                        else:
+                            st.write(
+                                "Push \"Cross-Validate\" to Grid Search for best hyperparameters using 5-fold backtesting cross-validation.")
+                    if st.session_state['best_params']:
+                        # Fit complete model after hyperparameter best are identified
+                        with st.expander("Fit Model to Complete Dataset"):
+                            st.write("Current Identified Best Parameters: ")
+                            st.write(st.session_state['best_params'])
+                            if st.button("Fit Model", key='fit_auto'):
+                                with st.spinner(fit_spinner_text):
+                                    st.session_state["m"], fit_metrics = self.fit_complete(params=st.session_state['best_params'],
+                                                                              df=st.session_state['forecast_df'],
+                                                                              events_df=st.session_state['events_df'])
+                                st.success("Model fit complete!", icon="✅")
+                            else:
+                                st.write("Fit the model with the full data-set and best hyperparameters from grid search for the selected product.  \n",
+                                         "This is required for moving to forecast prediction.")
+
+    @st.cache_resource(show_spinner=False)
+    def fit_complete(_self, params: dict, df: pd.DataFrame, events_df: pd.DataFrame = None) -> tuple:
+        """
+        Fit a NeuralProphet model to the complete dataset using the selected params or the best parameters obtained from cross-validation.
+
+        Args:
+            params: A dictionary containing the best hyperparameters.
+            df: A DataFrame containing the dataset to be fit.
+            events_df: A DataFrame containing events data (optional).
+
+        Returns:
+            A fitted NeuralProphet model.
+        """
+        # Fit the whole training set with best params
         m = NeuralProphet(**params)
         for col in df.columns:
             if col != 'y' and col != 'ds':
                 m = m.add_lagged_regressor(names=col)
-        if events_df is not None:
+        if not events_df.empty:
+            # Need to update this so it is flexible to different holiday names
             m.add_events(['Cyber Week'], mode='additive')
             data_ev = m.create_df_with_events(df, events_df)
             fit_metrics = m.fit(df=data_ev, freq="D")
         else:
             fit_metrics = m.fit(df=df, freq="D")
-        st.write("Metrics from model fit:", fit_metrics)
-        st.session_state['fit_flag'] = True
-    st.success("Model fit complete!", icon="✅")
-    return m
-
-
-@st.cache_resource(show_spinner=False)
-def cross_val_tune(params: dict, df: pd.DataFrame, forecast_product: str, events_df: pd.DataFrame = None, horizon: int = 30) -> tuple:
-    """
-    Perform hyperparameter tuning using cross-validation for a given forecast product.
+        return m, fit_metrics
 
-    Args:
-        params: A dictionary containing the parameters to be tuned.
-        df: A DataFrame containing the dataset.
-        forecast_product: The product to be forecasted.
-        events_df: A DataFrame containing events data (optional).
-        horizon: The forecast horizon in days (default: 30).
-
-    Returns:
-        A tuple containing:
-            1. best_metrics: A DataFrame containing the best test metrics from cross-validation.
-            2. best_params: A dictionary containing the best hyperparameters.
-    """
-    METRICS = ["MAE", "RMSE"]
-    fold_pct = horizon/len(df)
-
-    st.write(
-        "Applying five-fold cross-validation to the forecast model for " + forecast_product)
-
-    param_grid = params
-
-    # Generate all combinations of parameters
-    all_params = [dict(zip(param_grid.keys(), v))
-                  for v in itertools.product(*param_grid.values())]
-    cv_test_loss = []
-    test_metrics_list = []
-    best_metrics = []
-
-    # Use cross validation to evaluate all parameters
-    for i, params in enumerate(all_params):
-        folds = NeuralProphet(**params).crossvalidation_split_df(df,
-                                                                 freq="D", k=5, fold_pct=fold_pct, fold_overlap_pct=0)
-        metrics_train = pd.DataFrame(columns=METRICS)
-        metrics_test = pd.DataFrame(columns=METRICS)
-        for df_train, df_test in folds:
-            m = NeuralProphet(**params)
-            for col in df.columns:
-                if col != 'y' and col != 'ds':
-                    m = m.add_lagged_regressor(names=col)
-            if events_df is not None:
-                m.add_events(['Cyber Week'], mode='additive')
-                df_train_ev = m.create_df_with_events(df_train, events_df)
-                df_test_ev = m.create_df_with_events(df_test, events_df)
-                train = m.fit(df=df_train_ev, freq="D")
-                test = m.test(df=df_test_ev)
-            else:
-                train = m.fit(df=df_train, freq="D")
-                test = m.test(df=df_test)
-            metrics_train = metrics_train.append(train.iloc[-1])
-            metrics_test = metrics_test.append(test.iloc[-1])
-        cv_test_loss.append(metrics_test['MSELoss'].mean())
-        test_metrics_list.append(metrics_test)
-    best_params = all_params[np.argmin(cv_test_loss)]
-    best_metrics = test_metrics_list[np.argmin(cv_test_loss)]
-
-    st.write("Best model test metrics from cross-validation:")
-    st.write(best_metrics)
-    st.write("Best model test metrics mean across 5 folds: ")
-    st.write(best_metrics.mean())
-    st.write("Resulting hyperparmeters from cross-validation:")
-    st.write(best_params)
+    @st.cache_resource(show_spinner=False)
+    def cross_val_tune(_self, params: dict, df: pd.DataFrame, forecast_product: str, events_df: pd.DataFrame = None, horizon: int = 30) -> tuple:
+        """
+        Perform hyperparameter tuning using cross-validation for a given forecast product.
+
+        Args:
+            params: A dictionary containing the parameters to be tuned.
+            df: A DataFrame containing the dataset.
+            forecast_product: The product to be forecasted.
+            events_df: A DataFrame containing events data (optional).
+            horizon: The forecast horizon in days (default: 30).
+
+        Returns:
+            A tuple containing:
+                1. best_metrics: A DataFrame containing the best test metrics from cross-validation.
+                2. best_params: A dictionary containing the best hyperparameters.
+        """
+        METRICS = ["MAE", "RMSE"]
+        fold_pct = horizon/len(df)
+        st.write(
+            "Applying five-fold cross-validation to the forecast model for " + forecast_product)
+        param_grid = params
+        # Generate all combinations of parameters
+        all_params = [dict(zip(param_grid.keys(), v))
+                      for v in itertools.product(*param_grid.values())]
+        cv_test_loss = []
+        test_metrics_list = []
+        best_metrics = []
+        # Use cross validation to evaluate all parameters
+        for i, params in enumerate(all_params):
+            folds = NeuralProphet(**params).crossvalidation_split_df(df,
+                                                                     freq="D", k=5, fold_pct=fold_pct, fold_overlap_pct=0)
+            metrics_train = pd.DataFrame(columns=METRICS)
+            metrics_test = pd.DataFrame(columns=METRICS)
+            for df_train, df_test in folds:
+                m = NeuralProphet(**params)
+                for col in df.columns:
+                    if col != 'y' and col != 'ds':
+                        m = m.add_lagged_regressor(names=col)
+                if not events_df.empty:
+                    # Need to update this so that it is flexible to different holidays
+                    m.add_events(['Cyber Week'], mode='additive')
+                    df_train_ev = m.create_df_with_events(df_train, events_df)
+                    df_test_ev = m.create_df_with_events(df_test, events_df)
+                    train = m.fit(df=df_train_ev, freq="D")
+                    test = m.test(df=df_test_ev)
+                else:
+                    train = m.fit(df=df_train, freq="D")
+                    test = m.test(df=df_test)
+                metrics_train = metrics_train.append(train.iloc[-1])
+                metrics_test = metrics_test.append(test.iloc[-1])
+            cv_test_loss.append(metrics_test['MSELoss'].mean())
+            test_metrics_list.append(metrics_test)
+        best_params = all_params[np.argmin(cv_test_loss)]
+        best_metrics = test_metrics_list[np.argmin(cv_test_loss)]
+        st.write("Best model test metrics from cross-validation:")
+        st.write(best_metrics)
+        st.write("Best model test metrics mean across 5 folds: ")
+        st.write(best_metrics.mean())
+        st.write("Resulting hyperparmeters from cross-validation:")
+        st.write(best_params)
+        return best_metrics, best_params
+
+    @st.cache_resource(show_spinner=False)
+    def selections_to_lists(_self, selected_options: dict) -> dict:
+        """
+        Convert selected_options dictionary values to lists.
 
-    return best_metrics, best_params
+        Args:
+            selected_options (dict): A dictionary containing selected options.
 
-
-def is_events():
-    """
-    Check if events data is available in the session state.
-
-    Returns:
-        The events data if available, otherwise None.
+        Returns:
+            dict: A dictionary with values converted to lists.
     """
-    if 'events_df' in st.session_state:
-        return st.session_state['events_df']
-    else:
-        return None
-
-# Setup key session_state variables needed for cross-page use
-
-
-if 'hyperparam_options' not in st.session_state:
-    st.session_state['hyperparam_options'] = {}
-
-if 'selected_options' not in st.session_state:
-    st.session_state['selected_options'] = {}
-
-if 'best_params' not in st.session_state:
-    st.session_state["best_params"] = {}
-
-if 'metrics_test' not in st.session_state:
-    st.session_state["metrics_test"] = pd.DataFrame()
-
-if 'm' not in st.session_state:
-    st.session_state['m'] = None
-
-if 'forecast_df' not in st.session_state:
-    st.session_state['forecast_df'] = pd.DataFrame()
-
-if 'fit_flag' not in st.session_state:
-    st.session_state['fit_flag'] = False
-
-normalize_list = ['soft', 'minmax', 'soft1', 'standardize', 'off']
-
-# Start section for formatting the page
-
-st.header("3. Select, tune, and train the forecasting model.")
-
-if 'forecast_df' in st.session_state:
-    if st.session_state['forecast_df'].empty:
-        st.write("Please first load sales data and select a product to forecast to be able to setup and train a forecasting model.")
-    else:
-
-        tab_auto, tab_select = st.tabs(
-            ["Automatic Hyperparameter Tuning", "Manual Hyperparameter Selection"])
-
-        # Re-used variables across tabs
-        fit_spinner_text = "Fitting the model for product " + \
-            st.session_state['forecast_product'] + \
-            " with selected hyperparameters..."
-
-        with tab_select:
-
-            st.subheader("Select hyperparamters to tune a forecasting model for the selected product: ",
-                         st.session_state['forecast_product'])
-
-            with st.form("param_grid_form"):
-                # Add a title to the form
-                st.write("Select options for param_grid")
-
-                # Define the options for each parameter
-                seasonality_mode_options = st.selectbox(
-                    'Select seasonality_mode', ['additive', 'multiplicative'])
-                loss_func_options = st.selectbox(
-                    'Select loss_func', ['MSE', 'MAE'])
-                n_changepoints = 10
-                n_changepoints_options = st.slider(
-                    'Select n_changepoints', min_value=1, max_value=20, value=n_changepoints)
-                changepoints_range = 10.0
-                changepoints_range_options = st.slider(
-                    'Select changepoints_range', min_value=0.01, max_value=20.0, value=changepoints_range)
-                normalize_options = st.selectbox(
-                    'Select normalization method', normalize_list)
-                n_lags_options = st.slider(
-                    'Select n_lags', min_value=7, max_value=90, value=30)
-                n_forecasts_options = st.slider(
-                    'Select n_forecasts', min_value=7, max_value=90, value=30)
-                num_hidden_layers_options = st.selectbox(
-                    'Select num_hidden_layers', [0, 1, 2])
-
-                # Add a submit button to the form
-                submitted = st.form_submit_button("Submit")
-
-                # If the user submitted the form, print the selected options
-                if submitted:
-                    # Create a dictionary to store the selected options
-                    st.session_state['selected_options'] = {
-                        'seasonality_mode': seasonality_mode_options,
-                        'loss_func': loss_func_options,
-                        'n_changepoints': n_changepoints_options,
-                        'changepoints_range': changepoints_range_options,
-                        'normalize': normalize_options,
-                        'num_hidden_layers': num_hidden_layers_options,
-                        'n_lags': n_lags_options,
-                        'n_forecasts': n_forecasts_options
-                    }
-
-                    # Also store iterable version of params dict for common cross-validation function use.
-                    def selections_to_lists(x): return {
-                        k: [v] for k, v in x.items()}
-                    st.session_state['iter_selections'] = selections_to_lists(
-                        st.session_state['selected_options'])
-
-                st.write("Selected options:")
-                st.write(st.session_state['selected_options'])
-
-            if st.session_state['selected_options']:
-
-                with st.expander("Cross-Validation"):
-                    if st.button("Cross-Validate"):
-                        with st.spinner("Performing cross-validation... (Please do not refresh or close this tab while running to complete this task.)"):
-                            st.session_state['metrics_test'], st.session_state['selected_options'] = cross_val_tune(
-                                params=st.session_state['iter_selections'],
-                                df=st.session_state['forecast_df'],
-                                forecast_product=st.session_state['forecast_product'],
-                                events_df=is_events(),
-                                horizon=int(st.session_state['selected_options']['n_forecasts']))
-                        st.success("Cross-validation complete!", icon="✅")
-                    else:
-                        st.write(
-                            "Push \"Cross-Validate\" to perform 5-fold backtesting cross-validation with your selected hyperparameters.")
-
-                with st.expander("Fit Model to Complete Dataset"):
-                    st.write("Current Identified Best Parameters: ")
-                    st.write(st.session_state['selected_options'])
-                    if st.button("Fit Model", key='fit_select'):
-                        st.session_state["m"] = fit_complete(params=st.session_state['selected_options'],
-                                                             df=st.session_state['forecast_df'],
-                                                             events_df=is_events(),
-                                                             fit_spinner_text=fit_spinner_text)
-                    else:
-                        st.write(
-                            "Fit the model with the full data-set for the selected product.  This is required for moving to forecast prediction.")
-
-            with tab_auto:
-
-                st.subheader("Select options and ranges for an automated grid-search to find the best hyperparameters: ",
-                             st.session_state['forecast_product'])
+        return {k: [v] for k, v in selected_options.items()}
 
-                with st.form("hyper_grid_form"):
-                    # Add a title to the form
-                    st.write("Select options for hyperparameter search.")
-
-                    # Define the options for each parameter
-                    seasonality_mode_options = st.multiselect(
-                        'Select seasonality_mode', ['additive', 'multiplicative'], default='additive')
-                    loss_func_options = st.multiselect(
-                        'Select loss_func', ['MSE', 'MAE'], default='MSE')
-                    n_cp_min, n_cp_max = st.slider(
-                        'Select n_changepoints (min=1/max=20)', min_value=1, max_value=20, value=(5, 10))
-                    n_cp_steps = st.number_input(
-                        'Select step-size for n_changepoints (min=1/max=10)', min_value=1, max_value=10, value=5)
-                    cp_range_min, cp_range_max = st.slider(
-                        'Select changepoints_range (min=0.01/max=20.0)', min_value=0.01, max_value=20.0, value=(1.0, 10.0))
-                    cp_range_steps = st.number_input(
-                        'Select step-size for n_changepoints (min=0.01/max=10.0)', min_value=0.01, max_value=10.0, value=9.0)
-                    normalize_options = st.multiselect(
-                        'Select normalization method', normalize_list, default='soft')
-                    n_lags_options = st.slider(
-                        'Select n_lags', min_value=7, max_value=90, value=30)
-                    n_forecasts_options = st.slider(
-                        'Select n_forecasts', min_value=7, max_value=90, value=30)
-                    num_hidden_layers_options = st.multiselect(
-                        'Select num_hidden_layers', [0, 1, 2], default=0)
-
-                    # Add a submit button to the form
-                    submitted = st.form_submit_button("Submit")
-
-                    # If the user submitted the form, print the selected options
-                    if submitted:
-                        # Create a dictionary to store the selected options
-                        st.session_state['hyperparam_options'] = {
-                            'seasonality_mode': seasonality_mode_options,
-                            'loss_func': loss_func_options,
-                            'n_changepoints': np.arange(n_cp_min, n_cp_max+1, n_cp_steps).tolist(),
-                            'changepoints_range': np.arange(cp_range_min, cp_range_max+0.01, cp_range_steps).tolist(),
-                            'normalize': normalize_options,
-                            'num_hidden_layers': num_hidden_layers_options,
-                            'n_lags': [n_lags_options],
-                            'n_forecasts': [n_forecasts_options]
-
-                        }
+    @st.cache_resource(show_spinner=False)
+    def cross_validate(_self, forecast_df: pd.DataFrame, forecast_product: str, selected_options: dict, events_df: pd.DataFrame = None) -> tuple:
+        """
+        Perform cross-validation for the NeuralProphet model.
+
+        Args:
+            forecast_df (pd.DataFrame): DataFrame containing forecast data.
+            forecast_product (str): The product for forecasting.
+            selected_options (dict): A dictionary containing selected options.
+
+        Returns:
+            tuple: A tuple containing the test metrics and updated selected options.
+        """
+        if isinstance(selected_options['n_changepoints'], list):
+            iter_selections = selected_options
+        else:
+            iter_selections = _self.selections_to_lists(selected_options)
+        metrics_test, selected_options = _self.cross_val_tune(
+            params=iter_selections,
+            df=forecast_df,
+            forecast_product=forecast_product,
+            events_df=events_df,
+            horizon=int(iter_selections['n_forecasts'][0]))
+        return metrics_test, selected_options
+
+    def tab_select_form(self, normalize_list: list):
+        """
+        Create a form to select options for param_grid.
+        """
+        with st.form("param_grid_form"):
+            # Add a title to the form
+            st.write("Select options for param_grid")
+            # Define the options for each parameter
+            seasonality_mode_options = st.selectbox(
+                'Select seasonality_mode', ['additive', 'multiplicative'])
+            loss_func_options = st.selectbox(
+                'Select loss_func', ['MSE', 'MAE'])
+            n_changepoints = 10
+            n_changepoints_options = st.slider(
+                'Select n_changepoints', min_value=1, max_value=20, value=n_changepoints)
+            changepoints_range = 10.0
+            changepoints_range_options = st.slider(
+                'Select changepoints_range', min_value=0.01, max_value=20.0, value=changepoints_range)
+            normalize_options = st.selectbox(
+                'Select normalization method', normalize_list)
+            n_lags_options = st.slider(
+                'Select n_lags', min_value=7, max_value=90, value=30)
+            n_forecasts_options = st.slider(
+                'Select n_forecasts', min_value=7, max_value=90, value=30)
+            num_hidden_layers_options = st.selectbox(
+                'Select num_hidden_layers', [0, 1, 2])
+            # Add a submit button to the form
+            submitted = st.form_submit_button("Submit")
+            if submitted:
+                st.session_state['selected_options'] = {
+                    'seasonality_mode': seasonality_mode_options,
+                    'loss_func': loss_func_options,
+                    'n_changepoints': n_changepoints_options,
+                    'changepoints_range': changepoints_range_options,
+                    'normalize': normalize_options,
+                    'num_hidden_layers': num_hidden_layers_options,
+                    'n_lags': n_lags_options,
+                    'n_forecasts': n_forecasts_options
+                }
+
+    def tab_auto_form(self, normalize_list: list):
+        """
+        Create a form to select options for param_grid.
+        """
+        with st.form("hyper_grid_form"):
+            # Add a title to the form
+            st.write("Select options for hyperparameter search.")
+            # Define the options for each parameter
+            seasonality_mode_options = st.multiselect(
+                'Select seasonality_mode', ['additive', 'multiplicative'], default='additive')
+            loss_func_options = st.multiselect(
+                'Select loss_func', ['MSE', 'MAE'], default='MSE')
+            n_cp_min, n_cp_max = st.slider(
+                'Select n_changepoints (min=1/max=20)', min_value=1, max_value=20, value=(5, 10))
+            n_cp_steps = st.number_input(
+                'Select step-size for n_changepoints (min=1/max=10)', min_value=1, max_value=10, value=5)
+            cp_range_min, cp_range_max = st.slider(
+                'Select changepoints_range (min=0.01/max=20.0)', min_value=0.01, max_value=20.0, value=(1.0, 10.0))
+            cp_range_steps = st.number_input(
+                'Select step-size for n_changepoints (min=0.01/max=10.0)', min_value=0.01, max_value=10.0, value=9.0)
+            normalize_options = st.multiselect(
+                'Select normalization method', normalize_list, default='soft')
+            n_lags_options = st.slider(
+                'Select n_lags', min_value=7, max_value=90, value=30)
+            n_forecasts_options = st.slider(
+                'Select n_forecasts', min_value=7, max_value=90, value=30)
+            num_hidden_layers_options = st.multiselect(
+                'Select num_hidden_layers', [0, 1, 2], default=0)
+            # Add a submit button to the form
+            submitted = st.form_submit_button("Submit")
+            # If the user submitted the form, print the selected options
+            if submitted:
+                st.session_state['hyperparam_options'] = {
+                    'seasonality_mode': seasonality_mode_options,
+                    'loss_func': loss_func_options,
+                    'n_changepoints': np.arange(n_cp_min, n_cp_max+1, n_cp_steps).tolist(),
+                    'changepoints_range': np.arange(cp_range_min, cp_range_max+0.01, cp_range_steps).tolist(),
+                    'normalize': normalize_options,
+                    'num_hidden_layers': num_hidden_layers_options,
+                    'n_lags': [n_lags_options],
+                    'n_forecasts': [n_forecasts_options]
+                }
 
-                    st.write("Selected options:")
-                    st.write(st.session_state['hyperparam_options'])
 
-                if st.session_state['hyperparam_options']:
-                    with st.expander("Hyperparameter Search"):
-                        if st.button("Grid Search"):
-                            with st.spinner("Performing grid search for best hyperparameters... (Please do not refresh or close this tab while running to complete this task.)"):
-                                st.session_state['metrics_test'], st.session_state['best_params'] = cross_val_tune(
-                                    params=st.session_state['hyperparam_options'],
-                                    df=st.session_state['forecast_df'],
-                                    forecast_product=st.session_state['forecast_product'],
-                                    events_df=is_events(),
-                                    horizon=int(st.session_state['hyperparam_options']['n_forecasts'][0]))
-                            st.success("Cross-validation complete!", icon="✅")
-                        else:
-                            st.write(
-                                "Push \"Cross-Validate\" to Grid Search for best hyperparameters using 5-fold backtesting cross-validation.")
-
-                if st.session_state['best_params']:
-                    with st.expander("Fit Model to Complete Dataset"):
-                        st.write("Current Identified Best Parameters: ")
-                        st.write(st.session_state['best_params'])
-                        if st.button("Fit Model", key='fit_auto'):
-                            st.session_state["m"] = fit_complete(params=st.session_state['best_params'],
-                                                                 df=st.session_state['forecast_df'],
-                                                                 events_df=is_events(),
-                                                                 fit_spinner_text=fit_spinner_text)
-                        else:
-                            st.write("Fit the model with the full data-set and best hyperparameters from grid search for the selected product.  \n",
-                                     "This is required for moving to forecast prediction.")
+if __name__ == '__main__':
+    tt = TuneTrain()
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_4_Forecast_Product.py` & `d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_4_Forecast_Product.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,295 +11,259 @@
 from neuralprophet import NeuralProphet, set_log_level, set_random_seed, utils, plot_forecast
 from sklearn.metrics import mean_squared_error
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_absolute_percentage_error
 from sklearn.metrics.pairwise import cosine_similarity
 from d2c_mp_sales_forecaster.utils.db_manager import PostgreSQLManager
 
-# Page config
-st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
 
-@st.cache_data
-def convert_cols_to_int(df):
-    """
-    Convert specified columns of a DataFrame to integers.
-
-    Args:
-        df: A DataFrame containing the columns to be converted.
-
-    Returns:
-        The modified DataFrame with specified columns converted to integers.
-    """
-    for col in df.columns:
-        if col.startswith('y') or col.startswith('residual') or col.startswith('step'):
-            df[col].fillna(0, inplace=True)
-            df[col] = df[col].round(0).astype(int)
-    return df
-
-
-@st.cache_data
-def predict(_m: NeuralProphet, horizon: int, df: pd.DataFrame, events_df: pd.DataFrame = None) -> tuple:
-    """
-    Make predictions using a trained NeuralProphet model.
-
-    Args:
-        _m: A trained NeuralProphet model.
-        horizon: The forecast horizon in days.
-        df: A DataFrame containing the data for prediction.
-        events_df: A DataFrame containing events data (optional).
-
-    Returns:
-        A tuple containing the forecast DataFrame.
-    """
-    with st.spinner("Predicting with model... "):
-        if events_df is not None:
-            data_ev = _m.create_df_with_events(df, events_df)
-            future = _m.make_future_dataframe(
-                df=data_ev, events_df=events_df, periods=horizon)
-        else:
-            future = _m.make_future_dataframe(df=df, periods=horizon)
-        # convert predict output to integers as this application is focused on forecasting QTY which cannot be decimal
-        forecast = convert_cols_to_int(_m.predict(future))
-        # raw_forecast = convert_cols_to_int(_m.predict(future, raw=True))
-    st.success("Prediction complete", icon="✅")
-    return forecast  # , raw_forecast
-
-
-def is_events():
-    """
-    Check if events data is available in the session state.
-
-    Returns:
-        The events data if available, otherwise None.
-    """
-    if 'events_df' in st.session_state:
-        return st.session_state['events_df']
-    else:
-        return None
-
-
-@st.cache_resource
-def convert_df(df):
-    """
-    Convert a DataFrame to a CSV string and encode it as utf-8 bytes.
-
-    Args:
-        df: A DataFrame to be converted.
-
-    Returns:
-        A CSV string of the DataFrame encoded as utf-8 bytes.
-    """
-    return df.to_csv().encode('utf-8')
-
-
-def custom_plot_np_components(model, forecast, components=None):
-    """
-    Create custom component plots for a NeuralProphet model's forecast.
-
-    Args:
-        model: A trained NeuralProphet model.
-        forecast: A DataFrame containing the model's forecast.
-        components: A list of components to be plotted (default: None, which includes 'trend', 'season_yearly', 'season_weekly', and 'AR').
-
-    Returns:
-        A matplotlib figure containing the component plots.
-    """
-    if components is None:
-        components = ['trend', 'season_yearly', 'season_weekly', 'AR']
-
-    n_plots = len(components)
-    fig, axes = plt.subplots(n_plots, 1, figsize=(10, 4 * n_plots))
-    if n_plots == 1:
-        axes = [axes]
-
-    for idx, component in enumerate(components):
-        ax = axes[idx]
-        if component == 'AR':
-            ar_data = model.model.ar_weights.detach().numpy()
-            mean_ar_weights = ar_data.mean(axis=1).flatten()
-            time_steps = list(range(1, len(mean_ar_weights) + 1))
-            ax.bar(time_steps, mean_ar_weights, label=component)
-        elif component == 'season_weekly':
-            forecast['day_of_week'] = forecast['ds'].dt.dayofweek
-            weekly_data = forecast.groupby('day_of_week')[
-                'season_weekly'].agg(np.mean)
-            ax.plot(weekly_data.index, weekly_data.values, label=component)
-            ax.set_xticks(list(range(7)))
-            ax.set_xticklabels(
-                ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday'])
-        elif component == 'season_yearly':
-            forecast['day_of_year'] = forecast['ds'].dt.dayofyear
-            yearly_data = forecast.groupby('day_of_year')[
-                'season_yearly'].agg(np.mean)
-            ax.plot(yearly_data.index, yearly_data.values, label=component)
-        else:
-            data = forecast.loc[:, ['ds', component]]
-            ax.plot(data['ds'], data[component], label=component)
-        # Customize the plot
-        ax.set_title(f"{component.capitalize().replace('_', ' ')} Component")
-        ax.set_xlabel("Day of Week" if component ==
-                      "season_weekly" else "Lag" if component == "AR" else "Date")
-        ax.set_ylabel(component.capitalize().replace('_', ' '))
-        ax.legend()
-    plt.tight_layout()
-    return fig
-
-@st.cache_data
-def condense_fcst_df(forecast_df: pd.DataFrame, forecast_product: str, forecast_session_id: int) -> pd.DataFrame:
-    """
-    Condense a forecast dataframe by calculating the sum of the yhat columns and adding the specified columns.
-
-    Args:
-        forecast_df (pd.DataFrame): The original forecast dataframe.
-        forecast_product (str): The forecast product name.
-        forecast_session_id (int): The forecast session ID.
-
-    Returns:
-        pd.DataFrame: The condensed forecast dataframe.
-    """
-    forecast_df_dense = forecast_df.copy(deep=True)
-    forecast_df_dense['product'] = forecast_product
-    forecast_df_dense['fcst_session_id'] = forecast_session_id
-    forecast_df_dense['yhat'] = forecast_df_dense.filter(
-        regex='^yhat').sum(axis=1)
-    # round to int for qty prediction
-    forecast_df_dense['fcst_qty'] = forecast_df_dense['yhat'].round()
-    forecast_df_dense = forecast_df_dense.loc[:, [
-        'fcst_session_id', 'product', 'ds', 'y', 'yhat', 'fcst_qty']]
-
-    return forecast_df_dense
-
-def save_fcst_db(forecast_df: pd.DataFrame, forecast_product: str, fcst_session_name: str, user_tag: str = None):
-    """
-    Save the forecast to the database using the provided inputs.
-
-    Args:
-        forecast_df (pd.DataFrame): The forecast dataframe.
-        forecast_product (str): The forecast product name.
-        fcst_session_name (str): The forecast session name.
-        user_tag (Optional[str], optional): The user tag. Defaults to None.
-    """
-
-    pg_manager = PostgreSQLManager()
-
-    with st.form("fcst_session_form"):
-        fcst_session_name = st.text_input(
-            "Choose a UNIQUE Forecast Session Name", value=fcst_session_name)
-        user_tag = st.text_input("User Tag (optional)", value=user_tag)
-        date_input = st.date_input("Date")
-
-        submit_button = st.form_submit_button(label="Save Forecast")
-
-        # Save values to st.session_state and insert values into the database
-        if submit_button:
-            st.session_state['fcst_session_name'] = fcst_session_name
-            st.session_state['user_tag'] = user_tag
-            st.session_state['date_input'] = date_input.strftime("%Y-%m-%d")
-
-            query_a = "INSERT INTO streamlit.fcst_sessions (fcst_session_name, fcst_date, user_tag) VALUES (%s, %s, %s)"
-            params = (fcst_session_name, date_input, user_tag)
-            a_success = pg_manager.insert_data(query_a, params)
-
-            # QUERY DB TO GET FCST_SESSION_ID for entered values
-            query_id = "SELECT fcst_session_id FROM streamlit.fcst_sessions WHERE fcst_session_name = '" + \
-                st.session_state['fcst_session_name'] + "'"
-            fcst_session_res = pg_manager.execute_query(query_id)
-            fcst_session_id = fcst_session_res[0]['fcst_session_id']
-            st.session_state['fcst_session_id'] = fcst_session_id
-
-            dense_df = condense_fcst_df(
-                forecast_df, forecast_product, fcst_session_id)
-            b_success = pg_manager.insert_dataframe(
-                dense_df, 'streamlit.product_fcst')
+class ForecastProduct:
 
-            if a_success and b_success:
-                st.success("Forecast saved!")
+    def __init__(self):
+        # Initialize state-dependent streamlit variables
+        if 'forecast' not in st.session_state:
+            st.session_state['forecast'] = pd.DataFrame
+        if 'horizon' not in st.session_state:
+            st.session_state['horizon'] = int
+        if 'fit_flag' not in st.session_state:
+            st.session_state['fit_flag'] = False
+        if 'fcst_session_name' not in st.session_state:
+            st.session_state['fcst_session_name'] = ""
+        if 'fcst_session_id' not in st.session_state:
+            st.session_state['fcst_session_id'] = None
+        if 'user_tag' not in st.session_state:
+            st.session_state['user_tag'] = ""
+        if 'events_df' not in st.session_state:
+            st.session_state['events_df'] = pd.DataFrame()
+        # Layout page
+        st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
+        st.header("4. Predict")
+        if st.session_state['fit_flag'] == False:
+            st.write("Please first load your data and select or train a model in the \"Tune and Train\" page to proceed with forecast prediction.")
+        else:
+            st.session_state['horizon'] = st.number_input(
+                'Please enter the desired forecast horizon.', min_value=1, max_value=len(st.session_state['forecast_df']), value=30)
+            predict_check = st.checkbox(
+                "Predict with model.", help="Use fitted NeuralProphet model to predict chosen forecast horizon.")
+            if predict_check:
+                st.session_state['forecast'] = self.predict(st.session_state['m'],
+                                                            st.session_state['horizon'],
+                                                            st.session_state['forecast_df'],
+                                                            st.session_state['events_df'])
+                with st.expander("View and Download Forecast"):
+                    st.subheader("NeuralProphet Forecast Dataframe")
+                    st.write(
+                        "Please note that all forecast results (yhat) and residuals are rounded to nearest integer for representing whole quantities of product.")
+                    st.dataframe(data=st.session_state['forecast'])
+                    st.download_button(label="Download Forecast CSV",
+                                       data=self.convert_df(
+                                           st.session_state['forecast']),
+                                       file_name='forecast_df_' +
+                                       st.session_state['forecast_product']+'.csv',
+                                       mime='text/csv')
+                with st.expander("Visualize Results"):
+                    st.subheader("Forecasted values for " +
+                                 st.session_state['forecast_product'])
+                    fig, ax = plt.subplots()
+                    for label in ax.get_xticklabels(which='major'):
+                        label.set(rotation=30, horizontalalignment='right')
+                    fig = st.session_state['m'].plot_latest_forecast(st.session_state['forecast'],
+                                                                     df_name=st.session_state['forecast_df'],
+                                                                     ax=ax,
+                                                                     xlabel="Date",
+                                                                     ylabel="Quantity")
+                    st.pyplot(fig)
+                    st.subheader("Forecast components for " +
+                                 st.session_state['forecast_product'])
+                    fig2 = st.session_state['m'].plot_components(
+                        fcst=st.session_state['forecast'], plotting_backend='matplotlib')
+                    st.pyplot(fig2)
+                    st.subheader("Forecast parameters for " +
+                                 st.session_state['forecast_product'])
+                    fig3 = st.session_state['m'].plot_parameters(
+                        plotting_backend='matplotlib')
+                    st.pyplot(fig3)
+                with st.expander("Save Results to Database"):
+                    self.save_fcst_db(st.session_state['forecast'],
+                                      st.session_state['forecast_product'],
+                                      st.session_state['fcst_session_name'],
+                                      st.session_state['user_tag'])
+
+    @st.cache_data
+    def convert_cols_to_int(_self, df):
+        """
+        Convert specified columns of a DataFrame to integers.
+
+        Args:
+            df: A DataFrame containing the columns to be converted.
+
+        Returns:
+            The modified DataFrame with specified columns converted to integers.
+        """
+        for col in df.columns:
+            if col.startswith('y') or col.startswith('residual') or col.startswith('step'):
+                df[col].fillna(0, inplace=True)
+                df[col] = df[col].round(0).astype(int)
+        return df
+
+    @st.cache_data
+    def predict(_self, _m: NeuralProphet, horizon: int, df: pd.DataFrame, events_df: pd.DataFrame = None) -> tuple:
+        """
+        Make predictions using a trained NeuralProphet model.
+
+        Args:
+            _m: A trained NeuralProphet model.
+            horizon: The forecast horizon in days.
+            df: A DataFrame containing the data for prediction.
+            events_df: A DataFrame containing events data (optional).
+
+        Returns:
+            A tuple containing the forecast DataFrame.
+        """
+        with st.spinner("Predicting with model... "):
+            if not events_df.empty:
+                data_ev = _m.create_df_with_events(df, events_df)
+                future = _m.make_future_dataframe(
+                    df=data_ev, events_df=events_df, periods=horizon)
+            else:
+                future = _m.make_future_dataframe(df=df, periods=horizon)
+            # convert predict output to integers as this application is focused on forecasting QTY which cannot be decimal
+            forecast = _self.convert_cols_to_int(_m.predict(future))
+            # raw_forecast = convert_cols_to_int(_m.predict(future, raw=True))
+        st.success("Prediction complete", icon="✅")
+        return forecast  # , raw_forecast
+
+    def convert_df(self, df):
+        """
+        Convert a DataFrame to a CSV string and encode it as utf-8 bytes.
+
+        Args:
+            df: A DataFrame to be converted.
+
+        Returns:
+            A CSV string of the DataFrame encoded as utf-8 bytes.
+        """
+        return df.to_csv().encode('utf-8')
+
+    def custom_plot_np_components(self, model, forecast, components=None):
+        """
+        Create custom component plots for a NeuralProphet model's forecast.
+
+        Args:
+            model: A trained NeuralProphet model.
+            forecast: A DataFrame containing the model's forecast.
+            components: A list of components to be plotted (default: None, which includes 'trend', 'season_yearly', 'season_weekly', and 'AR').
+
+        Returns:
+            A matplotlib figure containing the component plots.
+        """
+        if components is None:
+            components = ['trend', 'season_yearly', 'season_weekly', 'AR']
+
+        n_plots = len(components)
+        fig, axes = plt.subplots(n_plots, 1, figsize=(10, 4 * n_plots))
+        if n_plots == 1:
+            axes = [axes]
+
+        for idx, component in enumerate(components):
+            ax = axes[idx]
+            if component == 'AR':
+                ar_data = model.model.ar_weights.detach().numpy()
+                mean_ar_weights = ar_data.mean(axis=1).flatten()
+                time_steps = list(range(1, len(mean_ar_weights) + 1))
+                ax.bar(time_steps, mean_ar_weights, label=component)
+            elif component == 'season_weekly':
+                forecast['day_of_week'] = forecast['ds'].dt.dayofweek
+                weekly_data = forecast.groupby('day_of_week')[
+                    'season_weekly'].agg(np.mean)
+                ax.plot(weekly_data.index, weekly_data.values, label=component)
+                ax.set_xticks(list(range(7)))
+                ax.set_xticklabels(
+                    ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday'])
+            elif component == 'season_yearly':
+                forecast['day_of_year'] = forecast['ds'].dt.dayofyear
+                yearly_data = forecast.groupby('day_of_year')[
+                    'season_yearly'].agg(np.mean)
+                ax.plot(yearly_data.index, yearly_data.values, label=component)
             else:
-                st.error("Failed to create forecast session.")
+                data = forecast.loc[:, ['ds', component]]
+                ax.plot(data['ds'], data[component], label=component)
+            # Customize the plot
+            ax.set_title(
+                f"{component.capitalize().replace('_', ' ')} Component")
+            ax.set_xlabel("Day of Week" if component ==
+                          "season_weekly" else "Lag" if component == "AR" else "Date")
+            ax.set_ylabel(component.capitalize().replace('_', ' '))
+            ax.legend()
+        plt.tight_layout()
+        return fig
+
+    @st.cache_data
+    def condense_fcst_df(_self, forecast_df: pd.DataFrame, forecast_product: str, forecast_session_id: int) -> pd.DataFrame:
+        """
+        Condense a forecast dataframe by calculating the sum of the yhat columns and adding the specified columns.
+
+        Args:
+            forecast_df (pd.DataFrame): The original forecast dataframe.
+            forecast_product (str): The forecast product name.
+            forecast_session_id (int): The forecast session ID.
+
+        Returns:
+            pd.DataFrame: The condensed forecast dataframe.
+        """
+        forecast_df_dense = forecast_df.copy(deep=True)
+        forecast_df_dense['product'] = forecast_product
+        forecast_df_dense['fcst_session_id'] = forecast_session_id
+        forecast_df_dense['yhat'] = forecast_df_dense.filter(
+            regex='^yhat').sum(axis=1)
+        # round to int for qty prediction
+        forecast_df_dense['fcst_qty'] = forecast_df_dense['yhat'].round()
+        forecast_df_dense = forecast_df_dense.loc[:, [
+            'fcst_session_id', 'product', 'ds', 'y', 'yhat', 'fcst_qty']]
+
+        return forecast_df_dense
+
+    def save_fcst_db(self, forecast_df: pd.DataFrame, forecast_product: str, fcst_session_name: str, user_tag: str = None):
+        """
+        Save the forecast to the database using the provided inputs.
+
+        Args:
+            forecast_df (pd.DataFrame): The forecast dataframe.
+            forecast_product (str): The forecast product name.
+            fcst_session_name (str): The forecast session name.
+            user_tag (Optional[str], optional): The user tag. Defaults to None.
+        """
+        pg_manager = PostgreSQLManager()
+        with st.form("fcst_session_form"):
+            fcst_session_name = st.text_input(
+                "Choose a UNIQUE Forecast Session Name", value=fcst_session_name)
+            user_tag = st.text_input("User Tag (optional)", value=user_tag)
+            date_input = st.date_input("Date")
+            submit_button = st.form_submit_button(label="Save Forecast")
+            # Save values to st.session_state and insert values into the database
+            if submit_button:
+                st.session_state['fcst_session_name'] = fcst_session_name
+                st.session_state['user_tag'] = user_tag
+                st.session_state['date_input'] = date_input.strftime(
+                    "%Y-%m-%d")
+                query_a = "INSERT INTO streamlit.fcst_sessions (fcst_session_name, fcst_date, user_tag) VALUES (%s, %s, %s)"
+                params = (fcst_session_name, date_input, user_tag)
+                a_success = pg_manager.insert_data(query_a, params)
+                # QUERY DB TO GET FCST_SESSION_ID for entered values
+                query_id = "SELECT fcst_session_id FROM streamlit.fcst_sessions WHERE fcst_session_name = '" + \
+                    st.session_state['fcst_session_name'] + "'"
+                fcst_session_res = pg_manager.execute_query(query_id)
+                fcst_session_id = fcst_session_res[0]['fcst_session_id']
+                st.session_state['fcst_session_id'] = fcst_session_id
+                dense_df = condense_fcst_df(
+                    forecast_df, forecast_product, fcst_session_id)
+                b_success = pg_manager.insert_dataframe(
+                    dense_df, 'streamlit.product_fcst')
+                if a_success and b_success:
+                    st.success("Forecast saved!")
+                else:
+                    st.error("Failed to create forecast session.")
+                pg_manager.close_pool()
 
-    # Close the database connection pool
-    pg_manager.close_pool()
 
-#initiliaze session_state variables
-if 'forecast' not in st.session_state:
-    st.session_state['forecast'] = pd.DataFrame
-
-if 'horizon' not in st.session_state:
-    st.session_state['horizon'] = int
-
-if 'fit_flag' not in st.session_state:
-    st.session_state['fit_flag'] = False
-
-if 'fcst_session_name' not in st.session_state:
-    st.session_state['fcst_session_name'] = ""
-
-if 'fcst_session_id' not in st.session_state:
-    st.session_state['fcst_session_id'] = None
-
-if 'user_tag' not in st.session_state:
-    st.session_state['user_tag'] = ""
-
-
-# Section for prediction and visualization
-st.header("4. Predict")
-
-if 'fit_flag' in st.session_state:
-    if st.session_state['fit_flag'] == False:
-        st.write("Please first load your data and select or train a model in the \"Tune and Train\" page to proceed with forecast prediction.")
-    else:
-
-        st.session_state['horizon'] = st.number_input(
-            'Please enter the desired forecast horizon.', min_value=1, max_value=len(st.session_state['forecast_df']), value=30)
-
-        predict_check = st.checkbox(
-            "Predict with model.", help="Use fitted NeuralProphet model to predict chosen forecast horizon.")
-
-        if predict_check:
-            st.session_state['forecast'] = predict(st.session_state['m'],
-                                                   st.session_state['horizon'],
-                                                   st.session_state['forecast_df'],
-                                                   is_events())
-
-            with st.expander("View and Download Forecast"):
-                st.subheader("NeuralProphet Forecast Dataframe")
-                st.write(
-                    "Please note that all forecast results (yhat) and residuals are rounded to nearest integer for representing whole quantities of product.")
-                st.dataframe(data=st.session_state['forecast'])
-                st.download_button(label="Download Forecast CSV",
-                                   data=convert_df(
-                                       st.session_state['forecast']),
-                                   file_name='forecast_df_' +
-                                   st.session_state['forecast_product']+'.csv',
-                                   mime='text/csv'
-                                   )
-
-            with st.expander("Visualize Results"):
-                st.subheader("Forecasted values for " +
-                             st.session_state['forecast_product'])
-                fig, ax = plt.subplots()
-                for label in ax.get_xticklabels(which='major'):
-                    label.set(rotation=30, horizontalalignment='right')
-                fig = st.session_state['m'].plot_latest_forecast(st.session_state['forecast'],
-                                                                 df_name=st.session_state['forecast_df'],
-                                                                 ax=ax,
-                                                                 xlabel="Date",
-                                                                 ylabel="Quantity"
-                                                                 )
-                st.pyplot(fig)
-
-                st.subheader("Forecast components for " +
-                             st.session_state['forecast_product'])
-                fig2 = st.session_state['m'].plot_components(
-                    fcst=st.session_state['forecast'], plotting_backend='matplotlib')
-                st.pyplot(fig2)
-
-                st.subheader("Forecast parameters for " +
-                             st.session_state['forecast_product'])
-                fig3 = st.session_state['m'].plot_parameters(
-                    plotting_backend='matplotlib')
-                st.pyplot(fig3)
-
-            with st.expander("Save Results to Database"):
-                save_fcst_db(st.session_state['forecast'],
-                             st.session_state['forecast_product'],
-                             st.session_state['fcst_session_name'],
-                             st.session_state['user_tag'])
+if __name__ == '__main__':
+    fp = ForecastProduct()
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_5_Distribute_Size_Forecast.py` & `d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/pages/_5_Distribute_Size_Forecast.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,223 +12,237 @@
 from sklearn.metrics.pairwise import cosine_similarity
 from hierarchicalforecast.core import HierarchicalReconciliation
 from hierarchicalforecast.methods import TopDown
 from hierarchicalforecast.evaluation import HierarchicalEvaluation
 from hierarchicalforecast.utils import aggregate
 from d2c_mp_sales_forecaster.utils.db_manager import PostgreSQLManager
 
-# Page config
-st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
 
+class DistributeSizeForecast:
 
-@st.cache_data
-def prep_data_topdown(forecast_product: str, forecast_df_product: pd.DataFrame, all_sales_size_data: pd.DataFrame) -> tuple:
-    """
-    Prepare data for top-down hierarchical forecasting.
-
-    Args:
-        forecast_product: The target product for forecasting.
-        forecast_df_product: A DataFrame containing the sales history of the target product.
-        all_sales_size_data: A DataFrame containing sales data for all products and sizes.
-
-    Returns:
-        A tuple containing the aggregate sales data, disaggregate sales data, and unique identifier tags.
-    """
-    hiers = [
-        ['product'],
-        ['product', 'size']
-    ]
-    dfd = all_sales_size_data.merge(forecast_df_product[['ds', 'product']], on=[
-                                    'ds', 'product'], how='inner')
-    dfd.loc[:, 'product'] = forecast_product
-    dfd.reset_index(inplace=True, drop=True)
-    # use hierarchicalforecast package aggregate function to prep needed dataframes
-    Y_df, S_df, tags = aggregate(dfd, hiers)
-    # setup historical 'fit' column since using NeuralProphet to create forecast
-    Y_df.loc[:, 'yhat'] = Y_df['y']
-    return Y_df, S_df, tags
-
-
-@st.cache_data
-def convert_forecast_for_reconciler(forecast: pd.DataFrame, horizon: int) -> pd.DataFrame:
-    """
-    Convert forecast data to a format suitable for the reconciler.
-
-    Args:
-        forecast: A DataFrame containing the forecast data.
-        horizon: The forecast horizon in days.
-
-    Returns:
-        A DataFrame containing the reformatted forecast data.
-    """
-    fcst = forecast.iloc[horizon:, :(horizon+2)].copy()
-    fcst['yhat'] = fcst.filter(regex='^yhat').sum(axis=1)
-    fcst['unique_id'] = st.session_state['forecast_product']
-    fcst = fcst.loc[:, ('ds', 'yhat', 'unique_id')]
-    return fcst
-
-
-@st.cache_data
-def add_size_fcst_frame(fcst_converted: pd.DataFrame, S: pd.DataFrame) -> pd.DataFrame:
-    """
-    Create size-level forecast frame and add zero forecast as base forecast for size-level to the forecast data.
-
-    Args:
-        fcst_converted: A DataFrame containing the converted forecast data.
-        S: A DataFrame containing the disaggregate sales data.
-
-    Returns:
-        A DataFrame containing the forecast data with added size-level forecasts.
-    """
-    # create template to add zero forecast as base forecast for size-level
-    dates = fcst_converted['ds'].to_list()
-    sizes = S_df.columns.to_list()
-    # Create a list of tuples with all combinations of dates and sizes
-    date_size_combinations = list(itertools.product(dates, sizes))
-    # Create the DataFrame with 'date' and 'size' columns
-    sizes_fcst_frame = pd.DataFrame(
-        date_size_combinations, columns=['ds', 'unique_id'])
-    sizes_fcst_frame.loc[:, 'yhat'] = 0
-    # Concat with product level predictions for the full forecast frame for reconciler
-    full_fcst_frame = pd.concat(
-        [fcst_converted, sizes_fcst_frame], ignore_index=True)
-    full_fcst_frame.index = full_fcst_frame['unique_id']
-    full_fcst_frame.drop(columns=['unique_id'], inplace=True)
-    full_fcst_frame.columns = ['ds', 'yhat']
-    return full_fcst_frame
-
-
-@st.cache_resource
-def convert_df(df):
-    """
-    Convert a DataFrame to a CSV string and encode it as utf-8 bytes.
-
-    Args:
-        df: A DataFrame to be converted.
-
-    Returns:
-        A CSV string of the DataFrame encoded as utf-8 bytes.
-    """
-    # IMPORTANT: Cache the conversion to prevent computation on every rerun
-    return df.to_csv().encode('utf-8')
-
-
-def save_size_fcst_db(forecast_df: pd.DataFrame, fcst_session_id: int, fcst_session_name: str, user_tag: str = ""):
-    """
-    Save the size forecast to the database using the provided inputs.
-
-    Args:
-        forecast_df (pd.DataFrame): The size forecast dataframe.
-        fcst_session_id (int): The forecast session ID.
-        fcst_session_name (str): The forecast session name.
-        user_tag (Optional[str], optional): The user tag. Defaults to an empty string.
-    """
-    pg_manager = PostgreSQLManager()
-
-    with st.form("size_fcst_session_form"):
-        st.write("UNIQUE Forecast Session Name : " + fcst_session_name)
-        user_tag = st.text_input("User Tag (optional)", value=user_tag)
-        date_input = st.date_input("Date")
-
-        submit_button = st.form_submit_button(label="Save Size Forecast")
-
-        if submit_button:
-            st.session_state['user_tag'] = user_tag
-            st.session_state['date_input'] = date_input.strftime("%Y-%m-%d")
-
-            # add session id to dataframe for db entry with reference to session
-            forecast_df.columns = ['unique_id', 'ds', 'yhat', 'fcst_qty']
-            forecast_df['fcst_session_id'] = fcst_session_id
-            size_save_success = pg_manager.insert_dataframe(
-                forecast_df, 'streamlit.product_size_fcst')
-
-            if size_save_success:
-                st.success("Size forecast saved!")
-            else:
-                st.error("Failed to save size forecast.")
-
-    pg_manager.close_pool()
-
-# initialize session_state vars
-if 'forecast' not in st.session_state:
-    st.session_state['forecast'] = pd.DataFrame
-
-if 'fcst_session_name' not in st.session_state:
-    st.session_state['fcst_session_name'] = ""
-
-if 'fcst_session_id' not in st.session_state:
-    st.session_state['fcst_session_id'] = None
-
-if 'user_tag' not in st.session_state:
-    st.session_state['user_tag'] = ""
-
-if 'Y_hat_sizes' not in st.session_state:
-    st.session_state['Y_hat_sizes'] = pd.DataFrame
-
-# Section for distribution by size
-st.header("5. Apply optional size level distribution to the forecast.")
-
-if 'forecast' in st.session_state and 'forecast_product' in st.session_state:
-    if st.session_state['forecast'].empty:
-        st.write("Please use the preceding pages to upload data, train a model, and form a product-level prediction before proceeding to size distribution.")
-    else:
-        method = st.selectbox("Choose method of calculating size curve from historical data:", [
-                              'average_proportions', 'proportion_averages'], index=0)
-        size_dist_check = st.checkbox(
-            "Distribute your forecast by size?", help="Distribute forecast to a size-curve using top-down average historical proportions."
-        )
-        if size_dist_check:
-
-            # Execute the reconciliation
-            Y_df, S_df, tags = prep_data_topdown(
-                st.session_state['forecast_product'], st.session_state['forecast_df_product'], st.session_state['all_sales_size_data'])
-            fcst = convert_forecast_for_reconciler(
-                st.session_state['forecast'], st.session_state['horizon'])
-            Y_hat_df = add_size_fcst_frame(fcst, S_df)
-
-            # Reconcile the base predictions
-            reconcilers = [
-                TopDown(method)
-            ]
-
-            hrec = HierarchicalReconciliation(reconcilers=reconcilers)
-            Y_hat_rec = hrec.reconcile(
-                Y_hat_df=Y_hat_df, S=S_df, tags=tags, Y_df=Y_df)
-            # convert forecast to int for qty sold
-            Y_hat_rec.loc[:, 'fcst_qty'] = Y_hat_rec['yhat/TopDown_method-'+method].round()
-            Y_hat_rec.reset_index(inplace=True)
-            Y_hat_sizes = Y_hat_rec[Y_hat_rec['unique_id'] !=
-                                    st.session_state['forecast_product']].iloc[:, [0, 1, 3, 4]]
-            st.session_state['Y_hat_sizes'] = Y_hat_sizes
-
-            st.write(Y_hat_sizes)
-            st.download_button(label="Download Forecast CSV",
-                               data=convert_df(Y_hat_sizes),
-                               file_name='forecast_bysize_df_' +
-                               st.session_state['forecast_product']+'.csv',
-                               mime='text/csv'
-                               )
-
-            with st.expander("Size Distribution Visualizations"):
-                # Check chart 1
-                size_grp = Y_hat_sizes.loc[:, ('ds', 'unique_id', 'fcst_qty')].groupby(
-                    'unique_id').sum().sort_values(by='fcst_qty')
-                st.subheader("Forecast Quantity by Size")
-                st.pyplot(size_grp.plot(kind='barh').figure)
-                # Check chart 2
-                Y_df_comp = Y_df.reset_index()
-                Y_df_comp = Y_df_comp[Y_df_comp['unique_id']
-                                      != st.session_state['forecast_product']]
-                Y_df_comp.rename(columns={"y": "qty"}, inplace=True)
-                st.subheader("Training Set Quantity Distribution")
-                st.pyplot(Y_df_comp.loc[:, ('ds', 'unique_id', 'qty')].groupby(
-                    'unique_id').sum().sort_values(by='qty').plot(kind='barh').figure)
-
-            with st.expander("Save Results to Database"):
-
-                if st.session_state['fcst_session_id'] is not None:
-                    save_size_fcst_db(st.session_state['Y_hat_sizes'], 
-                                      st.session_state['fcst_session_id'],
-                                      st.session_state['fcst_session_name'], st.session_state['user_tag'])
+    def __init__(self):
+        # Initialize state-dependent streamlit variables
+        # initialize session_state vars
+        if 'forecast' not in st.session_state:
+            st.session_state['forecast'] = pd.DataFrame
+        if 'fcst_session_name' not in st.session_state:
+            st.session_state['fcst_session_name'] = ""
+        if 'fcst_session_id' not in st.session_state:
+            st.session_state['fcst_session_id'] = None
+        if 'user_tag' not in st.session_state:
+            st.session_state['user_tag'] = ""
+        if 'Y_hat_sizes' not in st.session_state:
+            st.session_state['Y_hat_sizes'] = pd.DataFrame
+        if 'Y_df' not in st.session_state:
+            st.session_state['Y_df'] = pd.DataFrame
+        if 'forecast_product' not in st.session_state:
+            st.session_state['forecast_product'] = None
+        if 'forecast_df_product' not in st.session_state:
+            st.session_state['forecast_df_product'] = pd.DataFrame
+        if 'all_sales_size_data' not in st.session_state:
+            st.session_state['all_sales_size_data'] = pd.DataFrame()
+        if 'horizon' not in st.session_state:
+            st.session_state['horizon'] = int
+        # Layout page
+        st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
+        st.header("Step 5: Distribute forecast to product sizes.")
+        if st.session_state['forecast'].empty:
+            st.write("Please use the preceding pages to upload data, train a model, and form a product-level prediction before proceeding to size distribution.")
+        else:
+            method = st.selectbox("Choose method of calculating size curve from historical data:", [
+                'average_proportions', 'proportion_averages'], index=0)
+            size_dist_check = st.checkbox("Distribute your forecast by size?",
+                                          help="Distribute forecast to a size-curve using top-down average historical proportions.")
+            if size_dist_check:
+                # Execute the reconciliation
+                st.session_state['Y_hat_sizes'], st.session_state['Y_df'] = self.size_dist_recon(st.session_state['forecast_product'],
+                                                                                                 st.session_state['forecast_df_product'],
+                                                                                                 st.session_state['all_sales_size_data'],
+                                                                                                 st.session_state['forecast'],
+                                                                                                 st.session_state['horizon'],
+                                                                                                 method)
+                st.write(st.session_state['Y_hat_sizes'])
+                st.download_button(label="Download Forecast CSV",
+                                   data=self.convert_df(
+                                       st.session_state['Y_hat_sizes']),
+                                   file_name='forecast_bysize_df_' +
+                                   st.session_state['forecast_product']+'.csv',
+                                   mime='text/csv')
+                with st.expander("Size Distribution Visualizations"):
+                    # Check chart 1
+                    size_grp = st.session_state['Y_hat_sizes'].loc[:, ('ds', 'unique_id', 'fcst_qty')].groupby(
+                        'unique_id').sum().sort_values(by='fcst_qty')
+                    st.subheader("Forecast Quantity by Size")
+                    st.pyplot(size_grp.plot(kind='barh').figure)
+                    # Check chart 2
+                    Y_df_comp = st.session_state['Y_df'].reset_index()
+                    Y_df_comp = Y_df_comp[Y_df_comp['unique_id']
+                                          != st.session_state['forecast_product']]
+                    Y_df_comp.rename(columns={"y": "qty"}, inplace=True)
+                    st.subheader("Training Set Quantity Distribution")
+                    st.pyplot(Y_df_comp.loc[:, ('ds', 'unique_id', 'qty')].groupby(
+                        'unique_id').sum().sort_values(by='qty').plot(kind='barh').figure)
+                with st.expander("Save Results to Database"):
+                    if st.session_state['fcst_session_id'] is not None:
+                        self.save_size_fcst_db(st.session_state['Y_hat_sizes'],
+                                               st.session_state['fcst_session_id'],
+                                               st.session_state['fcst_session_name'], st.session_state['user_tag'])
+                    else:
+                        st.write(
+                            'Please save matching product-level forecast to DB first for referential integrity.')
+
+    @st.cache_data
+    def prep_data_topdown(_self, forecast_product: str, forecast_df_product: pd.DataFrame, all_sales_size_data: pd.DataFrame) -> tuple:
+        """
+        Prepare data for top-down hierarchical forecasting.
+
+        Args:
+            forecast_product: The target product for forecasting.
+            forecast_df_product: A DataFrame containing the sales history of the target product.
+            all_sales_size_data: A DataFrame containing sales data for all products and sizes.
+
+        Returns:
+            A tuple containing the aggregate sales data, disaggregate sales data, and unique identifier tags.
+        """
+        hiers = [
+            ['product'],
+            ['product', 'size']
+        ]
+        dfd = all_sales_size_data.merge(forecast_df_product[['ds', 'product']], on=[
+                                        'ds', 'product'], how='inner')
+        dfd.loc[:, 'product'] = forecast_product
+        dfd.reset_index(inplace=True, drop=True)
+        # use hierarchicalforecast package aggregate function to prep needed dataframes
+        Y_df, S_df, tags = aggregate(dfd, hiers)
+        # setup historical 'fit' column since using NeuralProphet to create forecast
+        Y_df.loc[:, 'yhat'] = Y_df['y']
+        return Y_df, S_df, tags
+
+    @st.cache_data
+    def convert_forecast_for_reconciler(_self, forecast: pd.DataFrame, horizon: int) -> pd.DataFrame:
+        """
+        Convert forecast data to a format suitable for the reconciler.
+
+        Args:
+            forecast: A DataFrame containing the forecast data.
+            horizon: The forecast horizon in days.
+
+        Returns:
+            A DataFrame containing the reformatted forecast data.
+        """
+        fcst = forecast.iloc[horizon:, :(horizon+2)].copy()
+        fcst['yhat'] = fcst.filter(regex='^yhat').sum(axis=1)
+        fcst['unique_id'] = st.session_state['forecast_product']
+        fcst = fcst.loc[:, ('ds', 'yhat', 'unique_id')]
+        return fcst
+
+    @st.cache_data
+    def add_size_fcst_frame(_self, fcst_converted: pd.DataFrame, S: pd.DataFrame) -> pd.DataFrame:
+        """
+        Create size-level forecast frame and add zero forecast as base forecast for size-level to the forecast data.
+
+        Args:
+            fcst_converted: A DataFrame containing the converted forecast data.
+            S: A DataFrame containing the disaggregate sales data.
+
+        Returns:
+            A DataFrame containing the forecast data with added size-level forecasts.
+        """
+        # create template to add zero forecast as base forecast for size-level
+        dates = fcst_converted['ds'].to_list()
+        sizes = S.columns.to_list()
+        # Create a list of tuples with all combinations of dates and sizes
+        date_size_combinations = list(itertools.product(dates, sizes))
+        # Create the DataFrame with 'date' and 'size' columns
+        sizes_fcst_frame = pd.DataFrame(
+            date_size_combinations, columns=['ds', 'unique_id'])
+        sizes_fcst_frame.loc[:, 'yhat'] = 0
+        # Concat with product level predictions for the full forecast frame for reconciler
+        full_fcst_frame = pd.concat(
+            [fcst_converted, sizes_fcst_frame], ignore_index=True)
+        full_fcst_frame.index = full_fcst_frame['unique_id']
+        full_fcst_frame.drop(columns=['unique_id'], inplace=True)
+        full_fcst_frame.columns = ['ds', 'yhat']
+        return full_fcst_frame
+
+    @st.cache_resource
+    def convert_df(_self, df):
+        """
+        Convert a DataFrame to a CSV string and encode it as utf-8 bytes.
+
+        Args:
+            df: A DataFrame to be converted.
+
+        Returns:
+            A CSV string of the DataFrame encoded as utf-8 bytes.
+        """
+        # IMPORTANT: Cache the conversion to prevent computation on every rerun
+        return df.to_csv().encode('utf-8')
+
+    def save_size_fcst_db(self, forecast_df: pd.DataFrame, fcst_session_id: int, fcst_session_name: str, user_tag: str = ""):
+        """
+        Save the size forecast to the database using the provided inputs.
+
+        Args:
+            forecast_df (pd.DataFrame): The size forecast dataframe.
+            fcst_session_id (int): The forecast session ID.
+            fcst_session_name (str): The forecast session name.
+            user_tag (Optional[str], optional): The user tag. Defaults to an empty string.
+        """
+        pg_manager = PostgreSQLManager()
+        with st.form("size_fcst_session_form"):
+            st.write("UNIQUE Forecast Session Name : " + fcst_session_name)
+            user_tag = st.text_input("User Tag (optional)", value=user_tag)
+            date_input = st.date_input("Date")
+
+            submit_button = st.form_submit_button(label="Save Size Forecast")
+
+            if submit_button:
+                st.session_state['user_tag'] = user_tag
+                st.session_state['date_input'] = date_input.strftime(
+                    "%Y-%m-%d")
+
+                # add session id to dataframe for db entry with reference to session
+                forecast_df.columns = ['unique_id', 'ds', 'yhat', 'fcst_qty']
+                forecast_df['fcst_session_id'] = fcst_session_id
+                size_save_success = pg_manager.insert_dataframe(
+                    forecast_df, 'streamlit.product_size_fcst')
+
+                if size_save_success:
+                    st.success("Size forecast saved!")
                 else:
-                    st.write('Please save matching product-level forecast to DB first for referential integrity.')
-                    
+                    st.error("Failed to save size forecast.")
+        pg_manager.close_pool()
+
+    def size_dist_recon(self, forecast_product: str, forecast_df_product: pd.DataFrame, all_sales_size_data: pd.DataFrame, forecast: pd.DataFrame, horizon: int, method: str) -> tuple:
+        """
+        Reconciles size distribution forecasts using a top-down approach.
+
+        Args:
+            forecast_product (str): The name of the forecasted product.
+            forecast_df_product (pd.DataFrame): The forecast data for the product.
+            all_sales_size_data (pd.DataFrame): The sales size data for all products.
+            forecast (pd.DataFrame): The original forecast data.
+            horizon (int): The forecast horizon.
+            method (str): The reconciliation method.
+
+        Returns:
+            tuple: A tuple containing Y_hat_sizes and Y_df.
+        """
+        Y_df, S_df, tags = self.prep_data_topdown(
+            forecast_product, forecast_df_product, all_sales_size_data)
+        fcst = self.convert_forecast_for_reconciler(forecast, horizon)
+        Y_hat_df = self.add_size_fcst_frame(fcst, S_df)
+        # Reconcile the base predictions
+        reconcilers = [TopDown(method)]
+        hrec = HierarchicalReconciliation(reconcilers=reconcilers)
+        Y_hat_rec = hrec.reconcile(
+            Y_hat_df=Y_hat_df, S=S_df, tags=tags, Y_df=Y_df)
+        # convert forecast to int for qty sold
+        Y_hat_rec.loc[:, 'fcst_qty'] = Y_hat_rec['yhat/TopDown_method-'+method].round()
+        Y_hat_rec.reset_index(inplace=True)
+        Y_hat_sizes = Y_hat_rec[Y_hat_rec['unique_id']
+                                != forecast_product].iloc[:, [0, 1, 3, 4]]
+        return Y_hat_sizes, Y_df
+    
+if __name__ == "__main__":
+    dsf = DistributeSizeForecast()
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/utils/db_manager.py` & `d2c_mp_sales_forecaster-0.0.3/src/d2c_mp_sales_forecaster/utils/db_manager.py`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/tests/test_1_Load_Data.py` & `d2c_mp_sales_forecaster-0.0.3/tests/test_1_Load_Data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import pytest
 import pandas as pd
+import streamlit as st
 from io import StringIO
-from d2c_mp_sales_forecaster.pages._1_Load_Data import (
-    upload_sales_size_data,
-    upload_master_data,
-    upload_events_data,
-    upload_lag_data,
-    upload_future_data,
-)
+from unittest.mock import MagicMock
+from d2c_mp_sales_forecaster.pages._1_Load_Data import LoadData
 
 class TestClassLoadData:
+
+    @pytest.fixture(autouse=True)
+    def set_up(self):
+        with MagicMock() as st.session_state:
+            yield
     
     @pytest.fixture
     def sample_sales_size_data(self):
         data = "product,size,ds,y\nA,Small,2022-01-01,100\nA,Medium,2022-01-01,200\nB,Small,2022-01-01,150\nB,Large,2022-01-01,300\nA,Small,2022-01-02,120\nA,Medium,2022-01-02,180\nB,Small,2022-01-02,140\nB,Large,2022-01-02,310"
         return StringIO(data)
 
     @pytest.fixture
@@ -27,33 +28,28 @@
         return StringIO(data)
 
     @pytest.fixture
     def sample_lag_data(self):
         data = "ds,lag1\n2022-01-01,10\n2022-01-02,12"
         return StringIO(data)
 
-    @pytest.fixture
-    def sample_future_data(self):
-        data = "ds,future1\n2022-01-03,15\n2022-01-04,18"
-        return StringIO(data)
-
     def test_upload_sales_size_data(self, sample_sales_size_data):
-        all_sales_data, all_sales_size_data = upload_sales_size_data(sample_sales_size_data)
+        ld = LoadData()
+        all_sales_data, all_sales_size_data = ld.upload_sales_size_data_func(sample_sales_size_data)
         assert isinstance(all_sales_data, pd.DataFrame)
         assert isinstance(all_sales_size_data, pd.DataFrame)
 
     def test_upload_master_data(self, sample_master_data):
-        master_data, master_data_enc = upload_master_data(sample_master_data)
+        ld = LoadData()
+        master_data, master_data_enc = ld.upload_master_data_func(sample_master_data)
         assert isinstance(master_data, pd.DataFrame)
         assert isinstance(master_data_enc, pd.DataFrame)
 
     def test_upload_events_data(self, sample_events_data):
-        events_df = upload_events_data(sample_events_data)
+        ld = LoadData()
+        events_df = ld.upload_events_data_func(sample_events_data)
         assert isinstance(events_df, pd.DataFrame)
 
     def test_upload_lag_data(self, sample_lag_data):
-        lag_data = upload_lag_data(sample_lag_data)
-        assert isinstance(lag_data, pd.DataFrame)
-
-    def test_upload_future_data(self, sample_future_data):
-        future_data = upload_future_data(sample_future_data)
-        assert isinstance(future_data, pd.DataFrame)
+        ld = LoadData()
+        lag_data = ld.upload_lag_data_func(sample_lag_data)
+        assert isinstance(lag_data, pd.DataFrame)
```

### Comparing `d2c_mp_sales_forecaster-0.0.2/tests/test_3_Tune_and_Train.py` & `d2c_mp_sales_forecaster-0.0.3/tests/test_3_Tune_and_Train.py`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/tests/test_4_Forecast_Product.py` & `d2c_mp_sales_forecaster-0.0.3/tests/test_4_Forecast_Product.py`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/tests/test_5_Distribute_Size_forecast.py` & `d2c_mp_sales_forecaster-0.0.3/tests/test_5_Distribute_Size_forecast.py`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/tests/select_product/lag_data.csv` & `d2c_mp_sales_forecaster-0.0.3/tests/select_product/lag_data.csv`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/tests/select_product/master_data_enc.csv` & `d2c_mp_sales_forecaster-0.0.3/tests/select_product/master_data_enc.csv`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/tests/select_product/sales_data.csv` & `d2c_mp_sales_forecaster-0.0.3/tests/select_product/sales_data.csv`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/.gitignore` & `d2c_mp_sales_forecaster-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/LICENSE` & `d2c_mp_sales_forecaster-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.2/pyproject.toml` & `d2c_mp_sales_forecaster-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "d2c_mp_sales_forecaster"
-version = "0.0.2"
+version = "0.0.003"
 authors = [
   { name="Ryan Handerhan", email="rhanderh@alumni.cmu.edu" },
 ]
 description = "An application for forecasting direct-to-consumer sales quantities using the NeuralProphet algorithm from Meta."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

