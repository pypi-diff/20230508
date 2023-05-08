# Comparing `tmp/dm-cli-1.0.8.tar.gz` & `tmp/dm-cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-cli-1.0.8.tar", last modified: Thu May  4 11:36:37 2023, max compression
+gzip compressed data, was "dm-cli-1.0.9.tar", last modified: Mon May  8 08:52:06 2023, max compression
```

## Comparing `dm-cli-1.0.8.tar` & `dm-cli-1.0.9.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.755676 dm-cli-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 11:36:27.000000 dm-cli-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-04 11:36:37.755676 dm-cli-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-04 11:36:27.000000 dm-cli-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.747676 dm-cli-1.0.8/dm_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.747676 dm-cli-1.0.8/dm_cli/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/bin/dm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.747676 dm-cli-1.0.8/dm_cli/command_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/command_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/command_group/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/command_group/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.751676 dm-cli-1.0.8/dm_cli/dmss_api/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.751676 dm-cli-1.0.8/dm_cli/dmss_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/access_control_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/blob_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/blueprint_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/datasource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   150478 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/document_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/export_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/health_check_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/lookup_table_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/personal_access_token_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/reference_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/whoami_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36779 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.755676 dm-cli-1.0.8/dm_cli/dmss_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/access_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/basic_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/data_source_information.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/data_source_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/get_blueprint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/pat_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/recipe_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/repository_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/storage_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/storage_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/storage_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.755676 dm-cli-1.0.8/dm_cli/dmss_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/import_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/import_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/package_tree_from_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.755676 dm-cli-1.0.8/dm_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/file_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.747676 dm-cli-1.0.8/dm_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-04 11:36:27.000000 dm-cli-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:36:37.755676 dm-cli-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-04 11:36:27.000000 dm-cli-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.831183 dm-cli-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 08:51:59.000000 dm-cli-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-08 08:52:06.831183 dm-cli-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-08 08:51:59.000000 dm-cli-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.827183 dm-cli-1.0.9/dm_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.827183 dm-cli-1.0.9/dm_cli/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/bin/dm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.827183 dm-cli-1.0.9/dm_cli/command_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/command_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/command_group/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/command_group/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.827183 dm-cli-1.0.9/dm_cli/dmss_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.831183 dm-cli-1.0.9/dm_cli/dmss_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/access_control_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/blob_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/blueprint_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/datasource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145993 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36939 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/document_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/export_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/health_check_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/lookup_table_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/personal_access_token_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/reference_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api/whoami_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36779 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.831183 dm-cli-1.0.9/dm_cli/dmss_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/access_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/data_source_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/data_source_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/get_blueprint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/pat_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/recipe_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/repository_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/storage_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/storage_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model/storage_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.831183 dm-cli-1.0.9/dm_cli/dmss_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/dmss_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/import_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/import_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/package_tree_from_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.831183 dm-cli-1.0.9/dm_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/utils/file_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/utils/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-08 08:51:59.000000 dm-cli-1.0.9/dm_cli/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:52:06.827183 dm-cli-1.0.9/dm_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-08 08:52:06.000000 dm-cli-1.0.9/dm_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-08 08:52:06.000000 dm-cli-1.0.9/dm_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:52:06.000000 dm-cli-1.0.9/dm_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-08 08:52:06.000000 dm-cli-1.0.9/dm_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-08 08:52:06.000000 dm-cli-1.0.9/dm_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-08 08:51:59.000000 dm-cli-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:52:06.831183 dm-cli-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 08:51:59.000000 dm-cli-1.0.9/setup.py
```

### Comparing `dm-cli-1.0.8/PKG-INFO` & `dm-cli-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/equinor/dm-cli
 Author: 
 Author-email: 
 License: MIT
 Description: [![PyPi version](https://img.shields.io/pypi/v/dm-cli)](https://pypi.org/project/dm-cli)
         [![PyPi downloads](https://img.shields.io/pypi/dm/dm-cli)](https://pypi.org/project/dm-cli)
```

### Comparing `dm-cli-1.0.8/README.md` & `dm-cli-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/bin/dm` & `dm-cli-1.0.9/dm_cli/bin/dm`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/command_group/data_source.py` & `dm-cli-1.0.9/dm_cli/command_group/data_source.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/command_group/entities.py` & `dm-cli-1.0.9/dm_cli/command_group/entities.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss.py` & `dm-cli-1.0.9/dm_cli/dmss.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/__init__.py` & `dm-cli-1.0.9/dm_cli/dmss_api/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/access_control_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/access_control_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/blob_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/blob_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/blueprint_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/blueprint_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/datasource_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/datasource_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/default_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/default_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1480,30 +1480,30 @@
                     'multipart/form-data'
                 ]
             },
             api_client=api_client,
             callable=__document_add_to_path
         )
 
-        def __document_get_by_id(
+        def __document_get(
             self,
-            id_reference,
+            reference,
             **kwargs
         ):
-            """Get By Id  # noqa: E501
+            """Get  # noqa: E501
 
-            Get document as JSON string.  - **id_reference**: <data_source>/<document_uuid> - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
+            Get document as JSON string.  - **reference**:   - By id: PROTOCOL://DATA SOURCE/$ID.Attribute   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY.Attribute   - By query: PROTOCOL://DATA SOURCE/$ID.list(key=value)    The PROTOCOL is optional, and the default is dmss.  - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_get_by_id(id_reference, async_req=True)
+            >>> thread = api.document_get(reference, async_req=True)
             >>> result = thread.get()
 
             Args:
-                id_reference (str):
+                reference (str):
 
             Keyword Args:
                 depth (int): [optional] if omitted the server will use the default value of 999
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
@@ -1543,197 +1543,76 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['id_reference'] = \
-                id_reference
+            kwargs['reference'] = \
+                reference
             return self.call_with_http_info(**kwargs)
 
-        self.document_get_by_id = _Endpoint(
+        self.document_get = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{id_reference}',
-                'operation_id': 'document_get_by_id',
+                'endpoint_path': '/api/documents/{reference}',
+                'operation_id': 'document_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id_reference',
+                    'reference',
                     'depth',
                 ],
                 'required': [
-                    'id_reference',
+                    'reference',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id_reference':
+                    'reference':
                         (str,),
                     'depth':
                         (int,),
                 },
                 'attribute_map': {
-                    'id_reference': 'id_reference',
+                    'reference': 'reference',
                     'depth': 'depth',
                 },
                 'location_map': {
-                    'id_reference': 'path',
+                    'reference': 'path',
                     'depth': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [],
             },
             api_client=api_client,
-            callable=__document_get_by_id
-        )
-
-        def __document_get_by_path(
-            self,
-            absolute_path,
-            **kwargs
-        ):
-            """Get By Path  # noqa: E501
-
-            Get a document by its absolute path.  - **absolute_path**: <protocol>://<data_source>/<path>.<attribute>  # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.document_get_by_path(absolute_path, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                absolute_path (str):
-
-            Keyword Args:
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (int/float/tuple): timeout setting for this request. If
-                    one number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_path'] = \
-                absolute_path
-            return self.call_with_http_info(**kwargs)
-
-        self.document_get_by_path = _Endpoint(
-            settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
-                'auth': [
-                    'APIKeyHeader',
-                    'OAuth2AuthorizationCodeBearer'
-                ],
-                'endpoint_path': '/api/documents-by-path/{absolute_path}',
-                'operation_id': 'document_get_by_path',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'absolute_path',
-                ],
-                'required': [
-                    'absolute_path',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'absolute_path':
-                        (str,),
-                },
-                'attribute_map': {
-                    'absolute_path': 'absolute_path',
-                },
-                'location_map': {
-                    'absolute_path': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json',
-                    'text/plain'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client,
-            callable=__document_get_by_path
+            callable=__document_get
         )
 
         def __document_remove(
             self,
             id_reference,
             **kwargs
         ):
```

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/document_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/document_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -448,30 +448,30 @@
                     'multipart/form-data'
                 ]
             },
             api_client=api_client,
             callable=__document_add_to_path
         )
 
-        def __document_get_by_id(
+        def __document_get(
             self,
-            id_reference,
+            reference,
             **kwargs
         ):
-            """Get By Id  # noqa: E501
+            """Get  # noqa: E501
 
-            Get document as JSON string.  - **id_reference**: <data_source>/<document_uuid> - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
+            Get document as JSON string.  - **reference**:   - By id: PROTOCOL://DATA SOURCE/$ID.Attribute   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY.Attribute   - By query: PROTOCOL://DATA SOURCE/$ID.list(key=value)    The PROTOCOL is optional, and the default is dmss.  - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_get_by_id(id_reference, async_req=True)
+            >>> thread = api.document_get(reference, async_req=True)
             >>> result = thread.get()
 
             Args:
-                id_reference (str):
+                reference (str):
 
             Keyword Args:
                 depth (int): [optional] if omitted the server will use the default value of 999
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
@@ -511,197 +511,76 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['id_reference'] = \
-                id_reference
+            kwargs['reference'] = \
+                reference
             return self.call_with_http_info(**kwargs)
 
-        self.document_get_by_id = _Endpoint(
+        self.document_get = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{id_reference}',
-                'operation_id': 'document_get_by_id',
+                'endpoint_path': '/api/documents/{reference}',
+                'operation_id': 'document_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id_reference',
+                    'reference',
                     'depth',
                 ],
                 'required': [
-                    'id_reference',
+                    'reference',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id_reference':
+                    'reference':
                         (str,),
                     'depth':
                         (int,),
                 },
                 'attribute_map': {
-                    'id_reference': 'id_reference',
+                    'reference': 'reference',
                     'depth': 'depth',
                 },
                 'location_map': {
-                    'id_reference': 'path',
+                    'reference': 'path',
                     'depth': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [],
             },
             api_client=api_client,
-            callable=__document_get_by_id
-        )
-
-        def __document_get_by_path(
-            self,
-            absolute_path,
-            **kwargs
-        ):
-            """Get By Path  # noqa: E501
-
-            Get a document by its absolute path.  - **absolute_path**: <protocol>://<data_source>/<path>.<attribute>  # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.document_get_by_path(absolute_path, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                absolute_path (str):
-
-            Keyword Args:
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (int/float/tuple): timeout setting for this request. If
-                    one number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_path'] = \
-                absolute_path
-            return self.call_with_http_info(**kwargs)
-
-        self.document_get_by_path = _Endpoint(
-            settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
-                'auth': [
-                    'APIKeyHeader',
-                    'OAuth2AuthorizationCodeBearer'
-                ],
-                'endpoint_path': '/api/documents-by-path/{absolute_path}',
-                'operation_id': 'document_get_by_path',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'absolute_path',
-                ],
-                'required': [
-                    'absolute_path',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'absolute_path':
-                        (str,),
-                },
-                'attribute_map': {
-                    'absolute_path': 'absolute_path',
-                },
-                'location_map': {
-                    'absolute_path': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json',
-                    'text/plain'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client,
-            callable=__document_get_by_path
+            callable=__document_get
         )
 
         def __document_remove(
             self,
             id_reference,
             **kwargs
         ):
```

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/entity_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/entity_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/export_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/health_check_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/health_check_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/lookup_table_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/lookup_table_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/personal_access_token_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/personal_access_token_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/reference_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/reference_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/search_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/search_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api/whoami_api.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api/whoami_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/api_client.py` & `dm-cli-1.0.9/dm_cli/dmss_api/api_client.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/configuration.py` & `dm-cli-1.0.9/dm_cli/dmss_api/configuration.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/exceptions.py` & `dm-cli-1.0.9/dm_cli/dmss_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/access_level.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/access_level.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/acl.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/acl.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/basic_entity.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/data_source_information.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from dm_cli.dmss_api.exceptions import ApiAttributeError
 
 
 
-class BasicEntity(ModelNormal):
+class DataSourceInformation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,40 +77,45 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'type': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
+            'host': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'host': 'host',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
-        """BasicEntity - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, name, *args, **kwargs):  # noqa: E501
+        """DataSourceInformation - a model defined in OpenAPI
 
         Args:
-            type (str):
+            id (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +140,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            host (str): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,15 +169,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
+        self.id = id
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -184,19 +191,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, type, *args, **kwargs):  # noqa: E501
-        """BasicEntity - a model defined in OpenAPI
+    def __init__(self, id, name, *args, **kwargs):  # noqa: E501
+        """DataSourceInformation - a model defined in OpenAPI
 
         Args:
-            type (str):
+            id (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,15 +229,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            host (str): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,15 +256,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
+        self.id = id
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/data_source_information.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from dm_cli.dmss_api.exceptions import ApiAttributeError
 
 
 
-class DataSourceInformation(ModelNormal):
+class Reference(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,14 +54,21 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('type',): {
+            'max_length': 128,
+            'min_length': 3,
+            'regex': {
+                'pattern': r'^[A-Z:a-z0-9_\/-]*$',  # noqa: E501
+            },
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -77,45 +84,44 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'host': (str,),  # noqa: E501
+            'address': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
+            'reference_type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'host': 'host',  # noqa: E501
+        'address': 'address',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'reference_type': 'referenceType',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, *args, **kwargs):  # noqa: E501
-        """DataSourceInformation - a model defined in OpenAPI
+    def _from_openapi_data(cls, address, type, reference_type, *args, **kwargs):  # noqa: E501
+        """Reference - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            address (str):
+            type (str):
+            reference_type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,16 +146,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            host (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -169,16 +173,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
+        self.address = address
+        self.type = type
+        self.reference_type = reference_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -191,20 +196,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, *args, **kwargs):  # noqa: E501
-        """DataSourceInformation - a model defined in OpenAPI
+    def __init__(self, address, type, reference_type, *args, **kwargs):  # noqa: E501
+        """Reference - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            address (str):
+            type (str):
+            reference_type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,16 +235,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            host (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,16 +260,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
+        self.address = address
+        self.type = type
+        self.reference_type = reference_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/data_source_request.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/data_source_request.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/entity.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/entity.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/error_response.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/error_response.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/get_blueprint_response.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/get_blueprint_response.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/lookup.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/lookup.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/pat_data.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/pat_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             pat_hash (str): [optional]  # noqa: E501
-            uuid (str): [optional] if omitted the server will use the default value of "2b08fad1-2d28-4d42-a399-58c7a7fb77f7"  # noqa: E501
+            uuid (str): [optional] if omitted the server will use the default value of "e298aba4-84af-4270-bf81-6f11f48680b0"  # noqa: E501
             roles ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -244,15 +244,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             pat_hash (str): [optional]  # noqa: E501
-            uuid (str): [optional] if omitted the server will use the default value of "2b08fad1-2d28-4d42-a399-58c7a7fb77f7"  # noqa: E501
+            uuid (str): [optional] if omitted the server will use the default value of "e298aba4-84af-4270-bf81-6f11f48680b0"  # noqa: E501
             roles ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/recipe.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/recipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,15 @@
             'attributes': ([RecipeAttribute],),  # noqa: E501
             'description': (str,),  # noqa: E501
             'plugin': (str,),  # noqa: E501
             'category': (str,),  # noqa: E501
             'roles': ([str],),  # noqa: E501
             'config': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'label': (str,),  # noqa: E501
+            'dimensions': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -109,14 +110,15 @@
         'attributes': 'attributes',  # noqa: E501
         'description': 'description',  # noqa: E501
         'plugin': 'plugin',  # noqa: E501
         'category': 'category',  # noqa: E501
         'roles': 'roles',  # noqa: E501
         'config': 'config',  # noqa: E501
         'label': 'label',  # noqa: E501
+        'dimensions': 'dimensions',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -163,14 +165,15 @@
             attributes ([RecipeAttribute]): [optional] if omitted the server will use the default value of []  # noqa: E501
             description (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
             plugin (str): [optional] if omitted the server will use the default value of "Default"  # noqa: E501
             category (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
             roles ([str]): [optional]  # noqa: E501
             config ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             label (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
+            dimensions (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,14 +259,15 @@
             attributes ([RecipeAttribute]): [optional] if omitted the server will use the default value of []  # noqa: E501
             description (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
             plugin (str): [optional] if omitted the server will use the default value of "Default"  # noqa: E501
             category (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
             roles ([str]): [optional]  # noqa: E501
             config ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             label (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
+            dimensions (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/recipe_attribute.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/recipe_attribute.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/reference.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/storage_recipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from dm_cli.dmss_api.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from dm_cli.dmss_api.model.storage_attribute import StorageAttribute
+    globals()['StorageAttribute'] = StorageAttribute
 
-class Reference(ModelNormal):
+
+class StorageRecipe(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,81 +58,71 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'max_length': 128,
-            'min_length': 1,
-            'regex': {
-                'pattern': r'^[A-Za-z0-9_-]*$',  # noqa: E501
-            },
-        },
-        ('type',): {
-            'max_length': 128,
-            'min_length': 3,
-            'regex': {
-                'pattern': r'^[A-Z:a-z0-9_\/-]*$',  # noqa: E501
-            },
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
+            'attributes': ({str: (StorageAttribute,)},),  # noqa: E501
+            'storage_affinity': (dict,),  # noqa: E501
+            'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': '_id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'storage_affinity': 'storageAffinity',  # noqa: E501
+        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, type, *args, **kwargs):  # noqa: E501
-        """Reference - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """StorageRecipe - a model defined in OpenAPI
 
         Args:
-            id (str):
             name (str):
-            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,14 +147,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (str): [optional] if omitted the server will use the default value of "dmss://system/SIMOS/StorageRecipe"  # noqa: E501
+            attributes ({str: (StorageAttribute,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
+            storage_affinity (dict): [optional]  # noqa: E501
+            description (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,17 +178,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         self.name = name
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -203,21 +199,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, type, *args, **kwargs):  # noqa: E501
-        """Reference - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """StorageRecipe - a model defined in OpenAPI
 
         Args:
-            id (str):
             name (str):
-            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -242,14 +236,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (str): [optional] if omitted the server will use the default value of "dmss://system/SIMOS/StorageRecipe"  # noqa: E501
+            attributes ({str: (StorageAttribute,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
+            storage_affinity (dict): [optional]  # noqa: E501
+            description (str): [optional] if omitted the server will use the default value of ""  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -267,17 +265,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         self.name = name
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/repository.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/repository.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/repository_type.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/repository_type.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/storage_attribute.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/storage_attribute.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model/storage_data_types.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model/storage_data_types.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/model_utils.py` & `dm-cli-1.0.9/dm_cli/dmss_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/models/__init__.py` & `dm-cli-1.0.9/dm_cli/dmss_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/dmss_api/rest.py` & `dm-cli-1.0.9/dm_cli/dmss_api/rest.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/domain.py` & `dm-cli-1.0.9/dm_cli/domain.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/enums.py` & `dm-cli-1.0.9/dm_cli/enums.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/import_entity.py` & `dm-cli-1.0.9/dm_cli/import_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 def import_folder_entity(source_path: Path, destination: str) -> None:
     print(f"Importing PACKAGE '{source_path.name}' --> '{destination}/'")
     destination_path = Path(destination)
     data_source = destination_path.parts[0]
 
     try:  # Check if target already exists on remote. Then delete or raise exception
-        dmss_api.document_get_by_path(f"dmss://{destination}/{source_path.name}")
+        dmss_api.document_get(f"dmss://{destination}/{source_path.name}")
         if not state.force:
             raise ValueError(f"Failed to upload to 'dmss://{destination}/{source_path.name}' - It already exists.")
         console.print(
             f"WARNING: '{destination}/{source_path.name}' already exists. Replacing it...", style="dark_orange"
         )
         dmss_api.document_remove_by_path(f"{destination}/{source_path.name}")
     except NotFoundException:
```

### Comparing `dm-cli-1.0.8/dm_cli/import_package.py` & `dm-cli-1.0.9/dm_cli/import_package.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/package_tree_from_zip.py` & `dm-cli-1.0.9/dm_cli/package_tree_from_zip.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/utils/file_structure.py` & `dm-cli-1.0.9/dm_cli/utils/file_structure.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/utils/reference.py` & `dm-cli-1.0.9/dm_cli/utils/reference.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli/utils/utils.py` & `dm-cli-1.0.9/dm_cli/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         return False
     return True
 
 
 def ensure_package_structure(path: Path):
     """Create any missing packages in the provided path (mkdir -R)"""
     try:
-        dmss_api.document_get_by_path(f"dmss://{path}/")
+        dmss_api.document_get(f"dmss://{path}/")
     except NotFoundException as e:
         error = json.loads(e.body)
         if error["status"] != 404:
             print(f"Target package '{path}' is likely corrupt!")
             pprint.pformat(error)
             raise typer.Exit(code=1)
```

### Comparing `dm-cli-1.0.8/dm_cli/utils/zip.py` & `dm-cli-1.0.9/dm_cli/utils/zip.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.8/dm_cli.egg-info/PKG-INFO` & `dm-cli-1.0.9/dm_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/equinor/dm-cli
 Author: 
 Author-email: 
 License: MIT
 Description: [![PyPi version](https://img.shields.io/pypi/v/dm-cli)](https://pypi.org/project/dm-cli)
         [![PyPi downloads](https://img.shields.io/pypi/dm/dm-cli)](https://pypi.org/project/dm-cli)
```

### Comparing `dm-cli-1.0.8/dm_cli.egg-info/SOURCES.txt` & `dm-cli-1.0.9/dm_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 dm_cli/dmss_api/api/personal_access_token_api.py
 dm_cli/dmss_api/api/reference_api.py
 dm_cli/dmss_api/api/search_api.py
 dm_cli/dmss_api/api/whoami_api.py
 dm_cli/dmss_api/model/__init__.py
 dm_cli/dmss_api/model/access_level.py
 dm_cli/dmss_api/model/acl.py
-dm_cli/dmss_api/model/basic_entity.py
 dm_cli/dmss_api/model/data_source_information.py
 dm_cli/dmss_api/model/data_source_request.py
 dm_cli/dmss_api/model/entity.py
 dm_cli/dmss_api/model/error_response.py
 dm_cli/dmss_api/model/get_blueprint_response.py
 dm_cli/dmss_api/model/lookup.py
 dm_cli/dmss_api/model/pat_data.py
```

### Comparing `dm-cli-1.0.8/setup.py` & `dm-cli-1.0.9/setup.py`

 * *Files identical despite different names*

