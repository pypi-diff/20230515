# Comparing `tmp/sportydatagen-0.2.1.tar.gz` & `tmp/sportydatagen-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportydatagen-0.2.1.tar", max compression
+gzip compressed data, was "sportydatagen-0.2.2.tar", max compression
```

## Comparing `sportydatagen-0.2.1.tar` & `sportydatagen-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-05-09 12:00:11.363491 sportydatagen-0.2.1/LICENSE
--rw-r--r--   0        0        0     1576 2023-05-09 12:00:11.363491 sportydatagen-0.2.1/README.md
--rw-r--r--   0        0        0     1800 2023-05-09 12:00:11.537493 sportydatagen-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      372 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/__init__.py
--rw-r--r--   0        0        0     5358 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/activity.py
--rw-r--r--   0        0        0     7186 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/convert_to_csv.py
--rw-r--r--   0        0        0     5419 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/csv_utils.py
--rw-r--r--   0        0        0     9004 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/feature_extraction_utils.py
--rw-r--r--   0        0        0      142 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/filetype.py
--rw-r--r--   0        0        0     8126 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/return_random_data.py
--rw-r--r--   0        0        0     2895 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/saf_extract_features_to_csv.py
--rw-r--r--   0        0        0      477 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/sportfile_utils.py
--rw-r--r--   0        0        0     2514 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/utils.py
--rw-r--r--   0        0        0     2358 2023-05-09 12:00:23.577822 sportydatagen-0.2.1/setup.py
--rw-r--r--   0        0        0     2298 2023-05-09 12:00:23.578082 sportydatagen-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-15 12:44:00.642575 sportydatagen-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1576 2023-05-15 12:44:00.642575 sportydatagen-0.2.2/README.md
+-rw-r--r--   0        0        0     1906 2023-05-15 12:44:00.796576 sportydatagen-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      372 2023-05-15 12:44:00.796576 sportydatagen-0.2.2/sportydatagen/__init__.py
+-rw-r--r--   0        0        0     5201 2023-05-15 12:44:00.796576 sportydatagen-0.2.2/sportydatagen/activity.py
+-rw-r--r--   0        0        0       37 2023-05-15 12:44:00.796576 sportydatagen-0.2.2/sportydatagen/cluster/__init__.py
+-rw-r--r--   0        0        0     5881 2023-05-15 12:44:00.796576 sportydatagen-0.2.2/sportydatagen/cluster/kmeans.py
+-rw-r--r--   0        0        0     7219 2023-05-15 12:44:00.796576 sportydatagen-0.2.2/sportydatagen/convert_to_csv.py
+-rw-r--r--   0        0        0     5333 2023-05-15 12:44:00.796576 sportydatagen-0.2.2/sportydatagen/csv_utils.py
+-rw-r--r--   0        0        0     8891 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/feature_extraction_utils.py
+-rw-r--r--   0        0        0      142 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/filetype.py
+-rw-r--r--   0        0        0       44 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/plot/__init__.py
+-rw-r--r--   0        0        0     1338 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/plot/correlation_heatmap.py
+-rw-r--r--   0        0        0      869 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/plot/frequency_distribution.py
+-rw-r--r--   0        0        0     2316 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/plot/kmeans_scatter_plot.py
+-rw-r--r--   0        0        0     1069 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/plot/retention_value.py
+-rw-r--r--   0        0        0     7781 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/return_random_data.py
+-rw-r--r--   0        0        0     2827 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/saf_extract_features_to_csv.py
+-rw-r--r--   0        0        0      477 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/sportfile_utils.py
+-rw-r--r--   0        0        0     2367 2023-05-15 12:44:00.797576 sportydatagen-0.2.2/sportydatagen/utils.py
+-rw-r--r--   0        0        0     2436 2023-05-15 12:44:07.236393 sportydatagen-0.2.2/setup.py
+-rw-r--r--   0        0        0     2343 2023-05-15 12:44:07.236832 sportydatagen-0.2.2/PKG-INFO
```

### Comparing `sportydatagen-0.2.1/LICENSE` & `sportydatagen-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.2.1/README.md` & `sportydatagen-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.2.1/pyproject.toml` & `sportydatagen-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "sportydatagen"
-version = "0.2.1"
+version = "0.2.2"
 description = "Sports activity generator module"
 license="MIT"
 readme = "README.md"
 keywords = ['artificial sport trainer', 'computational intelligence', 'data mining', 'sport activities', 'tcx']
 authors = ["Rok Kukovec <rok.kukovec1@student.um.si>", "Iztok Fister Jr. <iztok@iztok-jr-fister.eu>"]
 homepage = "https://gitlab.com/firefly-cpp/sportydatagen"
 repository = "https://gitlab.com/firefly-cpp/sportydatagen"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 niapy = "^2.0.5"
 sport-activities-features = "^0.3.12"
 numpy = "^1.24.2"
 pandas = "*"
+scikit-learn = "^1.2.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 black = "^23.1.0"
 isort = "^5.12.0"
 ruff = "^0.0.265"
 
@@ -65,14 +66,18 @@
 
 [tool.ruff.per-file-ignores]
 'basic_run.py' = ['T201'] # Prints output into console
 # Delete next 3 lines in release version
 'sportydatagen/*.py' = ['T201'] # Prints progress into console
 'examples/*.py' = ['T201'] # Prints progress into console
 'tests/*.py' = ['S101']
