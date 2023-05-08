# Comparing `tmp/encord-active-0.1.8.tar.gz` & `tmp/encord-active-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-active-0.1.8.tar", max compression
+gzip compressed data, was "encord-active-0.1.9.tar", max compression
```

## Comparing `encord-active-0.1.8.tar` & `encord-active-0.1.9.tar`

### file list

```diff
@@ -1,94 +1,99 @@
--rw-r--r--   0        0        0      203 2022-11-07 20:44:53.456367 encord-active-0.1.8/.env
--rw-r--r--   0        0        0    34523 2022-11-07 20:44:53.456367 encord-active-0.1.8/LICENSE
--rw-r--r--   0        0        0     3073 2022-11-07 20:45:26.492838 encord-active-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/__init__.py
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/__init__.py
--rw-r--r--   0        0        0    57557 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/assets/encord_2_02.png
--rw-r--r--   0        0        0     1064 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/assets/favicon-32x32.png
--rw-r--r--   0        0        0      912 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/colors.py
--rw-r--r--   0        0        0      134 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/components/__init__.py
--rw-r--r--   0        0        0     1953 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/components/bulk_tagging_form.py
--rw-r--r--   0        0        0     2467 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/components/data_tags.py
--rw-r--r--   0        0        0     2240 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/components/individual_tagging.py
--rw-r--r--   0        0        0     1232 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/components/multi_select.py
--rw-r--r--   0        0        0     1396 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/components/sticky/sticky.html
--rw-r--r--   0        0        0      383 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/components/sticky/sticky.py
--rw-r--r--   0        0        0     2219 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/css.py
--rw-r--r--   0        0        0     5965 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/embedding_utils.py
--rw-r--r--   0        0        0     1312 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/indexer.py
--rw-r--r--   0        0        0     1312 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/metric.py
--rw-r--r--   0        0        0     3633 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/page.py
--rw-r--r--   0        0        0     3381 2022-11-07 20:44:53.536368 encord-active-0.1.8/src/encord_active/app/common/state.py
--rw-r--r--   0        0        0     7852 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/common/utils.py
--rw-r--r--   0        0        0      205 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/conf/__init__.py
--rw-r--r--   0        0        0      207 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/conf/logging.py
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/data_quality/__init__.py
--rw-r--r--   0        0        0     2604 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/data_quality/common.py
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/data_quality/sub_pages/__init__.py
--rw-r--r--   0        0        0    17318 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/data_quality/sub_pages/explorer.py
--rw-r--r--   0        0        0     6664 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/data_quality/sub_pages/summary.py
--rw-r--r--   0        0        0      448 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/db/connection.py
--rw-r--r--   0        0        0     3658 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/db/merged_metrics.py
--rw-r--r--   0        0        0     1485 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/db/tags.py
--rw-r--r--   0        0        0      257 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/frontend_components.py
--rw-r--r--   0        0        0      162 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/known-issues.md
--rw-r--r--   0        0        0     3275 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/main.py
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/__init__.py
--rw-r--r--   0        0        0       90 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/components/__init__.py
--rw-r--r--   0        0        0     3212 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/components/false_negative_view.py
--rw-r--r--   0        0        0     2798 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/components/index_view.py
--rw-r--r--   0        0        0     2798 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/components/metric_view.py
--rw-r--r--   0        0        0     1329 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/components/utils.py
--rw-r--r--   0        0        0     7895 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/data.py
--rw-r--r--   0        0        0     8671 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/map_mar.py
--rw-r--r--   0        0        0     1781 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/settings.py
--rw-r--r--   0        0        0     4321 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/__init__.py
--rw-r--r--   0        0        0     2166 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/false_negatives.py
--rw-r--r--   0        0        0     1899 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/false_positives.py
--rw-r--r--   0        0        0     9541 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/metrics.py
--rw-r--r--   0        0        0     7336 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/performance_by_metric.py
--rw-r--r--   0        0        0     1798 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/true_positives.py
--rw-r--r--   0        0        0     2981 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/streamlit_entrypoint.py
--rw-r--r--   0        0        0     5175 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/views/export.py
--rw-r--r--   0        0        0     3477 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/views/getting_started.py
--rw-r--r--   0        0        0      962 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/views/indexes.py
--rw-r--r--   0        0        0     3207 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/app/views/model_assertions.py
--rw-r--r--   0        0        0       92 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/__init__.py
--rw-r--r--   0        0        0       22 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/common/__init__.py
--rw-r--r--   0        0        0     8242 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/common/iterator.py
--rw-r--r--   0        0        0     5705 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/common/metric.py
--rw-r--r--   0        0        0     5708 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/common/prepare.py
--rw-r--r--   0        0        0     2511 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/common/tester.py
--rw-r--r--   0        0        0     9349 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/common/utils.py
--rw-r--r--   0        0        0     8441 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/common/writer.py
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/embeddings/__init__.py
--rw-r--r--   0        0        0     8788 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/embeddings/cnn_embed.py
--rw-r--r--   0        0        0     2077 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/embeddings/hu_embed.py
--rw-r--r--   0        0        0     2632 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/example.py
--rw-r--r--   0        0        0     1868 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/fetch_prebuilt_metrics.py
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/geometric/__init__.py
--rw-r--r--   0        0        0     3073 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/geometric/annotation_duplicates.py
--rw-r--r--   0        0        0     4225 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/geometric/hu_static.py
--rw-r--r--   0        0        0     3115 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/geometric/hu_temporal.py
--rw-r--r--   0        0        0     2174 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/geometric/image_border_closeness.py
--rw-r--r--   0        0        0     6123 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/geometric/object_size.py
--rw-r--r--   0        0        0     5909 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/geometric/occlusion_detection_video.py
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/__init__.py
--rw-r--r--   0        0        0     1580 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/_annotation_time.py
--rw-r--r--   0        0        0     6710 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/high_iou_changing_classes.py
--rw-r--r--   0        0        0     9192 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/img_features.py
--rw-r--r--   0        0        0    10303 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/missing_objects_and_wrong_tracks.py
--rw-r--r--   0        0        0      754 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/object_counting.py
--rw-r--r--   0        0        0     5918 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/import_encord_project.py
--rw-r--r--   0        0        0     3979 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/run_all.py
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/semantic/__init__.py
--rw-r--r--   0        0        0    10085 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/semantic/_class_uncertainty.py
--rw-r--r--   0        0        0     8882 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/semantic/_heatmap_uncertainty.py
--rw-r--r--   0        0        0    13913 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/semantic/img_classification_quality.py
--rw-r--r--   0        0        0     7234 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/metrics/semantic/img_object_quality.py
--rw-r--r--   0        0        0        0 2022-11-07 20:44:53.540368 encord-active-0.1.8/src/encord_active/lib/model_predictions/__init__.py
--rw-r--r--   0        0        0     8902 2022-11-07 20:44:53.544368 encord-active-0.1.8/src/encord_active/lib/model_predictions/importers.py
--rw-r--r--   0        0        0     7858 2022-11-07 20:44:53.544368 encord-active-0.1.8/src/encord_active/lib/model_predictions/iterator.py
--rw-r--r--   0        0        0    19746 2022-11-07 20:44:53.544368 encord-active-0.1.8/src/encord_active/lib/model_predictions/prediction_writer.py
--rw-r--r--   0        0        0     2344 2022-11-07 20:47:59.506952 encord-active-0.1.8/setup.py
--rw-r--r--   0        0        0     1639 2022-11-07 20:47:59.507318 encord-active-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      203 2022-11-17 13:23:16.467728 encord-active-0.1.9/.env
+-rw-r--r--   0        0        0    34523 2022-11-17 13:23:16.467728 encord-active-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3134 2022-11-17 13:23:53.599684 encord-active-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.567728 encord-active-0.1.9/src/encord_active/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.567728 encord-active-0.1.9/src/encord_active/app/__init__.py
+-rw-r--r--   0        0        0     3550 2022-11-17 13:23:16.567728 encord-active-0.1.9/src/encord_active/app/app_config.py
+-rw-r--r--   0        0        0      463 2022-11-17 13:23:16.567728 encord-active-0.1.9/src/encord_active/app/app_print_utils.py
+-rw-r--r--   0        0        0    57557 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/assets/encord_2_02.png
+-rw-r--r--   0        0        0     1064 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/assets/favicon-32x32.png
+-rw-r--r--   0        0        0    11228 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/action_utils.py
+-rw-r--r--   0        0        0     1440 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/cli_helpers.py
+-rw-r--r--   0        0        0      912 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/colors.py
+-rw-r--r--   0        0        0      134 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/components/__init__.py
+-rw-r--r--   0        0        0     1953 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/components/bulk_tagging_form.py
+-rw-r--r--   0        0        0     2467 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/components/data_tags.py
+-rw-r--r--   0        0        0     3457 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/components/individual_tagging.py
+-rw-r--r--   0        0        0     1232 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/components/multi_select.py
+-rw-r--r--   0        0        0     1396 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/components/sticky/sticky.html
+-rw-r--r--   0        0        0      383 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/components/sticky/sticky.py
+-rw-r--r--   0        0        0     2855 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/css.py
+-rw-r--r--   0        0        0     8673 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/embedding_utils.py
+-rw-r--r--   0        0        0     1312 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/metric.py
+-rw-r--r--   0        0        0     3633 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/page.py
+-rw-r--r--   0        0        0     3863 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/state.py
+-rw-r--r--   0        0        0     7901 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/common/utils.py
+-rw-r--r--   0        0        0      205 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/conf/__init__.py
+-rw-r--r--   0        0        0      207 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/conf/logging.py
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/data_quality/__init__.py
+-rw-r--r--   0        0        0     2562 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/data_quality/common.py
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/data_quality/sub_pages/__init__.py
+-rw-r--r--   0        0        0    18881 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/data_quality/sub_pages/explorer.py
+-rw-r--r--   0        0        0     6664 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/data_quality/sub_pages/summary.py
+-rw-r--r--   0        0        0      448 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/db/connection.py
+-rw-r--r--   0        0        0     3651 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/db/merged_metrics.py
+-rw-r--r--   0        0        0     2807 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/db/predictions.py
+-rw-r--r--   0        0        0     1485 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/db/tags.py
+-rw-r--r--   0        0        0      257 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/frontend_components.py
+-rw-r--r--   0        0        0      162 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/known-issues.md
+-rw-r--r--   0        0        0     9011 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/main.py
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/__init__.py
+-rw-r--r--   0        0        0       90 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/components/__init__.py
+-rw-r--r--   0        0        0     3212 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/components/false_negative_view.py
+-rw-r--r--   0        0        0     2798 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/components/index_view.py
+-rw-r--r--   0        0        0     2798 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/components/metric_view.py
+-rw-r--r--   0        0        0     1329 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/components/utils.py
+-rw-r--r--   0        0        0     7895 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/data.py
+-rw-r--r--   0        0        0     8687 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/map_mar.py
+-rw-r--r--   0        0        0     1781 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/settings.py
+-rw-r--r--   0        0        0     4321 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/__init__.py
+-rw-r--r--   0        0        0     2166 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/false_negatives.py
+-rw-r--r--   0        0        0     1899 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/false_positives.py
+-rw-r--r--   0        0        0     9541 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/metrics.py
+-rw-r--r--   0        0        0     7658 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/performance_by_metric.py
+-rw-r--r--   0        0        0     1798 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/true_positives.py
+-rw-r--r--   0        0        0     3125 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/streamlit_entrypoint.py
+-rw-r--r--   0        0        0     7134 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/views/export_balance.py
+-rw-r--r--   0        0        0     6327 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/views/export_filter.py
+-rw-r--r--   0        0        0     3477 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/views/getting_started.py
+-rw-r--r--   0        0        0      962 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/views/metrics.py
+-rw-r--r--   0        0        0     3207 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/app/views/model_assertions.py
+-rw-r--r--   0        0        0       92 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/__init__.py
+-rw-r--r--   0        0        0       22 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/common/__init__.py
+-rw-r--r--   0        0        0     8383 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/common/iterator.py
+-rw-r--r--   0        0        0     5705 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/common/metric.py
+-rw-r--r--   0        0        0     5708 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/common/prepare.py
+-rw-r--r--   0        0        0     2511 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/common/tester.py
+-rw-r--r--   0        0        0    10140 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/common/utils.py
+-rw-r--r--   0        0        0     8441 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/common/writer.py
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/embeddings/__init__.py
+-rw-r--r--   0        0        0     8805 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/embeddings/cnn_embed.py
+-rw-r--r--   0        0        0     2085 2022-11-17 13:23:16.571728 encord-active-0.1.9/src/encord_active/lib/embeddings/hu_embed.py
+-rw-r--r--   0        0        0     2640 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/example.py
+-rw-r--r--   0        0        0     2099 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/fetch_prebuilt_metrics.py
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/geometric/__init__.py
+-rw-r--r--   0        0        0     3081 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/geometric/annotation_duplicates.py
+-rw-r--r--   0        0        0     4326 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/geometric/hu_static.py
+-rw-r--r--   0        0        0     3123 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/geometric/hu_temporal.py
+-rw-r--r--   0        0        0     2182 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/geometric/image_border_closeness.py
+-rw-r--r--   0        0        0     6155 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/geometric/object_size.py
+-rw-r--r--   0        0        0     5917 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/geometric/occlusion_detection_video.py
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/__init__.py
+-rw-r--r--   0        0        0     1580 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/_annotation_time.py
+-rw-r--r--   0        0        0     6710 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/high_iou_changing_classes.py
+-rw-r--r--   0        0        0     9192 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/img_features.py
+-rw-r--r--   0        0        0    10311 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/missing_objects_and_wrong_tracks.py
+-rw-r--r--   0        0        0      873 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/object_counting.py
+-rw-r--r--   0        0        0     3273 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/import_encord_project.py
+-rw-r--r--   0        0        0     3863 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/run_all.py
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/semantic/__init__.py
+-rw-r--r--   0        0        0    10085 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/semantic/_class_uncertainty.py
+-rw-r--r--   0        0        0     8882 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/semantic/_heatmap_uncertainty.py
+-rw-r--r--   0        0        0    13921 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/semantic/img_classification_quality.py
+-rw-r--r--   0        0        0     7269 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/metrics/semantic/img_object_quality.py
+-rw-r--r--   0        0        0        0 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/model_predictions/__init__.py
+-rw-r--r--   0        0        0     8902 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/model_predictions/importers.py
+-rw-r--r--   0        0        0     7858 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/model_predictions/iterator.py
+-rw-r--r--   0        0        0    20022 2022-11-17 13:23:16.575728 encord-active-0.1.9/src/encord_active/lib/model_predictions/prediction_writer.py
+-rw-r--r--   0        0        0     2397 2022-11-17 13:26:40.254175 encord-active-0.1.9/setup.py
+-rw-r--r--   0        0        0     1720 2022-11-17 13:26:40.254577 encord-active-0.1.9/PKG-INFO
```

### Comparing `encord-active-0.1.8/LICENSE` & `encord-active-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/pyproject.toml` & `encord-active-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord-active"
-version = "v0.1.8"
+version = "v0.1.9"
 description = ""
 authors = [
     "Frederik Hvilshøj <frederik@cord.tech>",
     "Gorkem Polat <gorkem@encord.com>",
     "Eloy Pérez <eloy@encord.com>",
     "Javier Leguina <javier@encord.com>"
 ]
