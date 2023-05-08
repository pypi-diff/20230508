# Comparing `tmp/Simba-UW-tf-dev-1.58.8.tar.gz` & `tmp/Simba-UW-tf-dev-1.58.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.58.8.tar", last modified: Thu May  4 20:00:38 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.58.9.tar", last modified: Mon May  8 03:11:47 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.58.8.tar` & `Simba-UW-tf-dev-1.58.9.tar`

### file list

```diff
@@ -1,482 +1,484 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-03 18:36:16.000000 Simba-UW-tf-dev-1.58.8/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9494 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12626 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6032 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12788 2023-05-01 23:51:03.000000 Simba-UW-tf-dev-1.58.8/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    33955 2023-05-04 19:55:21.000000 Simba-UW-tf-dev-1.58.8/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.58.8/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-28 20:24:21.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    20790 2023-05-04 17:45:45.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3466 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9910 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     6791 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8521 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    43012 2023-05-03 18:35:59.000000 Simba-UW-tf-dev-1.58.8/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42323 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13322 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23897 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.58.8/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41772 2023-05-03 16:41:23.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29306 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    17367 2023-05-01 18:54:03.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    23591 2023-05-04 16:32:32.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60449 2023-05-03 18:46:32.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    55362 2023-05-01 20:52:34.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6858 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7594 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12195 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15289 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12615 2023-05-01 19:51:32.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11617 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.58.8/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20258 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.8/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.58.8/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5837 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)    34295 2023-05-04 19:36:13.000000 Simba-UW-tf-dev-1.58.8/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.8/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    14109 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.58.8/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1573 2023-04-29 19:08:53.000000 Simba-UW-tf-dev-1.58.8/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8385 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     2641 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9140 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10199 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8571 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12404 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    15216 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15872 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12739 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10168 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12806 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12434 2023-05-04 17:45:23.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11263 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15234 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9514 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13232 2023-05-03 18:58:48.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11539 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13164 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9036 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9761 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16321 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6366 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11575 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7444 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12854 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8258 2023-05-04 17:41:51.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4800 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16856 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2945 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9608 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7755 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19187 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.58.8/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18698 2023-05-04 19:56:21.000000 Simba-UW-tf-dev-1.58.8/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-28 20:11:10.000000 Simba-UW-tf-dev-1.58.8/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5917 2023-05-04 19:36:28.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19806 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11373 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11432 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     7349 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_csv_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9719 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6451 2023-05-01 17:30:49.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10945 2023-05-01 17:21:29.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    22015 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    23524 2023-04-30 23:21:29.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    23603 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21021 2023-04-30 23:23:03.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6949 2023-04-28 20:19:13.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    41779 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24645 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7174 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8214 2023-04-28 19:26:14.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2913 2023-04-28 17:39:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64875 2023-05-03 18:36:47.000000 Simba-UW-tf-dev-1.58.8/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.58.8/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18464 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.58.8/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.58.8/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.58.8/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-04 20:00:28.000000 Simba-UW-tf-dev-1.58.8/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-03 18:36:16.000000 Simba-UW-tf-dev-1.58.9/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9493 2023-05-07 18:06:51.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.9/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6032 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.9/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12633 2023-05-08 03:02:50.000000 Simba-UW-tf-dev-1.58.9/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.9/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    33955 2023-05-04 19:55:21.000000 Simba-UW-tf-dev-1.58.9/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.58.9/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-28 20:24:21.000000 Simba-UW-tf-dev-1.58.9/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    20790 2023-05-04 17:45:45.000000 Simba-UW-tf-dev-1.58.9/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3466 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.9/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.9/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.9/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9910 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     6791 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8521 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    43012 2023-05-03 18:35:59.000000 Simba-UW-tf-dev-1.58.9/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42323 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13322 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23897 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.58.9/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42212 2023-05-08 03:07:31.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29499 2023-05-05 16:25:43.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    17367 2023-05-01 18:54:03.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    23591 2023-05-04 16:32:32.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60449 2023-05-03 18:46:32.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    55362 2023-05-01 20:52:34.000000 Simba-UW-tf-dev-1.58.9/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6858 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7594 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12195 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15289 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12615 2023-05-01 19:51:32.000000 Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11617 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.58.9/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20258 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.9/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.58.9/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.9/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5837 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)    34295 2023-05-04 19:36:13.000000 Simba-UW-tf-dev-1.58.9/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)     2335 2023-05-07 19:58:55.000000 Simba-UW-tf-dev-1.58.9/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.9/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    14225 2023-05-07 19:37:44.000000 Simba-UW-tf-dev-1.58.9/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1573 2023-04-29 19:08:53.000000 Simba-UW-tf-dev-1.58.9/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8385 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.9/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     2641 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.9/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9140 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10199 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8571 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12404 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    15294 2023-05-07 18:00:44.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15872 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12739 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10168 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12806 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12434 2023-05-04 17:45:23.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11263 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15234 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9514 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13232 2023-05-03 18:58:48.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11539 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13164 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9761 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16321 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6468 2023-05-07 17:57:11.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11814 2023-05-07 17:03:08.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7444 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12854 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8258 2023-05-04 17:41:51.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4817 2023-05-05 01:13:02.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16856 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2945 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9608 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7755 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19187 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.58.9/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18698 2023-05-04 19:56:21.000000 Simba-UW-tf-dev-1.58.9/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-28 20:11:10.000000 Simba-UW-tf-dev-1.58.9/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5917 2023-05-04 19:36:28.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19806 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11373 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11432 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     7349 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/sleap_csv_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9719 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6451 2023-05-01 17:30:49.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10945 2023-05-01 17:21:29.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    22015 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23524 2023-04-30 23:21:29.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    23603 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21021 2023-04-30 23:23:03.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6944 2023-05-07 17:07:14.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.9/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    41779 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24645 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7174 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8214 2023-04-28 19:26:14.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.9/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2853 2023-05-07 17:25:49.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-07 17:25:49.000000 Simba-UW-tf-dev-1.58.9/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.58.9/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.58.9/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.58.9/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.58.9/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.58.9/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.58.9/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.58.9/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.9/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-08 03:11:46.000000 Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18493 2023-05-08 03:11:46.000000 Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-08 03:11:46.000000 Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-08 03:11:46.000000 Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-08 03:11:46.000000 Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-08 03:11:46.000000 Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.58.9/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.58.9/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.58.9/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-08 03:11:32.000000 Simba-UW-tf-dev-1.58.9/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-08 03:11:47.000000 Simba-UW-tf-dev-1.58.9/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.58.8/PKG-INFO` & `Simba-UW-tf-dev-1.58.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.58.8
+Version: 1.58.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self.run_frm = LabelFrame(self.main_frm, text='RUN', font=Formats.LABELFRAME_HEADER_FORMAT.value, pady=5, padx=5, fg='black')
         self.run_single_video_frm = LabelFrame(self.run_frm, text='SINGLE VIDEO', font=Formats.LABELFRAME_HEADER_FORMAT.value,pady=5, padx=5, fg='black')
         self.run_single_video_btn = Button(self.run_single_video_frm, text='Create single video', fg='blue', command= lambda: self.__initiate_video_creation(multiple_videos=False))
         self.single_video_dropdown = DropDownMenu(self.run_single_video_frm, 'Video:', self.video_lst, '12')
         self.single_video_dropdown.setChoices(self.video_lst[0])
 
         self.run_multiple_videos = LabelFrame(self.run_frm, text='MULTIPLE VIDEO', font=Formats.LABELFRAME_HEADER_FORMAT.value,pady=5, padx=5, fg='black')
-        self.run_multiple_video_btn = Button(self.run_multiple_videos, text='Create multiple videos ({} video(s) found)'.format(str(len(self.video_lst))), fg='blue', command= lambda: self.__initiate_video_creation(multiple_videos=True))
+        self.run_multiple_video_btn = Button(self.run_multiple_videos, text=f'Create multiple videos ({len(self.machine_results_paths)} video(s) found)', fg='blue', command= lambda: self.__initiate_video_creation(multiple_videos=True))
 
         bp_threshold_frm.grid(row=0,sticky=NW)
         self.bp_threshold_lbl.grid(row=0,sticky=NW)
         self.bp_threshold_entry.grid(row=1,sticky=NW)
 
         self.style_settings_frm.grid(row=1,sticky=NW)
         self.auto_compute_font_cb.grid(row=0,sticky=NW)
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/create_project_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         parent_tab.add(self.import_videos_tab, text=f'{"[ Import videos ]": ^20s}', compound='left', image=self.btn_icons['video']['img'])
         parent_tab.add(self.import_data_tab, text=f'{"[ Import tracking data ]": ^20s}', compound='left', image=self.btn_icons['pose']['img'])
         parent_tab.add(self.extract_frms_tab, text=f'{"[ Extract frames ]": ^20s}', compound='left', image=self.btn_icons['frames']['img'])
 
         parent_tab.grid(row=0, column=0, sticky=NW)
 
         self.settings_frm = CreateLabelFrameWithIcon(parent=self.create_project_tab, header='SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.CREATE_PROJECT.value)
-        #self.settings_frm = LabelFrame(self.create_project_tab, text='SETTINGS', fg='black', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5)
         self.general_settings_frm = LabelFrame(self.settings_frm, text='GENERAL PROJECT SETTINGS',fg='black', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5)
 
         self.project_dir_select = FolderSelect(self.general_settings_frm, "Project directory:", lblwidth='25')
         self.project_name_eb = Entry_Box(self.general_settings_frm, 'Project name:', labelwidth='25')
         self.file_type_dropdown = DropDownMenu(self.general_settings_frm,'Workflow file type:', Options.WORKFLOW_FILE_TYPE_OPTIONS.value, '25')
         self.file_type_dropdown.setChoices(choice=Options.WORKFLOW_FILE_TYPE_OPTIONS.value[0])
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.58.9/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.58.9/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.58.9/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.58.9/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.58.9/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.58.9/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.58.9/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.9/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/requirements.txt` & `Simba-UW-tf-dev-1.58.9/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.58.9/simba/mixins/pop_up_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from tkinter import *
 from PIL import ImageTk
 import PIL.Image
 from tkinter import messagebox
 import os
 from simba.pose_importers import trk_importer
+from typing import Tuple
 
 
 from simba.utils.checks import (check_int,
                                 check_str,
                                 check_float,
                                 check_if_dir_exists)
 from simba.pose_importers.read_DANNCE_mat import import_DANNCE_file, import_DANNCE_folder
@@ -25,31 +26,32 @@
 from simba.utils.read_write import find_core_cnt, copy_single_video_to_project, copy_multiple_videos_to_project, read_config_file, read_config_entry
 from simba.ui.tkinter_functions import (hxtScrollbar,
                                         DropDownMenu,
                                         Entry_Box,
                                         FileSelect,
                                         FolderSelect)
 from simba.utils.checks import check_file_exist_and_readable
+from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import CountError
 from simba.utils.lookups import (get_icons_paths,
                                  get_color_dict,
                                  get_named_colors)
 
 class PopUpMixin(object):
     def __init__(self,
                  title: str,
-                 config_path: str or None=None,
-                 size: tuple=(400,400)):
+                 config_path: str or None = None,
+                 size: Tuple[int, int] = (400,400)):
 
         """
         Methods for pop-up windows in SimBa.
 
         :param str title: Pop-up window title
         :param configparser.Configparser config_path: path to SimBA project_config.ini
-        :param tuple size: HxW of the po-up window.
+        :param tuple size: HxW of the pop-up window.
         """
 
         self.main_frm = Toplevel()
         self.main_frm.minsize(size[0], size[1])
         self.main_frm.wm_title(title)
         self.main_frm.lift()
         self.main_frm = Canvas(hxtScrollbar(self.main_frm))
@@ -62,14 +64,17 @@
         self.dpi_options = Options.DPI_OPTIONS.value
         self.colors = get_named_colors()
         self.colors_dict = get_color_dict()
         self.cpu_cnt, _ = find_core_cnt()
         self.menu_icons = get_icons_paths()
         for k in self.menu_icons.keys():
             self.menu_icons[k]['img'] = ImageTk.PhotoImage(image=PIL.Image.open(os.path.join(os.path.dirname(__file__), self.menu_icons[k]['icon_path'])))
+        if config_path:
+            print(config_path)
+            ConfigReader.__init__(self, config_path=config_path, read_video_info=False)
 
     def create_clf_checkboxes(self, main_frm: Frame, clfs: list):
         self.choose_clf_frm = LabelFrame(self.main_frm, text='SELECT CLASSIFIER ANNOTATIONS', font=Formats.LABELFRAME_HEADER_FORMAT.value)
         self.clf_selections = {}
         for clf_cnt, clf in enumerate(clfs):
             self.clf_selections[clf] = BooleanVar(value=False)
             self.calculate_distance_moved_cb = Checkbutton(self.choose_clf_frm, text=clf, variable=self.clf_selections[clf])
@@ -250,14 +255,18 @@
             current_entries.append(entry)
             entry.grid(row=clf_cnt + 2, column=0, sticky=NW)
 
     def create_animal_names_entry_boxes(self, animal_cnt: str):
         check_int(name='NUMBER OF ANIMALS', value=animal_cnt, min_value=0)
         if hasattr(self, 'animal_names_frm'):
             self.animal_names_frm.destroy()
+        if not hasattr(self, 'multi_animal_id_list'):
+            self.multi_animal_id_list = []
+            for i in range(int(animal_cnt)):
+                self.multi_animal_id_list.append(f'Animal {i+1}')
         self.animal_names_frm = Frame(self.animal_settings_frm, pady=5, padx=5)
         self.animal_name_entry_boxes = {}
         for i in range(int(animal_cnt)):
             self.animal_name_entry_boxes[i+1] = Entry_Box(self.animal_names_frm, f'Animal {str(i+1)} name: ', '25')
             if i <= len(self.multi_animal_id_list)-1:
                 self.animal_name_entry_boxes[i+1].entry_set(self.multi_animal_id_list[i])
             self.animal_name_entry_boxes[i+1].grid(row=i, column=0, sticky=NW)
@@ -345,15 +354,15 @@
                     trk_importer(self.config_path, data_path, animal_ids, interpolation, smooth_settings)
                 except Exception as e:
                     messagebox.showerror("Error", str(e))
 
             if data_type == 'CSV (SLEAP)':
                 sleap_csv_importer = SLEAPImporterCSV(config_path=self.config_path,
                                                       data_folder=data_path,
-                                                      actor_IDs=animal_ids,
+                                                      id_lst=animal_ids,
                                                       interpolation_settings=interpolation,
                                                       smoothing_settings=smooth_settings)
                 sleap_csv_importer.run()
 
             if data_type == 'H5 (SLEAP)':
                 sleap_h5_importer = SLEAPImporterH5(config_path=self.config_path,
                                                     data_folder=data_path,
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.58.9/simba/mixins/config_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,18 @@
         roi_dict: dict
         """
         if not os.path.isfile(self.roi_coordinates_path):
             raise NoROIDataError(msg='SIMBA ERROR: No ROI definitions were found in your SimBA project. Please draw some ROIs before analyzing your ROI data')
         else:
             self.rectangles_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_RECTANGLES.value).dropna(how='any')
             self.circles_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_CIRCLES.value).dropna(how='any')
-            self.polygon_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_POLYGONS.value).dropna(how='any')
+            self.polygon_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_POLYGONS.value)
+            if 'Center_XCenter_Y' in self.polygon_df.columns:
+                self.polygon_df = self.polygon_df.drop(['Center_XCenter_Y'], axis=1)
+            self.polygon_df = self.polygon_df.dropna(how='any')
             self.shape_names = list(itertools.chain(self.rectangles_df['Name'].unique(), self.circles_df['Name'].unique(), self.polygon_df['Name'].unique()))
             self.roi_dict = {Keys.ROI_RECTANGLES.value: self.rectangles_df,
                              Keys.ROI_CIRCLES.value: self.circles_df,
                              Keys.ROI_POLYGONS.value: self.polygon_df}
             self.roi_types_names_lst = set()
             for idx, r in self.roi_dict[Keys.ROI_RECTANGLES.value].iterrows():
                 self.roi_types_names_lst.add(f'Rectangle: {r["Name"]}')
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.58.9/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.58.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.58.9/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.58.9/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.58.9/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.58.9/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.58.9/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.58.9/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/enums.py` & `Simba-UW-tf-dev-1.58.9/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.58.9/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/checks.py` & `Simba-UW-tf-dev-1.58.9/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.58.9/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.58.9/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/errors.py` & `Simba-UW-tf-dev-1.58.9/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/data.py` & `Simba-UW-tf-dev-1.58.9/simba/utils/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 from typing import List
 
 from simba.utils.read_write import (get_fn_ext,
                                     read_project_path_and_file_type,
                                     find_video_of_file,
                                     read_df,
                                     write_df,
+                                    read_config_file,
                                     read_config_entry,
                                     get_video_meta_data)
 from simba.utils.checks import check_file_exist_and_readable, check_int
 from simba.utils.errors import NoFilesFoundError,InvalidFileTypeError, CountError
 from simba.utils.printing import stdout_warning
 from simba.utils.enums import ConfigKey, Dtypes
+from simba.utils.lookups import get_bp_config_code_class_pairs
 
 
 
 
 def detect_bouts(data_df: pd.DataFrame,
                  target_lst: List[str],
                  fps: int) -> pd.DataFrame:
@@ -341,15 +343,14 @@
     if not 'Thickness' in shape_df.columns:
         shape_df['Thickness'] = [5] * len(shape_df)
     if not 'Color name' in shape_df.columns:
         shape_df['Color name'] = 'White'
 
     return shape_df
 
-
 def run_user_defined_feature_extraction_class(file_path: str,
                                               config_path: str) -> None:
     """
     Parameters
     ----------
     file_path: str
         Path to .py file holding user-defined feature extraction class
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/utils/printing.py` & `Simba-UW-tf-dev-1.58.9/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/plot_clf_results_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,16 +227,17 @@
             video_timer.stop_timer()
             pool.terminate()
             pool.join()
             print('Video {} complete (elapsed time: {}s)...'.format(self.video_name, video_timer.elapsed_time_str))
 
     def initialize_visualizations(self):
         if self.video_file_path is None:
-            print('Processing {} videos...'.format(str(len(self.files_found))))
-            for file_cnt, file_path in enumerate(self.files_found):
+            self.files_found = self.machine_results_paths
+            print('Processing {} videos...'.format(str(len(self.machine_results_paths))))
+            for file_cnt, file_path in enumerate(self.machine_results_paths):
                 self.file_cnt, self.file_path = file_cnt, file_path
                 self.create_visualizations()
         else:
             print('Processing 1 video...')
             self.file_cnt, file_path = 0, self.video_file_path
             _, file_name, _ = get_fn_ext(file_path)
             self.file_path = os.path.join(self.machine_results_dir, file_name + '.' + self.file_type)
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.58.9/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.58.9/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.58.9/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.58.9/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/agg_clf_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
 from typing import List
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
 
 from simba.utils.checks import check_file_exist_and_readable, check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/interpolation_smoothing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 __author__ = "Simon Nilsson"
 
 from scipy.signal import savgol_filter
 import glob, os
 import numpy as np
 import pandas as pd
 import shutil
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import read_df, write_df, get_video_meta_data, get_fn_ext, find_video_of_file
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.enums import Methods
 from simba.utils.errors import NoFilesFoundError
 
 
 class Interpolate(ConfigReader):
     def __init__(self,
                  input_path: str,
                  config_path: str,
-                 method: str,
+                 method: Literal['Animal(s): Nearest', 'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear', 'Body-parts: Quadratic'],
                  initial_import_multi_index: bool = False):
 
         super().__init__(config_path=config_path, read_video_info=False)
         self.interpolation_type, self.interpolation_method = method.split(':')[0], method.split(':')[1].replace(" ", "").lower()
         if os.path.isdir(input_path):
             self.files_found = glob.glob(input_path + '/*' + self.file_type)
             self.input_dir = input_path
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/severity_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,10 +89,10 @@
                 out_df.loc[len(out_df)] = [video_name, grade, grade_data]
         out_df.to_csv(self.save_path)
         self.timer.stop_timer()
         stdout_success(msg=f'Severity data saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
 
 
 # settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}
-# processor = SeverityProcessor(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini', settings=settings)
+# processor = SeverityCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
 # processor.run()
 # processor.save()
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.58.9/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.58.9/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.58.9/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.58.9/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.58.9/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/madlc_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/misc/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/dlc_importer_csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     original_file_name_dir = os.path.join(project_path, 'csv', 'input_csv', 'original_filename')
     input_csv_dir = os.path.join(project_path, 'csv', 'input_csv')
     imported_files = glob.glob(input_csv_dir + '/*.' + file_type)
     imported_file_names, imported_file_paths = [], []
     for file_path in imported_files:
         _, video_name, _ = get_fn_ext(filepath=file_path)
         imported_file_names.append(video_name)
-    if not os.path.exists(original_file_name_dir): os.makedirs(original_file_name_dir)
+    if not os.path.exists(original_file_name_dir):
+        os.makedirs(original_file_name_dir)
     if os.path.isdir(source):
         csv_files = glob.glob(source + '/*.csv')
         check_if_filepath_list_is_empty(csv_files, error_msg=f'SIMBA ERROR: NO .csv files found in {source} directory.')
     else:
         csv_files = [source]
 
     for file_path in csv_files:
@@ -84,37 +85,36 @@
         print(f'Pose-estimation data for video {video_name} imported to SimBA project (elapsed time: {video_timer.elapsed_time_str}s)...')
     return imported_file_paths
 
 def import_single_dlc_tracking_csv_file(config_path: str,
                                         interpolation_setting: str,
                                         smoothing_setting: str,
                                         smoothing_time: int,
-                                        file_path: str):
+                                        data_dir: str):
     timer = SimbaTimer(start=True)
     if (smoothing_setting == Methods.GAUSSIAN.value) or (smoothing_setting == Methods.SAVITZKY_GOLAY.value):
         check_int(name='SMOOTHING TIME WINDOW', value=smoothing_time, min_value=1)
-    check_file_exist_and_readable(file_path=file_path)
-    imported_file_paths = import_dlc_csv(config_path=config_path, source=file_path)
+    check_file_exist_and_readable(file_path=data_dir)
+    imported_file_paths = import_dlc_csv(config_path=config_path, source=data_dir)
     if interpolation_setting != 'None':
         _ = Interpolate(input_path=imported_file_paths[0], config_path=config_path, method=interpolation_setting, initial_import_multi_index=True)
     if (smoothing_setting == Methods.GAUSSIAN.value) or (smoothing_setting == Methods.SAVITZKY_GOLAY.value):
         _ = Smooth(config_path=config_path, input_path=imported_file_paths[0], time_window=smoothing_time, smoothing_method=smoothing_setting, initial_import_multi_index=True)
     timer.stop_timer()
     stdout_success(msg=f'Imported {str(len(imported_file_paths))} pose estimation file(s)', elapsed_time=timer.elapsed_time_str)
 
 def import_multiple_dlc_tracking_csv_file(config_path: str,
                                           interpolation_setting: str,
                                           smoothing_setting: str,
                                           smoothing_time: int,
-                                          folder_path: str):
+                                          data_dir: str):
     timer = SimbaTimer(start=True)
     if (smoothing_setting == Methods.GAUSSIAN.value) or (smoothing_setting == Methods.SAVITZKY_GOLAY.value):
         check_int(name='SMOOTHING TIME WINDOW', value=smoothing_time, min_value=1)
-    check_if_dir_exists(in_dir=folder_path)
-    imported_file_paths = import_dlc_csv(config_path=config_path, source=folder_path)
-
+    check_if_dir_exists(in_dir=data_dir)
+    imported_file_paths = import_dlc_csv(config_path=config_path, source=data_dir)
     if interpolation_setting != 'None':
         _ = Interpolate(input_path=os.path.dirname(imported_file_paths[0]), config_path=config_path, method=interpolation_setting, initial_import_multi_index=True)
     if (smoothing_setting == Methods.GAUSSIAN.value) or (smoothing_setting == Methods.SAVITZKY_GOLAY.value):
         _ = Smooth(config_path=config_path, input_path=os.path.dirname(imported_file_paths[0]), time_window=int(smoothing_time), smoothing_method=smoothing_setting, initial_import_multi_index=True)
     timer.stop_timer()
     stdout_success(msg=f'Imported {str(len(imported_file_paths))} pose estimation file(s)', elapsed_time=timer.elapsed_time_str)
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.58.9/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.58.9/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.58.9/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.58.9/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.58.9/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.58.9/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.58.9/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.58.9/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.58.9/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.58.9/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.58.9/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.58.9/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.58.9/simba/outlier_tools/skip_outlier_correction.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 
     Notes
     ----------
 
     Examples
     ----------
     >>> outlier_correction_skipper = OutlierCorrectionSkipper(config_path='MyProjectConfig')
-    >>> outlier_correction_skipper.skip_outlier_correction()
+    >>> outlier_correction_skipper.run()
 
     """
 
     def __init__(self, config_path: str):
 
         super().__init__(config_path=config_path)
         if not os.path.exists(self.outlier_corrected_dir):
             os.makedirs(self.outlier_corrected_dir)
         check_if_filepath_list_is_empty(
             filepaths=self.input_csv_paths,
             error_msg=f"No files found in {self.input_csv_dir}.",
         )
         print(f"Processing {len(self.input_csv_paths)} file(s)...")
 
-    def skip_outlier_correction(self):
+    def run(self):
         """
         Standardizes pose-estimation data (i.e., headers) from different pose-estimation packages.
         Results are stored in the project_folder/csv/outlier_corrected_movement_location` directory of
         the SimBA project
         """
 
         for file_cnt, file_path in enumerate(self.input_csv_paths):
@@ -68,8 +68,8 @@
         stdout_success(
             msg=f"Skipped outlier correction for {len(self.input_csv_paths)} files",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
 
 # test = OutlierCorrectionSkipper(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
-# test.skip_outlier_correction()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.9/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/SimBA.py` & `Simba-UW-tf-dev-1.58.9/simba/SimBA.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,15 +547,15 @@
 
     def create_video_info_table(self):
         video_info_tabler = VideoInfoTable(config_path=self.config_path)
         video_info_tabler.create_window()
 
     def initiate_skip_outlier_correction(self):
         outlier_correction_skipper = OutlierCorrectionSkipper(config_path=self.config_path)
-        outlier_correction_skipper.skip_outlier_correction()
+        outlier_correction_skipper.run()
 
 
     def validate_model_first_step(self):
         _ = InferenceValidation(config_path=self.config_path,
                                 input_file_path=self.csvfile.file_path,
                                 clf_path=self.modelfile.file_path)
```

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.58.9/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.58.9/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.9/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.58.9/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.58.9/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.58.9/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.58.9/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.58.9/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.58.9/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.58.9/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.58.9/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.58.9/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.58.9/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.9/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.58.9/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.58.9/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.58.9/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.58.8
+Version: 1.58.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -410,14 +410,15 @@
 simba/utils/data.py
 simba/utils/enums.py
 simba/utils/errors.py
 simba/utils/lookups.py
 simba/utils/printing.py
 simba/utils/read_write.py
 simba/utils/warnings.py
+simba/utils/cli/cli_tools.py
 simba/video_processors/.DS_Store
 simba/video_processors/__init__.py
 simba/video_processors/batch_process_create_ffmpeg_commands.py
 simba/video_processors/batch_process_menus.py
 simba/video_processors/calculate_px_dist.py
 simba/video_processors/extract_frames.py
 simba/video_processors/extract_seqframes.py
```

### Comparing `Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.58.9/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/LICENSE.md` & `Simba-UW-tf-dev-1.58.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/README.md` & `Simba-UW-tf-dev-1.58.9/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.8/setup.py` & `Simba-UW-tf-dev-1.58.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.58.8",
+    version="1.58.9",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

