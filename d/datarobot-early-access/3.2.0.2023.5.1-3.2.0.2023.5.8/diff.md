# Comparing `tmp/datarobot_early_access-3.2.0.2023.5.1.tar.gz` & `tmp/datarobot_early_access-3.2.0.2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.5.1.tar", last modified: Mon May  1 16:47:19 2023, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.5.8.tar", last modified: Mon May  8 16:47:08 2023, max compression
```

## Comparing `datarobot_early_access-3.2.0.2023.5.1.tar` & `datarobot_early_access-3.2.0.2023.5.8.tar`

### file list

```diff
@@ -1,168 +1,169 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   167636 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8482 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5638 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2298 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/data_matching.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      485 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54473 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7536 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17252 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1598 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24335 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7993 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1127 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/deployment_monitoring.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   100246 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4192 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7683 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23045 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    82114 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40817 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15409 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    56267 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12528 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12373 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    91264 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10058 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16677 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10333 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_fit.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21264 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   268121 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9419 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10203 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   209294 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55518 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/recommended_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6051 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      305 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20006 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/use_cases/use_case.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17381 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5622 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1079 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3184 2023-05-01 16:46:26.000000 datarobot_early_access-3.2.0.2023.5.1/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-05-01 16:46:26.000000 datarobot_early_access-3.2.0.2023.5.1/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-05-01 16:46:26.000000 datarobot_early_access-3.2.0.2023.5.1/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   169379 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8705 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5638 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2271 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/data_matching.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      485 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54473 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7536 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17252 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2063 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24305 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7993 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1127 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/deployment_monitoring.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   100246 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4044 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8437 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23045 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    83098 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40817 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15409 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    56459 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12528 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4829 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12639 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    93316 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10058 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16683 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21038 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   256106 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9565 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10203 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   209815 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55518 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/recommended_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6051 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19984 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1560 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17373 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5675 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1079 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3148 2023-05-08 16:46:20.000000 datarobot_early_access-3.2.0.2023.5.8/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-05-08 16:46:20.000000 datarobot_early_access-3.2.0.2023.5.8/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-05-08 16:46:20.000000 datarobot_early_access-3.2.0.2023.5.8/setup_weekly.py
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/CHANGES.rst` & `datarobot_early_access-3.2.0.2023.5.8/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,45 +28,65 @@
   :meth:`BatchMonitoringJobDefinition.create <datarobot.models.BatchMonitoringJobDefinition.create>`
   :meth:`BatchMonitoringJobDefinition.update <datarobot.models.BatchMonitoringJobDefinition.update>`
   :meth:`BatchMonitoringJobDefinition.delete <datarobot.models.BatchMonitoringJobDefinition.delete>`
   :meth:`BatchMonitoringJobDefinition.run_on_schedule <datarobot.models.BatchMonitoringJobDefinition.run_on_schedule>`
   :meth:`BatchMonitoringJobDefinition.run_once <datarobot.models.BatchMonitoringJobDefinition.run_once>`
 - Added a new method to retrieve a monitoring job
   :meth:`BatchMonitoringJob.get <datarobot.models.BatchMonitoringJob.get>`
-- Added the ability to filter return objects by Use Case ID to the following methods:
+- Added the ability to filter return objects by a Use Case ID passed to the following methods:
   :meth:`Dataset.list <datarobot.models.Dataset.list>`
   :meth:`Notebook.list <datarobot.Notebook.list>`
+  :meth:`Project.list <datarobot.models.Project.list>`
 
 - Added the ability to set a default :class:`UseCase <datarobot.UseCase>` for requests. It can be set by:
 
   - invoking `Client(..., use_case = <id>)`, or
   - setting `use_case: <id>` in drconfig.yaml, or
   - setting the env var DATAROBOT_DEFAULT_USE_CASE, or
   - calling `with UseCase.get(<id>):`.
 
+- Added method meth:`Deployment.get_predictions_over_time <datarobot.models.Deployment.get_predictions_over_time>` to retrieve deployment predictions over time data.
+
 Enhancements
 ************
 - Improve error message of :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>`
   to clarify that a selected parameter cannot be used when a project has not proceeded to the
   correct stage prior to calling this method.
 
 - Extended :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>` by two parameters
   to filter for a target value range in regression projects.
 
 - Added text explanations data to :meth:`PredictionExplanations <datarobot.PredictionExplanations>` and made sure it is returned in both :py:meth:`datarobot.PredictionExplanations.get_all_as_dataframe`  and :py:meth:`datarobot.PredictionExplanations.get_rows` method.
 
 Bugfixes
 ********
 - Fix incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
+- Fix a crash when using non-"latin-1" characters in Panda's DataFrame used as prediction data in :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
 
 API Changes
 ***********
 
 Deprecation Summary
 *******************
+- ``Model.get_feature_fit_metadata`` has been removed.
+  Use :meth:`Model.get_feature_effect_metadata <datarobot.models.Model.get_feature_effect_metadata>` instead.
+- ``DatetimeModel.get_feature_fit_metadata`` has been removed.
+  Use :meth:`DatetimeModel.get_feature_effect_metadata <datarobot.models.DatetimeModel.get_feature_effect_metadata>` instead.
+- ``Model.request_feature_fit`` has been removed.
+  Use :meth:`Model.request_feature_effect <datarobot.models.Model.request_feature_effect>` instead.
+- ``DatetimeModel.request_feature_fit`` has been removed.
+  Use :meth:`DatetimeModel.request_feature_effect <datarobot.models.DatetimeModel.request_feature_effect>` instead.
+- ``Model.get_feature_fit`` has been removed.
+  Use :meth:`Model.get_feature_effect <datarobot.models.Model.get_feature_effect>` instead.
+- ``DatetimeModel.get_feature_fit`` has been removed.
+  Use :meth:`DatetimeModel.get_feature_effect <datarobot.models.DatetimeModel.get_feature_effect>` instead.
+- ``Model.get_or_request_feature_fit`` has been removed.
+  Use :meth:`Model.get_or_request_feature_effect <datarobot.models.Model.get_or_request_feature_effect>` instead.
+- ``DatetimeModel.get_or_request_feature_fit`` has been removed.
+  Use :meth:`DatetimeModel.get_or_request_feature_effect <datarobot.models.DatetimeModel.get_or_request_feature_effect>` instead.
 
 Configuration Changes
 *********************
 - Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
 - Pins dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be less than version 2.0.0.
 
 Documentation Changes
