# Comparing `tmp/Simba-UW-tf-dev-1.59.3.tar.gz` & `tmp/Simba-UW-tf-dev-1.59.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.3.tar", last modified: Fri May 12 17:13:05 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.4.tar", last modified: Mon May 15 13:15:39 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.59.3.tar` & `Simba-UW-tf-dev-1.59.4.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-08 20:25:25.000000 Simba-UW-tf-dev-1.59.3/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9493 2023-05-07 18:06:51.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12626 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.3/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6032 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.3/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12633 2023-05-08 03:02:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.3/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    33955 2023-05-04 19:55:21.000000 Simba-UW-tf-dev-1.59.3/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.3/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20792 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3466 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)    10045 2023-05-09 12:31:02.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7036 2023-05-11 18:18:55.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23576 2023-05-11 15:34:10.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8522 2023-05-10 01:30:19.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6069 2023-05-09 14:09:16.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11275 2023-05-10 01:31:30.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-09 20:23:32.000000 Simba-UW-tf-dev-1.59.3/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42325 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21312 2023-05-10 01:45:20.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13664 2023-05-10 14:48:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46271 2023-05-10 14:43:16.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23787 2023-05-10 01:48:07.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16700 2023-05-10 01:45:20.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.3/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42147 2023-05-10 02:11:17.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29762 2023-05-10 01:52:46.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18516 2023-05-10 02:13:29.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    25962 2023-05-09 13:55:01.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61203 2023-05-10 11:39:12.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    56361 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6858 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7675 2023-05-10 01:34:21.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12265 2023-05-10 01:34:21.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16782 2023-05-10 01:34:21.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1720 2023-05-08 15:05:19.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15347 2023-05-10 01:37:18.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12672 2023-05-10 01:37:18.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11617 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.59.3/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.3/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.3/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-10 19:45:32.000000 Simba-UW-tf-dev-1.59.3/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    34300 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2703 2023-05-12 17:13:03.000000 Simba-UW-tf-dev-1.59.3/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.3/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    14225 2023-05-07 19:37:44.000000 Simba-UW-tf-dev-1.59.3/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8378 2023-05-09 12:23:43.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2641 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9140 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10199 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8571 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12404 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    15294 2023-05-07 18:00:44.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15872 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12769 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10168 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5217 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12806 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12434 2023-05-04 17:45:23.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7919 2023-05-11 20:33:52.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11289 2023-05-10 14:49:41.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15234 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9409 2023-05-10 14:54:58.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13262 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11539 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13164 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9046 2023-05-09 14:13:06.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9801 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16351 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6721 2023-05-10 01:37:18.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11848 2023-05-10 01:41:05.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7444 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12747 2023-05-10 01:39:08.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9692 2023-05-10 01:39:08.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8258 2023-05-04 17:41:51.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4837 2023-05-10 01:43:03.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16856 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2947 2023-05-10 01:43:03.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9643 2023-05-10 01:41:05.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7596 2023-05-09 14:38:58.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19309 2023-05-08 19:28:39.000000 Simba-UW-tf-dev-1.59.3/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.59.3/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18698 2023-05-04 19:56:21.000000 Simba-UW-tf-dev-1.59.3/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3256 2023-05-08 19:18:20.000000 Simba-UW-tf-dev-1.59.3/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5917 2023-05-04 19:36:28.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19774 2023-05-09 14:43:23.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11373 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11432 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8029 2023-05-09 19:08:37.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11066 2023-05-09 19:08:37.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7374 2023-05-09 19:41:31.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    11817 2023-05-09 19:15:18.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6947 2023-05-09 20:29:25.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    42300 2023-05-08 18:44:41.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24710 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7343 2023-05-08 18:23:30.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11101 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2804 2023-05-12 17:10:03.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-12 16:12:08.000000 Simba-UW-tf-dev-1.59.3/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-09 20:23:32.000000 Simba-UW-tf-dev-1.59.3/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-05-09 20:23:39.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    19089 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.3/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.3/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.3/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-12 17:13:03.000000 Simba-UW-tf-dev-1.59.3/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-08 20:25:25.000000 Simba-UW-tf-dev-1.59.4/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.4/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6032 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.4/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12633 2023-05-08 03:02:50.000000 Simba-UW-tf-dev-1.59.4/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.4/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    33955 2023-05-04 19:55:21.000000 Simba-UW-tf-dev-1.59.4/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.4/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.4/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.59.4/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3445 2023-05-13 17:39:29.000000 Simba-UW-tf-dev-1.59.4/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.59.4/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.59.4/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)    10045 2023-05-09 12:31:02.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.4/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6385 2023-05-14 18:27:47.000000 Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11388 2023-05-14 18:30:24.000000 Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.59.4/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-05-14 19:55:18.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.4/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42147 2023-05-10 02:11:17.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29958 2023-05-13 17:59:00.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18516 2023-05-10 02:13:29.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    31956 2023-05-13 20:39:19.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61099 2023-05-15 13:05:40.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    56956 2023-05-14 15:25:25.000000 Simba-UW-tf-dev-1.59.4/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6167 2023-05-14 16:16:53.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10047 2023-05-14 16:16:20.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9027 2023-05-14 16:18:29.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18244 2023-05-14 16:20:14.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8164 2023-05-14 16:18:29.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6847 2023-05-14 16:17:16.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-05-14 16:18:29.000000 Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7650 2023-05-14 19:13:54.000000 Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12215 2023-05-14 19:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16698 2023-05-14 19:13:54.000000 Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1870 2023-05-14 19:13:54.000000 Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15241 2023-05-14 19:13:54.000000 Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12659 2023-05-14 19:13:54.000000 Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.59.4/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.4/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.4/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.4/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-10 19:45:32.000000 Simba-UW-tf-dev-1.59.4/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    34680 2023-05-15 12:56:17.000000 Simba-UW-tf-dev-1.59.4/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.4/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2703 2023-05-12 17:13:03.000000 Simba-UW-tf-dev-1.59.4/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.4/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    14225 2023-05-07 19:37:44.000000 Simba-UW-tf-dev-1.59.4/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.4/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8273 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5189 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2625 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.4/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9146 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13238 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14624 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10086 2023-05-14 15:45:08.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15735 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8701 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    15248 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15873 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12810 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10168 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5191 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5822 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12950 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12791 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7913 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11269 2023-05-14 23:35:43.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15234 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11244 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9376 2023-05-14 23:35:43.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13340 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11536 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15598 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13205 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8294 2023-05-15 13:12:15.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9810 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16291 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.4/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6695 2023-05-14 19:17:05.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    14002 2023-05-14 19:35:26.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12807 2023-05-14 19:22:08.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4800 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9645 2023-05-14 19:37:14.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7732 2023-05-14 19:37:49.000000 Simba-UW-tf-dev-1.59.4/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19307 2023-05-14 15:34:06.000000 Simba-UW-tf-dev-1.59.4/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-05-14 15:34:06.000000 Simba-UW-tf-dev-1.59.4/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18658 2023-05-14 15:28:54.000000 Simba-UW-tf-dev-1.59.4/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3246 2023-05-14 15:34:06.000000 Simba-UW-tf-dev-1.59.4/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5916 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1730 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19762 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11342 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11300 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13781 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12429 2023-05-14 18:02:35.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7278 2023-05-14 18:01:57.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12140 2023-05-14 18:05:59.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7769 2023-05-14 17:38:13.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6963 2023-05-14 17:34:27.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.4/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24687 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7329 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.59.4/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8180 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64839 2023-05-14 16:16:53.000000 Simba-UW-tf-dev-1.59.4/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-09 20:23:32.000000 Simba-UW-tf-dev-1.59.4/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.4/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.4/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.4/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.4/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-05-09 20:23:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.4/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.4/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.4/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-15 13:15:38.000000 Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    19089 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-15 13:15:38.000000 Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-15 13:15:38.000000 Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-15 13:15:38.000000 Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-15 13:15:38.000000 Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.4/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.4/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.4/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-15 13:12:43.000000 Simba-UW-tf-dev-1.59.4/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-15 13:15:39.000000 Simba-UW-tf-dev-1.59.4/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.59.3/PKG-INFO` & `Simba-UW-tf-dev-1.59.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.3
+Version: 1.59.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,23 +110,23 @@
                                                           style_attr=style_attr,
                                                           final_img_setting=self.heatmap_last_frm_var.get(),
                                                           video_setting=self.heatmap_videos_var.get(),
                                                           frame_setting=self.heatmap_frames_var.get(),
                                                           bodypart=self.bp_dropdown.getChoices(),
                                                           files_found=data_paths)
 
-            heatmapper_clf_processor = multiprocessing.Process(heatmapper_clf.create_heatmaps())
+            heatmapper_clf_processor = multiprocessing.Process(heatmapper_clf.run())
             heatmapper_clf_processor.start()
 
         else:
             heatmapper_clf = HeatMapperLocationMultiprocess(config_path=self.config_path,
                                                             style_attr=style_attr,
                                                             final_img_setting=self.heatmap_last_frm_var.get(),
                                                             video_setting=self.heatmap_videos_var.get(),
                                                             frame_setting=self.heatmap_frames_var.get(),
                                                             bodypart=self.bp_dropdown.getChoices(),
                                                             files_found=data_paths,
                                                             core_cnt=int(self.multiprocess_dropdown.getChoices()))
 
-            heatmapper_clf.create_heatmaps()
+            heatmapper_clf.run()
 
 #_ = HeatmapLocationPopup(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,10 +130,10 @@
             simba_plotter = PlotSklearnResultsSingleCore(config_path=self.config_path,
                                                          video_setting=self.create_videos_var.get(),
                                                          rotate=self.rotate_img_var.get(),
                                                          video_file_path=video_file_path,
                                                          frame_setting=self.create_frames_var.get(),
                                                          print_timers=self.include_timers_var.get(),
                                                          text_settings=print_settings)
-        simba_plotter.initialize_visualizations()
+        simba_plotter.run()
 
 #_ = SklearnVisualizationPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,11 +67,11 @@
 
         kleinberg_analyzer = KleinbergCalculator(config_path=self.config_path,
                                                  classifier_names=targets,
                                                  sigma=self.k_sigma.entry_get,
                                                  gamma=self.k_gamma.entry_get,
                                                  hierarchy=self.k_hierarchy.entry_get,
                                                  hierarchical_search=hierarchical_search)
-        kleinberg_analyzer.perform_kleinberg()
+        kleinberg_analyzer.run()
 
 
 #_ = KleinbergPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         button_run.grid(row=2, column=1, sticky=W)
 
     def run_reorganization(self):
         if self.pose_tool == 'DLC':
             new_bp_list = []
             for curr_choice in self.newbplist:
                 new_bp_list.append(curr_choice.get())
-            self.keypoint_reorganizer.perform_reorganization(animal_list=None, bp_lst=new_bp_list)
+            self.keypoint_reorganizer.run(animal_list=None, bp_lst=new_bp_list)
 
         if self.pose_tool == 'maDLC':
             new_bp_list, new_animal_list = [], []
             for curr_animal, curr_bp in zip(self.newanimallist, self.newbplist):
                 new_bp_list.append(curr_bp.getChoices())
                 new_animal_list.append(curr_animal.getChoices())
-            self.keypoint_reorganizer.perform_reorganization(animal_list=new_animal_list, bp_lst=new_bp_list)
+            self.keypoint_reorganizer.run(animal_list=new_animal_list, bp_lst=new_bp_list)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,24 +115,24 @@
                                                      final_img_setting=self.heatmap_last_frm_var.get(),
                                                      video_setting=self.heatmap_videos_var.get(),
                                                      frame_setting=self.heatmap_frames_var.get(),
                                                      bodypart=self.bp_dropdown.getChoices(),
                                                      files_found=data_paths,
                                                      clf_name=self.clf_dropdown.getChoices())
 
-            heatmapper_clf_processor = multiprocessing.Process(heatmapper_clf.create_heatmaps())
+            heatmapper_clf_processor = multiprocessing.Process(heatmapper_clf.run())
             heatmapper_clf_processor.start()
 
         else:
             heatmapper_clf = HeatMapperClfMultiprocess(config_path=self.config_path,
                                                        style_attr=style_attr,
                                                        final_img_setting=self.heatmap_last_frm_var.get(),
                                                        video_setting=self.heatmap_videos_var.get(),
                                                        frame_setting=self.heatmap_frames_var.get(),
                                                        bodypart=self.bp_dropdown.getChoices(),
                                                        files_found=data_paths,
                                                        clf_name=self.clf_dropdown.getChoices(),
                                                        core_cnt=int(self.multiprocess_dropdown.getChoices()))
 
-            heatmapper_clf.create_heatmaps()
+            heatmapper_clf.run()
 
 #_ = HeatmapClfPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,25 +98,25 @@
         style_attr['Border_color'] = self.colors_dict[self.border_clr_dropdown.getChoices()]
         style_attr['Pose_estimation'] = self.show_pose_var.get()
         style_attr['Directionality_style'] = self.directionality_type_dropdown.getChoices()
 
         if not multiple:
             if not self.multiprocess_var.get():
                 roi_feature_visualizer = ROIfeatureVisualizer(config_path=self.config_path, video_name=self.single_video_dropdown.getChoices(), style_attr=style_attr)
-                roi_feature_visualizer.create_visualization()
+                roi_feature_visualizer.run()
             else:
                 roi_feature_visualizer = ROIfeatureVisualizerMultiprocess(config_path=self.config_path, video_name=self.single_video_dropdown.getChoices(), style_attr=style_attr, core_cnt=int(self.multiprocess_dropdown.getChoices()))
-                roi_feature_visualizer_mp = multiprocessing.Process(target=roi_feature_visualizer.create_visualization())
+                roi_feature_visualizer_mp = multiprocessing.Process(target=roi_feature_visualizer.run())
                 roi_feature_visualizer_mp.start()
         else:
             if not self.multiprocess_var.get():
                 for video_name in self.video_list:
                     roi_feature_visualizer = ROIfeatureVisualizer(config_path=self.config_path, video_name=video_name, style_attr=style_attr)
-                    roi_feature_visualizer.create_visualization()
+                    roi_feature_visualizer.run()
             else:
                 for video_name in self.video_list:
                     roi_feature_visualizer = ROIfeatureVisualizerMultiprocess(config_path=self.config_path, video_name=video_name, style_attr=style_attr, core_cnt=int(self.multiprocess_dropdown.getChoices()))
-                    roi_feature_visualizer_mp = multiprocessing.Process(target=roi_feature_visualizer.create_visualization())
+                    roi_feature_visualizer_mp = multiprocessing.Process(target=roi_feature_visualizer.run())
                     roi_feature_visualizer_mp.start()
 
 #_ = VisualizeROIFeaturesPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         gantt_frm.grid(row=3, column=0, sticky=NW)
         self.gantt_dropdown.grid(row=0, column=0, sticky=NW)
 
         self.create_run_frm(run_function=self.run)
         self.main_frm.mainloop()
 
     def run(self):
-
         settings = {'pose': str_2_bool(self.show_pose_dropdown.getChoices()), 'animal_names': str_2_bool(self.show_animal_names_dropdown.getChoices())}
         settings['styles'] = None
         if not self.default_style_var.get():
             check_float(name='FONT SIZE', value=self.font_size_eb.entry_get)
             check_float(name='CIRCLE SIZE', value=self.circle_size.entry_get)
             check_float(name='SPACE SCALE', value=self.spacing_eb.entry_get)
             settings['styles']['circle size'] = int(self.circle_size.entry_get)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,8 +59,8 @@
     def run(self):
         bp_to_remove_list, animal_names_list = [], []
         for number, drop_down in enumerate(self.drop_down_list):
             bp_to_remove_list.append(drop_down.getChoices())
         if self.pose_tool == 'maDLC':
             for number, drop_down in enumerate(self.animal_names_lst):
                 animal_names_list.append(drop_down.getChoices())
-        _ = self.keypoint_remover.run_bp_removal(bp_to_remove_list=bp_to_remove_list, animal_names=animal_names_list)
+        _ = self.keypoint_remover.run(bp_to_remove_list=bp_to_remove_list, animal_names=animal_names_list)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.59.4/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.59.4/simba/labelling/labelling_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,25 @@
 from simba.utils.read_write import read_config_entry, read_df, write_df, get_fn_ext, get_video_meta_data, get_all_clf_names
 from simba.utils.checks import check_file_exist_and_readable, check_int, check_float
 from simba.utils.printing import stdout_success
 import simba
 
 class LabellingInterface(ConfigReader):
     """
-    Class for launching ``standard`` and ``pseudo``-labelling (annotation) GUI interface in SimBA.
+    Launch ``standard`` or ``pseudo``-labelling (annotation) GUI interface in SimBA.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    file_path: str
-        Path to video that is to be annotated
-    setting: str
-        String representing annotation method. OPTIONS: 'from_scratch' or 'pseudo'
-    threshold_dict: dict
-        If setting is ``pseudo``, threshold_dict dict contains the machine probability thresholds, with the classifier
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str file_path: Path to video that is to be annotated
+    :parameter str setting: String representing annotation method. OPTIONS: ``from_scratch`` or ``pseudo``
+    :parameter dict threshold_dict: If setting ``pseudo``, threshold_dict dict contains the machine probability thresholds, with the classifier
         names as keys and the classification probabilities as values, e.g. {'Attack': 0.40, 'Sniffing': 0.7).
-    continuing: bool
-        If True, continouing previously started annotation session.
-
+    :parameter bool continuing: If True, continouing previously started annotation session.
 
-    Notes
-    ----------
-    `Annotation tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/label_behavior.md>`__.
+    .. note::
+       Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/label_behavior.md>`__.
 
     Examples
     ----------
     >>> select_labelling_video(config_path='MyConfigPath', threshold_dict={'Attack': 0.4}, file_path='MyVideoFilePath', setting='pseudo', continuing=False)
     """
 
     def __init__(self,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.59.4/simba/labelling/extract_labelled_frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 from simba.utils.printing import stdout_success
 from simba.utils.enums import Dtypes
 from simba.utils.errors import FrameRangeError
 from simba.utils.checks import check_that_column_exist
 
 
 class AnnotationFrameExtractor(ConfigReader):
+    """
+    Extracts all human annotated frames where behavior is annotated as present into .pngs within a SimBA project
+
+    :param list clfs: Names of classifiers to extract behavior-present images from.
+    :param dict settings: User-defined settings. E.g., how much to downsample the png images.
+    :param str config_path: path to SimBA configparser.ConfigParser project_config.in
+
+    :example:
+    >>> extractor = AnnotationFrameExtractor(config_path='project_folder/project_config.ini', clfs=['Sniffing', 'Attack'], settings={'downsample': 2})
+    >>> extractor.run()
+    """
+
+
     def __init__(self,
                  clfs: List[str],
                  settings: Dict[str, int],
                  config_path: str):
-        """
-        Extracts all human annotated frames where behavior is annotated as present into .pngs within a SimBA project
-
-        :param clfs: Names of classifiers to extract behavior-present images from.
-        :param settings: User-defined settings. E.g., how much to downsample the png images.
-        :param config_path: path to SimBA configparser.ConfigParser project_config.ini
-
-        :example:
-        >>> extractor = AnnotationFrameExtractor(config_path='project_folder/project_config.ini', clfs=['Sniffing', 'Attack'], settings={'downsample': 2})
-        >>> extractor.run()
-        """
 
         self.clfs = clfs
         self.settings = settings
         super().__init__(config_path=config_path)
 
     def run(self):
         if not os.path.exists(self.annotated_frm_dir): os.makedirs(self.annotated_frm_dir)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.59.4/simba/labelling/labelling_advanced_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,35 +18,26 @@
                                     get_all_clf_names)
 from simba.utils.errors import FrameRangeError, AdvancedLabellingError
 from simba.utils.printing import stdout_success
 from simba.mixins.config_reader import ConfigReader
 
 class AdvancedLabellingInterface(ConfigReader):
     """
-    Class for advanced labelling (annotation) interface in SimBA.
-    https://github.com/sgoldenlab/simba/blob/master/docs/advanced_labelling.md
+    Launch advanced labelling (annotation) interface in SimBA.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    file_path: str
-        Path to video that is to be annotated
-    continuing: bool
-        If True, the user is continuing the annotations of a video with started but incomplete annotations.
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str file_path: Path to video that is to be annotated
+    :parameter bool continuing: If True, user is continuing the annotations of a video with started but incomplete annotations.
 
-    Notes
-    ----------
-    `Advanced annotation tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/advanced_labelling.md>`__.
+    .. note::
+        `Advanced annotation tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/advanced_labelling.md>`__.
 
     Examples
     ----------
     >>> select_labelling_video_advanced(config_path='MyProjectConfig', file_path='MyVideoFilePath', continuing=True)
-
-
     """
 
     def __init__(self,
                  config_path: str,
                  file_path: str,
                  continuing: bool):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.59.4/simba/labelling/play_annotation_video.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import signal
 from simba.utils.read_write import get_video_meta_data
 from simba.utils.lookups import get_color_dict
 from simba.utils.checks import check_file_exist_and_readable
 
 def annotation_video_player():
+    """ Private methods for playing the video that is being annotated in SimBA GUI"""
 
     def labelling_log_writer(frame_number: int) -> None:
         f.seek(0)
         f.write(str(frame_number))
         f.truncate()
         f.flush()
         os.fsync(f.fileno())
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.59.4/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Simon Nilsson"
 import pandas as pd
 import os, glob
-from typing import List
+from typing import List, Union
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 
 from simba.utils.read_write import read_df, get_fn_ext
 from simba.utils.printing import stdout_success
@@ -14,36 +14,31 @@
 from simba.mixins.config_reader import ConfigReader
 
 class AggBoundaryStatisticsCalculator(ConfigReader):
 
     """
     Compute aggregate boundary statistics
 
-    Parameters
-    ----------
-    config_path: str Path to SimBA project config file in Configparser format
-    measures: list
-        Aggregate statistics measurements. OPTIONS: 'DETAILED INTERACTIONS TABLE', 'INTERACTION TIME (s)', 'INTERACTION BOUT COUNT', 'INTERACTION BOUT MEAN (s)', 'INTERACTION BOUT MEDIAN (s)'
-    shortest_allowed_interaction: int
-        The shortest allowed animal-anchored ROI intersection in millisecond.
+    :parameter str config_path: SimBA project config file in Configparser format
+    :parameter List[str] measures: Aggregate statistics measurements. OPTIONS: 'DETAILED INTERACTIONS TABLE', 'INTERACTION TIME (s)', 'INTERACTION BOUT COUNT', 'INTERACTION BOUT MEAN (s)', 'INTERACTION BOUT MEDIAN (s)'
+    :parameter int shortest_allowed_interaction: The shortest allowed animal-anchored ROI intersection in millisecond.
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>`_.
+    `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>`_.
 
     Examples
     ----------
     >>> boundary_stats_calculator = AggBoundaryStatisticsCalculator('MyProjectConfig', measures=['INTERACTION TIME (s)'], shortest_allowed_interaction=200)
     >>> boundary_stats_calculator.run()
     >>> boundary_stats_calculator.save()
     """
 
-
     def __init__(self,
-                 config_path: str,
+                 config_path: Union[str, os.PathLike],
                  measures: List[Literal['INTERACTION TIME (s)', 'INTERACTION BOUT COUNT', 'INTERACTION BOUT MEAN (s)', 'INTERACTION BOUT MEDIAN (s)']],
                  shortest_allowed_interaction: int):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.measures, self.shortest_allowed_interaction_ms = measures, shortest_allowed_interaction
         self.anchored_roi_path = os.path.join(self.project_path, 'logs', 'anchored_rois.pickle')
         self.data_path = os.path.join(self.project_path, 'csv', 'anchored_roi_data')
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/boundary_menus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import os, glob
 import pickle
 from tkinter import *
+from typing import Union
+
 from simba.bounding_box_tools.find_boundaries import AnimalBoundaryFinder
 from simba.bounding_box_tools.visualize_boundaries import BoundaryVisualizer
 from simba.bounding_box_tools.boundary_statistics import BoundaryStatisticsCalculator
 from simba.bounding_box_tools.agg_boundary_stats import AggBoundaryStatisticsCalculator
 from simba.utils.errors import NoFilesFoundError, NoChoosenMeasurementError
 from simba.utils.enums import Keys, Links
 from simba.mixins.config_reader import ConfigReader
@@ -20,29 +22,27 @@
 from simba.utils.lookups import get_named_colors
 
 class BoundaryMenus(ConfigReader, PopUpMixin):
     """
     Launch GUI interface for extrapolating bounding boxes from pose-estimation data, and calculating
     statstics on bounding boxes and pose-estimated key-point intersections.
 
-    Parameters
-    ----------
-    config_path: str path to SimBA project config file in Configparser format
+    :parameter str config_path: str path to SimBA project config file in Configparser format
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>`_.
+    `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>`_.
 
     Examples
     ----------
     >>> _ = BoundaryMenus(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini')
     """
 
     def __init__(self,
-                 config_path: str):
+                 config_path: Union[str, os.PathLike]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PopUpMixin.__init__(self, title="SIMBA ANCHORED ROI (BOUNDARY BOXES ANALYSIS)", size=(750, 300))
         self.named_shape_colors = get_named_colors()
         self.settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.BBOXES.value)
         self.max_animal_name_char = len(max([x for x in list(self.animal_bp_dict.keys())]))
         self.find_boundaries_btn = Button(self.settings_frm, text='FIND ANIMAL BOUNDARIES', command=lambda: self.__launch_find_boundaries_pop_up())
@@ -111,15 +111,15 @@
         parallel_offset = self.parallel_offset_entry.entry_get
         check_int(name='PARALLEL OFFSET', value=parallel_offset)
         boundary_finder = AnimalBoundaryFinder(config_path=self.config_path,
                                                roi_type=self.selected_shape_type,
                                                body_parts=body_parts,
                                                force_rectangle=force_rectangle,
                                                parallel_offset=int(parallel_offset))
-        boundary_finder.find_boundaries()
+        boundary_finder.run()
 
     def __launch_visualize_boundaries(self):
         self.anchored_roi_path = os.path.join(self.project_path, 'logs', 'anchored_rois.pickle')
         if not os.path.isfile(self.anchored_roi_path):
             raise NoFilesFoundError(msg='No anchored ROI found in {}.'.format(self.anchored_roi_path))
         with open(self.anchored_roi_path, 'rb') as fp: self.roi_data = pickle.load(fp)
         videos_in_project = find_all_videos_in_project(videos_dir=self.video_dir)
@@ -221,15 +221,15 @@
         video_visualizer = BoundaryVisualizer(config_path=self.config_path,
                                               video_name=self.select_video_dropdown.getChoices(),
                                               include_key_points=include_keypoints,
                                               greyscale=greyscale,
                                               show_intersections=highlight_intersections,
                                               roi_attributes=roi_attr)
 
-        video_visualizer.run_visualization()
+        video_visualizer.run()
 
     def __launch_boundary_statistics(self):
         self.anchored_roi_path = os.path.join(self.project_path, 'logs', 'anchored_rois.pickle')
         if not os.path.isfile(self.anchored_roi_path):
             raise NoFilesFoundError(msg='SIMBA ERROR: No anchored ROI found in {}.'.format(self.anchored_roi_path))
         self.statistics_frm = Toplevel()
         self.statistics_frm.minsize(400, 150)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/boundary_statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,24 @@
 from simba.utils.read_write import read_df, write_df
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success
 
 
 class BoundaryStatisticsCalculator(ConfigReader):
     """
-    Class computing boundary intersection statistics.
+    Compute boundary intersection statistics.
 
-    Parameters
-    ----------
-    config_path: str
-        Path to SimBA project config file in Configparser format
-    roi_intersections: bool
-        If True, calculates intersection of animal-anchored ROIs
-    roi_keypoint_intersections: bool
-        If True, calculates intersection of animal-anchored ROIs and pose-estimated animal key-points.
-    save_format: str
-        Output data format. OPTIONS: CSV, PARQUET, PICKLE.
+    :parameter str config_path: Path to SimBA project config file in Configparser format.
+    :parameter bool roi_intersections: If True, calculates intersection of animal-anchored ROIs
+    :parameter bool roi_keypoint_intersections: If True, calculates intersection of animal-anchored ROIs and pose-estimated animal key-points.
+    :parameter str save_format: Output data format. OPTIONS: CSV, PARQUET, PICKLE.
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>_`.
+    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>`_.
 
     Examples
     ----------
     >>> boundary_stats_calculator = BoundaryStatisticsCalculator(config_path='MyConfigFile',roi_intersections=True, roi_keypoint_intersections=True, save_format='CSV')
     >>> boundary_stats_calculator.save_results()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/find_boundaries.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,55 +4,51 @@
 import itertools
 import numpy as np
 from shapely.geometry import (Polygon,
                               Point,
                               LineString)
 import shapely.wkt
 from joblib import Parallel, delayed
+from typing import Optional
 from simba.utils.read_write import read_df, write_df, get_fn_ext, find_core_cnt
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.printing import stdout_success
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 
 class AnimalBoundaryFinder(ConfigReader, FeatureExtractionMixin):
     """
-    Class finding boundaries (animal-anchored) ROIs for animals in each frame. Result is saved as a pickle in the
-    `project_folder/logs` directory of the SimBA project.
+    Compute boundaries (animal-anchored) ROIs for animals in each frame. Result is saved
+    as a pickle in the ``project_folder/logs`` directory of the SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    roi_type: str
-        shape type of ROI. OPTIONS: ENTIRE ANIMAL, SINGLE BODY-PART SQUARE, SINGLE BODY-PART CIRCLE
-    force_rectangle: bool or None
-        If True, forces roi shape into rectangles.
-    body_parts: dict
-        Body-parts to anchor the ROI to with keys as animal names and values as body-parts. E.g., body_parts={'Animal_1': 'Head_1', 'Animal_2': 'Head_2'}.
-    parallel_offset: int
-        Offset of ROI from the animal outer bounds in millimeter.
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str roi_type: shape type of ROI. OPTIONS: "ENTIRE ANIMAL", "SINGLE BODY-PART SQUARE", "SINGLE BODY-PART CIRCLE". For
+                             more information/examples, see `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md/>`_.
+    :parameter bool force_rectangle: If True, forces roi shape into minimum bounding rectangle. If False, then polygon.
+    :parameter Optional[dict] or None body_parts: If roi_type is 'SINGLE BODY-PART CIRCLE' or 'SINGLE BODY-PART SQUARE', then body-parts to anchor the ROI to
+                                        with keys as animal names and values as body-parts. E.g., body_parts={'Animal_1': 'Head_1', 'Animal_2': 'Head_2'}.
+    :parameter Optional[int] parallel_offset: Offset of ROI from the animal outer bounds in millimeter. If None, then no offset.
 
     Notes
     ----------
     `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md/>`_.
 
     Examples
     ----------
-    >>> animal_boundary_finder= AnimalBoundaryFinder(config_path='/Users/simon/Desktop/troubleshooting/termites/project_folder/project_config.ini', roi_type='SINGLE BODY-PART CIRCLE',body_parts={'Animal_1': 'Head_1', 'Animal_2': 'Head_2'}, force_rectangle=False, parallel_offset=15)
-    >>> animal_boundary_finder.find_boundaries()
+    >>> animal_boundary_finder = AnimalBoundaryFinder(config_path='project_folder/project_config.ini', roi_type='SINGLE BODY-PART CIRCLE',body_parts={'Animal_1': 'Head_1', 'Animal_2': 'Head_2'}, force_rectangle=False, parallel_offset=15)
+    >>> animal_boundary_finder.run()
     """
 
 
     def __init__(self,
                  config_path: str,
                  roi_type: str or None,
                  force_rectangle: bool,
-                 body_parts: dict or None,
-                 parallel_offset: int or None):
+                 body_parts: Optional[dict] = None,
+                 parallel_offset: Optional[int] = None):
 
         ConfigReader.__init__(self, config_path=config_path)
         FeatureExtractionMixin.__init__(self)
         self.parallel_offset_mm, self.roi_type, self.force_rectangle = parallel_offset, roi_type, force_rectangle
         if self.parallel_offset_mm == 0: self.parallel_offset_mm += 1
         self.body_parts = body_parts
         check_if_filepath_list_is_empty(filepaths=self.outlier_corrected_paths,
@@ -80,15 +76,15 @@
             bottom_right = Point(int(point_array[0] + self.offset_px), int(point_array[1] + self.offset_px))
             animal_shape = Polygon([top_left, top_right, bottom_left, bottom_right])
         if self.force_rectangle:
             animal_shape = Polygon(self.minimum_bounding_rectangle(points=np.array(animal_shape.exterior.coords)))
         animal_shape = shapely.wkt.loads(shapely.wkt.dumps(animal_shape, rounding_precision=1)).simplify(0)
         return animal_shape
 
-    def find_boundaries(self):
+    def run(self):
         self.polygons = {}
         for file_cnt, file_path in enumerate(self.outlier_corrected_paths):
             _, self.video_name, _ = get_fn_ext(file_path)
             _, px_per_mm, _ = self.read_video_info(video_name=self.video_name)
             self.offset_px = px_per_mm * self.parallel_offset_mm
             self.polygons[self.video_name] = {}
             self.data_df = read_df(file_path=file_path,file_type=self.file_type).astype(int)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.59.4/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,38 +58,32 @@
 #         else:
 #             print('SIMBA WARNING: SimBA tried to grab frame number {} from video {}, but could not find it. The video has {} frames.'.format(str(current_frame), video_path, str(cap.get(cv2.CAP_PROP_FRAME_COUNT))))
 #     return img_lst
 
 class BoundaryVisualizer(ConfigReader,
                          PlottingMixin):
     """
-    Class visualizing user-specified animal-anchored ROI boundaries. Results are stored in the
-    `project_folder/frames/output/anchored_rois` directory of teh SimBA project
+    Visualisation of user-specified animal-anchored ROI boundaries. Results are stored in the
+    ``project_folder/frames/output/anchored_rois`` directory of the SimBA project
 
-    Parameters
-    ----------
-    config_path: str
-        Path to SimBA project config file in Configparser format
-    video_name: str
-        Name of the video in the SimBA project to create bounding box video for
-    include_key_points: bool
-        If True, includes pose-estimated body-parts in the visualization.
-    greyscale: bool
-        If True, converts the video (but not the shapes/keypoints) to greyscale.
-    show_intersections: bool or None
-        If True, then produce highlight boundaries/keypoints to signify present intersections.
+    :parameter str config_path: Path to SimBA project config file in Configparser format
+    :parameter str video_name: Name of the video in the SimBA project to create bounding box video for
+    :parameter bool include_key_points: If True, includes pose-estimated body-parts in the video.
+    :parameter bool greyscale:  If True, converts the video (but not the shapes/keypoints) to greyscale.
+    :parameter bool show_intersections:  If True, then produce highlight boundaries/keypoints to signify present intersections.
+                                         See `this example for highlighted intersections <https://github.com/sgoldenlab/simba/blob/master/images/termites_video_3.gif>`_
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>_`.
+    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>`_.
 
     Examples
     ----------
     >>> boundary_visualizer = BoundaryVisualizer(config_path='MySimBAConfig', video_name='MyVideoName', include_key_points=True, greyscale=True)
-    >>> boundary_visualizer.run_visualization()
+    >>> boundary_visualizer.run()
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  video_name: str,
                  include_key_points: bool,
                  greyscale: bool,
@@ -122,15 +116,15 @@
             print('SIMBA WARNING: No ROI intersection data found for video {} in directory {}. Skipping intersection visualizations'.format(self.video_name, self.intersection_data_folder))
             self.show_intersections = False
             self.intersections_df = None
         else:
             _, _, ext = get_fn_ext(filepath=self.intersection_path)
             self.intersections_df = read_df(file_path=self.intersection_path, file_type=ext[1:])
 
-    def run_visualization(self, chunk_size=50):
+    def run(self, chunk_size=50):
         if self.include_key_points:
             self.data_df_path = os.path.join(self.outlier_corrected_dir, self.video_name + '.' + self.file_type)
             if not os.path.isfile(self.data_df_path):
                 raise NoFilesFoundError(msg=f'SIMBA ERROR: No keypoint data found in {self.data_df_path}. Untick key-point checkbox or import pose-estimation data.')
             self.data_df = read_df(file_path=self.data_df_path, file_type=self.file_type).astype(int).reset_index(drop=True)
         else:
             self.data_df = None
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -745,16 +745,16 @@
 00002e80: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
 00002e90: 0064 6d6f 4444 626c 6f62 0000 0008 6269  .dmoDDblob....bi
 00002ea0: 0543 3a05 c541 0000 000c 0075 006e 0073  .C:..A.....u.n.s
 00002eb0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
 00002ec0: 0064 6d6f 6444 626c 6f62 0000 0008 6269  .dmodDblob....bi
 00002ed0: 0543 3a05 c541 0000 000c 0075 006e 0073  .C:..A.....u.n.s
 00002ee0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-00002ef0: 0064 7068 3153 636f 6d70 0000 0000 0007  .dph1Scomp......
-00002f00: 9000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+00002ef0: 0064 7068 3153 636f 6d70 0000 0000 0009  .dph1Scomp......
+00002f00: b000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
 00002f10: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
 00002f20: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
 00002f30: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
 00002f40: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
 00002f50: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 00002f60: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 00002f70: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
@@ -764,15 +764,15 @@
 00002fb0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
 00002fc0: 0809 5f10 197b 7b32 3332 2c20 3139 317d  .._..{{232, 191}
 00002fd0: 2c20 7b31 3330 322c 2037 3134 7d7d 0908  , {1302, 714}}..
 00002fe0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
 00002ff0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
 00003000: 0000 0000 0000 0000 0000 0010 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 0003 cc2d 0000 0005 0075  mp.......-.....u
+00003020: 6d70 0000 0000 0005 9dfc 0000 0005 0075  mp.............u
 00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
 00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
 00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -848,20 +848,20 @@
 000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
 00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
 00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
 00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
 00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
 00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
 00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 08e5 d1d7  smoDDblob.......
-00003570: 0ac9 04c5 4100 0000 0500 7500 7400 6900  ....A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 08e5  l.smodDblob.....
-00003590: d1d7 0ac9 04c5 4100 0000 0500 7500 7400  ......A.....u.t.
+00003560: 736d 6f44 4462 6c6f 6200 0000 08b8 f217  smoDDblob.......
+00003570: ee15 06c5 4100 0000 0500 7500 7400 6900  ....A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 08b8  l.smodDblob.....
+00003590: f217 ee15 06c5 4100 0000 0500 7500 7400  ......A.....u.t.
 000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000035b0: 0000 0490 0000 0000 0500 7500 7400 6900  ..........u.t.i.
+000035b0: 0000 06d0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
 000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 000035f0: 7200 7362 7773 7062 6c6f 6200 0000 ca62  r.sbwspblob....b
 00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00003610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00003620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
@@ -876,15 +876,15 @@
 000036b0: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 000036c0: 0000 0000 0000 0000 9b00 0000 1000 7600  ..............v.
 000036d0: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
 000036e0: 6300 6500 7300 7300 6f00 7200 7364 7363  c.e.s.s.o.r.sdsc
 000036f0: 6c62 6f6f 6c00 0000 0010 0076 0069 0064  lbool......v.i.d
 00003700: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00003710: 0073 0073 006f 0072 0073 6c67 3153 636f  .s.s.o.r.slg1Sco
-00003720: 6d70 0000 0000 0003 85ef 0000 0010 0076  mp.............v
+00003720: 6d70 0000 0000 0004 d59f 0000 0010 0076  mp.............v
 00003730: 0069 0064 0065 006f 005f 0070 0072 006f  .i.d.e.o._.p.r.o
 00003740: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
 00003750: 7643 626c 6f62 0000 0297 6270 6c69 7374  vCblob....bplist
 00003760: 3030 d801 0203 0405 0607 0809 0a0b 1949  00.............I
 00003770: 4a0a 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
 00003780: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
 00003790: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
@@ -972,15 +972,15 @@
 00003cb0: 3fde 4cbd 04c5 4100 0000 1000 7600 6900  ?.L...A.....v.i.
 00003cc0: 6400 6500 6f00 5f00 7000 7200 6f00 6300  d.e.o._.p.r.o.c.
 00003cd0: 6500 7300 7300 6f00 7200 736d 6f64 4462  e.s.s.o.r.smodDb
 00003ce0: 6c6f 6200 0000 0858 3fde 4cbd 04c5 4100  lob....X?.L...A.
 00003cf0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 00003d00: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 00003d10: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-00003d20: 0460 0000 0000 1000 7600 6900 6400 6500  .`......v.i.d.e.
+00003d20: 0600 0000 0000 1000 7600 6900 6400 6500  ........v.i.d.e.
 00003d30: 6f00 5f00 7000 7200 6f00 6300 6500 7300  o._.p.r.o.c.e.s.
 00003d40: 7300 6f00 7200 7376 5372 6e6c 6f6e 6700  s.o.r.svSrnlong.
 00003d50: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1034,24 +1034,24 @@
 00004090: 006d 0062 0061 005f 0064 0065 0076 002f  .m.b.a._.d.e.v./
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
-00004100: 005f 6c67 3153 636f 6d70 0000 0000 0042  ._lg1Scomp.....B
-00004110: 0340 0000 000b 005f 005f 0070 0079 0063  .@....._._.p.y.c
+00004100: 005f 6c67 3153 636f 6d70 0000 0000 003f  ._lg1Scomp.....?
+00004110: e690 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 3b88 1802 0f04 c541  blob....;......A
+00004130: 626c 6f62 0000 0008 ff8d e56c 4e07 c541  blob.......lN..A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
-00004160: 6f62 0000 0008 3b88 1802 0f04 c541 0000  ob....;......A..
+00004160: 6f62 0000 0008 ff8d e56c 4e07 c541 0000  ob.......lN..A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
-00004190: 0000 0000 004f e000 0000 0006 0061 0073  .....O.......a.s
+00004190: 0000 0000 004d c000 0000 0006 0061 0073  .....M.......a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
 000041b0: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
 000041c0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 000041d0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 000041e0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 000041f0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00004200: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
@@ -1059,15 +1059,15 @@
 00004220: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
 00004230: 0809 5f10 187b 7b33 362c 2031 3331 7d2c  .._..{{36, 131},
 00004240: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
 00004250: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 00004260: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 00004270: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
 00004280: 0600 6100 7300 7300 6500 7400 736c 6731  ..a.s.s.e.t.slg1
-00004290: 5363 6f6d 7000 0000 0000 7ddb 9300 0000  Scomp.....}.....
+00004290: 5363 6f6d 7000 0000 0000 7ddc 3800 0000  Scomp.....}.8...
 000042a0: 0600 6100 7300 7300 6500 7400 736c 7376  ..a.s.s.e.t.slsv
 000042b0: 4362 6c6f 6200 0002 b062 706c 6973 7430  Cblob....bplist0
 000042c0: 30da 0102 0304 0506 0708 090a 0b0c 0d1a  0...............
 000042d0: 4849 484a 0c4c 5869 636f 6e53 697a 655f  HIHJ.LXiconSize_
 000042e0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
 000042f0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
 00004300: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
@@ -1154,15 +1154,15 @@
 00004810: 0000 0000 0000 0000 01dd 0000 0006 0061  ...............a
 00004820: 0073 0073 0065 0074 0073 6d6f 4444 626c  .s.s.e.t.smoDDbl
 00004830: 6f62 0000 0008 cf95 8ce8 d0e1 c441 0000  ob...........A..
 00004840: 0006 0061 0073 0073 0065 0074 0073 6d6f  ...a.s.s.e.t.smo
 00004850: 6444 626c 6f62 0000 0008 cf95 8ce8 d0e1  dDblob..........
 00004860: c441 0000 0006 0061 0073 0073 0065 0074  .A.....a.s.s.e.t
 00004870: 0073 7068 3153 636f 6d70 0000 0000 0081  .sph1Scomp......
-00004880: a000 0000 0006 0061 0073 0073 0065 0074  .......a.s.s.e.t
+00004880: b000 0000 0006 0061 0073 0073 0065 0074  .......a.s.s.e.t
 00004890: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
 000048a0: 000c 0062 006c 006f 0062 005f 0073 0074  ...b.l.o.b._.s.t
 000048b0: 006f 0072 0061 0067 0065 6277 7370 626c  .o.r.a.g.ebwspbl
 000048c0: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
 000048d0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 000048e0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 000048f0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
@@ -1207,15 +1207,15 @@
 00004b60: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
 00004b70: 1200 6200 6f00 7500 6e00 6400 6900 6e00  ..b.o.u.n.d.i.n.
 00004b80: 6700 5f00 6200 6f00 7800 5f00 7400 6f00  g._.b.o.x._.t.o.
 00004b90: 6f00 6c00 7364 7363 6c62 6f6f 6c00 0000  o.l.sdsclbool...
 00004ba0: 0012 0062 006f 0075 006e 0064 0069 006e  ...b.o.u.n.d.i.n
 00004bb0: 0067 005f 0062 006f 0078 005f 0074 006f  .g._.b.o.x._.t.o
 00004bc0: 006f 006c 0073 6c67 3153 636f 6d70 0000  .o.l.slg1Scomp..
-00004bd0: 0000 0002 6c79 0000 0012 0062 006f 0075  ....ly.....b.o.u
+00004bd0: 0000 0003 1753 0000 0012 0062 006f 0075  .....S.....b.o.u
 00004be0: 006e 0064 0069 006e 0067 005f 0062 006f  .n.d.i.n.g._.b.o
 00004bf0: 0078 005f 0074 006f 006f 006c 0073 6c73  .x._.t.o.o.l.sls
 00004c00: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
 00004c10: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
 00004c20: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
 00004c30: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
 00004c40: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
@@ -1278,22 +1278,22 @@
 00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005000: 0000 0000 0000 0000 0000 001d 0000 0012  ................
 00005010: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 00005020: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 00005030: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
-00005040: c351 4bc6 4505 c541 0000 0012 0062 006f  .QK.E..A.....b.o
+00005040: 3d4b 2d20 b008 c541 0000 0012 0062 006f  =K- ...A.....b.o
 00005050: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
 00005060: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
-00005070: 6d6f 6444 626c 6f62 0000 0008 0270 b7c1  modDblob.....p..
-00005080: 4105 c541 0000 0012 0062 006f 0075 006e  A..A.....b.o.u.n
+00005070: 6d6f 6444 626c 6f62 0000 0008 5311 5fb9  modDblob....S._.
+00005080: 9505 c541 0000 0012 0062 006f 0075 006e  ...A.....b.o.u.n
 00005090: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
 000050a0: 005f 0074 006f 006f 006c 0073 7068 3153  ._.t.o.o.l.sph1S
-000050b0: 636f 6d70 0000 0000 0002 f000 0000 0012  comp............
+000050b0: 636f 6d70 0000 0000 0003 c000 0000 0012  comp............
 000050c0: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 000050d0: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 000050e0: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 000050f0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
 00005100: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
 00005110: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
 00005120: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
@@ -1310,25 +1310,25 @@
 000051d0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 000051e0: 0000 0000 0000 9a00 0000 0f00 6300 7500  ............c.u.
 000051f0: 6500 5f00 6c00 6900 6700 6800 7400 5f00  e._.l.i.g.h.t._.
 00005200: 7400 6f00 6f00 6c00 7364 7363 6c62 6f6f  t.o.o.l.sdsclboo
 00005210: 6c00 0000 000f 0063 0075 0065 005f 006c  l......c.u.e._.l
 00005220: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00005230: 006c 0073 6c67 3153 636f 6d70 0000 0000  .l.slg1Scomp....
-00005240: 0001 d983 0000 000f 0063 0075 0065 005f  .........c.u.e._
+00005240: 0002 99c1 0000 000f 0063 0075 0065 005f  .........c.u.e._
 00005250: 006c 0069 0067 0068 0074 005f 0074 006f  .l.i.g.h.t._.t.o
 00005260: 006f 006c 0073 6d6f 4444 626c 6f62 0000  .o.l.smoDDblob..
-00005270: 0008 a4c2 03c3 a304 c541 0000 000f 0063  .........A.....c
+00005270: 0008 8dcf 6f39 b508 c541 0000 000f 0063  ....o9...A.....c
 00005280: 0075 0065 005f 006c 0069 0067 0068 0074  .u.e._.l.i.g.h.t
 00005290: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
-000052a0: 626c 6f62 0000 0008 dc16 211a fb01 c541  blob......!....A
+000052a0: 626c 6f62 0000 0008 d824 2d67 9605 c541  blob.....$-g...A
 000052b0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
 000052c0: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
-000052d0: 0073 7068 3153 636f 6d70 0000 0000 0002  .sph1Scomp......
-000052e0: 6000 0000 000f 0063 0075 0065 005f 006c  `......c.u.e._.l
+000052d0: 0073 7068 3153 636f 6d70 0000 0000 0003  .sph1Scomp......
+000052e0: 7000 0000 000f 0063 0075 0065 005f 006c  p......c.u.e._.l
 000052f0: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00005300: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 00005310: 0000 0008 0064 0061 0073 0068 005f 0061  .....d.a.s.h._.a
 00005320: 0070 0070 6277 7370 626c 6f62 0000 00c9  .p.pbwspblob....
 00005330: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 00005340: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 00005350: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
@@ -1370,15 +1370,15 @@
 00005590: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 000055a0: 0000 0000 0000 0000 9b00 0000 0f00 6400  ..............d.
 000055b0: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
 000055c0: 6500 7300 7300 6f00 7200 7364 7363 6c62  e.s.s.o.r.sdsclb
 000055d0: 6f6f 6c00 0000 000f 0064 0061 0074 0061  ool......d.a.t.a
 000055e0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 000055f0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00005600: 0000 0002 c428 0000 000f 0064 0061 0074  .....(.....d.a.t
+00005600: 0000 0003 f399 0000 000f 0064 0061 0074  ...........d.a.t
 00005610: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
 00005620: 0073 006f 0072 0073 6c73 7643 626c 6f62  .s.o.r.slsvCblob
 00005630: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00005640: 0405 0607 0809 0a0b 1949 4a0a 4c58 6963  .........IJ.LXic
 00005650: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
 00005660: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 00005670: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
@@ -1458,22 +1458,22 @@
 00005b10: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
 00005b20: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
 00005b30: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
 00005b40: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
 00005b50: 0000 0000 0001 ac00 0000 0f00 6400 6100  ............d.a.
 00005b60: 7400 6100 5f00 7000 7200 6f00 6300 6500  t.a._.p.r.o.c.e.
 00005b70: 7300 7300 6f00 7200 736d 6f44 4462 6c6f  s.s.o.r.smoDDblo
-00005b80: 6200 0000 080b 5109 4149 05c5 4100 0000  b.....Q.AI..A...
+00005b80: 6200 0000 08bb 9c92 1397 05c5 4100 0000  b...........A...
 00005b90: 0f00 6400 6100 7400 6100 5f00 7000 7200  ..d.a.t.a._.p.r.
 00005ba0: 6f00 6300 6500 7300 7300 6f00 7200 736d  o.c.e.s.s.o.r.sm
-00005bb0: 6f64 4462 6c6f 6200 0000 080b 5109 4149  odDblob.....Q.AI
+00005bb0: 6f64 4462 6c6f 6200 0000 08bb 9c92 1397  odDblob.........
 00005bc0: 05c5 4100 0000 0f00 6400 6100 7400 6100  ..A.....d.a.t.a.
 00005bd0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 00005be0: 6f00 7200 7370 6831 5363 6f6d 7000 0000  o.r.sph1Scomp...
-00005bf0: 0000 03a0 0000 0000 0f00 6400 6100 7400  ..........d.a.t.
+00005bf0: 0000 0540 0000 0000 0f00 6400 6100 7400  ...@......d.a.t.
 00005c00: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
 00005c10: 7300 6f00 7200 7376 5372 6e6c 6f6e 6700  s.o.r.svSrnlong.
 00005c20: 0000 0100 0000 1200 6600 6500 6100 7400  ........f.e.a.t.
 00005c30: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00005c40: 6100 6300 7400 6f00 7200 7362 7773 7062  a.c.t.o.r.sbwspb
 00005c50: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
 00005c60: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
@@ -1490,15 +1490,15 @@
 00005d10: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
 00005d20: 9b00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
 00005d30: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
 00005d40: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
 00005d50: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
 00005d60: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d70: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00005d80: 6d70 0000 0000 0013 5536 163e 1640 0810  mp......U6.>.@..
+00005d80: 6d70 0000 0000 0015 5cdf 163e 1640 0810  mp......\..>.@..
 00005d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
 00005da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
 00005db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
 00005dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
 00005dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
 00005de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
 00005df0: bc00 c700 c800 cb00 cc00 d100 da00 db00  ................
@@ -1579,22 +1579,22 @@
 000062a0: a501 ae01 b001 b201 b301 b401 bd01 bf01  ................
 000062b0: c201 c301 c401 c501 ce01 d701 e400 0000  ................
 000062c0: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
 000062d0: 0000 0000 0000 0000 0000 0001 e500 0000  ................
 000062e0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000062f0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 00006300: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
-00006310: 08b3 7108 4149 05c5 4100 0000 1200 6600  ..q.AI..A.....f.
+00006310: 0889 1273 46d6 08c5 4100 0000 1200 6600  ...sF...A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
-00006340: 736d 6f64 4462 6c6f 6200 0000 0866 04c9  smodDblob....f..
-00006350: 1d50 01c5 4100 0000 1200 6600 6500 6100  .P..A.....f.e.a.
+00006340: 736d 6f64 4462 6c6f 6200 0000 083d 8fc4  smodDblob....=..
+00006350: 12f3 05c5 4100 0000 1200 6600 6500 6100  ....A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
-00006380: 5363 6f6d 7000 0000 0000 15d0 0000 0000  Scomp...........
+00006380: 5363 6f6d 7000 0000 0000 1820 0000 0000  Scomp...... ....
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
 000063e0: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000063f0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
@@ -1607,15 +1607,15 @@
 00006460: 095f 1019 7b7b 3233 322c 2031 3931 7d2c  ._..{{232, 191},
 00006470: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
 00006480: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
 00006490: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 000064a0: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
 000064b0: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
 000064c0: 6e00 676c 6731 5363 6f6d 7000 0000 0000  n.glg1Scomp.....
-000064d0: 019c f300 0000 0900 6c00 6100 6200 6500  ........l.a.b.e.
+000064d0: 0240 7500 0000 0900 6c00 6100 6200 6500  .@u.....l.a.b.e.
 000064e0: 6c00 6c00 6900 6e00 676c 7376 4362 6c6f  l.l.i.n.glsvCblo
 000064f0: 6200 0002 7962 706c 6973 7430 30d8 0102  b...ybplist00...
 00006500: 0304 0506 0708 090a 0b16 4647 480a 5f10  ..........FGH._.
 00006510: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
 00006520: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
 00006530: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
 00006540: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
@@ -1691,20 +1691,20 @@
 000069a0: 0161 0163 0164 0165 016e 0170 0172 0173  .a.c.d.e.n.p.r.s
 000069b0: 0174 017d 017f 0181 0182 0183 018c 018e  .t.}............
 000069c0: 0191 0192 0193 0194 019d 01a2 01ab 0000  ................
 000069d0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 000069e0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
 000069f0: 0009 006c 0061 0062 0065 006c 006c 0069  ...l.a.b.e.l.l.i
 00006a00: 006e 0067 6d6f 4444 626c 6f62 0000 0008  .n.gmoDDblob....
-00006a10: c446 b51b 4305 c541 0000 0009 006c 0061  .F..C..A.....l.a
+00006a10: 9c3c 7c32 d208 c541 0000 0009 006c 0061  .<|2...A.....l.a
 00006a20: 0062 0065 006c 006c 0069 006e 0067 6d6f  .b.e.l.l.i.n.gmo
 00006a30: 6444 626c 6f62 0000 0008 c446 b51b 4305  dDblob.....F..C.
 00006a40: c541 0000 0009 006c 0061 0062 0065 006c  .A.....l.a.b.e.l
 00006a50: 006c 0069 006e 0067 7068 3153 636f 6d70  .l.i.n.gph1Scomp
-00006a60: 0000 0000 0001 e000 0000 0009 006c 0061  .............l.a
+00006a60: 0000 0000 0002 a000 0000 0009 006c 0061  .............l.a
 00006a70: 0062 0065 006c 006c 0069 006e 0067 7653  .b.e.l.l.i.n.gvS
 00006a80: 726e 6c6f 6e67 0000 0001 0000 0006 006d  rnlong.........m
 00006a90: 0069 0078 0069 006e 0073 6277 7370 626c  .i.x.i.n.sbwspbl
 00006aa0: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00006ab0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00006ac0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00006ad0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
@@ -1714,15 +1714,15 @@
 00006b10: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
 00006b20: 0809 0809 5f10 197b 7b32 3332 2c20 3139  ...._..{{232, 19
 00006b30: 317d 2c20 7b31 3330 322c 2037 3134 7d7d  1}, {1302, 714}}
 00006b40: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
 00006b50: 0000 0000 0000 0101 0000 0000 0000 000f  ................
 00006b60: 0000 0000 0000 0000 0000 0000 0000 009b  ................
 00006b70: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00006b80: 6c67 3153 636f 6d70 0000 0000 000a 5c2e  lg1Scomp......\.
+00006b80: 6c67 3153 636f 6d70 0000 0000 000e 162f  lg1Scomp......./
 00006b90: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
 00006ba0: 6c73 7643 626c 6f62 0000 0297 6270 6c69  lsvCblob....bpli
 00006bb0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 00006bc0: 1949 4a0a 4c58 6963 6f6e 5369 7a65 5f10  .IJ.LXiconSize_.
 00006bd0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 00006be0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
 00006bf0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 0432 5913 6f05 c541  blob.....2Y.o..A
+00007020: 626c 6f62 0000 0008 07c0 8672 9a08 c541  blob.......r...A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 3b9d 9b1a  modDblob....;...
-00007050: 4405 c541 0000 0006 006d 0069 0078 0069  D..A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 07c0 8672  modDblob.......r
+00007050: 9a08 c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 000b 6000 0000 0006 006d 0069 0078 0069  ..`......m.i.x.i
+00007070: 000f 5000 0000 0006 006d 0069 0078 0069  ..P......m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -1811,15 +1811,15 @@
 00007120: 6261 7208 0809 0809 5f10 197b 7b32 3332  bar....._..{{232
 00007130: 2c20 3139 317d 2c20 7b31 3330 322c 2037  , 191}, {1302, 7
 00007140: 3134 7d7d 0908 1725 313d 4960 6d79 7a7b  14}}...%1=I`myz{
 00007150: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
 00007160: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 00007170: 0000 009b 0000 0005 006d 006f 0064 0065  .........m.o.d.e
 00007180: 006c 6c67 3153 636f 6d70 0000 0000 0001  .llg1Scomp......
-00007190: 1648 0000 0005 006d 006f 0064 0065 006c  .H.....m.o.d.e.l
+00007190: 7d9b 0000 0005 006d 006f 0064 0065 006c  }......m.o.d.e.l
 000071a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 000071b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 000071c0: 1846 470a 4958 6963 6f6e 5369 7a65 5f10  .FG.IXiconSize_.
 000071d0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 000071e0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
 000071f0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
 00007200: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
@@ -1895,17 +1895,17 @@
 00007660: 7b01 7d01 8601 8701 8801 8a01 8c01 9501  {.}.............
 00007670: 9601 9701 9a01 9c01 9d01 a601 ab00 0000  ................
 00007680: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
 00007690: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
 000076a0: 0500 6d00 6f00 6400 6500 6c6d 6f44 4462  ..m.o.d.e.lmoDDb
 000076b0: 6c6f 6200 0000 08dc c0ca 73c2 04c5 4100  lob.......s...A.
 000076c0: 0000 0500 6d00 6f00 6400 6500 6c6d 6f64  ....m.o.d.e.lmod
-000076d0: 4462 6c6f 6200 0000 087a 22ce b222 02c5  Dblob....z".."..
+000076d0: 4462 6c6f 6200 0000 08dc c0ca 73c2 04c5  Dblob.......s...
 000076e0: 4100 0000 0500 6d00 6f00 6400 6500 6c70  A.....m.o.d.e.lp
-000076f0: 6831 5363 6f6d 7000 0000 0000 0140 0000  h1Scomp......@..
+000076f0: 6831 5363 6f6d 7000 0000 0000 01c0 0000  h1Scomp.........
 00007700: 0000 0500 6d00 6f00 6400 6500 6c76 5372  ....m.o.d.e.lvSr
 00007710: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
 00007720: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
 00007730: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
 00007740: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 00007750: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 00007760: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
@@ -1917,15 +1917,15 @@
 000077c0: 095f 1019 7b7b 3233 322c 2031 3931 7d2c  ._..{{232, 191},
 000077d0: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
 000077e0: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
 000077f0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 00007800: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
 00007810: 0d00 6f00 7500 7400 6c00 6900 6500 7200  ..o.u.t.l.i.e.r.
 00007820: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00007830: 6f6d 7000 0000 0000 0124 b500 0000 0d00  omp......$......
+00007830: 6f6d 7000 0000 0000 0160 2b00 0000 0d00  omp......`+.....
 00007840: 6f00 7500 7400 6c00 6900 6500 7200 5f00  o.u.t.l.i.e.r._.
 00007850: 7400 6f00 6f00 6c00 736c 7376 4362 6c6f  t.o.o.l.slsvCblo
 00007860: 6200 0002 b062 706c 6973 7430 30da 0102  b....bplist00...
 00007870: 0304 0506 0708 090a 0b0c 0d18 4849 484a  ............HIHJ
 00007880: 0c4c 5f10 1276 6965 774f 7074 696f 6e73  .L_..viewOptions
 00007890: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
 000078a0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
@@ -2009,22 +2009,22 @@
 00007d80: 017e 0187 0189 018b 018c 018d 0196 0198  .~..............
 00007d90: 019a 019b 019c 01a5 01a7 01a9 01aa 01ab  ................
 00007da0: 01b4 01b5 01b8 01b9 01bb 01bc 01c5 01ce  ................
 00007db0: 01d3 01d4 0000 0000 0000 0201 0000 0000  ................
 00007dc0: 0000 004c 0000 0000 0000 0000 0000 0000  ...L............
 00007dd0: 0000 01dd 0000 000d 006f 0075 0074 006c  .........o.u.t.l
 00007de0: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00007df0: 0073 6d6f 4444 626c 6f62 0000 0008 0bdb  .smoDDblob......
-00007e00: a04e 0b04 c541 0000 000d 006f 0075 0074  .N...A.....o.u.t
+00007df0: 0073 6d6f 4444 626c 6f62 0000 0008 24ed  .smoDDblob....$.
+00007e00: a135 5507 c541 0000 000d 006f 0075 0074  .5U..A.....o.u.t
 00007e10: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
 00007e20: 006c 0073 6d6f 6444 626c 6f62 0000 0008  .l.smodDblob....
 00007e30: 0bdb a04e 0b04 c541 0000 000d 006f 0075  ...N...A.....o.u
 00007e40: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
 00007e50: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-00007e60: 0000 0002 0000 0000 000d 006f 0075 0074  ...........o.u.t
+00007e60: 0000 0002 5000 0000 000d 006f 0075 0074  ....P......o.u.t
 00007e70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
 00007e80: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 00007e90: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
 00007ea0: 006e 0067 6277 7370 626c 6f62 0000 00ca  .n.gbwspblob....
 00007eb0: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 00007ec0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 00007ed0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
@@ -2035,15 +2035,15 @@
 00007f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 00007f30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 00007f40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 00007f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00007f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00007f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 00007f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00007f90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+00007f90: 3153 636f 6d70 0000 0000 000c 8e04 0000  1Scomp..........
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
@@ -2088,134 +2088,134 @@
 00008270: 8701 8901 8b01 8c01 8d01 9601 9801 9a01  ................
 00008280: 9b01 9c01 a501 a701 a901 aa01 ab01 b401  ................
 00008290: b601 b901 ba01 bb01 bc01 c501 ce01 d301  ................
 000082a0: d400 0000 0000 0002 0100 0000 0000 0000  ................
 000082b0: 4c00 0000 0000 0000 0000 0000 0000 0001  L...............
 000082c0: dd00 0000 0800 7000 6c00 6f00 7400 7400  ......p.l.o.t.t.
 000082d0: 6900 6e00 676d 6f44 4462 6c6f 6200 0000  i.n.gmoDDblob...
-000082e0: 089a d621 3946 05c5 4100 0000 0800 7000  ...!9F..A.....p.
+000082e0: 08e0 6946 f1d4 08c5 4100 0000 0800 7000  ..iF....A.....p.
 000082f0: 6c00 6f00 7400 7400 6900 6e00 676d 6f64  l.o.t.t.i.n.gmod
-00008300: 4462 6c6f 6200 0000 089a d621 3946 05c5  Dblob......!9F..
+00008300: 4462 6c6f 6200 0000 08e0 6946 f1d4 08c5  Dblob.....iF....
 00008310: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
 00008320: 6900 6e00 6770 6831 5363 6f6d 7000 0000  i.n.gph1Scomp...
-00008330: 0000 0b30 0000 0000 0800 7000 6c00 6f00  ...0......p.l.o.
+00008330: 0000 0fb0 0000 0000 0800 7000 6c00 6f00  ..........p.l.o.
 00008340: 7400 7400 6900 6e00 6776 5372 6e6c 6f6e  t.t.i.n.gvSrnlon
 00008350: 6700 0000 0100 0000 1300 7000 6f00 7300  g.........p.o.s.
 00008360: 6500 5f00 6300 6f00 6e00 6600 6900 6700  e._.c.o.n.f.i.g.
 00008370: 7500 7200 6100 7400 6900 6f00 6e00 7362  u.r.a.t.i.o.n.sb
 00008380: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
 00008390: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
 000083a0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
 000083b0: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
 000083c0: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
 000083d0: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
 000083e0: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
 000083f0: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00008400: 6562 6172 0808 0908 095f 1019 7b7b 3135  ebar....._..{{15
-00008410: 392c 2031 3233 7d2c 207b 3130 3736 2c20  9, 123}, {1076, 
-00008420: 3632 317d 7d09 0817 2531 3d49 606d 797a  621}}...%1=I`myz
+00008400: 6562 6172 0808 0908 095f 1019 7b7b 3133  ebar....._..{{13
+00008410: 372c 2031 3433 7d2c 207b 3133 3032 2c20  7, 143}, {1302, 
+00008420: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
 00008430: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
 00008440: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 00008450: 0000 0000 9b00 0000 1300 7000 6f00 7300  ..........p.o.s.
 00008460: 6500 5f00 6300 6f00 6e00 6600 6900 6700  e._.c.o.n.f.i.g.
 00008470: 7500 7200 6100 7400 6900 6f00 6e00 7364  u.r.a.t.i.o.n.sd
 00008480: 7363 6c62 6f6f 6c00 0000 0013 0070 006f  sclbool......p.o
 00008490: 0073 0065 005f 0063 006f 006e 0066 0069  .s.e._.c.o.n.f.i
 000084a0: 0067 0075 0072 0061 0074 0069 006f 006e  .g.u.r.a.t.i.o.n
 000084b0: 0073 6c67 3153 636f 6d70 0000 0000 0006  .slg1Scomp......
 000084c0: ae56 0000 0013 0070 006f 0073 0065 005f  .V.....p.o.s.e._
 000084d0: 0063 006f 006e 0066 0069 0067 0075 0072  .c.o.n.f.i.g.u.r
 000084e0: 0061 0074 0069 006f 006e 0073 6c73 7643  .a.t.i.o.n.slsvC
 000084f0: 626c 6f62 0000 02b0 6270 6c69 7374 3030  blob....bplist00
-00008500: da01 0203 0405 0607 0809 0a0b 0b0d 1a48  ...............H
-00008510: 4948 4a4b 4c5f 1010 7573 6552 656c 6174  IHJKL_..useRelat
-00008520: 6976 6544 6174 6573 5f10 0f73 686f 7749  iveDates_..showI
-00008530: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00008540: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00008550: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
-00008560: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
-00008570: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
-00008580: 6f6e 585a 736f 7274 436f 6c75 6d6e 5869  onXZsortColumnXi
-00008590: 636f 6e53 697a 655f 1012 7669 6577 4f70  conSize_..viewOp
-000085a0: 7469 6f6e 7356 6572 7369 6f6e 0909 ab0e  tionsVersion....
-000085b0: 171c 2125 2a2f 3439 3e43 d40f 1011 1213  ..!%*/49>C......
-000085c0: 140b 0b5a 6964 656e 7469 6669 6572 5577  ...ZidentifierUw
-000085d0: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-000085e0: 6973 6962 6c65 546e 616d 6511 0127 0909  isibleTname..'..
-000085f0: d40f 1011 1218 191a 1a58 7562 6971 7569  .........Xubiqui
-00008600: 7479 1023 0808 d40f 1011 121d 1e1a 0b5c  ty.#...........\
-00008610: 6461 7465 4d6f 6469 6669 6564 10b5 0809  dateModified....
-00008620: d40f 1011 1222 1e1a 1a5b 6461 7465 4372  ....."...[dateCr
-00008630: 6561 7465 6408 08d4 0f10 1112 2627 1a0b  eated.......&'..
-00008640: 5473 697a 6510 6108 09d4 0f10 1112 2b2c  Tsize.a.......+,
-00008650: 0b0b 546b 696e 6410 7309 09d4 0f10 1112  ..Tkind.s.......
-00008660: 3031 0b1a 556c 6162 656c 1064 0908 d40f  01..Ulabel.d....
-00008670: 1011 1235 360b 1a57 7665 7273 696f 6e10  ...56..Wversion.
-00008680: 4b09 08d4 0f10 1112 3a3b 0b1a 5863 6f6d  K.......:;..Xcom
-00008690: 6d65 6e74 7311 012c 0908 d40f 1011 123f  ments..,.......?
-000086a0: 401a 1a5e 6461 7465 4c61 7374 4f70 656e  @..^dateLastOpen
-000086b0: 6564 10c8 0808 d40f 1011 1244 1e1a 1a59  ed.........D...Y
-000086c0: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
-000086d0: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
-000086e0: 616d 6523 4030 0000 0000 0000 1001 0008  ame#@0..........
-000086f0: 001d 0030 0042 004a 005e 0070 0079 008b  ...0.B.J.^.p.y..
-00008700: 0096 009f 00b4 00b5 00b6 00c2 00cb 00d6  ................
-00008710: 00dc 00e6 00ee 00f3 00f6 00f7 00f8 0101  ................
-00008720: 010a 010c 010d 010e 0117 0124 0126 0127  ...........$.&.'
-00008730: 0128 0131 013d 013e 013f 0148 014d 014f  .(.1.=.>.?.H.M.O
-00008740: 0150 0151 015a 015f 0161 0162 0163 016c  .P.Q.Z._.a.b.c.l
-00008750: 0172 0174 0175 0176 017f 0187 0189 018a  .r.t.u.v........
-00008760: 018b 0194 019d 01a0 01a1 01a2 01ab 01ba  ................
-00008770: 01bc 01bd 01be 01c7 01d1 01d2 01d3 01d4  ................
-00008780: 01dd 01e6 01eb 01f4 0000 0000 0000 0201  ................
+00008500: da01 0203 0405 0607 0809 0a0b 0c0d 1848  ...............H
+00008510: 4948 4a4b 0c5f 1012 7669 6577 4f70 7469  IHJK._..viewOpti
+00008520: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
+00008530: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+00008540: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+00008550: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
+00008560: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
+00008570: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
+00008580: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
+00008590: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
+000085a0: 656c 6174 6976 6544 6174 6573 1001 09ab  elativeDates....
+000085b0: 0e17 1c21 252a 2f34 393e 43d4 0f10 1112  ...!%*/49>C.....
+000085c0: 0c14 0c16 5776 6973 6962 6c65 5577 6964  ....WvisibleUwid
+000085d0: 7468 5961 7363 656e 6469 6e67 5a69 6465  thYascendingZide
+000085e0: 6e74 6966 6965 7209 1101 c709 546e 616d  ntifier.....Tnam
+000085f0: 65d4 0f10 1112 1819 181b 0810 2308 5875  e...........#.Xu
+00008600: 6269 7175 6974 79d4 0f10 1112 0c1e 1820  biquity........ 
+00008610: 0910 b508 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00008620: 64d4 0f10 1112 181e 1824 0808 5b64 6174  d........$..[dat
+00008630: 6543 7265 6174 6564 d40f 1011 120c 2718  eCreated......'.
+00008640: 2909 1061 0854 7369 7a65 d40f 1011 120c  )..a.Tsize......
+00008650: 2c0c 2e09 1073 0954 6b69 6e64 d40f 1011  ,....s.Tkind....
+00008660: 1218 310c 3308 1064 0955 6c61 6265 6cd4  ..1.3..d.Ulabel.
+00008670: 0f10 1112 1836 0c38 0810 4b09 5776 6572  .....6.8..K.Wver
+00008680: 7369 6f6e d40f 1011 1218 3b0c 3d08 1101  sion......;.=...
+00008690: 2c09 5863 6f6d 6d65 6e74 73d4 0f10 1112  ,.Xcomments.....
+000086a0: 1840 1842 0810 c808 5e64 6174 654c 6173  .@.B....^dateLas
+000086b0: 744f 7065 6e65 64d4 0f10 1112 181e 1846  tOpened........F
+000086c0: 0808 5964 6174 6541 6464 6564 0823 0000  ..YdateAdded.#..
+000086d0: 0000 0000 0000 2340 2800 0000 0000 0054  ......#@(......T
+000086e0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
+000086f0: 001d 0032 0044 004c 0060 0072 007b 008d  ...2.D.L.`.r.{..
+00008700: 0098 00a1 00b4 00b6 00b7 00c3 00cc 00d4  ................
+00008710: 00da 00e4 00ef 00f0 00f3 00f4 00f9 0102  ................
+00008720: 0103 0105 0106 010f 0118 0119 011b 011c  ................
+00008730: 0129 0132 0133 0134 0140 0149 014a 014c  .).2.3.4.@.I.J.L
+00008740: 014d 0152 015b 015c 015e 015f 0164 016d  .M.R.[.\.^._.d.m
+00008750: 016e 0170 0171 0177 0180 0181 0183 0184  .n.p.q.w........
+00008760: 018c 0195 0196 0199 019a 01a3 01ac 01ad  ................
+00008770: 01af 01b0 01bf 01c8 01c9 01ca 01d4 01d5  ................
+00008780: 01de 01e7 01ec 01f5 0000 0000 0000 0201  ................
 00008790: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
 000087a0: 0000 0000 0000 01f6 0000 0013 0070 006f  .............p.o
 000087b0: 0073 0065 005f 0063 006f 006e 0066 0069  .s.e._.c.o.n.f.i
 000087c0: 0067 0075 0072 0061 0074 0069 006f 006e  .g.u.r.a.t.i.o.n
 000087d0: 0073 6c73 7670 626c 6f62 0000 0295 6270  .slsvpblob....bp
 000087e0: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
-000087f0: 0a0b 0b0d 1c48 4948 4a4b 295f 1010 7573  .....HIHJK)_..us
-00008800: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-00008810: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00008820: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00008830: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00008840: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-00008850: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-00008860: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-00008870: 6c75 6d6e 5869 636f 6e53 697a 655f 1012  lumnXiconSize_..
-00008880: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00008890: 6f6e 0909 d90e 0f10 1112 1314 1516 1720  on............. 
-000088a0: 252a 2e33 383d 4258 636f 6d6d 656e 7473  %*.38=BXcomments
-000088b0: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
-000088c0: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
-000088d0: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
-000088e0: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
-000088f0: 546e 616d 65d4 1819 1a1b 1c1d 0b1f 5776  Tname.........Wv
-00008900: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00008910: 656e 6469 6e67 5569 6e64 6578 0811 012c  endingUindex...,
-00008920: 0910 07d4 1819 1a1b 1c22 1c24 0810 c808  .........".$....
-00008930: 1008 d418 191a 1b0b 271c 2909 10b5 0810  ........'.).....
-00008940: 01d4 1819 1a1b 1c27 1c2d 0808 1002 d418  .......'.-......
-00008950: 191a 1b0b 301c 3209 1061 0810 03d4 1819  ....0.2..a......
-00008960: 1a1b 1c35 0b37 0810 6409 1005 d418 191a  ...5.7..d.......
-00008970: 1b0b 3a0b 3c09 1073 0910 04d4 1819 1a1b  ..:.<..s........
-00008980: 1c3f 0b41 0810 4b09 1006 d418 191a 1b0b  .?.A..K.........
-00008990: 440b 4609 1101 2709 1000 0823 0000 0000  D.F...'....#....
-000089a0: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
-000089b0: 6d65 2340 3000 0000 0000 0000 0800 1d00  me#@0...........
-000089c0: 3000 4200 4a00 5e00 7000 7900 8b00 9600  0.B.J.^.p.y.....
-000089d0: 9f00 b400 b500 b600 c900 d200 e100 ee00  ................
-000089e0: fa00 ff01 0501 0a01 1201 1701 2001 2801  ............ .(.
-000089f0: 2e01 3801 3e01 3f01 4201 4301 4501 4e01  ..8.>.?.B.C.E.N.
-00008a00: 4f01 5101 5201 5401 5d01 5e01 6001 6101  O.Q.R.T.].^.`.a.
-00008a10: 6301 6c01 6d01 6e01 7001 7901 7a01 7c01  c.l.m.n.p.y.z.|.
-00008a20: 7d01 7f01 8801 8901 8b01 8c01 8e01 9701  }...............
-00008a30: 9801 9a01 9b01 9d01 a601 a701 a901 aa01  ................
-00008a40: ac01 b501 b601 b901 ba01 bc01 bd01 c601  ................
-00008a50: cf01 d400 0000 0000 0002 0100 0000 0000  ................
+000087f0: 0a0b 0c0d 1f47 4847 494a 0c5f 1012 7669  .....GHGIJ._..vi
+00008800: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00008810: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00008820: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00008830: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
+00008840: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
+00008850: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
+00008860: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
+00008870: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
+00008880: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+00008890: 6573 1001 09d9 0e0f 1011 1213 1415 1617  es..............
+000088a0: 2025 292d 3237 3c41 5863 6f6d 6d65 6e74   %)-27<AXcomment
+000088b0: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
+000088c0: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
+000088d0: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
+000088e0: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
+000088f0: 6e54 6e61 6d65 d418 191a 1b1c 1d0c 1f55  nTname.........U
+00008900: 696e 6465 7855 7769 6474 6859 6173 6365  indexUwidthYasce
+00008910: 6e64 696e 6757 7669 7369 626c 6510 0711  ndingWvisible...
+00008920: 012c 0908 d418 191a 1b21 221f 1f10 0810  .,.......!".....
+00008930: c808 08d4 1819 1a1b 0b26 1f0c 10b5 0809  .........&......
+00008940: d418 191a 1b2a 261f 1f10 0208 08d4 1819  .....*&.........
+00008950: 1a1b 2e2f 1f0c 1003 1061 0809 d418 191a  .../.....a......
+00008960: 1b33 340c 1f10 0510 6409 08d4 1819 1a1b  .34.....d.......
+00008970: 3839 0c0c 1004 1073 0909 d418 191a 1b3d  89.....s.......=
+00008980: 3e0c 1f10 0610 4b09 08d4 1819 1a1b 4243  >.....K.......BC
+00008990: 0c0c 1000 1101 c709 0908 2300 0000 0000  ..........#.....
+000089a0: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+000089b0: 6523 4030 0000 0000 0000 0900 0800 1d00  e#@0............
+000089c0: 3200 4400 4c00 6000 7200 7b00 8d00 9800  2.D.L.`.r.{.....
+000089d0: a100 b400 b600 b700 ca00 d300 e200 ef00  ................
+000089e0: fb01 0001 0601 0b01 1301 1801 2101 2701  ............!.'.
+000089f0: 2d01 3701 3f01 4101 4401 4501 4601 4f01  -.7.?.A.D.E.F.O.
+00008a00: 5101 5301 5401 5501 5e01 6001 6101 6201  Q.S.T.U.^.`.a.b.
+00008a10: 6b01 6d01 6e01 6f01 7801 7a01 7c01 7d01  k.m.n.o.x.z.|.}.
+00008a20: 7e01 8701 8901 8b01 8c01 8d01 9601 9801  ~...............
+00008a30: 9a01 9b01 9c01 a501 a701 a901 aa01 ab01  ................
+00008a40: b401 b601 b901 ba01 bb01 bc01 c501 ce01  ................
+00008a50: d301 dc00 0000 0000 0002 0100 0000 0000  ................
 00008a60: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
 00008a70: 0001 dd00 0000 1300 7000 6f00 7300 6500  ........p.o.s.e.
 00008a80: 5f00 6300 6f00 6e00 6600 6900 6700 7500  _.c.o.n.f.i.g.u.
 00008a90: 7200 6100 7400 6900 6f00 6e00 736d 6f44  r.a.t.i.o.n.smoD
 00008aa0: 4462 6c6f 6200 0000 08d9 7e4b 74e2 ddc4  Dblob.....~Kt...
 00008ab0: 4100 0000 1300 7000 6f00 7300 6500 5f00  A.....p.o.s.e._.
 00008ac0: 6300 6f00 6e00 6600 6900 6700 7500 7200  c.o.n.f.i.g.u.r.
@@ -2263,24 +2263,24 @@
 00008d60: 7c7d 7e99 0000 0000 0000 0101 0000 0000  |}~.............
 00008d70: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 00008d80: 0000 009a 0000 000e 0070 006f 0073 0065  .........p.o.s.e
 00008d90: 005f 0069 006d 0070 006f 0072 0074 0065  ._.i.m.p.o.r.t.e
 00008da0: 0072 0073 6473 636c 626f 6f6c 0000 0000  .r.sdsclbool....
 00008db0: 0e00 7000 6f00 7300 6500 5f00 6900 6d00  ..p.o.s.e._.i.m.
 00008dc0: 7000 6f00 7200 7400 6500 7200 736c 6731  p.o.r.t.e.r.slg1
-00008dd0: 5363 6f6d 7000 0000 0000 0327 2674 006c  Scomp......'&t.l
+00008dd0: 5363 6f6d 7000 0000 0000 03e6 cf74 006c  Scomp........t.l
 00008de0: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00008df0: 0073 6d6f 4444 626c 6f62 0000 0008 0bdb  .smoDDblob......
-00008e00: a04e 0b04 c541 0000 000d 006f 0075 0074  .N...A.....o.u.t
+00008df0: 0073 6d6f 4444 626c 6f62 0000 0008 24ed  .smoDDblob....$.
+00008e00: a135 5507 c541 0000 000d 006f 0075 0074  .5U..A.....o.u.t
 00008e10: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
 00008e20: 006c 0073 6d6f 6444 626c 6f62 0000 0008  .l.smodDblob....
 00008e30: 0bdb a04e 0b04 c541 0000 000d 006f 0075  ...N...A.....o.u
 00008e40: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
 00008e50: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-00008e60: 0000 0002 0000 0000 000d 006f 0075 0074  ...........o.u.t
+00008e60: 0000 0002 5000 0000 000d 006f 0075 0074  ....P......o.u.t
 00008e70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
 00008e80: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 00008e90: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
 00008ea0: 006e 0067 6277 7370 626c 6f62 0000 00ca  .n.gbwspblob....
 00008eb0: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 00008ec0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 00008ed0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
@@ -2291,15 +2291,15 @@
 00008f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 00008f30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 00008f40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 00008f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00008f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00008f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 00008f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00008f90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+00008f90: 3153 636f 6d70 0000 0000 000c 8e04 0000  1Scomp..........
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
@@ -2342,22 +2342,22 @@
 00009250: 0160 0162 0163 0165 016e 016f 0171 0172  .`.b.c.e.n.o.q.r
 00009260: 0174 017d 017e 0180 0181 0183 018c 018d  .t.}.~..........
 00009270: 0190 0191 0193 0194 019d 01aa 01b3 0000  ................
 00009280: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00009290: 0000 0000 0000 0000 0000 0000 01b4 0000  ................
 000092a0: 000e 0070 006f 0073 0065 005f 0069 006d  ...p.o.s.e._.i.m
 000092b0: 0070 006f 0072 0074 0065 0072 0073 6d6f  .p.o.r.t.e.r.smo
-000092c0: 4444 626c 6f62 0000 0008 fa4c 7240 5f05  DDblob.....Lr@_.
+000092c0: 4444 626c 6f62 0000 0008 6a31 d652 7205  DDblob....j1.Rr.
 000092d0: c541 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
 000092e0: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
-000092f0: 0073 6d6f 6444 626c 6f62 0000 0008 fa4c  .smodDblob.....L
-00009300: 7240 5f05 c541 0000 000e 0070 006f 0073  r@_..A.....p.o.s
+000092f0: 0073 6d6f 6444 626c 6f62 0000 0008 6a31  .smodDblob....j1
+00009300: d652 7205 c541 0000 000e 0070 006f 0073  .Rr..A.....p.o.s
 00009310: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00009320: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
-00009330: 0000 0003 e000 0000 000e 0070 006f 0073  ...........p.o.s
+00009330: 0000 0004 e000 0000 000e 0070 006f 0073  ...........p.o.s
 00009340: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00009350: 0065 0072 0073 7653 726e 6c6f 6e67 0000  .e.r.svSrnlong..
 00009360: 0001 0000 000f 0070 006f 0073 0065 005f  .......p.o.s.e._
 00009370: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
 00009380: 0072 0073 6277 7370 626c 6f62 0000 00ca  .r.sbwspblob....
 00009390: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 000093a0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
@@ -2370,15 +2370,15 @@
 00009410: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 00009420: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 00009430: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00009440: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00009450: 0000 0000 0000 0000 009b 0000 000f 0070  ...............p
 00009460: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
 00009470: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
-00009480: 636f 6d70 0000 0000 0000 9838 0000 000f  comp.......8....
+00009480: 636f 6d70 0000 0000 0000 d9db 0000 000f  comp............
 00009490: 0070 006f 0073 0065 005f 0070 0072 006f  .p.o.s.e._.p.r.o
 000094a0: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
 000094b0: 7643 626c 6f62 0000 0297 6270 6c69 7374  vCblob....bplist
 000094c0: 3030 d801 0203 0405 0607 0809 0a0b 1949  00.............I
 000094d0: 4a0a 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
 000094e0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
 000094f0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
@@ -2458,22 +2458,22 @@
 00009990: 6101 6a01 6b01 6d01 6e01 7001 7901 7a01  a.j.k.m.n.p.y.z.
 000099a0: 7c01 7d01 7f01 8801 8901 8c01 8d01 8f01  |.}.............
 000099b0: 9801 9901 9a01 9c01 9d01 a601 ab00 0000  ................
 000099c0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
 000099d0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
 000099e0: 0f00 7000 6f00 7300 6500 5f00 7000 7200  ..p.o.s.e._.p.r.
 000099f0: 6f00 6300 6500 7300 7300 6f00 7200 736d  o.c.e.s.s.o.r.sm
-00009a00: 6f44 4462 6c6f 6200 0000 0892 deca 6739  oDDblob.......g9
-00009a10: 05c5 4100 0000 0f00 7000 6f00 7300 6500  ..A.....p.o.s.e.
+00009a00: 6f44 4462 6c6f 6200 0000 0837 66e7 e79f  oDDblob....7f...
+00009a10: 08c5 4100 0000 0f00 7000 6f00 7300 6500  ..A.....p.o.s.e.
 00009a20: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 00009a30: 6f00 7200 736d 6f64 4462 6c6f 6200 0000  o.r.smodDblob...
 00009a40: 0892 deca 6739 05c5 4100 0000 0f00 7000  ....g9..A.....p.
 00009a50: 6f00 7300 6500 5f00 7000 7200 6f00 6300  o.s.e._.p.r.o.c.
 00009a60: 6500 7300 7300 6f00 7200 7370 6831 5363  e.s.s.o.r.sph1Sc
-00009a70: 6f6d 7000 0000 0000 0100 0000 0000 0f00  omp.............
+00009a70: 6f6d 7000 0000 0000 0180 0000 0000 0f00  omp.............
 00009a80: 7000 6f00 7300 6500 5f00 7000 7200 6f00  p.o.s.e._.p.r.o.
 00009a90: 6300 6500 7300 7300 6f00 7200 7376 5372  c.e.s.s.o.r.svSr
 00009aa0: 6e6c 6f6e 6700 0000 0100 0000 0900 7200  nlong.........r.
 00009ab0: 6f00 6900 5f00 7400 6f00 6f00 6c00 7362  o.i._.t.o.o.l.sb
 00009ac0: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
 00009ad0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
 00009ae0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
@@ -2485,15 +2485,15 @@
 00009b40: 6562 6172 0808 0908 095f 1019 7b7b 3233  ebar....._..{{23
 00009b50: 322c 2031 3931 7d2c 207b 3133 3032 2c20  2, 191}, {1302, 
 00009b60: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
 00009b70: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
 00009b80: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 00009b90: 0000 0000 9b00 0000 0900 7200 6f00 6900  ..........r.o.i.
 00009ba0: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00009bb0: 6f6d 7000 0000 0000 042b 6f00 0000 0900  omp......+o.....
+00009bb0: 6f6d 7000 0000 0000 05d9 9100 0000 0900  omp.............
 00009bc0: 7200 6f00 6900 5f00 7400 6f00 6f00 6c00  r.o.i._.t.o.o.l.
 00009bd0: 736c 7376 4362 6c6f 6200 0002 7962 706c  slsvCblob...ybpl
 00009be0: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
 00009bf0: 0b16 4647 480a 5f10 1276 6965 774f 7074  ..FGH._..viewOpt
 00009c00: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
 00009c10: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00009c20: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -2528,15 +2528,15 @@
 00009df0: 0125 012a 0133 0134 0136 0137 013c 0145  .%.*.3.4.6.7.<.E
 00009e00: 0146 0148 0149 014f 0158 0159 015b 015c  .F.H.I.O.X.Y.[.\
 00009e10: 0164 016d 016e 0171 0172 017b 0184 0185  .d.m.n.q.r.{....
 00009e20: 0187 0188 0197 01a0 01a1 01a2 01ac 01ad  ................
 00009e30: 01b6 01bb 01c4 0000 0000 0000 0201 0000  ................
 00009e40: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
 00009e50: 0000 0000 01c5 7068 3153 636f 6d70 0000  ......ph1Scomp..
-00009e60: 0000 0002 0000 0000 000d 006f 0075 0074  ...........o.u.t
+00009e60: 0000 0002 5000 0000 000d 006f 0075 0074  ....P......o.u.t
 00009e70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
 00009e80: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 00009e90: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
 00009ea0: 006e 0067 6277 7370 626c 6f62 0000 00ca  .n.gbwspblob....
 00009eb0: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 00009ec0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 00009ed0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
@@ -2547,30 +2547,30 @@
 00009f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 00009f30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 00009f40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 00009f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00009f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00009f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 00009f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00009f90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+00009f90: 3153 636f 6d70 0000 0000 000c 8e04 0000  1Scomp..........
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000a000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
 0000a010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
 0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 6cfb  .smoDDblob....l.
 0000a030: e0c5 4905 c541 0000 0009 0072 006f 0069  ..I..A.....r.o.i
 0000a040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
 0000a050: 626c 6f62 0000 0008 6cfb e0c5 4905 c541  blob....l...I..A
 0000a060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
 0000a070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-0000a080: 0000 0005 2000 0000 0009 0072 006f 0069  .... ......r.o.i
+0000a080: 0000 0007 6000 0000 0009 0072 006f 0069  ....`......r.o.i
 0000a090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
 0000a0a0: 6c6f 6e67 0000 0001 0000 001b 0074 0068  long.........t.h
 0000a0b0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
 0000a0c0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
 0000a0d0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
 0000a0e0: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
 0000a0f0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
@@ -2585,16 +2585,16 @@
 0000a180: 2c20 3735 347d 7d09 0817 2531 3d49 606d  , 754}}...%1=I`m
 0000a190: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
 0000a1a0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 0000a1b0: 0000 0000 0000 9a00 0000 1b00 7400 6800  ............t.h.
 0000a1c0: 6900 7200 6400 5f00 7000 6100 7200 7400  i.r.d._.p.a.r.t.
 0000a1d0: 7900 5f00 6c00 6100 6200 6500 6c00 5f00  y._.l.a.b.e.l._.
 0000a1e0: 6100 7000 7000 6500 6e00 6400 6500 7200  a.p.p.e.n.d.e.r.
-0000a1f0: 736c 6731 5363 6f6d 7000 0000 0000 021c  slg1Scomp.......
-0000a200: 9000 0000 1b00 7400 6800 6900 7200 6400  ......t.h.i.r.d.
+0000a1f0: 736c 6731 5363 6f6d 7000 0000 0000 02fc  slg1Scomp.......
+0000a200: 7d00 0000 1b00 7400 6800 6900 7200 6400  }.....t.h.i.r.d.
 0000a210: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
 0000a220: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
 0000a230: 6500 6e00 6400 6500 7200 736c 7376 4362  e.n.d.e.r.slsvCb
 0000a240: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
 0000a250: 0102 0304 0506 0708 090a 0b16 4647 480a  ............FGH.
 0000a260: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
 0000a270: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
@@ -2676,25 +2676,25 @@
 0000a730: 0183 018c 018e 0191 0192 0193 0194 019d  ................
 0000a740: 01a2 01ab 0000 0000 0000 0201 0000 0000  ................
 0000a750: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
 0000a760: 0000 01ac 0000 001b 0074 0068 0069 0072  .........t.h.i.r
 0000a770: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
 0000a780: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
 0000a790: 0070 0065 006e 0064 0065 0072 0073 6d6f  .p.e.n.d.e.r.smo
-0000a7a0: 4444 626c 6f62 0000 0008 b989 9f32 1302  DDblob.......2..
+0000a7a0: 4444 626c 6f62 0000 0008 0094 71df a008  DDblob......q...
 0000a7b0: c541 0000 001b 0074 0068 0069 0072 0064  .A.....t.h.i.r.d
 0000a7c0: 005f 0070 0061 0072 0074 0079 005f 006c  ._.p.a.r.t.y._.l
 0000a7d0: 0061 0062 0065 006c 005f 0061 0070 0070  .a.b.e.l._.a.p.p
 0000a7e0: 0065 006e 0064 0065 0072 0073 6d6f 6444  .e.n.d.e.r.smodD
 0000a7f0: 626c 6f62 0000 0008 b989 9f32 1302 c541  blob.......2...A
 0000a800: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
 0000a810: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
 0000a820: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
 0000a830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
-0000a840: 6d70 0000 0000 0002 b000 0000 001b 0074  mp.............t
+0000a840: 6d70 0000 0000 0003 e000 0000 001b 0074  mp.............t
 0000a850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
 0000a860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
 0000a870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
 0000a880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
 0000a890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
 0000a8a0: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
 0000a8b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
@@ -2707,15 +2707,15 @@
 0000a920: 0809 5f10 197b 7b32 3332 2c20 3139 317d  .._..{{232, 191}
 0000a930: 2c20 7b31 3330 322c 2037 3134 7d7d 0908  , {1302, 714}}..
 0000a940: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
 0000a950: 0000 0000 0101 0000 0000 0000 000f 0000  ................
 0000a960: 0000 0000 0000 0000 0000 0000 009b 0000  ................
 0000a970: 0002 0075 0069 6473 636c 626f 6f6c 0000  ...u.idsclbool..
 0000a980: 0000 0200 7500 696c 6731 5363 6f6d 7000  ....u.ilg1Scomp.
-0000a990: 0000 0000 0bda 1600 0000 0200 7500 696c  ............u.il
+0000a990: 0000 0000 0fd1 9a00 0000 0200 7500 696c  ............u.il
 0000a9a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 0000a9b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 0000a9c0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
 0000a9d0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
 0000a9e0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
 0000a9f0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
 0000aa00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
@@ -2792,26 +2792,26 @@
 0000ae70: 019d 01a2 01ab 0000 0000 0000 0201 0000  ................
 0000ae80: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
 0000ae90: 0000 0000 01ac 0000 0002 0075 0069 6d6f  ...........u.imo
 0000aea0: 4444 626c 6f62 0000 0008 c9ff d919 c904  DDblob..........
 0000aeb0: c541 0000 0002 0075 0069 6d6f 6444 626c  .A.....u.imodDbl
 0000aec0: 6f62 0000 0008 c9ff d919 c904 c541 0000  ob...........A..
 0000aed0: 0002 0075 0069 7068 3153 636f 6d70 0000  ...u.iph1Scomp..
-0000aee0: 0000 000f 1000 546f 6f6c 6261 725b 5368  ......Toolbar[Sh
+0000aee0: 0000 0014 7000 546f 6f6c 6261 725b 5368  ....p.Toolbar[Sh
 0000aef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 0000af00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 0000af10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
 0000af20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 0000af30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 0000af40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 0000af50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 0000af60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 0000af70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 0000af80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-0000af90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+0000af90: 3153 636f 6d70 0000 0000 000c 8e04 0000  1Scomp..........
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
@@ -2830,15 +2830,15 @@
 0000b0d0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
 0000b0e0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
 0000b0f0: 0000 0000 0000 0000 0000 0000 009b 0000  ................
 0000b100: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
 0000b110: 0076 0069 0073 0065 0064 6473 636c 626f  .v.i.s.e.ddsclbo
 0000b120: 6f6c 0000 0000 0c00 7500 6e00 7300 7500  ol......u.n.s.u.
 0000b130: 7000 6500 7200 7600 6900 7300 6500 646c  p.e.r.v.i.s.e.dl
-0000b140: 6731 5363 6f6d 7000 0000 0000 060e 7e00  g1Scomp.......~.
+0000b140: 6731 5363 6f6d 7000 0000 0000 07a9 8700  g1Scomp.........
 0000b150: 0000 0c00 7500 6e00 7300 7500 7000 6500  ....u.n.s.u.p.e.
 0000b160: 7200 7600 6900 7300 6500 646c 7376 4362  r.v.i.s.e.dlsvCb
 0000b170: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
 0000b180: 0102 0304 0506 0708 0909 0b18 4647 4849  ............FGHI
 0000b190: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
 0000b1a0: 7465 735f 100f 7368 6f77 4963 6f6e 5072  tes_..showIconPr
 0000b1b0: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
@@ -2921,16 +2921,16 @@
 0000b680: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
 0000b690: 0064 6d6f 4444 626c 6f62 0000 0008 6269  .dmoDDblob....bi
 0000b6a0: 0543 3a05 c541 0000 000c 0075 006e 0073  .C:..A.....u.n.s
 0000b6b0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
 0000b6c0: 0064 6d6f 6444 626c 6f62 0000 0008 6269  .dmodDblob....bi
 0000b6d0: 0543 3a05 c541 0000 000c 0075 006e 0073  .C:..A.....u.n.s
 0000b6e0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-0000b6f0: 0064 7068 3153 636f 6d70 0000 0000 0007  .dph1Scomp......
-0000b700: 9000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+0000b6f0: 0064 7068 3153 636f 6d70 0000 0000 0009  .dph1Scomp......
+0000b700: b000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
 0000b710: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
 0000b720: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
 0000b730: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
 0000b740: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
 0000b750: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 0000b760: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 0000b770: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
@@ -2942,15 +2942,15 @@
 0000b7d0: 2c20 7b31 3330 322c 2037 3134 7d7d 0908  , {1302, 714}}..
 0000b7e0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
 0000b7f0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
 0000b800: 0000 0000 0000 0000 0000 0000 009b 005f  ..............._
 0000b810: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
 0000b820: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
 0000b830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
-0000b840: 6d70 0000 0000 0002 b000 0000 001b 0074  mp.............t
+0000b840: 6d70 0000 0000 0003 e000 0000 001b 0074  mp.............t
 0000b850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
 0000b860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
 0000b870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
 0000b880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
 0000b890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
 0000b8a0: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
 0000b8b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
@@ -2963,15 +2963,15 @@
 0000b920: 0809 5f10 197b 7b32 3332 2c20 3139 317d  .._..{{232, 191}
 0000b930: 2c20 7b31 3330 322c 2037 3134 7d7d 0908  , {1302, 714}}..
 0000b940: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
 0000b950: 0000 0000 0101 0000 0000 0000 000f 0000  ................
 0000b960: 0000 0000 0000 0000 0000 0000 009b 0000  ................
 0000b970: 0002 0075 0069 6473 636c 626f 6f6c 0000  ...u.idsclbool..
 0000b980: 0000 0200 7500 696c 6731 5363 6f6d 7000  ....u.ilg1Scomp.
-0000b990: 0000 0000 0bda 1600 0000 0200 7500 696c  ............u.il
+0000b990: 0000 0000 0fd1 9a00 0000 0200 7500 696c  ............u.il
 0000b9a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 0000b9b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 0000b9c0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
 0000b9d0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
 0000b9e0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
 0000b9f0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
 0000ba00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
@@ -3048,26 +3048,26 @@
 0000be70: 019d 01a2 01ab 0000 0000 0000 0201 0000  ................
 0000be80: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
 0000be90: 0000 0000 01ac 0000 0002 0075 0069 6d6f  ...........u.imo
 0000bea0: 4444 626c 6f62 0000 0008 c9ff d919 c904  DDblob..........
 0000beb0: c541 0000 0002 0075 0069 6d6f 6444 626c  .A.....u.imodDbl
 0000bec0: 6f62 0000 0008 c9ff d919 c904 c541 0000  ob...........A..
 0000bed0: 0002 0075 0069 7068 3153 636f 6d70 0000  ...u.iph1Scomp..
-0000bee0: 0000 000f 1000 546f 6f6c 6261 725b 5368  ......Toolbar[Sh
+0000bee0: 0000 0014 7000 546f 6f6c 6261 725b 5368  ....p.Toolbar[Sh
 0000bef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 0000bf00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 0000bf10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
 0000bf20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 0000bf30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 0000bf40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 0000bf50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 0000bf60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 0000bf70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 0000bf80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-0000bf90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+0000bf90: 3153 636f 6d70 0000 0000 000c 8e04 0000  1Scomp..........
 0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,27 +12,26 @@
 from simba.feature_extractors.perimeter_jit import jitted_hull
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, write_df, read_df
 
 
 class ExtractFeaturesFrom14bps(ConfigReader, FeatureExtractionMixin):
     """
-    Class for creating a hard-coded set of features from two animals with 7 tracked body-parts
-    each using pose-estimation. Results are stored in the `project_folder/csv/features_extracted`
-    directory of the SimBA project.
+    Extracts hard-coded set of features from pose-estimation data from two animals with 7 tracked body-parts each.
+    Results are stored in the `project_folder/csv/features_extracted` directory of the SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-
-    Notes
-    ----------
-    Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
+    .. note::
+       `Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+       `Expected pose configuration <https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/schematics/6.png>`_
+
+       .. image:: _static/img/pose_configurations/6.png
+          :width: 150
+          :align: center
 
     Examples
     ----------
     >>> feature_extractor = ExtractFeaturesFrom14bps(config_path='MyProjectConfig')
     >>> feature_extractor.run()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,26 @@
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 from simba.feature_extractors.perimeter_jit import jitted_hull
 
 class ExtractFeaturesFrom7bps(ConfigReader, FeatureExtractionMixin):
-    
     """
-    Class for creating a hard-coded set of features from single animals with 7 tracked body-parts
-    using pose-estimation. Results are stored in the `project_folder/csv/features_extracted`
-    directory of the SimBA project.
+    Extracts hard-coded set of features from pose-estimation data from single animals with 7 tracked body-parts.
+    Results are stored in the `project_folder/csv/features_extracted` directory of the SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-        
-    Notes
-    ----------
-    Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+    :parameter str config_path: path to SimBA project config file in Configparser format
+
+    .. note::
+      `Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`_.
+      `Expected pose configuration <https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/schematics/2.png>`_
+       .. image:: _static/img/pose_configurations/2.png
+          :width: 150
+          :align: center
 
     Examples
     ----------
     >>> feature_extractor = ExtractFeaturesFrom7bps(config_path='MyProjectConfig')
     >>> feature_extractor.run()
 
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import Formats
 
 
 class ExtractFeaturesFrom8bps2Animals(ConfigReader, FeatureExtractionMixin):
     """
-    Class for creating a hard-coded set of features from two animals with 4 pose-estimated body-parts.
-    Results are stored in the `project_folder/csv/features_extracted`
-    directory of the SimBA project
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    Extracts hard-coded set of features from pose-estimation data from two animals with 4 tracked body-parts each.
+    Results are stored in the `project_folder/csv/features_extracted` directory of the SimBA project.
+
+    :parameter str config_path: path to SimBA project config file in Configparser format
+
+    .. note::
+       `Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+       `Expected pose configuration <https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/schematics/5.png>`_
+
+       .. image:: _static/img/pose_configurations/5.png
+          :width: 150
+          :align: center
 
-    Notes
-    ----------
-    Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
 
     Examples
     ----------
     >>> feature_extractor = ExtractFeaturesFrom8bps2Animals(config_path='MyProjectConfig')
     >>> feature_extractor.run()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/perimeter_jit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 __author__ = "Simon Nilsson"
-### modified from https://stackoverflow.com/questions/74812556/computing-quick-convex-hull-using-numba/74817179#74817179
 
 import numpy as np
 from numba import njit, jit, prange
 from numba.np.extensions import cross2d
 
 @njit('(float32[:,:], int64[:], int64, int64)')
 def process(S, P, a, b):
@@ -12,21 +11,25 @@
     if len(K) == 0:
         return [a, b]
     c = P[np.argmax(signed_dist)]
     return process(S, K, a, c)[:-1] + process(S, K, c, b)
 
 @njit('(float32[:, :,:], types.unicode_type)', fastmath=True)
 def jitted_hull(points: np.ndarray, target: str = 'perimeter') -> np.ndarray:
-
     """
+    Compute attributes (e.g., perimeter or area) of a polygon.
+
     :param array points: 3d array FRAMESxBODY-PARTxCOORDINATE
     :param str target: Options [perimeter, area]
-    :return: 1d np.array
+    :return: 1d np.array representing perimeter length or area of polygon on each frame
+
+    .. note::
+    Modified from `Jérôme Richard <https://stackoverflow.com/questions/74812556/computing-quick-convex-hull-using-numba/74817179#74817179>`_
 
-    :EXAMPLE:
+    :example:
     >>> points = np.random.randint(1, 50, size=(50, 5, 2)).astype(float)
     >>> results = jitted_hull(points, target='area')
     """
 
     def perimeter(xy):
         perimeter = np.linalg.norm(xy[0] - xy[-1])
         for i in prange(xy.shape[0]-1):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_subsets.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,41 +16,35 @@
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 
 
 class FeatureSubsetsCalculator(ConfigReader, FeatureExtractionMixin):
+    """
+    Computes a subset of features from pose for non-ML downstream purposes.
+    E.g., returns the size of animal convex hull in each frame.
+
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str save_dir: directory where to store results.
+    :parameter str feature_family: Feature subtype to calculate. E.g., "Two-point body-part distances (mm)".
+
+    .. note::
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/feature_subsets.md>_`
+
+    Examples
+    ----------
+    >>> _ = FeatureSubsetsCalculator(config_path='project_folder/project_config.ini', feature_family='Frame-by-frame body-parts inside ROIs (Boolean)', save_dir='data').run()
+    """
+
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  save_dir: Union[str, os.PathLike],
                  feature_family: Literal[Options.FEATURE_SUBSET_OPTIONS]):
 
-        """
-        Computes frame-wise user-defined family subset of features from pose for non-ML downstream purposes.
-        E.g., returns the size of animal convex hull in each frame.
-
-        Parameters
-        ----------
-        config_path: str
-            path to SimBA project config file in Configparser format
-        save_dir: str
-            directory where to store results.
-        feature_family: str
-            Feature subtype to calculate
-
-        Notes
-        ----------
-        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/feature_subsets.md>_`
-
-        Examples
-        ----------
-        >>> _ = FeatureSubsetsCalculator(config_path='project_folder/project_config.ini', feature_family='Frame-by-frame body-parts inside ROIs (Boolean)', save_dir='data').run()
-        """
-
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
         check_if_filepath_list_is_empty(
             filepaths=self.outlier_corrected_paths,
             error_msg=f"SIMBA ERROR: Zero data files found in {self.outlier_corrected_paths} directory",
         )
         self.feature_family, self.save_dir = feature_family, save_dir
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,31 +9,26 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 from simba.utils.checks import check_str
 
 class UserDefinedFeatureExtractor(ConfigReader, FeatureExtractionMixin):
     """
-    Class for featurizing data within SimBA project using user-defined body-parts in the pose-estimation data.
+    Generic featurizer of data within SimBA project using user-defined body-parts in the pose-estimation data.
     Results are stored in the `project_folder/csv/features_extracted` directory of the SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
-    Notes
-    ----------
-    Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+    .. note::
+       `Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
 
     Examples
     ----------
     >>> feature_extractor = UserDefinedFeatureExtractor(config_path='MyProjectConfig')
     >>> feature_extractor.run()
-
     """
 
     def __init__(self,
                  config_path: str):
 
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.feature_extractors.perimeter_jit import jitted_hull
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 
 class ExtractFeaturesFrom16bps(ConfigReader, FeatureExtractionMixin):
     """
-    Class for creating a hard-coded set of features from two animals with 8 tracked body-parts
-    each using pose-estimation. Results are stored in the `project_folder/csv/features_extracted`
-    directory of the SimBA project
+    Extracts hard-coded set of features from pose-estimation data from two animals with 8 tracked body-parts each.
+    Results are stored in the `project_folder/csv/features_extracted` directory of the SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
-    Notes
-    ----------
-    Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+    .. note::
+       `Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+       `Expected pose configuration <https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/schematics/7.png>`_
+
+       .. image:: _static/img/pose_configurations/7.png
+          :width: 150
+          :align: center
 
     Examples
     ----------
     >>> feature_extractor = ExtractFeaturesFrom16bps(config_path='MyProjectConfig')
     >>> feature_extractor.run()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,38 +10,39 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.printing import SimbaTimer, stdout_success
 from simba.feature_extractors.perimeter_jit import jitted_hull
 
 
 class ExtractFeaturesFrom9bps(ConfigReader, FeatureExtractionMixin):
+
+    """
+    Extracts hard-coded set of features from pose-estimation data from single animals with 9 tracked body-parts.
+    Results are stored in the `project_folder/csv/features_extracted` directory of the SimBA project.
+
+    :parameter str config_path: path to SimBA project config file in Configparser format
+
+    .. note::
+       `Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+       `Expected pose configuration <https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/schematics/4.png>`_
+
+       .. image:: _static/img/pose_configurations/4.png
+          :width: 150
+          :align: center
+
+
+    Examples
+    ----------
+    >>> feature_extractor = ExtractFeaturesFrom9bps(config_path='MyProjectConfig')
+    >>> feature_extractor.run()
+    """
+
     def __init__(self,
                  config_path: str):
 
-        """
-        Class for creating a hard-coded set of features from one animal with 9 tracked body-parts
-        each using pose-estimation. Results are stored in the `project_folder/csv/features_extracted`
-        directory of the SimBA project.
-
-        Parameters
-        ----------
-        config_path: str
-            path to SimBA project config file in Configparser format
-
-        Notes
-        ----------
-        Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
-
-
-        Examples
-        ----------
-        >>> feature_extractor = ExtractFeaturesFrom9bps(config_path='MyProjectConfig')
-        >>> feature_extractor.run()
-        """
-
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
         self.in_headers = self.get_feature_extraction_headers(pose='1 animal 9 body-parts')
         self.mouse_p_headers = [x for x in self.in_headers if x[-2:] == '_p']
         self.mouse_headers = [x for x in self.in_headers if x[-2:] != '_p']
 
     def run(self):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.feature_extractors.perimeter_jit import jitted_hull
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 
 class ExtractFeaturesFrom8bps(ConfigReader, FeatureExtractionMixin):
     """
-    Class for creating a hard-coded set of features from single animals with 8 tracked body-parts
-    using pose-estimation. Results are stored in the `project_folder/csv/features_extracted`
-    directory of the SimBA project.
+    Extracts hard-coded set of features from pose-estimation data from single animals with 8 tracked body-parts.
+    Results are stored in the `project_folder/csv/features_extracted` directory of the SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
-    Notes
-    ----------
-    Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+    .. note::
+       `Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`_.
+       `Expected pose configuration <https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/schematics/3.png>`_
+        .. image:: _static/img/pose_configurations/3.png
+           :width: 150
+           :align: center
 
     Examples
     ----------
     >>> feature_extractor = ExtractFeaturesFrom8bps(config_path='MyProjectConfig')
     >>> feature_extractor.run()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 
 class ExtractFeaturesFrom4bps(ConfigReader, FeatureExtractionMixin):
     """
-    Class for creating a hard-coded set of features from single animals with 4 tracked body-parts
-    using pose-estimation. Results are stored in the `project_folder/csv/features_extracted`
-    directory of the SimBA project.
+    Extracts hard-coded set of features from pose-estimation data with one animal and 4 tracked body-parts.
+    Results are stored in the ``project_folder/csv/features_extracted`` directory of the SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-        
-    Notes
-    ----------
-    Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`__.
+    :parameter str config_path: path to SimBA project config file in Configparser format
+
+    .. note::
+       `Feature extraction tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-5-extract-features>`_.
+
+       `Expected pose configuration <https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/schematics/1.png>`_
+        .. image:: _static/img/pose_configurations/1.png
+           :width: 150
+           :align: center
 
     Examples
     ----------
     >>> feature_extractor = ExtractFeaturesFrom4bps(config_path='MyProjectConfig')
     >>> feature_extractor.run()
 
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.4/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/requirements.txt` & `Simba-UW-tf-dev-1.59.4/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.59.4/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.59.4/simba/mixins/config_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,25 @@
                                     read_config_file,
                                     find_core_cnt,
                                     get_all_clf_names)
 from simba.utils.checks import check_file_exist_and_readable
 
 
 class ConfigReader(object):
+    """
+    Methods for reading SimBA configparser.Configparser project config and associated project data
+
+    :param configparser.Configparser config_path: path to SimBA project_config.ini
+    :param bool read_video_info: if true, read the project_folder/logs/video_info.csv file.
+    """
+
     def __init__(self,
                  config_path: str,
                  read_video_info: bool = True):
 
-        """
-        Methods for reading SimBA configparser.Configparser project config and associated project data.
-
-        :param configparser.Configparser config_path: path to SimBA project_config.ini
-        :param bool read_video_info: if true, read the project_folder/logs/video_info.csv file.
-        """
-
         self.timer = SimbaTimer(start=True)
         self.config_path = config_path
         self.config = read_config_file(config_path=config_path)
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
         self.input_csv_dir = os.path.join(self.project_path, Paths.INPUT_CSV.value)
         self.features_dir = os.path.join(self.project_path, Paths.FEATURES_EXTRACTED_DIR.value)
@@ -110,28 +110,19 @@
         self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.multi_animal_id_list, self.animal_cnt, self.x_cols, self.y_cols, self.p_cols, self.clr_lst)
         self.project_bps = list(set([x[:-2] for x in self.bp_headers]))
         self.color_dict = get_color_dict()
         self.emojis = get_emojis()
         if read_video_info:
             self.video_info_df = self.read_video_info_csv(file_path=self.video_info_path)
 
-    def read_roi_data(self):
+    def read_roi_data(self) -> None:
         """
         Method to read in ROI definitions from SimBA project
-
-        Returns
-        -------
-        roi_df: dict
-        rectangles_df: pd.DataFrame
-        circles_df: pd.DataFrame
-        polygon_df: pd.DataFrame
-        shape_names: list
-        roi_dict: dict
-
         """
+
         if not os.path.isfile(self.roi_coordinates_path):
             raise NoROIDataError(msg='SIMBA ERROR: No ROI definitions were found in your SimBA project. Please draw some ROIs before analyzing your ROI data')
         else:
             self.rectangles_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_RECTANGLES.value).dropna(how='any')
             self.circles_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_CIRCLES.value).dropna(how='any')
             self.polygon_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_POLYGONS.value)
             if 'Center_XCenter_Y' in self.polygon_df.columns:
@@ -156,15 +147,21 @@
                 elif shape_type == Keys.ROI_RECTANGLES.value:
                     self.roi_dict[Keys.ROI_RECTANGLES.value]['Center_X'] = self.roi_dict[Keys.ROI_RECTANGLES.value]['Bottom_right_X'] - ((self.roi_dict[Keys.ROI_RECTANGLES.value]['Bottom_right_X'] - self.roi_dict[Keys.ROI_RECTANGLES.value]['width']) / 2)
                     self.roi_dict[Keys.ROI_RECTANGLES.value]['Center_Y'] = self.roi_dict[Keys.ROI_RECTANGLES.value]['Bottom_right_Y'] - ((self.roi_dict[Keys.ROI_RECTANGLES.value]['Bottom_right_Y'] - self.roi_dict[Keys.ROI_RECTANGLES.value]['height']) / 2)
                 elif shape_type == Keys.ROI_POLYGONS.value:
                     self.roi_dict[Keys.ROI_POLYGONS.value]['Center_X'] = self.roi_dict[Keys.ROI_POLYGONS.value]['Center_X']
                     self.roi_dict[Keys.ROI_POLYGONS.value]['Center_Y'] = self.roi_dict[Keys.ROI_POLYGONS.value]['Center_Y']
 
-    def get_all_clf_names(self):
+    def get_all_clf_names(self) -> List[str]:
+        """
+        Helper to return all classifier names in SimBA project
+
+        :return List[str]:
+        """
+
         model_names = []
         for i in range(self.clf_cnt):
             entry_name = 'target_name_{}'.format(str(i + 1))
             model_names.append(self.read_config_entry(self.config, ConfigKey.SML_SETTINGS.value, entry_name, data_type=Dtypes.STR.value))
         return model_names
 
     def insert_column_headers_for_outlier_correction(self,
@@ -214,15 +211,28 @@
                                                                             str(bp_missing)))
             raise ValueError()
         else:
             data_df.columns = new_headers
             return data_df
 
     def get_number_of_header_columns_in_df(self,
-                                           df: pd.DataFrame):
+                                           df: pd.DataFrame) -> int:
+
+        """
+        Helper to find the number of non-numerical rows at the top of a dataframe.
+
+        Parameters
+        ----------
+        data_df:  pd.DataFrame
+
+        Returns
+        -------
+        int
+        """
+
         for i in range(len(df)):
             try:
                 temp = df.iloc[i:].apply(pd.to_numeric).reset_index(drop=True)
                 return i
             except ValueError:
                 pass
         raise DataHeaderError(msg='Could find the count of header columns in dataframe')
@@ -239,31 +249,34 @@
         video_dir: str
             Directory holding putative video file
         filename: str
             Data file name, e.g., ``Video_1``.
 
         Returns
         -------
-        return_path: str
+        str
+
+        Raises
+        -------
+        NoFileFoundWarning: No video file is found.
 
         """
         try:
             all_files_in_video_folder = [f for f in next(os.walk(video_dir))[2] if not f[0] == '.']
         except StopIteration:
             raise NoFilesFoundError(msg=f'No files found in the {video_dir} directory')
         all_files_in_video_folder = [os.path.join(video_dir, x) for x in all_files_in_video_folder]
         return_path = None
         for file_path in all_files_in_video_folder:
             _, video_filename, ext = get_fn_ext(file_path)
             if ((video_filename == filename) and ((ext.lower() == '.mp4') or (ext.lower() == '.avi'))):
                 return_path = file_path
 
         if return_path is None:
-            NoFileFoundWarning(
-                f'SimBA could not find a video file representing {filename} in the project video directory')
+            NoFileFoundWarning(f'SimBA could not find a video file representing {filename} in the project video directory')
         return return_path
 
     def add_missing_ROI_cols(self,
                              shape_df: pd.DataFrame) -> pd.DataFrame:
         """
         Helper to add missing ROI definitions in ROI info dataframes created by the first version of the SimBA ROI
         user-interface but analyzed using newer versions of SimBA.
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.59.4/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi` & `Simba-UW-tf-dev-1.59.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.59.4/simba/mixins/feature_extraction_mixin.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,23 +21,23 @@
                                     read_video_info_csv,
                                     read_config_file,
                                     get_bp_headers)
 from simba.utils.errors import CountError
 import simba
 
 class FeatureExtractionMixin(object):
+    """
+    Methods for featurizing pose-estimation data.
+
+    :param configparser.Configparser config_path: path to SimBA project_config.ini
+    """
 
     def __init__(self,
                  config_path: Optional[str] = None):
 
-        """
-        Methods for featurizing pose-estimation data
-        :param configparser.Configparser config_path: path to SimBA project_config.ini
-        """
-
         if config_path:
             self.config_path = config_path
             self.config = read_config_file(config_path=config_path)
             self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
             self.video_info_path = os.path.join(self.project_path, Paths.VIDEO_INFO.value)
             self.video_info_df = read_video_info_csv(file_path=self.video_info_path)
             self.data_in_dir = os.path.join(self.project_path, Paths.OUTLIER_CORRECTED.value)
@@ -50,16 +50,24 @@
             self.files_found = glob.glob(self.data_in_dir + '/*.' + self.file_type)
             check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg=f'No files of type {self.file_type} found in {self.data_in_dir}')
             self.col_headers = get_bp_headers(body_parts_lst=self.body_parts_lst)
             self.col_headers_shifted = [bp + '_shifted' for bp in self.col_headers]
 
     @staticmethod
     @jit(nopython=True)
-    def euclidean_distance(bp_1_x_vals, bp_2_x_vals, bp_1_y_vals, bp_2_y_vals, px_per_mm):
-        series = (np.sqrt((bp_1_x_vals - bp_2_x_vals) ** 2 + (bp_1_y_vals - bp_2_y_vals) ** 2)) / px_per_mm
+    def euclidean_distance(bp_1_x: pd.Series,
+                           bp_2_x: pd.Series,
+                           bp_1_y: pd.Series,
+                           bp_2_y: pd.Series,
+                           px_per_mm: float) -> pd.Series:
+        """
+        Helper to compute the Euclidean distance in millimeters between two body-parts in all frames of a video
+        """
+
+        series = (np.sqrt((bp_1_x - bp_2_x) ** 2 + (bp_1_y - bp_2_y) ** 2)) / px_per_mm
         return series
 
 
     @staticmethod
     @jit(nopython=True, fastmath=True)
     def angle3pt(ax: float, ay: float, bx: float, by: float, cx: float, cy: float) -> float:
         """
@@ -72,16 +80,16 @@
 
     @staticmethod
     @jit(nopython=True, fastmath=True)
     def angle3pt_serialized(data: np.ndarray) -> np.ndarray:
         """
         Jitted helper for frame-wise 3-point angles.
 
-        data : ndarray
-            2D numerical array with frame number on x and [ax, ay, bx, by, cx, cy] on y.
+        :parameter ndarray data: 2D numerical array with frame number on x and [ax, ay, bx, by, cx, cy] on y.
+        :return ndarray: 2D numerical array with frame number on x and angle on y.
         """
 
         results = np.full((data.shape[0]), 0.0)
         for i in prange(data.shape[0]):
             angle = math.degrees(
                 math.atan2(data[i][5] - data[i][3], data[i][4] - data[i][2]) - math.atan2(data[i][1] - data[i][3], data[i][0] - data[i][2]))
             if angle < 0:
@@ -89,15 +97,20 @@
             results[i] = angle
 
         return results
 
     @staticmethod
     def convex_hull_calculator_mp(arr: np.ndarray, px_per_mm: float) -> float:
         """
-        Helper calculating single frame convex hull perimeter length. Call using ``parallel.delayed``.
+        Calculate single frame convex hull perimeter length in millimeters. For acceptable run-time,
+        Call using ``parallel.delayed``. For large data, use ``simba.feature_extractors.perimeter_jit.jitted_hull``.
+
+        :parameter np.ndarray arr: 2D array of size len(body-parts) x 2.
+        :parameter float px_per_mm: Video pixels per millimeter.
+        :return float: The length of the animal perimeter in millimeters.
         """
         arr = np.unique(arr, axis=0).astype(int)
         if arr.shape[0] < 3:
             return 0
         for i in range(1, arr.shape[0]):
             if (arr[i] != arr[0]).all():
                 try:
@@ -108,55 +121,65 @@
                 pass
         return 0
 
     @staticmethod
     @jit(nopython=True)
     def count_values_in_range(data: np.ndarray, ranges: np.ndarray) -> np.ndarray:
         """
-        Jitted helper finding count of values within data that falls within ranges. Returns np.ndarray of
-        size data.shape[0], ranges.shape[1].
+        Jitted helper finding count of values that falls within ranges. E.g., the number of pose-estimated
+        body-parts that fall within defined bracket of probabilities.
+
+        :parameter np.ndarray data: 2D numpy array with frames on X.
+        :parameter np.ndarray ranges: 2D numpy array representing the brackets. E.g., [[0, 0.1], [0.1, 0.5]]
+        :return np.ndarray: 2D numpy array of size data.shape[0], ranges.shape[1]
         """
+
         results = np.full((data.shape[0], ranges.shape[0]), 0)
         for i in prange(data.shape[0]):
             for j in prange(ranges.shape[0]):
                 lower_bound, upper_bound = ranges[j][0], ranges[j][1]
                 results[i][j] = data[i][np.logical_and(data[i] >= lower_bound, data[i] <= upper_bound)].shape[0]
         return results
 
     @staticmethod
     @jit(nopython=True)
     def framewise_euclidean_distance_roi(location_1: np.ndarray,
                                          location_2: np.ndarray,
                                          px_per_mm: float,
                                          centimeter: bool = False) -> np.ndarray:
         """
-        Jitted helper finding frame-wise distances between moving location (location_1) and static location (location_2)
-        in millimeter or centimeter.
+        Jitted helper finding frame-wise distances between a moving location (location_1) and
+        static location (location_2) in millimeter or centimeter.
+
+        :parameter ndarray location_1: 2D numpy array of size len(frames) x 2.
+        :parameter ndarray location_1: 1D numpy array holding the X and Y of the static location.
+        :parameter float px_per_mm: The pixels per millimeter in the video.
+        :parameter bool centimeter: If true, the value in centimeters is returned. Else the value in millimeters.
+
+        :return np.ndarray: 2D array of size location_1.shape[0] x 1.
+
         """
 
         results = np.full((location_1.shape[0]), np.nan)
         for i in prange(location_1.shape[0]):
             results[i] = np.linalg.norm(location_1[i] - location_2) / px_per_mm
         if centimeter:
             results = results / 10
         return results
 
     @staticmethod
     @jit(nopython=True)
     def framewise_inside_rectangle_roi(bp_location: np.ndarray,
                                        roi_coords: np.ndarray) -> np.ndarray:
         """
-        Jitted helper for frame-wise detection of animal is inside static rectangular ROI.
-        Returns boolean 1d ndarray.
-
-        bp_location: np.ndarray
-            2d numeric np.ndarray size len(frames) x 2
-        roi_coords:
-            2d numeric np.ndarray size 1x2 (top left, bottom right)
+        Jitted helper for frame-wise analysis if animal is inside static rectangular ROI.
 
+        :parameter np.ndarray bp_location:  2d numeric np.ndarray size len(frames) x 2
+        :parameter np.ndarray roi_coords: 2d numeric np.ndarray size 1x2 (top left[x, y], bottom right[x, y)
+        :return ndarray: 2d numeric boolean np.ndarray size len(frames) x 1 with 0 representing outside the rectangle and 1 representing inside the rectangle
         """
         results = np.full((bp_location.shape[0]), 0)
         within_x_idx = np.argwhere((bp_location[:, 0] <= roi_coords[1][0]) & (bp_location[:, 0] >= roi_coords[0][0])).flatten()
         within_y_idx = np.argwhere((bp_location[:, 1] <= roi_coords[1][1]) & (bp_location[:, 1] >= roi_coords[0][1])).flatten()
         for i in prange(within_x_idx.shape[0]):
             match = np.argwhere(within_y_idx == within_x_idx[i])
             if match.shape[0] > 0:
@@ -165,20 +188,21 @@
 
     @staticmethod
     @jit(nopython=True)
     def framewise_inside_polygon_roi(bp_location: np.ndarray,
                                      roi_coords: np.ndarray) -> np.ndarray:
 
         """
-        Jitted helper for frame-wise detection of animal is inside static polygon ROI.  Returns boolean 1d ndarray.
+        Jitted helper for frame-wise detection if animal is inside static polygon ROI.
+
+        :parameter np.ndarray bp_location:  2d numeric np.ndarray size len(frames) x 2
+        :parameter np.ndarray roi_coords: 2d numeric np.ndarray size len(polygon points) x 2
+
+        :return ndarray: 2d numeric boolean np.ndarray size len(frames) x 1 with 0 representing outside the polygon and 1 representing inside the polygon
 
-        bp_location: np.ndarray
-            2d numeric np.ndarray size len(frames) x 2
-        roi_coords:
-            2d numeric np.ndarray size len(polygon points) x 2
         """
         results = np.full((bp_location.shape[0]), 0)
         for i in prange(0, results.shape[0]):
             x, y, n = bp_location[i][0], bp_location[i][1], len(roi_coords)
             p2x, p2y, xints, inside = 0.0, 0.0, 0.0, False
             p1x, p1y = roi_coords[0]
             for j in prange(n + 1):
@@ -195,16 +219,24 @@
         return results
 
     def windowed_frequentist_distribution_tests(self,
                                                 data: np.ndarray,
                                                 feature_name: str,
                                                 fps: int) -> pd.DataFrame:
         """
-        Helper to compare (i) feature value distributions in 1-s sequential time-bins: Kolmogorov-Smirnov and T-tests,
-        (ii) compare feature values against a normal distribution: Shapiro, and (iii) find peak count in *rolling* 1s long feature window.
+        Calculates feature value distributions and feature peak counts in 1-s sequential time-bins.
+
+        Computes (i) feature value distributions in 1-s sequential time-bins: Kolmogorov-Smirnov and T-tests.
+        Computes (ii)  feature values against a normal distribution: Shapiro-Wilks.
+        Computes (iii) peak count in *rolling* 1s long feature window: scipy.find_peaks.
+
+        :parameter np.ndarray data: Single feature 2D array with frames on X.
+        :parameter np.ndarray feature_name: The name of the input feature.
+        :parameter int fps: The framerate of the video representing the data.
+        :return pd.DataFrame: Of size len(data) x 4 with columns representing KS, T, Shapiro-Wilks, and peak count statistics.
         """
 
         ks_results, = np.full((data.shape[0]), -1.0),
         t_test_results = np.full((data.shape[0]), -1.0)
         shapiro_results = np.full((data.shape[0]), -1.0)
         peak_cnt_results = np.full((data.shape[0]), -1.0)
 
@@ -232,45 +264,48 @@
 
     @staticmethod
     @jit(nopython=True, cache=True)
     def cdist(array_1: np.ndarray,
               array_2: np.ndarray) -> np.ndarray:
         """
         Jitted analogue of scipy.cdist.
+
+        :parameter np.ndarray array_1: 2D array of body-part coordinates
+        :parameter np.ndarray array_2: 2D array of body-part coordinates
+
+        :return np.ndarray: 2D array of euclidean distances between body-parts in ``array_1`` and ``array_2``
+
         """
         results = np.full((array_1.shape[0], array_2.shape[0]), np.nan)
         for i in prange(array_1.shape[0]):
             for j in prange(array_2.shape[0]):
                 results[i][j] = np.linalg.norm(array_1[i] - array_2[j])
         return results
 
     @staticmethod
     def create_shifted_df(df: pd.DataFrame) -> pd.DataFrame:
         """
-        Helper for creating df with duplicated shifted columns with ``_shifted`` suffix.
+        Create dataframe including duplicated shifted (1) columns with ``_shifted`` suffix.
+
+        :parameter pd.DataFrame df
+        :return pd.DataFrame: Dataframe including original and shifted columns.
         """
         data_df_shifted = df.shift(periods=1)
         data_df_shifted = data_df_shifted.combine_first(df).add_suffix('_shifted')
         return pd.concat([df, data_df_shifted], axis=1, join='inner').reset_index(drop=True)
 
     def check_directionality_viable(self):
         """
-        Helper to check if it is possible to calculate ``directionality`` statistics (i.e., nose, and ear coordinates from
-        pose estimation has to be present)
+        Check if it is possible to calculate ``directionality`` statistics
+        (i.e., nose, and ear coordinates from pose estimation has to be present)
 
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        directionalitySetting: bool
-        NoseCoords: list
-        EarLeftCoords: list
-        EarRightCoords: list
+        :return bool: If True, directionality is viable. Else, not viable.
+        :return np.ndarray nose_coord: If viable, then 2D array with coordinates of the nose in all frames. Else, empty array.
+        :return np.ndarray ear_left_coord: If viable, then 2D array with coordinates of the left ear in all frames. Else, empty array.
+        :return np.ndarray ear_right_coord: If viable, then 2D array with coordinates of the right ear in all frames. Else, empty array.
         """
 
         direction_viable = True
         nose_cords, ear_left_cords, ear_right_cords = [], [], []
         for animal_name in self.animal_bp_dict.keys():
             for bp_cord in ['X_bps', 'Y_bps']:
                 bp_list = self.animal_bp_dict[animal_name][bp_cord]
@@ -295,44 +330,48 @@
             ear_left_cords = [ear_left_cords[i * 2:(i + 1) * 2] for i in range((len(ear_left_cords) + 2 - 1) // 2)]
             ear_right_cords = [ear_right_cords[i * 2:(i + 1) * 2] for i in range((len(ear_right_cords) + 2 - 1) // 2)]
 
         return direction_viable, nose_cords, ear_left_cords, ear_right_cords
 
     def get_feature_extraction_headers(self,
                                        pose: str) -> List[str]:
-        """ Helper to return the headers names (body-part location columns) that should be used during feature extraction"""
+        """
+        Helper to return the headers names (body-part location columns) that should be used during feature extraction.
+
+        :parameter str pose: Pose-estimation setting, e.g., ``16``.
+        :return List[str]: The names and order of the pose-estimation columns.
+        """
         simba_dir = os.path.dirname(simba.__file__)
         feature_categories_csv_path = os.path.join(simba_dir, Paths.SIMBA_FEATURE_EXTRACTION_COL_NAMES_PATH.value)
         check_file_exist_and_readable(file_path=feature_categories_csv_path)
         bps = list(pd.read_csv(feature_categories_csv_path)[pose])
         return [x for x in bps if str(x) != 'nan']
 
     @staticmethod
     @jit(nopython=True)
     def jitted_line_crosses_to_nonstatic_targets(left_ear_array: np.ndarray,
                                                  right_ear_array: np.ndarray,
                                                  nose_array: np.ndarray,
                                                  target_array: np.ndarray) -> np.ndarray:
         """
-        Jitted helper to calculate if an animal is directing towards another animals body-part coordinate.
+        Jitted helper to calculate if an animal is directing towards another animals body-part coordinate,
+        given the target body-part and the left ear, right ear, and nose coordinates of the observer.
 
-        Parameters
-        ----------
-        left_ear_array: array
-            left ear coordinates of observing animal.
-        right_ear_array: array
-            right ear coordinates of observing animal.
-        nose_array: array
-            nose coordinates of observing animal.
-        target_array: array
-            The location of the target coordinates.
-
-        Returns
-        -------
-        np.array
+        :parameter np.ndarray left_ear_array: 2D array of size len(frames) x 2 with the coordinates of the observer animals left ear
+        :parameter np.ndarray right_ear_array: 2D array of size len(frames) x 2 with the coordinates of the observer animals right ear
+        :parameter np.ndarray nose_array: 2D array of size len(frames) x 2 with the coordinates of the observer animals nose
+        :parameter np.ndarray target_array: 2D array of size len(frames) x 2 with the target body-part location
+
+        :return np.ndarray: 2D array of size len(frames) x 4. First column represent the side of the observer that the target is in view. 0 = Left side, 1 = Right side, 2 = Not in view.
+        Second and third column represent the x and y location of the observer animals ``eye`` (half-way between the ear and the nose).
+        Fourth column represent if target is is view (bool).
+
+        .. note::
+           Input left ear, right ear, and nose coordinates of the observer is returned by
+           :meth:`simba.mixins.feature_extraction_mixin.FeatureExtractionMixin.check_directionality_viable`
         """
 
         results_array = np.zeros((left_ear_array.shape[0], 4))
         for frame_no in prange(results_array.shape[0]):
             Px = np.abs(left_ear_array[frame_no][0] - target_array[frame_no][0])
             Py = np.abs(left_ear_array[frame_no][1] - target_array[frame_no][1])
             Qx = np.abs(right_ear_array[frame_no][0] - target_array[frame_no][0])
@@ -354,31 +393,29 @@
     @staticmethod
     @jit(nopython=True)
     def jitted_line_crosses_to_static_targets(left_ear_array: np.ndarray,
                                               right_ear_array: np.ndarray,
                                               nose_array: np.ndarray,
                                               target_array: np.ndarray) -> np.ndarray:
         """
-        Jitted helper to calculate if an animal is directing towards a static coordinate
-        (e.g., the center of a user-defined ROI)
+        Jitted helper to calculate if an animal is directing towards a static location (ROI centroid),
+        given the target location and the left ear, right ear, and nose coordinates of the observer.
 
-        Parameters
-        ----------
-        left_ear_array: array
-            left ear coordinates of observing animal.
-        right_ear_array: array
-            right ear coordinates of observing animal.
-        nose_array: array
-            nose coordinates of observing animal.
-        target_array: array
-            The location of the target coordinates.
-
-        Returns
-        -------
-        np.array
+        :parameter np.ndarray left_ear_array: 2D array of size len(frames) x 2 with the coordinates of the observer animals left ear
+        :parameter np.ndarray right_ear_array: 2D array of size len(frames) x 2 with the coordinates of the observer animals right ear
+        :parameter np.ndarray nose_array: 2D array of size len(frames) x 2 with the coordinates of the observer animals nose
+        :parameter np.ndarray target_array: 2D array of size len(frames) x 2 with the target location
+
+        :return np.ndarray: 2D array of size len(frames) x 4. First column represent the side of the observer that the target is in view. 0 = Left side, 1 = Right side, 2 = Not in view.
+        Second and third column represent the x and y location of the observer animals ``eye`` (half-way between the ear and the nose).
+        Fourth column represent if target is is view (bool).
+
+        .. note::
+           Input left ear, right ear, and nose coordinates of the observer is returned by
+           :meth:`simba.mixins.feature_extraction_mixin.FeatureExtractionMixin.check_directionality_viable`
         """
 
         results_array = np.zeros((left_ear_array.shape[0], 4))
         for frame_no in range(results_array.shape[0]):
             Px = np.abs(left_ear_array[frame_no][0] - target_array[0])
             Py = np.abs(left_ear_array[frame_no][1] - target_array[1])
             Qx = np.abs(right_ear_array[frame_no][0] - target_array[0])
@@ -399,15 +436,22 @@
 
 
     def minimum_bounding_rectangle(self,
                                    points: np.ndarray) -> np.ndarray:
 
         """
         Finds the minimum bounding rectangle of a convex hull perimeter.
-        https://stackoverflow.com/questions/13542855/algorithm-to-find-the-minimum-area-rectangle-for-given-points-in-order-to-comput
+
+        :parameter np.ndarray points: 2D array representing the convexhull vertices of the animal.
+        :return np.ndarray: 2D array representing minimum bounding rectangle of the convexhull vertices of the animal.
+
+        .. note::
+           Modified from `JesseBuesking <https://stackoverflow.com/questions/13542855/algorithm-to-find-the-minimum-area-rectangle-for-given-points-in-order-to-comput>`_
+
+           See :meth:`simba.mixins.feature_extractors.perimeter_jit.jitted_hull` for computing the convexhull vertices.
 
         TODO: Place in numba njit.
         """
 
         pi2 = np.pi / 2.
         hull_points = points[ConvexHull(points).vertices]
         edges = hull_points[1:] - hull_points[:-1]
@@ -435,75 +479,86 @@
     @staticmethod
     @jit(nopython=True)
     def framewise_euclidean_distance(location_1: np.ndarray,
                                      location_2: np.ndarray,
                                      px_per_mm: float,
                                      centimeter: bool = False) -> np.ndarray:
         """
-        Jitted helper finding frame-wise distances between two non-static locations in millimeter or centimeter.
+        Jitted helper finding frame-wise distances between two moving locations in millimeter or centimeter.
+
+        :parameter ndarray location_1: 2D array of size len(frames) x 2.
+        :parameter ndarray location_1: 2D array of size len(frames) x 2.
+        :parameter float px_per_mm: The pixels per millimeter in the video.
+        :parameter bool centimeter: If true, the value in centimeters is returned. Else the value in millimeters.
+
+        :return np.ndarray: 2D array of size location_1.shape[0] x 1.
         """
+
         results = np.full((location_1.shape[0]), np.nan)
         for i in prange(location_1.shape[0]):
             results[i] = np.linalg.norm(location_1[i] - location_2[i]) / px_per_mm
         if centimeter:
             results = results / 10
         return results
 
     def dataframe_gaussian_smoother(self,
                                     df: pd.DataFrame,
                                     fps: int,
                                     time_window: int=100) -> pd.DataFrame:
         """
-        Helper performing column-wise Gaussian smoothing of dataframe.
+        Column-wise Gaussian smoothing of dataframe.
+
+        :parameter pd.DataFrame df: Dataframe with un-smoothened data.
+        :parameter int fps: The frame-rate of the video representing the data.
+        :parameter int time_window: Time-window in milliseconds to use for Gaussian smoothing.
+        :return pd.DataFrame: Dataframe with smoothened data
         """
 
         frames_in_time_window = int(time_window / (1000 / fps))
         for c in df.columns:
             df[c] = df[c].rolling(window=int(frames_in_time_window), win_type='gaussian', center=True).mean(std=5).fillna(df[c]).abs()
         return df
 
 
     def dataframe_savgol_smoother(self,
                                   df: pd.DataFrame,
                                   fps: int,
-                                  time_window: int = 150):
+                                  time_window: int = 150) -> pd.DataFrame:
+        """
+        Column-wise Savitzky-Golay smoothing of dataframe.
+
+        :parameter pd.DataFrame df: Dataframe with un-smoothened data.
+        :parameter int fps: The frame-rate of the video representing the data.
+        :parameter int time_window: Time-window in milliseconds to use for Gaussian smoothing.
+        :return pd.DataFrame: Dataframe with smoothened data
         """
-         Helper performing column-wise Savitzky-Golay smoothing of dataframe.
-         """
         frames_in_time_window = int(time_window / (1000 / fps))
         if (frames_in_time_window % 2) == 0: frames_in_time_window = frames_in_time_window - 1
         if (frames_in_time_window % 2) <= 3: frames_in_time_window = 5
         for c in df.columns:
             df[c] = savgol_filter(x=df[c].to_numpy(), window_length=frames_in_time_window, polyorder=3, mode='nearest')
         return df
 
-    def get_bp_headers(self):
+    def get_bp_headers(self) -> None:
         """
         Helper to create ordered list of all column header fields for SimBA project dataframes.
         """
         self.col_headers = []
         for bp in self.body_parts_lst:
             c1, c2, c3 = (f'{bp}_x', f'{bp}_y', f'{bp}_p')
             self.col_headers.extend((c1, c2, c3))
 
     def check_directionality_cords(self) -> dict:
 
         """
         Helper to check if ear and nose body-parts are present within the pose-estimation data.
 
-        Parameters
-        ----------
-        animal_bp_dict: dict
-            Python dictionary created by ``create_body_part_dictionary``.
-
-        Returns
-        -------
-        dict
-            body-part names of ear and nose body-parts as values and animal names as keys. If empty,
+        :return dict: Body-part names of ear and nose body-parts as values and animal names as keys. If empty,
             ear and nose body-parts are not present within the pose-estimation data
+
         """
         results = {}
         for animal in self.animal_bp_dict.keys():
             results[animal] = {}
             results[animal]['Nose'] = {}
             results[animal]['Ear_left'] = {}
             results[animal]['Ear_right'] = {}
@@ -524,49 +579,45 @@
         return results
 
     def insert_default_headers_for_feature_extraction(self,
                                                       df: pd.DataFrame,
                                                       headers: List[str],
                                                       pose_config: str,
                                                       filename: str) -> pd.DataFrame:
+        """
+        Helper to insert correct body-part column names prior to defualt feature extraction methods.
+        """
         if len(headers) != len(df.columns):
             raise CountError(f'Your SimBA project is set to using the default {pose_config} pose-configuration. '
                              f'SimBA therefore expects {str(len(headers))} columns of data inside the files within the project_folder. However, '
                              f'within file {filename} file, SimBA found {str(len(df.columns))} columns.')
         else:
             df.columns = headers
             return df
 
     @staticmethod
     def line_crosses_to_static_targets(p: List[float],
                                        q: List[float],
                                        n: List[float],
                                        M: List[float],
-                                       coord: List[float]):
+                                       coord: List[float]) -> (bool, List[float]):
         """
-        Legacy non-jitted helper to calculate if an animal is directing towards a coordinate.
-        For improved runtime, use ``simba.mixins.feature_extraction_mixin.jitted_line_crosses_to_static_targets``
+        Legacy non-jitted helper to calculate if an animal is directing towards a static coordinate (e.g., ROI centroid).
+
+        .. note:
+           For improved runtime, use :meth:`simba.mixins.feature_extraction_mixin.jitted_line_crosses_to_static_targets`
+
+        :parameter list p: left ear coordinates of observing animal.
+        :parameter list q: right ear coordinates of observing animal.
+        :parameter list n: nose coordinates of observing animal.
+        :parameter list M: The location of the target coordinates.
+        :parameter list coord: empty list to store the eye coordinate of the observing animal.
 
-        Parameters
-        ----------
-        p: list
-            left ear coordinates of observing animal.
-        q: list
-            right ear coordinates of observing animal.
-        n: list
-            nose coordinates of observing animal.
-        M: list
-            The location of the target coordinates.
-        coord: list
-            empty list to store the eye coordinate of the observing animal.
-
-        Returns
-        -------
-        bool
-        coord: list
+        :return bool: If True, static coordinate is in view.
+        :return List: If True, the coordinate of the observing animals ``eye`` (half-way between nose and ear).
         """
 
         Px = np.abs(p[0] - M[0])
         Py = np.abs(p[1] - M[1])
         Qx = np.abs(q[0] - M[0])
         Qy = np.abs(q[1] - M[1])
         Nx = np.abs(n[0] - M[0])
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.59.4/simba/mixins/plotting_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,20 +23,16 @@
 import simba
 from simba.utils.lookups import get_color_dict, get_named_colors
 from simba.utils.read_write import get_fn_ext
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import Formats, Options
 
 class PlottingMixin(object):
-    def __init__(self):
-
-        """
-        Methods for plotting
-        """
 
+    def __init__(self):
         pass
 
     def create_gantt_img(self,
                          bouts_df: pd.DataFrame,
                          clf_name: str,
                          image_index: int,
                          fps: int,
@@ -1031,21 +1027,19 @@
 
         fourcc, font = cv2.VideoWriter_fourcc(*'mp4v'), cv2.FONT_HERSHEY_COMPLEX
         cap = cv2.VideoCapture(video_path)
         group = data['group'].iloc[0]
         start_frm, current_frm, end_frm = data.index[0], data.index[0], data.index[-1]
         video_save_path = os.path.join(video_save_dir, '{}.mp4'.format(str(group)))
         if gantt_setting is not None:
-            writer = cv2.VideoWriter(video_save_path, fourcc, video_meta_data['fps'], (
-            int(video_meta_data['width'] + final_gantt.shape[1]), int(video_meta_data['height'])))
+            writer = cv2.VideoWriter(video_save_path, fourcc, video_meta_data['fps'], (int(video_meta_data['width'] + final_gantt.shape[1]), int(video_meta_data['height'])))
         else:
-            writer = cv2.VideoWriter(video_save_path, fourcc, video_meta_data['fps'],
-                                     (video_meta_data['width'], video_meta_data['height']))
-        cap.set(1, start_frm)
+            writer = cv2.VideoWriter(video_save_path, fourcc, video_meta_data['fps'], (video_meta_data['width'], video_meta_data['height']))
 
+        cap.set(1, start_frm)
         while current_frm < end_frm:
             clf_frm_cnt = np.sum(clf_data[0:current_frm])
             ret, img = cap.read()
             if settings['pose']:
                 for animal_cnt, (animal_name, animal_data) in enumerate(bp_dict.items()):
                     for bp_cnt, bp in enumerate(range(len(animal_data['X_bps']))):
                         x_header, y_header = animal_data['X_bps'][bp], animal_data['Y_bps'][bp]
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.59.4/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.59.4/simba/mixins/train_model_mixin.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,15 +24,19 @@
 import configparser
 import platform
 from sklearn.utils import parallel_backend
 import pickle
 from dtreeviz.trees import tree, dtreeviz
 import matplotlib.pyplot as plt
 import multiprocessing
-from typing import List, Optional
+from typing import List, Optional, Union, Dict, Any
+try:
+    from typing import Literal
+except:
+    from typing_extensions import Literal
 
 from simba.utils.enums import ConfigKey, Dtypes, MetaKeys, Defaults
 from simba.plotting.shap_agg_stats_visualizer import ShapAggregateStatisticsVisualizer
 from simba.utils.data import detect_bouts, create_color_palette
 from simba.utils.read_write import find_core_cnt, get_memory_usage_of_df, read_config_entry, read_df, get_fn_ext
 from simba.utils.checks import (check_int,
                                 check_str,
@@ -54,39 +58,28 @@
 
 
 plt.switch_backend('agg')
 
 class TrainModelMixin(object):
     def __init__(self):
         pass
-    """
-    Methods for training and evaluating classifiers.
-    """
 
     def read_all_files_in_folder(self,
                                  file_paths: List[str],
                                  file_type: str,
                                  classifier_names: Optional[List[str]] = None) -> pd.DataFrame:
         """
-        Helper function to read in all data files in a folder to a single pd.DataFrame for downstream ML algorithm.
-        Asserts that all classifiers have annotation fields present in concatenated dataframes.
+        Read in all data files in a folder to a single pd.DataFrame for downstream ML algo.
+        Asserts that all classifiers have annotation fields present in concatenated dataframe.
 
-        Parameters
-        ----------
-        file_paths: list
-            List of file paths representing files to be read in.
-        file_type: str
-            Type of files in ``file_paths``. OPTIONS: csv or parquet.
-        classifier_names: list or None
-            List of classifier names representing fields of human annotations. If not None, then assert that classifier names
+        :parameter List[str] file_paths: List of file paths representing files to be read in.
+        :parameter str file_type: List of file paths representing files to be read in.
+        :parameter str or None classifier_names: List of classifier names representing fields of human annotations. If not None, then assert that classifier names
             are present in each data file.
-
-        Returns
-        -------
-        df_concat: pd.DataFrame
+        :return pd.DataFrame: concatenated dataframe if all data represented in ``file_paths``.
 
         """
 
         timer = SimbaTimer()
         timer.start_timer()
         df_concat = pd.DataFrame()
         for file_cnt, file in enumerate(file_paths):
@@ -115,30 +108,22 @@
         print(f'Dataset size: {memory_size["megabytes"]}MB / {memory_size["gigabytes"]}GB')
         print('{} file(s) read (elapsed time: {}s) ...'.format(str(len(file_paths)), timer.elapsed_time_str))
         return df_concat.astype(np.float32)
 
     def read_in_all_model_names_to_remove(self,
                                           config: configparser.ConfigParser,
                                           model_cnt: int,
-                                          clf_name: str):
+                                          clf_name: str) -> List[str]:
         """
-        Helper to find all field names that contain annotations but are not the target.
+        Helper to find all field names that are annotations but are not the target.
 
-        Parameters
-        ----------
-        config: Configparser,
-            Configparser object holding data from the project_config.ini
-        model_cnt: int,
-            Number of classifiers in the SimBA project.
-        clf_name
-            Name of the classifier.
-
-        Returns
-        -------
-        annotation_cols_to_remove: list
+        :parameter configparser.ConfigParser config: Configparser object holding data from the project_config.ini
+        :parameter int model_cnt: Number of classifiers in the SimBA project
+        :parameter str clf_name: Name of the classifier.
+        :return List[str]: List of non-target annotation column names.
         """
 
         annotation_cols_to_remove = []
         for model_no in range(model_cnt):
             model_name = config.get(ConfigKey.SML_SETTINGS.value, 'target_name_' + str(model_no + 1))
             if model_name != clf_name:
                 annotation_cols_to_remove.append(model_name)
@@ -146,74 +131,55 @@
 
     def delete_other_annotation_columns(self,
                                         df: pd.DataFrame,
                                         annotations_lst: List[str]) -> pd.DataFrame:
         """
         Helper to delete fields that contain annotations which are not the target.
 
-        Parameters
-        ----------
-        df: pd.DataFrame
-            pandas Dataframe holding features and annotations.
-        annotations_lst: list
-            Column fields to be removed from df
-
-        Returns
-        -------
-        df: pd.DataFrame
+        :parameter pd.DataFrame df: Dataframe holding features and annotations.
+        :parameter List[str] annotations_lst: column fields to be removed from df
+        :return pd.DataFrame: Dataframe without non-target annotation columns
         """
 
         for a_col in annotations_lst:
             df = df.drop([a_col], axis=1)
         return df
 
     def split_df_to_x_y(self,
                         df: pd.DataFrame,
                         clf_name: str) -> (pd.DataFrame, pd.DataFrame):
         """
         Helper to split dataframe into features and target.
 
-        Parameters
-        ----------
-        df: pd.DataFrame
-            pandas Dataframe holding features and annotations.
-        clf_name: str
-            Name of target.
-
-        Returns
-        -------
-        df: pd.DataFrame
-        y: pd.DataFrame
+        :parameter pd.DataFrame df: Dataframe holding features and annotations.
+        :parameter str clf_name: Name of target.
+
+        :return pd.DataFrame: features
+        :return pd.DataFrame: target
         """
 
         df = deepcopy(df)
         y = df.pop(clf_name)
         return df, y
 
     def random_undersampler(self,
                             x_train: np.ndarray,
                             y_train: np.ndarray,
                             sample_ratio: float) -> (pd.DataFrame, pd.DataFrame):
         """
-        Helper to perform random undersampling of behavior-absent frames in a dataframe.
+        Helper to perform random under-sampling of behavior-absent frames in a dataframe.
 
-        Parameters
-        ----------
-        x_train: pd.DataFrame
-            Features in train set
-        y_train: pd.DataFrame
-            Target in train set
-        sample_ratio: float,
-            Ratio of behavior-absent frames to keep relative to the behavior-present frames. E.g., ``1.0`` returns an equal
+        :parameter np.ndarray x_train: Features in train set
+        :parameter np.ndarray y_train: Target in train set
+        :parameter float sample_ratio: Ratio of behavior-absent frames to keep relative to the behavior-present frames. E.g., ``1.0`` returns an equal
             count of behavior-absent and behavior-present frames. ``2.0`` returns twice as many behavior-absent frames as
             and behavior-present frames.
 
-        Returns
-        -------
-        df: pd.DataFrame
+        :return pd.DataFrame: Under-sampled feature-set
+        :return pd.DataFrame: Under-sampled target-set
         """
 
         print(f'Performing under-sampling at sample ratio {str(sample_ratio)}...')
         data_df = pd.concat([x_train, y_train], axis=1)
         present_df, absent_df = data_df[data_df[y_train.name] == 1], data_df[data_df[y_train.name] == 0]
         ratio_n = int(len(present_df) * sample_ratio)
         if len(absent_df) < ratio_n:
@@ -224,99 +190,68 @@
 
     def smoteen_oversampler(self,
                             x_train: pd.DataFrame,
                             y_train: pd.DataFrame,
                             sample_ratio: float) -> (np.ndarray, np.ndarray):
 
         """
-        Helper to perform smoteen oversampling of behavior-present frames in a dataframe
+        Helper to perform SMOTEEN oversampling of behavior-present annotations.
 
-        Parameters
-        ----------
-        x_train: pd.DataFrame or array
-            pandas Dataframe holding features and annotations.
-        y_train: pd.DataFrame or array
-            List of column fields to be removed from df
-        sample_ratio:
-            New behavior-present frames.
-
-        Returns
-        -------
-        x_train: array
-        y_train: array
+        :parameter np.ndarray x_train: Features in train set
+        :parameter np.ndarray y_train: Target in train set
+        :parameter float sample_ratio: Over-sampling ratio
+        :return np.ndarray: Oversampled features.
+        :return np.ndarray: Oversampled target.
 
         """
 
         print('Performing SMOTEEN oversampling...')
         smt = SMOTEENN(sampling_strategy=sample_ratio)
         return smt.fit_sample(x_train, y_train)
 
     def smote_oversampler(self,
                           x_train: pd.DataFrame or np.array,
                           y_train: pd.DataFrame or np.array,
                           sample_ratio: float) -> (np.ndarray, np.ndarray):
         """
-        Helper to perform smote oversampling of behavior-present frames in a dataframe
+        Helper to perform SMOTE oversampling of behavior-present annotations.
 
-        Parameters
-        ----------
-        x_train: pd.DataFrame or array
-            pandas Dataframe holding features and annotations.
-        y_train: pd.DataFrame or array
-            List of column fields to be removed from df
-        sample_ratio:
-            New behavior-present frames.
-
-        Returns
-        -------
-        x_train: array
-        y_train: array
+        :parameter np.ndarray x_train: Features in train set
+        :parameter np.ndarray y_train: Target in train set
+        :parameter float sample_ratio: Over-sampling ratio
+        :return np.ndarray: Oversampled features.
+        :return np.ndarray: Oversampled target.
 
         """
         print('Performing SMOTE oversampling...')
         smt = SMOTE(sampling_strategy=sample_ratio)
         return smt.fit_sample(x_train, y_train)
 
     def calc_permutation_importance(self,
                                     x_test: np.ndarray,
                                     y_test: np.ndarray,
                                     clf: RandomForestClassifier,
                                     feature_names: List[str],
                                     clf_name: str,
-                                    save_dir: str,
-                                    save_file_no: Optional[int] = None):
+                                    save_dir: Union[str, os.PathLike],
+                                    save_file_no: Optional[int] = None) -> None:
         """
         Helper to calculate feature permutation importance scores.
 
-        Parameters
-        ----------
-        x_test: np.array,
-            Array holding feature test data
-        y_test: np.array
-            Array holding target test data
-        clf: object
-            sklearn RandomForestClassifier object
-        feature_names: list,
-            list of feature names
-        clf_name: str,
-            Name of classifier
-        save_dir: str,
-            Directory where to save output in csv file format.
-        save_file_no: int or None.
-            If integer, represents the count of the classifier within a grid search. If none, the classifier is not
-            part of a grid search.
-
-        Returns
-        -------
-        None
+        :parameter np.ndarray x_test: feature test data
+        :parameter np.ndarray y_test: target test data
+        :parameter RandomForestClassifier clf: random forest classifier
+        :parameter List[str] feature_names: Names of features
+        :parameter str clf_name: Name of classifier.
+        :parameter str save_dir: Directory where to save results
+        :parameter Optional[int] save_file_no: If permutation importance calculation is part of a grid search, provide integer representing sequence.
 
         """
         print('Calculating feature permutation importances...')
-        timer = SimbaTimer()
-        timer.start_timer()
+        timer = SimbaTimer(start=True)
         p_importances = permutation_importance(clf, x_test, y_test, n_repeats=10, random_state=0)
         df = pd.DataFrame(
             np.column_stack([feature_names, p_importances.importances_mean, p_importances.importances_std]),
             columns=['FEATURE_NAME', 'FEATURE_IMPORTANCE_MEAN', 'FEATURE_IMPORTANCE_STDEV'])
         df = df.sort_values(by=['FEATURE_IMPORTANCE_MEAN'], ascending=False)
         if save_file_no != None:
             save_file_path = os.path.join(save_dir,
@@ -335,38 +270,23 @@
                             tt_size: float,
                             rf_clf: RandomForestClassifier,
                             save_dir: str,
                             save_file_no: Optional[int] = None) -> None:
         """
         Helper to compute random forest learning curves with cross-validation.
 
-        Parameters
-        ----------
-        x_y_df: pd.DataFrame
-            Pandas dataframe holding features and targets.
-        clf_name: str,
-            Name of the classifier
-        shuffle_splits: int
-            Number of cross-validation datasets at each data split.
-        dataset_splits: int
-            Number of data splits.
-        tt_size: float
-            dataset test size.
-        rf_clf: RandomForestClassifier
-            sklearn RandomForestClassifier object.
-        save_dir: str,
-            Directory where to save output in csv file format.
-        save_file_no: int or None.
-            If integer, represents the count of the classifier within a grid search. If none, the classifier is not
+        :parameter pd.DataFrame x_y_df: dataframe holding features and targets.
+        :parameter str clf_name: Name of the classifier
+        :parameter int shuffle_splits: Number of cross-validation datasets at each data split.
+        :parameter int dataset_splits: Number of data splits.
+        :parameter float tt_size: test size
+        :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object
+        :parameter str save_dir: Directory where to save output in csv file format.
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
-
-        Returns
-        -------
-        None
-
         """
 
         print('Calculating learning curves...')
         timer = SimbaTimer(start=True)
         x_df, y_df = self.split_df_to_x_y(x_y_df, clf_name)
         cv = ShuffleSplit(n_splits=shuffle_splits, test_size=tt_size)
         if platform.system() == "Darwin":
@@ -401,39 +321,25 @@
                       y_df: pd.DataFrame,
                       clf_name: str,
                       save_dir: str,
                       save_file_no: Optional[int] = None)  -> None:
         """
         Helper to compute random forest precision-recall curve.
 
-        Parameters
-        ----------
-        rf_clf: RandomForestClassifier
-            sklearn RandomForestClassifier object.
-        x_df: pd.DataFrame
-            Pandas dataframe holding test features.
-        y_df: pd.DataFrame
-            Pandas dataframe holding test target.
-        clf_name: str
-            Classifier name.
-        save_dir: str,
-            Directory where to save output in csv file format.
-        save_file_no: int or None.
-            If integer, represents the count of the classifier within a grid search. If none, the classifier is not
+        :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object.
+        :parameter pd.DataFrame x_df: Pandas dataframe holding test features.
+        :parameter pd.DataFrame y_df: Pandas dataframe holding test target.
+        :parameter str clf_name: Classifier name.
+        :parameter str save_dir: Directory where to save output in csv file format.
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
-
-        Returns
-        -------
-        None
-
         """
 
         print('Calculating PR curves...')
-        timer = SimbaTimer()
-        timer.start_timer()
+        timer = SimbaTimer(start=True)
         p = rf_clf.predict_proba(x_df)[:, 1]
         precision, recall, thresholds = precision_recall_curve(y_df, p, pos_label=1)
         pr_df = pd.DataFrame()
         pr_df['PRECISION'] = precision
         pr_df['RECALL'] = recall
         pr_df['F1'] = 2 * pr_df['RECALL'] * pr_df['PRECISION'] / (pr_df['RECALL'] + pr_df['PRECISION'])
         thresholds = list(thresholds)
@@ -451,35 +357,23 @@
                           rf_clf: RandomForestClassifier,
                           clf_name: str,
                           feature_names: List[str],
                           class_names: List[str],
                           save_dir: str,
                           save_file_no: Optional[int] = None) -> None:
         """
-        Helper to produce visualization of random forest decision tree.
+        Helper to produce visualization of random forest decision tree using graphviz.
 
-        Parameters
-        ----------
-        rf_clf: RandomForestClassifier
-            sklearn RandomForestClassifier object.
-        clf_name: str
-            Classifier name.
-        feature_names: list
-            List of feature names.
-        class_names
-            List of classes. E.g., ['Attack absent', 'Attack present']
-        save_dir: str,
-            Directory where to save output in csv file format.
-        save_file_no: int or None.
-            If integer, represents the count of the classifier within a grid search. If none, the classifier is not
+        :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object.
+        :parameter str clf_name: Classifier name.
+        :parameter List[str] feature_names: List of feature names.
+        :parameter List[str] class_names: List of classes. E.g., ['Attack absent', 'Attack present']
+        :parameter str save_dir: Directory where to save output in csv file format.
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
-
-        Returns
-        -------
-        None
         """
 
         print('Visualizing example decision tree using graphviz...')
         estimator = rf_clf.estimators_[3]
         if save_file_no != None:
             dot_name = os.path.join(save_dir, str(clf_name) + '_' + str(save_file_no) + '_tree.dot')
             file_name = os.path.join(save_dir, str(clf_name) + '_' + str(save_file_no) + '_tree.pdf')
@@ -497,33 +391,21 @@
                           y_df: pd.DataFrame,
                           class_names: List[str],
                           save_dir: str,
                           save_file_no: Optional[int] = None) -> None:
         """
         Helper to create classifier truth table report.
 
-        Parameters
-        ----------
-        rf_clf: RandomForestClassifier
-            sklearn RandomForestClassifier object.
-        x_df: pd.DataFrame
-            Pandas dataframe holding test features.
-        y_df: pd.DataFrame
-            Pandas dataframe holding test target.
-        class_names: list
-            List of classes. E.g., ['Attack absent', 'Attack present']
-        save_dir: str,
-            Directory where to save output in csv file format.
-        save_file_no: int or None.
-            If integer, represents the count of the classifier within a grid search. If none, the classifier is not
+        :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object.
+        :parameter pd.DataFrame x_df: dataframe holding test features
+        :parameter pd.DataFrame y_df: dataframe holding test target
+        :parameter List[str] class_names: List of classes. E.g., ['Attack absent', 'Attack present']
+        :parameter str save_dir: Directory where to save output in csv file format.
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
-
-        Returns
-        -------
-        None
         """
 
         print('Creating classification report visualization...')
         try:
             visualizer = ClassificationReport(rf_clf, classes=class_names, support=True)
             visualizer.score(x_df, y_df)
             if save_file_no != None:
@@ -533,39 +415,27 @@
                 save_path = os.path.join(save_dir, class_names[1] + '_classification_report.png')
             visualizer.poof(outpath=save_path, clear_figure=True)
         except KeyError as e:
             NotEnoughDataWarning(msg=f'Not enough data to create classification report: {class_names[1]}')
 
     def create_x_importance_log(self,
                                 rf_clf: RandomForestClassifier,
-                                x_names: list,
+                                x_names: List[str],
                                 clf_name: str,
                                 save_dir: str,
                                 save_file_no: Optional[int] = None) -> None:
         """
         Helper to save gini or entropy based feature importance scores.
 
-        Parameters
-        ----------
-        rf_clf: RandomForestClassifier
-            sklearn RandomForestClassifier object.
-        x_names: list
-            Names of features.
-        clf_name: str
-            Name of classifier.
-        save_dir: str,
-            Directory where to save output in csv file format.
-        save_file_no: int or None.
-            If integer, represents the count of the classifier within a grid search. If none, the classifier is not
+        :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object.
+        :parameter List[str] x_names: Names of features.
+        :parameter str clf_name: Name of classifier
+        :parameter str save_dir: Directory where to save output in csv file format.
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
-
-        Returns
-        -------
-        None
-
         """
 
         print('Creating feature importance log...')
         importances = list(rf_clf.feature_importances_)
         feature_importances = [(feature, round(importance, 2)) for feature, importance in zip(x_names, importances)]
         df = pd.DataFrame(feature_importances, columns=['FEATURE', 'FEATURE_IMPORTANCE']).sort_values(
             by=['FEATURE_IMPORTANCE'], ascending=False)
@@ -581,33 +451,21 @@
                                       clf_name: str,
                                       save_dir: str,
                                       n_bars: int,
                                       save_file_no: Optional[int] = None) -> None:
         """
         Helper to create a bar chart displaying the top N gini or entropy feature importance scores.
 
-        Parameters
-        ----------
-        rf_clf: RandomForestClassifier
-            sklearn RandomForestClassifier object.
-        x_names: list
-            Names of features.
-        clf_name: str
-            Name of classifier.
-        save_dir: str
-            Directory where to save output in csv file format.
-        n_bars: int
-            Number of bars in the plot.
-        save_file_no: str or None
-            If integer, represents the count of the classifier within a grid search. If none, the classifier is not
-            part of a grid search.
-
-        Returns
-        -------
-        None
+        :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object.
+        :parameter List[str] x_names: Names of features.
+        :parameter str clf_name: Name of classifier.
+        :parameter str save_dir: Directory where to save output in csv file format.
+        :parameter int n_bars: Number of bars in the plot.
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
+            part of a grid search
         """
 
         print('Creating feature importance bar chart...')
         self.create_x_importance_log(rf_clf, x_names, clf_name, save_dir)
         importances_df = pd.read_csv(os.path.join(save_dir, clf_name + '_feature_importance_log.csv'))
         importances_head = importances_df.head(n_bars)
         colors = create_color_palette(pallete_name='hot', increments=n_bars, as_rgb_ratio=True)
@@ -627,32 +485,21 @@
     def dviz_classification_visualization(self,
                                           x_train: np.ndarray,
                                           y_train: np.ndarray,
                                           clf_name: str,
                                           class_names: List[str],
                                           save_dir: str) -> None:
         """
-        Helper to create visualization of example decision tree.
+        Helper to create visualization of example decision tree using dtreeviz.
 
-        Parameters
-        ----------
-        x_train: np.array
-            Array with training features
-        y_train: np.array
-            Array with training targets
-        clf_name: str
-            Name of classifier
-        class_names:
-            List of class names. E.g., ['Attack absent', 'Attack present']
-        save_dir: str
-            Directory where to save output in svg file format.
-
-        Returns
-        -------
-        None
+        :parameter np.ndarray x_train: training features
+        :parameter np.ndarray y_train: training targets
+        :parameter str clf_name: Name of classifier
+        :parameter List[str] class_names: List of class names. E.g., ['Attack absent', 'Attack present']
+        :parameter str save_dir: Directory where to save output in csv file format.
         """
 
         clf = tree.DecisionTreeClassifier(max_depth=5, random_state=666)
         clf.fit(x_train, y_train)
         try:
             svg_tree = dtreeviz(clf, x_train, y_train, target_name=clf_name, feature_names=x_train.columns,
                                 orientation="TD", class_names=class_names, fancy=True, histtype='strip', X=None,
@@ -698,18 +545,14 @@
         cnt_absent: int
             Number of behavior-absent frames to calculate SHAP values for.
         save_dir: str,
             Directory where to save output in csv file format.
         save_file_no: int or None.
             If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
-
-        Returns
-        -------
-
         """
 
         print('Calculating SHAP values...')
         shap_timer = SimbaTimer(start=True)
         data_df = pd.concat([x_df, y_df], axis=1)
         if save_file_no == None:
             out_df_shap_path = os.path.join(save_path, f'SHAP_values_{clf_name}.csv')
@@ -761,22 +604,16 @@
                                               save_path=save_path)
 
     def print_machine_model_information(self,
                                         model_dict: dict) -> None:
         """
         Helper to print model information in tabular form.
 
-        Parameters
-        ----------
-        model_dict: dict
-            Python dictionary holding model meta data in SimBA meta-config format.
+        :parameter dict model_dict: dictionary holding model meta data in SimBA meta-config format.
 
-        Returns
-        -------
-        None
         """
 
         table_view = [["Model name", model_dict[MetaKeys.CLF_NAME.value]], ["Ensemble method", 'RF'],
                       ["Estimators (trees)", model_dict[MetaKeys.RF_ESTIMATORS.value]],
                       ["Max features", model_dict[MetaKeys.RF_MAX_FEATURES.value]],
                       ["Under sampling setting", model_dict[ConfigKey.UNDERSAMPLE_SETTING.value]],
                       ["Under sampling ratio", model_dict[ConfigKey.UNDERSAMPLE_RATIO.value]],
@@ -787,31 +624,24 @@
         table = tabulate(table_view, ["Setting", "value"], tablefmt="grid")
         print(f'{table} {Defaults.STR_SPLIT_DELIMITER.value}TABLE')
 
 
     def create_meta_data_csv_training_one_model(self,
                                                 meta_data_lst: list,
                                                 clf_name: str,
-                                                save_dir: str) -> None:
+                                                save_dir: Union[str, os.PathLike]) -> None:
         """
-        Helper to save single model meta data (hyperparameters, sampling settings etc.) into SimBA
+        Helper to save single model meta data (hyperparameters, sampling settings etc.) from list format into SimBA
         compatible CSV config file.
 
-        Parameters
-        ----------
-        meta_data_lst: list
-            list of meta data
-        clf_name: str
-            name of classifier
-        save_dir: str,
-            Directory where to save output in csv file format.
 
-        Returns
-        -------
-        None
+        :parameter list meta_data_lst: Meta data in list format
+        :parameter str clf_name: Name of classifier
+        :parameter str clf_name: Name of classifier
+        :parameter str save_dir: Directory where to save output in csv file format.
         """
         print('Saving model meta data file...')
         save_path = os.path.join(save_dir, clf_name + '_meta.csv')
         out_df = pd.DataFrame(columns=get_meta_data_file_headers())
         out_df.loc[len(out_df)] = meta_data_lst
         out_df.to_csv(save_path)
 
@@ -824,58 +654,41 @@
         save_path = os.path.join(save_dir, f'{clf_name}_{str(save_file_no)}_meta.csv')
         out_df = pd.DataFrame.from_dict(meta_data, orient='index').T
         out_df.to_csv(save_path)
 
     def save_rf_model(self,
                       rf_clf: RandomForestClassifier,
                       clf_name: str,
-                      save_dir: str,
+                      save_dir: Union[str, os.PathLike],
                       save_file_no: Optional[int] = None) -> None:
         """
         Helper to save pickled classifier object to disk.
 
-        Parameters
-        ----------
-        rf_clf: RandomForestClassifier
-            sklearn random forest classifier
-        clf_name: str
-            Classifier name
-        save_dir: str,
-            Directory where to save output in csv file format.
-        save_file_no: int or None.
-            If integer, represents the count of the classifier within a grid search. If none, the classifier is not
+        :parameter RandomForestClassifier rf_clf: sklearn random forest classifier
+        :parameter str clf_name: Classifier name
+        :parameter str save_dir: Directory where to save output in csv file format.
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
-
-        Returns
-        -------
-        None
         """
 
         if save_file_no != None:
             save_path = os.path.join(save_dir, clf_name + '_' + str(save_file_no) + '.sav')
         else:
             save_path = os.path.join(save_dir, clf_name + '.sav')
         pickle.dump(rf_clf, open(save_path, 'wb'))
 
     def get_model_info(self,
                        config: configparser.ConfigParser,
-                       model_cnt: int) -> dict:
+                       model_cnt: int) -> Dict[int, Any]:
         """
         Helper to read in N SimBA random forest config meta files to python dict memory.
 
-        Parameters
-        ----------
-        config:  configparser.ConfigParser
-            Parsed SimBA project_config.ini
-        model_cnt
-            Count of models
-
-        Returns
-        -------
-        model_dict: dict
+        :parameter configparser.ConfigParser config: Parsed SimBA project_config.ini
+        :parameter int model_cnt: Count of models
+        :return dict: Dictionary with integers as keys and hyperparameter dictionaries as keys.
         """
 
         model_dict = {}
         for n in range(model_cnt):
             try:
                 model_dict[n] = {}
                 if config.get('SML settings', 'model_path_' + str(n + 1)) == '':
@@ -907,53 +720,36 @@
 
     def get_all_clf_names(self,
                           config: configparser.ConfigParser,
                           target_cnt: int) -> List[str]:
         """
         Helper to get all classifier names in a SimBA project.
 
-        Parameters
-        ----------
-        config:  configparser.ConfigParser
-            Parsed SimBA project_config.ini
-        target_cnt
-            Count of models
-
-        Returns
-        -------
-        model_names: list
+        :parameter configparser.ConfigParser config: Parsed SimBA project_config.ini
+        :parameter int.ConfigParser target_cnt: Parsed SimBA project_config.ini
+        :return List[str]: All classifier names in project
         """
 
         model_names = []
         for i in range(target_cnt):
             entry_name = 'target_name_{}'.format(str(i + 1))
             model_names.append(
                 read_config_entry(config, ConfigKey.SML_SETTINGS.value, entry_name, data_type=Dtypes.STR.value))
         return model_names
 
     def insert_column_headers_for_outlier_correction(self,
                                                      data_df: pd.DataFrame,
                                                      new_headers: List[str],
                                                      filepath: str) -> pd.DataFrame:
         """
-        Helper to insert new column headers onto a dataframe.
+        Helper to insert new column headers onto a dataframe following outlier correction.
 
-        Parameters
-        ----------
-        data_df:  pd.DataFrame
-            Dataframe where headers to to-bo replaced.
-        new_headers: list
-            Names of new headers.
-        filepath: str
-            Path to where ``data_df`` is stored on disk
-
-        Returns
-        -------
-        data_df: pd.DataFrame
-            Dataframe with new headers
+        :parameter pd.DataFrame data_df: Dataframe with headers to-be replaced.
+        :parameter str filepath: Path to where ``data_df`` is stored on disk.
+        :parameter List[str] new_headers: New headers.
         """
 
         if len(new_headers) != len(data_df.columns):
             difference = int(len(data_df.columns) - len(new_headers))
             bp_missing = int(abs(difference) / 3)
             if difference < 0:
 
@@ -978,44 +774,47 @@
                                                                             str(bp_missing)))
             raise ValueError()
         else:
             data_df.columns = new_headers
             return data_df
 
     def read_pickle(self,
-                    file_path: str) -> object:
+                    file_path: Union[str, os.PathLike]) -> object:
+        """
+        Read pickle file
+
+        :parameter str file_path: Path to pickle file on disk.
+        :return dict
+
+        """
+
         try:
             clf = pickle.load(open(file_path, 'rb'))
         except pickle.UnpicklingError:
             raise CorruptedFileError(msg=f'Can not read {file_path} as a classifier file (pickle).')
         return clf
 
     def bout_train_test_splitter(self,
                                  x_df: pd.DataFrame,
                                  y_df: pd.Series,
                                  test_size: float) -> (np.ndarray, np.ndarray, np.ndarray, np.ndarray):
         """
         Helper to split train and test based on annotated `bouts`.
 
-        Parameters
-        ----------
-        x_df:  pd.DataFrame
-            Features
-        y_df: pd.Series
-            Target
-        test_size: float
-            Size of test as ratio of all annotated bouts.
-
-        Returns
-        -------
-        x_train, x_test, y_train, y_test
-        """
 
+        :parameter pd.DataFrame x_df: Features
+        :parameter pd.Series y_df: Target
+        :parameter float test_size: Size of test as ratio of all annotated bouts (e.g., ``0.2``).
+
+        :return np.ndarray x_train: Features for training
+        :return np.ndarray x_test: Features for testing
+        :return np.ndarray y_train: Target for training
+        :return np.ndarray y_test: Target for testing
+        """
         print('Using bout sampling...')
-
         def find_bouts(s: pd.Series, type: str):
             test_bouts_frames, train_bouts_frames = [], []
             bouts = detect_bouts(pd.DataFrame(s), target_lst=pd.DataFrame(s).columns, fps=-1)
             print(f'{str(len(bouts))} {type} bouts found...')
             bouts = list(bouts.apply(lambda x: list(range(int(x['Start_frame']), int(x['End_frame']) + 1)), 1).values)
             test_bouts_idx = np.random.choice(np.arange(0, len(bouts)), int(len(bouts) * test_size))
             train_bouts_idx = np.array([x for x in list(range(len(bouts))) if x not in test_bouts_idx])
@@ -1036,15 +835,22 @@
 
         return x_train, x_test, y_train, y_test
 
     def check_sampled_dataset_integrity(self,
                                         x_df: pd.DataFrame,
                                         y_df: pd.DataFrame) -> None:
 
-        """ Helper to check for non-numerical entries post sampling"""
+        """
+        Helper to check for non-numerical entries post data sampling
+
+        :parameter pd.DataFrame x_df: Features
+        :parameter pd.DataFrame y_df: Target
+
+        :raise FaultyTrainingSetError: Training or testing data sets contain non-numerical values
+        """
 
         x_df = x_df.replace([np.inf, -np.inf, None], np.nan)
         x_nan_cnt = x_df.isna().sum()
         x_nan_cnt = x_nan_cnt[x_nan_cnt > 0]
 
         if len(x_nan_cnt) > 0:
             if len(x_nan_cnt) < 10:
@@ -1066,19 +872,26 @@
                 raise FaultyTrainingSetError(
                     msg=f'All training annotations for classifier {str(y_df.name)} is labelled as PRESENT. A classifier has be be trained with both behavior PRESENT and ABSENT ANNOTATIONS.')
 
     def partial_dependence_calculator(self,
                                       clf: RandomForestClassifier,
                                       x_df: pd.DataFrame,
                                       clf_name: str,
-                                      save_dir: str,
-                                      clf_cnt: int or None = None) -> None:
+                                      save_dir: Union[str, os.PathLike],
+                                      clf_cnt: Optional[int] = None) -> None:
 
         """
-        Helper to compute single feature partial dependencies
+        Compute feature partial dependencies for every feature in training set.
+
+        :parameter RandomForestClassifier clf: Random forest classifier
+        :parameter pd.DataFrame x_df: Features training set
+        :parameter str clf_name: Name of classifier
+        :parameter str save_dir: Directory where to save the data
+        :parameter Optional[int] clf_cnt: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
+            part of a grid search.
         """
         print(f'Calculating partial dependencies for {len(x_df.columns)} features...')
         clf.verbose = 0
         check_if_dir_exists(save_dir)
         if clf_cnt:
             save_dir = os.path.join(save_dir, f'partial_dependencies_{clf_name}_{clf_cnt}')
         else:
@@ -1090,84 +903,95 @@
             df = pd.DataFrame({'partial dependence': pdp[0], 'feature value': axes[0]})
             df.to_csv(save_path)
             print(f'Partial dependencies for {feature_name} complete...')
 
     def clf_predict_proba(self,
                           clf: RandomForestClassifier,
                           x_df: pd.DataFrame,
-                          model_name: str or None = None,
-                          data_path: str or None = None) -> np.ndarray:
-        """ Helper to run clf inference """
+                          model_name: Optional[str] = None,
+                          data_path: Optional[Union[str, os.PathLike]] = None) -> np.ndarray:
+        """
+
+        :param RandomForestClassifier clf: Random forest classifier object
+        :param pd.DataFrame x_df: Features df
+        :param Optional[str] model_name: Name of model
+        :param Optional[str] data_path: Path to model on disk
+        :return np.ndarray: 2D array with frame represented by rows and present/absent probabilities as columns
+        :raises FeatureNumberMismatchError: If shape of x_df and clf.n_features_ show mismatch
+        """
+
         if len(x_df.columns) != clf.n_features_:
             if model_name and data_path:
                 raise FeatureNumberMismatchError(f'Mismatch in the number of features in input file {data_path}, and what is expected by the model {model_name}. The model expects {str(clf.n_features_)} features. The data contains {len(x_df.columns)} features.')
             else:
                 raise FeatureNumberMismatchError(f'The model expects {str(clf.n_features_)} features. The data contains {len(x_df.columns)} features.')
         p_vals = clf.predict_proba(x_df)
         if p_vals.shape[1] != 2:
             raise ClassifierInferenceError(
                 msg='The classifier {model_name} has not been created properly. See The SimBA GitHub FAQ page or Gitter for more information and suggested fixes.')
         return p_vals[:, 1]
 
     def clf_fit(self,
                 clf: RandomForestClassifier,
                 x_df: pd.DataFrame,
-                y_df: pd.DataFrame) -> np.ndarray:
+                y_df: pd.DataFrame) -> RandomForestClassifier:
+        """
+        Helper to fit clf model
 
-        """Helper to fit clf model"""
+        :param clf: Un-fitted random forest classifier object
+        :param pd.DataFrame x_df: Pandas dataframe with features.
+        :param pd.DataFrame y_df: Pandas dataframe/Series with target
+        :return RandomForestClassifier: Fitted random forest classifier object
+        """
         nan_features = x_df[~x_df.applymap(np.isreal).all(1)]
         nan_target = y_df.loc[pd.to_numeric(y_df).isna()]
         if len(nan_features) > 0:
             raise FaultyTrainingSetError(
                 msg=f'{len(nan_features)} frame(s) in your project_folder/csv/targets_inserted directory contains FEATURES with non-numerical values')
         if len(nan_target) > 0:
             raise FaultyTrainingSetError(
                 msg=f'{len(nan_target)} frame(s) in your project_folder/csv/targets_inserted directory contains ANNOTATIONS with non-numerical values')
         return clf.fit(x_df, y_df)
 
     def _read_data_file_helper(self,
                                file_path: str,
                                file_type: str,
                                clf_names: Optional[List[str]] = None):
-        """ Private function called by ``simba.train_model_functions.read_all_files_in_folder_mp`` """
+        """
+        Private function called by :meth:`simba.train_model_functions.read_all_files_in_folder_mp`
+        """
+
         timer = SimbaTimer(start=True)
         _, vid_name, _ = get_fn_ext(file_path)
         df = read_df(file_path, file_type).dropna(axis=0, how='all').fillna(0)
         df.index = [vid_name] * len(df)
         if clf_names != None:
             for clf_name in clf_names:
                 if not clf_name in df.columns:
                     raise ColumnNotFoundError(column_name=clf_name, file_name=file_path)
         timer.stop_timer()
         print(f'Reading complete {vid_name} (elapsed time: {timer.elapsed_time_str}s)...')
         return df
 
     def read_all_files_in_folder_mp(self,
-                                    file_paths: list,
-                                    file_type: str,
-                                    classifier_names: Optional[List[str]] = None):
+                                    file_paths: List[str],
+                                    file_type: Literal['csv', 'parquet', 'pickle'],
+                                    classifier_names: Optional[List[str]] = None) -> pd.DataFrame:
         """
 
         Multiprocessing helper function to read in all data files in a folder to a single
         pd.DataFrame for downstream ML. Defaults to ceil(CPU COUNT / 2) cores. Asserts that all classifiers
         have annotation fields present in each dataframe.
 
-        Parameters
-        ----------
-        file_paths: list
-            List of file paths representing files to be read in.
-        file_type: str
-            Type of files in ``file_paths``. OPTIONS: csv or parquet.
-        classifier_names: list or None
-            List of classifier names representing fields of human annotations. If not None, then assert that classifier names
-            are present in each data file.
 
-        Returns
-        -------
-        pd.DataFrame
+        :parameter List[str] file_paths: List of file-paths
+        :parameter List[str] file_paths: The filetype of ``file_paths`` OPTIONS: csv or parquet.
+        :parameter Optional[List[str]] classifier_names: List of classifier names representing fields of human annotations. If not None, then assert that classifier names
+            are present in each data file.
+        :return pd.DataFrame: Concatenated dataframe of all data in ``file_paths``.
 
         """
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
         cpu_cnt, _ = find_core_cnt()
         df_lst = []
         try:
@@ -1187,17 +1011,24 @@
         except BrokenProcessPool or AttributeError:
             return self.read_all_files_in_folder(file_paths=file_paths,
                                             file_type=file_type,
                                             classifier_names=classifier_names)
 
     def check_raw_dataset_integrity(self,
                                     df: pd.DataFrame,
-                                    logs_path: str) -> pd.DataFrame:
+                                    logs_path: Optional[Union[str, os.PathLike]]) -> None:
 
-        """ Helper to check column-wise NaNs in raw input data for fitting model"""
+        """
+        Helper to check column-wise NaNs in raw input data for fitting model.
+
+        :param pd.DataFrame df
+        :param str logs_path: The logs directory of the SimBA project
+        :raise FaultyTrainingSetError: When the dataset contains NaNs
+
+        """
 
         nan_cols = df.reset_index(drop=True).replace([np.inf, -np.inf, None], np.nan).columns[df.isna().any()].tolist()
         if len(nan_cols) == 0:
             return df.reset_index(drop=True)
         else:
             save_log_path = os.path.join(logs_path, f'missing_columns_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
             results = {}
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from simba.utils.printing import stdout_success
 from simba.utils.checks import check_if_filepath_list_is_empty,check_if_dir_exists
 from simba.mixins.config_reader import ConfigReader
 
 class DeepEthogramImporter(ConfigReader):
 
     """
-    Class for appending DeepEthogram optical flow annotations onto featurized pose-estimation data.
+    Append DeepEthogram optical flow annotations onto featurized pose-estimation data.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     deep_ethogram_dir: str
         path to folder holding DeepEthogram data files is CSV format
@@ -25,15 +25,15 @@
     ----------
     `Third-party import tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
     `Example expected input <https://github.com/sgoldenlab/simba/blob/master/misc/deep_ethogram_labels.csv>`__.
 
     Examples
     ----------
     >>> deepethogram_importer = DeepEthogramImporter(config_path=r'MySimBAConfigPath', deep_ethogram_dir=r'MyDeepEthogramDir')
-    >>> deepethogram_importer.import_deepethogram()
+    >>> deepethogram_importer.run()
 
     References
     ----------
 
     .. [1] `DeepEthogram repo <https://github.com/jbohnslav/deepethogram>`__.
     .. [2] `Example DeepEthogram input file <https://github.com/sgoldenlab/simba/blob/master/misc/deep_ethogram_labels.csv>`__.
     """
@@ -64,15 +64,15 @@
                 if short_file_name in feature_file_names:
                     self.matches_dict[file_path] = os.path.join(self.features_dir, short_file_name + ext)
                     pass
             else:
                 print('SIMBA ERROR: Could not find file in project_folder/csv/features_extracted directory representing {}'.format(file_name))
                 raise FileNotFoundError()
 
-    def import_deepethogram(self):
+    def run(self):
         for cnt, (k, v) in enumerate(self.matches_dict.items()):
             _, video_name, _ = get_fn_ext(filepath=v)
             self.annotations_df = read_df(file_path=k, file_type=self.file_type).reset_index(drop=True)
             self.features_df = read_df(file_path=v, file_type=self.file_type).reset_index(drop=True)
             _, _, self.fps = self.read_video_info(video_name=video_name)
             for clf_name in self.clf_names:
                 if clf_name not in self.annotations_df.columns:
@@ -98,8 +98,8 @@
             write_df(df=self.out_data, file_type=self.file_type, save_path=save_path)
             print('DeepEthogram annotation for video {} saved...'.format(video_name))
 
         stdout_success(msg=f'Annotations for {str(len(list(self.clf_names)))} behaviors added to {len(self.matches_dict.keys())} videos and saved in the project_folder/csv/targets_inserted directory.')
 
 # test = DeepEthogramImporter(deep_ethogram_dir='/Users/simon/Desktop/troubleshooting/deepethnogram/deepethnogram',
 #                             config_path='/Users/simon/Desktop/troubleshooting/deepethnogram/project_folder/project_config.ini')
-# test.import_deepethogram()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,27 @@
                                 ThirdPartyAnnotationEventCountError)
 from simba.utils.warnings import (ThirdPartyAnnotationsOutsidePoseEstimationDataWarning,
                                   ThirdPartyAnnotationsInvalidFileFormatWarning)
 
 class BorisAppender(ConfigReader):
 
     """
-    Class for appending BORIS human annotations onto featurized pose-estimation data.
+    Append BORIS human annotations onto featurized pose-estimation data.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     boris_folder: str
         path to folder holding BORIS data files is CSV format
 
     Notes
     ----------
-    `Example BORIS input file <https://github.com/sgoldenlab/simba/blob/master/misc/boris_example.csv`__.
+    `Third-party import tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
+    `Example BORIS input file <https://github.com/sgoldenlab/simba/blob/master/misc/boris_example.csv>`_.
 
     Examples
     ----------
     >>> boris_appender = BorisAppender(config_path='MyProjectConfigPath', boris_folder=r'BorisDataFolder')
     >>> boris_appender.create_boris_master_file()
     >>> boris_appender.run()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/observer_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 POINT_EVENT = 'Point'
 START = 'State start'
 STOP = 'State stop'
 EXPECTED_FIELDS = [TIME_FIELD, VIDEO_NAME_FIELD, BEHAVIOR_FIELD, EVENT_TYPE_FIELD]
 
 class NoldusObserverImporter(ConfigReader):
     """
-    Class for appending Noldu Observer human annotations onto featurized pose-estimation data.
+    Append Noldus Observer human annotations onto featurized pose-estimation data.
     Results are saved within the project_folder/csv/targets_inserted directory of
     the SimBA project (as parquets' or CSVs).
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
@@ -41,16 +41,15 @@
     -----
     `Third-party import GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
     `Expected input example 1 <https://github.com/sgoldenlab/simba/blob/master/misc/Observer_example_1.xlsx>`__.
     `Expected input example 2 <https://github.com/sgoldenlab/simba/blob/master/misc/Observer_example_2.xlsx>`__.
 
     Examples
     -----
-    >>> importer = NoldusObserverImporter(config_path='MyConfigPath', data_dir='MyNoldusObserverDataDir')
-    >>> importer.run()
+    >>> _ = NoldusObserverImporter(config_path='MyConfigPath', data_dir='MyNoldusObserverDataDir'),run()
     """
 
     def __init__(self,
                  config_path: str,
                  data_dir: str):
 
         super().__init__(config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/third_party_appender.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 SOLOMON = 'SOLOMON'
 BENTO = 'BENTO'
 BEHAVIOR = 'BEHAVIOR'
 
 class ThirdPartyLabelAppender(ConfigReader):
 
     """
-    Class for concatenate third-party annotations to featurized pose-estimation datasets in SimBA.
+    Concatenate third-party annotations to featurized pose-estimation datasets in SimBA.
 
     Parameters
     ----------
     app: str
         Third-party application. OPTIONS: ['BORIS', 'BENTO', 'DEEPETHOGRAM', 'ETHOVISION', 'OBSERVER', 'SOLOMON'].
     config_path: str
         path to SimBA project config file in Configparser format.
@@ -56,20 +56,20 @@
         User-defined settings including how to handle errors, logging, and data file types associated with the third-party application.
 
     Notes
     ----------
     `Third-party import tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
 
     `BENTO: expected input <https://github.com/sgoldenlab/simba/blob/master/misc/bento_example.annot`__.
-    `BORIS: expected input <https://github.com/sgoldenlab/simba/blob/master/misc/boris_example.csv`__..
-    `DEEPETHOGRAM: expected input <https://github.com/sgoldenlab/simba/blob/master/misc/deep_ethogram_labels.csv`__.
-    `ETHOVISION: expected input <https://github.com/sgoldenlab/simba/blob/master/misc/ethovision_example.xlsx`__.
-    `OBSERVER: expected input I <https://github.com/sgoldenlab/simba/blob/master/misc/Observer_example_1.xlsx`__.
-    `OBSERVER: expected input II <https://github.com/sgoldenlab/simba/blob/master/misc/Observer_example_2.xlsx`__.
-    `SOLOMON: expected input II <https://github.com/sgoldenlab/simba/blob/master/misc/solomon_example.csv`__.
+    `BORIS: expected input <https://github.com/sgoldenlab/simba/blob/master/misc/boris_example.csv>`__..
+    `DEEPETHOGRAM: expected input <https://github.com/sgoldenlab/simba/blob/master/misc/deep_ethogram_labels.csv>`__.
+    `ETHOVISION: expected input <https://github.com/sgoldenlab/simba/blob/master/misc/ethovision_example.xlsx>`__.
+    `OBSERVER: expected input I <https://github.com/sgoldenlab/simba/blob/master/misc/Observer_example_1.xlsx>`__.
+    `OBSERVER: expected input II <https://github.com/sgoldenlab/simba/blob/master/misc/Observer_example_2.xlsx>`__.
+    `SOLOMON: expected input II <https://github.com/sgoldenlab/simba/blob/master/misc/solomon_example.csv>`__.
 
 
     Examples
     ----------
     >>> settings = {'log': True,  'file_format': 'csv', 'errors': {'INVALID annotations file data format': 'WARNING',
     >>>                                                             'ADDITIONAL third-party behavior detected': 'NONE',
     >>>                                                             'Annotations EVENT COUNT conflict': 'WARNING',
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/ethovision_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from simba.utils.read_write import get_fn_ext, read_df, write_df, read_config_file
 from simba.utils.checks import check_if_filepath_list_is_empty, check_that_column_exist
 from simba.utils.printing import stdout_success
 from simba.mixins.config_reader import ConfigReader
 
 class ImportEthovision(ConfigReader):
     """
-    Class for appending ETHOVISION human annotations onto featurized pose-estimation data.
+    Append ETHOVISION human annotations onto featurized pose-estimation data.
     Results are saved within the project_folder/csv/targets_inserted directory of
     the SimBA project (as parquets' or CSVs).
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
@@ -24,15 +24,15 @@
     Notes
     -----
     `Third-party import GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
     `Example of expected ETHOVISION file <https://github.com/sgoldenlab/simba/blob/master/misc/ethovision_example.xlsx>`__.
 
     Examples
     -----
-    >>> ImportEthovision(config_path="MyConfigPath", folder_path="MyEthovisionFolderPath")
+    >>> _ = ImportEthovision(config_path="MyConfigPath", folder_path="MyEthovisionFolderPath")
     """
 
     def __init__(self,
                  config_path: str,
                  folder_path: str):
 
         super().__init__(config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,33 +11,33 @@
                                   ThirdPartyAnnotationsClfMissingWarning,
                                   ThirdPartyAnnotationsAdditionalClfWarning)
 from simba.utils.errors import AnnotationFileNotFoundError
 
 
 class BentoAppender(ConfigReader):
     """
-    Class for appending BENTO annotation to SimBA featurized datasets.
+    Append BENTO annotation to SimBA featurized datasets.
 
     Notes
     ----------
-    `Example BORIS input file <https://github.com/sgoldenlab/simba/blob/master/misc/boris_example.csv`__.
-    'GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md`__.
+    `Example BENTO input file <https://github.com/sgoldenlab/simba/blob/master/misc/bento_example.annot>`_.
+
+    'GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`_.
 
     Examples
     ----------
     >>> bento_dir = 'tests/test_data/bento_example'
     >>> config_path = 'tests/test_data/import_tests/project_folder/project_config.ini'
     >>> bento_appender = BentoAppender(config_path=config_path, bento_dir=bento_dir)
     >>> bento_appender.run()
 
     References
     ----------
 
     .. [1] Segalin et al., eLife, https://doi.org/10.7554/eLife.63720
-
     """
 
     def __init__(self,
                  config_path: str,
                  bento_dir: str):
 
         ConfigReader.__init__(self, config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.59.4/simba/third_party_label_appenders/solomon_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from simba.utils.printing import stdout_success
 from simba.utils.checks import check_that_column_exist, check_if_filepath_list_is_empty
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 from simba.mixins.config_reader import ConfigReader
 
 class SolomonImporter(ConfigReader):
     """
-    Class for appending SOLOMON human annotations onto featurized pose-estimation data.
+    Append SOLOMON human annotations onto featurized pose-estimation data.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     solomon_dir: str
         path to folder holding SOLOMON data files is CSV format
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,25 @@
 from simba.utils.checks import check_that_column_exist
 from simba.cue_light_tools.cue_light_tools import find_frames_when_cue_light_on
 from simba.utils.errors import NoFilesFoundError
 from simba.mixins.config_reader import ConfigReader
 
 class CueLightClfAnalyzer(ConfigReader):
     """
-    Class for computing aggregate statistics when classified behaviors are occurring in relation to the cue light
+    Compute aggregate statistics when classified behaviors are occurring in relation to the cue light
     ON and OFF states.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    pre_window: int
-        Time period (in millisecond) before the onset of each cue light to compute aggregate classification
-        statistics for.
-    post_window: int
-        Time period (in millisecond) after the offset of each cue light to compute aggregate classification
-        statistics for.
-    cue_light_names: list
-        Names of cue lights, as defined in the SimBA ROI interface.
-    clf_list: list
-        Names of the classifiers we want to compute aggregate statistics for.
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter int pre_window: Time period (in millisecond) before the onset of each cue light to compute aggregate classification
+        statistics within.
+    :parameter int post_window: Time period (in millisecond) after the offset of each cue light to compute aggregate classification
+        statistics within.
+    :parameter List[str] cue_light_names: Names of cue lights, as defined in the SimBA ROI interface.
+    :parameter List[str] list: Names of the classifiers we want to compute aggregate statistics for.
 
-    Notes
     ----------
     `Cue light tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/cue_light_tutorial.md>`__.
 
     Examples
     ----------
     >>> cue_light_clf_analyzer = CueLightClfAnalyzer(config_path='MyProjectConfig', pre_window=1000, post_window=1000, cue_light_names=['Cue_light'], clf_list=['Attack'])
     >>> cue_light_clf_analyzer.analyze_clf()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,34 +58,29 @@
             roi_image = bg + dst
             results_dict[frm_cnt][circle['Name']] = int(np.average(np.linalg.norm(roi_image, axis=2)) / np.sqrt(3))
         frm_cnt+=1
     return results_dict
 
 class CueLightAnalyzer(ConfigReader):
     """
-    Class for analyzing when cue lights are in ON and OFF states. Results are stored in the
-    `project_folder/csv/cue_lights` cue lights directory.
+    Analyze when cue lights are in ON and OFF states. Results are stored in the
+    ``project_folder/csv/cue_lights`` cue lights directory.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    in_dir: str
-        directory holding pose-estimation data. E.g., `project_folder/csv/outlier_corrected_movement_location`
-    cue_light_names: list
-        Names of cue lights, as defined in the SimBA ROI interface.
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str in_dir: directory holding pose-estimation data. E.g., ``project_folder/csv/outlier_corrected_movement_location``
+    :parameter List[str] cue_light_names: Names of cue light ROIs, as defined in the SimBA ROI interface.
 
     Notes
     ----------
     `Cue light tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/cue_light_tutorial.md>`__.
 
     Examples
     ----------
     >>> cue_light_analyzer = CueLightAnalyzer(config_path='MyProjectConfig', in_dir='project_folder/csv/outlier_corrected_movement_location', cue_light_names=['Cue_light'])
-    >>> cue_light_analyzer.analyze_files()
+    >>> cue_light_analyzer.run()
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  in_dir: Union[str, os.PathLike],
                  cue_light_names: List[str]):
 
@@ -146,15 +141,15 @@
                 self.data_df.loc[r['Start_frame'] - 1:r['End_frame']+1,cue_light_name] = 0
 
     def insert_light_data(self):
         for shape_name in self.cue_light_names:
             self.data_df.loc[list(self.light_descriptive_statistics[shape_name]['ON_FRAMES']), shape_name] = 1
         self.data_df = self.data_df.fillna(0)
 
-    def analyze_files(self):
+    def run(self):
         start_time = time.time()
         for file_cnt, file_path in enumerate(self.files_found):
             self.data_df = read_df(file_path, self.file_type)
             _, self.video_name, _ = get_fn_ext(file_path)
             self.save_path = os.path.join(self.out_dir, self.video_name + '.' + self.file_type)
             video_settings, pix_per_mm, self.fps = self.read_video_info(video_name=self.video_name)
             self.video_recs = self.rectangles_df.loc[(self.rectangles_df['Video'] == self.video_name) & (self.rectangles_df['Name'].isin(self.cue_light_names))]
@@ -193,10 +188,10 @@
             write_df(self.data_df, self.file_type, self.save_path)
         elapsed_time = str(round(time.time() - start_time, 2)) + 's'
         stdout_success(msg=f'Analysed {str(len(self.files_found))} files. Data stored in project_folder/csv/cue_lights', elapsed_time=elapsed_time)
 
 # test = CueLightAnalyzer(config_path='/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/project_config.ini',
 #                         in_dir='/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/csv/outlier_corrected_movement_location',
 #                         cue_light_names=['Cue_light'])
-# test.analyze_files()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_menues.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,34 +18,29 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
 import webbrowser
 
 
 class CueLightAnalyzerMenu(ConfigReader, PopUpMixin):
     """
-    Class for lunching cue light analysis GUI in SimBA.
+    Launch cue light analysis GUI in SimBA.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
     Notes
     ----------
     `Cue light tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/cue_light_tutorial.md>`__.
 
 
     Examples
     ----------
     >>> cue_light_gui = CueLightAnalyzerMenu(config_path='MySimBAConfigPath')
-    >>> cue_light_gui.cue_light_main_frame.mainloop()
+    >>> cue_light_gui.main_frm.mainloop()
     """
 
-
-
     def __init__(self,
                  config_path: Union[str, os.PathLike]):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.data_dir = os.path.join(self.project_path, 'csv', 'outlier_corrected_movement_location')
         self.cue_light_data_folder = os.path.join(self.project_path, 'csv', 'cue_lights')
         self.read_roi_data()
@@ -106,15 +101,15 @@
             self.lights_dict[light_cnt]['dropdown'] = OptionMenu(self.cue_light_settings_frm, self.lights_dict[light_cnt]['light_chosen'], *self.shape_names, command=None)
             self.lights_dict[light_cnt]['label'].grid(row=current_row, column=0, sticky=W)
             self.lights_dict[light_cnt]['dropdown'].grid(row=current_row, column=1, sticky=W)
 
     def __analyze_cue_light_data(self):
         self.__get_cue_light_names()
         cue_light_analyzer = CueLightAnalyzer(config_path=self.config_path, in_dir=self.data_dir, cue_light_names=self.light_lst)
-        cue_light_analyzer.analyze_files()
+        cue_light_analyzer.run()
 
     def __visualize_cue_light_data(self):
         self.cue_light_data_files = glob.glob(self.cue_light_data_folder + '/*' + self.file_type)
         if len(self.cue_light_data_files) == 0:
             raise NoFilesFoundError(msg='SIMBA ERROR: Zero data files found. Please analyze cue light data prior to visualizing cue light data')
         else:
             self.__get_cue_light_names()
@@ -122,15 +117,15 @@
                 _, file_name, _ = get_fn_ext(data_path)
                 video_path = find_video_of_file(self.video_dir, file_name)
                 cue_light_visualizer = CueLightVisualizer(config_path=self.config_path,
                                                           cue_light_names=self.light_lst,
                                                           video_path=video_path,
                                                           video_setting=self.video_var.get(),
                                                           frame_setting=self.frames_var.get())
-                cue_light_visualizer.visualize_cue_light_data()
+                cue_light_visualizer.run()
 
     def __inititate_animal_movement_menu(self):
         self.movement_main_frame = Toplevel()
         self.movement_main_frame.minsize(400, 400)
         self.movement_main_frame.wm_title("SIMBA CUE LIGHT ANALYZER: MOVEMENTS")
         self.movement_main_frame.lift()
         self.animal_cnt_frm = LabelFrame(self.movement_main_frame, text='SETTINGS', font=('Helvetica', 15, 'bold'), pady=5, padx=15)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from simba.utils.data import detect_bouts
 
 def find_frames_when_cue_light_on(data_df: pd.DataFrame,
                                   cue_light_names: List[str],
                                   fps: int,
                                   prior_window_frames_cnt: int,
                                   post_window_frames_cnt: int):
+    """
+    Multiprocess helper for finding cue-light states.
+    Called by meth:`simba.cue_light_tools.cue_light_analyzer.CueLightAnalyzer`.
+    """
     light_on_dict = {}
     for cue_light in cue_light_names:
         light_on_dict[cue_light] = {}
         light_bouts = detect_bouts(data_df=data_df, target_lst=[cue_light], fps=fps)
         light_bouts['Start_pre_window'] = light_bouts['Start_frame'] - prior_window_frames_cnt
         light_bouts['Start_pre_window'] = light_bouts['Start_pre_window'].clip(lower=0)
         light_bouts['Start_post_window'] = light_bouts['End_frame']
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,35 +10,28 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_df, get_fn_ext, get_video_meta_data
 from simba.utils.printing import stdout_success
 from simba.utils.checks import check_file_exist_and_readable
 
 class CueLightVisualizer(ConfigReader):
     """
-    Class for visualizing SimBA computed cue-light ON and OFF states and the aggregate statistics of ON and OFF
+
+    Visualize SimBA computed cue-light ON and OFF states and the aggregate statistics of ON and OFF
     states.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    cue_light_names: list
-        Names of cue lights, as defined in the SimBA ROI interface.
-    video_path: float
-        Path to video which user wants to create visualizations of cue light states and aggregate statistics for.
-    frame_setting: bool
-        If True, SimBA creates individual frames in png format.
-    video_setting: bool
-        If True, SimBA creates compressed videos in mp4 format.
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter List[str] cue_light_names: Names of cue lights, as defined in the SimBA ROI interface.
+    :parameter str video_path: Path to video which user wants to create visualizations of cue light states and aggregate statistics for.
+    :parameter bool frame_setting: If True, creates individual frames in png format.
+    :parameter bool video_setting: If True, creates compressed videos in mp4 format.
 
     Notes
     ----------
     `Cue light tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/cue_light_tutorial.md>`__.
 
-
     Examples
     ----------
     >>> cue_light_visualizer = CueLightVisualizer(config_path='SimBAConfig', cue_light_names=['Cue_light'], video_path='VideoPath', video_setting=True, frame_setting=False)
     >>> cue_light_visualizer.visualize_cue_light_data()
     """
 
     def __init__(self,
@@ -154,27 +147,19 @@
 
     def __insert_body_parts(self):
         for animal_name, animal_data in self.animal_bp_dict.items():
             for cnt, (x_bp, y_bp) in enumerate(zip(animal_data['X_bps'], animal_data['Y_bps'])):
                 cord = tuple(self.data_df.loc[self.frame_cnt, [x_bp, y_bp]].astype(int).values)
                 cv2.circle(self.border_img, cord, 0, animal_data['colors'][cnt], self.draw_scale)
 
-    def visualize_cue_light_data(self):
+    def run(self):
         """
         Method to create cue light visualizations. Results are stored in the ``project_folder/frames/output/cue_lights``
         directory of the SimBA project.
-
-        Returns
-        -------
-        None
         """
-
-
-
-
         self.cap = cv2.VideoCapture(self.video_path)
         self.frame_cnt = 0
         self.__update_video_meta_data()
         if self.video_setting:
             self.fourcc = cv2.VideoWriter_fourcc(*'mp4v')
             self.save_video_path = os.path.join(self.output_folder, self.video_name + '.mp4')
             self.writer = cv2.VideoWriter(self.save_video_path, self.fourcc, self.fps, (self.border_img_w, self.border_img_h))
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.59.4/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,34 +12,26 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.printing import stdout_success
 
 
 class CueLightMovementAnalyzer(ConfigReader):
     """
-    Class for computing aggregate statistics of animal movement in relation to the cue light
+    Compute aggregate statistics of animal movement in relation to the cue light
     ON and OFF states.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    pre_window: int
-        Time period (in millisecond) before the onset of each cue light to compute aggregate classification
-        statistics for.
-    post_window: int
-        Time period (in millisecond) after the offset of each cue light to compute aggregate classification
-        statistics for.
-    cue_light_names: list
-        Names of cue lights, as defined in the SimBA ROI interface.
-    threshold: float
-        The body-part post-estimation probability threshold. SimBA omits movement calculations for frames where the
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter int pre_window: Time period (in millisecond) before the onset of each cue light to compute aggregate classification
+        statistics within.
+    :parameter int post_window: Time period (in millisecond) after the offset of each cue light to compute aggregate classification
+        statistics within.
+    :parameter List[str] cue_light_names: Names of cue lights, as defined in the SimBA ROI interface.
+    :parameter float threshold: The body-part post-estimation probability threshold. SimBA omits movement calculations for frames where the
         body-part probability threshold is lower than the user-specified threshold.
-    roi_setting: bool
-        If True, SimBA calculates movement statistics within non-light cue ROIs.
+    :parameter bool roi_setting: If True, SimBA calculates movement statistics within non-light cue ROIs.
 
     Notes
     ----------
     `Cue light tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/cue_light_tutorial.md>`__.
 
 
     Examples
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/config_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,39 +11,29 @@
 from simba.utils.errors import DirectoryExistError
 from simba.utils.enums import (DirNames,
                                ConfigKey,
                                Dtypes,
                                Paths)
 
 class ProjectConfigCreator(object):
-
     """
-    Class for creating SimBA project directory tree and project_config.ini
+    Create SimBA project directory tree and associated project_config.ini config file.
 
-    Parameters
-    ----------
-    project_path: str
-        Path to directory where to save the SimBA project directory tree
-    project_name: str
-        Name of the SimBA project
-    target_list: list
-        Classifiers in the SimBA project
-    pose_estimation_bp_cnt: str
-        String representing the number of body-parts in the pose-estimation data used in the simba project. E.g.,
-        '16' or 'user-defined'.
-    body_part_config_idx: int
-        The index of the SimBA GUI dropdown pose-estimation selection. E.g., ``1``.
-    animal_cnt: int
-        Number of animals tracked in the input pose-estimation data.
-    file_type: str
-        The SimBA project file type. OPTIONS: ``csv`` or ``parquet``.
+    :parameter str project_path: path to directory where to save the SimBA project directory tree
+    :parameter str project_name: Name of the SimBA project
+    :parameter List[str] target_list: Classifier names in the SimBA project
+    :parameter str pose_estimation_bp_cnt: String representing the number of body-parts in the pose-estimation data used in the simba project.
+                                           E.g., '4', '7', '8', '9', '14', '16' or 'user_defined', '3D_user_defined'.
+    :parameter int body_part_config_idx: The index of the SimBA GUI dropdown pose-estimation selection. E.g., ``1``. I.e., the row representing
+                                         your pose-estimated body-parts in `this file <https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/bp_names/bp_names.csv>`_.
+    :parameter int animal_cnt: Number of animals tracked in the input pose-estimation data.
+    :parameter str file_type: The SimBA project file type. OPTIONS: ``csv`` or ``parquet``.
 
-    Notes
-    ----------
-    `Create project tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#part-1-create-a-new-project-1>`__.
+    .. note::
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#part-1-create-a-new-project-1>`__.
 
     Examples
     ----------
     >>> _ = ProjectConfigCreator(project_path = 'project/path', project_name='project_name', target_list=['Attack'], pose_estimation_bp_cnt='16', body_part_config_idx=9, animal_cnt=2, file_type='csv')
 
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/enums.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/checks.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/read_write.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,43 +34,35 @@
                                 FileExistError)
 from simba.utils.warnings import InvalidValueWarning, NoFileFoundWarning, FileExistWarning
 from simba.utils.printing import stdout_success
 from simba.utils.enums import Formats, Dtypes, ConfigKey
 from simba.utils.checks import (check_file_exist_and_readable,
                                 check_if_filepath_list_is_empty)
 
-
-
 PARSE_OPTIONS = csv.ParseOptions(delimiter=',')
 READ_OPTIONS = csv.ReadOptions(encoding='utf8')
 
-def read_df(file_path: str,
-            file_type: str,
+def read_df(file_path: Union[str, os.PathLike],
+            file_type: Union[str, os.PathLike],
             remove_columns: Optional[List[str]] = None,
             usecols: Optional[List[str]] = None,
             check_multiindex: bool = False) -> pd.DataFrame:
 
     """
-    Helper function to read single data file into memory.
+    Read single tabular data file.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to data file.
-    file_type: str
-        Type of data. OPTIONS: 'parquet' or 'csv'.
-    remove_columns: list or None,
-        If list, then remove columns
-    usecols: list or None,
-        If list, keep columns
-
-    Returns
-    -------
-    df: pd.DataFrame
+    .. note::
+       For improved runtime, defaults to ``pyarrow.csv`` if file_type == ``csv``.
 
+    :parameter str file_path: Path to data file
+    :parameter str file_type: Path to data file. OPTIONS: 'parquet', 'csv', 'pickle'.
+    :parameter Optional[List[str]] remove_columns: If not None, then remove columns in lits.
+    :parameter Optional[List[str]] usecols: If not None, then keep columns in list.
+    :parameter bool check_multiindex: check file is multi-index headers. Default: False.
+    :return pd.DataFrame
     """
     check_file_exist_and_readable(file_path=file_path)
     if file_type == Formats.CSV.value:
         try:
             df = csv.read_csv(file_path, parse_options=PARSE_OPTIONS, read_options=READ_OPTIONS)
             duplicate_headers = list(set([x for x in df.column_names if df.column_names.count(x) > 1]))
             if len(duplicate_headers) > 0:
@@ -101,34 +93,27 @@
     else:
         raise InvalidFileTypeError(msg=f'{file_type} is not a valid filetype OPTIONS: [pickle, csv, parquet]')
 
     return df
 
 def write_df(df: pd.DataFrame,
              file_type: str,
-             save_path: str,
+             save_path: Union[str, os.PathLike],
              multi_idx_header: bool = False) -> None:
 
     """
-    Helper function to save single dataframe from memory.
+    Write single tabular data file.
 
-    Parameters
-    ----------
-    df: pd.DataFrame
-        Pandas dataframe to save to disk.
-    file_type: str
-        Type of data. OPTIONS: 'parquet' or 'csv'.
-    save_path: str,
-        Location where to store the data.
-    multi_idx_header: bool,
-        If the data should be saved as a multi-index header file.
-
-    Returns
-    -------
-    None
+    .. note::
+       For improved runtime, defaults to ``pyarrow.csv`` if file_type == ``csv``.
+
+    :parameter pd.DataFrame df: Pandas dataframe to save to disk.
+    :parameter str file_type: Type of data. OPTIONS: ``parquet``, ``csv``,  ``pickle``.
+    :parameter str save_path: Location where to store the data.
+    :parameter bool check_multiindex: check if input file is multi-index headers. Default: False.
     """
 
     if file_type == Formats.CSV.value:
         if not multi_idx_header:
             df = df.drop('scorer', axis=1, errors='ignore')
             idx = np.arange(len(df)).astype(str)
             df.insert(0, '', idx)
@@ -147,27 +132,26 @@
                 pickle.dump(df, f, protocol=pickle.HIGHEST_PROTOCOL)
         except Exception as e:
             print(e.args[0])
             raise InvalidFileTypeError(msg='Data could not be saved as a pickle.')
     else:
         raise InvalidFileTypeError(msg=f'{file_type} is not a valid filetype OPTIONS: [csv, pickle, parquet]')
 
-def get_fn_ext(filepath: str) -> (str, str, str):
+def get_fn_ext(filepath: Union[os.PathLike, str]) -> (str, str, str):
     """
-    Helper to split file path into three components: (i) directory, (ii) file name, and (iii) file extension.
-    Parameters
-    ----------
-    filepath: str
-        Path to file.
-
-    Returns
-    -------
-    dir_name: str
-    file_name: str
-    file_extension: str
+    Split file path into three components: (i) directory, (ii) file name, and (iii) file extension.
+
+    :parameter str filepath: Path to file.
+    :return str: File directory name
+    :return str: File name
+    :return str: File extension
+
+    :example:
+    >>> get_fn_ext(filepath='C:/My_videos/MyVideo.mp4')
+    >>> ('My_videos', 'MyVideo', '.mp4')
     """
     file_extension = Path(filepath).suffix
     try:
         file_name = os.path.basename(filepath.rsplit(file_extension, 1)[0])
     except ValueError:
         raise InvalidFilepathError(msg='{} is not a valid filepath'.format(filepath))
     dir_name = os.path.dirname(filepath)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/errors.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/data.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/utils/printing.py` & `Simba-UW-tf-dev-1.59.4/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_processors/reorganize_keypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from simba.utils.checks import check_if_filepath_list_is_empty, check_if_dir_exists
 from simba.utils.printing import stdout_success
 from simba.utils.enums import Formats
 
 class KeypointReorganizer(object):
     """
-    Class for re-organizing the order of pose-estimated keypoints in directory containing
+    Re-organizing the order of pose-estimated keypoints in directory containing
     CSV or H5 format files.
 
     Parameters
     ----------
     data_folder: str
         Path to directory containing pose-estiation CSV or H5 data
     pose_tool: str
@@ -27,17 +27,17 @@
     Notes
     ----------
     `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Tutorial_tools.md#re-organize-tracking-data>`__.
 
     Examples
     ----------
     >>> keypoint_reorganizer = KeypointReorganizer(data_folder="test_data/misc_test_files", pose_tool='maDLC', file_format='h5')
-    >>> keypoint_reorganizer.perform_reorganization(animal_list=['UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'UM', 'UM', 'UM', 'LM', 'LM'], bp_lst=['Lateral_left', 'Nose', 'Tail_base', 'Lateral_right', 'Ear_right', 'Center', 'Nose', 'Ear_left', 'Ear_right', 'Center', 'Tail_end', 'Ear_left', 'Tail_base', 'Lateral_left', 'Tail_end', 'Lateral_right'])
+    >>> keypoint_reorganizer.run(animal_list=['UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'UM', 'UM', 'UM', 'LM', 'LM'], bp_lst=['Lateral_left', 'Nose', 'Tail_base', 'Lateral_right', 'Ear_right', 'Center', 'Nose', 'Ear_left', 'Ear_right', 'Center', 'Tail_end', 'Ear_left', 'Tail_base', 'Lateral_left', 'Tail_end', 'Lateral_right'])
     >>> keypoint_reorganizer = KeypointReorganizer(data_folder="test_data/misc_test_files", pose_tool='DLC', file_format='csv')
-    >>> keypoint_reorganizer.perform_reorganization(bp_lst=['Ear_left_1', 'Ear_right_1', 'Nose_1', 'Center_1', 'Lateral_left_1', 'Lateral_right_1', 'Tail_base_1', 'Ear_left_2', 'Ear_right_2', 'Nose_2', 'Center_2', 'Lateral_left_2', 'Lateral_right_2', 'Tail_base_2'], animal_list=None)
+    >>> keypoint_reorganizer.run(bp_lst=['Ear_left_1', 'Ear_right_1', 'Nose_1', 'Center_1', 'Lateral_left_1', 'Lateral_right_1', 'Tail_base_1', 'Ear_left_2', 'Ear_right_2', 'Nose_2', 'Center_2', 'Lateral_left_2', 'Lateral_right_2', 'Tail_base_2'], animal_list=None)
     """
 
     def __init__(self,
                  data_folder: str,
                  pose_tool: str,
                  file_format: Optional[str] = None):
 
@@ -93,15 +93,15 @@
                 self.header_list = list(zip(scorer, bodyparts, coords))
 
         elif (file_format == Formats.CSV.value) and (pose_tool == 'SLEAP'):
             print('s')
 
 
 
-    def perform_reorganization(self,
+    def run(self,
                                bp_lst: list,
                                animal_list: list = None):
         save_directory = os.path.join(self.data_folder, 'Reorganized_bp_{}'.format(self.datetime))
         if not os.path.exists(save_directory): os.makedirs(save_directory)
         print('Saving {} new pose-estimation files in {} directory...'.format(str(len(self.files_found)), save_directory))
         header_tuples = []
         if self.pose_tool == 'maDLC':
@@ -129,11 +129,11 @@
                 df_reorganized.to_csv(df_save_path)
             print('Saved {}, Video {}/{}.'.format(os.path.basename(file_path), str(file_cnt + 1), str(len(self.files_found))))
         stdout_success(msg=f'{str(len(self.files_found))} new data files with reorganized body-parts saved in {save_directory} directory')
 
 #keypoint_reorganizer = KeypointReorganizer(data_folder="/Users/simon/Desktop/envs/troubleshooting/Termites_5/import_h5", pose_tool='SLEAP', file_format='csv')
 #keypoint_reorganizer = KeypointReorganizer(data_folder="/Users/simon/Desktop/envs/troubleshooting/Termites_5/import_h5", pose_tool='SLEAP', file_format='SLEAP H5')
 #keypoint_reorganizer = KeypointReorganizer(data_folder="/Users/simon/Desktop/troubleshooting/B1-MS_US/el_import", pose_tool='maDLC', file_format='h5')
-#keypoint_reorganizer.perform_reorganization(animal_list=['UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'UM', 'UM', 'UM', 'LM', 'LM'], bp_lst=['Nose', 'Tail_base', 'Tail_base', 'Lateral_right', 'Ear_right', 'Center', 'Nose', 'Ear_left', 'Ear_right', 'Center', 'Tail_end', 'Ear_left', 'Tail_base', 'Lateral_left', 'Tail_end', 'Lateral_right'])
+#keypoint_reorganizer.run(animal_list=['UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'UM', 'UM', 'UM', 'LM', 'LM'], bp_lst=['Nose', 'Tail_base', 'Tail_base', 'Lateral_right', 'Ear_right', 'Center', 'Nose', 'Ear_left', 'Ear_right', 'Center', 'Tail_end', 'Ear_left', 'Tail_base', 'Lateral_left', 'Tail_end', 'Lateral_right'])
 
 #keypoint_reorganizer = KeypointReorganizer(data_folder="//Users/simon/Desktop/simbapypi_dev/tests/test_data/misc_test_files", pose_tool='DLC', file_format='csv')
-#keypoint_reorganizer.perform_reorganization(bp_lst=['Ear_left_1', 'Ear_right_1', 'Nose_1', 'Center_1', 'Lateral_left_1', 'Lateral_right_1', 'Tail_base_1', 'Ear_left_2', 'Ear_right_2', 'Nose_2', 'Center_2', 'Lateral_left_2', 'Lateral_right_2', 'Tail_base_2'], animal_list=None)
+#keypoint_reorganizer.run(bp_lst=['Ear_left_1', 'Ear_right_1', 'Nose_1', 'Center_1', 'Lateral_left_1', 'Lateral_right_1', 'Tail_base_1', 'Ear_left_2', 'Ear_right_2', 'Nose_2', 'Center_2', 'Lateral_left_2', 'Lateral_right_2', 'Tail_base_2'], animal_list=None)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_processors/remove_keypoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.errors import NotDirectoryError, BodypartColumnNotFoundError, InvalidFileTypeError
 warnings.filterwarnings('ignore', category=NaturalNameWarning)
 
 class KeypointRemover(object):
     """
-    Class for removing pose-estimated keypoints from data in CSV or H5 format.
+    Remove pose-estimated keypoints from data in CSV or H5 format.
 
     Parameters
     ----------
     data_folder: str
         Path to directory containing pose-estiation CSV or H5 data
     pose_tool: str
         Tool used to perform pose-estimation.
@@ -26,15 +26,15 @@
     Notes
     ----------
     `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Tutorial_tools.md#remove-body-parts-from-tracking-data>`__.
 
     Examples
     ----------
     >>> keypoint_remover = KeypointRemover(data_folder="MyDataFolder", pose_tool='maDLC', file_format='h5')
-    >>> keypoint_remover.run_bp_removal(bp_to_remove_list=['Nose_1, Nose_2'])
+    >>> keypoint_remover.run(bp_to_remove_list=['Nose_1, Nose_2'])
     """
 
     def __init__(self,
                  data_folder: str,
                  pose_tool: str,
                  file_format: str):
 
@@ -62,15 +62,15 @@
             for header_entry in header_list:
                 if header_entry[1] not in self.body_part_names:
                     self.animal_names.append(header_entry[1])
                     self.body_part_names.append(header_entry[2])
 
         self.body_part_names, self.animal_names = list(set(self.body_part_names)), list(set(self.animal_names))
 
-    def run_bp_removal(self, animal_names: list, bp_to_remove_list: list):
+    def run(self, animal_names: list, bp_to_remove_list: list):
         self.timer = SimbaTimer()
         self.timer.start_timer()
         save_directory = os.path.join(self.data_folder, 'Reorganized_bp_{}'.format(self.datetime))
         if not os.path.exists(save_directory): os.makedirs(save_directory)
         print('Saving {} new pose-estimation files in {} directory...'.format(str(len(self.files_found)), save_directory))
         if (self.pose_tool == 'DLC') or (self.pose_tool == 'maDLC'):
             for file_cnt, file_path in enumerate(self.files_found):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_processors/pose_reset.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,22 @@
 from simba.utils.printing import stdout_trash
 from simba.utils.lookups import get_bp_config_codes
 from simba.utils.checks import check_file_exist_and_readable
 
 
 class PoseResetter(object):
     """
-    Class for deleting all user-defined pose-estimation schematics, diagrams and other settings from the
-    SimBA installation
+    Launch GUI for deleting all **user-defined** pose-estimation schematics, diagrams and other settings from the
+    SimBA installation.
 
     Parameters
     ----------
     master: tk
         tkinter master window, (default=None).
 
-    Notes
-    ----------
-
     Examples
     ----------
     >>> _ = PoseResetter(master=None)
     """
 
     def __init__(self,
                  master: Toplevel):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/gantt_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.read_write import read_df, get_fn_ext
 from simba.utils.checks import check_if_filepath_list_is_empty
 
 class GanttCreatorSingleProcess(ConfigReader, PlottingMixin):
     """
-    Class for creating gantt chart videos and/or images using a single core.
+    Create gantt chart videos and/or images using a single core.
+    For improved run-time, see :meth:`simba.gantt_creator_mp.GanttCreatorMultiprocess` for multiprocess class.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     frame_setting: bool
         If True, creates individual frames
@@ -33,18 +34,16 @@
     video_setting: bool
         If True, creates videos
     style_attr: dict
         Attributes of gannt chart (size, font size, font rotation etc).
     files_found: list
         File paths representing files with machine predictions e.g., ['project_folder/csv/machine_results/My_results.csv']
 
-    Notes
-    ----------
-    `GitHub gantt tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#gantt-plot>`__.
-    See ``simba.gantt_creator_mp.GanttCreatorMultiprocess`` for multiprocess class.
+    .. note::
+       `GitHub gantt tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#gantt-plot>`__.
 
     Examples
     ----------
     >>> style_attr = {'width': 640, 'height': 480, 'font size': 12, 'font rotation': 45}
     >>> gantt_creator = GanttCreatorSingleProcess(config_path='tests/test_data/multi_animal_dlc_two_c57/project_folder/project_config.ini', frame_setting=False, video_setting=True, files_found=['tests/test_data/multi_animal_dlc_two_c57/project_folder/csv/machine_results/Together_1.csv'])
     >>> gantt_creator.run()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/ROI_plotter_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.errors import NoFilesFoundError, DuplicationError
 from simba.utils.read_write import get_video_meta_data, concatenate_videos_in_folder, get_fn_ext
 pd.options.mode.chained_assignment = None
 
 class ROIPlotMultiprocess(ConfigReader, PlottingMixin):
     """
-    Class for visualizing the ROI data (number of entries/exits, time-spent-in etc)
+    Visualize the ROI data (number of entries/exits, time-spent-in etc)
 
     Parameters
     ----------
     config_path: str
         Path to SimBA project config file in Configparser format
     video_path: str
         Name of video to create ROI visualizations for
 
     Notes
     ----------
     `ROI tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial_new.md>`__.
 
     Examples
     ----------
-    >>> roi_visualizer = ROIPlot(ini_path=r'MyProjectConfig', video_path="MyVideo.mp4")
+    >>> roi_visualizer = ROIPlotMultiprocess(ini_path=r'MyProjectConfig', video_path="MyVideo.mp4")
     >>> roi_visualizer.insert_data()
     >>> roi_visualizer.visualize_ROI_data()
     """
 
     def __init__(
             self,
             ini_path: str,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from simba.utils.warnings import ShapWarning
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.checks import check_file_exist_and_readable
 
 class ShapAggregateStatisticsVisualizer(ConfigReader):
 
     """
-    Class for calculating aggregate, binned, SHAP value statistics where individual bins represent reaulated features.
+    Caluclate aggregate (binned) SHAP value statistics where individual bins represent reaulated features.
     Also creates line chart visualizations reprsenting aggregations of behavior-present SHAP values.
 
     Parameters
     ----------
     config_path: str
         Path to SimBA project config file in Configparser format
     classifier_name: str
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/gantt_creator_mp.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.data import detect_bouts
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 
 class GanttCreatorMultiprocess(ConfigReader, PlottingMixin):
-
     """
-    Class for multiprocess creation of classifier gantt charts in video and/or image format.
+    Multiprocess creation of classifier gantt charts in video and/or image format.
+    See meth:`simba.gantt_creator.GanttCreatorSingleProcess` for single-process class.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     frame_setting: bool
         If True, creates individual frames
@@ -37,24 +37,21 @@
     files_found: list
         File paths representing files with machine predictions e.g., ['project_folder/csv/machine_results/My_results.csv']
     cores: int
         Number of cores to use
     style_attr: dict
         Output image style attributes, e.g., {'width': 640, 'height': 480, 'font size': 8, 'font rotation': 45}
 
-
     Notes
     ----------
     `GitHub gantt tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#gantt-plot>`__.
-    See ``simba.gantt_creator.GanttCreatorSingleProcess`` for single-process class.
 
     Examples
     ----------
-    >>> gantt_creator = GanttCreatorMultiprocess(config_path='tests/test_data/multi_animal_dlc_two_c57/project_folder/project_config.ini', frame_setting=False, video_setting=True, files_found=['tests/test_data/multi_animal_dlc_two_c57/project_folder/csv/machine_results/Together_1.csv'], cores=5, style_attr={'width': 640, 'height': 480, 'font size': 8, 'font rotation': 45})
-    >>> gantt_creator.run()
+    >>> gantt_creator = GanttCreatorMultiprocess(config_path='project_folder/project_config.ini', frame_setting=False, video_setting=True, files_found=['project_folder/csv/machine_results/Together_1.csv'], cores=5, style_attr={'width': 640, 'height': 480, 'font size': 8, 'font rotation': 45}).run()
 
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/heat_mapper_clf_mp.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         video_writer.release()
 
     return group
 
 class HeatMapperClfMultiprocess(ConfigReader, PlottingMixin):
 
     """
-    Class for creating heatmaps representing the locations of the classified behavior
+    Create heatmaps representing the locations of the classified behavior
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     final_img_setting: bool
         If True, then  create the a single image representing the last frame of the input video
@@ -205,24 +205,15 @@
 
         return clf_array, aspect_ratio
 
     def __calculate_max_scale(self,
                               clf_array: np.array):
         return np.round(np.max(np.max(clf_array[-1], axis=0)), 3)
 
-    def create_heatmaps(self):
-        '''
-        Creates heatmap charts. Results are stored in the `project_folder/frames/heatmaps_classifier_locations`
-        directory of SimBA project.
-
-        Returns
-        ----------
-        None
-        '''
-
+    def run(self):
         for file_cnt, file_path in enumerate(self.files_found):
             video_timer = SimbaTimer()
             video_timer.start_timer()
             _, self.video_name, _ = get_fn_ext(file_path)
             self.video_info, self.px_per_mm, self.fps = self.read_video_info(video_name=self.video_name)
             self.width, self.height = int(self.video_info['Resolution_width'].values[0]), int(self.video_info['Resolution_height'].values[0])
             self.save_frame_folder_dir = os.path.join(self.heatmap_clf_location_dir, self.video_name + '_' + self.clf_name)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/probability_plot_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.read_write import read_df, get_fn_ext
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_that_column_exist
 
 class TresholdPlotCreatorSingleProcess(ConfigReader, PlottingMixin):
     '''
-    Class for creating line chart visualizations displaying the classification probabilities of a single classifier.
+    Create line chart visualizations displaying the classification probabilities of a single classifier.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     clf_name: str
         Name of the classifier to create visualizations for
@@ -31,14 +31,18 @@
     video_setting: bool
        When True, SimBA creates compressed video in mp4 format
     files_found: list
         File paths to create probability plots for, e.g., ['project_folder/csv/machine_results/MyVideo.csv]
     style_attr: dict
         Output image style attributes, e.g., {'width': 640, 'height': 480, 'font size': 10, 'line width': 6, 'color': 'magneta', 'circle size': 20}
 
+    Notes
+    ----------
+    `Documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`_.
+
 
     Examples
     -----
     >>> style_attr = {'width': 640, 'height': 480, 'font size': 10, 'line width': 6, 'color': 'blue', 'circle size': 20}
     >>> clf_name='Attack'
     >>> files_found=['/_test/project_folder/csv/machine_results/Together_1.csv']
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/plot_clf_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,21 @@
 from simba.utils.enums import ConfigKey, Formats, Dtypes
 from simba.utils.read_write import get_fn_ext, read_df, get_video_meta_data, read_config_entry
 from simba.utils.checks import check_file_exist_and_readable, check_float, check_int
 from simba.utils.data import create_color_palette
 
 class PlotSklearnResultsSingleCore(ConfigReader, TrainModelMixin, PlottingMixin):
     """
-    Class for plotting classification results on videos. Results are stored in the
+    Plot classification results overlays on videos. Results are stored in the
     `project_folder/frames/output/sklearn_results` directory of the SimBA project.
 
+    .. note::
+       For improved run-time, see :meth:`simba.plot_clf_results_mp.PlotSklearnResultsMultiProcess` for multiprocess class.
+
+
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     rotate: bool
         If True, the output video will be rotated 90 degrees from the input.
     video_setting: bool
@@ -38,16 +42,16 @@
 
     Notes
     ----------
     `Scikit visualization documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-10-sklearn-visualization__.
 
     Examples
     ----------
-    >>> clf_plotter = PlotSklearnResults(config_path='MyProjectConfig', video_setting=True, frame_setting=False, rotate=False, video_file_path='VideoPath')
-    >>> clf_plotter.initialize_visualizations()
+    >>> clf_plotter = PlotSklearnResultsSingleCore(config_path='MyProjectConfig', video_setting=True, frame_setting=False, rotate=False, video_file_path='VideoPath')
+    >>> clf_plotter.run()
     """
 
     def __init__(self,
                  config_path: str,
                  video_setting: bool,
                  frame_setting: bool,
                  text_settings: Union[Dict[str, float], bool],
@@ -175,15 +179,15 @@
             except KeyError as e:
                 print(e.args, e)
                 print('SIMBA INDEX WARNING: Some frames appears to be missing in the dataframe and could not be created')
                 print('Video {} saved...'.format(self.video_name))
                 self.cap.release()
                 self.writer.release()
 
-    def initialize_visualizations(self):
+    def run(self):
         if self.video_file_path is None:
             for file_cnt, file_path in enumerate(self.files_found):
                 self.file_cnt, self.file_path = file_cnt, file_path
                 self.create_visualizations()
         else:
             self.file_cnt, file_path = 0, self.video_file_path
             _, file_name, _ = get_fn_ext(file_path)
@@ -198,15 +202,15 @@
 # test = PlotSklearnResultsSingleCore(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                       video_setting=True,
 #                                       frame_setting=False,
 #                                       video_file_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Together_1.avi',
 #                                       print_timers=True,
 #                                       text_settings=False,
 #                                       rotate=False)
-# test.initialize_visualizations()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/plot_clf_results_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         video_writer.release()
 
     return group
 
 
 class PlotSklearnResultsMultiProcess(ConfigReader, TrainModelMixin, PlottingMixin):
     """
-    Class for plotting classification results on videos. Results are stored in the
+    Plot classification results on videos. Results are stored in the
     `project_folder/frames/output/sklearn_results` directory of the SimBA project.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     rotate: bool
@@ -116,16 +116,16 @@
 
     Notes
     ----------
     `Scikit visualization documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-10-sklearn-visualization__.
 
     Examples
     ----------
-    >>> clf_plotter = PlotSklearnResults(config_path='MyProjectConfig', video_setting=True, frame_setting=False, rotate=False, video_file_path='VideoPath', cores=5)
-    >>> clf_plotter.initialize_visualizations()
+    >>> clf_plotter = PlotSklearnResultsMultiProcess(config_path='MyProjectConfig', video_setting=True, frame_setting=False, rotate=False, video_file_path='VideoPath', cores=5)
+    >>> clf_plotter.run()
     """
 
     def __init__(self,
                  config_path: str,
                  video_setting: bool,
                  frame_setting: bool,
                  text_settings: Union[Dict[str, float], bool],
@@ -225,15 +225,15 @@
                 print('Joining {} multiprocessed video...'.format(self.video_name))
                 concatenate_videos_in_folder(in_folder=self.video_temp_dir, save_path=self.video_save_path)
             video_timer.stop_timer()
             pool.terminate()
             pool.join()
             print('Video {} complete (elapsed time: {}s)...'.format(self.video_name, video_timer.elapsed_time_str))
 
-    def initialize_visualizations(self):
+    def run(self):
         if self.video_file_path is None:
             self.files_found = self.machine_results_paths
             print('Processing {} videos...'.format(str(len(self.machine_results_paths))))
             for file_cnt, file_path in enumerate(self.machine_results_paths):
                 self.file_cnt, self.file_path = file_cnt, file_path
                 self.create_visualizations()
         else:
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/ROI_feature_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,34 +9,36 @@
 from simba.utils.enums import Formats
 from simba.utils.read_write import get_video_meta_data, get_fn_ext, read_df
 from simba.roi_tools.ROI_feature_analyzer import ROIFeatureCreator
 from simba.utils.checks import check_file_exist_and_readable
 
 class ROIfeatureVisualizer(ConfigReader):
     """
-    Class for visualizing features that depend on the relationships between the location of the animals and user-defined
+    Visualizing features that depend on the relationships between the location of the animals and user-defined
     ROIs. E.g., distances to centroids of ROIs, cumulative time spent in ROIs, if animals are directing towards ROIs
     etc.
 
+    .. note::
+       For improved run-time, see :meth:`simba.ROI_feature_visualizer_mp.ROIfeatureVisualizerMultiprocess` for multiprocess class.
+
     Parameters
     ----------
     config_path: str
         Path to SimBA project config file in Configparser format
 
     video_name: str
         Name of video to create feature visualizations for.
 
     Notes
     ----------
     `Tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#part-5-visualizing-roi-features>`__.
 
     Examples
     ----------
-    >>> roi_feature_visualizer = ROIfeatureVisualizer(config_path='MyProjectConfig', video_name='MyVideo.mp4')
-    >>> roi_feature_visualizer.create_visualization()
+    >>> _ = ROIfeatureVisualizer(config_path='MyProjectConfig', video_name='MyVideo.mp4').run()
     """
 
     def __init__(self,
                  config_path: str,
                  video_name: str,
                  style_attr: dict):
 
@@ -119,15 +121,15 @@
                                         [r['ROI_edge_2_x'], r['ROI_edge_2_y']],
                                         [r['Eye_x'], r['Eye_y']]]).reshape(-1, 2).astype(int)
             cv2.fillPoly(self.img_w_border, [convex_hull_arr], clr)
 
         if self.style_attr['Directionality_style'] == 'Lines':
             cv2.line(self.img_w_border, (int(r['Eye_x']), int(r['Eye_y'])), (int(r['ROI_x']), int(r['ROI_y'])), clr, int(thickness))
 
-    def create_visualization(self):
+    def run(self):
         """
         Creates and saves visualizations of ROI-based features. Results are stored in the ``project_folder/frames/
         output/ROI_features`` directory  of the SimBA project.
 
         Returns
         ----------
         None
@@ -213,19 +215,19 @@
         self.timer.stop_timer()
         self.cap.release()
         self.writer.release()
         stdout_success('Feature video {} saved in {} directory ...', elapsed_time=self.timer.elapsed_time_str)
 
 # style_attr = {'ROI_centers': True, 'ROI_ear_tags': True, 'Directionality': True, 'Border_color': (0, 128, 0), 'Pose_estimation': True}
 # test = ROIfeatureVisualizer(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', video_name='Together_1.avi', style_attr=style_attr)
-# test.create_visualization()
+# test.run()
 
 
 # style_attr = {'ROI_centers': True, 'ROI_ear_tags': True, 'Directionality': True, 'Directionality_style': 'Line', 'Border_color': (0, 128, 0), 'Pose_estimation': True}
 # test = ROIfeatureVisualizer(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/mouse_open_field/project_folder/project_config.ini', video_name='Video1.mp4', style_attr=style_attr)
-# test.create_visualization()
+# test.run()
 
 
 # test = ROIfeatureVisualizer(config_path='/Users/simon/Desktop/train_model_project/project_folder/project_config.ini', video_name='Together_1.avi')
-# test.create_visualization()
+# test.run()
 # test.save_new_features_files()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/heat_mapper_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df
 
 class HeatmapperLocationSingleCore(ConfigReader, PlottingMixin):
     """
-    Class for creating heatmaps representing the location where animals spend time.
+    Create heatmaps representing the location where animals spend time.
+    For improved run-time, see :meth:`simba.heat_mapper_location_mp.HeatMapperLocationMultiprocess` for multiprocess class.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     bodypart: str
         The name of the body-part used to infer the location of the classified behavior
@@ -34,23 +35,23 @@
         >= 10 within a rectangular bins, it will be filled with the same color.
     final_img_setting: bool
         If True, create a single image representing the last frame of the input video
     video_setting: bool
         If True, then create a video of heatmaps.
     frame_setting: bool
         If True, then create individual heatmap frames
+
     Notes
     -----
     `GitHub visualizations tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
     Examples
     -----
 
-    >>> heat_mapper_location = HeatmapperLocationSingleCore(config_path='MyConfigPath', final_img_setting=False, video_setting=True, frame_setting=False, bin_size=50, palette='jet', bodypart='Nose_1', max_scale=20)
-    >>> heat_mapper_location.create_heatmaps()
+    >>> _ = HeatmapperLocationSingleCore(config_path='MyConfigPath', final_img_setting=False, video_setting=True, frame_setting=False, bin_size=50, palette='jet', bodypart='Nose_1', max_scale=20).run()
     """
 
     def __init__(self,
                  config_path: str,
                  bodypart: str,
                  style_attr: dict,
                  final_img_setting: bool,
@@ -139,15 +140,15 @@
                     for k in range(sliced_arr.shape[2]):
                         frame_cum_sum[j][k] += sliced_arr[i][j][k]
             cum_sum_arr[frm_idx] = frame_cum_sum
 
 
         return cum_sum_arr / fps
 
-    def create_heatmaps(self):
+    def run(self):
         for file_cnt, file_path in enumerate(self.files_found):
             video_timer = SimbaTimer()
             video_timer.start_timer()
             _, self.video_name, _ = get_fn_ext(file_path)
             self.video_info, self.px_per_mm, self.fps = self.read_video_info(video_name=self.video_name)
             self.width, self.height = int(self.video_info['Resolution_width'].values[0]), int(self.video_info['Resolution_height'].values[0])
             if self.video_setting:
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/interactive_probability_grapher.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from simba.utils.errors import InvalidInputError, ColumnNotFoundError
 from simba.utils.checks import check_file_exist_and_readable
 from simba.plotting.tools.tkinter_tools import InteractiveVideoPlotterWindow
 from simba.utils.read_write import read_df, get_fn_ext
 
 class InteractiveProbabilityGrapher(ConfigReader):
     """
-    Class for launching and creating interactive GUI for classifier probability inspection.
+    Launch interactive GUI for classifier probability inspection.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     clf_name: str
         Name of the classifier to create visualizations for
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/plot_pose_in_dir.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ACCEPTED_DIRECTORIES = ['input_csv', 'outlier_corrected_movement', 'outlier_corrected_movement_location']
 
 def create_video_from_dir(in_directory: str,
                           out_directory: str,
                           circle_size: int,
                           clr_attr: Optional[Dict[str, Tuple[int, int, int]]] = None):
     """
-    Class for creating pose-estimation visualizations from data within a SimBA project folder.
+    Create pose-estimation visualizations from data within a SimBA project folder.
 
     Parameters
     ----------
     in_directory: str
         Path to SimBA project directory containing pose-estimation data in parquet or CSV format.
     out_directory: str
         Directory to where to save the pose-estimation videos.
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/single_run_model_validation_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,20 @@
 
 plt.interactive(True)
 plt.ioff()
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 class ValidateModelOneVideo(ConfigReader, PlottingMixin):
     """
-    Class for creating classifier validation video for a single input video. Results are stored in the
+    Create classifier validation video for a single input video. Results are stored in the
     `project_folder/frames/output/validation directory`.
 
+    .. note::
+       For improved run-time, see :meth:`simba.sing_run_model_validation_video_mp.ValidateModelOneVideoMultiprocess` for multiprocess class.
+
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     feature_file_path: str
         path to SimBA file (parquet or CSV) containing pose-estimation and feature fields.
     model_path: str
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,33 +13,32 @@
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import Paths
 from simba.mixins.config_reader import ConfigReader
 
 
 class FrameMergererFFmpeg(ConfigReader):
     """
-    Class for merging separate visualizations of classifications, descriptive statistics etc., into  single
+    Merge separate visualizations of classifications, descriptive statistics etc., into  single
     video mosaic.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    concat_type: str
-        Type of concatenation. E.g. ``vertical``, ``horizontal``
-    frame_types: dict
-        Dict holding video  path to videos to concatenate. E.g., {'Video 1': path, 'Video 2': path}
-    video_height: int
-        Output video height (width depends on frame_types count)
-
-    Notes
-    -----
-    `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-12-merge-frames>`__.
 
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str concat_type: Type of concatenation. E.g. ``vertical``, ``horizontal``
+    :parameter dict frame_types: Dict holding video path to videos to concatenate. E.g., {'Video 1': path, 'Video 2': path}
+    :parameter int video_height: Output video height.
+    :parameter int video_width: Output video width.
+
+    .. note:
+       `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-12-merge-frames>`_.
 
+    Example
+    ----------
+    >>> frame_types={'Video 1': 'project_folder/videos/Video_1.avi', 'Video 2': 'project_folder/videos/Video_2.avi'}
+    >>> video_height, video_width, concat_type = 640, 480, 'vertical'
+    >>> FrameMergererFFmpeg(config_path='MySimBaConfigPath', frame_types=frame_types, video_height=video_height, video_width=video_width, concat_type=concat_type)
     """
 
     def __init__(self,
                  concat_type: Literal['horizontal', 'vertical', 'mosaic', 'mixed_mosaic'],
                  frame_types: Dict[str, str],
                  video_height: int,
                  video_width: int,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,30 +16,24 @@
 from simba.data_processors.directing_other_animals_calculator import DirectingOtherAnimalsAnalyzer
 from simba.mixins.config_reader import ConfigReader
 
 class DirectingOtherAnimalsVisualizerMultiprocess(ConfigReader, PlottingMixin):
     """
     Class for visualizing when animals are directing towards body-parts of other animals using multiprocessing.
 
-    > Note: Requires the pose-estimation data for the left ear, right ears and nose of individual animals.
+    .. important::
+       Requires the pose-estimation data for the left ear, right ears and nose of individual animals.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    video_name: str
-        Video to visualize directionality for (e.g., ``My_video.mp4``)
-    style_attr: dict
-        Video style attribitions.
-    core_cnt: int
-        How many cores to use to create the video.
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str video_name: Video to visualize directionality for in the project_folder/videos directory (e.g., ``My_video.mp4``)
+    :parameter dict style_attr: Video style attribitions (colors and sizes etc.)
+    :parameter dict core_cnt: How many cores to use to create the video.
 
     .. note::
-        Requires the pose-estimation data for the ``left ear``, ``right ear`` and ``nose`` of
-        each individual animals. `YouTube example of expected output <https://youtu.be/4WXs3sKu41I>`__.
+        `Example of expected output <https://www.youtube.com/watch?v=d6pAatreb1E&list=PLi5Vwf0hhy1R6NDQJ3U28MOUJPfl2YWYl&index=22`_.
 
     Examples
     -----
     >>> style_attr = {'Show_pose': True, 'Pose_circle_size': 3, "Direction_color": 'Random', 'Direction_thickness': 4, 'Highlight_endpoints': True}
     >>> directing_visualizer = DirectingOtherAnimalsVisualizerMultiprocess(config_path='project_folder/project_config.ini', video_name='Testing_Video_3.mp4', style_attr=style_attr)
     >>> directing_visualizer.run()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/clf_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,54 +14,42 @@
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_int, check_that_column_exist , check_if_filepath_list_is_empty
 from simba.utils.read_write import get_video_meta_data, get_fn_ext, read_df
 from simba.utils.data import detect_bouts
 
 class ClassifierValidationClips(ConfigReader):
     """
-    Class for creating video clips of classified events. Helpful for faster detection of false positive event bouts.
+    Create video clips of classified events for detection of false positive event bouts.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    window: int
-        Number of seconds before and after the event bout that should be included in the output video.
-    clf_name: str
-        Name of the classifier to create validation videos for.
-    clips: bool
-        If True, creates individual video file clips for each validation bout.
-    text_clr: tuple
-        Color of text overlay in BGR
-    highlight_clr: None or tuple,
-        Color of text when probability values are above threshold. If None, same as text_clr.
-    video_speed: float,
-        FPS rate in relation to original video. E.g., the same as original video if 1.0.
-    concat_video: bool
-        If True, creates a single video including all events bouts for each video.
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter int window: Number of seconds before and after the event bout that should be included in the output video.
+    :parameter str clf_name: Name of the classifier to create validation videos for.
+    :parameter bool clips: If True, creates individual video file clips for each validation bout.
+    :parameter Tuple[int, int, int] text_clr: Color of text overlay in BGR.
+    :parameter Optional[Tuple[int, int, int]] highlight_clr: Color of text when probability values are above threshold. If None, same as text_clr.
+    :parameter float video_speed:  FPS rate in relation to original video. E.g., the same as original video if 1.0. Default: 1.0.
+    :parameter bool concat_video:  If True, creates a single video including all events bouts for each video. Default: False.
 
-    Notes
-    ----------
-    `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/classifier_validation.md#classifier-validation>`_.
+    .. note::
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/classifier_validation.md#classifier-validation>`_.
 
     Examples
     ----------
-    >>> clf_validator = ClassifierValidationClips(config_path='MyProjectConfigPath', window=5, clf_name='Attack', text_clr=(255,255,0), clips=False, concat_video=True)
-    >>> clf_validator.run()
+    >>> _ = ClassifierValidationClips(config_path='MyProjectConfigPath', window=5, clf_name='Attack', text_clr=(255,255,0), clips=False, concat_video=True).run()
     """
 
     def __init__(self,
                  config_path: str,
                  window: int,
                  clf_name: str,
                  clips: bool,
-                 text_clr: Tuple[int, int, int],
-                 concat_video: bool,
-                 video_speed: float,
                  data_paths: List[str],
+                 text_clr: Tuple[int, int, int],
+                 concat_video: bool = False,
+                 video_speed: float = 1.0,
                  highlight_clr: Optional[Tuple[int, int, int]] = None):
 
         super().__init__(config_path=config_path)
         if (not clips) and (not concat_video):
             raise NoSpecifiedOutputError(msg='Please select to create clips and/or a concatenated video')
 
         check_int(name='Time window', value=window)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_file_exist_and_readable
 from simba.utils.enums import Formats, Paths
 from simba.roi_tools.ROI_feature_analyzer import ROIFeatureCreator
 
 class ROIfeatureVisualizerMultiprocess(ConfigReader, PlottingMixin):
     """
-    Class for visualizing features that depend on the relationships between the location of the animals and user-defined
+    Visualize features that depend on the relationships between the location of the animals and user-defined
     ROIs. E.g., distances to centroids of ROIs, cumulative time spent in ROIs, if animals are directing towards ROIs
     etc.
 
     Parameters
     ----------
     config_path: str
         Path to SimBA project config file in Configparser format
@@ -33,17 +33,16 @@
 
     Notes
     ----------
     `Tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#part-5-visualizing-roi-features>`__.
 
     Examples
     ----------
-    style_attr = {'ROI_centers': True, 'ROI_ear_tags': True, 'Directionality': True, 'Directionality_style': 'Funnel', 'Border_color': (0, 128, 0), 'Pose_estimation': True}
-    roi_feature_visualizer = ROIfeatureVisualizerMultiprocess(config_path='test_/project_folder/project_config.ini', video_name='Together_1.avi', style_attr=style_attr, core_cnt=3)
-    roi_feature_visualizer.create_visualization()
+    >>> style_attr = {'ROI_centers': True, 'ROI_ear_tags': True, 'Directionality': True, 'Directionality_style': 'Funnel', 'Border_color': (0, 128, 0), 'Pose_estimation': True}
+    >>> _ = ROIfeatureVisualizerMultiprocess(config_path='test_/project_folder/project_config.ini', video_name='Together_1.avi', style_attr=style_attr, core_cnt=3).run()
     """
 
     def __init__(self,
                  config_path: str,
                  video_name: str,
                  core_cnt: int,
                  style_attr: dict):
@@ -119,15 +118,15 @@
                 add_spacer += 1
                 if self.roi_directing_viable and self.style_attr['Directionality']:
                     self.loc_dict[animal_name][shape]['directing_text'] = '{} {} {}'.format(shape, animal_name, 'facing')
                     self.loc_dict[animal_name][shape]['directing_text_loc'] = ((self.video_meta_data['width'] + 5), (self.video_meta_data['height'] - (self.video_meta_data['height'] + 10) + self.scalers['spacing_size'] * add_spacer))
                     self.loc_dict[animal_name][shape]['directing_data_loc'] = (int(self.img_w_border_w - (self.img_w_border_w / 8)), (self.video_meta_data['height'] - (self.video_meta_data['height'] + 10) + self.scalers['spacing_size'] * add_spacer))
                     add_spacer += 1
 
-    def create_visualization(self):
+    def run(self):
         """
         Creates and saves visualizations of ROI-based features. Results are stored in the ``project_folder/frames/
         output/ROI_features`` directory  of the SimBA project.
 
         Returns
         ----------
         None
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/data_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,18 @@
 from simba.utils.read_write import get_fn_ext
 
 class DataPlotter(ConfigReader):
     """
     Tabular data visualization of animal movement and distances in the current frame and their aggregate
     statistics.
 
-    Parameters
-    ----------
-    config_path: str path to SimBA project config file in Configparser format
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
-    Notes
-    ----------
-    `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-data-tables`>_.
+    .. note::
+        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-data-tables`>_.
 
     Examples
     -----
     >>> _ = DataPlotter(config_path='MyConfigPath').run()
     """
 
     def __init__(self,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/path_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.printing import stdout_success, SimbaTimer
 
 class PathPlotterSingleCore(ConfigReader, PlottingMixin):
     """
-    Class for creating "path plots" videos and/or images detailing the movement paths of
+    Create "path plots" videos and/or images detailing the movement paths of
     individual animals in SimBA.
 
+    .. note::
+        For improved run-time, see :meth:`simba.path_plotter_mp.PathPlotterMulticore` for multiprocess class.
+
     Parameters
     ----------
     config_path: str
         Path to SimBA project config file in Configparser format
     frame_setting: bool
         If True, individual frames will be created.
     video_setting: bool
@@ -39,16 +42,15 @@
     ----------
     `Visualization tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
     Examples
     ----------
     >>> style_attr = {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': 'White', 'max lines': 100}
     >>> animal_attr = {0: ['Ear_right_1', 'Red']}
-    >>> path_plotter = PathPlotterSingleCore(config_path=r'MyConfigPath', frame_setting=False, video_setting=True, style_attr=style_attr, animal_attr=animal_attr, files_found=['project_folder/csv/machine_results/MyVideo.csv'])
-    >>> path_plotter.create_path_plots()
+    >>> path_plotter = PathPlotterSingleCore(config_path=r'MyConfigPath', frame_setting=False, video_setting=True, style_attr=style_attr, animal_attr=animal_attr, files_found=['project_folder/csv/machine_results/MyVideo.csv']).run()
     """
 
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/distance_plotter_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.read_write import read_df, get_fn_ext, concatenate_videos_in_folder
 
 class DistancePlotterMultiCore(ConfigReader, PlottingMixin):
     """
-     Class for visualizing the distances between pose-estimated body-parts (e.g., two animals) through line
+     Visualize the distances between pose-estimated body-parts (e.g., two animals) through line
      charts. Results are saved as individual line charts, and/or a video of line charts.
+     Uses multiprocessing.
 
      Parameters
      ----------
      config_path: str
          path to SimBA project config file in Configparser format
      frame_setting: bool
          If True, creates individual frames
@@ -33,23 +34,22 @@
      style_attr: dict
         Video style attributes (font sizes, line opacity etc.)
      files_found: list
         Files to visualize
      line_attr: dict[list]
         Representing the body-parts to visualize the distance between and their colors.
 
-    Notes
-    -----
-    `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
+    .. note::
+       `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
     Examples
     -----
     >>> style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 8, 'opacity': 0.5}
     >>> line_attr = {0: ['Center_1', 'Center_2', 'Green'], 1: ['Ear_left_2', 'Ear_left_1', 'Red']}
-    >>> distance_plotter = DistancePlotterMultiCore(config_path=r'/tests_/project_folder/project_config.ini', frame_setting=False, video_setting=True, final_img=True, style_attr=style_attr, line_attr=line_attr,  files_found=['/test_/project_folder/csv/machine_results/Together_1.csv'], core_cnt=5)
+    >>> _ = DistancePlotterMultiCore(config_path=r'/tests_/project_folder/project_config.ini', frame_setting=False, video_setting=True, final_img=True, style_attr=style_attr, line_attr=line_attr,  files_found=['/test_/project_folder/csv/machine_results/Together_1.csv'], core_cnt=5)
 
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/ROI_plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, get_video_meta_data
 from simba.utils.data import create_color_palettes
 
 
 class ROIPlot(ConfigReader, PlottingMixin):
     """
-    Class for visualizing the ROI data (number of entries/exits, time-spent-in etc)
+    Visualize the ROI data (number of entries/exits, time-spent-in etc)
 
     Parameters
     ----------
     config_path: str
         Path to SimBA project config file in Configparser format
     video_path: str
         Name of video to create ROI visualizations for
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/heat_mapper_clf.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.errors import NoSpecifiedOutputError
 
 class HeatMapperClfSingleCore(ConfigReader, PlottingMixin):
-
     """
-    Class for creating heatmaps representing the locations of the classified behavior.
+    Create heatmaps representing the locations of the classified behavior.
+    For improved run-time, see :meth:`simba.heat_mapper_clf_mp.HeatMapperClfMultiprocess` for multiprocess class.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     final_img_setting: bool
         If True, then  create the a single image representing the last frame of the input video
@@ -48,16 +48,15 @@
     Notes
     -----
     `GitHub visualizations tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
     Examples
     -----
 
-    >>> heat_mapper_clf = HeatMapperClfSingleCore(config_path='MyConfigPath', final_img_setting=False, video_setting=True, frame_setting=False, bin_size=50, palette='jet', bodypart='Nose_1', clf_name='Attack', max_scale=20)
-    >>> heat_mapper_clf.create_heatmaps()
+    >>> heat_mapper_clf = HeatMapperClfSingleCore(config_path='MyConfigPath', final_img_setting=False, video_setting=True, frame_setting=False, bin_size=50, palette='jet', bodypart='Nose_1', clf_name='Attack', max_scale=20).run()
 
     """
 
     def __init__(self,
                  config_path: str,
                  final_img_setting: bool,
                  video_setting: bool,
@@ -142,15 +141,15 @@
 
         return clf_array, aspect_ratio
 
     def __calculate_max_scale(self,
                               clf_array: np.array):
         return np.round(np.max(np.max(clf_array[-1], axis=0)), 3)
 
-    def create_heatmaps(self):
+    def run(self):
         '''
         Creates heatmap charts. Results are stored in the `project_folder/frames/heatmaps_classifier_locations`
         directory of SimBA project.
 
         Returns
         ----------
         None
@@ -249,9 +248,9 @@
 #                      style_attr = {'palette': 'jet', 'shading': 'gouraud', 'bin_size': 75, 'max_scale': 'auto'},
 #                      final_img_setting=False,
 #                      video_setting=True,
 #                      frame_setting=False,
 #                      bodypart='Nose_1',
 #                      clf_name='Attack',
 #                      files_found=['/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/csv/machine_results/Together_3.csv'])
-# test.create_heatmaps()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/distance_plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,30 +15,25 @@
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.enums import Formats
 from simba.utils.read_write import read_df, get_fn_ext
 
 class DistancePlotterSingleCore(ConfigReader, PlottingMixin):
     """
-     Class for visualizing the distance between two pose-estimated body-parts (e.g., two animals) through line
-     charts. Results are saved as individual line charts, and/or a video of line charts.
+    Class for visualizing the distance between two pose-estimated body-parts (e.g., two animals) through line
+    charts. Results are saved as individual line charts, and/or videos of line charts.
 
-     Parameters
-     ----------
-     config_path: str
-         path to SimBA project config file in Configparser format
-     frame_setting: bool
-         If True, creates individual frames
-     video_setting: bool
-         If True, creates videos
+    .. note::
+       For better runtime, use :meth:`simba.plotting.distance_plotter_mp.DistancePlotterMultiCore`.
 
+       `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
-    Notes
-    -----
-    `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter bool frame_setting: If True, creates individual frames.
+    :parameter bool video_setting: If True, creates videos
 
     Examples
     -----
     >>> distance_plotter = DistancePlotterSingleCore(config_path=r'MyProjectConfig', frame_setting=False, video_setting=True)
     >>> distance_plotter.create_distance_plot()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 __author__ = "Simon Nilsson"
 
 import warnings
 warnings.filterwarnings('ignore',category=FutureWarning)
 warnings.filterwarnings('ignore',category=DeprecationWarning)
-import pandas as pd
 import numpy as np
-import cv2
 import os
 import platform
 import functools
 import multiprocessing
-import matplotlib
 from typing import Dict, Any
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.data import plug_holes_shortest_bout
 from simba.utils.read_write import get_fn_ext, read_df, write_df, get_video_meta_data, concatenate_videos_in_folder
 from simba.utils.printing import stdout_success
 
 class ValidateModelOneVideoMultiprocess(ConfigReader,
                                         PlottingMixin):
     """
-    Class for creating classifier validation video for a single input video. Results are stored in the
-    `project_folder/frames/output/validation directory`.
+    Create classifier validation video for a single input video. Results are stored in the
+    ``project_folder/frames/output/validation`` directory.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     feature_file_path: str
         path to SimBA file (parquet or CSV) containing pose-estimation and feature fields.
@@ -57,16 +54,19 @@
                  settings: Dict[str, Any]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
 
+
+
         _, self.feature_filename, ext = get_fn_ext(feature_file_path)
         self.discrimination_threshold, self.cores, self.shortest_bout, self.create_gantt, self.settings = float(discrimination_threshold), cores, shortest_bout, create_gantt, settings
+        if self.create_gantt == 'None': self.create_gantt = None
         if not os.path.exists(self.single_validation_video_save_dir): os.makedirs(self.single_validation_video_save_dir)
         _, _, self.fps = self.read_video_info(video_name=self.feature_filename)
         self.clf_name = os.path.basename(model_path).replace('.sav', '')
         self.video_path = self.find_video_of_file(self.video_dir, self.feature_filename)
         self.clf_data_save_path = os.path.join(self.clf_data_validation_dir, self.feature_filename + '.csv')
         self.video_meta_data = get_video_meta_data(video_path=self.video_path)
         self.clf = read_df(file_path=model_path, file_type='pickle')
@@ -143,17 +143,17 @@
         self.__save()
         self.__create_video()
 
 #
 
 
 # test = ValidateModelOneVideoMultiprocess(config_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                              feature_file_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/features_extracted/Together_2.csv',
+#                              feature_file_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/features_extracted/Together_1.csv',
 #                              model_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/models/generated_models/Attack.sav',
 #                              discrimination_threshold=0.6,
 #                              shortest_bout=50,
 #                              cores=6,
 #                              settings={'pose': True, 'animal_names': True, 'styles': None},
-#                              create_gantt='Gantt chart: video')
+#                              create_gantt=None)
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/Directing_animals_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,31 @@
 from simba.utils.lookups import get_color_dict
 from simba.utils.read_write import read_df, get_video_meta_data, get_fn_ext
 from simba.utils.data import create_color_palettes
 
 
 class DirectingOtherAnimalsVisualizer(ConfigReader, PlottingMixin):
     """
-    Class for visualizing when animals are directing towards body-parts of other animals.
+    Visualize when animals are directing towards body-parts of other animals.
 
-    > Note: Requires the pose-estimation data for the left ear, right ears and nose of individual animals.
+    .. important::
+       Requires the pose-estimation data for the left ear, right ears and nose of individual animals.
+       For better runtime, use :meth:`simba.plotting.Directing_animals_visualizer.DirectingOtherAnimalsVisualizerMultiprocess`.
+
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str data_path: path to data file
+    :parameter dict style_attr: Visualisation attributes (colors and sizes etc.)
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    data_path: str
-        path to data file
-    style_attr: dict
-        Visualisation attributes.
-
-    Notes
-    -----
-    Requires the pose-estimation data for the ``left ear``, ``right ear`` and ``nose`` of
-    each individual animals.
-    `YouTube example of expected output <https://youtu.be/4WXs3sKu41I>`__.
+    .. note::
+       `Example of expected output <https://www.youtube.com/watch?v=d6pAatreb1E&list=PLi5Vwf0hhy1R6NDQJ3U28MOUJPfl2YWYl&index=22`_.
 
     Examples
     -----
     >>> style_attr = {'Show_pose': True, 'Pose_circle_size': 3, "Direction_color": 'Random', 'Direction_thickness': 4, 'Highlight_endpoints': True}
-    >>> directing_visualizer = DirectingOtherAnimalsVisualizer(config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini', video_name='Testing_Video_3.mp4', style_attr=style_attr)
-    >>> directing_visualizer.run()
+    >>> _ = DirectingOtherAnimalsVisualizer(config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini', video_name='Testing_Video_3.mp4', style_attr=style_attr).run()
     """
 
 
     def __init__(self,
                  config_path: str,
                  data_path: str,
                  style_attr: dict):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.59.4/simba/plotting/heat_mapper_location_mp.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         video_writer.release()
 
     return group
 
 class HeatMapperLocationMultiprocess(ConfigReader, PlottingMixin):
 
     """
-    Class for creating heatmaps representing the locations of animal body-part
+    Create heatmaps representing the locations of animal body-part
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     final_img_setting: bool
         If True, then  create the a single image representing the last frame of the input video
@@ -93,16 +93,15 @@
     Notes
     -----
     `GitHub visualizations tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
     Examples
     -----
 
-    >>> heat_mapper_clf = HeatMapperLocationMultiprocess(config_path='MyConfigPath', final_img_setting=False, video_setting=True, frame_setting=False, bin_size=50, palette='jet', bodypart='Nose_1', clf_name='Attack', max_scale=20)
-    >>> heat_mapper_clf.create_heatmaps()
+    >>> heat_mapper_clf = HeatMapperLocationMultiprocess(config_path='MyConfigPath', final_img_setting=False, video_setting=True, frame_setting=False, bin_size=50, palette='jet', bodypart='Nose_1', clf_name='Attack', max_scale=20).run()
     """
 
     def __init__(self,
                  config_path: str,
                  final_img_setting: bool,
                  video_setting: bool,
                  frame_setting: bool,
@@ -203,15 +202,15 @@
 
         return location_array, aspect_ratio
 
     def __calculate_max_scale(self,
                               clf_array: np.array):
         return np.round(np.max(np.max(clf_array[-1], axis=0)), 3)
 
-    def create_heatmaps(self):
+    def run(self):
         '''
         Creates heatmap charts. Results are stored in the `project_folder/frames/heatmaps_classifier_locations`
         directory of SimBA project.
 
         Returns
         ----------
         None
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.59.4/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.59.4/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.59.4/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/agg_clf_calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,30 +12,24 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
 
 class AggregateClfCalculator(ConfigReader):
     """
-    Class for calculating aggregate statistics from classification data.
+    Compute aggregate descriptive statistics from classification data.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    data_measures: list
-        Aggregate statistics measures to calculate. OPTIONS: ['Bout count', 'Total event duration (s)',
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter List[str] data_measures: Aggregate statistics measures to calculate. OPTIONS: ['Bout count', 'Total event duration (s)',
         'Mean event bout duration (s)', 'Median event bout duration (s)', 'First event occurrence (s)',
         'Mean event bout interval duration (s)', 'Median event bout interval duration (s)']
-    classifiers: list
-        Classifiers to calculate aggregate statistics for. E.g.,: ['Attack', 'Sniffing']
+    :parameter List[str] classifiers: Classifiers to calculate aggregate statistics for. E.g.,: ['Attack', 'Sniffing']
 
-    Notes
-    ----------
-    `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results`__.
+    .. note::
+       `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results>`__.
 
     Examples
     -----
     >>> clf_log_creator = AggregateClfCalculator(config_path="MyConfigPath", data_measures=['Bout count', 'Total event duration'], classifiers=['Attack', 'Sniffing'])
     >>> clf_log_creator.run()
     >>> clf_log_creator.save()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/interpolation_smoothing.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,33 @@
 from simba.utils.read_write import read_df, write_df, get_video_meta_data, get_fn_ext, find_video_of_file
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.enums import Methods
 from simba.utils.errors import NoFilesFoundError
 
 
 class Interpolate(ConfigReader):
+    """
+    Interpolate missing body-parts in pose-estimation data. "Missing" is defined as either (i) when a single body-parts is None or
+    when all body-parts belonging to an animal are identical (i.e., the same 2D coordinate or all None).
+
+    :parameter str input_path path to pose-estimation data in CSV or parquet format
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter Literal str: Type of interpolation. OPTIONS: 'Animal(s): Nearest', 'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear', 'Body-parts: Quadratic']
+                            See `tutorial for info/images of the different interpolation types <<https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`>__.
+    :parameter bool initial_import_multi_index: If True, the incoming data is multi-index columns dataframes. Default: False.
+
+    .. note::
+       `Interpolation tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
+
+    Examples
+    -----
+    >>> _ = Interpolate(input_path=data_path, config_path=SimBaProjectConfigPath, Method='Animal(s): Nearest')
+    """
+
+
     def __init__(self,
                  input_path: str,
                  config_path: str,
                  method: Literal['Animal(s): Nearest', 'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear', 'Body-parts: Quadratic'],
                  initial_import_multi_index: bool = False):
 
         super().__init__(config_path=config_path, read_video_info=False)
@@ -89,14 +108,31 @@
                 for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
                 df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
             write_df(df=df, file_type=self.file_type, save_path=file_path, multi_idx_header=self.initial_import_multi_index)
             video_timer.stop_timer()
             print(f'Video {video_name} interpolated (elapsed time {video_timer.elapsed_time_str}) ...')
 
 class Smooth(ConfigReader):
+    """
+    Smooth pose-estimation data according to user-defined method.
+
+    :parameter str input_path path to pose-estimation data in CSV or parquet format
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter Literal str: Type of smoothing_method. OPTIONS: '`Gaussian'`, '`Savitzky-Golay`'.
+    :parameter int time_window: Rolling time window in millisecond to use when smoothing. Larger time-windows and greater smoothing.
+    :parameter bool initial_import_multi_index: If True, the incoming data is multi-index columns dataframes. Default: False.
+
+    .. note::
+        `Smoothing tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
+
+    Examples
+    -----
+    >>> _ = Smooth(input_path=data_path, config_path=SimBaProjectConfigPath, smoothing_method='Savitzky-Golay', time_window=300)
+    """
+
     def __init__(self,
                  config_path: str,
                  input_path: str,
                  time_window: int,
                  smoothing_method: Literal['Gaussian', 'Savitzky-Golay'],
                  initial_import_multi_index: bool = False):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/timebins_clf_calculator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os, glob
 from collections import defaultdict
 from typing import List
+try:
+    from typing import Literal
+except:
+    from typing_extensions import Literal
 
 from simba.utils.checks import check_int, check_if_filepath_list_is_empty
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoChoosenMeasurementError
 
 class TimeBinsClfCalculator(ConfigReader):
 
     """
-    Class for aggregating classification results into user-defined time-bins. Results are stored in
+    Computes aggregate classification results in user-defined time-bins. Results are stored in
     the ``project_folder/logs`` directory of the SimBA project`
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    bin_length: int
-        Integer representing the time bin size in seconds
-    measurements: list
-        Aggregate statistic measures to calculate for each time bin. OPTIONS: ['First occurance (s)', 'Event count',
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter int bin_length: Integer representing the time bin size in seconds
+    :parameter List[str] measurements: Aggregate statistic measures calculated for each time bin. OPTIONS: ['First occurance (s)', 'Event count',
         Total event duration (s)', 'Mean event duration (s)', 'Median event duration (s)', 'Mean event interval (s)',
         'Median event interval (s)']
-    classifiers: list
-        Names of classifiers to calculate aggregate statistics in time-bins for. EXAMPLE: ['Attack', 'Sniffing']
+    :parameter List[str] classifiers: Names of classifiers to calculate aggregate statistics in time-bins for. EXAMPLE: ['Attack', 'Sniffing']
+
+    .. note::
+    `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results>`__.
 
     Example
     ----------
-
     >>> timebin_clf_analyzer = TimeBinsClfCalculator(config_path='MyConfigPath', bin_length=15, measurements=['Event count', 'Total event duration (s)'])
     >>> timebin_clf_analyzer.run()
 
     """
-
     def __init__(self,
                  config_path: str,
                  bin_length: int,
-                 measurements: List[str],
+                 measurements: List[Literal['First occurance (s)', 'Event count', 'Total event duration (s)', 'Mean event duration (s)', 'Median event duration (s)', 'Mean event interval (s)', 'Median event interval (s)']],
                  classifiers: List[str]):
 
         super().__init__(config_path=config_path)
         if len(measurements) == 0:
             raise NoChoosenMeasurementError()
         check_int(name='Bin length', value=bin_length, min_value=1)
         self.bin_length, self.measurements, self.classifiers = int(bin_length), measurements, classifiers
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/fsttc_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,24 @@
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.errors import CountError
 from simba.mixins.config_reader import ConfigReader
 
 class FSTTCCalculator(ConfigReader):
     """
-    Class for calculating forward spike-time tiling coefficients between pairs of
+    Compute forward spike-time tiling coefficients between pairs of
     classified behaviors.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    time_window: int
-        Integer representing the time window in seconds
-    behavior_lst: list
-        Behaviors to calculate FSTTC between.
-    create_graphs: bool
-        If True, created violin plots representing each FSTTC
-
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter int time_window: FSTTC hyperparameter; Integer representing the time window in seconds.
+    :parameter List[str] behavior_lst: Behaviors to calculate FSTTC between. FSTTC will be computed for all combinations of behaviors.
+    :parameter bool create_graphs: If True, created violin plots representing each FSTTC. Default: False.
 
-    Notes
-    -----
-    `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/FSTTC.md>`__.
+    .. note::
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/FSTTC.md>`__.
 
     Examples
     -----
     >>> fsttc_calculator = FSTTCCalculator(config_path='MyConfigPath', time_window=2, behavior_lst=['Attack', 'Sniffing'], create_graphs=True)
     >>> fsttc_calculator.run()
 
     References
@@ -48,15 +40,15 @@
     """
 
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  time_window: int,
                  behavior_lst: List[str],
-                 create_graphs: bool):
+                 create_graphs: bool = False):
 
         super().__init__(config_path=config_path)
         self.time_delta = int(time_window)
         self.behavior_lst = behavior_lst
         if len(self.behavior_lst) < 2:
             raise CountError(msg='FSTCC requires at least two behaviors')
         self.graph_status = create_graphs
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/interpolate_pose.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 import numpy as np
 from simba.mixins.config_reader import ConfigReader
 
 class Interpolate(ConfigReader):
 
     '''
-    Class for interpolating missing body-parts in pose-estimation data
+    Interpolate missing body-parts in pose-estimation data.
 
     Parameters
     ----------
     config_file_path: str
         path to SimBA project config file in Configparser format
     in_file: pd.DataFrame
         Pose-estimation data
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/directing_other_animals_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,23 @@
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import read_df, get_fn_ext
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import AnimalNumberError
 
 class DirectingOtherAnimalsAnalyzer(ConfigReader, FeatureExtractionMixin):
     """
-    Class for calculating when animals are directing towards body-parts of other animals. Results are stored in
-    the `project_folder/logs/directionality_dataframes` directory of the SimBA project
+    Calculate when animals are directing towards body-parts of other animals. Results are stored in
+    the ``project_folder/logs/directionality_dataframes`` directory of the SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-
-    Notes
-    -----
-    Requires the pose-estimation data for the ``left ear``, ``right ear`` and ``nose`` of each individual animals.
-    `GitHub documentation <https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#part-3-generating-features-from-roi-data>`__.
-    `Expected output <https://github.com/sgoldenlab/simba/blob/master/misc/Direction_data_example.csv>`__.
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
+    .. important::
+       Requires the pose-estimation data for the ``left ear``, ``right ear`` and ``nose`` of each individual animals.
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#part-3-generating-features-from-roi-data>`__.
+       `Expected output <https://github.com/sgoldenlab/simba/blob/master/misc/Direction_data_example.csv>`__.
 
     Examples
     -----
     >>> directing_analyzer = DirectingOtherAnimalsAnalyzer(config_path='MyProjectConfig')
     >>> directing_analyzer.process_directionality()
     >>> directing_analyzer.create_directionality_dfs()
     >>> directing_analyzer.save_directionality_dfs()
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/timebins_movement_calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,36 +12,35 @@
 from simba.utils.checks import check_that_column_exist, check_if_filepath_list_is_empty, check_int
 from simba.utils.read_write import get_fn_ext, read_df, read_config_entry
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 
 class TimeBinsMovementCalculator(ConfigReader, FeatureExtractionMixin):
     """
-    Class for calculating and aggregating movement statistics into user-defined time-bins.
+    Computes aggregate movement statistics in user-defined time-bins.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    bin_length: int
-        Integer representing the time bin size in seconds
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter int bin_length: Integer representing the time bin size in seconds.
+    :parameter bool plots: If True, creates time-bin line plots representing the movement in each time-bin per video. Results are saved in the ``project_folder/logs/`` sub-directory.
+
+    .. note::
+        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results>`__.
 
     Example
     ----------
-
-    >>> timebin_movement_analyzer = TimeBinsMovementCalculator(config_path='MyConfigPath', bin_length=15, )
+    >>> timebin_movement_analyzer = TimeBinsMovementCalculator(config_path='MyConfigPath', bin_length=15, plots=True)
     >>> timebin_movement_analyzer.run()
 
     """
 
     def __init__(self,
                  config_path: str,
                  bin_length: int,
                  body_parts: List[str],
-                 plots: bool):
+                 plots: bool = False):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.bin_length, self.plots = bin_length, plots
         check_int(name='TIME BIN', value=bin_length, min_value=1)
         self.col_headers, self.bp_dict = [], {}
         for bp_cnt, bp in enumerate(body_parts):
             self.col_headers.extend((f'{bp}_x', f'{bp}_y'))
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/severity_calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,32 +12,27 @@
 from simba.utils.printing import stdout_success
 from simba.utils.warnings import NoDataFoundWarning
 from simba.mixins.config_reader import ConfigReader
 
 
 class SeverityCalculator(ConfigReader):
     """
-    Class for analyzing the `severity` of classification frame events based on how much
-    the animals are moving. Frames are scored as less or more severe at lower and higher movements.
+    Computes the "severity" of classification frame events based on how much
+    the animals are moving. Frames are scored as less or more severe at lower and higher movements, respectively.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    settings: dict
-        how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}.
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter dict settings: how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}.
 
-    Notes
-    ----------
-    `GitHub documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md__.
+    .. note::
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md>`__.
 
     Examples
     ----------
     >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}
-    >>> processor = SeverityProcessor(config_path='project_folder/project_config.ini', settings=settings)
+    >>> processor = SeverityCalculator(config_path='project_folder/project_config.ini', settings=settings)
     >>> processor.run()
     >>> processor.save()
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  settings: Dict):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/pup_retrieval_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,33 +16,39 @@
                                     get_fn_ext,
                                     read_df)
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.data import detect_bouts
 from simba.utils.enums import Paths, ConfigKey, Dtypes
 
 class PupRetrieverCalculator(ConfigReader):
+    """
+    Pup retreival calculator used in ``Winters et al., `Sci Reports`, 2022``
+
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter dict settings: user-defined setting for pup retrieval.
+
+    .. note::
+       `Documentation <https://github.com/sgoldenlab/simba/blob/master/docs/add_on_pup_ret.md>`_
+
+    Examples
+    ----------
+    >>> settings = {'pup_track_p': 0.025, 'dam_track_p': 0.5, 'start_distance_criterion': 80.0, 'carry_frames': 90.0, 'core_nest': 'corenest', 'nest': 'nest', 'dam_name': '1_mother', 'pup_name': '2_pup', 'smooth_function': 'gaussian', 'smooth_factor': 5, 'max_time': 90.0, 'clf_carry': 'carry', 'clf_approach': 'approach', 'clf_dig': 'digging', 'distance_plots': True, 'log': True, 'swarm_plot': True}
+    >>> config_path = '/Users/simon/Downloads/Automated PRT_test/project_folder/project_config.ini'
+    >>> calculator = PupRetrieverCalculator(config_path=config_path, settings=settings)
+    >>> calculator.run()
+
+    References
+    ----------
+    .. [1] Winters et al., Automated procedure to assess pup retrieval in laboratory mice, `Sci Reports`, 2022.
+    """
+
+
     def __init__(self,
                  config_path: str,
                  settings: Dict[str, Union[float, str, bool]]):
-        """
-        Pup retreival calculator used in Winters
-
-        :param config_path: path to SimBA configparser.ConfigParser project_config.ini
-        :param settings: user-defined setting for pup retrieval
-
-        :Example:
-        >>> settings = {'pup_track_p': 0.025, 'dam_track_p': 0.5, 'start_distance_criterion': 80.0, 'carry_frames': 90.0, 'core_nest': 'corenest', 'nest': 'nest', 'dam_name': '1_mother', 'pup_name': '2_pup', 'smooth_function': 'gaussian', 'smooth_factor': 5, 'max_time': 90.0, 'clf_carry': 'carry', 'clf_approach': 'approach', 'clf_dig': 'digging', 'distance_plots': True, 'log': True, 'swarm_plot': True}
-        >>> config_path = '/Users/simon/Downloads/Automated PRT_test/project_folder/project_config.ini'
-        >>> calculator = PupRetrieverCalculator(config_path=config_path, settings=settings)
-        >>> calculator.run()
-
-        References
-        ----------
-        .. [1] Winters et al., Automated procedure to assess pup retrieval in laboratory mice, `Sci Reports`, 2022.
-        """
 
         ConfigReader.__init__(config_path=config_path)
         self.config = read_config_file(config_path=config_path)
         self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
         self.settings, self.datetime = settings, datetime.now().strftime('%Y%m%d%H%M%S')
         self.animal_cnt = read_config_entry(self.config, ConfigKey.GENERAL_SETTINGS.value, ConfigKey.ANIMAL_CNT.value, Dtypes.INT.value)
         self.clf_lst = [settings['clf_approach'], settings['clf_carry'], settings['clf_dig']]
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/pybursts_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 import numpy as np
 import math
 
 def kleinberg_burst_detection(offsets: np.ndarray,
                               s: float,
                               gamma: float):
 
+    """
+    Burst detection using `pyburst <https://pypi.org/project/pybursts/>`_.
+    Private method called by ``simba.data_processors.kleinberg_calculator.KleinbergCalculator``.
+
+    """
+
     offsets = np.array(offsets, dtype=object)
 
     if offsets.size == 1:
         bursts = np.array([0, offsets[0], offsets[0]], ndmin=2, dtype=object)
         return bursts
 
     offsets = np.sort(offsets)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/kleinberg_calculator.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,40 +16,30 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.warnings import KleinbergWarning
 from simba.data_processors.pybursts_calculator import kleinberg_burst_detection
 from simba.utils.enums import Paths
 
 class KleinbergCalculator(ConfigReader):
     '''
-    Class for smoothing classification results using the Kleinberg burst
-    detection algorithm.
+    Smooth classification data using the Kleinberg burst detection algorithm.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    classifier_names: list
-        Classifier names to apply Kleinberg smoothing to.
-    sigma: float
-        Burst detection sigma value. Higher sigma values and fewer, longer, behavioural bursts will be recognised.
-    gamma: float
-        Burst detection gamma value. Higher gamma values and fewer behavioural bursts will be recognised
-    hierarchy: float
-        Burst detection hierarchy level. Higher hierarchy values and fewer behavioural bursts will to be recognised.
-    hierarchical_search: bool
-        If true, then finds the minimum hierarchy where each bout is expressed. Default is False.
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter List[str] classifier_names: Classifier names to apply Kleinberg smoothing to.
+    :parameter float sigma: Burst detection sigma value. Higher sigma values and fewer, longer, behavioural bursts will be recognised. Default: 2.
+    :parameter float gamma: Burst detection gamma value. Higher gamma values and fewer behavioural bursts will be recognised. Default: 0.3.
+    :parameter int hierarchy: Burst detection hierarchy level. Higher hierarchy values and fewer behavioural bursts will to be recognised. Default: 1.
+    :parameter bool hierarchical_search: See `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/kleinberg_filter.md#hierarchical-search-example>`_ Default: False.
 
-    Notes
-    ----------
-    `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/kleinberg_filter.md>`__.
+    .. note::
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/kleinberg_filter.md>`__.
 
     Examples
     ----------
     >>> kleinberg_calculator = KleinbergCalculator(config_path='MySimBAConfigPath', classifier_names=['Attack'], sigma=2, gamma=0.3, hierarchy=2, hierarchical_search=False)
-    >>> kleinberg_calculator.perform_kleinberg()
+    >>> kleinberg_calculator.run()
 
     References
     ----------
 
     .. [1] Kleinberg, Bursty and Hierarchical Structure in Streams, `Data Mining and Knowledge Discovery`,
            vol. 7, pp. 373–397, 2003.
     .. [2] Lee et al., Temporal microstructure of dyadic social behavior during relationship formation in mice, `PLOS One`,
@@ -107,15 +97,15 @@
                 if len(target_hierarchy_in_hierarchies_bout) > 0:
                     results.append(target_hierarchy_in_hierarchies_bout)
             if len(results) > 0:
                 self.clf_bouts_in_hierarchy = pd.concat(results, axis=0).drop(['prior_hierarchy', 'hierarchy_difference'], axis=1)
             else:
                 self.clf_bouts_in_hierarchy = pd.DataFrame(columns=['Video', 'Classifier', 'Hierarchy', 'Start', 'Stop'])
 
-    def perform_kleinberg(self):
+    def run(self):
         '''
         Method to perform Kleinberg smoothing. Results are stored in the `project_folder/csv/targets_inserted` directory.
         Detailed log is saved in the `project_folder/logs/` directory.
 
         Returns
         ----------
         None
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/data_processors/movement_calculator.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,24 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.feature_extractors.perimeter_jit import jitted_centroid
 
 class MovementCalculator(ConfigReader,
                          FeatureExtractionMixin):
     """
-    Class for computing aggregate movement statistics.
+    Compute aggregate movement statistics from pose-estimation data in SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    :parameters str config_path: path to SimBA project config file in Configparser format
 
-    Notes
-    ----------
+    .. note::
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results>`__.
 
     Examples
     ----------
-    >>> movement_processor = MovementCalculator(config_path='MyConfigPath')
+    >>> movement_processor = MovementCalculator(config_path='project_folder/project_config.ini')
     >>> movement_processor.run()
     >>> movement_processor.save()
 
     """
 
     def __init__(self,
                  config_path: str,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.59.4/simba/model/train_rf.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 from simba.utils.enums import (Options,
                                ConfigKey,
                                Dtypes,
                                Methods)
 
 class TrainRandomForestClassifier(ConfigReader, TrainModelMixin):
     """
-    Class for training a single random forest model from hyper-parameter setting and sampling methods
+    Train a single random forest model from hyper-parameter setting and sampling methods
     stored within the SimBA project config .ini file (`global environment`).
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
 
     Example
     ----------
-    >>> model_trainer = TrainSingleModel(config_path='MyConfigPath')
+    >>> model_trainer = TrainRandomForestClassifier(config_path='MyConfigPath')
     >>> model_trainer.perform_sampling()
     >>> model_trainer.train_model()
     >>> model_trainer.save_model()
 
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.59.4/simba/model/inference_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,25 @@
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.errors import NoFilesFoundError
 
 class InferenceBatch(TrainModelMixin,
                      ConfigReader):
 
     """
-    Class for running classifier inference. Results are stored in the `project_folder/csv/machine_results`
+    Run classifier inference. Results are stored in the `project_folder/csv/machine_results`
     directory of the SimBA project.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
 
     Example
     ----------
-    >>> inferencer = RunModel(config_path='MyConfigPath')
-    >>> inferencer.run()
+    >>> _ = InferenceBatch(config_path='MyConfigPath').run()
     """
 
     def __init__(self,
                  config_path: str):
         """
         Method to run classifier inference. Results are stored in the ``project_folder/csv/machine_results`` directory
         of the SimBA project.
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.59.4/simba/model/grid_search_rf.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,25 @@
 from ast import literal_eval
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.train_model_mixin import TrainModelMixin
 
 
 class GridSearchRandomForestClassifier(ConfigReader, TrainModelMixin):
     """
-    Class for grid-searching random forest models from hyperparameter setting and sampling methods
+    Grid-searching random forest models from hyperparameter setting and sampling methods
     stored within the `project_folder/configs` directory of a SimBA project.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
 
     Example
     ----------
-    >>> model_trainer = TrainMultipleModelsFromMeta(config_path='MyConfigPath')
-    >>> model_trainer.run()
+    >>> _ = GridSearchRandomForestClassifier(config_path='MyConfigPath').run()
     """
 
     def __init__(self,
                  config_path: str):
 
         ConfigReader.__init__(self, config_path=config_path)
         TrainModelMixin.__init__(self)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.59.4/simba/model/inference_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 from simba.utils.checks import check_file_exist_and_readable
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.train_model_mixin import TrainModelMixin
 
 class InferenceValidation(ConfigReader, TrainModelMixin):
     """
-    Class for running a single classifier on a single featurized input file. Results are saved within the
-    project_folder/csv/validation directory of the SimBA project.
+    Run a single classifier on a single featurized input file. Results are saved within the
+    ``project_folder/csv/validation`` directory of the SimBA project.
 
     Parameters
     ----------
     config_file_path: str
         path to SimBA project config file in Configparser format
     input_file_path: str
         path to file containing features
@@ -30,15 +30,15 @@
 
     Notes
     -----
 
     Examples
     -----
 
-    >>> ValidateModelRunClf(config_path=r"MyProjectConfigPath", input_file_path=r"FeatureFilePath", clf_path=r"ClassifierPath")
+    >>> InferenceValidation(config_path=r"MyProjectConfigPath", input_file_path=r"FeatureFilePath", clf_path=r"ClassifierPath")
 
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  input_file_path: Union[str, os.PathLike],
                  clf_path: Union[str, os.PathLike]):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from simba.utils.enums import DirNames
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 from simba.utils.errors import ROICoordinatesNotFoundError
 
 class ROITimebinCalculator(ConfigReader):
     """
-    Class for calulating how much time and how many entries animals are making into user-defined ROIs
-    in user-defined time bins. Results are stored in the `project_folder/logs` directory of the SimBA project.
+    Calculate how much time and how many entries animals are making into user-defined ROIs
+    within user-defined time bins. Results are stored in the ``project_folder/logs`` directory of
+    the SimBA project.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     bin_length: int
         length of time bins in seconds.
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from simba.utils.printing import stdout_success
 from simba.mixins.config_reader import ConfigReader
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 
 class ROIMovementAnalyzer(ConfigReader):
     """
 
-    Class for computing movements of individual animals within individual user-defined ROIs.
+    Compute movements of individual animals within user-defined ROIs.
 
     Parameters
     ----------
     config_path: str
         Path to SimBA project config file in Configparser format
 
     Notes
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_define.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from simba.utils.printing import stdout_success
 from simba.utils.lookups import get_color_dict
 from simba.mixins.config_reader import ConfigReader
 
 
 class ROI_definitions(ConfigReader):
     """
-    Class for creating ROI user-interface for drawing user-defined shapes in a video.
+    Launch ROI user-interface for drawing user-defined shapes in a video.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     video_path: str
         path to video file for which ROIs should be defined.
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from simba.utils.errors import NoFilesFoundError, BodypartColumnNotFoundError
 from simba.utils.warnings import NoDataFoundWarning
 from simba.utils.read_write import get_fn_ext, read_df, read_config_entry
 
 class ROIAnalyzer(ConfigReader, FeatureExtractionMixin):
     """
 
-    Class for analyzing movements, entries, exits, and time-spent-in user-defined ROIs. Results are stored in the
+    Analyze movements, entries, exits, and time-spent-in user-defined ROIs. Results are stored in the
     'project_folder/logs' directory of the SimBA project.
 
     Parameters
     ----------
     ini_path: str
         Path to SimBA project config file in Configparser format
     data_path: str or None,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from simba.utils.errors import NoFilesFoundError, NoROIDataError
 from simba.utils.warnings import NoFileFoundWarning
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 
 
 class ROIFeatureCreator(ConfigReader, FeatureExtractionMixin):
     """
-    Class for computing features based on the relationships between the location of the animals and the location of
+    Compute features based on the relationships between the location of the animals and the location of
     user-defined ROIs.
 
     Parameters
     ----------
     config_path: str
         Path to SimBA project config file in Configparser format
 
@@ -84,15 +84,15 @@
         self.roi_analyzer.files_found = self.files_found
         self.all_shape_names = self.roi_analyzer.shape_names
         self.roi_analyzer.run()
         self.roi_analyzer.compute_framewise_distance_to_roi_centroids()
         self.roi_distances_dict = self.roi_analyzer.roi_centroid_distance
         self.roi_entries_df = self.roi_analyzer.detailed_df
         if self.roi_directing_viable:
-            self.directing_analyzer.calc_directing_to_ROIs()
+            self.directing_analyzer.run()
             self.roi_direction_df = self.directing_analyzer.results_df
 
         self.data = {}
         for file_cnt, file_path in enumerate(self.features_files):
             _, self.video_name, _ = get_fn_ext(file_path)
             _, _, self.fps = self.read_video_info(video_name=self.video_name)
             data_df = read_df(file_path, self.file_type)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.read_write import get_fn_ext
 
 class DirectingROIAnalyzer(ConfigReader, FeatureExtractionMixin):
     """
-    Class for computing aggregate statistics for animals are directing towards ROIs.
+    Compute aggregate statistics for animals directing towards ROIs.
 
     Parameters
     ----------
     config_path: str
         Path to SimBA project config file in Configparser format
 
     Notes
     ----------
     `ROI tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial_new.md>`__.
 
     Examples
     ----------
-    >>> roi_directing_calculator = DirectingROIAnalyzer(config_path='MyProjectConfig')
-    >>> roi_directing_calculator.calc_directing_to_ROIs()
-
+    >>> _ = DirectingROIAnalyzer(config_path='MyProjectConfig').run()
     """
 
     def __init__(self,
                  config_path: str,
                  data_path: Optional[str] = None,
                  settings: Optional[dict] = None):
 
@@ -117,15 +115,15 @@
             center = self.shape_info[['centerX' , 'centerY']].values.astype(int)
             roi_lines = np.full((2, 4), np.nan)
             roi_lines[0] = np.array([center[0], center[1] - self.shape_info['radius'], center[0], center[1] + self.shape_info['radius']])
             roi_lines[1] = np.array([center[0] - self.shape_info['radius'], center[1], center[0] + self.shape_info['radius'], center[1]])
 
         return self.ccw(roi_lines=roi_lines, eye_lines=eye_lines, shape_type=self.shape_info['Shape_type'])
 
-    def calc_directing_to_ROIs(self):
+    def run(self):
         """
         Method to calculate directing-towards ROI data
 
         Returns
         -------
         Attribute: pd.DataFrame
             results_df
@@ -178,13 +176,13 @@
                     self.bp_data = self.__format_direction_data()
                     eye_roi_intersections = pd.DataFrame(self.__find_roi_intersections(), columns=['ROI_edge_1_x', 'ROI_edge_1_y', 'ROI_edge_2_x', 'ROI_edge_2_y'])
                     self.bp_data = pd.concat([self.bp_data, eye_roi_intersections], axis=1)
                     self.results_lst.append(self.bp_data)
         self.results_df = pd.concat(self.results_lst, axis=0)
 #
 # test = DirectingROIAnalyzer(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/mouse_open_field/project_folder/project_config.ini')
-# test.calc_directing_to_ROIs()
+# test.run()
 #
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_clf_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from simba.utils.warnings import ROIWarning, NoDataFoundWarning
 from simba.utils.read_write import get_fn_ext, read_config_entry, read_df
 from simba.utils.checks import check_that_column_exist, check_if_filepath_list_is_empty
 
 
 class ROIClfCalculator(ConfigReader):
     """
-    Class for computing aggregate statistics of classification results within user-defined ROIs.
+    Compute aggregate statistics of classification results within user-defined ROIs.
     results are stored in `project_folder/logs` directory of the SimBA project.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.59.4/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/sleap_csv_importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,42 +12,35 @@
 from simba.utils.read_write import write_df, find_video_of_file, get_video_meta_data, get_fn_ext
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import Methods
 
 class SLEAPImporterCSV(ConfigReader, PoseImporterMixin):
 
     """
-    Class for importing SLEAP pose-estimation data into SimBA project.
+    Importing SLEAP pose-estimation data into SimBA project in ``CSV`` format.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    data_folder: str
-        Path to folder containing SLEAP data in `.slp` format.
-    actor_IDs: list
-         Animal names.
-    interpolation_settings: str
-        String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
+    .. note::
+      `Google Colab notebook for converting SLEAP .slp to CSV written by @Toshea111  <https://colab.research.google.com/drive/1EpyTKFHVMCqcb9Lj9vjMrriyaG9SvrPO?usp=sharing>`__.
+      `Example expected SLEAP csv data file for 5 animals / 4 pose-estimated body-parts  <https://github.com/sgoldenlab/simba/blob/master/misc/sleap_csv_example.csv>`__.
+
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str data_folder: Path to folder containing SLEAP data in `csv` format.
+    :parameter List[str] id_lst: Animal names. This will be ignored in one animal projects and default to ``Animal_1``.
+    :parameter str interpolation_settings: String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
         'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear',
         'Body-parts: Quadratic'.
-    smoothing_settings: dict
-        Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
+    :parameter str smoothing_settings: Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
         'Parameters': {'Time_window': '200'}})
 
-    Notes
-    ----------
-    `Google Colab notebook for converting SLEAP .slp to CSV  <https://colab.research.google.com/drive/1EpyTKFHVMCqcb9Lj9vjMrriyaG9SvrPO?usp=sharing>`__.
-    `Example expected SLEAP csv data file for 5 animals / 4 pose-estimated body-parts  <https://github.com/sgoldenlab/simba/blob/master/misc/sleap_csv_example.csv>`__.
-
-
-    Example
+    References
     ----------
+    .. [1] Pereira et al., SLEAP: A deep learning system for multi-animal pose tracking, `Nature Methods`,
+           2022.
 
-    >>> sleap_csv_importer = SLEAPImporterCSV(config_path=r'/Users/simon/Desktop/envs/troubleshooting/slp_1_animal_1_bp/project_folder/project_config.ini', data_folder=r'/Users/simon/Desktop/envs/troubleshooting/slp_1_animal_1_bp/import/temp', actor_IDs=['Termite_1', 'Termite_2', 'Termite_3', 'Termite_4', 'Termite_5'], interpolation_settings="Body-parts: Nearest", smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+    >>> sleap_csv_importer = SLEAPImporterCSV(config_path=r'project_folder/project_config.ini', data_folder=r'data_folder', actor_IDs=['Termite_1', 'Termite_2', 'Termite_3', 'Termite_4', 'Termite_5'], interpolation_settings="Body-parts: Nearest", smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
     >>> sleap_csv_importer.run()
     """
 
     def __init__(self,
                  config_path: str,
                  data_folder: str,
                  id_lst: list,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/sleap_h5_importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,35 @@
 from simba.data_processors.interpolation_smoothing import Smooth, Interpolate
 from simba.utils.errors import BodypartColumnNotFoundError
 from simba.utils.read_write import get_video_meta_data, write_df, find_all_videos_in_project
 from simba.utils.printing import stdout_warning, stdout_success, SimbaTimer
 from simba.utils.enums import Methods
 
 class SLEAPImporterH5(ConfigReader, PoseImporterMixin):
+    """
+    Importing SLEAP pose-estimation data into SimBA project in ``H5`` format
+
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str data_folder: Path to folder containing SLEAP data in `csv` format.
+    :parameter List[str] id_lst: Animal names. This will be ignored in one animal projects and default to ``Animal_1``.
+    :parameter str interpolation_settings: String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
+        'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear',
+        'Body-parts: Quadratic'.
+    :parameter str smoothing_settings: Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
+        'Parameters': {'Time_window': '200'}}
+
+    References
+    ----------
+    .. [1] Pereira et al., SLEAP: A deep learning system for multi-animal pose tracking, `Nature Methods`,
+           2022.
+
+    >>> sleap_h5_importer = SLEAPImporterH5(config_path=r'project_folder/project_config.ini', data_folder=r'data_folder', actor_IDs=['Termite_1', 'Termite_2', 'Termite_3', 'Termite_4', 'Termite_5'], interpolation_settings="Body-parts: Nearest", smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+    >>> sleap_h5_importer.run()
+    """
+
     def __init__(self,
                  config_path: str,
                  data_folder: str,
                  id_lst: list,
                  interpolation_settings: str,
                  smoothing_settings: dict):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/madlc_importer.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,44 +10,35 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import write_df, get_video_meta_data, find_all_videos_in_project
 from simba.utils.enums import Formats, Methods
 from simba.mixins.pose_importer_mixin import PoseImporterMixin
 from simba.utils.printing import stdout_success, SimbaTimer
 
 class MADLCImporterH5(ConfigReader, PoseImporterMixin):
+
     """
-    Class for importing multi-animal deeplabcut (maDLC) pose-estimation data (in H5 format)
+    Importing multi-animal deeplabcut (maDLC) pose-estimation data (in H5 format)
     into a SimBA project in parquet or CSV format.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    data_folder: str
-        Path to folder containing maDLC data in `.h5` format.
-    file_type: str
-        Method used to perform pose-estimation in maDLC. OPTIONS: `skeleton`, `box`, `ellipse`.
-    id_lst: list
-        Animal names.
-    interpolation_settings: str
-        String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str data_folder: Path to folder containing maDLC data in ``.h5`` format.
+    :parameter str file_type: Method used to perform pose-estimation in maDLC. OPTIONS: `skeleton`, `box`, `ellipse`.
+    :parameter str interpolation_setting: String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
         'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear',
         'Body-parts: Quadratic'.
-    smoothing_settings: dict
-        Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
+    :parameter dict smoothing_settings: Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
         'Parameters': {'Time_window': '200'}})
 
     Notes
     -----
     `Multi-animal import tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Multi_animal_pose.md>`__.
 
     Examples
     -----
-    >>> madlc_importer =MADLC_Importer(config_path=r'MyConfigPath', data_folder=r'maDLCDataFolder', file_type='ellipse', id_lst=['Animal_1', 'Animal_2'], interpolation_settings='None', smoothing_settings={'Method': 'None', 'Parameters': {'Time_window': '200'}})
-    >>> madlc_importer.run()
+    >>> _ = MADLCImporterH5(config_path=r'MyConfigPath', data_folder=r'maDLCDataFolder', file_type='ellipse', id_lst=['Animal_1', 'Animal_2'], interpolation_settings='None', smoothing_settings={'Method': 'None', 'Parameters': {'Time_window': '200'}}).run()
 
     References
     ----------
     .. [1] Lauer et al., Multi-animal pose estimation, identification and tracking with DeepLabCut, `Nature Methods`,
            2022.
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/sleap_slp_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,37 +16,37 @@
 from simba.utils.read_write import get_video_meta_data, write_df, find_all_videos_in_project
 from simba.utils.enums import Methods
 
 class SLEAPImporterSLP(ConfigReader, PoseImporterMixin):
     """
     Class for importing SLEAP pose-estimation data into a SimBA project.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    data_folder: str
-        Path to folder containing SLEAP data in `.slp` format.
-    actor_IDs: list
-        Animal names.
-    interpolation_settings: str
-        String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
+    .. note::
+      Importing SLEAP .SLP files into SimBA come at long runtimes. For fater runtimes, use
+      :meth:`simba.pose_importers.sleap_h5_importer.SLEAPImporterH5` or :meth:`simba.pose_importers.sleap_csv_importer.SLEAPImporterCSV`
+
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str data_folder: Path to folder containing SLEAP data in `csv` format.
+    :parameter List[str] id_lst: Animal names. This will be ignored in one animal projects and default to ``Animal_1``.
+    :parameter str interpolation_settings: String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
         'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear',
         'Body-parts: Quadratic'.
-    smoothing_settings: dict
-        Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
-        'Parameters': {'Time_window': '200'}})
+    :parameter str smoothing_settings: Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
+        'Parameters': {'Time_window': '200'}}.
 
     Example
     ----------
-    >>> slp_importer = ImportSLEAP(project_path="MyConfigPath", data_folder=r'MySLPDataFolder', actor_IDs=['Mouse_1', 'Mouse_2'], interpolation_settings="Body-parts: Nearest", smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
-    >>> slp_importer.initate_import_slp()
-    >>> slp_importer.visualize_sleap()
-    >>> slp_importer.perform_interpolation()
-    >>> slp_importer.perform_smothing()
+    >>> slp_importer = SLEAPImporterSLP(project_path="MyConfigPath", data_folder=r'MySLPDataFolder', actor_IDs=['Mouse_1', 'Mouse_2'], interpolation_settings="Body-parts: Nearest", smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+    >>> slp_importer.run()
+
+    References
+    ----------
+    .. [1] Pereira et al., SLEAP: A deep learning system for multi-animal pose tracking, `Nature Methods`,
+           2022.
+
     """
 
 
     def __init__(self,
                  project_path: str,
                  data_folder: str,
                  id_lst: list,
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/import_mars.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from simba.data_processors.interpolate_pose import Interpolate
 from simba.utils.data import smooth_data_gaussian, smooth_data_savitzky_golay
 from simba.utils.read_write import get_fn_ext, write_df, read_config_file, read_project_path_and_file_type
 
 class MarsImporter(object):
 
     """
-    Class for importing two animal BENTO pose-estimation data (in JSON format) into a SimBA project in
+    Import two animal MARS pose-estimation data (in JSON format) into a SimBA project in
     parquet or CSV format.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     data_folder: str
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/dlc_importer_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 __author__ = "Simon Nilsson"
 
 import shutil
 import os, glob
 import pandas as pd
+from typing import Union, List
 
 from simba.data_processors.interpolation_smoothing import Interpolate, Smooth
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import Methods
 from simba.utils.errors import NoFilesFoundError, FileExistError
 from simba.utils.read_write import get_fn_ext, read_config_file, read_project_path_and_file_type, get_number_of_header_columns_in_df
 from simba.utils.checks import check_file_exist_and_readable, check_if_filepath_list_is_empty, check_int, check_if_dir_exists
 from simba.utils.data import smooth_data_savitzky_golay, smooth_data_gaussian
 
-def import_dlc_csv(config_path: str,
-                   source: str) -> list:
+def import_dlc_csv(config_path: Union[str, os.PathLike],
+                   source: str) -> List[str]:
     """
-    Imports file or folder DLC pose-estimation CSV files to SimBA project. Returns list of file paths to the imported files.
+    Imports file or folder of  DLC pose-estimation CSV files to SimBA project.
+    Returns list of file paths to the imported files.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    source: str
-        path to file or folder containing DLC pose-estimation CSV files
-
-    :return
-    ----------
-    list
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str source: path to file or folder containing DLC pose-estimation CSV files
+    :return List[str]: Paths of imported files.
 
-    Examples
-    ----------
     >>> import_dlc_csv(config_path='project_folder/project_config.ini', source='CSV_import/Together_1.csv')
     >>> ['project_folder/csv/input_csv/Together_1.csv']
     """
 
     config = read_config_file(config_path=config_path)
     project_path, file_type = read_project_path_and_file_type(config=config)
     original_file_name_dir = os.path.join(project_path, 'csv', 'input_csv', 'original_filename')
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.59.4/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -334,131 +334,131 @@
 000014d0: 4701 5001 5201 5401 5501 5601 5f01 6101  G.P.R.T.U.V._.a.
 000014e0: 6301 6401 6501 6e01 7001 7201 7301 7401  c.d.e.n.p.r.s.t.
 000014f0: 7d01 7f01 8101 8201 8301 8c01 8e01 9101  }...............
 00001500: 9201 9301 9401 9d01 a201 ab00 0000 0000  ................
 00001510: 0002 0100 0000 0000 0000 4900 0000 0000  ..........I.....
 00001520: 0000 0000 0000 0000 0001 ac00 0000 0a00  ................
 00001530: 6e00 6f00 5f00 6100 6e00 6900 6d00 6100  n.o._.a.n.i.m.a.
-00001540: 6c00 736d 6f44 4462 6c6f 6200 0000 08bd  l.smoDDblob.....
-00001550: ed7f 0bcf e1c4 4100 0000 0a00 6e00 6f00  ......A.....n.o.
+00001540: 6c00 736d 6f44 4462 6c6f 6200 0000 083e  l.smoDDblob....>
+00001550: a4ce dfcb eac4 4100 0000 0a00 6e00 6f00  ......A.....n.o.
 00001560: 5f00 6100 6e00 6900 6d00 6100 6c00 736d  _.a.n.i.m.a.l.sm
-00001570: 6f64 4462 6c6f 6200 0000 08bd ed7f 0bcf  odDblob.........
-00001580: e1c4 4100 0000 0a00 6e00 6f00 5f00 6100  ..A.....n.o._.a.
+00001570: 6f64 4462 6c6f 6200 0000 083e a4ce dfcb  odDblob....>....
+00001580: eac4 4100 0000 0a00 6e00 6f00 5f00 6100  ..A.....n.o._.a.
 00001590: 6e00 6900 6d00 6100 6c00 7370 6831 5363  n.i.m.a.l.sph1Sc
 000015a0: 6f6d 7000 0000 0000 0030 0000 0000 0a00  omp......0......
 000015b0: 6e00 6f00 5f00 6100 6e00 6900 6d00 6100  n.o._.a.n.i.m.a.
 000015c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000015d0: 0000 0a00 7300 6300 6800 6500 6d00 6100  ....s.c.h.e.m.a.
 000015e0: 7400 6900 6300 7362 7773 7062 6c6f 6200  t.i.c.sbwspblob.
 000015f0: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 00001600: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 00001610: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
 00001620: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
 00001630: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
 00001640: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
 00001650: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
 00001660: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00001670: 095f 1019 7b7b 3135 392c 2031 3233 7d2c  ._..{{159, 123},
-00001680: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
+00001670: 095f 1019 7b7b 3133 372c 2031 3433 7d2c  ._..{{137, 143},
+00001680: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
 00001690: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
 000016a0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 000016b0: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
 000016c0: 0a00 7300 6300 6800 6500 6d00 6100 7400  ..s.c.h.e.m.a.t.
 000016d0: 6900 6300 736c 6731 5363 6f6d 7000 0000  i.c.slg1Scomp...
-000016e0: 0000 0648 0300 0000 0a00 7300 6300 6800  ...H......s.c.h.
+000016e0: 0000 0627 ff00 0000 0a00 7300 6300 6800  ...'......s.c.h.
 000016f0: 6500 6d00 6100 7400 6900 6300 736c 7376  e.m.a.t.i.c.slsv
 00001700: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
-00001710: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
-00001720: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
-00001730: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-00001740: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-00001750: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-00001760: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-00001770: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-00001780: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-00001790: 4461 7465 7310 0109 ab0c 151a 1f23 282d  Dates........#(-
-000017a0: 3237 3c41 d40d 0e0f 100a 120a 1457 7669  27<A.........Wvi
-000017b0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
-000017c0: 6e64 696e 675a 6964 656e 7469 6669 6572  ndingZidentifier
-000017d0: 0911 0127 0954 6e61 6d65 d40d 0e0f 1016  ...'.Tname......
-000017e0: 1716 1908 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
-000017f0: d40d 0e0f 100a 1c16 1e09 10b5 085c 6461  .............\da
-00001800: 7465 4d6f 6469 6669 6564 d40d 0e0f 1016  teModified......
-00001810: 1c16 2208 085b 6461 7465 4372 6561 7465  .."..[dateCreate
-00001820: 64d4 0d0e 0f10 0a25 1627 0910 6108 5473  d......%.'..a.Ts
-00001830: 697a 65d4 0d0e 0f10 0a2a 0a2c 0910 7309  ize......*.,..s.
-00001840: 546b 696e 64d4 0d0e 0f10 162f 0a31 0810  Tkind....../.1..
-00001850: 6409 556c 6162 656c d40d 0e0f 1016 340a  d.Ulabel......4.
-00001860: 3608 104b 0957 7665 7273 696f 6ed4 0d0e  6..K.Wversion...
-00001870: 0f10 1639 0a3b 0811 012c 0958 636f 6d6d  ...9.;...,.Xcomm
-00001880: 656e 7473 d40d 0e0f 1016 3e16 4008 10c8  ents......>.@...
-00001890: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-000018a0: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
-000018b0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
-000018c0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
-000018d0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
-000018e0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
-000018f0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
-00001900: 00de 00e7 00f0 00f1 00f3 00f4 0101 010a  ................
-00001910: 010b 010c 0118 0121 0122 0124 0125 012a  .......!.".$.%.*
-00001920: 0133 0134 0136 0137 013c 0145 0146 0148  .3.4.6.7.<.E.F.H
-00001930: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
-00001940: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
-00001950: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
-00001960: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
+00001710: 30d8 0102 0304 0506 0708 090a 0b18 4647  0.............FG
+00001720: 0a49 5869 636f 6e53 697a 655f 100f 7368  .IXiconSize_..sh
+00001730: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00001740: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00001750: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+00001760: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+00001770: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00001780: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00001790: 7273 696f 6e23 4030 0000 0000 0000 09ab  rsion#@0........
+000017a0: 0c15 1a1f 2328 2d32 373c 41d4 0d0e 0f10  ....#(-27<A.....
+000017b0: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
+000017c0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+000017d0: 7669 7369 626c 6554 6e61 6d65 1101 c709  visibleTname....
+000017e0: 09d4 0d0e 0f10 1617 1818 5875 6269 7175  ..........Xubiqu
+000017f0: 6974 7910 2308 08d4 0d0e 0f10 1b1c 180a  ity.#...........
+00001800: 5c64 6174 654d 6f64 6966 6965 6410 b508  \dateModified...
+00001810: 09d4 0d0e 0f10 201c 1818 5b64 6174 6543  ...... ...[dateC
+00001820: 7265 6174 6564 0808 d40d 0e0f 1024 2518  reated.......$%.
+00001830: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
+00001840: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
+00001850: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
+00001860: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
+00001870: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
+00001880: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
+00001890: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
+000018a0: 6e65 6410 c808 08d4 0d0e 0f10 421c 1818  ned.........B...
+000018b0: 5964 6174 6541 6464 6564 0808 0823 4028  YdateAdded...#@(
+000018c0: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
+000018d0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
+000018e0: 008c 0095 0096 00a2 00ab 00b6 00bc 00c6  ................
+000018f0: 00ce 00d3 00d6 00d7 00d8 00e1 00ea 00ec  ................
+00001900: 00ed 00ee 00f7 0104 0106 0107 0108 0111  ................
+00001910: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
+00001920: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
+00001930: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
+00001940: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
+00001950: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
+00001960: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00001970: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
 00001980: 01c5 0000 000a 0073 0063 0068 0065 006d  .......s.c.h.e.m
 00001990: 0061 0074 0069 0063 0073 6c73 7670 626c  .a.t.i.c.slsvpbl
 000019a0: 6f62 0000 025e 6270 6c69 7374 3030 d801  ob...^bplist00..
-000019b0: 0203 0405 0607 0809 0a0b 1d45 4647 0a5f  ...........EFG._
-000019c0: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-000019d0: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
-000019e0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-000019f0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-00001a00: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
-00001a10: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
-00001a20: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-00001a30: 6573 1001 09d9 0c0d 0e0f 1011 1213 1415  es..............
-00001a40: 1e23 272b 3035 3a3f 5863 6f6d 6d65 6e74  .#'+05:?Xcomment
-00001a50: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
-00001a60: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
-00001a70: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
-00001a80: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
-00001a90: 6e54 6e61 6d65 d416 1718 191a 1b0a 1d55  nTname.........U
-00001aa0: 696e 6465 7855 7769 6474 6859 6173 6365  indexUwidthYasce
-00001ab0: 6e64 696e 6757 7669 7369 626c 6510 0711  ndingWvisible...
-00001ac0: 012c 0908 d416 1718 191f 201d 1d10 0810  .,........ .....
-00001ad0: c808 08d4 1617 1819 0924 1d0a 10b5 0809  .........$......
-00001ae0: d416 1718 1928 241d 1d10 0208 08d4 1617  .....($.........
-00001af0: 1819 2c2d 1d0a 1003 1061 0809 d416 1718  ..,-.....a......
-00001b00: 1931 320a 1d10 0510 6409 08d4 1617 1819  .12.....d.......
-00001b10: 3637 0a0a 1004 1073 0909 d416 1718 193b  67.....s.......;
-00001b20: 3c0a 1d10 0610 4b09 08d4 1617 1819 4041  <.....K.......@A
-00001b30: 0a0a 1000 1101 2709 0908 2340 2800 0000  ......'...#@(...
-00001b40: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
-00001b50: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-00001b60: 0070 0079 008c 008e 008f 00a2 00ab 00ba  .p.y............
-00001b70: 00c7 00d3 00d8 00de 00e3 00eb 00f0 00f9  ................
-00001b80: 00ff 0105 010f 0117 0119 011c 011d 011e  ................
-00001b90: 0127 0129 012b 012c 012d 0136 0138 0139  .'.).+.,.-.6.8.9
-00001ba0: 013a 0143 0145 0146 0147 0150 0152 0154  .:.C.E.F.G.P.R.T
-00001bb0: 0155 0156 015f 0161 0163 0164 0165 016e  .U.V._.a.c.d.e.n
-00001bc0: 0170 0172 0173 0174 017d 017f 0181 0182  .p.r.s.t.}......
-00001bd0: 0183 018c 018e 0191 0192 0193 0194 019d  ................
-00001be0: 01a2 01ab 0000 0000 0000 0201 0000 0000  ................
+000019b0: 0203 0405 0607 0809 0a0b 1a46 470a 2758  ...........FG.'X
+000019c0: 6963 6f6e 5369 7a65 5f10 0f73 686f 7749  iconSize_..showI
+000019d0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+000019e0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+000019f0: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
+00001a00: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
+00001a10: 5265 6c61 7469 7665 4461 7465 735f 1012  RelativeDates_..
+00001a20: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00001a30: 6f6e 2340 3000 0000 0000 0009 d90c 0d0e  on#@0...........
+00001a40: 0f10 1112 1314 151e 2328 2c31 363b 4058  ........#(,16;@X
+00001a50: 636f 6d6d 656e 7473 5e64 6174 654c 6173  comments^dateLas
+00001a60: 744f 7065 6e65 645c 6461 7465 4d6f 6469  tOpened\dateModi
+00001a70: 6669 6564 5b64 6174 6543 7265 6174 6564  fied[dateCreated
+00001a80: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
+00001a90: 5776 6572 7369 6f6e 546e 616d 65d4 1617  WversionTname...
+00001aa0: 1819 1a1b 0a1d 5776 6973 6962 6c65 5577  ......WvisibleUw
+00001ab0: 6964 7468 5961 7363 656e 6469 6e67 5569  idthYascendingUi
+00001ac0: 6e64 6578 0811 012c 0910 07d4 1617 1819  ndex...,........
+00001ad0: 1a20 1a22 0810 c808 1008 d416 1718 190a  . ."............
+00001ae0: 251a 2709 10b5 0810 01d4 1617 1819 1a25  %.'............%
+00001af0: 1a2b 0808 1002 d416 1718 190a 2e1a 3009  .+............0.
+00001b00: 1061 0810 03d4 1617 1819 1a33 0a35 0810  .a.........3.5..
+00001b10: 6409 1005 d416 1718 190a 380a 3a09 1073  d.........8.:..s
+00001b20: 0910 04d4 1617 1819 1a3d 0a3f 0810 4b09  .........=.?..K.
+00001b30: 1006 d416 1718 190a 420a 4409 1101 c709  ........B.D.....
+00001b40: 1000 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00001b50: 6509 0008 0019 0022 0034 003c 0050 0059  e......".4.<.P.Y
+00001b60: 0064 0077 008c 0095 0096 00a9 00b2 00c1  .d.w............
+00001b70: 00ce 00da 00df 00e5 00ea 00f2 00f7 0100  ................
+00001b80: 0108 010e 0118 011e 011f 0122 0123 0125  ...........".#.%
+00001b90: 012e 012f 0131 0132 0134 013d 013e 0140  .../.1.2.4.=.>.@
+00001ba0: 0141 0143 014c 014d 014e 0150 0159 015a  .A.C.L.M.N.P.Y.Z
+00001bb0: 015c 015d 015f 0168 0169 016b 016c 016e  .\.]._.h.i.k.l.n
+00001bc0: 0177 0178 017a 017b 017d 0186 0187 0189  .w.x.z.{.}......
+00001bd0: 018a 018c 0195 0196 0199 019a 019c 019d  ................
+00001be0: 01a6 01ab 0000 0000 0000 0201 0000 0000  ................
 00001bf0: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
 00001c00: 0000 01ac 0000 000a 0073 0063 0068 0065  .........s.c.h.e
 00001c10: 006d 0061 0074 0069 0063 0073 6d6f 4444  .m.a.t.i.c.smoDD
-00001c20: 626c 6f62 0000 0008 f2a9 afd8 cfea c441  blob...........A
+00001c20: 626c 6f62 0000 0008 7413 24a9 cbfe c441  blob....t.$....A
 00001c30: 0000 000a 0073 0063 0068 0065 006d 0061  .....s.c.h.e.m.a
 00001c40: 0074 0069 0063 0073 6d6f 6444 626c 6f62  .t.i.c.smodDblob
-00001c50: 0000 0008 f2a9 afd8 cfea c441 0000 000a  ...........A....
+00001c50: 0000 0008 7413 24a9 cbfe c441 0000 000a  ....t.$....A....
 00001c60: 0073 0063 0068 0065 006d 0061 0074 0069  .s.c.h.e.m.a.t.i
 00001c70: 0063 0073 7068 3153 636f 6d70 0000 0000  .c.sph1Scomp....
-00001c80: 0006 9000 0000 000a 0073 0063 0068 0065  .........s.c.h.e
+00001c80: 0006 6000 0000 000a 0073 0063 0068 0065  ..`......s.c.h.e
 00001c90: 006d 0061 0074 0069 0063 0073 7653 726e  .m.a.t.i.c.svSrn
 00001ca0: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -607,17 +607,17 @@
 000025e0: 015f 0168 0169 016b 016c 016e 0177 0178  ._.h.i.k.l.n.w.x
 000025f0: 017a 017b 017d 0186 0187 0189 018a 018c  .z.{.}..........
 00002600: 0195 0196 0199 019a 019c 019d 01a6 01ab  ................
 00002610: 0000 0000 0000 0201 0000 0000 0000 0049  ...............I
 00002620: 0000 0000 0000 0000 0000 0000 0000 01ac  ................
 00002630: 0000 0008 0062 0070 005f 006e 0061 006d  .....b.p._.n.a.m
 00002640: 0065 0073 6d6f 4444 626c 6f62 0000 0008  .e.smoDDblob....
-00002650: a3be e06f cee1 c441 0000 0008 0062 0070  ...o...A.....b.p
+00002650: 8878 7882 1bf2 c441 0000 0008 0062 0070  .xx....A.....b.p
 00002660: 005f 006e 0061 006d 0065 0073 6d6f 6444  ._.n.a.m.e.smodD
-00002670: 626c 6f62 0000 0008 a3be e06f cee1 c441  blob.......o...A
+00002670: 626c 6f62 0000 0008 8878 7882 1bf2 c441  blob.....xx....A
 00002680: 0000 0008 0062 0070 005f 006e 0061 006d  .....b.p._.n.a.m
 00002690: 0065 0073 7068 3153 636f 6d70 0000 0000  .e.sph1Scomp....
 000026a0: 0000 3000 0000 0008 0062 0070 005f 006e  ..0......b.p._.n
 000026b0: 0061 006d 0065 0073 7653 726e 6c6f 6e67  .a.m.e.svSrnlong
 000026c0: 0000 0001 0000 0013 0063 006f 006e 0066  .........c.o.n.f
 000026d0: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
 000026e0: 006e 005f 006e 0061 006d 0065 0073 6277  .n._.n.a.m.e.sbw
@@ -721,19 +721,19 @@
 00002d00: 7201 7301 7401 7d01 7f01 8101 8201 8301  r.s.t.}.........
 00002d10: 8c01 8e01 9101 9201 9301 9401 9d01 a201  ................
 00002d20: ab00 0000 0000 0002 0100 0000 0000 0000  ................
 00002d30: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
 00002d40: ac00 0000 1300 6300 6f00 6e00 6600 6900  ......c.o.n.f.i.
 00002d50: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
 00002d60: 5f00 6e00 6100 6d00 6500 736d 6f44 4462  _.n.a.m.e.smoDDb
-00002d70: 6c6f 6200 0000 08ac 24ce 05cf e1c4 4100  lob.....$.....A.
+00002d70: 6c6f 6200 0000 08cb d495 c5cb eac4 4100  lob...........A.
 00002d80: 0000 1300 6300 6f00 6e00 6600 6900 6700  ....c.o.n.f.i.g.
 00002d90: 7500 7200 6100 7400 6900 6f00 6e00 5f00  u.r.a.t.i.o.n._.
 00002da0: 6e00 6100 6d00 6500 736d 6f64 4462 6c6f  n.a.m.e.smodDblo
-00002db0: 6200 0000 08ac 24ce 05cf e1c4 4100 0000  b.....$.....A...
+00002db0: 6200 0000 08cb d495 c5cb eac4 4100 0000  b...........A...
 00002dc0: 1300 6300 6f00 6e00 6600 6900 6700 7500  ..c.o.n.f.i.g.u.
 00002dd0: 7200 6100 7400 6900 6f00 6e00 5f00 6e00  r.a.t.i.o.n._.n.
 00002de0: 6100 6d00 6500 7370 6831 5363 6f6d 7000  a.m.e.sph1Scomp.
 00002df0: 0000 0000 0030 0000 0000 1300 6300 6f00  .....0......c.o.
 00002e00: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
 00002e10: 6900 6f00 6e00 5f00 6e00 6100 6d00 6500  i.o.n._.n.a.m.e.
 00002e20: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
@@ -863,17 +863,17 @@
 000035e0: 015f 0168 0169 016b 016c 016e 0177 0178  ._.h.i.k.l.n.w.x
 000035f0: 017a 017b 017d 0186 0187 0189 018a 018c  .z.{.}..........
 00003600: 0195 0196 0199 019a 019c 019d 01a6 01ab  ................
 00003610: 0000 0000 0000 0201 0000 0000 0000 0049  ...............I
 00003620: 0000 0000 0000 0000 0000 0000 0000 01ac  ................
 00003630: 0000 0008 0062 0070 005f 006e 0061 006d  .....b.p._.n.a.m
 00003640: 0065 0073 6d6f 4444 626c 6f62 0000 0008  .e.smoDDblob....
-00003650: a3be e06f cee1 c441 0000 0008 0062 0070  ...o...A.....b.p
+00003650: 8878 7882 1bf2 c441 0000 0008 0062 0070  .xx....A.....b.p
 00003660: 005f 006e 0061 006d 0065 0073 6d6f 6444  ._.n.a.m.e.smodD
-00003670: 626c 6f62 0000 0008 a3be e06f cee1 c441  blob.......o...A
+00003670: 626c 6f62 0000 0008 8878 7882 1bf2 c441  blob.....xx....A
 00003680: 0000 0008 0062 0070 005f 006e 0061 006d  .....b.p._.n.a.m
 00003690: 0065 0073 7068 3153 636f 6d70 0000 0000  .e.sph1Scomp....
 000036a0: 0000 3000 0000 0008 0062 0070 005f 006e  ..0......b.p._.n
 000036b0: 0061 006d 0065 0073 7653 726e 6c6f 6e67  .a.m.e.svSrnlong
 000036c0: 0000 0001 0000 0013 0063 006f 006e 0066  .........c.o.n.f
 000036d0: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
 000036e0: 006e 005f 006e 0061 006d 0065 0073 6277  .n._.n.a.m.e.sbw
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.59.4/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.59.4/simba/video_processors/video_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,35 +35,25 @@
                                 DirectoryExistError)
 from simba.utils.warnings import (SameInputAndOutputWarning,
                                   FileExistWarning)
 
 
 MAX_FRM_SIZE = 1080, 650
 
-def change_img_format(directory: str,
+def change_img_format(directory: Union[str, os.PathLike],
                       file_type_in: str,
                       file_type_out: str) -> None:
     """
-    Helper to convert file type of all image files in a folder.
+    Convert the file type of all image files within a directory.
 
-    Parameters
-    ----------
-    directory: str
-        Path to directory holding image files
-    file_type_in: str
-        Input file type
-    file_type_out: str
-        Output file type
-
-    Returns
-    -------
-    None
+    :parameter Union[str, os.PathLike] directory: Path to directory holding image files
+    :parameter str file_type_in: Input file type, e.g., 'bmp' or 'png.
+    :parameter str file_type_out: Output file type, e.g., 'bmp' or 'png.
 
-    Example
-    ----------
+    :example:
     >>> _ = change_img_format(directory='MyDirectoryWImages', file_type_in='bmp', file_type_out='png')
 
     """
     if not os.path.isdir(directory):
         raise NotDirectoryError('SIMBA ERROR: {} is not a valid directory'.format(directory))
     files_found = glob.glob(directory + '/*.{}'.format(file_type_in))
     if len(files_found) < 1:
@@ -75,25 +65,21 @@
         im.save(save_name)
         os.remove(file_path)
     stdout_success(msg=f'SIMBA COMPLETE: Files in {directory} directory converted to {file_type_out}')
 
 
 def clahe_enhance_video(file_path: Union[str, os.PathLike]) -> None:
     """
-    Helper to convert a single video file to clahe-enhanced greyscale .avi file. The result is saved with prefix
+    Convert a single video file to clahe-enhanced greyscale .avi file. The result is saved with prefix
     ``CLAHE_`` in the same directory as in the input file.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
-
-    Returns
-    -------
-    None
+    :parameter Union[str, os.PathLike] file_path: Path to video file.
+
+    :example:
+    >>> _ = clahe_enhance_video(file_path: 'project_folder/videos/Video_1.mp4')
     """
 
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, file_ext = get_fn_ext(filepath=file_path)
     save_path = os.path.join(dir, 'CLAHE_{}.avi'.format(file_name))
     video_meta_data = get_video_meta_data(file_path)
     fourcc = cv2.VideoWriter_fourcc(*Formats.AVI_CODEC.value)
@@ -117,33 +103,27 @@
     except Exception as se:
         print(se.args)
         print('CLAHE conversion failed for video {}'.format(file_name))
         cap.release()
         writer.release()
         raise ValueError()
 
-def extract_frame_range(file_path: str,
+def extract_frame_range(file_path: Union[str, os.PathLike],
                         start_frame: int,
                         end_frame: int) -> None:
     """
-    Helper to extract a user-defined range of frames from a video file and save those in png format. Images
+    Extract a user-defined range of frames from a video file to `png` format. Images
     are saved in a folder with the suffix `_frames` within the same directory as the video file.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
-    start_frame: int
-        First frame in range to extract.
-    end_frame: int
-        Last frame in range to extract.
-
-    Returns
-    -------
-    None
+    :parameter Union[str, os.PathLike] file_path: Path to video file
+    :parameter int start_frame: First frame in range to extract
+    :parameter int end_frame: Last frame in range to extract.
+
+    :example:
+    >>> _ = extract_frame_range(file_path='project_folder/videos/Video_1.mp4', start_frame=100, end_frame=500)
     """
 
     check_file_exist_and_readable(file_path=file_path)
     video_meta_data = get_video_meta_data(file_path)
     check_int(name='start frame', value=start_frame, min_value=0)
     file_dir, file_name, file_ext = get_fn_ext(filepath=file_path)
     check_int(name='end frame', value=end_frame, max_value=video_meta_data['frame_count'])
@@ -159,23 +139,22 @@
         print('Frame {} saved (Frame {}/{})'.format(str(frm_number), str(frm_cnt), str(len(frame_range))))
     stdout_success(msg=f'{str(len(frame_range))} frames extracted for video {file_name}')
 
 
 def change_single_video_fps(file_path: Union[str, os.PathLike],
                             fps: int) -> None:
     """
-    Helper to change the fps of a single video file. Results are stored in the same directory as in the input file with
+    Change the fps of a single video file. Results are stored in the same directory as in the input file with
     the suffix ``_fps_new_fps``.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
-    fps: int
-        Fps of the new video file
+    :parameter Union[str, os.PathLike] file_path: Path to video file
+    :parameter int fps: Fps of the new video file.
+
+    :example:
+    >>> _ = change_single_video_fps(file_path='project_folder/videos/Video_1.mp4', fps=15)
     """
 
     check_file_exist_and_readable(file_path=file_path)
     check_int(name='New fps', value=fps)
     video_meta_data = get_video_meta_data(video_path=file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     if int(fps) == int(video_meta_data['fps']):
@@ -186,23 +165,22 @@
     command = str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
     subprocess.call(command, shell=True)
     stdout_success(msg=f'SIMBA COMPLETE: FPS of video {file_name} changed from {str(video_meta_data["fps"])} to {str(fps)} and saved in directory {save_path}')
 
 def change_fps_of_multiple_videos(directory: Union[str, os.PathLike],
                                   fps: int) -> None:
     """
-    Helper to change the fps of video files in a folder. Results are stored in the same directory as in the input files with
+    Change the fps of all video files in a folder. Results are stored in the same directory as in the input files with
     the suffix ``_fps_new_fps``.
 
-    Parameters
-    ----------
-    directory: str
-        Path to directory with video files
-    fps: int
-        Fps of the new video file
+    :parameter Union[str, os.PathLike] directory: Path to video file directory
+    :parameter int fps: Fps of the new video files.
+
+    :example:
+    >>> _ = change_fps_of_multiple_videos(directory='project_folder/videos/Video_1.mp4', fps=15)
     """
 
     if not os.path.isdir(directory):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory))
     check_int(name='New fps', value=fps)
     video_paths = []
     file_paths_in_folder = [f for f in glob.glob(directory + '/*') if os.path.isfile(f)]
@@ -219,45 +197,42 @@
         command = str('ffmpeg -i ') + str(file_path) + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
         subprocess.call(command, shell=True)
         print('Video {} complete...'.format(file_name))
     stdout_success(msg=f'SIMBA COMPLETE: FPS of {str(len(video_paths))} videos changed to { str(fps)}')
 
 def convert_video_powerpoint_compatible_format(file_path: Union[str, os.PathLike]) -> None:
     """
-    Helper to make a powerpoint compatible copy of a video file. The results is stored in the same directory as the
+    Create MS PowerPoint compatible copy of a video file. The result is stored in the same directory as the
     input file with the ``_powerpointready`` suffix.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
+    :parameter Union[str, os.PathLike] file_path: Path to video file.
 
+    :example:
+    >>> _ = convert_video_powerpoint_compatible_format(file_path='project_folder/videos/Video_1.mp4')
     """
 
-
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_powerpointready.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -c:v libx264 -preset slow  -profile:v high -level:v 4.0 -pix_fmt yuv420p -crf 22 -codec:a aac ' + '"' + save_name + '"')
     print('Creating video in powerpoint compatible format... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def convert_to_mp4(file_path: Union[str, os.PathLike]) -> None:
     """
-    Helper to convert a video file to mp4 format. The results is stored in the same directory as the
+    Convert a video file to mp4 format. The result is stored in the same directory as the
     input file with the ``_converted.mp4`` suffix.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
+    :parameter Union[str, os.PathLike] file_path: Path to video file.
 
+    :example:
+    >>> _ = convert_to_mp4(file_path='project_folder/videos/Video_1.avi')
     """
 
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_converted.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
@@ -265,22 +240,21 @@
     print('Converting to mp4... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def video_to_greyscale(file_path: Union[str, os.PathLike]) -> None:
     """
-    Helper to convert a video file to greyscale mp4 format. The results is stored in the same directory as the
+    Convert a video file to greyscale mp4 format. The result is stored in the same directory as the
     input file with the ``_grayscale.mp4`` suffix.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
+    :parameter Union[str, os.PathLike] file_path: Path to video file.
 
+    :example:
+    >>> _ = video_to_greyscale(file_path='project_folder/videos/Video_1.avi')
     """
 
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_grayscale.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
@@ -288,22 +262,21 @@
     print('Converting to greyscale... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def superimpose_frame_count(file_path: Union[str, os.PathLike]) -> None:
     """
-    Helper to superimpose frame count on a video file. The results is stored in the same directory as the
+    Superimpose frame count on a video file. The result is stored in the same directory as the
     input file with the ``_frame_no.mp4`` suffix.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
+    :parameter Union[str, os.PathLike] file_path: Path to video file.
 
+    :example:
+    >>> _ = superimpose_frame_count(file_path='project_folder/videos/Video_1.avi')
     """
 
 
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_frame_no.mp4')
     print('Superimposing frame numbers...... ')
@@ -317,21 +290,22 @@
         command = 'ffmpeg -y -i ' + file_path + ' -vf "drawtext=fontfile={}:'.format(simba_font_path) + "text='%{frame_num}': start_number=1: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" + '" ' + "-c:a copy " + save_name
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def remove_beginning_of_video(file_path: Union[str, os.PathLike],
                               time: int) -> None:
     """
-    Helper to remove N seconds from the beginning of a video file. The results is stored in the same directory as the
+    Remove N seconds from the beginning of a video file. The result is stored in the same directory as the
     input file with the ``_shorten.mp4`` suffix.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
+    :parameter Union[str, os.PathLike] file_path: Path to video file
+    :parameter int time: Number of seconds to remove from the beginning of the video.
+
+    :example:
+    >>> _ = remove_beginning_of_video(file_path='project_folder/videos/Video_1.avi', time=10)
     """
 
     check_file_exist_and_readable(file_path=file_path)
     check_int(name='Cut time', value=time)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_shorten.mp4')
     if os.path.isfile(save_name):
@@ -342,25 +316,23 @@
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def clip_video_in_range(file_path: Union[str, os.PathLike],
                         start_time: str,
                         end_time: str) -> None:
     """
-    Helper to clip video in a specific range. The results is stored in the same directory as the
+    Clip video within a specific range. The result is stored in the same directory as the
     input file with the ``_clipped.mp4`` suffix.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
-    start_time: str
-        Start time of clip in HH:MM:SS format.
-    end_time: str
-        End time of clip in HH:MM:SS format.
+    :parameter Union[str, os.PathLike] file_path: Path to video file
+    :parameter str start_time: Start time in HH:MM:SS format.
+    :parameter str end_time: End time in HH:MM:SS format.
+
+    :example:
+    >>> _ = clip_video_in_range(file_path='project_folder/videos/Video_1.avi', start_time='00:00:05', end_time='00:00:10')
     """
 
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_clipped.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
@@ -369,25 +341,23 @@
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def downsample_video(file_path: Union[str, os.PathLike],
                      video_height: int,
                      video_width: int) -> None:
     """
-    Helper to down-sample a video file. The results is stored in the same directory as the
+    Down-sample a video file. The result is stored in the same directory as the
     input file with the ``_downsampled.mp4`` suffix.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
-    video_height: int
-        The height of the output video.
-    video_width: int
-        The width of the output video.
+    :parameter Union[str, os.PathLike] file_path: Path to video file.
+    :parameter int video_height: height of new video.
+    :parameter int video_width: width of new video.
+
+    :example:
+    >>> _ = downsample_video(file_path='project_folder/videos/Video_1.avi', video_height=600, video_width=400)
     """
 
     check_int(name='Video height', value=video_height)
     check_int(name='Video width', value=video_width)
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_downsampled.mp4')
@@ -399,28 +369,27 @@
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def gif_creator(file_path: str,
                 start_time: int,
                 duration: int,
                 width: int) -> None:
     """
-    Helper to create a sample gif from a video file. The results is stored in the same directory as the
-    input file with the ``.mp4`` file-ending.
+    Create a sample gif from a video file. The result is stored in the same directory as the
+    input file with the ``.gif`` file-ending.
+
+    .. note::
+       The height is auto-computed to retain aspect ratio
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
-    start_time: int
-        The time of the first frame in the gif in seconds.
-    duration: int
-        The duration of the gif in seconds.
-    width: int
-        The width of the gif in pixels. The aspect ratio of the gif will be the same as in the video, i.e.,
-        height is automatically computed.
+    :parameter Union[str, os.PathLike] file_path: Path to video file.
+    :parameter int start_time: Start time of the gif in relation to the video in seconds.
+    :parameter int duration: Duration of the gif.
+    :parameter int width: Width of the gif.
+
+    :example:
+    >>> _ = gif_creator(file_path='project_folder/videos/Video_1.avi', start_time=5, duration=10, width=600)
     """
 
     check_file_exist_and_readable(file_path=file_path)
     check_int(name='Start time', value=start_time)
     check_int(name='Duration', value=duration)
     check_int(name='Width', value=width)
     _ = get_video_meta_data(file_path)
@@ -434,25 +403,23 @@
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def batch_convert_video_format(directory: Union[str, os.PathLike],
                                input_format: str,
                                output_format: str) -> None:
     """
-    Helper to batch convert all videos in a folder of specific format into a different video format. The results are
+    Batch convert all videos in a folder of specific format into a different video format. The results are
     stored in the same directory as the input files.
 
-    Parameters
-    ----------
-    directory: str
-        Path to directory containing video files.
-    input_format: str
-        Format of the input files (e.g., avi)
-    output_format: str
-        Format of the output files (e.g., mp4)
+    :parameter Union[str, os.PathLike] directory: Path to video file directory.
+    :parameter str input_format: Format of the input files (e.g., avi).
+    :parameter str output_format: Format of the output files (e.g., mp4).
+
+    :example:
+    >>> _ = gif_creator(directory='project_folder/videos', input_format='avi', output_format='mp4')
     """
 
     if not os.path.isdir(directory):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory))
     video_paths = []
     file_paths_in_folder = [f for f in glob.glob(directory + '/*') if os.path.isfile(f)]
     for file_path in file_paths_in_folder:
@@ -471,21 +438,21 @@
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
         print('Video {} complete, (Video {}/{})...'.format(file_name, str(file_cnt+1), str(len(video_paths))))
 
     stdout_success(msg=f'SIMBA COMPLETE: {str(len(video_paths))} videos converted in {directory} directory!')
 
 def batch_create_frames(directory: Union[str, os.PathLike]) -> None:
     """
-    Helper to extract all frames for all videos in a directory. Results are stored within sub-directories in the input
+    Extract all frames for all videos in a directory. Results are stored within sub-directories in the input
     directory named according to the video files.
 
-    Parameters
-    ----------
-    directory: str
-        Path to directory containing video files.
+    :parameter str directory: Path to directory containing video files.
+
+    :example:
+    >>> _ = batch_create_frames(directory='project_folder/videos')
     """
 
     if not os.path.isdir(directory):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory))
     video_paths = []
     file_paths_in_folder = [f for f in glob.glob(directory + '/*') if os.path.isfile(f)]
     for file_path in file_paths_in_folder:
@@ -501,21 +468,21 @@
         if not os.path.exists(save_dir): os.makedirs(save_dir)
         video_to_frames(file_path, save_dir, overwrite=True, every=1, chunk_size=1000)
         print('Video {} complete, (Video {}/{})...'.format(file_name, str(file_cnt + 1), str(len(video_paths))))
     stdout_success(msg=f'{str(len(video_paths))} videos converted into frames in {directory} directory!')
 
 def extract_frames_single_video(file_path: Union[str, os.PathLike]) -> None:
     """
-    Helper to extract all frames for a single. Results are stored within a sub-directory in the same
+    Extract all frames for a single. Results are stored within a sub-directory in the same
     directory as the input file.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
+    :parameter str file_path: Path to video file.
+
+    :example:
+    >>> _ = extract_frames_single_video(file_path='project_folder/videos/Video_1.mp4')
     """
 
     check_file_exist_and_readable(file_path=file_path)
     _ = get_video_meta_data(file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     save_dir = os.path.join(dir_name, file_name)
     if not os.path.exists(save_dir): os.makedirs(save_dir)
@@ -523,24 +490,22 @@
     video_to_frames(file_path, save_dir, overwrite=True, every=1, chunk_size=1000)
     stdout_success(msg=f'Video {file_name} converted to images in {dir_name} directory!')
 
 def multi_split_video(file_path: Union[str, os.PathLike],
                       start_times: List[str],
                       end_times: List[str]) -> None:
     """
-    Helper divide a video file into multiple video files from specified start and stop times.
+    Divide a video file into multiple video files from specified start and stop times.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
-    start_times: list
-       Clip start times in [HH:MM:SS] format.
-    end_times: list
-        Clip end times in [HH:MM:SS] format.
+    :parameter str file_path: Path to input video file.
+    :parameter List[str] start_times: Start times in HH:MM:SS format.
+    :parameter List[str] end_times: End times in HH:MM:SS format.
+
+    :example:
+    >>> _ = multi_split_video(file_path='project_folder/videos/Video_1.mp4', start_times=['00:00:05', '00:00:20'], end_times=['00:00:10', '00:00:25'])
     """
 
     check_file_exist_and_readable(file_path=file_path)
     video_meta_data = get_video_meta_data(file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     r = re.compile('.{2}:.{2}:.{2}')
     for start_time_cnt, start_time in enumerate(start_times):
@@ -566,20 +531,21 @@
         command = (str('ffmpeg -i ') + '"' + file_path + '"' + ' -ss ' + start_time + ' -to ' + end_time + ' -async 1 ' + '"' + save_path + '"')
         print('Processing video clip {}...'.format(str(clip_cnt+1)))
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'Video {file_name} converted into {str(len(start_times))} clips in directory {dir_name}!')
 
 def crop_single_video(file_path: Union[str, os.PathLike]) -> None:
     """
-    Helper to crop a single video,
+    Crop a single video using cv2.selectROI interface. Results is saved in the same directory as input video with the
+    ``_cropped.mp4`` suffix`.
+
+    :parameter str file_path: Path to video file.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to video file.
+    :example:
+    >>> _ = crop_single_video(file_path='project_folder/videos/Video_1.mp4')
     """
 
     check_file_exist_and_readable(file_path=file_path)
     _ = get_video_meta_data(video_path=file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     cap = cv2.VideoCapture(file_path)
     cap.set(1, 0)
@@ -599,22 +565,21 @@
     command = str('ffmpeg -y -i ') + '"' + str(file_path) + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
     subprocess.call(command, shell=True)
     stdout_success(f'Video {file_name} cropped and saved at {save_path}')
 
 def crop_multiple_videos(directory_path: Union[str, os.PathLike],
                          output_path: Union[str, os.PathLike]) -> None:
     """
-    Helper to crop multiple videos in a folder according to coordinates defines in one video.
+    Crop multiple videos in a folder according to crop-coordinates defines in the **first** video.
 
-    Parameters
-    ----------
-    directory_path: str
-        Path to directory holding video files.
-    output_path:
-        Directory where to store the cropped videos.
+    :parameter str directory_path: Directory containing input videos.
+    :parameter str output_path: Directory where to save the cropped videos.
+
+    :example:
+    >>> _ = crop_multiple_videos(directory_path='project_folder/videos', output_path='project_folder/videos/my_new_folder')
     """
 
     if not os.path.isdir(directory_path):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory_path))
     video_paths = []
     file_paths_in_folder = [f for f in glob.glob(directory_path + '/*') if os.path.isfile(f)]
     for file_path in file_paths_in_folder:
@@ -647,27 +612,27 @@
 
 def frames_to_movie(directory: Union[str, os.PathLike],
                     fps: int,
                     bitrate: int,
                     img_format: str) -> None:
 
     """
-    Helper to merge frames in a folder to a mp4 video file. Video file is stored in the same directory as the
+    Merge all image files in a folder to a mp4 video file. Video file is stored in the same directory as the
     input directory sub-folder.
 
-    Parameters
-    ----------
-    directory_path: str
-        Path to directory holding images.
-    fps: int
-        Frame rate of output video
-    bitrate:
-        Bitrate of output video
-    img_format:
-        Type of images inside the input directory path.
+    .. note::
+       The Image files have to have ordered numerical names e.g., ``1.png``, ``2.png`` etc...
+
+    :parameter str directory: Directory containing the images.
+    :parameter int fps: The frame rate of the output video.
+    :parameter int bitrate: The bitrate of the output video (e.g., 32000).
+    :parameter str img_format: The format of the input image files (e.g., ``png``).
+
+    :example:
+    >>> _ = crop_multiple_videos(directory_path='project_folder/video_img', fps=15, bitrate=32000, img_format='png')
     """
 
 
     if not os.path.isdir(directory):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory))
     check_int(name='FPS', value=fps)
     check_int(name='BITRATE', value=bitrate)
@@ -686,14 +651,26 @@
 
 
 def video_concatenator(video_one_path: Union[str, os.PathLike],
                        video_two_path: Union[str, os.PathLike],
                        resolution: Union[int, str],
                        horizontal: bool) -> None:
 
+    """
+    Concatenate two videos to a single video
+
+    :param str video_one_path: Path to the first video in the concatenated video
+    :param str video_two_path: Path to the second video in the concatenated video
+    :param int or str resolution: If str, then the name of the video which resolution you want to retain. E.g., `Video_1`. Else int, representinmg the video width (if vertical concat) or height (if horizontal concat). Aspect raio will be retained.
+    :param horizontal: If true, then horizontal concatenation. Else vertical concatenation.
+
+    :example:
+    >>> video_concatenator(video_one_path='project_folder/videos/Video_1.mp4', video_two_path='project_folder/videos/Video_2.mp4', resolution=800, horizontal=True)
+    """
+
 
     for file_path in [video_one_path, video_two_path]:
         check_file_exist_and_readable(file_path=file_path)
         _ = get_video_meta_data(file_path)
     if type(resolution) is int:
         video_meta_data = {}
         if horizontal:
@@ -712,16 +689,26 @@
         command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale=-1:{}[v0];[v0][1:v]hstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['height'], save_path)
     else:
         command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale={}:-1[v0];[v0][1:v]vstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['width'], save_path)
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'Videos concatenated and saved at {save_path}')
 
 
-
 class VideoRotator(ConfigReader):
+    """
+    GUI Tool for rotating video. Rotated video is saved with the ``_rotated_DATETIME.mp4`` suffix.
+
+    :parameter str input_path: Path to video to rotate.
+    :parameter str output_dir: Directory where to save the rotated video.
+
+    :example:
+    >>> VideoRotator(input_path='project_folder/videos/Video_1.mp4', output_dir='project_folder/videos')
+    """
+
+
     def __init__(self,
                  input_path: Union[str, os.PathLike],
                  output_dir: Union[str, os.PathLike]) -> None:
 
         _, self.cpu_cnt  = find_core_cnt()
         self.save_dir = output_dir
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
@@ -819,35 +806,24 @@
         self.main_frm.mainloop()
 
 
 def extract_frames_from_all_videos_in_directory(config_path: Union[str, os.PathLike],
                                                 directory: Union[str, os.PathLike]) -> None:
 
     """
-    Helper to extract all frames from all videos in a directory. The results are saved in the project_folder/frames/input
-    directory of the SimBa project
+    Extract all frames from all videos in a directory. The results are saved in the project_folder/frames/input directory of the SimBA project
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    directory: str
-        path to file or folder containing videos in mp4 and/or avi format
-
-    :return
-    ----------
-    list
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter str directory: path to file or folder containing videos in mp4 and/or avi format.
 
-    Examples
-    ----------
+    :example:
     >>> extract_frames_from_all_videos_in_directory(config_path='project_folder/project_config.ini', source='/tests/test_data/video_tests')
     """
 
-    timer = SimbaTimer()
-    timer.start_timer()
+    timer = SimbaTimer(start=True)
     video_paths, video_types = [], ['.avi', '.mp4']
     files_in_folder = glob.glob(directory + '/*')
     for file_path in files_in_folder:
         _, _, ext = get_fn_ext(filepath=file_path)
         if ext.lower() in video_types:
             video_paths.append(file_path)
     if len(video_paths) == 0:
@@ -864,19 +840,25 @@
         video_to_frames(video_path, save_path, overwrite=True, every=1, chunk_size=1000)
     timer.stop_timer()
     stdout_success(f'Frames created for {str(len(video_paths))} videos', elapsed_time=timer.elapsed_time_str)
 
 
 def copy_img_folder(config_path: Union[str, os.PathLike], source: Union[str, os.PathLike]) -> None:
     """
-    Copy directory of png files to the SimBA project. The directory is stored in the project_folder/frames/input
-    folder of the SimBA project.
+    Copy directory of png files to the SimBA project. The directory is stored in the project_folder/frames/input folder of the SimBA project
+
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter str source: path to image folder outside SimBA project.
+
+    :example:
+    >>> copy_img_folder(config_path='MySimBAprojectConfig', source='/DirectoryWithVideos/')
+
+
     """
-    timer = SimbaTimer()
-    timer.start_timer()
+    timer = SimbaTimer(start=True)
     if not os.path.isdir(source):
         raise NotDirectoryError(msg=f'SIMBA ERROR: source {source} is not a directory.')
     if len(glob.glob(source + '/*.png')) == 0:
         raise NoFilesFoundError(msg=f'SIMBA ERROR: source {source} does not contain any .png files.')
     input_basename = os.path.basename(source)
     config = read_config_file(config_path)
     project_path = read_config_entry(config, ConfigKey.GENERAL_SETTINGS.value, ConfigKey.PROJECT_PATH.value, data_type='folder_path')
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.59.4/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.59.4/simba/video_processors/batch_process_menus.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from simba.utils.errors import InvalidInputError, IntegerError, NoFilesFoundError
 from simba.utils.checks import check_file_exist_and_readable
 from simba.utils.read_write import get_fn_ext, get_video_meta_data
 from simba.ui.tkinter_functions import CreateLabelFrameWithIcon
 
 class BatchProcessFrame(PopUpMixin):
     """
-    Class for creating interactive windows that collect user-inputs for batch processing videos (e.g., cropping,
+    Interactive GUI that collect user-inputs for batch processing videos (e.g., cropping,
     clipping etc.). User-selected output is stored in json file format within the user-defined `output_dir`
 
     Parameters
     ----------
     input_dir: str
         Input folder path containing videos for bath processing.
     output_dir: str
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.59.4/simba/video_processors/multi_cropper.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from simba.utils.checks import  (check_int, check_str, check_if_filepath_list_is_empty)
 from simba.utils.read_write import get_fn_ext
 from simba.utils.enums import Formats
 from simba.utils.errors import CountError, InvalidVideoFileError
 
 class MultiCropper(object):
     """
-    Class for cropping single video into multiple videos
+    Crop single video into multiple videos
 
     Parameters
     ----------
     file_type: str
         File type of input video files (e.g., 'mp4', 'avi')
     input_folder: str
         Folder path holding videos to be cropped.
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.59.4/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.59.4/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.59.4/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.59.4/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from simba.utils.read_write import get_video_meta_data
 from simba.utils.checks import check_file_exist_and_readable
 
 
 class FFMPEGCommandCreator(object):
 
     """
-    Class for executing FFmpeg commands from instructions stored in json format.
-
-
+    Execute FFmpeg commands from instructions stored in json format.
 
     Parameters
     ----------
     json_path: str
         path to json file storing FFmpeg instructions as created by ``simba.batch_process_vides.BatchProcessFrame``.
 
     Notes
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.59.4/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,22 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_df, write_df, get_fn_ext, read_config_entry
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import ConfigKey, Dtypes
 
 class OutlierCorrecterMovement(ConfigReader):
     """
-    Class for detecting and amending outliers in pose-estimation data based on movement sizes of the body-parts
-    in the current frame.
+    Detect and ammend outliers in pose-estimation data based on movement lenghth (Euclidean) of the body-parts
+    in the current frame from preceeding frame. Uses critera stored in the SimBA project project_config.ini
+    under the [Outlier settings] header.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
-    Notes
-    ----------
-    `Outlier correction documentation <https://github.com/sgoldenlab/simba/blob/master/misc/Outlier_settings.pdf>`__.
+    .. note::
+       `Outlier correction documentation <https://github.com/sgoldenlab/simba/blob/master/misc/Outlier_settings.pdf>`__.
 
     Examples
     ----------
     >>> outlier_correcter_movement = OutlierCorrecterMovement(config_path='MyProjectConfig')
     >>> outlier_correcter_movement.run()
 
     """
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.59.4/simba/outlier_tools/outlier_corrector_location.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,30 +7,26 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import read_df, write_df, get_fn_ext, read_config_entry
 
 
 class OutlierCorrecterLocation(ConfigReader):
     """
-    Class for detecting and amending outliers in pose-estimation data based in the location of the body-parts
-    in the current frame relative to the location of the body-part in the preceding frame.
+    Detect and amend outliers in pose-estimation data based in the location of the body-parts
+    in the current frame relative to the location of the body-part in the preceding frame. Uses critera
+    stored in the SimBA project project_config.ini under the [Outlier settings] header.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
-    Notes
-    ----------
-    Outlier correction documentation <https://github.com/sgoldenlab/simba/blob/master/misc/Outlier_settings.pdf>`__.
+    .. note::
+       `Outlier correction documentation <https://github.com/sgoldenlab/simba/blob/master/misc/Outlier_settings.pdf>`_.
 
     Examples
     ----------
-    >>> outlier_correcter_location = OutlierCorrecterLocation(config_path='MyProjectConfig')
-    >>> outlier_correcter_location.run()
+    >>> _ = OutlierCorrecterLocation(config_path='MyProjectConfig').run()
     """
 
     def __init__(self,
                  config_path: str):
 
         super().__init__(config_path=config_path)
         if not os.path.exists(self.outlier_corrected_dir): os.makedirs(self.outlier_corrected_dir)
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.59.4/simba/outlier_tools/skip_outlier_correction.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,21 @@
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
 
 
 class OutlierCorrectionSkipper(ConfigReader):
     """
-    Class for skipping outlier correction in SimBA projects.
+    Skip outlier correction in SimBA projects.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-
-    Notes
-    ----------
+    :parameter str config_path: path to SimBA project config file in Configparser format
 
     Examples
     ----------
-    >>> outlier_correction_skipper = OutlierCorrectionSkipper(config_path='MyProjectConfig')
-    >>> outlier_correction_skipper.run()
-
+    >>> _ = OutlierCorrectionSkipper(config_path='MyProjectConfig').run()
     """
 
     def __init__(self, config_path: str):
 
         ConfigReader.__init__(self, config_path=config_path, read_video_info=False)
         if not os.path.exists(self.outlier_corrected_dir): os.makedirs(self.outlier_corrected_dir)
         check_if_filepath_list_is_empty(filepaths=self.input_csv_paths, error_msg=f"No files found in {self.input_csv_dir}.", )
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.4/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/SimBA.py` & `Simba-UW-tf-dev-1.59.4/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
     def import_ethovision(self):
         ann_folder = askdirectory()
         ImportEthovision(config_path=self.config_path, folder_path=ann_folder)
 
     def import_deepethogram(self):
         ann_folder = askdirectory()
         deepethogram_importer = DeepEthogramImporter(config_path=self.config_path, deep_ethogram_dir=ann_folder)
-        deepethogram_importer.import_deepethogram()
+        deepethogram_importer.run()
 
     def import_noldus_observer(self):
         directory = askdirectory()
         noldus_observer_importer = NoldusObserverImporter(config_path=self.config_path, data_dir=directory)
         noldus_observer_importer.run()
 
     def importMARS(self):
```

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.59.4/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.59.4/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.4/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.59.4/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.59.4/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.59.4/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.59.4/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.59.4/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.59.4/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.59.4/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.59.4/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.59.4/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.59.4/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.4/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.59.4/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.59.4/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.59.4/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.3
+Version: 1.59.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.59.4/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/LICENSE.md` & `Simba-UW-tf-dev-1.59.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/README.md` & `Simba-UW-tf-dev-1.59.4/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.3/setup.py` & `Simba-UW-tf-dev-1.59.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.59.3",
+    version="1.59.4",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

