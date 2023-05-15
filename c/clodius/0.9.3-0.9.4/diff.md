# Comparing `tmp/clodius-0.9.3.tar.gz` & `tmp/clodius-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clodius-0.9.3.tar", last modified: Wed Jun 27 14:47:59 2018, max compression
+gzip compressed data, was "dist/clodius-0.9.4.tar", last modified: Thu Sep 27 13:40:54 2018, max compression
```

## Comparing `clodius-0.9.3.tar` & `clodius-0.9.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-06-27 14:47:59.000000 clodius-0.9.3/
--rw-r--r--   0 peter      (502) staff       (20)      225 2018-06-27 14:47:59.000000 clodius-0.9.3/PKG-INFO
-drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-06-27 14:47:59.000000 clodius-0.9.3/test/
--rw-r--r--   0 peter      (502) staff       (20)        0 2016-05-09 18:37:43.000000 clodius-0.9.3/test/__init__.py
--rw-r--r--   0 peter      (502) staff       (20)      584 2018-05-06 18:53:22.000000 clodius-0.9.3/test/tile_2d_bedfile_test.py
--rw-r--r--   0 peter      (502) staff       (20)     1037 2017-03-21 20:40:16.000000 clodius-0.9.3/test/utils.py
--rw-r--r--   0 peter      (502) staff       (20)       25 2016-12-15 20:17:34.000000 clodius-0.9.3/MANIFEST.in
--rw-r--r--   0 peter      (502) staff       (20)     2135 2018-06-27 14:47:56.000000 clodius-0.9.3/setup.py
-drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-06-27 14:47:59.000000 clodius-0.9.3/scripts/
--rw-r--r--   0 peter      (502) staff       (20)     3011 2017-03-21 20:40:25.000000 clodius-0.9.3/scripts/conversion_wrapper.py
--rw-r--r--   0 peter      (502) staff       (20)      533 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/make_big_file.py
--rw-r--r--   0 peter      (502) staff       (20)     5773 2017-03-21 20:40:16.000000 clodius-0.9.3/scripts/tile_1d.py
--rw-r--r--   0 peter      (502) staff       (20)     2241 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/make_streaming_tiles.py
--rw-r--r--   0 peter      (502) staff       (20)        0 2017-03-21 20:40:16.000000 clodius-0.9.3/scripts/__init__.py
--rw-r--r--   0 peter      (502) staff       (20)     4095 2018-06-15 20:10:09.000000 clodius-0.9.3/scripts/exonU.py
--rw-r--r--   0 peter      (502) staff       (20)    18376 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/make_single_threaded_tiles.py
--rw-r--r--   0 peter      (502) staff       (20)      256 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/temp.py
--rw-r--r--   0 peter      (502) staff       (20)     1203 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/get_hitile.py
--rw-r--r--   0 peter      (502) staff       (20)     5002 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/make_autocomplete_list.py
--rw-r--r--   0 peter      (502) staff       (20)      722 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/check_sorted.py
--rw-r--r--   0 peter      (502) staff       (20)      590 2017-03-21 20:40:16.000000 clodius-0.9.3/scripts/big_spark.py
--rw-r--r--   0 peter      (502) staff       (20)     8251 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/cooler_to_tiles.py
--rw-r--r--   0 peter      (502) staff       (20)     2597 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/process_file.py
--rw-r--r--   0 peter      (502) staff       (20)     1918 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/test_1d.py
--rw-r--r--   0 peter      (502) staff       (20)    10477 2016-12-15 20:17:34.000000 clodius-0.9.3/scripts/make_tiles.py
-drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-06-27 14:47:59.000000 clodius-0.9.3/clodius/
--rw-r--r--   0 peter      (502) staff       (20)    10169 2018-06-15 20:10:09.000000 clodius-0.9.3/clodius/multivec.py
--rw-r--r--   0 peter      (502) staff       (20)     6019 2018-05-06 18:53:22.000000 clodius-0.9.3/clodius/db_tiles.py
--rw-r--r--   0 peter      (502) staff       (20)      969 2018-02-14 21:12:00.000000 clodius-0.9.3/clodius/chromosomes.py
--rw-r--r--   0 peter      (502) staff       (20)     3768 2016-12-15 20:17:34.000000 clodius-0.9.3/clodius/higlass_getter.py
--rw-r--r--   0 peter      (502) staff       (20)     4129 2016-12-15 20:17:34.000000 clodius-0.9.3/clodius/fpark.py
--rw-r--r--   0 peter      (502) staff       (20)     7650 2017-10-06 13:46:07.000000 clodius-0.9.3/clodius/hdf_tiles.py
--rw-r--r--   0 peter      (502) staff       (20)    17819 2016-12-15 20:17:34.000000 clodius-0.9.3/clodius/tiles.py
--rw-r--r--   0 peter      (502) staff       (20)        0 2016-12-15 20:17:34.000000 clodius-0.9.3/clodius/__init__.py
-drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-06-27 14:47:59.000000 clodius-0.9.3/clodius/cli/
--rw-r--r--   0 peter      (502) staff       (20)    48438 2018-06-21 20:49:59.000000 clodius-0.9.3/clodius/cli/aggregate.py
--rw-r--r--   0 peter      (502) staff       (20)     7971 2018-06-15 20:10:09.000000 clodius-0.9.3/clodius/cli/convert.py
--rw-r--r--   0 peter      (502) staff       (20)      333 2018-05-06 18:53:22.000000 clodius-0.9.3/clodius/cli/__init__.py
--rw-r--r--   0 peter      (502) staff       (20)     1305 2018-05-06 18:53:22.000000 clodius-0.9.3/clodius/cli/utils.py
--rw-r--r--   0 peter      (502) staff       (20)   312218 2017-07-14 15:30:08.000000 clodius-0.9.3/clodius/fast.c
--rw-r--r--   0 peter      (502) staff       (20)    15458 2017-07-31 16:32:38.000000 clodius-0.9.3/clodius/save_tiles.py
--rw-r--r--   0 peter      (502) staff       (20)     1510 2017-07-13 20:58:54.000000 clodius-0.9.3/clodius/fast.pyx
--rw-r--r--   0 peter      (502) staff       (20)      856 2016-12-15 20:17:34.000000 clodius-0.9.3/clodius/describe_dataset.py
--rw-r--r--   0 peter      (502) staff       (20)       38 2018-06-27 14:47:59.000000 clodius-0.9.3/setup.cfg
-drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-06-27 14:47:59.000000 clodius-0.9.3/clodius.egg-info/
--rw-r--r--   0 peter      (502) staff       (20)      225 2018-06-27 14:47:58.000000 clodius-0.9.3/clodius.egg-info/PKG-INFO
--rw-r--r--   0 peter      (502) staff       (20)      997 2018-06-27 14:47:59.000000 clodius-0.9.3/clodius.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (502) staff       (20)       55 2018-06-27 14:47:58.000000 clodius-0.9.3/clodius.egg-info/entry_points.txt
--rw-r--r--   0 peter      (502) staff       (20)       82 2018-06-27 14:47:58.000000 clodius-0.9.3/clodius.egg-info/requires.txt
--rw-r--r--   0 peter      (502) staff       (20)        8 2018-06-27 14:47:59.000000 clodius-0.9.3/clodius.egg-info/top_level.txt
--rw-r--r--   0 peter      (502) staff       (20)        1 2018-06-27 14:47:58.000000 clodius-0.9.3/clodius.egg-info/dependency_links.txt
+drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-09-27 13:40:54.000000 clodius-0.9.4/
+-rw-r--r--   0 peter      (502) staff       (20)      225 2018-09-27 13:40:54.000000 clodius-0.9.4/PKG-INFO
+drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-09-27 13:40:54.000000 clodius-0.9.4/test/
+-rw-r--r--   0 peter      (502) staff       (20)        0 2016-05-09 18:37:43.000000 clodius-0.9.4/test/__init__.py
+-rw-r--r--   0 peter      (502) staff       (20)      584 2018-05-06 18:53:22.000000 clodius-0.9.4/test/tile_2d_bedfile_test.py
+-rw-r--r--   0 peter      (502) staff       (20)     1037 2017-03-21 20:40:16.000000 clodius-0.9.4/test/utils.py
+-rw-r--r--   0 peter      (502) staff       (20)       25 2016-12-15 20:17:34.000000 clodius-0.9.4/MANIFEST.in
+-rw-r--r--   0 peter      (502) staff       (20)     2139 2017-10-06 13:46:07.000000 clodius-0.9.4/README.md
+-rw-r--r--   0 peter      (502) staff       (20)      930 2018-09-27 13:40:40.000000 clodius-0.9.4/setup.py
+drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-09-27 13:40:54.000000 clodius-0.9.4/scripts/
+-rw-r--r--   0 peter      (502) staff       (20)     3011 2017-03-21 20:40:25.000000 clodius-0.9.4/scripts/conversion_wrapper.py
+-rw-r--r--   0 peter      (502) staff       (20)      533 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/make_big_file.py
+-rw-r--r--   0 peter      (502) staff       (20)     5773 2017-03-21 20:40:16.000000 clodius-0.9.4/scripts/tile_1d.py
+-rw-r--r--   0 peter      (502) staff       (20)     2241 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/make_streaming_tiles.py
+-rw-r--r--   0 peter      (502) staff       (20)        0 2017-03-21 20:40:16.000000 clodius-0.9.4/scripts/__init__.py
+-rw-r--r--   0 peter      (502) staff       (20)     4095 2018-06-15 20:10:09.000000 clodius-0.9.4/scripts/exonU.py
+-rw-r--r--   0 peter      (502) staff       (20)    18376 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/make_single_threaded_tiles.py
+-rw-r--r--   0 peter      (502) staff       (20)      256 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/temp.py
+-rw-r--r--   0 peter      (502) staff       (20)     1203 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/get_hitile.py
+-rw-r--r--   0 peter      (502) staff       (20)     5002 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/make_autocomplete_list.py
+-rw-r--r--   0 peter      (502) staff       (20)      722 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/check_sorted.py
+-rw-r--r--   0 peter      (502) staff       (20)      590 2017-03-21 20:40:16.000000 clodius-0.9.4/scripts/big_spark.py
+-rw-r--r--   0 peter      (502) staff       (20)     8251 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/cooler_to_tiles.py
+-rw-r--r--   0 peter      (502) staff       (20)     2597 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/process_file.py
+-rw-r--r--   0 peter      (502) staff       (20)     1918 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/test_1d.py
+-rw-r--r--   0 peter      (502) staff       (20)    10477 2016-12-15 20:17:34.000000 clodius-0.9.4/scripts/make_tiles.py
+drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-09-27 13:40:54.000000 clodius-0.9.4/clodius/
+-rw-r--r--   0 peter      (502) staff       (20)    10529 2018-06-27 17:04:00.000000 clodius-0.9.4/clodius/multivec.py
+-rw-r--r--   0 peter      (502) staff       (20)     6019 2018-05-06 18:53:22.000000 clodius-0.9.4/clodius/db_tiles.py
+-rw-r--r--   0 peter      (502) staff       (20)      969 2018-02-14 21:12:00.000000 clodius-0.9.4/clodius/chromosomes.py
+-rw-r--r--   0 peter      (502) staff       (20)     3768 2016-12-15 20:17:34.000000 clodius-0.9.4/clodius/higlass_getter.py
+-rw-r--r--   0 peter      (502) staff       (20)     4129 2016-12-15 20:17:34.000000 clodius-0.9.4/clodius/fpark.py
+-rw-r--r--   0 peter      (502) staff       (20)     7650 2017-10-06 13:46:07.000000 clodius-0.9.4/clodius/hdf_tiles.py
+-rw-r--r--   0 peter      (502) staff       (20)    18120 2018-09-27 13:40:12.000000 clodius-0.9.4/clodius/tiles.py
+-rw-r--r--   0 peter      (502) staff       (20)        0 2016-12-15 20:17:34.000000 clodius-0.9.4/clodius/__init__.py
+drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-09-27 13:40:54.000000 clodius-0.9.4/clodius/cli/
+-rw-r--r--   0 peter      (502) staff       (20)    48438 2018-06-21 20:49:59.000000 clodius-0.9.4/clodius/cli/aggregate.py
+-rw-r--r--   0 peter      (502) staff       (20)     7971 2018-06-15 20:10:09.000000 clodius-0.9.4/clodius/cli/convert.py
+-rw-r--r--   0 peter      (502) staff       (20)      333 2018-05-06 18:53:22.000000 clodius-0.9.4/clodius/cli/__init__.py
+-rw-r--r--   0 peter      (502) staff       (20)     1305 2018-05-06 18:53:22.000000 clodius-0.9.4/clodius/cli/utils.py
+-rw-r--r--   0 peter      (502) staff       (20)   312218 2017-07-14 15:30:08.000000 clodius-0.9.4/clodius/fast.c
+-rw-r--r--   0 peter      (502) staff       (20)    15458 2017-07-31 16:32:38.000000 clodius-0.9.4/clodius/save_tiles.py
+-rw-r--r--   0 peter      (502) staff       (20)      856 2016-12-15 20:17:34.000000 clodius-0.9.4/clodius/describe_dataset.py
+-rw-r--r--   0 peter      (502) staff       (20)       38 2018-09-27 13:40:54.000000 clodius-0.9.4/setup.cfg
+drwxr-xr-x   0 peter      (502) staff       (20)        0 2018-09-27 13:40:54.000000 clodius-0.9.4/clodius.egg-info/
+-rw-r--r--   0 peter      (502) staff       (20)      225 2018-09-27 13:40:54.000000 clodius-0.9.4/clodius.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (502) staff       (20)      990 2018-09-27 13:40:54.000000 clodius-0.9.4/clodius.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (502) staff       (20)       55 2018-09-27 13:40:54.000000 clodius-0.9.4/clodius.egg-info/entry_points.txt
+-rw-r--r--   0 peter      (502) staff       (20)       75 2018-09-27 13:40:54.000000 clodius-0.9.4/clodius.egg-info/requires.txt
+-rw-r--r--   0 peter      (502) staff       (20)        8 2018-09-27 13:40:54.000000 clodius-0.9.4/clodius.egg-info/top_level.txt
+-rw-r--r--   0 peter      (502) staff       (20)        1 2018-09-27 13:40:54.000000 clodius-0.9.4/clodius.egg-info/dependency_links.txt
```

### Comparing `clodius-0.9.3/test/tile_2d_bedfile_test.py` & `clodius-0.9.4/test/tile_2d_bedfile_test.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/test/utils.py` & `clodius-0.9.4/test/utils.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/conversion_wrapper.py` & `clodius-0.9.4/scripts/conversion_wrapper.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/make_big_file.py` & `clodius-0.9.4/scripts/make_big_file.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/tile_1d.py` & `clodius-0.9.4/scripts/tile_1d.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/make_streaming_tiles.py` & `clodius-0.9.4/scripts/make_streaming_tiles.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/exonU.py` & `clodius-0.9.4/scripts/exonU.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/make_single_threaded_tiles.py` & `clodius-0.9.4/scripts/make_single_threaded_tiles.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/get_hitile.py` & `clodius-0.9.4/scripts/get_hitile.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/make_autocomplete_list.py` & `clodius-0.9.4/scripts/make_autocomplete_list.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/check_sorted.py` & `clodius-0.9.4/scripts/check_sorted.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/big_spark.py` & `clodius-0.9.4/scripts/big_spark.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/cooler_to_tiles.py` & `clodius-0.9.4/scripts/cooler_to_tiles.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/process_file.py` & `clodius-0.9.4/scripts/process_file.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/test_1d.py` & `clodius-0.9.4/scripts/test_1d.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/scripts/make_tiles.py` & `clodius-0.9.4/scripts/make_tiles.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/multivec.py` & `clodius-0.9.4/clodius/multivec.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,25 @@
     # the start of the batch in the dataset
     batch_start_index = 0
     
     if has_header:
         f.readline()
 
     prev_chrom = None