@@ -547,17 +567,17 @@
 - Fix a bug in :meth:`datarobot.models.BatchPredictionJobDefinition.create` where `schedule` was not optional for all cases
 
 API Changes
 ***********
 
 - User can include ICE plots data in the response when requesting Feature Effects/Feature Fit. Extended methods are
     - :meth:`Model.get_feature_effect <datarobot.models.Model.get_feature_effect>`,
-    - :meth:`Model.get_feature_fit <datarobot.models.Model.get_feature_fit>`,
+    - ``Model.get_feature_fit <datarobot.models.Model.get_feature_fit>``,
     - :meth:`DatetimeModel.get_feature_effect <datarobot.models.DatetimeModel.get_feature_effect>` and
-    - :meth:`DatetimeModel.get_feature_fit <datarobot.models.DatetimeModel.get_feature_fit>`.
+    - ``DatetimeModel.get_feature_fit <datarobot.models.DatetimeModel.get_feature_fit>``.
 
 Deprecation Summary
 *******************
 
 - `attrs` library is removed from library dependencies
 - ``ImageAugmentationSample.compute`` was marked as deprecated and will be removed in v2.30. You
   can get the same information with newly introduced method ``ImageAugmentationList.compute_samples``
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/LICENSE.txt` & `datarobot_early_access-3.2.0.2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/PKG-INFO` & `datarobot_early_access-3.2.0.2023.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.2.0.2023.5.1
+Version: 3.2.0.2023.5.8
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/README.md` & `datarobot_early_access-3.2.0.2023.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,40 +31,51 @@
 ```
 
 Note: This may have to be run as `root` or with `--user` flag if you are not
 using python virtual environment.
 
 ## Build the documentation
 
+Docker env:
+
+```console
+make clean test-docs
+```
+
+Local virtual env:
+
+| WARNING: currently the documentation commands below needs py3.11 env in order to work (there seem to be an issue with type hinting) |
+| --- |
+
 > Be sure to install pandoc before building documentation. Available via `apt-get` and `brew`
 
 DataRobot has extensive documentation, which you can build locally for your
 own reference. Before running the following build commands, please make sure that your
 [public_api_client configuration](https://datarobot-public-api-client.readthedocs-hosted.com/en/v2.22.1/setup/getting_started.html#use-a-configuration-file)
 is present and valid or you have set the
 [correct environment variables](https://datarobot-public-api-client.readthedocs-hosted.com/en/v2.22.1/setup/getting_started.html#set-credentials-using-environment-variables).
 Otherwise building the docs will take a lot of time.
 
 ```console
-cd docs
+cd sdk_docs
 make clean html
 ```
 
 The documentation will then be built in a subdirectory, and can be viewed with
 your web browser.
 
 Alternatively, see <https://datarobot.atlassian.net/wiki/spaces/AIAPI/pages/28967932/Release+Tracker>
 for pre-built documentation for the current cloud release and all enterprise
 releases, as well as guidance on which version of the API goes with which
 enterprise release.
 
 To build a PDF of the docs for release:
 
 ```console