@@ -46,29 +46,32 @@
 loguru = "^0.6.0"
 python-dotenv = "^0.21.0"
 streamlit-nested-layout = "^0.1.1"
 typer = "^0.6.1"
 inquirer = "^2.10.0"
 rich = "^12.6.0"
 PyYAML = "^6.0"
+toml = "^0.10.2"
+pydantic = "^1.10.2"
+
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 black = "^22.6.0"
 isort = "^5.10.1"
 pre-commit = "^2.16.0"
 mypy = "^0.981"
 pylint = "^2.14.5"
 types-requests = "^2.28.8"
 types-PyYAML = "^6.0.12"
 ipython = "^8.5.0"
 tabulate = "^0.9.0"
 types-tabulate = "^0.8.5"
 ipdb = "^0.13.9"
-
+types-toml = "^0.10.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `encord-active-0.1.8/src/encord_active/app/assets/encord_2_02.png` & `encord-active-0.1.9/src/encord_active/app/assets/encord_2_02.png`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/assets/favicon-32x32.png` & `encord-active-0.1.9/src/encord_active/app/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/common/colors.py` & `encord-active-0.1.9/src/encord_active/app/common/colors.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/common/components/bulk_tagging_form.py` & `encord-active-0.1.9/src/encord_active/app/common/components/bulk_tagging_form.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/common/components/data_tags.py` & `encord-active-0.1.9/src/encord_active/app/common/components/data_tags.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/common/components/multi_select.py` & `encord-active-0.1.9/src/encord_active/app/common/components/multi_select.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/common/components/sticky/sticky.html` & `encord-active-0.1.9/src/encord_active/app/common/components/sticky/sticky.html`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/common/css.py` & `encord-active-0.1.9/src/encord_active/app/common/css.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,16 +78,42 @@
     }}
 
     .encord-active-info-box {{
         width: 100%; 
         padding: 1em; 
         background-color: rgba(28, 131, 225, 0.1); 
         color: rgb(0, 66, 128); 
-        padding: 1em; 
         border-radius: 0.25rem;
         margin-top: 1em;
         margin-bottom: 1em;
     }}
