# Comparing `tmp/wildlife-datasets-0.3.3.tar.gz` & `tmp/wildlife-datasets-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adamluk3/Projects/wildlife-datasets/dist/.tmp-ecmv4pbx/wildlife-datasets-0.3.3.tar", last modified: Thu Apr 20 13:41:44 2023, max compression
+gzip compressed data, was "/home/adamluk3/Projects/wildlife-datasets/dist/.tmp-hiblwyxk/wildlife-datasets-0.3.4.tar", last modified: Mon May 15 13:42:45 2023, max compression
```

## Comparing `wildlife-datasets-0.3.3.tar` & `wildlife-datasets-0.3.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.858718 wildlife-datasets-0.3.3/
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1090 2023-02-15 08:36:46.000000 wildlife-datasets-0.3.3/LICENSE
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     7595 2023-04-20 13:42:42.856993 wildlife-datasets-0.3.3/PKG-INFO
--rw-r--r--   0 adamluk3 (436797) ai         (501)     5460 2023-04-19 07:30:02.000000 wildlife-datasets-0.3.3/README.md
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1645 2023-04-20 13:42:22.000000 wildlife-datasets-0.3.3/pyproject.toml
--rw-rw-r--   0 adamluk3 (436797) ai         (501)       38 2023-04-20 13:42:42.860030 wildlife-datasets-0.3.3/setup.cfg
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.676347 wildlife-datasets-0.3.3/wildlife_datasets/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      133 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.3/wildlife_datasets/__init__.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.714094 wildlife-datasets-0.3.3/wildlife_datasets/analysis/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      107 2023-02-14 10:36:30.000000 wildlife-datasets-0.3.3/wildlife_datasets/analysis/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     5059 2023-03-06 09:03:18.000000 wildlife-datasets-0.3.3/wildlife_datasets/analysis/plots.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2698 2023-02-28 08:53:31.000000 wildlife-datasets-0.3.3/wildlife_datasets/analysis/statistics.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.741225 wildlife-datasets-0.3.3/wildlife_datasets/datasets/
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2784 2023-03-17 15:45:48.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    49977 2023-04-20 12:56:02.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/datasets.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     8059 2023-03-17 12:53:50.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/metadata.csv
--rw-r--r--   0 adamluk3 (436797) ai         (501)      822 2023-02-14 14:45:05.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/metadata.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2843 2023-02-10 15:33:13.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/utils.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.784002 wildlife-datasets-0.3.3/wildlife_datasets/downloads/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       25 2023-03-11 08:49:06.000000 wildlife-datasets-0.3.3/wildlife_datasets/downloads/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    26116 2023-04-18 10:44:32.000000 wildlife-datasets-0.3.3/wildlife_datasets/downloads/downloads.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1495 2023-03-16 15:44:33.000000 wildlife-datasets-0.3.3/wildlife_datasets/downloads/utils.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.795113 wildlife-datasets-0.3.3/wildlife_datasets/loader/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       22 2023-02-14 10:26:57.000000 wildlife-datasets-0.3.3/wildlife_datasets/loader/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2958 2023-03-16 15:27:00.000000 wildlife-datasets-0.3.3/wildlife_datasets/loader/loader.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.806196 wildlife-datasets-0.3.3/wildlife_datasets/metrics/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       23 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.3/wildlife_datasets/metrics/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     3269 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.3/wildlife_datasets/metrics/metrics.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.842364 wildlife-datasets-0.3.3/wildlife_datasets/splits/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      191 2023-04-20 11:10:08.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2653 2023-03-07 14:12:11.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/analysis.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1896 2023-04-17 11:37:36.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/balanced_split.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    12258 2023-04-20 13:03:08.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/identity_split.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1753 2023-03-07 14:02:45.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/lcg.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     9516 2023-04-17 12:29:03.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/time_aware_split.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.698273 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     7595 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     1077 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)        1 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)      130 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/requires.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)       18 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/top_level.txt
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-05-15 13:43:49.548591 wildlife-datasets-0.3.4/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1090 2023-02-15 08:36:46.000000 wildlife-datasets-0.3.4/LICENSE
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     5224 2023-05-15 13:43:49.546645 wildlife-datasets-0.3.4/PKG-INFO
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     3090 2023-05-15 10:41:08.000000 wildlife-datasets-0.3.4/README.md
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1645 2023-05-15 13:42:54.000000 wildlife-datasets-0.3.4/pyproject.toml
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)       38 2023-05-15 13:43:49.550134 wildlife-datasets-0.3.4/setup.cfg
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-05-15 13:43:49.398667 wildlife-datasets-0.3.4/wildlife_datasets/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      133 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.4/wildlife_datasets/__init__.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-05-15 13:43:49.439295 wildlife-datasets-0.3.4/wildlife_datasets/analysis/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      107 2023-02-14 10:36:30.000000 wildlife-datasets-0.3.4/wildlife_datasets/analysis/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     5059 2023-03-06 09:03:18.000000 wildlife-datasets-0.3.4/wildlife_datasets/analysis/plots.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2698 2023-02-28 08:53:31.000000 wildlife-datasets-0.3.4/wildlife_datasets/analysis/statistics.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-05-15 13:43:49.467227 wildlife-datasets-0.3.4/wildlife_datasets/datasets/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2784 2023-03-17 15:45:48.000000 wildlife-datasets-0.3.4/wildlife_datasets/datasets/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    51696 2023-05-15 13:36:02.000000 wildlife-datasets-0.3.4/wildlife_datasets/datasets/datasets.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     8059 2023-03-17 12:53:50.000000 wildlife-datasets-0.3.4/wildlife_datasets/datasets/metadata.csv
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      822 2023-02-14 14:45:05.000000 wildlife-datasets-0.3.4/wildlife_datasets/datasets/metadata.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2843 2023-02-10 15:33:13.000000 wildlife-datasets-0.3.4/wildlife_datasets/datasets/utils.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-05-15 13:43:49.484204 wildlife-datasets-0.3.4/wildlife_datasets/downloads/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       25 2023-03-11 08:49:06.000000 wildlife-datasets-0.3.4/wildlife_datasets/downloads/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    26116 2023-04-18 10:44:32.000000 wildlife-datasets-0.3.4/wildlife_datasets/downloads/downloads.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1495 2023-03-16 15:44:33.000000 wildlife-datasets-0.3.4/wildlife_datasets/downloads/utils.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-05-15 13:43:49.495305 wildlife-datasets-0.3.4/wildlife_datasets/loader/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       22 2023-02-14 10:26:57.000000 wildlife-datasets-0.3.4/wildlife_datasets/loader/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2958 2023-03-16 15:27:00.000000 wildlife-datasets-0.3.4/wildlife_datasets/loader/loader.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-05-15 13:43:49.507039 wildlife-datasets-0.3.4/wildlife_datasets/metrics/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       23 2023-05-15 10:50:57.000000 wildlife-datasets-0.3.4/wildlife_datasets/metrics/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     9951 2023-05-15 13:07:44.000000 wildlife-datasets-0.3.4/wildlife_datasets/metrics/metrics.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-05-15 13:43:49.539971 wildlife-datasets-0.3.4/wildlife_datasets/splits/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      191 2023-04-20 11:10:08.000000 wildlife-datasets-0.3.4/wildlife_datasets/splits/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2653 2023-03-07 14:12:11.000000 wildlife-datasets-0.3.4/wildlife_datasets/splits/analysis.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1896 2023-04-17 11:37:36.000000 wildlife-datasets-0.3.4/wildlife_datasets/splits/balanced_split.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    12258 2023-04-20 13:03:08.000000 wildlife-datasets-0.3.4/wildlife_datasets/splits/identity_split.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1753 2023-03-07 14:02:45.000000 wildlife-datasets-0.3.4/wildlife_datasets/splits/lcg.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     9516 2023-04-17 12:29:03.000000 wildlife-datasets-0.3.4/wildlife_datasets/splits/time_aware_split.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-05-15 13:43:49.423625 wildlife-datasets-0.3.4/wildlife_datasets.egg-info/
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     5224 2023-05-15 13:43:49.000000 wildlife-datasets-0.3.4/wildlife_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     1077 2023-05-15 13:43:49.000000 wildlife-datasets-0.3.4/wildlife_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)        1 2023-05-15 13:43:49.000000 wildlife-datasets-0.3.4/wildlife_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)      130 2023-05-15 13:43:49.000000 wildlife-datasets-0.3.4/wildlife_datasets.egg-info/requires.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)       18 2023-05-15 13:43:49.000000 wildlife-datasets-0.3.4/wildlife_datasets.egg-info/top_level.txt
```

### Comparing `wildlife-datasets-0.3.3/LICENSE` & `wildlife-datasets-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/pyproject.toml` & `wildlife-datasets-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wildlife-datasets"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
 ]
 maintainers = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