-cd docs
+cd sdk_docs
 make clean xelatexpdf
 ```
 
 ## Topics
 
 * Setup topics:
   * [Common DataRobot Client setup](#datarobot-client-setup)
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/common_setup.py` & `datarobot_early_access-3.2.0.2023.5.8/common_setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flake8: noqa
 
 from ._version import __version__
 from .client import Client
-from .context import _context
+from .context import Context
 from .enums import (
     AUTOPILOT_MODE,
     NETWORK_EGRESS_POLICY,
     QUEUE_STATUS,
     SCORING_TYPE,
     SNAPSHOT_POLICY,
     TARGET_TYPE,
@@ -100,9 +100,7 @@
     ShapMatrixJob,
     SharingAccess,
     TrainingPredictions,
     TrainingPredictionsJob,
     UseCase,
     UserBlueprint,
 )
-
-Context = _context.get()
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_compat.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/documentai/document.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model_package.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/client.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/context.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/context.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,17 +20,33 @@
 if TYPE_CHECKING:
     from .models.use_cases.use_case import UseCase
 
 DefaultUseCase = Optional[Union["UseCase", str]]
 
 
 @dataclass
-class Context:
+class _ContextGlobals:
     """
     Interface for initializing, accessing, and setting variables that should persist.
+
+    This class should not be used directly; rather, reference `datarobot.context.Context`.
+
+    Examples
+    --------
+        .. code-block:: python
+
+            from datarobot.context import Context
+
+            >>> def foobar(value: str) -> None:
+            ...  print(f"hey {value}")
+            ...  Context.use_case = value
+            ...
+            >>> foobar("Jude")
+            hey Jude
+            >>>
     """
 
     _use_case: DefaultUseCase = field(init=False, default=None)
 
     @property
     def use_case(self) -> DefaultUseCase:
         """Returns the default Use Case. If a string representing the Use Case ID
@@ -47,8 +63,10 @@
         return self._use_case or None
 
     @use_case.setter
     def use_case(self, value: DefaultUseCase = None) -> None:
         self._use_case = value
 
 
-_context: ContextVar[Context] = ContextVar("current_context", default=Context())
+_context: ContextVar[_ContextGlobals] = ContextVar("current_context", default=_ContextGlobals())
+
+Context = _context.get()
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/enums.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,14 @@
 
 JOB_TYPE = enum(
     BATCH_MONITORING="batchMonitoring",
     BATCH_PREDICTIONS="batchPredictions",
     BATCH_PREDICTION_JOB_DEFINITIONS="batchPredictionJobDefinitions",
     FEATURE_IMPACT="featureImpact",
     FEATURE_EFFECTS="featureEffects",
-    FEATURE_FIT="featureFit",
     MODEL="model",
     MODEL_EXPORT="modelExport",
     PREDICT="predict",
     TRAINING_PREDICTIONS="trainingPredictions",
     PRIME_MODEL="primeModel",
     PRIME_RULESETS="primeRulesets",
     PRIME_VALIDATION="primeDownloadValidation",
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/errors.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/deployment_monitoring.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/deployment_monitoring.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,20 +57,14 @@
 from .feature_effect import (
     FeatureEffectMetadata,
     FeatureEffectMetadataDatetime,
     FeatureEffectMetadataDatetimePerBacktest,
     FeatureEffects,
     FeatureEffectsMulticlass,
 )
-from .feature_fit import (
-    FeatureFit,
-    FeatureFitMetadata,
-    FeatureFitMetadataDatetime,
-    FeatureFitMetadataDatetimePerBacktest,
-)
 from .featurelist import DatasetFeaturelist, Featurelist, ModelingFeaturelist
 from .imported_model import ImportedModel
 from .job import FeatureImpactJob, Job, TrainingPredictionsJob
 from .model import (
     BlenderModel,
     ClusteringModel,
     CombinedModel,
@@ -116,9 +110,9 @@
     AnomalyAssessmentDataPoint,
     AnomalyAssessmentPreviewBin,
     AnomalyAssessmentRecordMetadata,
     RegionExplanationsData,
     RocCurveEstimatedMetric,
     ShapleyFeatureContribution,
 )
-from .use_cases import UseCase, UseCaseUser
+from .use_cases.use_case import UseCase
 from .user_blueprints import UserBlueprint
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/api_object.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/application.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,16 +188,48 @@
         self.deactivation_status_id = deactivation_status_id
         self.created_first_name = created_first_name
         self.creator_last_name = creator_last_name
         self.creator_userhash = creator_userhash
         self.deployments = deployments
 
     @classmethod
-    def list(cls, offset: Optional[int] = None, limit: Optional[int] = None) -> List[Application]:
+    def list(
+        cls,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+    ) -> List[Application]:
+        """
+        Retrieve a list of user applications.
+
+        Parameters
+        ----------
+        offset : Optional[int]
+            Optional. Retrieve applications in a list after this number.
+        limit : Optional[int]
+            Optional. Retrieve only this number of applications.
+
+        Returns
+        -------
+        applications : List[Application]
+            The requested list of user applications.
+        """
         query = {"offset": offset, "limit": limit}
         applications = unpaginate(initial_url=cls._path, initial_params=query, client=cls._client)
         return [cls.from_server_data(application) for application in applications]
 
     @classmethod
     def get(cls, application_id: str) -> Application:
+        """
+        Retrieve a single application.
+
+        Parameters
+        ----------
+        application_id : str
+            The ID of the application to retrieve.
+
+        Returns
+        -------
+        application : Application
+            The requested application.
+        """
         r_data = cls._client.get(f"{cls._path}{application_id}/")
         return cls.from_server_data(r_data.json())
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_prediction_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 
 import csv
 import datetime
 import io
 import os
 import threading
 import time
-from typing import cast, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
+from typing import Any, cast, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
 
 import pandas as pd
 import requests
 import trafaret as t
 
 from datarobot import errors
 from datarobot._compat import Int, String
 from datarobot.models.credential import Credential
 from datarobot.models.dataset import Dataset
 from datarobot.models.job import AbstractSpecificJob
 from datarobot.models.prediction_explanations import PredictionExplanationsMode
 from datarobot.models.project import Project
-from datarobot.utils import get_id_from_response, pagination, recognize_sourcedata, to_api
+from datarobot.utils import get_id_from_response, pagination
+from datarobot.utils import recognize_sourcedata as orig_recognize_sourcedata
+from datarobot.utils import to_api
 
 from ..enums import AVAILABLE_STATEMENT_TYPES, DEFAULT_TIMEOUT, JOB_TYPE, QUEUE_STATUS
 from ..utils import logger, parse_time
 from .api_object import APIObject
 
 LOG = logger.get_logger(__name__)
 
@@ -100,14 +102,31 @@
         day_of_week: List[Union[int, str]]
         month: List[Union[int, str]]
         hour: List[Union[int, str]]
         minute: List[Union[int, str]]
         day_of_month: List[Union[int, str]]
 
 
+def recognize_sourcedata(sourcedata: Any, default_fname: str) -> Dict[str, Any]:
+    """Override the default recognize_sourcedata with one that converts
+    DataFrame to io.BytesIO"""
+    if not isinstance(sourcedata, pd.DataFrame):
+        return orig_recognize_sourcedata(sourcedata, default_fname)
+    # The original recognize_sourcedata will encode dataframes into StringIO
+    # To pass this to requests.put, we need BytesIO - otherwise, requests will
+    # try to encode it using latin-1 encoding (the default HTTP encoding),
+    # which will crash when a charater not contained in latin-1 is used
+    #
+    # https://github.com/python/cpython/blob/b9797417315cc2d1700cb2d427685016d3380711/Lib/http/client.py#L1046
+    buf = io.BytesIO()
+    sourcedata.to_csv(buf, encoding="utf-8", index=False, quoting=csv.QUOTE_ALL)
+    buf.seek(0)
+    return {"filelike": buf, "fname": default_fname}
+
+
 class BatchPredictionJob(AbstractSpecificJob):
     """
     A Batch Prediction Job is used to score large data sets on
     prediction servers using the Batch Prediction API.
 
     Attributes
     ----------
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/blueprint.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/calendar_file.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/change_request.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/cluster.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/connector.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/credential.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_source.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_store.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/dataset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from datarobot.utils import assert_single_parameter, dataframe_to_buffer
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.source import parse_source_type
 from datarobot.utils.sourcedata import list_of_records_to_buffer
 from datarobot.utils.waiters import wait_for_async_resolution
 
 from ..enums import DEFAULT_MAX_WAIT, DEFAULT_TIMEOUT
+from .use_cases.utils import resolve_use_case
 
 ProjectLocation = namedtuple("ProjectLocation", ["url", "id"])
 
 FeatureTypeCount = namedtuple("FeatureTypeCount", ["count", "feature_type"])
 
 
 TDataset = TypeVar("TDataset", bound="Dataset")
@@ -677,14 +678,17 @@
             "offset": offset,
             "limit": limit,
             "category": category,
             "order_by": order_by,
             "filter_failed": filter_failed,
             "experiment_container_ids": use_case_ids,
         }
+        all_params = resolve_use_case(
+            use_case_id=use_case_ids, use_case_key="experiment_container_ids", params=all_params
+        )
         params = _remove_empty_params(all_params)
         _update_filter_failed(params)
 
         for dataset_json in unpaginate(cls._path, params, cls._client):
             yield cls.from_server_data(dataset_json)
 
     def update(self) -> None:
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/data_drift.py`

 * *Files 4% similar despite different names*