+'docs/*.py' = ['INP001','A001']
 
 [tool.ruff.flake8-quotes]
 inline-quotes = 'single'
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
+
+[tool.pytest.ini_options]
+testpaths =  "./tests"
```

### Comparing `sportydatagen-0.2.1/sportydatagen/activity.py` & `sportydatagen-0.2.2/sportydatagen/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,32 @@
         ascent (float): Ascent during the activity.
         descent (float): Descent during the activity.
         speed_max (float): Maximum speed during the activity.
         speed_avg (float): Average speed during the activity.
         file_name (str): Name of the file containing the activity.
     """
 
-    def __init__(self: 'Activity',
-                 activity_type: str = None,
-                 distance: float = None,
-                 duration: float = None,
-                 calories: float = None,
-                 hr_avg: float = None,
-                 hr_min: float = None,
-                 hr_max: float = None,
-                 altitude_avg: float = None,
-                 altitude_min: float = None,
-                 altitude_max: float = None,
-                 ascent: float = None,
-                 descent: float = None,
-                 speed_max: float = None,
-                 speed_avg: float = None,
-                 file_name: str = None) -> None:
+    def __init__(
+        self: 'Activity',
+        activity_type: str = None,
+        distance: float = None,
+        duration: float = None,
+        calories: float = None,
+        hr_avg: float = None,
+        hr_min: float = None,
+        hr_max: float = None,
+        altitude_avg: float = None,
+        altitude_min: float = None,
+        altitude_max: float = None,
+        ascent: float = None,
+        descent: float = None,
+        speed_max: float = None,
+        speed_avg: float = None,
+        file_name: str = None,
+    ) -> None:
         """Initialize the activity."""
         self.activity_type = activity_type
         self.duration = duration
         self.distance = distance
         self.calories = calories
         self.hr_avg = hr_avg
         self.hr_min = hr_min
@@ -55,69 +57,84 @@
         self.descent = descent
         self.speed_max = speed_max
         self.speed_avg = speed_avg
         self.file_name = file_name
 
     def __str__(self: 'Activity') -> str:
         """Return the string representation of the activity."""
-        return (f'Activity: {self.activity_type}, '
-                f'Total duration: {self.duration} seconds, '
-                f'Total distance: {self.distance} meters, '
-                f'Calories burned: {self.calories}, '
-                f'Average hertrate: {self.hr_avg}, '
-                f'Minimum heartrate: {self.hr_min}, '
-                f'Maximum heartrate: {self.hr_max}, '
-                f'Average altitude: {self.altitude_avg}, '
-                f'Minimum altitude: {self.altitude_min}, '
-                f'Maximum altitude: {self.altitude_max}, '
-                f'Ascent: {self.ascent}, '
-                f'Descent: {self.descent}, '
-                f'Maximum speed: {self.speed_max}, '
-                f'Average speed: {self.speed_avg}, '
-                f'Original filename: {self.file_name}'
-                )
+        return (
+            f'Activity: {self.activity_type}, '
+            f'Total duration: {self.duration} seconds, '
+            f'Total distance: {self.distance} meters, '
+            f'Calories burned: {self.calories}, '
+            f'Average hertrate: {self.hr_avg}, '
+            f'Minimum heartrate: {self.hr_min}, '
+            f'Maximum heartrate: {self.hr_max}, '
+            f'Average altitude: {self.altitude_avg}, '
+            f'Minimum altitude: {self.altitude_min}, '
+            f'Maximum altitude: {self.altitude_max}, '
+            f'Ascent: {self.ascent}, '
+            f'Descent: {self.descent}, '
+            f'Maximum speed: {self.speed_max}, '
+            f'Average speed: {self.speed_avg}, '
+            f'Original filename: {self.file_name}'
+        )
 
     def get_activity_type(self: 'Activity') -> str:
         """Return the type of the activity."""
         return self.activity_type
+
     def get_total_duration(self: 'Activity') -> float:
         """Return the total duration of the activity."""
         return self.duration
+
     def get_total_distance(self: 'Activity') -> float:
         """Return total distance in seconds of the activity."""
         return self.distance
+
     def get_calories(self: 'Activity') -> float:
         """Return the calories burned during the activity."""
         return self.calories
+
     def get_avg_hr(self: 'Activity') -> float:
         """Return the average heartrate during the activity."""
         return self.hr_avg
+
     def get_min_hr(self: 'Activity') -> float:
         """Return the minimum heartrate during the activity."""
         return self.hr_min
+
     def get_max_hr(self: 'Activity') -> float:
         """Return the maximum heartrate during the activity."""
         return self.hr_max
+
     def get_avg_altitude(self: 'Activity') -> float:
         """Return the average altitude during the activity."""
         return self.altitude_avg
+
     def get_min_altitude(self: 'Activity') -> float:
         """Return the minimum altitude during the activity."""
         return self.altitude_min
+
     def get_max_altitude(self: 'Activity') -> float:
         """Return the maximum altitude during the activity."""
         return self.altitude_max
+
     def get_ascent(self: 'Activity') -> float:
         """Return the ascent during the activity."""
         return self.ascent
+
     def get_descent(self: 'Activity') -> float:
         """Return the descent during the activity."""
         return self.descent
+
     def get_max_speed(self: 'Activity') -> float:
         """Return the maximum speed during the activity."""
         return self.speed_max
+
     def get_avg_speed(self: 'Activity') -> float:
         """Return the average speed during the activity."""
         return self.speed_avg
+
     def get_file_name(self: 'Activity') -> str:
         """Return the original filename of the activity."""
         return self.file_name
```

### Comparing `sportydatagen-0.2.1/sportydatagen/convert_to_csv.py` & `sportydatagen-0.2.2/sportydatagen/convert_to_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     check_file_delete_csv_if_columns_are_nan,
     delete_empty_csv_files,
 )
 
 
 # Function to merge CSV files
 def merge_csv_files(
-        input_files: list,
-        output_file: str,
+    input_files: list,
+    output_file: str,
 ) -> None:
     """Merge CSV files with same columns."""
     # Path to output file
     output_file = str(Path(output_file))
 
     # List of DataFrames
     dataframes = []
@@ -52,72 +52,81 @@
     merged_dataframe = merged_dataframe[cols]
 
     # Write merged DataFrame to CSV file
     merged_dataframe.to_csv(output_file, index=False, sep=';')
 
 
 def check_missing_only_heartrates(
-        df: pd.DataFrame,
-        percent_miss_hr_allowed: int = 3,
+    df: pd.DataFrame,
+    percent_miss_hr_allowed: int = 3,
 ) -> bool:
     """Check if only heartrates are missing and in less than 3%."""
     # Get percentage of missing values for each column
     percent_missing_values = 100 * df.isna().sum() / len(df)
     # Create table with results
     missing_values_df = pd.concat([percent_missing_values], axis=1)
     # Rename column
     mis_val_table_ren_columns = missing_values_df.rename(
-    columns = {0 : '% of missing total values'})
+        columns={0: '% of missing total values'},
+    )
     # Sort table by percentage of missing values
     # Only keep columns with missing values
-    mis_val_table_ren_columns = mis_val_table_ren_columns[
-        mis_val_table_ren_columns.iloc[:,0] != 0].sort_values(
-    '% of missing total values', ascending=False).round(1)
+    mis_val_table_ren_columns = (
+        mis_val_table_ren_columns[mis_val_table_ren_columns.iloc[:, 0] != 0]
+        .sort_values('% of missing total values', ascending=False)
+        .round(1)
+    )
     # If only one column is missing
-    return len(mis_val_table_ren_columns) == 1 and (
-        # And that column is heartrates
-        mis_val_table_ren_columns.index[0] == 'heartrates') and (
-        # And that column has less than 2% of missing values
-        mis_val_table_ren_columns['% of missing total values'][0]
-                                        < percent_miss_hr_allowed)
+    return (
+        len(mis_val_table_ren_columns) == 1
+        and (
+            # And that column is heartrates
+            mis_val_table_ren_columns.index[0]
+            == 'heartrates'
+        )
+        and (
+            # And that column has less than 2% of missing values
+            mis_val_table_ren_columns['% of missing total values'][0]
+            < percent_miss_hr_allowed
+        )
+    )
 
 
 def fill_empty_heartrates(heartrates: pd.Series) -> pd.Series:
     """Fill empty heartrates with linear interpolation."""
     try:
         heartrates = heartrates.interpolate(
-            method='linear',
-            limit=45,
-            limit_direction='both')
+            method='linear', limit=45, limit_direction='both',
+        )
         if str(heartrates[0]) == 'nan':
             heartrates[0] = heartrates[1]
-        if str(heartrates[len(heartrates)-1]) == 'nan':
-            heartrates[len(heartrates)-1] = heartrates[len(heartrates)-2]
+        if str(heartrates[len(heartrates) - 1]) == 'nan':
+            heartrates[len(heartrates) - 1] = heartrates[len(heartrates) - 2]
     except ValueError:
         # Too many consecutive NaN values
         return heartrates
     return heartrates
 
 
 def check_file_type(
-        input_file: str,
+    input_file: str,
 ) -> TCXFile | GPXFile | None:
     """Check file type and return corresponding class."""
     if input_file.endswith('.tcx'):
         # Class for reading TCX files
         return TCXFile()
     if input_file.endswith('.gpx'):
         # Class for reading GPX files
         return GPXFile()
     return None
 
 
 def convert_single_file(
-        input_file: str,
-        output_dir: str,
+    input_file: str,
+    output_dir: str,
 ) -> pd.DataFrame | None:
     """Read and convert TCX/GPX file to CSV file."""
     sport_file = check_file_type(input_file)
 
     data = sport_file.read_one_file(input_file)
     if data is None:
         print('File format not supported: ' + input_file)
@@ -157,53 +166,57 @@
 
         # Round DataFrame to 2 decimals
         df_to_csv = df_to_csv.round(
             {'altitudes': 2, 'distances': 2, 'speeds': 2},
         )
         # Check if DataFrame contains NaN values
         # and if only heartrates are missing
-        if df_to_csv.isna().to_numpy().any() and \
-                check_missing_only_heartrates(df_to_csv):
+        if df_to_csv.isna().to_numpy().any() and check_missing_only_heartrates(
+            df_to_csv,
+        ):
             # Interpolate missing heartrates
             df_to_csv['heartrates'] = fill_empty_heartrates(
-                                        df_to_csv['heartrates'])
+                df_to_csv['heartrates'],
+            )
         # Some GPX files are missing heartrates
         try:
             # Remove decimals from heartrates
             df_to_csv['heartrates'] = df_to_csv.heartrates.apply(int)
         except TypeError:
             contextlib.suppress(TypeError)
         # Save DataFrame to CSV file with semicolon as separator
         df_to_csv.to_csv(output_file, header=True, sep=';')
     except ValueError:
         print('Error reading file: ' + input_file)
         pass
     return df_to_csv
 
+
 def convert_directory_of_files_to_csv(
     input_sportfile_directory: str,
     output_csv_dir: str,
 ) -> None:
     """Read and convert all TCX/GPX files in directory to CSV files."""
     for filename in os.listdir(input_sportfile_directory):
         # Path to input TCX/GPX file
         input_file = str(Path(input_sportfile_directory, filename))
         # Path to newly created output CSV file
         convert_single_file(input_file, output_csv_dir)
 
 
 def convert_sportfiles_and_remove_empty_csvs(
-        input_sportfile_directory: str,
-        output_csv_dir: str,
-    ) -> None:
+    input_sportfile_directory: str,
+    output_csv_dir: str,
+) -> None:
     """Read, convert and remove empty csv files."""
     # Read and convert TCX files to CSV files
     convert_directory_of_files_to_csv(
         input_sportfile_directory=input_sportfile_directory,
-        output_csv_dir=output_csv_dir)
+        output_csv_dir=output_csv_dir,
+    )
     # Remove empty CSV files
     delete_empty_csv_files(csv_directory=output_csv_dir)
     # Remove CSV files with NaN values
     check_file_delete_csv_if_columns_are_nan(
         csv_directory=output_csv_dir,
-        columns_to_check=None, # If None, all columns are checked
+        columns_to_check=None,  # If None, all columns are checked
     )
```

### Comparing `sportydatagen-0.2.1/sportydatagen/csv_utils.py` & `sportydatagen-0.2.2/sportydatagen/csv_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 tcx_file = TCXFile()
 
 
 def create_list_of_all_possible_files(number_of_files: int) -> list:
     """Create a list of all possible files.
 
     Args:
-    ----------------
-        number_of_files (int): Number of files.
+    ----
+    number_of_files (int): Number of files.
 
     Returns:
-    ----------------
-        all_possible_csv_files (list): List of all possible files."""
+    -------
+    all_possible_csv_files (list): List of all possible files.
+    """
     all_possible_csv_files = []
     for i in range(1, number_of_files + 1):
         all_possible_csv_files.append(f'{i}.csv')
     return all_possible_csv_files
 
 
 def missing_csv_files(directory_path: str, number_of_files: int) -> list:
@@ -33,20 +34,20 @@
 
     Prints missing files from all possible numbered
     sequence of tcx/gpx files converted to csv files. Csv files are stored in
     tcx_csv directory. The script will print a list of missing files.
     Files are missing if they have not been correctly converted to csv format.
 
     Args:
-    ----------------
+    ----
     directory_path (str): Path to directory with csv files.
     number_of_files (int): Number of files.
 
     Returns:
-    ----------------
+    -------
     str: List of missing files.
     """
     csv_files_in_directory = os.listdir(Path(directory_path))
 
     all_possible_files = create_list_of_all_possible_files(number_of_files)
 
     set_of_actual_csv_files = set(csv_files_in_directory)
@@ -78,27 +79,27 @@
         if temp_file_size <= basically_empty:
             print(f'Empty csv file: {file} in {csv_directory} directory')
             Path.unlink(Path(csv_directory, file))
 
 
 # Function to check if heartrate exists
 def check_file_delete_csv_if_columns_are_nan(
-        csv_directory: str,
-        columns_to_check: list = None,
+    csv_directory: str,
+    columns_to_check: list = None,
 ) -> None:
     """Check if columns are nan in df and delete corresponding csv file.
 
     Args:
-    ----------------
-        csv_directory (str): Path to csv directory.
-        columns_to_check (list): List of columns to check.
+    ----
+    csv_directory (str): Path to csv directory.
+    columns_to_check (list): List of columns to check.
 
     Returns:
-    ----------------
-        None
+    -------
+    None
     """
     if columns_to_check is None:
         columns_to_check = [
             'heartrates',
             'latitude',
             'longitude',
             'altitudes',
```

### Comparing `sportydatagen-0.2.1/sportydatagen/feature_extraction_utils.py` & `sportydatagen-0.2.2/sportydatagen/feature_extraction_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 from sportydatagen.filetype import Filetype
 
 
 def calculate_duration(read_df_tcx_csv: pd.DataFrame) -> int:
     """Calculate duration of activity in seconds.
 
     Args:
-    ----------------
-        read_df_tcx_csv (pd.DataFrame): Dataframe with timestamps.
+    ----
+    read_df_tcx_csv (pd.DataFrame): Dataframe with timestamps.
+
     Returns:
-    ----------------
-        total_seconds (int): Duration of activity in seconds.
+    -------
+    total_seconds (int): Duration of activity in seconds.
     """
     try:
         start_time = dt.datetime.strptime(
             read_df_tcx_csv['timestamps'][0],
             '%Y-%m-%d %H:%M:%S',
         ).astimezone()
         end_time = dt.datetime.strptime(
@@ -51,16 +52,17 @@
                 '%Y-%m-%d %H:%M:%S%z',
             ).astimezone()
             end_time = dt.datetime.strptime(
                 read_df_tcx_csv['timestamps'][len(read_df_tcx_csv) - 1],
                 '%Y-%m-%d %H:%M:%S%z',
             ).astimezone()
         except ValueError:
-            error_message = ('Timestamps in dataframe are not'
-                            ' in ISO 8601 format')
+            error_message = (
+                'Timestamps in dataframe are not in ISO 8601 format'
+            )
             raise ValueError from ValueError(error_message)
     except KeyError:
         error_message = 'No column timestamp in dataframe'
         raise KeyError from KeyError(error_message)
 
     return int((end_time - start_time).total_seconds())
 
@@ -82,29 +84,28 @@
     read_df_tcx_csv['descent'] = (-diff).where(diff < 0, 0)
     # Sum of dataframe column descent
     full_descent = read_df_tcx_csv['descent'].sum()
     return full_ascent, full_descent
 
 
 def extract_features(
-        read_df_csv: pd.DataFrame,
-        sport_file: GPXFile() or TCXFile() or None = None,
-        sportfile_directory: str | None = None,
-        original_filename: str | None = None,
-        index: int = 1) -> dict:
+    read_df_csv: pd.DataFrame,
+    sport_file: GPXFile() or TCXFile() or None = None,
+    sportfile_directory: str | None = None,
+    original_filename: str | None = None,
+    index: int = 1,
+) -> dict:
     """Extract features from a single TCX/GPX file."""
     calories = 'NULL'
     lucia_trimp = 'NULL'
     edwards_trimp = 'NULL'
 
     # Extract metrics manually from dataframe
     activity_type = read_df_csv['activity_type'][0]
-    total_distance = read_df_csv['total_distance'][
-        len(read_df_csv) - 1
-        ]
+    total_distance = read_df_csv['total_distance'][len(read_df_csv) - 1]
     hr_avg = read_df_csv['heartrates'].mean()
     hr_max = read_df_csv['heartrates'].max()
     hr_min = read_df_csv['heartrates'].min()
     altitude_avg = read_df_csv['altitudes'].mean()
     altitude_max = read_df_csv['altitudes'].max()
     altitude_min = read_df_csv['altitudes'].min()
     duration = calculate_duration(read_df_csv)
@@ -127,29 +128,32 @@
     if sport_file is not None and sportfile_directory is not None:
         if original_filename is None:
             original_filename = 'NULL'
             relative_path_of_original_file = None
         else:
             # Check if original file exists
             relative_path_of_original_file = Path(
-                sportfile_directory, original_filename)
-        if relative_path_of_original_file is not None \
-                and Path.exists(Path(sportfile_directory, original_filename)):
+                sportfile_directory, original_filename,
+            )
+        if relative_path_of_original_file is not None and Path.exists(
+            Path(sportfile_directory, original_filename),
+        ):
             # Extract Integral Metrics using sports_activities_features
             activity_metrics = sport_file.extract_integral_metrics(
-                str(relative_path_of_original_file))
+                str(relative_path_of_original_file),
+            )
             # Extract calories from dictionary
             calories = activity_metrics['calories']
             activity = sport_file.read_one_file(relative_path_of_original_file)
             timestamps = activity['timestamps']
             heart_rates = activity['heartrates']
 
-            edwards = EdwardsTRIMP(heart_rates,
-                                   timestamps,
-                                   max_heart_rate=hr_max)
+            edwards = EdwardsTRIMP(
+                heart_rates, timestamps, max_heart_rate=hr_max,
+            )
             edwards_trimp = edwards.calculate_TRIMP()
 
             lucia = LuciaTRIMP(heart_rates, timestamps, VT1=160, VT2=180)
             lucia_trimp = lucia.calculate_TRIMP()
 
     # Calories are not available in TCX files
     # they are calculated in sport_activities_features
@@ -173,15 +177,14 @@
         'banister_TRIMP': banister_trimp_v2,
         'edwards_TRIMP': edwards_trimp,
         'lucia_TRIMP': lucia_trimp,
         'file_name': original_filename,
     }
 
 
-
 def extract_single_sportfile_metrics_to_csv(
     read_df_csv: pd.DataFrame,
     sportfile_directory: str | None = None,
     original_filename: str | None = None,
     index: int = 1,
 ) -> dict | None:
     """Metric extraction from sports file using saf.