+
+    span.data-tag {{
+        color: #fff;
+        background-color: {Color.PURPLE.value};
+        border-radius: 10rem;
+        display: inline-block;
+        padding: 0.25em 0.4em;
+        font-size: 75%;
+        font-weight: 700;
+        line-height: 1;
+        text-align: center;
+        white-space: nowrap;
+        vertical-align: baseline;
+        border-radius: 0.25rem;
+    }}
+
+    span.data-tag-count {{
+        margin-left: 0.2rem;
+        background: rgba(255, 255, 255, 0.2);
+    }}
+
+    /* Place expand button within image */
+    .element-container > div > button[title='View fullscreen'] {{
+        right: 0.2rem;
+        top: 0.2rem;
+    }}
+
 </style>
         """,
         unsafe_allow_html=True,
     )
```

### Comparing `encord-active-0.1.8/src/encord_active/app/common/indexer.py` & `encord-active-0.1.9/src/encord_active/app/common/metric.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/common/page.py` & `encord-active-0.1.9/src/encord_active/app/common/page.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/common/state.py` & `encord-active-0.1.9/src/encord_active/app/common/state.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,29 @@
 IGNORE_FRAMES_WO_PREDICTIONS = "ignore_frames_wo_predictions"
 METRIC_NAME = "metric_name"
 IOU_THRESHOLD = "iou_threshold_scaled"  # After normalization
 IOU_THRESHOLD_ = "iou_threshold_"  # Before normalization
 MERGED_DATAFRAME = "merged_dataframe"
 ALL_TAGS = "all_tags"
 
+# SIMILARITY KEYS
+OBJECT_KEYS_HAVING_SIMILARITIES = "object_keys_having_similarities"
+IMAGE_KEYS_HAVING_SIMILARITIES = "image_keys_having_similarity"
+OBJECT_SIMILARITIES = "object_similarities"
+IMAGE_SIMILARITIES = "image_similarities"
+IMAGE_SIMILARITIES_NO_LABEL = "image_similarities_no_label"
+FAISS_INDEX_OBJECT = "faiss_index_object"
+FAISS_INDEX_IMAGE = "faiss_index_image"
+FAISS_INDEX_IMAGE_NO_LABEL = "faiss_index_image_no_label"
+CURRENT_INDEX_HAS_ANNOTATION = "current_index_has_annotation"
+QUESTION_HASH_TO_COLLECTION_INDEXES = "question_hash_to_collection_indexes"
+COLLECTIONS_IMAGES = "collections_images"
+COLLECTIONS_OBJECTS = "collections_objects"
+
+
 # DATA QUALITY PAGE
 DATA_PAGE_TYPE = "data_page_type"  # Summary | Explorer
 DATA_PAGE_METRIC_TYPE = "data_page_metric_type"  # Label quality | Data Quality
 DATA_PAGE_METRIC = "data_page_metric"  # metric
 DATA_PAGE_METRIC_NAME = "data_page_metric_name"  # metric name
 DATA_PAGE_CLASS = "data_page_class_selection"  # class
 DATA_PAGE_ANNOTATOR = "data_page_annotator_selection"  # annotator
@@ -36,32 +51,30 @@
 PREDICTIONS_SHOW_DOWNLOAD_BUTTON = "predictions_show_download_button"
 
 # TILING & PAGINATION
 MAIN_VIEW_COLUMN_NUM = "main_view_column_num"
 MAIN_VIEW_ROW_NUM = "main_view_row_num"
 K_NEAREST_NUM = "k_nearest_num"
 
-IDENTIFIER_TO_NEIGHBORS_CLASSES = "identifier_to_neighbors_classes"
-IDENTIFIER_TO_NEIGHBORS_OBJECTS = "identifier_to_neighbors_objects"
-QUESTION_HASH_TO_COLLECTION_INDEXES = "question_hash_to_collection_indexes"
-COLLECTIONS = "collections"
-
 DATA_PAGE_NUMBER = "data_page_number"
 METRIC_VIEW_PAGE_NUMBER = "metric_view_page_number"
 FALSE_NEGATIVE_VIEW_PAGE_NUMBER = "false_negative_view_page_number"
 
 NORMALIZATION_STATUS = "normalization_status"
 PREVIOUS_METRIC_TITLE = "previous_metric_title"
 METRIC_METADATA_SCORE_NORMALIZATION = "score_normalization"
 METRIC_METADATA_TITLE = "title"
 METRIC_METADATA_NUM_ROWS = "num_rows"
 METRIC_METADATA_DATA_TYPE = "data_type"
 TOTAL_UNIQUE_CLASSES = "total_unique_classes"
 TOTAL_UNIQUE_IMAGES = "total_unique_images"
 
+# Export page
+NUMBER_OF_PARTITIONS = "number_of_partitions"
+
 
 def set_project_dir(project_dir: str) -> bool:
     _project_dir = Path(project_dir).expanduser().absolute()
 
     if not _project_dir.is_dir():
         return False
     else:
```

### Comparing `encord-active-0.1.8/src/encord_active/app/common/utils.py` & `encord-active-0.1.9/src/encord_active/app/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,20 @@
         h = image.shape[0]
         w = image.shape[1]
     else:
         w = int(du["width"])
         h = int(du["height"])
 
     geometries = []
-    objects = du["labels"]["objects"] if "video" not in du["data_type"] else du["labels"][str(int(frame))]["objects"]
+
+    objects = (
+        du["labels"].get("objects", [])
+        if "video" not in du["data_type"]
+        else du["labels"][str(int(frame))].get("objects", [])
+    )
 
     if remainder and not skip_object_hash:
         # Return specific geometries
         geometry_object_hashes = set(remainder)
         for obj in objects:
             if obj["objectHash"] in geometry_object_hashes:
                 geometries.append(__get_geometry(obj, w, h))
```

### Comparing `encord-active-0.1.8/src/encord_active/app/data_quality/common.py` & `encord-active-0.1.9/src/encord_active/app/data_quality/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,16 +52,15 @@
 
     out: List[MetricData] = []
 
     if not meta_data:
         return out
 
     for p, n, m, l in zip(paths, names, meta_data, levels):
-        annotation_type = m.get("annotation_type")
-        if m is None or not l or not criterion(annotation_type):
+        if m is None or not l or not criterion(m.get("annotation_type")):
             continue
 
         out.append(MetricData(name=n, path=p, meta=m, level=l))
 
     out = natsorted(out, key=lambda i: (i.level, i.name))  # type: ignore
     return out
```

### Comparing `encord-active-0.1.8/src/encord_active/app/data_quality/sub_pages/explorer.py` & `encord-active-0.1.9/src/encord_active/app/data_quality/sub_pages/explorer.py`

 * *Files 8% similar despite different names*

```diff
@@ -223,96 +223,124 @@
         )
     ):  # TODO find a better way to filter these later because titles can change
         embedding_type = str(EmbeddingType.CLASSIFICATION.value)
     else:
         embedding_type = str(EmbeddingType.OBJECT.value)
 
     populate_embedding_information(embedding_type)
-    if len(st.session_state[state.COLLECTIONS]) == 0:
-        st.write("Embedding file is not available for this project")
-    else:
-        n_cols = int(st.session_state[state.MAIN_VIEW_COLUMN_NUM])
-        n_rows = int(st.session_state[state.MAIN_VIEW_ROW_NUM])
 
-        chart = get_histogram(current_df)
-        st.altair_chart(chart, use_container_width=True)
-        subset = get_df_subset(current_df, "score")
+    if (embedding_type == str(EmbeddingType.CLASSIFICATION.value)) and len(
+        st.session_state[state.COLLECTIONS_IMAGES]
+    ) == 0:
+        st.write("Image-level embedding file is not available for this project.")
+        return
+    if (embedding_type == str(EmbeddingType.OBJECT.value)) and len(st.session_state[state.COLLECTIONS_OBJECTS]) == 0:
+        st.write("Object-level embedding file is not available for this project.")
+        return
+
+    n_cols = int(st.session_state[state.MAIN_VIEW_COLUMN_NUM])
+    n_rows = int(st.session_state[state.MAIN_VIEW_ROW_NUM])
 
-        st.write(f"Interval contains {subset.shape[0]} of {current_df.shape[0]} annotations")
+    chart = get_histogram(current_df)
+    st.altair_chart(chart, use_container_width=True)
+    subset = get_df_subset(current_df, "score")
 
-        paginated_subset = build_pagination(subset, n_cols, n_rows, "score")
+    st.write(f"Interval contains {subset.shape[0]} of {current_df.shape[0]} annotations")
 
-        form = bulk_tagging_form()
+    paginated_subset = build_pagination(subset, n_cols, n_rows, "score")
 
-        if form and form.submitted:
-            df = paginated_subset if form.level == BulkLevel.PAGE else subset
-            action_bulk_tags(df, form.tags, form.action)
+    form = bulk_tagging_form()
 
-        if len(paginated_subset) == 0:
-            st.error("No data in selected interval")
-        else:
-            cols: List = []
-            similarity_expanders = []
-            for i, (row_no, row) in enumerate(paginated_subset.iterrows()):
-                if not cols:
-                    cols = list(st.columns(n_cols))
-                    similarity_expanders.append(st.expander("Similarities", expanded=True))
+    if form and form.submitted:
+        df = paginated_subset if form.level == BulkLevel.PAGE else subset
+        action_bulk_tags(df, form.tags, form.action)
+
+    if len(paginated_subset) == 0:
+        st.error("No data in selected interval")
+    else:
+        cols: List = []
+        similarity_expanders = []
+        for i, (row_no, row) in enumerate(paginated_subset.iterrows()):
+            if not cols:
+                cols = list(st.columns(n_cols))
+                similarity_expanders.append(st.expander("Similarities", expanded=True))
 
-                with cols.pop(0):
-                    build_card(embedding_type, i, row, similarity_expanders)
+            with cols.pop(0):
+                build_card(embedding_type, i, row, similarity_expanders)
 
 
 def populate_embedding_information(embedding_type: str):
     if embedding_type == EmbeddingType.CLASSIFICATION.value:
         if st.session_state[state.DATA_PAGE_METRIC].meta.get("title") == "Image-level Annotation Quality":
             collections, question_hash_to_collection_indexes = embedding_utils.get_collections_and_metadata(
                 "cnn_classifications.pkl"
             )
-            identifier_to_neighbors = embedding_utils.get_identifiers_to_nearest_items(
-                collections, question_hash_to_collection_indexes, int(st.session_state[state.K_NEAREST_NUM])
-            )
-            st.session_state[state.COLLECTIONS] = collections
+            st.session_state[state.COLLECTIONS_IMAGES] = collections
             st.session_state[state.QUESTION_HASH_TO_COLLECTION_INDEXES] = question_hash_to_collection_indexes
-            st.session_state[state.IDENTIFIER_TO_NEIGHBORS_CLASSES] = identifier_to_neighbors
+            st.session_state[state.IMAGE_KEYS_HAVING_SIMILARITIES] = embedding_utils.get_image_keys_having_similarities(
+                collections
+            )
+            st.session_state[state.FAISS_INDEX_IMAGE] = embedding_utils.get_faiss_index_image(collections)
+            st.session_state[state.CURRENT_INDEX_HAS_ANNOTATION] = True
+
+            if state.IMAGE_SIMILARITIES not in st.session_state:
+                st.session_state[state.IMAGE_SIMILARITIES] = {}
+                for question_hash in st.session_state[state.QUESTION_HASH_TO_COLLECTION_INDEXES].keys():
+                    st.session_state[state.IMAGE_SIMILARITIES][question_hash] = {}
         else:
             collections = embedding_utils.get_collections("cnn_classifications.pkl")
-            identifier_to_neighbors = embedding_utils.get_collections_to_neighbors(
-                collections, int(st.session_state[state.K_NEAREST_NUM]), has_annotation=False
+            st.session_state[state.COLLECTIONS_IMAGES] = collections
+            st.session_state[state.IMAGE_KEYS_HAVING_SIMILARITIES] = embedding_utils.get_image_keys_having_similarities(
+                collections
+            )
+            st.session_state[state.FAISS_INDEX_IMAGE_NO_LABEL] = embedding_utils.get_faiss_index_object(
+                collections, state.FAISS_INDEX_IMAGE_NO_LABEL
             )
-            st.session_state[state.COLLECTIONS] = collections
-            st.session_state[state.IDENTIFIER_TO_NEIGHBORS_CLASSES] = identifier_to_neighbors
+            st.session_state[state.CURRENT_INDEX_HAS_ANNOTATION] = False
+
+            if state.IMAGE_SIMILARITIES_NO_LABEL not in st.session_state:
+                st.session_state[state.IMAGE_SIMILARITIES_NO_LABEL] = {}
+
     elif embedding_type == EmbeddingType.OBJECT.value:
         collections = embedding_utils.get_collections("cnn_objects.pkl")
-        identifier_to_neighbors = embedding_utils.get_collections_to_neighbors(
-            collections, int(st.session_state[state.K_NEAREST_NUM])
+        st.session_state[state.COLLECTIONS_OBJECTS] = collections
+        st.session_state[state.OBJECT_KEYS_HAVING_SIMILARITIES] = embedding_utils.get_object_keys_having_similarities(
+            collections
+        )
+        st.session_state[state.FAISS_INDEX_OBJECT] = embedding_utils.get_faiss_index_object(
+            collections, state.FAISS_INDEX_OBJECT
         )
-        st.session_state[state.COLLECTIONS] = collections
-        st.session_state[state.IDENTIFIER_TO_NEIGHBORS_OBJECTS] = identifier_to_neighbors
+        st.session_state[state.CURRENT_INDEX_HAS_ANNOTATION] = True
+
+        if state.OBJECT_SIMILARITIES not in st.session_state:
+            st.session_state[state.OBJECT_SIMILARITIES] = {}
 
 
 def build_card(card_type: str, card_no: int, row: Series, _similarity_expanders: list[DeltaGenerator]):
     """
     Builds each sub card (the content displayed for each row in a csv file).
     """
 
     if card_type == EmbeddingType.CLASSIFICATION.value:
+
         button_name = "show similar images"
         if st.session_state[state.DATA_PAGE_METRIC].meta.get("title") == "Image-level Annotation Quality":
             image = load_or_fill_image(row)
             similarity_callback = show_similar_classification_images
         else:
             if st.session_state[state.DATA_PAGE_METRIC].meta.get("annotation_type") is None:
                 image = load_or_fill_image(row)
             else:
                 image = show_image_and_draw_polygons(row)
             similarity_callback = show_similar_images
     elif card_type == EmbeddingType.OBJECT.value:
         image = show_image_and_draw_polygons(row)
         button_name = "show similar objects"
         similarity_callback = show_similar_object_images
+
     else:
         st.write(f"{card_type} card type is not defined in EmbeddingTypes")
         return
 
     st.image(image)
     multiselect_tag(row, "explorer")
 
@@ -362,15 +390,19 @@
         .properties(height=200)
     )
     return bar_chart
 
 
 def show_similar_classification_images(row: Series, expander: DeltaGenerator):
     feature_hash = row["identifier"].split("_")[-1]
-    nearest_images = st.session_state[state.IDENTIFIER_TO_NEIGHBORS_CLASSES][feature_hash][row["identifier"]]
+
+    if row["identifier"] not in st.session_state[state.IMAGE_SIMILARITIES][feature_hash].keys():
+        embedding_utils.add_labeled_image_neighbors_to_cache(row["identifier"], feature_hash)
+
+    nearest_images = st.session_state[state.IMAGE_SIMILARITIES][feature_hash][row["identifier"]]
 
     division = 4
     column_id = 0
 
     for nearest_image in nearest_images:
         if column_id == 0:
             st_columns = expander.columns(division)
@@ -380,18 +412,20 @@
         st_columns[column_id].image(image)
         st_columns[column_id].write(f"Annotated as `{nearest_image['name']}`")
         column_id += 1
         column_id = column_id % division
 
 
 def show_similar_images(row: Series, expander: DeltaGenerator):
-    label_hash, data_unit_hash, frame_id, *rest = row["identifier"].split("_")
-    nearest_images = st.session_state[state.IDENTIFIER_TO_NEIGHBORS_CLASSES][
-        "_".join([label_hash, data_unit_hash, frame_id])
-    ]
+    image_identifier = "_".join(row["identifier"].split("_")[:3])
+
+    if image_identifier not in st.session_state[state.IMAGE_SIMILARITIES_NO_LABEL].keys():
+        embedding_utils.add_image_neighbors_to_cache(image_identifier)
+
+    nearest_images = st.session_state[state.IMAGE_SIMILARITIES_NO_LABEL][image_identifier]
 
     division = 4
     column_id = 0
 
     for nearest_image in nearest_images:
         if column_id == 0:
             st_columns = expander.columns(division)
@@ -402,19 +436,23 @@
         st_columns[column_id].write(f"Annotated as `{nearest_image['name']}`")
         column_id += 1
         column_id = column_id % division
 
 
 def show_similar_object_images(row: Series, expander: DeltaGenerator):
     object_identifier = "_".join(row["identifier"].split("_")[:4])
-    if object_identifier not in st.session_state[state.IDENTIFIER_TO_NEIGHBORS_OBJECTS].keys():
+
+    if object_identifier not in st.session_state[state.OBJECT_KEYS_HAVING_SIMILARITIES]:
         expander.write("Similarity search is not available for this object.")
         return
 
-    nearest_images = st.session_state[state.IDENTIFIER_TO_NEIGHBORS_OBJECTS][object_identifier]
+    if object_identifier not in st.session_state[state.OBJECT_SIMILARITIES].keys():
+        embedding_utils.add_object_neighbors_to_cache(object_identifier)
+
+    nearest_images = st.session_state[state.OBJECT_SIMILARITIES][object_identifier]
 
     division = 4
     column_id = 0
 
     for nearest_image in nearest_images:
         if column_id == 0:
             st_columns = expander.columns(division)
```

### Comparing `encord-active-0.1.8/src/encord_active/app/data_quality/sub_pages/summary.py` & `encord-active-0.1.9/src/encord_active/app/data_quality/sub_pages/summary.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/db/merged_metrics.py` & `encord-active-0.1.9/src/encord_active/app/db/merged_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,32 +18,32 @@
         meta_pth = index.with_suffix(".meta.json")
         if not meta_pth.is_file():
             continue
 
         with meta_pth.open("r", encoding="utf-8") as f:
             meta = json.load(f)
 
-        indexer_scores = pd.read_csv(index)
-        if indexer_scores.shape[0] == 0:
+        metric_scores = pd.read_csv(index)
+        if metric_scores.shape[0] == 0:
             continue
 
-        if len(indexer_scores["identifier"][0].split("_")) == 3:
+        if len(metric_scores["identifier"][0].split("_")) == 3:
             # Image-level index
             if main_df_images.shape[0] == 0:
-                columns_to_merge = indexer_scores[["identifier", "url", "score"]]
+                columns_to_merge = metric_scores[["identifier", "url", "score"]]
             else:
-                columns_to_merge = indexer_scores[["identifier", "score"]]
+                columns_to_merge = metric_scores[["identifier", "score"]]
             main_df_images = pd.merge(main_df_images, columns_to_merge, how="outer", on="identifier")
             main_df_images.rename(columns={"score": f"{meta['title']}"}, inplace=True)
         else:
             # Object-level-index
             if main_df_objects.shape[0] == 0:
-                columns_to_merge = indexer_scores[["identifier", "url", "score"]]
+                columns_to_merge = metric_scores[["identifier", "url", "score"]]
             else:
-                columns_to_merge = indexer_scores[["identifier", "score"]]
+                columns_to_merge = metric_scores[["identifier", "score"]]
             main_df_objects = pd.merge(main_df_objects, columns_to_merge, how="outer", on="identifier")
             main_df_objects.rename(columns={"score": f"{meta['title']}"}, inplace=True)
 
     main_df = pd.concat([main_df_images, main_df_objects])
     main_df["tags"] = None
     main_df.set_index("identifier", inplace=True)
     return main_df
```

### Comparing `encord-active-0.1.8/src/encord_active/app/db/tags.py` & `encord-active-0.1.9/src/encord_active/app/db/tags.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/main.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/import_encord_project.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,105 @@
+import re
 import sys
 from pathlib import Path
+from typing import Optional
 
-import inquirer as i
+import encord.exceptions
 import typer
-from streamlit.web import cli as stcli
-
-import encord_active.app.conf  # pylint: disable=unused-import
-from encord_active.lib.metrics.fetch_prebuilt_metrics import (
-    PREBUILT_PROJECT_TO_STORAGE,
-    PREBUILT_PROJECTS,
-    fetch_metric,
-)
-
-APP_NAME = "encord-active"
-
-cli = typer.Typer(rich_markup_mode="markdown")
-
-__PREBUILT_PROJECT_NAMES = list(PREBUILT_PROJECTS.keys())
-
-
-@cli.command(rich_help_panel="Utils")
-def download(
-    project_dir: Path = typer.Option(
-        None,
-        help="Location where to download the project. Prebuilt metrics will be downloaded as well.",
-        prompt="Where should the prebuilt project be stored (absolute/relative path)?",
-        file_okay=False,
-    ),
-    project_name: str = typer.Option(
-        None, help=f"Name of the chosen project. Available prebuilt projects: {__PREBUILT_PROJECT_NAMES}."
-    ),
-):
-    """
-    **Downloads** a prebuilt project and metrics 📁
-
-    * If --project_name is not given as an argument, available prebuilt projects will be listed
-     and the user can select one from the menu.
-    """
-    project_parent_dir = Path(project_dir).resolve()
-    if not project_parent_dir.exists():
-        create = typer.confirm("Such directory does not exist, do you want to create it?")
-        if not create:
-            print("Canceling project download.")
-            raise typer.Abort()
-        project_parent_dir.mkdir(parents=True)
-
-    if project_name is not None and project_name not in PREBUILT_PROJECTS:
-        print("No such project in prebuilt projects.")
-        raise typer.Abort()
-
-    if not project_name:
-        project_names_with_storage = [p + f" ({PREBUILT_PROJECT_TO_STORAGE[p]})" for p in __PREBUILT_PROJECT_NAMES]
-        questions = [i.List("project_name", message="Choose a project", choices=project_names_with_storage)]
-        answers = i.prompt(questions)
-        if not answers or "project_name" not in answers:
-            print("No project was selected.")
-            raise typer.Abort()
-        project_name = answers["project_name"].rsplit(" (", maxsplit=1)[0]
-
-    # create project folder
-    project_dir = project_parent_dir / project_name
-    project_dir.mkdir(exist_ok=True)
-
-    fetch_metric(project_name, project_dir)
-
-
-@cli.command(name="import", rich_help_panel="Utils")
-def import_project():
-    """
-    **Imports** a project from Encord 📦
-    """
-
-    from encord_active.lib.metrics.import_encord_project import main as import_script
-
-    # TODO: move the setup into a config command.
-    # currently the import setup will run every time.
-    import_script()
-
-
-@cli.command()
-def visualise(
-    project_path: Path = typer.Argument(
-        ...,
-        help="Path of the project you would like to visualise",
-        file_okay=False,
-    ),
-):
-    """
-    Launches the application with the provided project ✨
-    """
-    streamlit_page = (Path(__file__).parent / "streamlit_entrypoint.py").expanduser().absolute()
-
-    data_dir = Path(project_path).expanduser().absolute().as_posix()
-    sys.argv = ["streamlit", "run", streamlit_page.as_posix(), data_dir]
-    sys.exit(stcli.main())  # pylint: disable=no-value-for-parameter
-
-
-if __name__ == "__main__":
-    cli(prog_name=APP_NAME)
+import yaml
+from encord import EncordUserClient, Project
+from rich import print
+from rich.panel import Panel
+
+from encord_active.app.app_config import AppConfig
+from encord_active.app.app_print_utils import get_projects_json
+
+project_root = Path(__file__).parents[1]
+sys.path.append(project_root.as_posix())
+
+from encord_active.lib.metrics.run_all import run_metrics
+
+PROJECT_HASH_REGEX = r"([0-9a-f]{8})-([0-9a-f]{4})-([0-9a-f]{4})-([0-9a-f]{4})-([0-9a-f]{12})"
+
+
+def main(config: AppConfig):
+    ssh_key_path = config.get_or_query_ssh_key()
+    projects_root = config.get_or_query_project_path()
+
+    client = EncordUserClient.create_with_ssh_private_key(ssh_key_path.read_text(encoding="utf-8"))
+
+    # == Get project hash === #
+    print(
+        Panel(
+            """
+Encord Active will need to know the project hash associated with the project you 
+wish to import. If you don't know this hash already, [bold green]you can enter "?"[/bold green] in the following 
+prompt to get all your `project_hash`es and associated project titles listed.
+    """,
+            title="The Encord Project",
+            expand=False,
+        )
+    )
+
+    encord_project_hash = ""
+    project: Optional[Project] = None
+    while not encord_project_hash:
+        _encord_project_hash = typer.prompt("Specify project hash").strip().lower()
+
+        if _encord_project_hash == "?":
+            print(get_projects_json(config))
+
+        if not re.match(PROJECT_HASH_REGEX, _encord_project_hash):
+            print("🙈 [orange]Project hash does not have the correct format.")
+            print("The format is a (hex) uuid: aaaaaaaa-bbbb-bbbb-bbbb-000000000000")
+            print("💡 Hint: You can type [green]?[/green] to list all your projects")
+            continue
+
+        project = client.get_project(_encord_project_hash)
+        try:
+            _ = project.title
+        except encord.exceptions.AuthorisationError:
+            print("⚡️ [red]You don't have access to the project, sorry[/red] 😫")
+            continue
+
+        encord_project_hash = _encord_project_hash
+
+    if project is None:
+        exit()
+
+    project_path = projects_root / project.title.replace(" ", "-")
+    project_path.mkdir(exist_ok=True, parents=True)
+
+    meta_data = {
+        "project_name": project.title,
+        "project_description": project.description,
+        "project_hash": project.project_hash,
+        "ssh_key_path": ssh_key_path.as_posix(),
+    }
+    meta_file_path = project_path / "project_meta.yaml"
+    yaml_str = yaml.dump(meta_data)
+    with meta_file_path.open("w", encoding="utf-8") as f:
+        f.write(yaml_str)
+
+    print("Stored the following data:")
+    print(f"[magenta]{yaml_str}")
+    print(f"In file: [blue]`{meta_file_path}`")
+    print()
+    print("Now downloading data and running metrics")
+
+    run_metrics(data_dir=project_path)
+
+    panel = Panel(
+        f"""
+The data is downloaded and the metrics are complete.  
+
+Now run
+
+[cyan blink]encord-active visualise "{project_path}"[/cyan blink]
+
+to open the app and see the results. 
+""",
+        title="🌟 Success 🌟",
+        style="green",
+        expand=False,
+    )
+    print(panel)
```

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/components/false_negative_view.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/components/false_negative_view.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/components/index_view.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/components/index_view.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/components/metric_view.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/components/metric_view.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/components/utils.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/components/utils.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/data.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/data.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/map_mar.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/map_mar.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,18 +103,18 @@
     label_include_ids = set(_labels.index[_labels["img_id"].isin(pred_img_ids)])
 
     cidx = 0
     for class_idx in _class_map:
         if ignore_unmatched_frames:
             # nb_labels = sum([len([c for c in l if c in pred_img_ids]) for l in _gt_matched[class_idx].values()])
             nb_labels = sum(
-                [len([t for t in l if t["lidx"] in label_include_ids]) for l in _gt_matched[class_idx].values()]
+                [len([t for t in l if t["lidx"] in label_include_ids]) for l in _gt_matched.get(class_idx, {}).values()]
             )
         else:
-            nb_labels = sum([len(l) for l in _gt_matched[class_idx].values()])
+            nb_labels = sum([len(l) for l in _gt_matched.get(class_idx, {}).values()])
 
         if nb_labels == 0:
             continue
 
         class_idx_map[cidx] = class_idx  # Keep track of the order of the output lists
         pred_select = pred_class_list == int(class_idx)
         if pred_select.sum() == 0:
```

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/settings.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/settings.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/__init__.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/__init__.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/false_negatives.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/false_negatives.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/false_positives.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/false_positives.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/metrics.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/metrics.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/performance_by_metric.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/performance_by_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,17 +151,28 @@
 
             metric_name = st.session_state[state.PREDICTIONS_METRIC]
             num_unique_values = model_predictions[metric_name].unique().shape[0]
             n_bins = min(st.session_state.get(state.PREDICTIONS_NBINS, 100), num_unique_values)
             sorted_predictions = (
                 model_predictions[[metric_name, "tps", "class_name"]].copy().dropna(subset=[metric_name])
             )
+
+            if sorted_predictions.empty:
+                st.info(f"No scores for metric: {metric_name}")
+                st.stop()
+
             sorted_predictions["bin"] = pd.qcut(sorted_predictions[metric_name], q=n_bins, duplicates="drop").map(
                 lambda x: x.mid
             )
+
+            # Why only NaN's in 'bin'??
+            if sorted_predictions["bin"].dropna().empty:
+                st.info(f"No scores for metric: {metric_name}")
+                st.stop()
+
             sorted_predictions["average"] = "average"
 
             show_decomposition = st.session_state[state.PREDICTIONS_DECOMPOSE_CLASSES]
             bar_chart = self.build_bar_chart(sorted_predictions, metric_name, show_decomposition)
             line_chart = self.build_line_chart(bar_chart, metric_name, show_decomposition)
             mean_rule = self.build_average_rule(model_predictions["tps"].mean())
```

### Comparing `encord-active-0.1.8/src/encord_active/app/model_assertions/sub_pages/true_positives.py` & `encord-active-0.1.9/src/encord_active/app/model_assertions/sub_pages/true_positives.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/streamlit_entrypoint.py` & `encord-active-0.1.9/src/encord_active/app/streamlit_entrypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 from encord_active.app.model_assertions.sub_pages.metrics import MetricsPage
 from encord_active.app.model_assertions.sub_pages.performance_by_metric import (
     PerformanceMetric,
 )
 from encord_active.app.model_assertions.sub_pages.true_positives import (
     TruePositivesPage,
 )
-from encord_active.app.views.export import export
+from encord_active.app.views.export_balance import export_balance
+from encord_active.app.views.export_filter import export_filter
 from encord_active.app.views.getting_started import getting_started
-from encord_active.app.views.indexes import explorer, summary
+from encord_active.app.views.metrics import explorer, summary
 from encord_active.app.views.model_assertions import model_assertions
 
 Pages = Dict[str, Union[Callable, "Pages"]]  # type: ignore
 
 pages: Pages = {
     "Getting Started": getting_started,
     "Data Quality": {"Summary": summary(MetricType.DATA_QUALITY), "Explorer": explorer(MetricType.DATA_QUALITY)},
@@ -35,15 +36,15 @@
     "Model Assertions": {
         "Metrics": model_assertions(MetricsPage()),
         "Performance By Metric": model_assertions(PerformanceMetric()),
         "True Positives": model_assertions(TruePositivesPage()),
         "False Positives": model_assertions(FalsePositivesPage()),
         "False Negatives": model_assertions(FalseNegativesPage()),
     },
-    "Actions": export,
+    "Actions": {"Filter & Export": export_filter, "Balance & Export": export_balance},
 }
 
 SEPARATOR = "#"
 
 
 def to_item(k, v, parent_key: Optional[str] = None):
     # NOTE: keys must be unique for the menu to render properly
```

### Comparing `encord-active-0.1.8/src/encord_active/app/views/export.py` & `encord-active-0.1.9/src/encord_active/app/views/export_filter.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,117 +3,110 @@
 
 import pandas as pd
 import streamlit as st
 from pandas.api.types import (
     is_categorical_dtype,
     is_datetime64_any_dtype,
     is_numeric_dtype,
-    is_object_dtype,
 )
 
 import encord_active.app.common.state as state
+from encord_active.app.common.action_utils import create_new_project_on_encord_platform
 from encord_active.app.common.utils import load_merged_df, set_page_config, setup_page
 from encord_active.app.db.tags import Tags
 
 
 def filter_dataframe(df: pd.DataFrame) -> pd.DataFrame:
     """
     Adds a UI on top of a dataframe to let apps filter columns
 
     Args:
         df (pd.DataFrame): Original dataframe
 
     Returns:
         pd.DataFrame: Filtered dataframe
     """
-    modify = st.checkbox("Add filters")
-
-    if not modify:
-        return df
-
-    df = df.copy()
-
-    # Try to convert datetimes into a standard format (datetime, no timezone)
-    for col in df.columns:
-        if is_object_dtype(df[col]):
-            try:
-                df[col] = pd.to_datetime(df[col])
-            except Exception:
-                pass
-
-        if is_datetime64_any_dtype(df[col]):
-            df[col] = df[col].dt.tz_localize(None)
-
-    modification_container = st.container()
-
-    with modification_container:
+    with st.container():
         columns_to_filter = df.columns.to_list()
-        columns_to_filter.remove("url")
+        if "url" in columns_to_filter:
+            columns_to_filter.remove("url")
+        # Move tags to first option.
+        tags_column = columns_to_filter.pop(columns_to_filter.index("tags"))
+        columns_to_filter = [tags_column] + columns_to_filter
+
         to_filter_columns = st.multiselect("Filter dataframe on", columns_to_filter)
+        if to_filter_columns:
+            df = df.copy()
+
         for column in to_filter_columns:
             left, right = st.columns((1, 20))
             left.write("↳")
+            key = f"filter-select-{column.replace(' ', '_').lower()}"
 
             if column == "tags":
-                tag_filters = right.multiselect("Choose tags to filter", options=Tags().all())
+                tag_filters = right.multiselect("Choose tags to filter", options=Tags().all(), key=key)
                 filtered_rows = [True if set(tag_filters) <= set(x) else False for x in df["tags"]]
                 df = df.loc[filtered_rows]
 
             # Treat columns with < 10 unique values as categorical
             elif is_categorical_dtype(df[column]) or df[column].nunique() < 10:
                 if df[column].isnull().sum() != df.shape[0]:
                     user_cat_input = right.multiselect(
                         f"Values for {column}",
                         df[column].unique(),
                         default=list(df[column].unique()),
+                        key=key,
                     )
                     df = df[df[column].isin(user_cat_input)]
                 else:
                     right.markdown(f"For column *{column}*, all values are NaN")
             elif is_numeric_dtype(df[column]):
                 _min = float(df[column].min())
                 _max = float(df[column].max())
                 step = (_max - _min) / 100
                 user_num_input = right.slider(
                     f"Values for {column}",
                     min_value=_min,
                     max_value=_max,
                     value=(_min, _max),
                     step=step,
+                    key=key,
                 )
                 df = df[df[column].between(*user_num_input)]
             elif is_datetime64_any_dtype(df[column]):
                 first = df[column].min()
                 last = df[column].max()
                 res = right.date_input(
-                    f"Values for {column}",
-                    min_value=first,
-                    max_value=last,
-                    value=(first, last),
+                    f"Values for {column}", min_value=first, max_value=last, value=(first, last), key=key
                 )
                 if isinstance(res, tuple) and len(res) == 2:
                     res = cast(Tuple[pd.Timestamp, pd.Timestamp], map(pd.to_datetime, res))  # type: ignore
                     start_date, end_date = res
                     df = df.loc[df[column].between(start_date, end_date)]
             else:
                 user_text_input = right.text_input(
                     f"Substring or regex in {column}",
+                    key=key,
                 )
                 if user_text_input:
                     df = df[df[column].astype(str).str.contains(user_text_input)]
 
     return df
 
 
-def export():
+def export_filter():
     setup_page()
     message_placeholder = st.empty()
 
+    st.markdown("# Actions")
+
     load_merged_df()
     filtered_df = filter_dataframe(st.session_state[state.MERGED_DATAFRAME].copy())
+    filtered_df.reset_index(inplace=True)
+    st.subheader("Filter & Export")
     st.markdown(f"**Total row:** {filtered_df.shape[0]}")
     st.dataframe(filtered_df, use_container_width=True)
 
     action_columns = st.columns((5, 2, 2, 2))
     action_columns[0].download_button(
         "⬇ Download filtered data",
         filtered_df.to_csv(index=False).encode("utf-8"),
@@ -125,19 +118,46 @@
 
     if any([delete_btn, edit_btn, augment_btn]):
         message_placeholder.markdown(
             """
 <div class="encord-active-info-box">
     🛠️ We're working hard on this feature - but not quite there yet.
     Please get in touch with Encord on the
