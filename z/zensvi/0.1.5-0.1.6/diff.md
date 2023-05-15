# Comparing `tmp/zensvi-0.1.5.tar.gz` & `tmp/zensvi-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.1.5.tar", max compression
+gzip compressed data, was "zensvi-0.1.6.tar", max compression
```

## Comparing `zensvi-0.1.5.tar` & `zensvi-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.1.5/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.1.5/README.md
--rwxr-xr-x   0        0        0      694 2023-05-14 13:26:50.320956 zensvi-0.1.5/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.1.5/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.1.5/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.1.5/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    38123 2023-05-14 01:59:06.770688 zensvi-0.1.5/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       55 2023-05-14 01:59:06.771355 zensvi-0.1.5/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    14464 2023-05-14 13:02:40.359162 zensvi-0.1.5/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.1.5/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.1.5/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8291 2023-05-14 13:25:54.052907 zensvi-0.1.5/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.1.5/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.1.5/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     8149 2023-05-14 12:56:31.947970 zensvi-0.1.5/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.1.5/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.1.5/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.1.5/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.1.5/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.1.6/README.md
+-rwxr-xr-x   0        0        0      694 2023-05-15 13:48:54.949007 zensvi-0.1.6/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.1.6/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.1.6/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.1.6/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    39332 2023-05-15 13:48:37.483726 zensvi-0.1.6/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       55 2023-05-14 01:59:06.771355 zensvi-0.1.6/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    20153 2023-05-15 13:48:37.484588 zensvi-0.1.6/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.1.6/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.1.6/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8291 2023-05-14 13:25:54.052907 zensvi-0.1.6/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.1.6/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.1.6/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.1.6/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.1.6/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.1.6/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.1.6/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.1.6/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.1.6/PKG-INFO
```

### Comparing `zensvi-0.1.5/LICENSE` & `zensvi-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.5/README.md` & `zensvi-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.5/pyproject.toml` & `zensvi-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.1.5"
+version = "0.1.6"
 description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zensvi-0.1.5/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.1.6/src/zensvi/cv/segmentation/segmentation.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from transformers import OneFormerProcessor, OneFormerForUniversalSegmentation
 from transformers import AutoImageProcessor, Mask2FormerForUniversalSegmentation
 import os
 from tqdm.auto import tqdm
 import json
 from collections import defaultdict
 from tqdm.contrib.concurrent import thread_map
