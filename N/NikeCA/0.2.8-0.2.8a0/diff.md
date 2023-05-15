# Comparing `tmp/NikeCA-0.2.8.tar.gz` & `tmp/NikeCA-0.2.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.2.8.tar", last modified: Mon May 15 16:25:23 2023, max compression
+gzip compressed data, was "NikeCA-0.2.8a0.tar", last modified: Mon May 15 19:33:36 2023, max compression
```

## Comparing `NikeCA-0.2.8.tar` & `NikeCA-0.2.8a0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 16:25:23.038257 NikeCA-0.2.8/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.8/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-15 16:25:23.037840 NikeCA-0.2.8/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.8/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-15 16:25:23.038365 NikeCA-0.2.8/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2539 2023-05-15 16:24:54.000000 NikeCA-0.2.8/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 16:25:23.030169 NikeCA-0.2.8/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 16:25:23.031167 NikeCA-0.2.8/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4244 2023-05-10 19:45:47.000000 NikeCA-0.2.8/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 16:25:23.032324 NikeCA-0.2.8/src/Dashboards/IMP/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4387 2023-05-11 20:42:04.000000 NikeCA-0.2.8/src/Dashboards/IMP/IMP.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:04.000000 NikeCA-0.2.8/src/Dashboards/IMP/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 16:25:23.033276 NikeCA-0.2.8/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)    10886 2023-05-10 19:45:47.000000 NikeCA-0.2.8/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 20:46:33.000000 NikeCA-0.2.8/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 16:25:23.035089 NikeCA-0.2.8/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     6967 2023-05-10 19:41:44.000000 NikeCA-0.2.8/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7325 2023-05-10 19:45:47.000000 NikeCA-0.2.8/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.8/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.8/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 16:25:23.037392 NikeCA-0.2.8/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-15 16:25:22.000000 NikeCA-0.2.8/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      729 2023-05-15 16:25:22.000000 NikeCA-0.2.8/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-15 16:25:22.000000 NikeCA-0.2.8/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-15 16:25:22.000000 NikeCA-0.2.8/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      394 2023-05-15 16:25:22.000000 NikeCA-0.2.8/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 20:48:35.000000 NikeCA-0.2.8/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-10 19:40:28.000000 NikeCA-0.2.8/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    20111 2023-05-12 22:28:52.000000 NikeCA-0.2.8/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-10 19:40:28.000000 NikeCA-0.2.8/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13660 2023-05-11 05:36:47.000000 NikeCA-0.2.8/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-10 19:40:28.000000 NikeCA-0.2.8/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-10 19:40:28.000000 NikeCA-0.2.8/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14378 2023-05-12 22:30:50.000000 NikeCA-0.2.8/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    12515 2023-05-15 16:22:54.000000 NikeCA-0.2.8/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7154 2023-05-10 19:40:28.000000 NikeCA-0.2.8/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:43:36.000000 NikeCA-0.2.8/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 19:33:36.279801 NikeCA-0.2.8a0/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.8a0/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-15 19:33:36.279251 NikeCA-0.2.8a0/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.8a0/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-15 19:33:36.279977 NikeCA-0.2.8a0/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2540 2023-05-15 19:33:32.000000 NikeCA-0.2.8a0/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 19:33:36.266899 NikeCA-0.2.8a0/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 19:33:36.268623 NikeCA-0.2.8a0/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4244 2023-05-10 19:45:47.000000 NikeCA-0.2.8a0/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 19:33:36.270350 NikeCA-0.2.8a0/src/Dashboards/IMP/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4387 2023-05-11 20:42:04.000000 NikeCA-0.2.8a0/src/Dashboards/IMP/IMP.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:04.000000 NikeCA-0.2.8a0/src/Dashboards/IMP/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 19:33:36.271786 NikeCA-0.2.8a0/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    10886 2023-05-10 19:45:47.000000 NikeCA-0.2.8a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 20:46:33.000000 NikeCA-0.2.8a0/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 19:33:36.274665 NikeCA-0.2.8a0/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6967 2023-05-10 19:41:44.000000 NikeCA-0.2.8a0/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7325 2023-05-10 19:45:47.000000 NikeCA-0.2.8a0/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.8a0/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.8a0/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-15 19:33:36.278383 NikeCA-0.2.8a0/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-15 19:33:36.000000 NikeCA-0.2.8a0/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      729 2023-05-15 19:33:36.000000 NikeCA-0.2.8a0/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-15 19:33:36.000000 NikeCA-0.2.8a0/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-15 19:33:36.000000 NikeCA-0.2.8a0/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      394 2023-05-15 19:33:36.000000 NikeCA-0.2.8a0/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 20:48:35.000000 NikeCA-0.2.8a0/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-10 19:40:28.000000 NikeCA-0.2.8a0/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    20111 2023-05-12 22:28:52.000000 NikeCA-0.2.8a0/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-10 19:40:28.000000 NikeCA-0.2.8a0/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13660 2023-05-11 05:36:47.000000 NikeCA-0.2.8a0/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-10 19:40:28.000000 NikeCA-0.2.8a0/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-10 19:40:28.000000 NikeCA-0.2.8a0/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14378 2023-05-12 22:30:50.000000 NikeCA-0.2.8a0/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    12828 2023-05-15 19:33:14.000000 NikeCA-0.2.8a0/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7154 2023-05-10 19:40:28.000000 NikeCA-0.2.8a0/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:43:36.000000 NikeCA-0.2.8a0/src/__init__.py
```

### Comparing `NikeCA-0.2.8/LICENSE` & `NikeCA-0.2.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/PKG-INFO` & `NikeCA-0.2.8a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.8
+Version: 0.2.8a0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.8/README.md` & `NikeCA-0.2.8a0/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/setup.py` & `NikeCA-0.2.8a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.2.8',
+	version='0.2.8a',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"_BuildSearchQuery",
 		"_GitHub",
 		"_SearchFiles",
 		"_SnowflakeData",