-    <a href="https://encordactive.slack.com" target="_blank"><i class="fa-brands fa-slack"></i> Encord Active Slack community</a>
+    <a href="https://encordactive.slack.com" target="_blank"><i class="fa-brands fa-slack"></i> Encord Active Slack 
+community</a>
     or shoot us an
-    <a href="mailto:support@encord.com" target="_blank"><i class="fa fa-envelope"></i> email</a> for more information and help 🙏
+    <a href="mailto:support@encord.com" target="_blank"><i class="fa fa-envelope"></i> email</a> for more information 
+and help 🙏
 </div>
 """,
             unsafe_allow_html=True,
         )
 
+    with st.expander("Create a new project with the selected items"):
+        l_column, r_column = st.columns(2)
+
+        dataset_title = l_column.text_input(
+            "Dataset title", value=f"Subset: {st.session_state.project_dir.name} ({filtered_df.shape[0]})"
+        )
+        dataset_description = l_column.text_area("Dataset description")
+
+        project_title = r_column.text_input(
+            "Project title", value=f"Sub-project: {st.session_state.project_dir.name} ({filtered_df.shape[0]})"
+        )
+        project_description = r_column.text_area("Project description")
+
+        create_new_project = st.button("➕ Create")
+        if create_new_project:
+            if dataset_title == "":
+                st.error("Dataset title cannot be empty!")
+                return
+            if project_title == "":
+                st.error("Project title cannot be empty!")
+                return
+            create_new_project_on_encord_platform(
+                dataset_title, dataset_description, project_title, project_description, filtered_df
+            )
+
 
 if __name__ == "__main__":
     set_page_config()
-    export()
+    export_filter()
```

### Comparing `encord-active-0.1.8/src/encord_active/app/views/getting_started.py` & `encord-active-0.1.9/src/encord_active/app/views/getting_started.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/views/indexes.py` & `encord-active-0.1.9/src/encord_active/app/views/metrics.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/app/views/model_assertions.py` & `encord-active-0.1.9/src/encord_active/app/views/model_assertions.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         setup_page()
 
         if not pred_data.check_model_prediction_availability():
             st.markdown(
                 "# Missing Model Predictions\n"
                 "This project does not have any imported predictions. "
                 "Please refer to the "
-                "[Importing Model Predictions](https://encord-active-docs.web.app/api/importing-model-predictions) "
+                "[Importing Model Predictions](https://encord-active-docs.web.app/sdk/importing-model-predictions) "
                 "section of the documentation to learn how to import your predictions."
             )
             return
 
         st.session_state.selected_class_idx = pred_data.get_class_idx()
         st.session_state.full_class_idx = deepcopy(pred_data.get_class_idx())
         (
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/common/iterator.py` & `encord-active-0.1.9/src/encord_active/lib/common/iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,19 @@
             else:
                 objects = object  # object is expected to be a list[dict]
             hashes = [obj["objectHash"] if "objectHash" in obj else obj["classificationHash"] for obj in objects]
             return "_".join(chain([key], hashes))
         return key
 
     def get_data_url(self) -> str:
-        return f"https://app.encord.com/label_editor/{self.label_row_meta[self.label_hash]['data_hash']}&{self.project.project_hash}"
+        base_url = "https://app.encord.com/label_editor/"
+        data_url = f"{base_url}{self.label_row_meta[self.label_hash]['data_hash']}&{self.project.project_hash}"
+        if isinstance(self.frame, int):
+            data_url += f"/{self.frame}"
+        return data_url
 
     @staticmethod
     def __filter_logs_on_object_hash(logs: List[dict], object_hash: Optional[str] = None) -> List[dict]:
         if object_hash is None:
             return logs
 
         return list(filter(lambda x: x["annotation_hash"] == object_hash, logs))
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/common/metric.py` & `encord-active-0.1.9/src/encord_active/lib/common/metric.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/common/prepare.py` & `encord-active-0.1.9/src/encord_active/lib/common/prepare.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/common/tester.py` & `encord-active-0.1.9/src/encord_active/lib/common/tester.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/common/utils.py` & `encord-active-0.1.9/src/encord_active/lib/common/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     private_key_file = Path(project_meta["ssh_key_path"]).expanduser().absolute()
     with private_key_file.open("r", encoding="utf-8") as f:
         private_key = f.read()
     client = EncordUserClient.create_with_ssh_private_key(private_key)
 
     # == Project hash == #
     if "project_hash" not in project_meta:
-        raise ValueError("Project ID is missing in project metadata.")
+        raise ValueError("`project_hash` is missing in project metadata.")
     project_hash = project_meta["project_hash"]
     project = client.get_project(project_hash=project_hash)
     return project
 
 
 def get_du_size(data_unit, img_pth):
     if "width" not in data_unit.keys() or "height" not in data_unit.keys():
@@ -199,32 +199,49 @@
     if transformed_obj is not None:
         return cv2.boundingRect(transformed_obj)
     else:
         logger.debug("Detected invalid polygon (self-crossing or less than 3 vertices).")
         return None
 
 
-def fix_duplicate_image_orders_in_knn_graph(nearest_metrics: np.ndarray) -> np.ndarray:
+def fix_duplicate_image_orders_in_knn_graph_all_rows(nearest_items: np.ndarray) -> np.ndarray:
     """
     Duplicate images create problem in nearest neighbor order, for example for index 6 its closest
     neighbors can be [5,6,1,9,3] if 5 and 6 is duplicate, it should be [6,5,1,9,3]. This function ensures that
     the first item is the queried index.
 