-
+import glob
+import shutil
 
 # a label and all meta information
 Label = namedtuple( 'Label' , [
 
             'name'        , # The identifier of this label, e.g. 'car', 'person', ... .
                             # We use them to uniquely name a class
 
@@ -206,24 +207,23 @@
     return (height, width)
 
 class ImageDataset(Dataset):
     """
     Custom Dataset class for images.
     """
 
-    def __init__(self, dir_input: Union[str, Path], rgb: bool = True) -> None:
+    def __init__(self, image_files: List[Path], rgb: bool = True) -> None:
         """
         Initialize the ImageDataset.
 
         Args:
-            dir_input (Union[str, Path]): Input directory containing image files.
+            image_files (List[Path]): List of image files.
             rgb (bool, optional): Flag to convert images to RGB. Defaults to True.
         """
-        self.dir_input = Path(dir_input)
-        self.image_files = list(self.dir_input.glob("*.jpg"))
+        self.image_files = image_files
         self.rgb = rgb
 
     def __len__(self) -> int:
         """
         Get the length of the dataset.
 
         Returns:
@@ -513,75 +513,103 @@
         if task == "panoptic":
             outputs = self._panoptic_segmentation(images, original_img_shape)
         elif task == "semantic":
             outputs, pixel_ratios = self._semantic_segmentation(images, original_img_shape)
 
         if outputs is not None:
             for image_file, img, output, pixel_ratio in zip(image_files, images, outputs, pixel_ratios):
-                if len(self.save_image_options) > 0:
+                if (len(self.save_image_options) > 0) & (dir_output is not None):
                     self._save_segmentation_image(task, image_file, img, dir_output, output)
                 image_file_key = Path(image_file).stem
                 pixel_ratio_dict[image_file_key] = pixel_ratio
 
     # Modify the segment method inside the Segmenter class
-    def segment(self, dir_input: Union[str, Path], dir_image_output: Union[str, Path, None] = None, dir_pixel_ratio_output: Union[str, Path, None] = None, task="semantic", batch_size=1, num_workers=1, save_image_options = ["segmented_image", "blend_image"], pixel_ratio_save_format = ["json", "csv"]):
-        """
-        Perform segmentation on the input images and save the segmented images.
-
-        Args:
-            dir_input (Union[str, Path]): The directory containing the input images.
-            dir_image_output (Union[str, Path , None]): The output directory where the segmented images will be saved. Default is None.
-            dir_pixel_ratio_output (Union[str, Path, None]): The output directory where the pixel ratio data will be saved. Default is None.
-            task (str): The segmentation task to perform, either "panoptic" or "semantic". Default is "semantic".
-            batch_size (int): The batch size to use for segmentation. Default is 1.
-            num_workers (int): The number of worker threads to use for segmentation. Default is 0.
-            save_image_options (List[str]): A list of options for saving the segmented images. Possible options are "segmented_image" and "blend_image". Default is ["segmented_image", "blend_image"].
-            pixel_ratio_save_format (List[str]): A list of output formats for the pixel ratio data. Possible options are "json" and "csv". Default is ["json", "csv"].
-
-        Returns:
-            None
-        """
+    def segment(self, dir_input: Union[str, Path], dir_image_output: Union[str, Path, None] = None, dir_pixel_ratio_output: Union[str, Path, None] = None, task="semantic", batch_size=1, save_image_options = ["segmented_image", "blend_image"], pixel_ratio_save_format = ["json", "csv"]):
         # make sure that at least one of dir_image_output and dir_pixel_ratio_output is not None
-        if dir_image_output is None and dir_pixel_ratio_output is None:
+        if (dir_image_output is None) & (dir_pixel_ratio_output is None):
             raise ValueError("At least one of dir_image_output and dir_pixel_ratio_output must not be None.")
         
         # save_image_options as a property of the class
         self.save_image_options = save_image_options
         
         # make directory
         dir_input = Path(dir_input)
-        dir_image_output = Path(dir_image_output)
-        dir_image_output.mkdir(parents=True, exist_ok=True)
-        dir_pixel_ratio_output = Path(dir_pixel_ratio_output)
-        dir_pixel_ratio_output.mkdir(parents=True, exist_ok=True)
-
-        dataset = ImageDataset(dir_input)
-        dataloader = DataLoader(dataset, batch_size=batch_size, collate_fn=dataset.collate_fn, num_workers=num_workers)
+        dir_cache_pixel_ratio = None
+        if dir_image_output is not None:
+            dir_image_output = Path(dir_image_output)
+            dir_image_output.mkdir(parents=True, exist_ok=True)
+        if dir_pixel_ratio_output is not None:
+            dir_pixel_ratio_output = Path(dir_pixel_ratio_output)
+            dir_pixel_ratio_output.mkdir(parents=True, exist_ok=True)
+            # Create a new directory called "pixel_ratio_checkpoints"
+            dir_cache_pixel_ratio = dir_pixel_ratio_output / 'pixel_ratio_checkpoints'
+            dir_cache_pixel_ratio.mkdir(parents=True, exist_ok=True)
+
+            # Load all the checkpoint json files
+            checkpoints = glob.glob(str(dir_cache_pixel_ratio / '*.json'))
+            checkpoint_start_index = len(checkpoints)
+
+            completed_image_files = set()  # completed_image_files will store the keys in the pixel_ratio_dict
+            if checkpoint_start_index > 0:
+                for checkpoint in checkpoints:
+                    with open(checkpoint, 'r') as f:
+                        checkpoint_dict = json.load(f)
+                        completed_image_files.update(checkpoint_dict.keys())
+
+        # Get the list of all image files and filter the ones that are not completed yet
+        image_files = [str(f) for f in Path(dir_input).glob("*.jpg") if str(f) not in completed_image_files]
+
+        outer_batch_size = 1000  # Number of inner batches in one outer batch
+        num_outer_batches = (len(image_files) + outer_batch_size * batch_size - 1) // (outer_batch_size * batch_size)
+
+        for i in tqdm(range(num_outer_batches), desc=f"Processing outer batches of size {min(outer_batch_size * batch_size, len(image_files))}"):
+            # Get the image files for the current outer batch
+            outer_batch_image_files = image_files[i * outer_batch_size * batch_size : (i+1) * outer_batch_size * batch_size]
+
+            dataset = ImageDataset(outer_batch_image_files)
+            dataloader = DataLoader(dataset, batch_size=batch_size, collate_fn=dataset.collate_fn)
+
+            pixel_ratio_dict = defaultdict(dict)  # reset pixel_ratio_dict for each outer batch
+
+            with ThreadPoolExecutor() as executor:
+                futures = []
+
+                for batch in dataloader:
+                    image_files, images, original_img_shape = batch
+                    future = executor.submit(self._process_images, task, image_files, images, dir_image_output, pixel_ratio_dict, original_img_shape)
+                    futures.append(future)
+
+                for completed_future in tqdm(as_completed(futures), total=len(futures), desc=f"Processing outer batch #{i+1}"):
+                    completed_future.result()
+
+                # Save checkpoint for each outer batch
+                with open(f'{dir_cache_pixel_ratio}/checkpoint_batch_{checkpoint_start_index+i+1}.json', 'w') as f:
+                    json.dump(pixel_ratio_dict, f)
 
+        # Merge all checkpoints into a single pixel_ratio_dict
         pixel_ratio_dict = defaultdict(dict)
-
-        with ThreadPoolExecutor(max_workers=num_workers) as executor:
-            futures = []
-
-            for batch in tqdm(dataloader, desc="Submitting tasks"):
-                image_files, images, original_img_shape = batch
-                future = executor.submit(self._process_images, task, image_files, images, dir_image_output, pixel_ratio_dict, original_img_shape)
-                futures.append(future)
-
-            for completed_future in tqdm(as_completed(futures), total=len(futures), desc="Processing tasks"):
-                completed_future.result()
+        for checkpoint in glob.glob(str(dir_cache_pixel_ratio / '*.json')):
+            with open(checkpoint, 'r') as f:
+                checkpoint_dict = json.load(f)
+                for key, value in checkpoint_dict.items():
+                    pixel_ratio_dict[key] = value
 
         # Save pixel_ratio_dict as a JSON or CSV file
         if "json" in pixel_ratio_save_format:
             with open(dir_pixel_ratio_output / "pixel_ratios.json", "w") as f:
                 json.dump(pixel_ratio_dict, f)
         if "csv" in pixel_ratio_save_format:
             self._save_pixel_ratios_as_csv(pixel_ratio_dict, dir_pixel_ratio_output)
             
-    def calculate_pixel_ratio_post_process(self, dir_input, dir_output, pixel_ratio_save_format = ["json", "csv"], num_workers=1):
+        # Delete the "pixel_ratio_checkpoints" directory
+        if dir_pixel_ratio_output is not None:
+            shutil.rmtree(dir_cache_pixel_ratio)
+
+            
+    def calculate_pixel_ratio_post_process(self, dir_input, dir_output, pixel_ratio_save_format = ["json", "csv"]):
         """
         Calculates the pixel ratio of different classes present in the segmented images and saves the results in either JSON or CSV format.
 
         Args:
             dir_input: A string or Path object representing the input directory containing the segmented images.
             dir_output: A string or Path object representing the output directory where the pixel ratio results will be saved.
             pixel_ratio_save_format: A list containing the file formats in which the results will be saved. The allowed file formats are "json" and "csv". The default value is ["json", "csv"].
@@ -670,15 +698,15 @@
             dir_input = Path(dir_input)
 
         # Set image file extensions
         image_extensions = ['.jpg', '.png']
 
         image_files = [file for file in dir_input.rglob('*') if file.suffix.lower() in image_extensions and '_colored_segmented' in file.stem]
 
-        results = thread_map(process_image_file, image_files, [self.label_map] * len(image_files), max_workers=num_workers)
+        results = thread_map(process_image_file, image_files, [self.label_map] * len(image_files))
 
         if "json" in pixel_ratio_save_format:
             json_output_file = Path(dir_output) / 'pixel_ratio.json'
             nested_dict = results_to_nested_dict(results)
             with open(json_output_file, 'w') as f:
                 json.dump(nested_dict, f, indent=2)
```

### Comparing `zensvi-0.1.5/src/zensvi/download/streetview_downloader.py` & `zensvi-0.1.6/src/zensvi/download/streetview_downloader.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 from pathlib import Path
 import geopandas as gpd
 from tqdm import tqdm
 from shapely.geometry import Point
 import warnings
 from shapely.errors import ShapelyDeprecationWarning
 warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
-import csv 
+import csv
+import glob
+import shutil
 
 from zensvi.download.utils.imtool import ImageTool
 from zensvi.download.utils.get_pids import panoids
 from zensvi.download.utils.geoprocess import GeoProcessor
 from zensvi.download.utils.helpers import standardize_column_names, create_buffer_gdf
 
 class StreetViewDownloader:
@@ -110,39 +112,60 @@
     def _read_pids(self, path_pid):
         pid_df = pd.read_csv(path_pid)
         # get unique pids as a list
         pids = pid_df.iloc[:,0].unique().tolist()
         return pids
 
     def _check_already(self, all_panoids):
-        name_r, all_panoids_f = set(), []
-        for name in os.listdir(self.dir_output):
-            name_r.add(name.split(".")[0])
-
-        for pid in all_panoids:
-            if pid not in name_r:
-                all_panoids_f.append(pid)
-        return all_panoids_f
+        # Get the list of already downloaded images
+        name_r = set(name.split(".")[0] for name in os.listdir(self.panorama_output))
+
+        # Filter the list of all panoids to only include those not already downloaded
+        all_panoids[:] = [pid for pid in all_panoids if pid not in name_r]
+
+        return all_panoids
+
 
     def _log_write(self, pids):
         with open(self.log_path, 'a+') as fw:
             for pid in pids:
                 fw.write(pid+'\n')
     
     def _augment_metadata(self, df):
+        if self.cache_pids_augmented.exists():
+            df = pd.read_csv(self.cache_pids_augmented)
+            print("The augmented panorama IDs have been read from the cache")
+            return df
+        
+        # Create a new directory called "augmented_metadata_checkpoints"
+        dir_cache_augmented_metadata = self.dir_cache / 'augmented_pids'
+        dir_cache_augmented_metadata.mkdir(parents=True, exist_ok=True)
+
+        # Load all the checkpoint csv files
+        checkpoints = glob.glob(str(dir_cache_augmented_metadata / '*.csv'))
+        checkpoint_start_index = len(checkpoints)
+
+        if checkpoint_start_index > 0:
+            completed_rows = pd.concat([pd.read_csv(checkpoint) for checkpoint in checkpoints], ignore_index=True)
+            completed_indices = completed_rows.index.unique()
+
+            # Filter df to get remaining indices to augment metadata for
+            df = df.loc[~df.index.isin(completed_indices)]
+
         def get_year_month(pid, proxies):
             url = "https://maps.googleapis.com/maps/api/streetview/metadata?pano={}&key={}".format(pid, self.gsv_api_key)
             while True:
                 proxy = random.choice(proxies)
                 try:
                     response = requests.get(url, proxies=proxy, timeout=5)
                     break
                 except Exception as e:
                     print(f"Proxy {proxy} is not working. Exception: {e}")
                     continue
+
             response = response.json()
             if response['status'] == 'OK':
                 # get year and month from date
                 try:
                     date = response['date']
                     year = date.split("-")[0]
                     month = date.split("-")[1]
@@ -152,28 +175,64 @@
                 return {"year": year, "month": month}
             return {"year": None, "month": None}    
 
         def worker(row, proxies):
             panoid = row.panoid
             year_month = get_year_month(panoid, proxies)
             return row.Index, year_month
-        
+
         batch_size = 1000  # Modify this to a suitable value
         num_batches = (len(df) + batch_size - 1) // batch_size
 
         for i in tqdm(range(num_batches), desc=f"Augmenting metadata by batch size {min(batch_size, len(df))}"):
+            batch_df = df.iloc[i*batch_size : (i+1)*batch_size].copy()  # Copy the batch data to a new dataframe
             with ThreadPoolExecutor() as executor:
-                batch_futures = {executor.submit(worker, row, self.proxies): row.Index for row in df.iloc[i*batch_size : (i+1)*batch_size].itertuples()}
+                batch_futures = {executor.submit(worker, row, self.proxies): row.Index for row in batch_df.itertuples()}
                 for future in tqdm(as_completed(batch_futures), total=len(batch_futures), desc=f"Augmenting metadata for batch #{i+1}"):
                     row_index, year_month = future.result()
-                    df.at[row_index, 'year'] = year_month['year']
-                    df.at[row_index, 'month'] = year_month['month']
+                    batch_df.at[row_index, 'year'] = year_month['year']
+                    batch_df.at[row_index, 'month'] = year_month['month']
+
+            # Save checkpoint for each batch
+            batch_df.to_csv(f'{dir_cache_augmented_metadata}/checkpoint_batch_{checkpoint_start_index+i+1}.csv', index=False)
+        
+        # Merge all checkpoints into a single dataframe
+        df = pd.concat([pd.read_csv(checkpoint) for checkpoint in glob.glob(str(dir_cache_augmented_metadata / '*.csv'))], ignore_index=True)
+
+        # save the augmented metadata
+        df.to_csv(self.cache_pids_augmented, index=False)
+        # delete cache_lat_lon
+        self.cache_lat_lon.unlink() 
+        # delete cache_pids_raw
+        self.cache_pids_raw.unlink()
+        # delete the cache directory
+        if dir_cache_augmented_metadata.exists():
+            shutil.rmtree(dir_cache_augmented_metadata)
         return df
-                    
-    def _get_pids_from_csv(self, df, id_columns, closest=False, disp=False):
+
+    def _get_pids_from_csv(self, df, id_columns=None, closest=False, disp=False):
+        # 1. Create a new directory called "pids" to store each batch pids
+        dir_cache_pids = self.dir_cache / 'raw_pids'
+        dir_cache_pids.mkdir(parents=True, exist_ok=True)
+
+        # 2. Load all the checkpoint csv files
+        checkpoints = glob.glob(str(dir_cache_pids / '*.csv'))
+        checkpoint_start_index = len(checkpoints)
+        if checkpoint_start_index > 0:
+            completed_rows = pd.concat([pd.read_csv(checkpoint) for checkpoint in checkpoints], ignore_index=True)
+
+            if id_columns is None:
+                # Use 'longitude' and 'latitude' columns to filter rows if id_columns is None
+                id_columns = ['longitude', 'latitude']
+
+            completed_ids = completed_rows[id_columns].drop_duplicates()
+
+            # Filter df to get remaining lat lon to get pids for
+            df = df[~df[id_columns].isin(completed_ids).all(axis=1)]
+
         def get_street_view_info(longitude, latitude, proxies):
             results = panoids(latitude, longitude, proxies, closest=closest, disp=disp)
             return results
 
         def worker(row):
             input_longitude = row.longitude
             input_latitude = row.latitude
@@ -195,14 +254,21 @@
                             result['input_latitude'] = input_latitude
                             result.update(id_dict)
                             results.append(result)
                     except Exception as e:
                         print(f"Error: {e}")
                         failed_rows.append(batch_futures[future])  # Store the failed row
 
+                # Save checkpoint for each batch
+                pd.DataFrame(results).to_csv(f'{dir_cache_pids}/checkpoint_batch_{checkpoint_start_index+i+1}.csv', index=False)
+                results = []  # Clear the results list for the next batch
+
+        # Merge all checkpoints into a single dataframe
+        results_df = pd.concat([pd.read_csv(checkpoint) for checkpoint in glob.glob(str(dir_cache_pids / '*.csv'))], ignore_index=True)
+
         # Retry failed rows
         if failed_rows:
             print("Retrying failed rows...")
             with ThreadPoolExecutor() as executor:
                 retry_futures = {executor.submit(worker, row): row for row in failed_rows}
                 for future in tqdm(as_completed(retry_futures), total=len(retry_futures), desc="Retrying failed rows"):
                     try:
@@ -211,24 +277,46 @@
                             result['input_longitude'] = input_longitude
                             result['input_latitude'] = input_latitude
                             result.update(id_dict)
                             results.append(result)
                     except Exception as e:
                         print(f"Failed again: {e}")
 
-        results_df = pd.DataFrame(results)
+            # Save the results of retried rows as another checkpoint
+            pd.DataFrame(results).to_csv(f'{dir_cache_pids}/checkpoint_retry.csv', index=False)
+
+            # Merge the retry checkpoint into the final dataframe
+            retry_df = pd.read_csv(f'{dir_cache_pids}/checkpoint_retry.csv')
+            results_df = pd.concat([results_df, retry_df], ignore_index=True)
+
+        # now save results_df as a new cache
+        results_df.to_csv(self.cache_pids_raw, index=False)
+        
+        # delete the cache directory
+        if dir_cache_pids.exists():
+            shutil.rmtree(dir_cache_pids)
         return results_df
 
+
     def _get_pids_from_gdf(self, gdf, id_columns, closest=False, disp=False):  
-        # read shapefile
-        gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, id_columns = id_columns)
-        df = gp.get_lat_lon()
+        if self.cache_lat_lon.exists():
+            df = pd.read_csv(self.cache_lat_lon)
+            print("The lat and lon have been read from the cache")
+        else:
+            # read shapefile
+            gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, id_columns = id_columns)
+            df = gp.get_lat_lon()
+            # save df to cache
+            df.to_csv(self.cache_lat_lon, index=False)
 