```

### Comparing `NikeCA-0.2.8/src/Dashboards/Dashboards.py` & `NikeCA-0.2.8a0/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/Dashboards/IMP/IMP.py` & `NikeCA-0.2.8a0/src/Dashboards/IMP/IMP.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.2.8a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.2.8a0/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.2.8a0/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.2.8a0/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.8
+Version: 0.2.8a0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.8/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.2.8a0/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.2.8a0/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/NikeQA.py` & `NikeCA-0.2.8a0/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/NikeSF.py` & `NikeCA-0.2.8a0/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/_BuildSearchQuery.py` & `NikeCA-0.2.8a0/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/_GitHub.py` & `NikeCA-0.2.8a0/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/_QA.py` & `NikeCA-0.2.8a0/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/_SearchFiles.py` & `NikeCA-0.2.8a0/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/_SnowflakeData.py` & `NikeCA-0.2.8a0/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.8/src/_SnowflakeDependencies.py` & `NikeCA-0.2.8a0/src/_SnowflakeDependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -262,15 +262,17 @@
                 # read the new file created from the above steps to check for sub-dependencies
                 df_final_tables = []
 
                 try:
                     [df_final_tables.append(v['Object'][v['Object'].rindex('.') + 1:]) for k, v in df_final.iterrows()]
                     df_final_tables = list(set(df_final_tables))
                 except KeyError:
-                    continue
+                    if save_path is not None:
+                        final_df.to_csv(save_path)
+                    return final_df
                 # iterate through the select get_ddl() for the 3375 tables and views in the NGP_DA_PROD database and
                 # look for the dependent table names from the schemas to be divested
                 d = self.snowflake_dependencies_loop(
                     tables=df_final_tables
                     , role=role
                     , database=database
                     , warehouse=warehouse
@@ -287,35 +289,37 @@
 
                     df_final_schemas = list(set(df_final_schemas))
 
                     df_final = self.dict_convert_into_dataframe(d_dict=d_final, cols=col_names,
                                                                 schema_list=df_final_schemas)
 
                 except KeyError:
-                    continue
+                    if save_path is not None:
+                        final_df.to_csv(save_path)
+                    return final_df
 
                 df_final.columns = col_names
 
                 for i, v in final_df.iterrows():
                     for x, y in df_final.iterrows():
                         try:
                             df_final.loc[x, 'MergeCol'] = v['Object'][:str(v['Object']).index('.') + 1] + y['Table']
                         except KeyError:
-                            continue
+                            if save_path is not None:
+                                final_df.to_csv(save_path)
+                            return final_df
                 try:
                     final_df = final_df.merge(df_final, left_on='Object', right_on='MergeCol', how='left',
                                               suffixes=(f'_Round{str(counter)}', f'_Round{str(counter + 1)}'))
                     final_df.drop(columns=['MergeCol'], inplace=True)
                 except KeyError:
-                    continue
 
-                counter += 1
-
-                if save_path is not None:
-                    final_df.to_csv(save_path)
+                    if save_path is not None:
+                        final_df.to_csv(save_path)
+                    return final_df
 
         print('process complete')
 
         return final_df
```

### Comparing `NikeCA-0.2.8/src/_SnowflakePull.py` & `NikeCA-0.2.8a0/src/_SnowflakePull.py`

 * *Files identical despite different names*

