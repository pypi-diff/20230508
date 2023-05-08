# Comparing `tmp/domino-py-0.1.8.tar.gz` & `tmp/domino-py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.1.8.tar", last modified: Fri Apr 28 14:22:35 2023, max compression
+gzip compressed data, was "domino-py-0.1.9.tar", last modified: Fri Apr 28 19:15:19 2023, max compression
```

## Comparing `domino-py-0.1.8.tar` & `domino-py-0.1.9.tar`

### file list

```diff
@@ -1,104 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.403661 domino-py-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 14:22:19.000000 domino-py-0.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 14:22:19.000000 domino-py-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 14:22:35.403661 domino-py-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-28 14:22:19.000000 domino-py-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.391661 domino-py-0.1.8/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.391661 domino-py-0.1.8/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.391661 domino-py-0.1.8/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/cli/utils/config-domino-local.toml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/cli/utils/create_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    22570 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.391661 domino-py-0.1.8/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.391661 domino-py-0.1.8/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/bash_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.395661 domino-py-0.1.8/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/sidecar/fuse.conf
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/sidecar/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/sidecar/rclone.conf
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/custom_operators/sidecar/sidecar_lifecycle.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.395661 domino-py-0.1.8/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.395661 domino-py-0.1.8/domino/helm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.395661 domino-py-0.1.8/domino/helm/domino-airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-airflow/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.395661 domino-py-0.1.8/domino/helm/domino-airflow/charts/
--rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-airflow/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.395661 domino-py-0.1.8/domino/helm/domino-base/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/Chart.lock
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.395661 domino-py-0.1.8/domino/helm/domino-base/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/templates/domino-backend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/templates/domino-frontend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/templates/domino-postgres-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/templates/ingress-api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/templates/ingress-frontend.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.395661 domino-py-0.1.8/domino/helm/domino-base/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/templates/jobs/domino-migrations.yml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/templates/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.395661 domino-py-0.1.8/domino/helm/domino-base/templates/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/templates/volumes/domino-rest-volume-claim-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/templates/volumes/domino-rest-volume-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/helm/domino-base/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/piece_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.399661 domino-py-0.1.8/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.399661 domino-py-0.1.8/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/generate_infrasctructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/run_piece_dry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.399661 domino-py-0.1.8/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/utils/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/utils/enum_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/utils/types_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 14:22:19.000000 domino-py-0.1.8/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:22:35.403661 domino-py-0.1.8/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 14:22:34.000000 domino-py-0.1.8/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-28 14:22:35.000000 domino-py-0.1.8/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:22:34.000000 domino-py-0.1.8/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 14:22:34.000000 domino-py-0.1.8/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 14:22:34.000000 domino-py-0.1.8/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 14:22:34.000000 domino-py-0.1.8/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-28 14:22:19.000000 domino-py-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 14:22:35.403661 domino-py-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-28 14:22:19.000000 domino-py-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.462423 domino-py-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 19:15:06.000000 domino-py-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-28 19:15:06.000000 domino-py-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 19:15:19.462423 domino-py-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-28 19:15:06.000000 domino-py-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/config-domino-local.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/bash_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/fuse.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/rclone.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/sidecar_lifecycle.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/helm/domino-airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-airflow/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-airflow/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-airflow/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-base/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/Chart.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-base/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/domino-backend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/domino-frontend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/domino-postgres-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/ingress-api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/ingress-frontend.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-base/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/jobs/domino-migrations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-base/templates/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/volumes/domino-rest-volume-claim-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/volumes/domino-rest-volume-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/piece_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/generate_infrasctructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/run_piece_dry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/run_piece_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.462423 domino-py-0.1.9/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/enum_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/types_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.462423 domino-py-0.1.9/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-28 19:15:06.000000 domino-py-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:15:19.462423 domino-py-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-28 19:15:06.000000 domino-py-0.1.9/setup.py
```

### Comparing `domino-py-0.1.8/LICENSE.md` & `domino-py-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/MANIFEST.in` & `domino-py-0.1.9/MANIFEST.in`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 include requirements.txt
 include domino/cli/utils/config-domino-local.toml
-include domino/cli/utils/create_cluster.sh
 include domino/helm/domino-airflow/kind-cluster-config
 include domino/helm/domino-airflow/**
 include domino/helm/domino-airflow/charts/**
 include domino/helm/domino-base/**
 include domino/helm/domino-base/templates/**
 include domino/helm/domino-base/templates/jobs/**
 include domino/helm/domino-base/templates/volumes/**
```