-        # Use _get_pids_from_csv to get pids from df
-        results_df = self._get_pids_from_csv(df, id_columns, closest=closest, disp=disp)
+        if self.cache_pids_raw.exists():
+            results_df = pd.read_csv(self.cache_pids_raw)
+        else:
+            # Use _get_pids_from_csv to get pids from df
+            results_df = self._get_pids_from_csv(df, id_columns, closest=closest, disp=disp)
 
         # Check if lat and lon are within input polygons
         polygons = gpd.GeoSeries([geom for geom in gdf['geometry'] if geom.type in ['Polygon', 'MultiPolygon']])
 
         # Convert lat, lon to Points and create a GeoSeries
         points = gpd.GeoSeries([Point(lon, lat) for lon, lat in zip(results_df['lon'], results_df['lat'])])
 
@@ -276,15 +364,19 @@
             df = pd.read_csv(input_csv_file)
             df = standardize_column_names(df)
             if buffer > 0:
                 gdf = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df.longitude, df.latitude), crs='EPSG:4326')
                 gdf = create_buffer_gdf(gdf, buffer)
                 pid = self._get_pids_from_gdf(gdf, id_columns, closest=False, disp=False)
             else:
-                pid = self._get_pids_from_csv(df, id_columns, closest=False, disp=False)
+                if self.cache_pids_raw.exists():
+                    pid = pd.read_csv(self.cache_pids_raw)
+                    print("The raw panorama IDs have been read from the cache")
+                else:
+                    pid = self._get_pids_from_csv(df, id_columns, closest=False, disp=False)
         elif input_shp_file != "":
             gdf = gpd.read_file(input_shp_file)
             if buffer > 0:
                 gdf = create_buffer_gdf(gdf, buffer)
             pid = self._get_pids_from_gdf(gdf, id_columns, closest=False, disp=False)
         else:
             raise ValueError("Please input the lat and lon, csv file, or shapefile.")