-    :param nearest_metrics: nearest metrics obtained from search method of faiss index
+    :param nearest_items: nearest metrics obtained from search method of faiss index
     :return: fixed nearest metrics
     """
-    for i, row in enumerate(nearest_metrics):
+    for i, row in enumerate(nearest_items):
         if i != row[0]:
             target_index = np.where(row == i)
             if len(target_index[0]) == 0:
                 row[0] = i
             else:
                 row[0], row[target_index[0][0]] = row[target_index[0][0]], row[0]
 
-    return nearest_metrics
+    return nearest_items
+
+
+def fix_duplicate_image_orders_in_knn_graph_single_row(row_no: int, nearest_items: np.ndarray) -> np.ndarray:
+    """
+    Duplicate images create problem in nearest neighbor order, for example for index 6 its closest
+    neighbors can be [5,6,1,9,3] if 5 and 6 is duplicate, it should be [6,5,1,9,3]. This function ensures that
+    the first item is the queried index.
+
+    :param nearest_items: nearest metrics obtained from search method of faiss index
+    :return: fixed nearest metrics
+    """
+    if nearest_items[0, 0] == row_no:
+        return nearest_items
+    else:
+        target_index = np.where(nearest_items[0] == row_no)
+        nearest_items[0, 0], nearest_items[0, target_index[0]] = nearest_items[0, target_index[0]], nearest_items[0, 0]
+        return nearest_items
 
 
 def binary_mask_to_rle(mask: np.ndarray) -> Dict[str, list]:
     """
     Converts a binary mask into a Run-length Encoding (RLE).
 
     :param binary_mask: A [h, w] binary mask.
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/common/writer.py` & `encord-active-0.1.9/src/encord_active/lib/common/writer.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/embeddings/cnn_embed.py` & `encord-active-0.1.9/src/encord_active/lib/embeddings/cnn_embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 
 def assemble_object_batch(data_unit: dict, img_path: Path, transforms: Optional[nn.Module]):
     if transforms is None:
         transforms = torch.nn.Sequential()
 
     image = image_path_to_tensor(img_path)
     img_batch: List[torch.Tensor] = []