@@ -193,19 +196,21 @@
     if original_filename is not None:
         if original_filename.endswith('.gpx'):
             sport_file = GPXFile()
         elif original_filename.endswith('.tcx'):
             sport_file = TCXFile()
 
     # Extract Integral Metrics using sports_activities_features
-    return extract_features(read_df_csv=read_df_csv,
-                            sport_file=sport_file,
-                            sportfile_directory=sportfile_directory,
-                            original_filename=original_filename,
-                            index=index)
+    return extract_features(
+        read_df_csv=read_df_csv,
+        sport_file=sport_file,
+        sportfile_directory=sportfile_directory,
+        original_filename=original_filename,
+        index=index,
+    )
 
 
 def extract_features_csv_files_directory_to_csv(
     input_csv_directory: str,
     output_file: str,
     filetype: Filetype = Filetype.UNKNOWN,
     sportfile_directory: str | None = None,
@@ -214,32 +219,33 @@
     # Counter for index
     i = 1
     # Create a new dataframe for the extracted metrics
     df_to_save_to = pd.DataFrame()
 
     for filename in os.listdir(input_csv_directory):
         # Print progress
-        print(f'Progress: {i}/{len(os.listdir(input_csv_directory))},'
-              f' Extracting from: {filename}')
+        print(
+            f'Progress: {i}/{len(os.listdir(input_csv_directory))},'
+            f' Extracting from: {filename}',
+        )
 
         # Pandas read csv
         read_df_csv = pd.read_csv(input_csv_directory + filename, sep=';')
         # Set original filename
         original_filename = None
         # If filetype is not unknown, set original filename
         if filetype is not filetype.UNKNOWN:
             if filetype == filetype.GPX:
-                original_filename=filename.replace('.csv','.gpx')
+                original_filename = filename.replace('.csv', '.gpx')
             elif filetype == filetype.TCX:
-                original_filename=filename.replace('.csv','.tcx')
-
+                original_filename = filename.replace('.csv', '.tcx')
 
         # Extract data from a single GPX/TCX file, add filename and index
         row_to_append = extract_single_sportfile_metrics_to_csv(
-            read_df_csv = read_df_csv,
+            read_df_csv=read_df_csv,
             sportfile_directory=sportfile_directory,
             original_filename=original_filename,
             index=i,
         )
 
         # Pandas concat dictionary to empty dataframe
         row_to_append = pd.DataFrame([row_to_append]).round(2)
```

### Comparing `sportydatagen-0.2.1/sportydatagen/return_random_data.py` & `sportydatagen-0.2.2/sportydatagen/return_random_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Return random data from extracted features."""
 import pandas as pd
 
 
 def return_number_random_data(
-        filepath: str,
-        random_size: int,
-        random_state: int = 1,
+    filepath: str,
+    random_size: int,
+    random_state: int = 1,
 ) -> pd.DataFrame:
     """Return a number of random data from extracted features.
 
     Args:
-    ----------------
+    ----
     filepath (str): Path where the extracted features are stored.
     random_size (int): Number of random data to return.
     random_state (int): Random state for reproducibility.
 
     Returns:
-    ----------------
+    -------
     pd.DataFrame: Random data from extracted features.
     """
     # Pandas read csv
     read_df_tcx_csv = pd.read_csv(
         filepath_or_buffer=filepath,
         sep=';',
         index_col='index',
@@ -31,28 +31,28 @@
         error_message = 'random_size is larger than nO. of rows in .csv'
         raise ValueError(error_message)
 
     return read_df_tcx_csv.sample(n=random_size, random_state=random_state)
 
 
 def return_percent_random_data(
-        filepath: str,
-        random_percent: float,
-        random_state: int = 1,
+    filepath: str,
+    random_percent: float,
+    random_state: int = 1,
 ) -> pd.DataFrame:
     """Return a percent of random data from extracted features.
 
     Args:
-    ----------------
+    ----
     filepath (str): Path where the extracted features are stored.
     random_percent (float): Percent of random data to return.
     random_state (int): Random state for reproducibility.
 
     Returns:
-    ----------------
+    -------
     pd.DataFrame: Random data from extracted features.
     """
     # Pandas read csv
     read_df_tcx_csv = pd.read_csv(
         filepath_or_buffer=filepath,
         sep=';',
         index_col='index',
@@ -66,49 +66,49 @@
     return read_df_tcx_csv.sample(
         frac=random_percent,
         random_state=random_state,
     )
 
 
 def return_condition_random_data(
-        filepath: str,
-        random_size: int = 10,
-        random_state: int = 1,
-        activity_type: str = 'any',
-        min_total_distance: float = 0,
-        max_total_distance: float = 999999,
-        min_duration: float = 0,
-        max_duration: float = 99999,
-        min_calories: float = 0,
-        max_calories: float = 99999,
-        min_hr_avg: float = 0,
-        max_hr_avg: float = 999,
-        min_hr_min: float = 0,
-        max_hr_min: float = 999,
-        min_hr_max: float = 0,
-        max_hr_max: float = 999,
-        min_altitude_avg: float = 0,
-        max_altitude_avg: float = 9999,
-        min_altitude_min: float = 0,
-        max_altitude_min: float = 9999,
-        min_altitude_max: float = 0,
-        max_altitude_max: float = 9999,
-        min_ascent: float = 0,
-        max_ascent: float = 99999,
-        min_descent: float = 0,
-        max_descent: float = 99999,
-        min_speed_max: float = 0,
-        max_speed_max: float = 9999,
-        min_speed_avg: float = 0,
-        max_speed_avg: float = 9999,
+    filepath: str,
+    random_size: int = 10,
+    random_state: int = 1,
+    activity_type: str = 'any',
+    min_total_distance: float = 0,
+    max_total_distance: float = 999999,
+    min_duration: float = 0,
+    max_duration: float = 99999,
+    min_calories: float = 0,
+    max_calories: float = 99999,
+    min_hr_avg: float = 0,
+    max_hr_avg: float = 999,
+    min_hr_min: float = 0,
+    max_hr_min: float = 999,
+    min_hr_max: float = 0,
+    max_hr_max: float = 999,
+    min_altitude_avg: float = 0,
+    max_altitude_avg: float = 9999,
+    min_altitude_min: float = 0,
+    max_altitude_min: float = 9999,
+    min_altitude_max: float = 0,
+    max_altitude_max: float = 9999,
+    min_ascent: float = 0,
+    max_ascent: float = 99999,
+    min_descent: float = 0,
+    max_descent: float = 99999,
+    min_speed_max: float = 0,
+    max_speed_max: float = 9999,
+    min_speed_avg: float = 0,
+    max_speed_avg: float = 9999,
 ) -> pd.DataFrame:
     """Return a number of rows based on conditions.
 
     Args:
-    ----------------
+    ----
     filepath (str): Path where the extracted features are stored.
     random_size (int): Number of random data to return.
     random_state (int): Random state for reproducibility.
     activity_type (str): Activity type to return.
     min_total_distance (float): Minimum total distance in column to return.
     max_total_distance (float): Maximum total distance in column to return.
     min_duration (float): Minimum duration in column to return.
@@ -133,38 +133,42 @@
     max_descent (float): Maximum descent in column to return.
     min_speed_max (float): Minimum maximum speed in column to return.
     max_speed_max (float): Maximum maximum speed in column to return.
     min_speed_avg (float): Minimum average speed in column to return.
     max_speed_avg (float): Maximum average speed in column to return.
 
     Returns:
-    ----------------
+    -------
     pd.DataFrame: Random data from extracted features.
     """
     # Pandas read csv
     read_df_tcx_csv = pd.read_csv(
         filepath_or_buffer=filepath,
         sep=';',
         index_col='index',
     )
 
     filters = [
-        read_df_tcx_csv['total_distance'].between(min_total_distance,
-                                                  max_total_distance),
+        read_df_tcx_csv['total_distance'].between(
+            min_total_distance, max_total_distance,
+        ),
         read_df_tcx_csv['duration'].between(min_duration, max_duration),
         read_df_tcx_csv['calories'].between(min_calories, max_calories),
         read_df_tcx_csv['hr_avg'].between(min_hr_avg, max_hr_avg),
         read_df_tcx_csv['hr_min'].between(min_hr_min, max_hr_min),
         read_df_tcx_csv['hr_max'].between(min_hr_max, max_hr_max),
-        read_df_tcx_csv['altitude_avg'].between(min_altitude_avg,
-                                                max_altitude_avg),
-        read_df_tcx_csv['altitude_min'].between(min_altitude_min,
-                                                max_altitude_min),
-        read_df_tcx_csv['altitude_max'].between(min_altitude_max,
-                                                max_altitude_max),
+        read_df_tcx_csv['altitude_avg'].between(
+            min_altitude_avg, max_altitude_avg,
+        ),
+        read_df_tcx_csv['altitude_min'].between(
+            min_altitude_min, max_altitude_min,
+        ),
+        read_df_tcx_csv['altitude_max'].between(
+            min_altitude_max, max_altitude_max,
+        ),
         read_df_tcx_csv['ascent'].between(min_ascent, max_ascent),
         read_df_tcx_csv['descent'].between(min_descent, max_descent),
         read_df_tcx_csv['speed_max'].between(min_speed_max, max_speed_max),
         read_df_tcx_csv['speed_avg'].between(min_speed_avg, max_speed_avg),
     ]
 
     # Check conditions
@@ -172,43 +176,45 @@
         filters.append(read_df_tcx_csv['activity_type'] == activity_type)
 
     for f in filters:
         read_df_tcx_csv = read_df_tcx_csv.loc[f]
 
     # Try to return condition based data
     try:
-        return read_df_tcx_csv.sample(
-            n=random_size,
-            random_state=random_state)
+        return read_df_tcx_csv.sample(n=random_size, random_state=random_state)
     except ValueError:
-        error_message = (f'Not enough data left to return {random_size} '
-                         f'random data. Ease the conditions.')
+        error_message = (
+            f'Not enough data left to return {random_size} '
+            f'random data. Ease the conditions.'
+        )
         raise ValueError from ValueError(error_message)
 
 
 def filter_returned_columns(
-        columns_to_return: list,
-        df_to_filter: pd.DataFrame,
+    columns_to_return: list,
+    df_to_filter: pd.DataFrame,
 ) -> pd.DataFrame:
     """Filter returned columns and their order.
 
     Args:
-    ----------------
+    ----
     columns_to_return (list): Specific columns to return.
     df_to_filter (pd.DataFrame): Any dataframe.
 
     Returns:
-    ----------------
+    -------
     pd.DataFrame: Random data from extracted features.
     """
     all_possible_columns = df_to_filter.columns
 
     # Check if columns to return are in dataframe
     error_cols = list(set(columns_to_return) - set(all_possible_columns))
     if error_cols:
         # Raise error if columns are not in dataframe
         # and show possible columns
-        error_message = (f'Columns {error_cols} not found in dataframe. '
-                         f'Possible columns are {all_possible_columns}.')
+        error_message = (
+            f'Columns {error_cols} not found in dataframe. '
+            f'Possible columns are {all_possible_columns}.'
+        )
         raise ValueError(error_message)
 
     return df_to_filter[columns_to_return]
```

### Comparing `sportydatagen-0.2.1/sportydatagen/saf_extract_features_to_csv.py` & `sportydatagen-0.2.2/sportydatagen/saf_extract_features_to_csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import pandas as pd
 from sport_activities_features import GPXFile, TCXFile
 
 from sportydatagen.convert_to_csv import check_file_type
 
 
 def saf_extract_metrics_convert_to_csv(
-        sportfile_directory: str,
-        output_file: str,
+    sportfile_directory: str,
+    output_file: str,
 ) -> None:
     """Convert TCX/GPX files to CSV file using sports-activities-features."""
     # Create a new dataframe for the extracted metrics
     df_to_save_to = pd.DataFrame(
         columns=[
             'index',
             'filename',
@@ -42,15 +42,14 @@
     # Remove first row beacuse it is empty
     df_to_save_to = df_to_save_to.drop(df_to_save_to.index[0])
 
     # Extract data from a single TCX file using sports_activities_features
     TCXFile()
     GPXFile()
 
-
     for filename in os.listdir(sportfile_directory):
         """Extract metrics from sportfile file using sports_activities_features
         :return: pd.DataFrame with metrics"""
 
         # Print progress
         print(filename)
 
@@ -81,18 +80,18 @@
         Path(output_file),
         sep=';',
         na_rep='NULL',
         index=False,
     )
     # Drop rows with any null values, ignore activity_type column
     df_to_save_to = df_to_save_to.dropna(
-            subset=df_to_save_to.columns.difference(['activity_type',
-                                                     'steps']),
-            how='any',
-            axis=0)
+        subset=df_to_save_to.columns.difference(['activity_type', 'steps']),
+        how='any',
+        axis=0,
+    )
     # Replace output file with no null values
     output_file = output_file.replace('.csv', '_no_null.csv')
     # Save new csv with no null values
     df_to_save_to.to_csv(
         Path(output_file),
         sep=';',
         na_rep='NULL',
```

### Comparing `sportydatagen-0.2.1/sportydatagen/utils.py` & `sportydatagen-0.2.2/sportydatagen/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,42 +16,51 @@
         reader = csv.reader(file, delimiter=',')
         # Reset file pointer to beginning.
         file.seek(0)
         if has_header:
             # Skip header row.
             next(reader)
         for activity in reader:
-            dataset.append(Activity(activity[4],
-                                    float(activity[2]),
-                                    float(activity[1]),
-                                    float(activity[3])))
+            dataset.append(
+                Activity(
+                    activity[4],
+                    float(activity[2]),
+                    float(activity[1]),
+                    float(activity[3]),
+                ),
+            )
         return dataset
 
+
 def read_dataset(filename: str) -> list:
     """Read full dataset from a csv file."""
     dataset = []
     with Path.open(Path(filename)) as file:
         # Check if file has header.
         has_header = csv.Sniffer().has_header(file.read(4096))
-        reader = csv.reader(file,  delimiter=';')
+        reader = csv.reader(file, delimiter=';')
         # Reset file pointer to beginning.
         file.seek(0)
         if has_header:
             # Skip header row.
             next(reader)
         for activity in reader:
-            dataset.append(Activity(activity_type = activity[1], # string
-                                    distance = float(activity[2]), # float
-                                    duration = float(activity[3]), # float
-                                    calories = float(activity[4]), # float
-                                    hr_avg = float(activity[5]), # float
-                                    hr_min = float(activity[6]), # float
-                                    hr_max = float(activity[7]), # float
-                                    altitude_avg = float(activity[8]), # float
-                                    altitude_min = float(activity[9]), # float
-                                    altitude_max = float(activity[10]), # float
-                                    ascent = float(activity[11]), # float
-                                    descent = float(activity[12]), # float
-                                    speed_max = float(activity[13]), # float
-                                    speed_avg = float(activity[14]), # float
-                                    file_name = activity[15])) # string
+            dataset.append(
+                Activity(
+                    activity_type=activity[1],  # string
+                    distance=float(activity[2]),  # float
+                    duration=float(activity[3]),  # float
+                    calories=float(activity[4]),  # float
+                    hr_avg=float(activity[5]),  # float
+                    hr_min=float(activity[6]),  # float
+                    hr_max=float(activity[7]),  # float
+                    altitude_avg=float(activity[8]),  # float
+                    altitude_min=float(activity[9]),  # float
+                    altitude_max=float(activity[10]),  # float
+                    ascent=float(activity[11]),  # float
+                    descent=float(activity[12]),  # float
+                    speed_max=float(activity[13]),  # float
+                    speed_avg=float(activity[14]),  # float
+                    file_name=activity[15],
+                ),
+            )  # string
         return dataset
```

### Comparing `sportydatagen-0.2.1/setup.py` & `sportydatagen-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['sportydatagen']
+['sportydatagen', 'sportydatagen.cluster', 'sportydatagen.plot']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['niapy>=2.0.5,<3.0.0',
  'numpy>=1.24.2,<2.0.0',
  'pandas',
+ 'scikit-learn>=1.2.2,<2.0.0',
  'sport-activities-features>=0.3.12,<0.4.0']
 
 setup_kwargs = {
     'name': 'sportydatagen',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Sports activity generator module',
     'long_description': '# SportyDataGen -- Generator of Endurance Sports Activity Collections (datasets)\n\n## About\n\nSportyDataGen Library is a Python library designed to work with sport GPX and TCX files. It allows users to easily convert these file types into CSV format, extract feature data, and return random data based on specified conditions.\n\nIt aims to help researchers to create datasets for machine learning and data mining applications.\n\n## Features\n* Conversion of GPX and TCX files to CSV format\n* Extraction of feature data from sport files, including GPS coordinates, ascent, heart rate, distance and more\n* Merge of multiple csv files into a single dataset\n* Random selection of data based on the number of rows, percentage of rows in a file or custom conditions\n* Integration with Python scripts to provide an efficient data processing pipeline\n\n## Reference Papers:\n\nIdeas are based on the following research papers:\n\n[1] Fister, I., Jr.; Vrbančič, G.; Brezočnik, L.; Podgorelec, V.; Fister, I. [SportyDataGen: An Online Generator of Endurance Sports Activity Collections](https://www.iztok-jr-fister.eu/static/publications/225.pdf). In Proceedings of the Central European Conference on Information and Intelligent Systems, Varaždin, Croatia, 19–21 September 2018; pp. 171–178.\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n',
     'author': 'Rok Kukovec',
     'author_email': 'rok.kukovec1@student.um.si',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/firefly-cpp/sportydatagen',
```

### Comparing `sportydatagen-0.2.1/PKG-INFO` & `sportydatagen-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sportydatagen
-Version: 0.2.1
+Version: 0.2.2
 Summary: Sports activity generator module
 Home-page: https://gitlab.com/firefly-cpp/sportydatagen
 License: MIT
 Keywords: artificial sport trainer,computational intelligence,data mining,sport activities,tcx
 Author: Rok Kukovec
 Author-email: rok.kukovec1@student.um.si
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: niapy (>=2.0.5,<3.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: sport-activities-features (>=0.3.12,<0.4.0)
 Project-URL: Repository, https://gitlab.com/firefly-cpp/sportydatagen
 Description-Content-Type: text/markdown
 
 # SportyDataGen -- Generator of Endurance Sports Activity Collections (datasets)
 
 ## About
```