@@ -292,47 +384,70 @@
         pid_df = pd.DataFrame(pid)
         pid_df = pid_df.drop_duplicates(subset='panoid')
         if augment_metadata & (self.gsv_api_key != None):
             pid_df = self._augment_metadata(pid_df)
         elif augment_metadata & (self.gsv_api_key == None):
             raise ValueError("Please set the gsv api key by calling the gsv_api_key method.")
         pid_df.to_csv(path_pid, index=False)
-        print("The panorama IDs have been saved to {}".format(path_pid))
-    
-    def download_gsv(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
-                lat=None, lon=None, input_csv_file="", input_shp_file = "", id_columns=None, buffer = 0, closest=False, disp=False, augment_metadata=False):
+        print("The panorama IDs have been saved to {}".format(path_pid)) 
+
+    def _set_dirs(self, dir_output):
         # set dir_output as attribute and create the directory
-        self.dir_output = dir_output
-        Path(dir_output).mkdir(parents=True, exist_ok=True)
+        self.dir_output = Path(dir_output)
+        self.dir_output.mkdir(parents=True, exist_ok=True)
+        # set dir_cache as attribute and create the directory
+        self.dir_cache = self.dir_output / "cache_zensvi"
+        self.dir_cache.mkdir(parents=True, exist_ok=True)
+        # set other cache directories
+        self.cache_lat_lon = self.dir_cache / "lat_lon.csv"
+        self.cache_pids_raw = self.dir_cache / "pids_raw.csv"
+        self.cache_pids_augmented = self.dir_cache / "pids_augemented.csv"
+        
+    def download_gsv(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
+                lat=None, lon=None, input_csv_file="", input_shp_file = "", id_columns=None, buffer = 0, closest=False, 
+                disp=False, augment_metadata=False, update_pids = False):
+        # set necessary directories
+        self._set_dirs(dir_output)
         
         # call get_pids function first if path_pid is None