-    for obj in data_unit["labels"]["objects"]:
+
+    for obj in data_unit["labels"].get("objects", []):
         if obj["shape"] in [ObjectShape.POLYGON.value, ObjectShape.BOUNDING_BOX.value]:
             try:
                 out = get_bbox_from_encord_label_object(
                     obj,
                     image.shape[2],
                     image.shape[1],
                 )
@@ -144,15 +145,15 @@
         temp_entry = {}
         temp_entry["label_row"] = iterator.label_hash
         temp_entry["data_unit"] = data_unit["data_hash"]
         temp_entry["frame"] = data_unit["data_sequence"]
         temp_entry["url"] = data_unit["data_link"]
 
         temp_classification_hash = {}
-        for classification in data_unit["labels"]["classifications"]:
+        for classification in data_unit["labels"].get("classifications", []):
 
             classification_hash = classification["classificationHash"]
             question_feature_hash = classification["featureHash"]
             if question_feature_hash in feature_node_hash_to_index:
                 for classification_answer in iterator.label_rows[iterator.label_hash]["classification_answers"][
                     classification_hash
                 ]["classifications"]:
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/embeddings/hu_embed.py` & `encord-active-0.1.9/src/encord_active/lib/embeddings/hu_embed.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def generate_hu_embeddings(iterator: Iterator):
     with CSVEmbeddingWriter(iterator.cache_dir, iterator, prefix=HU_FILENAME) as writer:
         for data_unit, img_pth in iterator.iterate(desc="Generating HU embeddings"):
             height, width = get_du_size(data_unit, img_pth)
 
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 if obj["shape"] != "polygon":
                     continue
 
                 points = get_object_coordinates(obj)
                 if not points:  # avoid corrupted objects without vertices (empty list - [])
                     continue
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/example.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/example.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         # You can build/load databases of embeddings, compute statistics etc,
         # ...
 
         for data_unit, img_pth in iterator.iterate(desc="Progress bar description"):
             # Frame level score (data quality)
             writer.write_score(score=1337, description="Your description of the index score [can be omitted]")
 
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 # Object level score (label / model prediction quality)
                 if not obj["shape"] in valid_annotation_types:
                     continue
 
                 # This is where you do the actual inference.
 
                 # Some convenient properties associated with the current data.
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/fetch_prebuilt_metrics.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/fetch_prebuilt_metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import shutil
 from pathlib import Path
 
 import gdown