### Comparing `domino-py-0.1.8/PKG-INFO` & `domino-py-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Domino project
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description:
```

### Comparing `domino-py-0.1.8/README.md` & `domino-py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/base_piece.py` & `domino-py-0.1.9/domino/base_piece.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             self.airflow_context['ti'].xcom_push(key=self.task_id, value=xcom_obj)
         elif self.deploy_mode == "local-bash":
             # For our extended BashOperator, return XCom must be stored in /opt/mnt/fs/tmp/xcom_output.json
             file_path = Path("/opt/mnt/fs/tmp/xcom_output.json")
             file_path.parent.mkdir(parents=True, exist_ok=True)
             with open(str(file_path), 'w') as fp:
                 json.dump(xcom_obj, fp, indent=4)
-        elif self.deploy_mode == "k8s":
+        elif self.deploy_mode in ["k8s", "local-k8s", "local-k8s-dev"]:
             # In Kubernetes, return XCom must be stored in /airflow/xcom/return.json
             # https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/stable/pieces.html#how-does-xcom-work
             file_path = Path('/airflow/xcom/return.json')
             file_path.parent.mkdir(parents=True, exist_ok=True)
             with open(str(file_path), 'w') as fp:
                 json.dump(xcom_obj, fp)
```

### Comparing `domino-py-0.1.8/domino/cli/cli.py` & `domino-py-0.1.9/domino/cli/cli.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/cli/utils/pieces_repository.py` & `domino-py-0.1.9/domino/cli/utils/pieces_repository.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/cli/utils/platform.py` & `domino-py-0.1.9/domino/cli/utils/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
     
     running_path = str(Path().cwd().resolve())
     config_dict["path"]["DOMINO_LOCAL_RUNNING_PATH"] = running_path
     config_dict["kind"]["DOMINO_KIND_CLUSTER_NAME"] = cluster_name
     config_dict['kind']['DOMINO_DEPLOY_MODE'] = deploy_mode
 
     config_dict['local_pieces_repositories'] = {}
-    config_dict['local_domino_repository'] = {"DOMINO_LOCAL_DOMINO_REPOSITORY": ""}
+    config_dict['local_domino_package'] = {"DOMINO_LOCAL_DOMINO_PACKAGE": ""}
     if deploy_mode == 'local-k8s-dev':
-        config_dict['local_domino_repository']['DOMINO_LOCAL_DOMINO_REPOSITORY'] = local_domino_path
+        config_dict['local_domino_package']['DOMINO_LOCAL_DOMINO_PACKAGE'] = local_domino_path
         for local_pieces_repository in local_pieces_repository_path:
             # Read repo config.toml to get repo name to map it to cluster path
             repo_config_file_path = Path(local_pieces_repository).resolve() / "config.toml"
             with open(str(repo_config_file_path), "rb") as f:
                 repo_toml = tomli.load(f)
             
             repo_name = repo_toml['repository']['REPOSITORY_NAME'] 
@@ -126,18 +126,18 @@
                 dict(
                     hostPath=repo_path,
                     containerPath=f"/pieces_repositories/{repo_name}",
                     readOnly=True,
                     propagation='HostToContainer'
                 )
             )
-        if platform_config['local_domino_repository'].get('DOMINO_LOCAL_DOMINO_REPOSITORY'):
+        if platform_config['local_domino_package'].get('DOMINO_LOCAL_DOMINO_PACKAGE'):
             extra_mounts_local_repositories.append(
                 dict(
-                    hostPath=platform_config['local_domino_repository']['DOMINO_LOCAL_DOMINO_REPOSITORY'],
+                    hostPath=platform_config['local_domino_package']['DOMINO_LOCAL_DOMINO_PACKAGE'],
                     containerPath=f"/domino/domino_py",
                     readOnly=True,
                     propagation='HostToContainer'
                 )
             )
 
     kubeadm_parsed = AsLiteral(yaml.dump(kubeadm_config_patches))
@@ -268,15 +268,15 @@
     )
     airflow_ssh_config_parsed = AsLiteral(yaml.dump(airflow_ssh_config))
 
     workers_extra_volumes = []
     workers_extra_volumes_mounts = []
     workers = {}
     scheduler = {}