```diff
@@ -362,14 +362,15 @@
         cls,
         deployment_id: str,
         model_ids: Optional[List[str]] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         bucket_size: Optional[BUCKET_SIZE] = None,
         target_classes: Optional[List[str]] = None,
+        include_percentiles: Optional[bool] = False,
     ) -> PredictionsOverTime:
         """Retrieve information for deployment's prediction response over a certain time period.
 
         .. versionadded:: v3.2
 
         Parameters
         ----------
@@ -381,25 +382,29 @@
             start of the time period
         end_time : datetime
             end of the time period
         bucket_size : BUCKET_SIZE
             time duration of each bucket
         target_classes : list[str]
             class names of target, only for deployments with multiclass target
+        include_percentiles : bool
+            if the returned data includes percentiles,
+            only for a deployment with a binary and regression target
 
         Returns
         -------
         predictions_over_time : PredictionsOverTime
             the queried predictions over time information
         """
 
         path = cls._path.format(deployment_id)
         params = cls._build_query_params(
             start_time=start_time,
             end_time=end_time,
             model_ids=model_ids,
             bucket_size=bucket_size,
             target_class=target_classes,
+            include_percentiles=include_percentiles,
         )
         data = cls._client.get(path, params=params).json()
         case_converted = from_api(data, keep_null_keys=True)
         return cls.from_data(case_converted)
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from datarobot.errors import InvalidUsageError
 from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject, ServerDataDictType
 from datarobot.models.batch_prediction_job import BatchPredictionJob
 from datarobot.models.custom_model_version import CustomModelVersion
 from datarobot.models.deployment.accuracy import Accuracy, AccuracyOverTime
+from datarobot.models.deployment.bias_and_fairness import FairnessScoresOverTime
 from datarobot.models.deployment.data_drift import FeatureDrift, PredictionsOverTime, TargetDrift
 from datarobot.models.deployment.service_stats import ServiceStats, ServiceStatsOverTime
 from datarobot.models.deployment.sharing import (
     DeploymentGrantSharedRoleWithId,
     DeploymentGrantSharedRoleWithUsername,
     DeploymentSharedRole,
 )
@@ -1759,14 +1760,15 @@
     def get_predictions_over_time(
         self,
         model_ids: Optional[List[str]] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         bucket_size: Optional[BUCKET_SIZE] = None,
         target_classes: Optional[List[str]] = None,
+        include_percentiles: Optional[bool] = False,
     ) -> PredictionsOverTime:
         """Retrieve stats of deployment's prediction response over a certain time period.
 
         .. versionadded:: v3.2
 
         Parameters
         ----------
@@ -1776,39 +1778,47 @@
             start of the time period
         end_time : datetime
             end of the time period
         bucket_size : BUCKET_SIZE
             time duration of each bucket
         target_classes : list[str]
             class names of target, only for deployments with multiclass target
+        include_percentiles : bool
+            if the returned data includes percentiles,
+            only for a deployment with a binary and regression target
 
         Returns
         -------
         predictions_over_time : PredictionsOverTime
             the queried predictions over time information
 
         Examples
         --------
         .. code-block:: python
 
             from datarobot import Deployment
             deployment = Deployment.get(deployment_id='5c939e08962d741e34f609f0')
             predictions_over_time = deployment.get_predictions_over_time()
+            predictions_over_time.buckets[0]['mean_predicted_value']
+            >>>0.3772
+            predictions_over_time.buckets[0]['row_count']
+            >>>2000
         """
 
         if not self.id:
             raise ValueError("Deployment ID is required to get predictions over time.")
 
         return PredictionsOverTime.get(
             self.id,
             model_ids=model_ids,
             start_time=start_time,
             end_time=end_time,
             bucket_size=bucket_size,
             target_classes=target_classes,
+            include_percentiles=include_percentiles,
         )
 
     def get_accuracy(
         self,
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
@@ -1895,14 +1905,59 @@
             model_id=model_id,
             start_time=start_time,
             end_time=end_time,
             bucket_size=bucket_size,
             target_classes=target_classes,
         )
 
+    def get_fairness_scores_over_time(
+        self,
+        start_time: Optional[datetime] = None,
+        end_time: Optional[datetime] = None,
+        bucket_size: Optional[BUCKET_SIZE] = None,
+        model_id: Optional[str] = None,
+        protected_feature: Optional[str] = None,
+        fairness_metric: Optional[str] = None,
+    ) -> FairnessScoresOverTime:
+        """Retrieves values of a single fairness score over a time period.
+
+        .. versionadded:: v3.2
+
+        Parameters
+        ----------
+        model_id : str
+            the id of the model
+        start_time : datetime
+            start of the time period
+        end_time : datetime
+            end of the time period
+        bucket_size : str
+            time duration of a bucket, in ISO 8601 time duration format
+        protected_feature : str
+            name of protected feature
+        fairness_metric : str
+            A consolidation of the fairness metrics by the use case.
+
+        Returns
+        -------
+        fairness_scores_over_time : FairnessScoresOverTime
+            the queried fairness score over time information
+        """
+        if not self.id:
+            raise ValueError("Deployment ID is required to get fairness score.")
+        return FairnessScoresOverTime.get(
+            self.id,
+            start_time=start_time,
+            end_time=end_time,
+            model_id=model_id,
+            bucket_size=bucket_size,
+            fairness_metric=fairness_metric,
+            protected_feature=protected_feature,
+        )
+
     def update_secondary_dataset_config(
         self,
         secondary_dataset_config_id: str,
         credential_ids: Optional[List[str]] = None,
     ) -> str:
         """Update the secondary dataset config used by Feature discovery model for a
         given deployment.
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/driver.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/execution_environment.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_effect.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_effect.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class FeatureEffectMetadata(APIObject):
     """Feature Effect Metadata for model, contains status and available model sources.
 
     Notes
     -----
 
-    `source` is expected parameter to retrieve Feature Fit. One of provided sources
+    `source` is expected parameter to retrieve Feature Effect. One of provided sources
     shall be used.
 
     """
 
     _converter = t.Dict({t.Key("status"): String, t.Key("sources"): t.List(String)}).ignore_extra(
         "*"
     )
@@ -48,15 +48,15 @@
     Notes
     -----
     ``feature effect metadata per backtest`` contains:
         * ``status`` : string.
         * ``backtest_index`` : string.
         * ``sources`` : list(string).
 
-    `source` is expected parameter to retrieve Feature Fit. One of provided sources
+    `source` is expected parameter to retrieve Feature Effect. One of provided sources
     shall be used.
 
     `backtest_index` is expected parameter to submit compute request and retrieve Feature Effect.
     One of provided backtest indexes shall be used.
 
     Attributes
     ----------
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/featurelist.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/imported_model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Optional, Tuple, Type, TypeVar
 
 import trafaret as t
 
 from datarobot._compat import Int, String
-from datarobot.models.feature_fit import FeatureFit
 from datarobot.models.shap_impact import ShapImpact
 from datarobot.models.validators import feature_impact_trafaret, single_feature_impact_trafaret
 from datarobot.utils.waiters import wait_for_async_resolution
 
 from .. import errors
 from ..client import get_client, staticproperty
 from ..enums import DEFAULT_MAX_WAIT, JOB_TYPE, PREDICTION_PREFIX, QUEUE_STATUS
@@ -143,15 +142,15 @@
     def get_result(self, params=None):
         """
         Parameters
         ----------
         params : dict or None
             Query parameters to be added to request to get results.
 
-        For featureEffects and featureFit, source param is required to define source,
+        For featureEffects, source param is required to define source,
         otherwise the default is `training`
 
         Returns
         -------
         result : object
             Return type depends on the job type:
                 - for model jobs, a Model is returned
@@ -161,15 +160,14 @@
                 - for primeRulesets jobs, a list of Rulesets
                 - for primeModel jobs, a PrimeModel
                 - for primeDownloadValidation jobs, a PrimeFile
                 - for predictionExplanationInitialization jobs, a
                   PredictionExplanationsInitialization
                 - for predictionExplanations jobs, a PredictionExplanations
                 - for featureEffects, a FeatureEffects
-                - for featureFit, a FeatureFit
 
         Raises
         ------
         JobNotFinished
             If the job is not finished, the result is not available.
         AsyncProcessUnsuccessfulError
             If the job errored or was aborted
@@ -188,16 +186,14 @@
         elif self.job_type == JOB_TYPE.PREDICT:
             return raw_prediction_response_to_dataframe(server_data, PREDICTION_PREFIX.DEFAULT)
         elif self.job_type == JOB_TYPE.FEATURE_IMPACT:
             # Note: a custom FeatureImpactJob class is used for high level API now.
             return server_data["featureImpacts"]
         elif self.job_type == JOB_TYPE.FEATURE_EFFECTS:
             return FeatureEffects.from_server_data(server_data)
-        elif self.job_type == JOB_TYPE.FEATURE_FIT:
-            return FeatureFit.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PRIME_RULESETS:
             return [Ruleset.from_server_data(ruleset_data) for ruleset_data in server_data]
         elif self.job_type == JOB_TYPE.PRIME_MODEL:
             return PrimeModel.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PRIME_VALIDATION:
             return PrimeFile.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PREDICTION_EXPLANATIONS_INITIALIZATION:
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/missing_report.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 from datarobot.models.external_dataset_scores_insights import ExternalScores
 from datarobot.models.feature_effect import (
     FeatureEffectMetadata,
     FeatureEffectMetadataDatetime,
     FeatureEffects,
     FeatureEffectsMulticlass,
 )
-from datarobot.models.feature_fit import FeatureFit, FeatureFitMetadata, FeatureFitMetadataDatetime
 from datarobot.models.lift_chart import LiftChart
 from datarobot.models.missing_report import MissingValuesReport
 from datarobot.models.pareto_front import ParetoFront
 from datarobot.models.residuals import ResidualsChart
 from datarobot.models.roc_curve import LabelwiseRocCurve, RocCurve
 from datarobot.models.ruleset import Ruleset
 from datarobot.models.segmentation import SegmentInfo
@@ -1186,16 +1185,16 @@
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_model_url() + "featureEffectsMetadata/"
 
     def get_feature_effect_metadata(self):
         """
         Retrieve Feature Effects metadata. Response contains status and available model sources.
 
-        * Feature Fit for the `training` partition is always available, with the exception of older
-          projects that only supported Feature Fit for `validation`.
+        * Feature Effect for the `training` partition is always available, with the exception of older
+          projects that only supported Feature Effect for `validation`.
 
         * When a model is trained into `validation` or `holdout` without stacked predictions
           (i.e., no out-of-sample predictions in those partitions),
           Feature Effects is not available for `validation` or `holdout`.
 
         * Feature Effects for `holdout` is not available when holdout was not unlocked for
           the project.
@@ -1207,44 +1206,14 @@
         feature_effect_metadata: FeatureEffectMetadata
 
         """
         fe_metadata_url = self._get_feature_effect_metadata_url()
         server_data = self._client.get(fe_metadata_url).json()
         return FeatureEffectMetadata.from_server_data(server_data)
 
-    def _get_feature_fit_metadata_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_model_url() + "featureFitMetadata/"
-
-    def get_feature_fit_metadata(self):
-        """
-         Retrieve Feature Fit metadata. Response contains status and available model sources.
-
-        * Feature Fit of `training` is always available
-          (except for the old project which supports only Feature Fit for `validation`).
-
-        * When a model is trained into `validation` or `holdout` without stacked prediction
-          (e.g. no out-of-sample prediction in `validation` or `holdout`),
-          Feature Fit is not available for `validation` or `holdout`.
-
-        * Feature Fit for `holdout` is not available when there is no holdout configured for
-          the project.
-
-         `source` is expected parameter to retrieve Feature Fit. One of provided sources
-         shall be used.
-
-         Returns
-         -------
-         feature_effect_metadata: FeatureFitMetadata
-
-        """
-        ff_metadata_url = self._get_feature_fit_metadata_url()
-        server_data = self._client.get(ff_metadata_url).json()
-        return FeatureFitMetadata.from_server_data(server_data)
-
     def _get_feature_effect_url(self) -> str:
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_model_url() + "featureEffects/"
 
     def request_feature_effect(self, row_count: Optional[int] = None):
         """
         Request feature effects to be computed for the model.
@@ -1481,117 +1450,14 @@
             from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
 
             feature_effect_job = Job.get(self.project_id, qid)
 
         params = {"source": source}
         return feature_effect_job.get_result_when_complete(max_wait=max_wait, params=params)
 
-    def _get_feature_fit_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_model_url() + "featureFit/"
-
-    def request_feature_fit(self):
-        """
-        Request feature fit to be computed for the model.
-
-        See :meth:`get_feature_effect <datarobot.models.Model.get_feature_fit>` for more
-        information on the result of the job.
-
-        Returns
-        -------
-         job : Job
-            A Job representing the feature fit computation. To get the completed feature fit
-            data, use `job.get_result` or `job.get_result_when_complete`.
-
-        Raises
-        ------
-        JobAlreadyRequested (422)
-            If the feature effect have already been requested.
-        """
-        from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
-
-        route = self._get_feature_fit_url()
-        response = self._client.post(route)
-        job_id = get_id_from_response(response)
-        return Job.get(self.project_id, job_id)
-
-    def get_feature_fit(self, source: str):
-        """
-        Retrieve Feature Fit for the model.
-
-        Feature Fit provides partial dependence and predicted vs actual values for top-500
-        features ordered by feature importance score.
-
-        The partial dependence shows marginal effect of a feature on the target variable after
-        accounting for the average effects of all other predictive features. It indicates how,
-        holding all other variables except the feature of interest as they were,
-        the value of this feature affects your prediction.
-
-        Requires that Feature Fit has already been computed with
-        :meth:`request_feature_effect <datarobot.models.Model.request_feature_fit>`.
-
-        See :meth:`get_feature_fit_metadata <datarobot.models.Model.get_feature_fit_metadata>`
-        for retrieving information the available sources.
-
-        Parameters
-        ----------
-        source : string
-            The source Feature Fit are retrieved for.
-            One value of [FeatureFitMetadata.sources].
-
-        Returns
-        -------
-        feature_fit : FeatureFit
-           The feature fit data.
-
-        Raises
-        ------
-        ClientError (404)
-            If the feature fit have not been computed or source is not valid value.
-        """
-        params = {"source": source}
-        fe_url = self._get_feature_fit_url()
-        server_data = self._client.get(fe_url, params=params).json()
-        return FeatureFit.from_server_data(server_data)
-
-    def get_or_request_feature_fit(self, source: str, max_wait: int = DEFAULT_MAX_WAIT):
-        """
-        Retrieve feature fit for the model, requesting a job if it hasn't been run previously
-
-        See :meth:`get_feature_fit_metadata \
-        <datarobot.models.Model.get_feature_fit_metadata>`
-        for retrieving information of source.
-
-        Parameters
-        ----------
-        max_wait : int, optional
-            The maximum time to wait for a requested feature fit job to complete before erroring
-
-        source : string
-            The source Feature Fit are retrieved for.
-            One value of [FeatureFitMetadata.sources].
-
-        Returns
-        -------
-        feature_effects : FeatureFit
-           The feature fit data.
-        """
-        try:
-            feature_fit_job = self.request_feature_fit()
-        except JobAlreadyRequested as e:
-            # if already requested it may be still running
-            # check and get the jobid in that case
-            qid = e.json["jobId"]
-            from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
-
-            feature_fit_job = Job.get(self.project_id, qid)
-
-        params = {"source": source}
-        return feature_fit_job.get_result_when_complete(max_wait=max_wait, params=params)
-
     def get_prime_eligibility(self):
         """Check if this model can be approximated with DataRobot Prime
 
         Returns
         -------
         prime_eligibility : dict
             a dict indicating whether a model can be approximated with DataRobot Prime
@@ -4330,55 +4196,14 @@
         feature_effect_metadata: FeatureEffectMetadataDatetime
 
         """
         fe_metadata_url = self._get_feature_effect_metadata_url()
         server_data = self._client.get(fe_metadata_url).json()
         return FeatureEffectMetadataDatetime.from_server_data(server_data)
 
-    def _get_feature_fit_metadata_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_datetime_model_url() + "featureFitMetadata/"
-
-    def get_feature_fit_metadata(self):
-        """
-        Retrieve Feature Fit metadata for each backtest. Response contains status and available
-        sources for each backtest of the model.
-
-        * Each backtest is available for `training` and `validation`
-
-        * If holdout is configured for the project it has `holdout` as `backtestIndex`. It has
-          `training` and `holdout` sources available.
-
-        Start/stop models contain a single response item with `startstop` value for `backtestIndex`.
-
-        * Feature Fit of `training` is always available
-          (except for the old project which supports only Feature Effect for `validation`).
-
-        * When a model is trained into `validation` or `holdout` without stacked prediction
-          (e.g. no out-of-sample prediction in `validation` or `holdout`),
-          Feature Fit is not available for `validation` or `holdout`.
-
-        * Feature Fit for `holdout` is not available when there is no holdout configured for
-          the project.
-
-        `source` is expected parameter to retrieve Feature Fit. One of provided sources
-        shall be used.
-
-        `backtestIndex` is expected parameter to submit compute request and retrieve Feature Fit.
-        One of provided backtest indexes shall be used.
-
-        Returns
-        -------
-        feature_effect_metadata: FeatureFitMetadataDatetime
-
-        """
-        ff_metadata_url = self._get_feature_fit_metadata_url()
-        server_data = self._client.get(ff_metadata_url).json()
-        return FeatureFitMetadataDatetime.from_server_data(server_data)
-
     def _get_feature_effect_url(self) -> str:
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_datetime_model_url() + "featureEffects/"
 
     # pylint: disable-next=arguments-renamed
     def request_feature_effect(self, backtest_index):
         """
@@ -4644,142 +4469,14 @@
                     max_wait=max_wait, params=params
                 )
             else:
                 raise e
 
         return feature_effects
 
-    def _get_feature_fit_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_datetime_model_url() + "featureFit/"
-
-    # pylint: disable-next=arguments-differ
-    def request_feature_fit(self, backtest_index):
-        """
-        Request feature fit to be computed for the model.
-
-        See :meth:`get_feature_fit <datarobot.models.DatetimeModel.get_feature_fit>` for more
-        information on the result of the job.
-
-        See :meth:`get_feature_fit_metadata \
-        <datarobot.models.DatetimeModel.get_feature_fit_metadata>`
-        for retrieving information of backtest_index.
-
-        Parameters
-        ----------
-        backtest_index: string, FeatureFitMetadataDatetime.backtest_index.
-            The backtest index to retrieve Feature Fit for.
-
-        Returns
-        -------
-         job : Job
-            A Job representing the feature fit computation. To get the completed feature fit
-            data, use `job.get_result` or `job.get_result_when_complete`.
-
-        Raises
-        ------
-        JobAlreadyRequested (422)
-            If the feature fit have already been requested.
-        """
-        from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
-
-        payload = {"backtestIndex": backtest_index}
-        route = self._get_feature_fit_url()
-        response = self._client.post(route, data=payload)
-        job_id = get_id_from_response(response)
-        return Job.get(self.project_id, job_id)
-
-    # pylint: disable-next=arguments-differ
-    def get_feature_fit(self, source, backtest_index):
-        """
-        Retrieve Feature Fit for the model.
-
-        Feature Fit provides partial dependence and predicted vs actual values for top-500
-        features ordered by feature impact score.
-
-        The partial dependence shows marginal effect of a feature on the target variable after
-        accounting for the average effects of all other predictive features. It indicates how,
-        holding all other variables except the feature of interest as they were,
-        the value of this feature affects your prediction.
-
-        Requires that Feature Fit has already been computed with
-        :meth:`request_feature_fit <datarobot.models.Model.request_feature_fit>`.
-
-        See :meth:`get_feature_fit_metadata \
-        <datarobot.models.DatetimeModel.get_feature_fit_metadata>`
-        for retrieving information of source, backtest_index.
-
-        Parameters
-        ----------
-        source: string
-            The source Feature Fit are retrieved for.
-            One value of [FeatureFitMetadataDatetime.sources]. To retrieve the available
-            sources for feature fit.
-
-        backtest_index: string, FeatureFitMetadataDatetime.backtest_index.
-            The backtest index to retrieve Feature Fit for.
-
-        Returns
-        -------
-        feature_fit: FeatureFit
-           The feature fit data.
-
-        Raises
-        ------
-        ClientError (404)
-            If the feature fit have not been computed or source is not valid value.
-        """
-        params = {
-            "source": source,
-            "backtestIndex": backtest_index,
-        }
-        fe_url = self._get_feature_fit_url()
-        server_data = self._client.get(fe_url, params=params).json()
-        return FeatureFit.from_server_data(server_data)
-
-    # pylint: disable-next=arguments-renamed
-    def get_or_request_feature_fit(self, source, backtest_index, max_wait=DEFAULT_MAX_WAIT):
-        """
-        Retrieve feature fit for the model, requesting a job if it hasn't been run previously
-
-        See :meth:`get_feature_fit_metadata \
-        <datarobot.models.DatetimeModel.get_feature_fit_metadata>`
-        for retrieving information of source, backtest_index.
-
-        Parameters
-        ----------
-        max_wait : int, optional
-            The maximum time to wait for a requested feature fit job to complete before erroring
-
-        source : string
-            The source Feature Fit are retrieved for.
-            One value of [FeatureFitMetadataDatetime.sources]. To retrieve the available sources
-            for feature effect.
-
-        backtest_index: string, FeatureFitMetadataDatetime.backtest_index.
-            The backtest index to retrieve Feature Fit for.
-
-        Returns
-        -------
-        feature_fit : FeatureFit
-           The feature fit data.
-        """
-        try:
-            feature_fit_job = self.request_feature_fit(backtest_index)
-        except JobAlreadyRequested as e:
-            # if already requested it may be still running
-            # check and get the jobid in that case
-            qid = e.json["jobId"]
-            from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
-
-            feature_fit_job = Job.get(self.project_id, qid)
-
-        params = {"source": source}
-        return feature_fit_job.get_result_when_complete(max_wait=max_wait, params=params)
-
     def calculate_prediction_intervals(self, prediction_intervals_size: int) -> Job:
         """
         Calculate prediction intervals for this DatetimeModel for the specified size.
 
         .. versionadded:: v2.19
 
         Parameters
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/modeljob.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/notebooks.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/notebooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from typing import Any, Dict, List, Optional
 
 import trafaret as t
 
 from datarobot.enums import NotebookPermissions
 from datarobot.models.api_object import APIObject
+from datarobot.models.use_cases.utils import resolve_use_case
 from datarobot.utils.pagination import unpaginate
 
 notebook_user_trafaret = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("username"): t.String,
         t.Key("first_name"): t.String,
@@ -297,12 +298,14 @@
         params = {
             "created_before": created_before,
             "created_after": created_after,
             "order_by": order_by,
             "tags": tags,
             "owners": owners,
             "query": query,
-            "use_case_id": use_case_id,
         }
+        params = resolve_use_case(
+            use_case_id=use_case_id, params=params, use_case_key="use_case_id"
+        )
         url = f"{cls._client.domain}/{cls._path}"
         r_data = unpaginate(url, params, cls._client)
         return [Notebook.from_server_data(data) for data in r_data]
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/pareto_front.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/predict_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_server.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/predictions.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prime_file.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/project.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 from datarobot.models.relationships_configuration import RelationshipsConfiguration
 from datarobot.models.restore_discarded_features import (
     DiscardedFeaturesInfo,
     FeatureRestorationStatus,
 )
 from datarobot.models.segmentation import SegmentationTask
 from datarobot.models.sharing import SharingAccess
+from datarobot.models.use_cases.utils import resolve_use_case
 from datarobot.utils import (
     assert_single_or_zero_parameter,
     camelize,
     datetime_to_string,
     deprecated,
     from_api,
     get_duplicate_features,
@@ -1220,15 +1221,17 @@
             relationships_configuration_id=relationships_configuration_id,
             unsupervised_type=unsupervised_type,
             autopilot_cluster_list=autopilot_cluster_list,
         )
         return project
 
     @classmethod
-    def list(cls, search_params: Optional[Dict[str, str]] = None) -> List[Project]:
+    def list(
+        cls, search_params: Optional[Dict[str, str]] = None, use_case_id: Optional[str] = None
+    ) -> List[Project]:
         """
         Returns the projects associated with this account.
 
         Parameters
         ----------
         search_params : dict, optional.
             If not `None`, the returned projects are filtered by lookup.
@@ -1270,14 +1273,18 @@
                 get_params.update(search_params)
             else:
                 raise TypeError(
                     "Provided search_params argument {} is invalid type {}".format(
                         search_params, type(search_params)
                     )
                 )
+        # This is a special case we needed to cover. A user could pass in "experiment_container_id" themselves to
+        # `search_params`, so we need to check for that and default to `use_case_id` if that was passed in.
+        # Then we proceed to check if `use_case_id` was set, and use a global use case if it's available.
+        get_params = resolve_use_case(use_case_id=use_case_id, params=get_params)
         r_data = cls._client.get(cls._path, params=get_params).json()
         return [cls.from_server_data(item) for item in r_data]
 
     def _update(self, **data) -> Project:
         """
         Change the project properties.
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/project_options.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/rating_table.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/recommended_model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/residuals.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/roc_curve.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/ruleset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/segmentation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_impact.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/sharing.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/trafarets.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/training_predictions.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/types.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/use_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from __future__ import annotations
 
 from types import TracebackType
 from typing import cast, Dict, List, Optional, Tuple, Type, Union
 
 import trafaret as t
 
-from datarobot.context import _context
+from datarobot.context import Context
 from datarobot.enums import SHARING_ROLE, UseCaseEntities
 from datarobot.errors import InvalidUsageError
 from datarobot.models.api_object import APIObject
 from datarobot.models.application import Application
 from datarobot.models.dataset import Dataset
 from datarobot.models.notebooks import Notebook
 from datarobot.models.project import Project
@@ -332,26 +332,26 @@
         cls._client.delete(path)
         return None
 
     def __enter__(self) -> UseCase:
         # Not declared in __init__ because this attribute has a very
         # specific use in context management and nowhere else
         self.__previous: UseCase = cast(  # pylint: disable=attribute-defined-outside-init
-            UseCase, _context.get().use_case
+            UseCase, Context.use_case
         )
-        _context.get().use_case = self
+        Context.use_case = self
         return self
 
     def __exit__(
         self,
         __exc_type: Type[BaseException] | None,
         __exc_value: BaseException | None,
         __traceback: TracebackType | None,
     ) -> bool | None:
-        _context.get().use_case = self.__previous
+        Context.use_case = self.__previous
         return None
 
     def update(self, name: Optional[str] = None, description: Optional[str] = None) -> UseCase:
         """
         Update a Use Case's name or description.
 
         Parameters
@@ -426,15 +426,15 @@
         use_case_reference_entity : UseCaseReferenceEntity
             The newly created reference link between this Use Case and the entity.
         """
         e_type = entity_type
         e_id = entity_id
         if entity and (e_type or entity_id):
             raise InvalidUsageError(
-                "Can only except either an entity, or an entity type and entity id."
+                "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not e_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
         if entity:
             e_type, e_id = self._get_reference_entity_info(entity)
         path = f"{self._path}{self.id}/{e_type}/{e_id}/"
         r_data = self._client.post(path)
@@ -461,15 +461,15 @@
         entity_id : str
             The ID of the entity to link to this Use Case.  Can not be used if entity is passed.
         """
         e_type = entity_type
         e_id = entity_id
         if entity and (entity_type or entity_id):
             raise InvalidUsageError(
-                "Can only except either an entity, or an entity type and entity id."
+                "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not entity_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
         if entity:
             e_type, e_id = self._get_reference_entity_info(entity)
         path = f"{self._path}{self.id}/{e_type}/{e_id}/"
         self._client.delete(path)
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/validators.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/images.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/word_cloud.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/rest.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import trafaret as t
 from urllib3 import Retry
 
 from datarobot.mixins.browser_mixin import BrowserMixin
 
 from ._compat import Int, String
 from ._version import __version__
-from .context import _context
+from .context import Context
 from .enums import DEFAULT_TIMEOUT
 from .errors import ClientError, JobAlreadyRequested, PlatformDeprecationWarning, ServerError
 from .utils import to_api
 
 if TYPE_CHECKING:
     from io import BufferedReader, IOBase
 
@@ -434,13 +434,13 @@
         self.ssl_verify = ssl_verify
         self.user_agent_suffix = user_agent_suffix
         self.max_retries = max_retries
         self.token_type = token_type
         self.use_case = use_case
 
         if self.use_case is not None:
-            _context.get().use_case = self.use_case
+            Context.use_case = self.use_case
 
     @classmethod
     def from_data(cls, data: Dict[str, Any]) -> DataRobotClientConfig:
         checked = {k: v for k, v in cls._converter.check(data).items() if k in cls._fields}
         return cls(**checked)
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/deprecation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/pagination.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/retry.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/source.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/waiters.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.2.0.2023.5.1
+Version: 3.2.0.2023.5.8
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 datarobot/models/datetime_trend_plots.py
 datarobot/models/driver.py
 datarobot/models/execution_environment.py
 datarobot/models/execution_environment_version.py
 datarobot/models/external_baseline_validation.py
 datarobot/models/feature.py
 datarobot/models/feature_effect.py
-datarobot/models/feature_fit.py
 datarobot/models/featurelist.py
 datarobot/models/imported_model.py
 datarobot/models/job.py
 datarobot/models/lift_chart.py
 datarobot/models/missing_report.py
 datarobot/models/model.py
 datarobot/models/modeljob.py
@@ -108,14 +107,15 @@
 datarobot/models/trafarets.py
 datarobot/models/training_predictions.py
 datarobot/models/types.py
 datarobot/models/validators.py
 datarobot/models/word_cloud.py
 datarobot/models/deployment/__init__.py
 datarobot/models/deployment/accuracy.py
+datarobot/models/deployment/bias_and_fairness.py
 datarobot/models/deployment/data_drift.py
 datarobot/models/deployment/deployment.py
 datarobot/models/deployment/service_stats.py
 datarobot/models/deployment/sharing.py
 datarobot/models/external_dataset_scores_insights/__init__.py
 datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
 datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
@@ -125,14 +125,15 @@
 datarobot/models/external_dataset_scores_insights/external_scores.py
 datarobot/models/feature_association_matrix/__init__.py
 datarobot/models/feature_association_matrix/feature_association_featurelists.py
 datarobot/models/feature_association_matrix/feature_association_matrix.py
 datarobot/models/feature_association_matrix/feature_association_matrix_details.py
 datarobot/models/use_cases/__init__.py
 datarobot/models/use_cases/use_case.py
+datarobot/models/use_cases/utils.py
 datarobot/models/user_blueprints/__init__.py
 datarobot/models/user_blueprints/models.py
 datarobot/models/user_blueprints/trafarets.py
 datarobot/models/visualai/__init__.py
 datarobot/models/visualai/augmentation.py
 datarobot/models/visualai/images.py
 datarobot/models/visualai/insights.py
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/pyproject.toml` & `datarobot_early_access-3.2.0.2023.5.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     "datarobot.models.custom_task_version",
     "datarobot.models.data_engine_query_generator",
     "datarobot.models.datetime_trend_plots",
     "datarobot.models.execution_environment",
     "datarobot.models.execution_environment_version",
     "datarobot.models.feature",
     "datarobot.models.feature_effect",
-    "datarobot.models.feature_fit",
     "datarobot.models.job",
     "datarobot.models.lift_chart",
     "datarobot.models.model",
     "datarobot.models.modeljob",
     "datarobot.models.pairwise_statistics",
     "datarobot.models.pareto_front",
     "datarobot.models.predict_job",
```

### Comparing `datarobot_early_access-3.2.0.2023.5.1/setup.py` & `datarobot_early_access-3.2.0.2023.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.1/setup_weekly.py` & `datarobot_early_access-3.2.0.2023.5.8/setup_weekly.py`

 * *Files identical despite different names*