+    print('base_resolution:', base_resolution)
+    warned = False
+
     for line in f:
         chrom,start,end,vector = bedline_to_chrom_start_end_vector(line)
 
+        if end - start != base_resolution and not warned:
+            print("WARNING: interval length ({}) doesn't match base resolution ({}): {}".
+                    format(end - start, base_resolution, line))
+            warned = True
+
         if prev_chrom is not None and chrom != prev_chrom:
             # we've reached a new chromosome so we'll dump all
             # the previous values
             print("len(batch:", len(batch))
             f_out[prev_chrom][batch_start_index:batch_start_index+len(batch)] = np.array(batch)
             
             # we're starting a new chromosome so we start from the beginning
@@ -127,14 +135,15 @@
     # store some metadata
     f.create_group('info')
     f['info'].attrs['tile-size'] = tile_size
     
     f.create_group('resolutions')
     f.create_group('chroms')
 
+    print("array_data:", array_data['segment1'][-20:])
     # start with a resolution of 1 element per pixel
     curr_resolution = starting_resolution
 
     # this will be our sample highest-resolution array
     # and it will be stored under the resolutions['1']
     # dataset
     f['resolutions'].create_group(str(curr_resolution))
@@ -221,15 +230,14 @@
             new_shape = list(chrom_data.shape)
             new_shape[0] = math.ceil(new_shape[0] / 2)
             new_shape = tuple(new_shape)
 
             f['resolutions'][str(curr_resolution)]['values'].create_dataset(chrom, 
                                             new_shape, compression='gzip')
 