```

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/analysis/plots.py` & `wildlife-datasets-0.3.4/wildlife_datasets/analysis/plots.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/analysis/statistics.py` & `wildlife-datasets-0.3.4/wildlife_datasets/analysis/statistics.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/datasets/__init__.py` & `wildlife-datasets-0.3.4/wildlife_datasets/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/datasets/datasets.py` & `wildlife-datasets-0.3.4/wildlife_datasets/datasets/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     def check_required_columns(self, df: pd.DataFrame) -> None:
         """Check if all required columns are present.
 
         Args:
             df (pd.DataFrame): A full dataframe of the data.
         """
 
-        for col_name in ['id', 'identity', 'path']:
+        for col_name in ['image_id', 'identity', 'path']:
             if col_name not in df.columns:
                 raise(Exception('Column %s must be in the dataframe columns.' % col_name))
 
     def check_types_columns(self, df: pd.DataFrame) -> None:
         """Checks if columns are in correct formats.
 
         The format are specified in `requirements`, which is list
@@ -147,15 +147,15 @@
         must be at least one of the formats.
 
         Args:
             df (pd.DataFrame): A full dataframe of the data.
         """
 
         requirements = [
-            ('id', ['int', 'str']),
+            ('image_id', ['int', 'str']),
             ('identity', ['int', 'str']),
             ('path', ['str']),
             ('bbox', ['list_numeric']),
             ('date', ['date']),
             ('keypoints', ['list_numeric']),
             ('position', ['str']),
             ('species', ['str', 'list']),
@@ -220,25 +220,25 @@
         Args:
             df (pd.DataFrame): A full dataframe of the data.
 
         Returns:
             A full dataframe of the data, slightly modified.
         """
 
-        default_order = ['id', 'identity', 'path', 'bbox', 'date', 'keypoints', 'orientation', 'segmentation', 'species']
+        default_order = ['image_id', 'identity', 'path', 'bbox', 'date', 'keypoints', 'orientation', 'segmentation', 'species']
         df_names = list(df.columns)
         col_names = []
         for name in default_order:
             if name in df_names:
                 col_names.append(name)
         for name in df_names:
             if name not in default_order:
                 col_names.append(name)
         
-        df = df.sort_values('id').reset_index(drop=True)
+        df = df.sort_values('image_id').reset_index(drop=True)
         return df.reindex(columns=col_names)
 
     def remove_constant_columns(self, df: pd.DataFrame) -> pd.DataFrame:
         """Removes columns with a single unique value.
 
         Args:
             df (pd.DataFrame): A full dataframe of the data.
@@ -255,15 +255,15 @@
     def check_unique_id(self, df: pd.DataFrame) -> None:
         """Checks if values in the id column are unique.
 
         Args:
             df (pd.DataFrame): A full dataframe of the data.
         """
 
-        if len(df['id'].unique()) != len(df):
+        if len(df['image_id'].unique()) != len(df):
             raise(Exception('Image ID not unique.'))
 
     def check_files_exist(self, col: pd.Series) -> None:
         """Checks if paths in a given column exist.
 
         Args:
             col (pd.Series): A column of a dataframe.
@@ -315,14 +315,15 @@
         # Rename empty dates
         df.loc[df['date'] == 'NA', 'date'] = np.nan
 
         # Remove superficial columns
         df = df.drop(['image_id', 'file_name', 'supercategory', 'category_id'], axis=1)
         if len(df['species'].unique()) == 1:
             df = df.drop(['species'], axis=1)
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class AAUZebraFish(DatasetFactory):
     downloader = downloads.AAUZebraFish
     metadata = metadata['AAUZebraFish']
     
@@ -362,14 +363,15 @@
             'path': 'data' + os.path.sep + data['Filename'],
             'identity': data['Object ID'],
             'video': video,
             'bbox': bbox,
             'orientation': orientation,
         })
         df = df.join(attributes)
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class AerialCattle2017(DatasetFactory):
     downloader = downloads.AerialCattle2017
     metadata = metadata['AerialCattle2017']
 
@@ -381,14 +383,15 @@
         # Finalize the dataframe
         df = pd.DataFrame({
             'id': utils.create_id(data['file']),
             'path': data['path'] + os.path.sep + data['file'],
             'identity': folders[1].astype(int),
             'video': folders[2].astype(int),
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class ATRW(DatasetFactory):
     downloader = downloads.ATRW
     metadata = metadata['ATRW']
 
@@ -458,15 +461,16 @@
         df_test2['path'] = 'atrw_detection_test' + os.path.sep + 'test' + os.path.sep + df_test2['file']
         df_test2['id'] = df_test2['imgid'].astype(str) + '_' + df_test2['identity'].astype(str)
         df_test2['split'] = 'test'
         df_test2 = df_test2.drop(['file', 'imgid'], axis=1)
 
         # Finalize the dataframe
         df = pd.concat([df_train, df_test1, df_test2])
-        df['id'] = utils.create_id(df.id.astype(str))
+        df['id'] = utils.create_id(df['id'].astype(str))
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class BelugaID(DatasetFactoryWildMe):
     downloader = downloads.BelugaID
     metadata = metadata['BelugaID']
 
@@ -520,15 +524,17 @@
         df2 = pd.DataFrame({    
             'id': utils.create_id(data['file']),
             'path': self.prefix1 + os.path.sep + 'New_birds' + os.path.sep + data['path'] + os.path.sep + data['file'],
             'identity': self.unknown_name,
             'species': species,
             'split': 'unassigned',
         })
-        return self.finalize_catalogue(pd.concat([df1, df2]))
+        df = pd.concat([df1, df2])
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
+        return self.finalize_catalogue(df)
 
 
 class BirdIndividualIDSegmented(BirdIndividualID):
     downloader = downloads.Segmented
     prefix1 = 'Cropped_pictures'
     prefix2 = 'IndividuaID'
 
@@ -568,14 +574,15 @@
             'age_group': data[7],
             'gender': data[9],
         })
 
         # Replace the wrong identities
         for replace_tuple in replace_names:
             df['identity'] = df['identity'].replace({replace_tuple[0]: replace_tuple[1]})
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class CZoo(DatasetFactory):
     downloader = downloads.CZoo
     metadata = metadata['CZoo']
 
@@ -595,14 +602,15 @@
             'path': path + os.path.sep + data[1],
             'identity': data[3],
             'keypoints': keypoints,
             'age': data[5],
             'age_group': data[7],
             'gender': data[9],
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class Cows2021(DatasetFactory):
     downloader = downloads.Cows2021
     metadata = metadata['Cows2021']
 
@@ -619,14 +627,15 @@
         # Finalize the dataframe
         df = pd.DataFrame({
             'id': utils.create_id(data['file']),
             'path': data['path'] + os.path.sep + data['file'],
             'identity': folders[4].astype(int),
         })
         df['date'] = df['path'].apply(lambda x: self.extract_date(x))
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
     def extract_date(self, x):
         x = os.path.split(x)[1]
         if x.startswith('image_'):
             x = x[6:]
         if x[7] == '_':
@@ -659,14 +668,15 @@
         
         # Create id and path
         data['id'] = utils.create_id(folders[0] + data['file'])
         data['path'] = data['path'] + os.path.sep + data['file']
         
         # Finalize the dataframe
         df = data.drop(['file'], axis=1)
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class FriesianCattle2015(DatasetFactory):
     downloader = downloads.FriesianCattle2015
     metadata = metadata['FriesianCattle2015']
 
@@ -682,14 +692,15 @@
         # Finalize the dataframe
         df = pd.DataFrame({
             'id': utils.create_id(identity.astype(str) + split + data['file']),
             'path': data['path'] + os.path.sep + data['file'],
             'identity': identity,
             'split': split
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class FriesianCattle2017(DatasetFactory):
     downloader = downloads.FriesianCattle2017
     metadata = metadata['FriesianCattle2017']
 
@@ -700,14 +711,15 @@
 
         # Finalize the dataframe
         df = pd.DataFrame({
             'id': utils.create_id(data['file']),
             'path': data['path'] + os.path.sep + data['file'],
             'identity': folders[1].astype(int),
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class GiraffeZebraID(DatasetFactoryWildMe):
     downloader = downloads.GiraffeZebraID
     metadata = metadata['GiraffeZebraID']
     
@@ -731,14 +743,15 @@
 
         # Finalize the dataframe
         df = pd.DataFrame({    
             'id': utils.create_id(data['file']),
             'path': path + os.path.sep + data['path'] + os.path.sep + data['file'],
             'identity': folders[1],
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class HappyWhale(DatasetFactory):
     downloader = downloads.HappyWhale
     metadata = metadata['HappyWhale']
     
@@ -773,15 +786,16 @@
             'path': 'test_images' + os.path.sep + test_files,
             'identity': self.unknown_name,
             'species': np.nan,
             'split': 'test'
             })
         
         # Finalize the dataframe        
-        df = pd.concat([df1, df2])    
+        df = pd.concat([df1, df2])
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class HumpbackWhaleID(DatasetFactory):
     downloader = downloads.HumpbackWhaleID
     metadata = metadata['HumpbackWhaleID']
 
@@ -806,15 +820,16 @@
             'id': test_files.str.split('.', expand=True)[0],
             'path': 'test' + os.path.sep + test_files,
             'identity': self.unknown_name,
             'split': 'test'
             })
         
         # Finalize the dataframe
-        df = pd.concat([df1, df2])    
+        df = pd.concat([df1, df2])
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class HyenaID2022(DatasetFactoryWildMe):
     downloader = downloads.HyenaID2022
     metadata = metadata['HyenaID2022']
 
@@ -853,14 +868,15 @@
         # Finalize the dataframe
         df = pd.DataFrame({
             'id': utils.create_id(data['file']),
             'path': data['path'] + os.path.sep + data['file'],
             'identity': folders[1],
             'keypoints': keypoints
             })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class LeopardID2022(DatasetFactoryWildMe):
     downloader = downloads.LeopardID2022
     metadata = metadata['LeopardID2022']
 
@@ -879,14 +895,15 @@
 
         # Finalize the dataframe
         df = pd.DataFrame({
             'id': utils.create_id(data['file']),
             'path': data['path'] + os.path.sep + data['file'],
             'identity': folders[3],
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class MacaqueFaces(DatasetFactory):
     downloader = downloads.MacaqueFaces
     metadata = metadata['MacaqueFaces']
     
@@ -899,14 +916,15 @@
         df = pd.DataFrame({
             'id': pd.Series(range(len(data))),
             'path': 'MacaqueFaces' + os.path.sep + data['Path'].str.strip(os.path.sep) + os.path.sep + data['FileName'],
             'identity': data['ID'],
             'date': pd.Series(date_taken),
             'category': data['Category']
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class NDD20(DatasetFactory):
     downloader = downloads.NDD20
     metadata = metadata['NDD20']
 
@@ -967,14 +985,15 @@
         if len(df.reg_type.unique()) != 1:
             raise(Exception('Multiple segmentation types'))
 
         # Finalize the dataframe
         df['id'] = range(len(df))
         df['path'] = df['orientation'].str.upper() + os.path.sep + df['file_name']
         df = df.drop(['reg_type', 'file_name'], axis=1)
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class NOAARightWhale(DatasetFactory):
     downloader = downloads.NOAARightWhale
     metadata = metadata['NOAARightWhale']
 
@@ -993,15 +1012,16 @@
         df2 = pd.DataFrame({
             'id': data['Image'].str.split('.', expand=True)[0].str.strip('w_').astype(int),
             'path': 'imgs' + os.path.sep + data['Image'],
             'identity': self.unknown_name,
             })
         
         # Finalize the dataframe
-        df = pd.concat([df1, df2])    
+        df = pd.concat([df1, df2])
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class NyalaData(DatasetFactory):
     downloader = downloads.NyalaData
     metadata = metadata['NyalaData']
 
@@ -1019,14 +1039,15 @@
         # Finalize the dataframe
         df = pd.DataFrame({
             'id': utils.create_id(data['file']),
             'path': data['path'] + os.path.sep + data['file'],
             'identity': identity,
             'orientation': orientation,
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)   
 
 
 class OpenCows2020(DatasetFactory):
     downloader = downloads.OpenCows2020
     metadata = metadata['OpenCows2020']
 
@@ -1046,14 +1067,15 @@
         # Finalize the dataframe
         df = pd.DataFrame({
             'id': utils.create_id(identity.astype(str) + split + data['file']),
             'path': data['path'] + os.path.sep + data['file'],
             'identity': identity,
             'split': split
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)    
 
 
 class SealID(DatasetFactory):
     downloader = downloads.SealID
     metadata = metadata['SealID']
     prefix = 'source_'
@@ -1066,14 +1088,15 @@
         df = pd.DataFrame({    
             'id': data['file'].str.split('.', expand=True)[0],
             'path': 'full images' + os.path.sep + self.prefix + data['reid_split'] + os.path.sep + data['file'],
             'identity': data['class_id'].astype(int),
             'reid_split': data['reid_split'],
             'segmentation_split': data['segmentation_split'],
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class SealIDSegmented(SealID):
     downloader = downloads.Segmented
     prefix = 'segmented_'
 
@@ -1099,14 +1122,15 @@
         # Merge the information from the JSON file
         df = pd.merge(df_annotation, df_images, on='image_id')
         df['path'] = 'images' + os.path.sep + df['identity'] + os.path.sep + df['file_name']        
         df = df.drop(['image_id', 'file_name'], axis=1)
         df['date'] = df['date'].apply(lambda x: x[:4] + '-' + x[5:7] + '-' + x[8:])
 
         # Finalize the dataframe
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class SeaTurtleIDHeads(DatasetFactory):
     downloader = downloads.SeaTurtleIDHeads
     metadata = metadata['SeaTurtleIDHeads']
 
@@ -1125,14 +1149,15 @@
         # Merge the information from the JSON file
         df = pd.merge(df_annotation, df_images, on='image_id')
         df['path'] = 'images' + os.path.sep + df['identity'] + os.path.sep + df['file_name']        
         df = df.drop(['image_id', 'file_name'], axis=1)
         df['date'] = df['date'].apply(lambda x: x[:4] + '-' + x[5:7] + '-' + x[8:])
 
         # Finalize the dataframe
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class SMALST(DatasetFactory):
     downloader = downloads.SMALST
     metadata = metadata['SMALST']
 
@@ -1154,14 +1179,15 @@
         path = masks['file'].str.strip('zebra_')
         masks['id'] = [int(p[1:].strip('_frame_').split('.')[0]) for p in path]
         masks['segmentation'] = 'zebra_training_set' + os.path.sep + 'bgsub' + os.path.sep + masks['file']
         masks = masks.drop(['path', 'file'], axis=1)
 
         # Finalize the dataframe
         df = pd.merge(data, masks, on='id')
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
 
 
 class StripeSpotter(DatasetFactory):
     downloader = downloads.StripeSpotter
     metadata = metadata['StripeSpotter']
 
@@ -1184,14 +1210,15 @@
             'id': utils.create_id(data['file']),
             'path':  data['path'] + os.path.sep + data['file'],
             'identity': data['animal_name'],
             'bbox': pd.Series([[int(a) for a in b.split(' ')] for b in data['roi']]),
             'orientation': data['flank'],
             'photo_quality': data['photo_quality'],
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)  
 
 
 class WhaleSharkID(DatasetFactoryWildMe):
     downloader = downloads.WhaleSharkID
     metadata = metadata['WhaleSharkID']
 
@@ -1220,14 +1247,15 @@
         data = pd.merge(data, df_keypoints, how='left', on='file')
         data['id'] = utils.create_id(data['file'])
         data['identity'] = folders[1].astype(int)
         data['path'] = data['path'] + os.path.sep + data['file']
         data = data.drop(['file'], axis=1)
 
         # Finalize the dataframe
+        data.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(data)
 
     def extract_keypoints(self, row: pd.DataFrame) -> List[float]:
         keypoints = [row['keypoints']['too']['median_x'], row['keypoints']['too']['median_y'],
                 row['keypoints']['toh']['median_x'], row['keypoints']['toh']['median_y'],
                 row['keypoints']['ni']['median_x'], row['keypoints']['ni']['median_y'],
                 row['keypoints']['fbh']['median_x'], row['keypoints']['fbh']['median_y'],
@@ -1261,8 +1289,9 @@
         df = pd.DataFrame({
             'id': data['image_id'],
             'path': 'images' + os.path.sep + data['image_id'] + '.JPG',
             'identity': data['turtle_id'],
             'orientation': data['image_location'].str.lower(),
             'split': data['split'],
         })
+        df.rename({'id': 'image_id'}, axis=1, inplace=True)
         return self.finalize_catalogue(df)
```

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/datasets/metadata.csv` & `wildlife-datasets-0.3.4/wildlife_datasets/datasets/metadata.csv`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/datasets/metadata.py` & `wildlife-datasets-0.3.4/wildlife_datasets/datasets/metadata.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/datasets/utils.py` & `wildlife-datasets-0.3.4/wildlife_datasets/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/downloads/downloads.py` & `wildlife-datasets-0.3.4/wildlife_datasets/downloads/downloads.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/downloads/utils.py` & `wildlife-datasets-0.3.4/wildlife_datasets/downloads/utils.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/loader/loader.py` & `wildlife-datasets-0.3.4/wildlife_datasets/loader/loader.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/splits/analysis.py` & `wildlife-datasets-0.3.4/wildlife_datasets/splits/analysis.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/splits/balanced_split.py` & `wildlife-datasets-0.3.4/wildlife_datasets/splits/balanced_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/splits/identity_split.py` & `wildlife-datasets-0.3.4/wildlife_datasets/splits/identity_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/splits/lcg.py` & `wildlife-datasets-0.3.4/wildlife_datasets/splits/lcg.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets/splits/time_aware_split.py` & `wildlife-datasets-0.3.4/wildlife_datasets/splits/time_aware_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.3/wildlife_datasets.egg-info/SOURCES.txt` & `wildlife-datasets-0.3.4/wildlife_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