+from rich import print
+from rich.panel import Panel
 
 # Google Drive links for the projects will be added here
 PREBUILT_PROJECTS = {
     "[open-source][validation]-coco-2017-dataset": "https://drive.google.com/file/d/1iWx_y0r9I9Aay-nCo0ZMob2bI176v95b/view?usp=sharing",
     "[open-source][test]-limuc-ulcerative-colitis-classification": "https://drive.google.com/file/d/1Bw3uBIxDqyOlt7hincYbFgusU9FVf-OT/view?usp=sharing",
     "[open-source]-covid-19-segmentations": "https://drive.google.com/file/d/1Alo-4cqeGd1gcwQRxr3axz_QL8au1mjo/view?usp=sharing",
     "[open-source][validation]-bdd-dataset": "https://drive.google.com/file/d/1mJisC2yLU_5lzrrZquIXe5KJ2txkgdXx/view?usp=sharing",
@@ -33,10 +35,20 @@
     if not out_dir.is_dir():
         exit()
 
     gdown.download(url=url, output=output_file_path.as_posix(), quiet=False, fuzzy=True)
     print("Unpacking zip file. May take a bit.")
     shutil.unpack_archive(output_file_path, out_dir)
     os.remove(output_file_path)
-    print("Done.\n")
 
-    print("To view the data, run:\n" f'encord-active visualise "{out_dir}"')
+    print(
+        Panel(
+            f"""
+Successfully downloaded sandbox dataset. To view the data, run:
+
+[cyan blink]encord-active visualise "{out_dir}"
+        """,
+            title="🌟 Success 🌟",
+            style="green",
+            expand=False,
+        )
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/geometric/annotation_duplicates.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/geometric/annotation_duplicates.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.threshold = threshold
 
     def test(self, iterator: Iterator, writer: CSVMetricWriter):
         valid_annotation_types = {annotation_type.value for annotation_type in self.ANNOTATION_TYPE}
         found_any = False
 
         for data_unit, _ in iterator.iterate(desc="Looking for duplicates"):
-            objects = [obj for obj in data_unit["labels"]["objects"] if obj["shape"] in valid_annotation_types]
+            objects = [obj for obj in data_unit["labels"].get("objects", []) if obj["shape"] in valid_annotation_types]
             polygons = [get_polygon(obj) for obj in objects]
 
             duplicated_annotations = set()
             for i, obj1 in enumerate(objects):
                 score = 0.0
                 match = None
                 for j, obj2 in enumerate(objects):
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/geometric/hu_static.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/geometric/hu_static.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         hu_moments_df = get_hu_embeddings(iterator, force=True)
 
         moments_list: List[np.ndarray] = []
         obj_list: List[dict] = []
         obj_hashes: List[str] = []
         cls_list: List[str] = []
         for data_unit, img_pth in iterator.iterate(desc="Computing HU moments"):
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 if obj["shape"] not in valid_annotation_types:
                     continue
 
                 points = get_object_coordinates(obj)
                 if not points:  # avoid corrupted objects without vertices ([])
                     continue
 
@@ -71,27 +71,28 @@
 
         X = np.stack(moments_list, axis=0)
         X = (X - X.mean(0)) / X.std(0)
 
         distance_vector = 1 / compute_cls_distances(X, cls_ary)
         n = len(obj_list)
         for data_unit, img_pth in iterator.iterate(desc="writing scores"):
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 try:
                     index = obj_hashes.index(obj["objectHash"])
                 except:
                     continue
 
                 writer.write_score(objects=obj, score=float(distance_vector[index]), object_class=cls_list[index])
 
         pca_coordinates = PCA(n_components=2).fit_transform(X)
         with CSVEmbeddingWriter(iterator.cache_dir, iterator, prefix="hu_2d-embedding") as coords_writer:
             for data_unit, img_pth in iterator.iterate(desc="writing scores"):
-                for obj in data_unit["labels"]["objects"]:
-                    try:
-                        index = obj_hashes.index(obj["objectHash"])
-                    except:
-                        continue
-
-                    coords_writer.write_embedding(
-                        objects=obj, value=pca_coordinates[index].tolist(), object_class=cls_list[index]
-                    )
+                if "objects" in data_unit["labels"]:
+                    for obj in data_unit["labels"]["objects"]:
+                        try:
+                            index = obj_hashes.index(obj["objectHash"])
+                        except:
+                            continue
+
+                        coords_writer.write_embedding(
+                            objects=obj, value=pca_coordinates[index].tolist(), object_class=cls_list[index]
+                        )
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/geometric/hu_temporal.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/geometric/hu_temporal.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         found_any = False
 
         moment_store = MomentStore()
         hu_moments_df = get_hu_embeddings(iterator)
         hu_moments_identifiers = set(hu_moments_df["identifier"])
 
         for data_unit, img_pth in iterator.iterate(desc="Computing moment similarity"):
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 if obj["shape"] not in valid_annotation_types:
                     continue
 
                 key = writer.get_identifier(obj)
                 if key not in hu_moments_identifiers:  # check if identifier was discarded by get_hu_embeddings
                     continue
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/geometric/image_border_closeness.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/geometric/image_border_closeness.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ]
 
     def test(self, iterator: Iterator, writer: CSVMetricWriter):
         valid_annotation_types = {annotation_type.value for annotation_type in self.ANNOTATION_TYPE}
         found_any = False
 
         for data_unit, _ in iterator.iterate(desc="Computing closeness to border"):
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 if obj["shape"] not in valid_annotation_types:
                     continue
 
                 coordinates = get_object_coordinates(obj)
                 if not coordinates:  # avoid corrupted objects without vertices ([]) and unknown objects' shape (None)
                     continue
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/geometric/object_size.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/geometric/object_size.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ]
 
     def test(self, iterator: Iterator, writer: CSVMetricWriter):
         valid_annotation_types = {annotation_type.value for annotation_type in self.ANNOTATION_TYPE}
         found_any = False
 
         for data_unit, _ in iterator.iterate(desc="Computing object area"):
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 if obj["shape"] not in valid_annotation_types:
                     continue
                 obj_area = get_area(obj)
                 writer.write_score(objects=obj, score=100 * obj_area)
                 found_any = True
 
         if not found_any:
@@ -67,15 +67,15 @@
 
     def test(self, iterator: Iterator, writer: CSVMetricWriter):
         valid_annotation_types = {annotation_type.value for annotation_type in self.ANNOTATION_TYPE}
         found_any = False
 
         for data_unit, _ in iterator.iterate(desc="Computing total object area"):
             polygons = []
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 if obj["shape"] not in valid_annotation_types:
                     continue
 
                 poly = get_polygon(obj)
                 if not poly:  # avoid corrupted objects without vertices ([]) and polygons with less than 3 vertices
                     continue
                 polygons.append(poly)
@@ -105,15 +105,15 @@
         valid_annotation_types = {annotation_type.value for annotation_type in self.ANNOTATION_TYPE}
         found_any = False
 
         for data_unit, img_pth in iterator.iterate(desc="Computing pixel area"):
             img_h, img_w = get_du_size(data_unit, img_pth)
             img_area = img_h * img_w
 
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 if obj["shape"] not in valid_annotation_types:
                     continue
                 obj_area = get_area(obj)
                 pixel_area = int(img_area * obj_area)
                 writer.write_score(objects=obj, score=pixel_area)
                 found_any = True
 
@@ -136,15 +136,15 @@
 
     def test(self, iterator: Iterator, writer: CSVMetricWriter):
         valid_annotation_types = {annotation_type.value for annotation_type in self.ANNOTATION_TYPE}
         found_any = False
 
         for data_unit, img_pth in iterator.iterate(desc="Computing aspect ratio"):
             img_h, img_w = get_du_size(data_unit, img_pth)
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 if obj["shape"] not in valid_annotation_types:
                     continue
 
                 bbox = get_bbox_from_encord_label_object(obj, w=img_w, h=img_h)
                 if bbox is None:
                     continue
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/geometric/occlusion_detection_video.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/geometric/occlusion_detection_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             logger.info("<yellow>[Skipping]</yellow> No videos in dataset. ")
 
         for data_unit, img_pth in iterator.iterate(desc="Storing occlusion index"):
             label_row_hash = iterator.label_hash
             if label_row_hash not in videos.keys():
                 continue
 
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 object_hash = obj["objectHash"]
                 if (
                     obj["shape"] not in valid_annotation_types
                     or "scores" not in videos[label_row_hash][object_hash].keys()
                 ):
                     continue
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/_annotation_time.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/_annotation_time.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/high_iou_changing_classes.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/high_iou_changing_classes.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/img_features.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/img_features.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/missing_objects_and_wrong_tracks.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/missing_objects_and_wrong_tracks.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             )
             return
 
         # Collect the results in the CSV file.
         # Everything not found above with get score "1" meaning "no issues".
         annotated = {k: False for k in error_store.errors}
         for data_unit, _ in iterator.iterate(desc="Storing results"):
-            for obj in data_unit["labels"]["objects"]:
+            for obj in data_unit["labels"].get("objects", []):
                 oh = obj["objectHash"]
                 if oh in error_store.errors:
                     annotated[oh] = True
                     _obj, score, desc = error_store.errors[oh]
                     writer.write_score(objects=_obj, score=score, description=desc)
 
         if not all(annotated.values()):
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/heuristic/object_counting.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/heuristic/object_counting.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,9 +9,12 @@
     LONG_DESCRIPTION = r"""Counts number of objects in the image."""
     METRIC_TYPE = MetricType.HEURISTIC
     DATA_TYPE = DataType.IMAGE
     ANNOTATION_TYPE = AnnotationType.ALL
 
     def test(self, iterator: Iterator, writer: CSVMetricWriter):
         for data_unit, img_pth in iterator.iterate(desc="Counting objects"):
-            score = len(data_unit["labels"]["objects"])
-            writer.write_score(score=score)
+            if "objects" in data_unit["labels"]:
+                score = len(data_unit["labels"]["objects"])
+                writer.write_score(score=score)
+            else:
+                writer.write_score(score=0)
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/run_all.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/run_all.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from encord_active.lib.common.metric import AnnotationType, DataType, Metric, MetricType
 from encord_active.lib.common.tester import perform_test
 
 
 def get_metrics(module: Optional[Union[str, list[str]]] = None, filter_func=lambda x: True):
     if module is None:
         module = ["geometric", "heuristic", "semantic"]
+    elif isinstance(module, str):
+        module = [module]
 
-    metrics = []
-    if isinstance(module, list):  # type: ignore
-        for module in module:
-            metrics.extend(get_metrics(module, filter_func))
-    else:
-        metrics.extend(get_module_metrics(module, filter_func))
-
-    return metrics
+    return [i for m in module for i in get_module_metrics(m, filter_func)]
 
 
 def get_module_metrics(module_name: str, filter_func: Callable) -> List:
     base_module_name = __name__[: __name__.rindex(".")]  # Remove "run_all"
     metrics = []
     path = os.path.join(os.path.dirname(__file__), *module_name.split("."))
     for file in os.listdir(path):
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/semantic/_class_uncertainty.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/semantic/_class_uncertainty.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/semantic/_heatmap_uncertainty.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/semantic/_heatmap_uncertainty.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/semantic/img_classification_quality.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/semantic/img_classification_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
             nearest_indexes = self.get_nearest_indexes()
             self.fix_nearest_indexes(nearest_indexes)
             key_score_pairs = self.create_key_score_pairs(nearest_indexes)
 
             for data_unit, img_pth in iterator.iterate(desc="Storing index"):
                 key = iterator.get_identifier()
                 if key in key_score_pairs:
-                    for classification in data_unit["labels"]["classifications"]:
+                    for classification in data_unit["labels"].get("classifications", []):
                         question_featureHash = classification["featureHash"]
                         if question_featureHash in key_score_pairs[key]:
                             writer.write_score(
                                 key=key + "_" + question_featureHash,
                                 value=key_score_pairs[key][question_featureHash]["score"],
                                 description=key_score_pairs[key][question_featureHash]["description"],
                                 objects=classification,
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/metrics/semantic/img_object_quality.py` & `encord-active-0.1.9/src/encord_active/lib/metrics/semantic/img_object_quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from encord_active.lib.common.metric import (
     AnnotationType,
     DataType,
     EmbeddingType,
     Metric,
     MetricType,
 )
-from encord_active.lib.common.utils import fix_duplicate_image_orders_in_knn_graph
+from encord_active.lib.common.utils import (
+    fix_duplicate_image_orders_in_knn_graph_all_rows,
+)
 from encord_active.lib.common.writer import CSVMetricWriter
 from encord_active.lib.embeddings.cnn_embed import get_cnn_embeddings
 
 logger = logging.getLogger(__name__)
 
 
 class ObjectEmbeddingSimilarityTest(Metric):
@@ -112,26 +114,26 @@
 
             self.unpack_collections(collections)
 
             embedding_database, index, noisy_labels = self.convert_to_index()
             nearest_distances, nearest_metrics = index.search(  # pylint: disable=no-value-for-parameter
                 embedding_database, self.num_nearest_neighbors
             )
-            nearest_metrics = fix_duplicate_image_orders_in_knn_graph(nearest_metrics)
+            nearest_metrics = fix_duplicate_image_orders_in_knn_graph_all_rows(nearest_metrics)
 
             nearest_labels = np.take(noisy_labels, nearest_metrics)
             noisy_labels_tmp, nearest_labels_except_self = np.split(nearest_labels, [1], axis=-1)
             assert np.all(noisy_labels == noisy_labels_tmp.squeeze()), "Failed class index extraction"
 
             label_matches = np.equal(nearest_labels_except_self, np.expand_dims(noisy_labels, axis=-1))
             collections_scores = label_matches.mean(axis=-1)
 
             valid_annotation_types = {annotation_type.value for annotation_type in self.ANNOTATION_TYPE}
             for data_unit, img_pth in iterator.iterate(desc="Storing index"):
-                for obj in data_unit["labels"]["objects"]:
+                for obj in data_unit["labels"].get("objects", []):
                     if obj["shape"] not in valid_annotation_types:
                         continue
 
                     key = iterator.get_identifier(object=obj)
                     if key in self.collections:
                         assert obj["name"] == self.collections[key]["name"], "Indexing inconsistencies"
                         idx = embedding_identifiers.index(key)
```

### Comparing `encord-active-0.1.8/src/encord_active/lib/model_predictions/importers.py` & `encord-active-0.1.9/src/encord_active/lib/model_predictions/importers.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/model_predictions/iterator.py` & `encord-active-0.1.9/src/encord_active/lib/model_predictions/iterator.py`

 * *Files identical despite different names*

### Comparing `encord-active-0.1.8/src/encord_active/lib/model_predictions/prediction_writer.py` & `encord-active-0.1.9/src/encord_active/lib/model_predictions/prediction_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,28 +245,35 @@
                 None,  # bbox.y1
                 None,  # bbox.x2
                 None,  # bbox.y2
                 None,  # RLE encoding of mask
             ]
 
             if o["shape"] == "bounding_box":
-                x, y, w, h = [o["boundingBox"][k] for k in ["x", "y", "w", "h"]]
+                bbox = o.get("boundingBox")
+                if not (bbox and self.__check_bbox(bbox)):
+                    return  # Invalid bounding box object
+
+                x, y, w, h = [bbox[k] for k in ["x", "y", "w", "h"]]
                 row[LKey.X1.value] = round(x * width, 2)  # bbox.x1
                 row[LKey.Y1.value] = round(y * height, 2)  # bbox.y1
                 row[LKey.X2.value] = round((x + w) * width, 2)  # bbox.x2
                 row[LKey.Y2.value] = round((y + h) * height, 2)  # bbox.y2
             elif o["shape"] == "polygon":
                 points = polyobj_to_nparray(o, width=width, height=height)
-                mask = points_to_mask(points, width=width, height=height)
+                if points.size == 0:
+                    return
                 x1, y1 = points.min(axis=0)
                 x2, y2 = points.max(axis=0)
                 row[LKey.X1.value] = x1  # bbox.x1
                 row[LKey.Y1.value] = y1  # bbox.y1
                 row[LKey.X2.value] = x2  # bbox.x2
                 row[LKey.Y2.value] = y2  # bbox.y2
+
+                mask = points_to_mask(points, width=width, height=height)
                 row[LKey.RLE.value] = binary_mask_to_rle(mask)
             else:
                 # Only supporting polygons and bounding boxes.
                 return
             self.object_labels.append(row)
 
         for label_hash, lr in tqdm(self.label_rows.items(), desc="Preparing labels", leave=True):
@@ -389,22 +396,22 @@
         mask = None
         label_hash = self.lr_lookup.get(data_hash, "unmatched")
         du = self.label_rows[label_hash]["data_units"][data_hash]
         if du is None:
             logger.warning(f"Couldn't match data hash `{data_hash}` to any label row")
             return
 
+        width = int(du["width"])
+        height = int(du["height"])
+
         ptype: PredictionType
         if bbox is None and polygon is None:
             raise NotImplementedError("Frame level classifications are not supported at the moment.")
             # ptype = PredictionType.FRAME
         elif bbox is None and isinstance(polygon, (np.ndarray, list)):
-            width = int(du["width"])
-            height = int(du["height"])
-
             ptype = PredictionType.POLYGON
             if isinstance(polygon, list):
                 polygon = np.array(polygon)
 
             if polygon.ndim != 2:
                 raise ValueError("Polygon argument should have just 2 dimensions: [h, w] or [N, 2]")
 
@@ -421,34 +428,38 @@
             x2, y2 = x1 + w, y1 + h
             points = [x1, y1, x2, y2]
             mask = binary_mask_to_rle(np_mask)
 
         elif isinstance(bbox, dict) and polygon is None:
             ptype = PredictionType.BBOX
             self.__check_bbox(bbox)
-            points = list(map(float, [bbox["x"], bbox["y"], bbox["x"] + bbox["w"], bbox["y"] + bbox["h"]]))
+            points = [
+                bbox["x"] * width,
+                bbox["y"] * height,
+                (bbox["x"] + bbox["w"]) * width,
+                (bbox["y"] + bbox["h"]) * height,
+            ]
         else:
             raise ValueError(
                 "Something seems wrong. Did you use the wrong types or did you parse both a bbox and polygon?"
             )
 
         # === Write key similar to the index writer (though object_hash will not be accessible here) === #
         label_hash = self.lr_lookup.get(data_hash, "unmatched")
         key = f"{label_hash}_{data_hash}"
 
-        _frame = -1
+        _frame = 0
         if frame is None:  # Try to infer frame number from data hash.
             if label_hash != "unmatched":
                 label_row = self.label_rows[label_hash]
                 data_unit = label_row["data_units"][data_hash]
 
                 if "data_sequence" in data_unit:
                     _frame = int(data_unit["data_sequence"])
-        if _frame != -1:
-            key += f"_{_frame:05d}"
+        key += f"_{_frame:05d}"
 
         object_hash = self.__get_unique_object_hash()
         key += f"_{object_hash}"
 
         class_id = self.object_class_id_lookup.get(class_uid)
         if class_id is None:
             raise ValueError(
```

### Comparing `encord-active-0.1.8/setup.py` & `encord-active-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,36 +40,38 @@
  'loguru>=0.6.0,<0.7.0',
  'matplotlib>=3.5.3,<4.0.0',
  'natsort>=8.1.0,<9.0.0',
  'numpy>=1.23.1,<2.0.0',
  'opencv-python==4.5.5.64',
  'pandas>=1.4.3,<2.0.0',
  'plotly>=5.10.0,<6.0.0',
+ 'pydantic>=1.10.2,<2.0.0',
  'python-dotenv>=0.21.0,<0.22.0',
  'pytz>=2022.2.1,<2023.0.0',
  'rich>=12.6.0,<13.0.0',
  'scikit-learn>=1.0.1,<2.0.0',
  'scipy==1.8.1',
  'screeninfo>=0.8.1,<0.9.0',
  'shapely>=1.7.0,<2.0.0',
  'streamlit-nested-layout>=0.1.1,<0.2.0',
  'streamlit==1.13.0',
  'termcolor>=2.0.1,<3.0.0',
+ 'toml>=0.10.2,<0.11.0',
  'torch>=1.12.1,<2.0.0',
  'torchvision>=0.13.1,<0.14.0',
  'typer>=0.6.1,<0.7.0',
  'types-pytz>=2022.2.1,<2023.0.0',
  'watchdog>=2.1.9,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['encord-active = encord_active.app.main:cli']}
 
 setup_kwargs = {
     'name': 'encord-active',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'Frederik Hvilshøj',
     'author_email': 'frederik@cord.tech',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `encord-active-0.1.8/PKG-INFO` & `encord-active-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord-active
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: AGPL-3.0-only
 Author: Frederik Hvilshøj
 Author-email: frederik@cord.tech
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -19,22 +19,24 @@
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: natsort (>=8.1.0,<9.0.0)
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
 Requires-Dist: opencv-python (==4.5.5.64)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: plotly (>=5.10.0,<6.0.0)
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: pytz (>=2022.2.1,<2023.0.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: scikit-learn (>=1.0.1,<2.0.0)
 Requires-Dist: scipy (==1.8.1)
 Requires-Dist: screeninfo (>=0.8.1,<0.9.0)
 Requires-Dist: shapely (>=1.7.0,<2.0.0)
 Requires-Dist: streamlit (==1.13.0)
 Requires-Dist: streamlit-nested-layout (>=0.1.1,<0.2.0)
 Requires-Dist: termcolor (>=2.0.1,<3.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: torch (>=1.12.1,<2.0.0)
 Requires-Dist: torchvision (>=0.13.1,<0.14.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: types-pytz (>=2022.2.1,<2023.0.0)
 Requires-Dist: watchdog (>=2.1.9,<3.0.0)
```

