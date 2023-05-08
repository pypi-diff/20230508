# Comparing `tmp/autogluon.cloud-0.2.1b20230506.tar.gz` & `tmp/autogluon.cloud-0.2.1b20230507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autogluon.cloud-0.2.1b20230506.tar", last modified: Sat May  6 09:04:36 2023, max compression
+gzip compressed data, was "dist/autogluon.cloud-0.2.1b20230507.tar", last modified: Sun May  7 09:04:24 2023, max compression
```

## Comparing `autogluon.cloud-0.2.1b20230506.tar` & `autogluon.cloud-0.2.1b20230507.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/ray_aws_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    58093 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/tabular_sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/cluster_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/cluster_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/ray_cluster_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/ray_cluster_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/data/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/data/format_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/endpoint/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/endpoint/sagemaker_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/job/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/job/ray_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/job/remote_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/job/sagemaker_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35615 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/cloud_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/tabular_cloud_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/scripts/script_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/ag_sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/aws_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/deserializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/dlc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/ray_aws_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/sagemaker_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-06 09:04:24.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:04:36.000000 autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/ray_aws_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58093 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/tabular_sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/cluster_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/cluster_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/ray_cluster_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/ray_cluster_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/data/format_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/endpoint/sagemaker_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/job/ray_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/job/remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/job/sagemaker_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35615 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/cloud_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/tabular_cloud_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/scripts/script_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/ag_sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/aws_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/deserializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/dlc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/ray_aws_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/sagemaker_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-07 09:04:11.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-07 09:04:23.000000 autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-07 09:04:23.000000 autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-07 09:04:24.000000 autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:04:23.000000 autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 09:04:23.000000 autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-07 09:04:23.000000 autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 09:04:23.000000 autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:04:23.000000 autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/zip-safe
```

### Comparing `autogluon.cloud-0.2.1b20230506/LICENSE` & `autogluon.cloud-0.2.1b20230507/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/PKG-INFO` & `autogluon.cloud-0.2.1b20230507/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.cloud
-Version: 0.2.1b20230506
+Version: 0.2.1b20230507
 Summary: Train and deploy AutoGluon backed models on the cloud
 Home-page: https://github.com/autogluon/autogluon-cloud
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-cloud/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-cloud/
```

### Comparing `autogluon.cloud-0.2.1b20230506/README.md` & `autogluon.cloud-0.2.1b20230507/README.md`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/setup.cfg` & `autogluon.cloud-0.2.1b20230507/setup.cfg`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/setup.py` & `autogluon.cloud-0.2.1b20230507/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/backend.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/backend_factory.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/backend_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/ray_aws_backend.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/ray_aws_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/ray_backend.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/ray_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/sagemaker_backend.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/tabular_sagemaker_backend.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/tabular_sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/cluster_config_generator.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/cluster_config_generator.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/cluster_manager.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/constants.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/cluster/ray_cluster_manager.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/cluster/ray_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/data/format_converter.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/data/format_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/endpoint/endpoint.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/endpoint/sagemaker_endpoint.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/endpoint/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/job/ray_job.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/job/ray_job.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/job/remote_job.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/job/remote_job.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/job/sagemaker_job.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/job/sagemaker_job.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/cloud_predictor.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/tabular_cloud_predictor.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/tabular_cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/scripts/script_manager.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/scripts/script_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/ag_sagemaker.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/ag_sagemaker.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/aws_utils.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/deserializers.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/deserializers.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/dlc_utils.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/dlc_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/ec2.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/ec2.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/iam.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/iam.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/ray_aws_iam.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/ray_aws_iam.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/s3_utils.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/sagemaker_iam.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/sagemaker_iam.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/serializers.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon/cloud/utils/utils.py` & `autogluon.cloud-0.2.1b20230507/src/autogluon/cloud/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/PKG-INFO` & `autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.cloud
-Version: 0.2.1b20230506
+Version: 0.2.1b20230507
 Summary: Train and deploy AutoGluon backed models on the cloud
 Home-page: https://github.com/autogluon/autogluon-cloud
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-cloud/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-cloud/
```

### Comparing `autogluon.cloud-0.2.1b20230506/src/autogluon.cloud.egg-info/SOURCES.txt` & `autogluon.cloud-0.2.1b20230507/src/autogluon.cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