-        if path_pid is None:
+        if (path_pid is None) & (self.cache_pids_augmented.exists() == False):
             print("Getting pids...")
-            path_pid = os.path.join(self.dir_output, "pids.csv")
-            self.get_pids(path_pid, lat=lat, lon=lon,
-                        input_csv_file=input_csv_file, input_shp_file = input_shp_file, id_columns=id_columns, buffer = buffer, closest=closest, disp=disp, augment_metadata=augment_metadata)
-
-
+            path_pid = self.dir_output / "pids.csv"
+            if path_pid.exists() & (update_pids == False):
+                print("update_pids is set to False. So the following csv file will be used: {}".format(path_pid))
+            else:
+                self.get_pids(path_pid, lat=lat, lon=lon,
+                            input_csv_file=input_csv_file, input_shp_file = input_shp_file, id_columns=id_columns, buffer = buffer, closest=closest, disp=disp, augment_metadata=augment_metadata)
+        elif self.cache_pids_augmented.exists():
+            # copy the cache pids_augmented to path_pid
+            path_pid = self.dir_output / "pids.csv"
+            shutil.copy2(self.cache_pids_augmented, path_pid)
+            print("The augmented panorama IDs have been saved to {}".format(path_pid))
         # Horizontal Google Street View tiles
         # zoom 3: (8, 4); zoom 5: (26, 13) zoom 2: (4, 2) zoom 1: (2, 1);4:(8,16)
         # zoom = 2
         # h_tiles = 4  # 26
         # v_tiles = 2  # 13
         # cropped = False
         # full = True
         # create a folder within self.dir_output