-
             while start < len(chrom_data):
                 print('start:', start)
                 old_data = f['resolutions'][str(prev_resolution)]['values'][chrom][start:start+chunk_size]
                 #print("prev_resolution:", prev_resolution)
                 #print("old_data.shape", old_data.shape)
 
                 # this is a sort of roundabout way of calculating the
```

### Comparing `clodius-0.9.3/clodius/db_tiles.py` & `clodius-0.9.4/clodius/db_tiles.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/chromosomes.py` & `clodius-0.9.4/clodius/chromosomes.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/higlass_getter.py` & `clodius-0.9.4/clodius/higlass_getter.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/fpark.py` & `clodius-0.9.4/clodius/fpark.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/hdf_tiles.py` & `clodius-0.9.4/clodius/hdf_tiles.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/tiles.py` & `clodius-0.9.4/clodius/tiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 from __future__ import print_function
 
 import json
 import math
 import numpy as np
 import sys
 import time
-import clodius.fast as cf
 
-def aggregate(in_array, num_to_agg):
-    return cf.aggregate(in_array.astype(np.float32), num_to_agg)
+def aggregate(x, k):
+    x  = np.asarray(x)
+
+    if len(x) % k != 0:
+        extend = (k - len(x) % k)
+        x = np.r_[x, [np.nan] * extend]
+
+    xr = x.reshape((-1, k))
+    is_allnan = np.all(np.isnan(xr), axis=1)
+    agg = np.nansum(xr, axis=1)
+    
+    if np.any(is_allnan):
+        if not issubclass(agg.dtype.type, np.floating):
+            agg = agg.astype(np.float64)
+        agg[is_allnan] = np.nan
+    
+    return agg
 
 def load_entries_from_file(sc, filename, column_names=None, delimiter=None, 
         elasticsearch_path=None):
     '''
     Load a dataset from file.
 
     :parma sc: SparkContext (or FakeSparkContext)
```

### Comparing `clodius-0.9.3/clodius/cli/aggregate.py` & `clodius-0.9.4/clodius/cli/aggregate.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/cli/convert.py` & `clodius-0.9.4/clodius/cli/convert.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/cli/utils.py` & `clodius-0.9.4/clodius/cli/utils.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/fast.c` & `clodius-0.9.4/clodius/fast.c`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/save_tiles.py` & `clodius-0.9.4/clodius/save_tiles.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius/describe_dataset.py` & `clodius-0.9.4/clodius/describe_dataset.py`

 * *Files identical despite different names*

### Comparing `clodius-0.9.3/clodius.egg-info/SOURCES.txt` & `clodius-0.9.4/clodius.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 MANIFEST.in
+README.md
 setup.py
 clodius/__init__.py
 clodius/chromosomes.py
 clodius/db_tiles.py
 clodius/describe_dataset.py
 clodius/fast.c
-clodius/fast.pyx
 clodius/fpark.py
 clodius/hdf_tiles.py
 clodius/higlass_getter.py
 clodius/multivec.py
 clodius/save_tiles.py
 clodius/tiles.py
 clodius.egg-info/PKG-INFO
```