-    if platform_config['kind']["DOMINO_DEPLOY_MODE"] == 'local-k8s-dev' and platform_config['local_domino_repository'].get('DOMINO_LOCAL_DOMINO_REPOSITORY'):
+    if platform_config['kind']["DOMINO_DEPLOY_MODE"] == 'local-k8s-dev' and platform_config['local_domino_package'].get('DOMINO_LOCAL_DOMINO_PACKAGE'):
         workers_extra_volumes = [
             {
                 "name": "domino-dev-extra",
                 "persistentVolumeClaim": {
                     "claimName": "domino-dev-volume-claim"
                 }
             }
@@ -296,14 +296,16 @@
         scheduler = {
             "scheduler": {
                 "extraVolumes": workers_extra_volumes,
                 "extraVolumeMounts": workers_extra_volumes_mounts,
             }
         }
 
+    
+
     airflow_values_override_config = {
         "airflow": {
             "enabled": True,
             "env": [
                 {
                     "name": "DOMINO_DEPLOY_MODE",
                     "value": platform_config['kind']["DOMINO_DEPLOY_MODE"]
@@ -464,15 +466,15 @@
                                 ]
                             )
                         )
                     )
                 )
                 k8s_client.create_persistent_volume(body=pv)
         
-        if platform_config['local_domino_repository'].get('DOMINO_LOCAL_DOMINO_REPOSITORY'):
+        if platform_config['local_domino_package'].get('DOMINO_LOCAL_DOMINO_PACKAGE'):
             console.print("Creating PV's and PVC's for Local Domino Package...")
             # Create pv and pvc for local dev domino
             pvc = client.V1PersistentVolumeClaim(
                 metadata=client.V1ObjectMeta(name="domino-dev-volume-claim"),
                 spec=client.V1PersistentVolumeClaimSpec(
                     access_modes=["ReadWriteMany"],
                     volume_name="domino-dev-volume",
```

### Comparing `domino-py-0.1.8/domino/client/airflow_client.py` & `domino-py-0.1.9/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/client/domino_backend_client.py` & `domino-py-0.1.9/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/client/fs_client.py` & `domino-py-0.1.9/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/client/github_rest_client.py` & `domino-py-0.1.9/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/client/local_files_client.py` & `domino-py-0.1.9/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/client/s3_client.py` & `domino-py-0.1.9/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/custom_operators/bash_operator.py` & `domino-py-0.1.9/domino/custom_operators/bash_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/custom_operators/k8s_operator.py` & `domino-py-0.1.9/domino/custom_operators/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/custom_operators/python_operator.py` & `domino-py-0.1.9/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/custom_operators/sidecar/logger.py` & `domino-py-0.1.9/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/custom_operators/sidecar/mount.py` & `domino-py-0.1.9/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/exceptions/exceptions.py` & `domino-py-0.1.9/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz` & `domino-py-0.1.9/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/helm/domino-airflow/values.yaml` & `domino-py-0.1.9/domino/helm/domino-airflow/values.yaml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/helm/domino-base/templates/domino-backend-deployment.yml` & `domino-py-0.1.9/domino/helm/domino-base/templates/domino-backend-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/helm/domino-base/templates/domino-frontend-deployment.yml` & `domino-py-0.1.9/domino/helm/domino-base/templates/domino-frontend-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/helm/domino-base/templates/domino-postgres-deployment.yml` & `domino-py-0.1.9/domino/helm/domino-base/templates/domino-postgres-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/helm/domino-base/templates/jobs/domino-migrations.yml` & `domino-py-0.1.9/domino/helm/domino-base/templates/jobs/domino-migrations.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/logger.py` & `domino-py-0.1.9/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/schemas/piece_metadata.py` & `domino-py-0.1.9/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/schemas/shared_storage.py` & `domino-py-0.1.9/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/scripts/build_docker_images_pieces.py` & `domino-py-0.1.9/domino/scripts/build_docker_images_pieces.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/scripts/create_docker_compose_file.py` & `domino-py-0.1.9/domino/scripts/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/scripts/docker_compose_constants.py` & `domino-py-0.1.9/domino/scripts/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/scripts/docker_compose_scripts.py` & `domino-py-0.1.9/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/scripts/generate_infrasctructure.py` & `domino-py-0.1.9/domino/scripts/generate_infrasctructure.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/scripts/load_piece.py` & `domino-py-0.1.9/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/scripts/run_piece_bash.py` & `domino-py-0.1.9/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/scripts/run_piece_dry.py` & `domino-py-0.1.9/domino/scripts/run_piece_dry.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/scripts/run_piece_k8s.py` & `domino-py-0.1.9/domino/scripts/run_piece_k8s.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino/task.py` & `domino-py-0.1.9/domino/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self, 
         dag: DAG, 
         task_id: str,
         piece: dict,
         piece_input_kwargs: dict,
         workflow_shared_storage: dict = None,
         container_resources: dict = None,
-        deploy_mode: str = 'local-k8s-dev',
+        **kwargs
     ) -> None:
         # Task configuration and attributes
         self.task_id = task_id
         self.logger = get_configured_logger(f"{self.__class__.__name__ }-{self.task_id}")
         self.logger.info('### Configuring task object ###')
         self.dag = dag
         self.dag_id = self.dag.dag_id
@@ -46,15 +46,15 @@
         workflow_shared_storage_source = StorageSource(workflow_shared_storage.pop("source", "None")).name
         provider_options = workflow_shared_storage.pop("provider_options", {})
         self.workflow_shared_storage = shared_storage_map[workflow_shared_storage_source](**workflow_shared_storage, **provider_options) if shared_storage_map[workflow_shared_storage_source] else shared_storage_map[workflow_shared_storage_source]
         # Container resources
         self.container_resources = container_resources if container_resources else {}
         self.provide_gpu = self.container_resources.pop("use_gpu", False)
         
-        self.deploy_mode = deploy_mode
+        self.deploy_mode = os.environ.get('DOMINO_DEPLOY_MODE')
 
         config.load_incluster_config()
         self.k8s_client = client.CoreV1Api()
 
         # Clients
         self.backend_client = DominoBackendRestClient(base_url="http://domino-backend-service:8000/")
 
@@ -141,17 +141,17 @@
             container_resources_obj = k8s.V1ResourceRequirements(**basic_container_resources)
 
             # Volumes
             all_volumes = []
             all_volume_mounts = []
 
             ######################## For local DOMINO_DEPLOY_MODE Operators dev ###########################################
-            if os.environ.get('DOMINO_DEPLOY_MODE') == 'local-k8s-dev':
+            if self.deploy_mode == 'local-k8s-dev':
                 source_image = self.piece.get('source_image')
-                repository_raw_project_name = str(source_image).split('/')[1].split(':')[0]
+                repository_raw_project_name = str(source_image).split('/')[2].split(':')[0]
                 persistent_volume_claim_name = 'pvc-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
 
                 persistent_volume_name = 'pv-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
                 persistent_volume_claim_name = 'pvc-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
 
                 pvc_exists = False
                 try:
```

### Comparing `domino-py-0.1.8/domino/utils/validators.py` & `domino-py-0.1.9/domino/utils/validators.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.8/domino_py.egg-info/PKG-INFO` & `domino-py-0.1.9/domino_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Domino project
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description:
```

### Comparing `domino-py-0.1.8/domino_py.egg-info/SOURCES.txt` & `domino-py-0.1.9/domino_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 domino/task.py
 domino/version.py
 domino/cli/__init__.py
 domino/cli/cli.py
 domino/cli/utils/__init__.py
 domino/cli/utils/config-domino-local.toml
 domino/cli/utils/constants.py
-domino/cli/utils/create_cluster.sh
 domino/cli/utils/pieces_repository.py
 domino/cli/utils/platform.py
 domino/client/__init__.py
 domino/client/airflow_client.py
 domino/client/domino_backend_client.py
 domino/client/fs_client.py
 domino/client/github_rest_client.py
```

### Comparing `domino-py-0.1.8/setup.py` & `domino-py-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     author="Luiz Tauffer and Vinicius Vaz",
     author_email="luiz@taufferconsulting.com",
     keywords=["airflow", "UI"],
     packages=find_packages(),
     package_data={
         'domino': [
             'cli/utils/config-domino-local.toml',
-            'cli/utils/create_cluster.sh',
             'helm/domino-airflow/kind-cluster-config',
             'helm/domino-airflow/**/*',
             'helm/domino-base/**/*',
             'helm/domino-airflow/charts/**',
             'domino/helm/domino-base/**',
             'domino/helm/domino-base/templates/**',
             'domino/helm/domino-base/templates/jobs/**',
```