-        panorama_output = os.path.join(self.dir_output, "panorama")
-        os.makedirs(panorama_output, exist_ok=True)
+        self.panorama_output = self.dir_output / "panorama"
+        self.panorama_output.mkdir(parents=True, exist_ok=True)
         
         panoids = self._read_pids(path_pid)
-
+        
         if len(panoids) == 0:
-            print("There is no panorama ID to download.")
+            print("There is no panorama ID to download")
             return
         else:
             panoids_rest = self._check_already(panoids)
 
         if len(panoids_rest) > 0:
             UAs = random.choices(self.user_agent, k = len(panoids_rest))
-            ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, panorama_output, UAs, self.proxies, cropped, full, log_path=self.log_path)
+            ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, self.panorama_output, UAs, self.proxies, cropped, full, log_path=self.log_path)
         else:
-            print("All images have been downloaded.")
+            print("All images have been downloaded")
+        
+        # delete the cache directory
+        if self.dir_cache.exists():
+            shutil.rmtree(self.dir_cache)
+            print("The cache directory has been deleted")
```

### Comparing `zensvi-0.1.5/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.1.6/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.5/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.1.6/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.5/src/zensvi/download/utils/get_pids.py` & `zensvi-0.1.6/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.5/src/zensvi/download/utils/helpers.py` & `zensvi-0.1.6/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.5/src/zensvi/download/utils/imtool.py` & `zensvi-0.1.6/src/zensvi/download/utils/imtool.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,20 +130,21 @@
             h_c = int(h * 0.812)
             w_c = int(w * 0.812)
             if sun_i == 0:
                 pre_image = image[0:h_c, 0:w_c]
             else:
                 pre_image = image
             pillow_image = Image.fromarray(pre_image)
-            pillow_image.save(f'{name}.jpg')
-        # if cropped:
-        #     first_slice.crop((0, 0, size[1], size[1])).save(f'{name}_p1.jpg')
-        #     first_slice.crop((size[1], 0, size[0], size[1])).save(f'{name}_p2.jpg')
-        
-        return identif
+            # Validate image before saving
+            if pillow_image.size[0] > 0 and pillow_image.size[1] > 0:
+                pillow_image.save(f'{name}.jpg')
+            else:
+                raise ValueError(f"Invalid image for pano_id {pano_id}")
+
+            return identif
 
     @staticmethod
     def dwl_multiple(panoids, zoom, v_tiles, h_tiles, out_path, uas, proxies, cropped=True, full=False, log_path=None):
         """
         Description of dwl_multiple
         
         Calls the get_and_save_image function using multiple threads.
```

### Comparing `zensvi-0.1.5/src/zensvi/download/utils/proxies.csv` & `zensvi-0.1.6/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.5/src/zensvi/transform/transform_image.py` & `zensvi-0.1.6/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.5/PKG-INFO` & `zensvi-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.1.5
+Version: 0.1.6
 Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

