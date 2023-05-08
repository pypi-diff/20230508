# Comparing `tmp/aikoai-2.2.tar.gz` & `tmp/aikoai-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikoai-2.2.tar", last modified: Mon May  8 17:57:26 2023, max compression
+gzip compressed data, was "aikoai-3.1.tar", last modified: Mon May  8 18:13:31 2023, max compression
```

## Comparing `aikoai-2.2.tar` & `aikoai-3.1.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:26.892163 aikoai-2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 17:57:26.892163 aikoai-2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:26.884163 aikoai-2.2/aikoai/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/_aikoai_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/aikoai_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/aikoai_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:26.888163 aikoai-2.2/aikoai/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:26.888163 aikoai-2.2/aikoai/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/abstract/api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/abstract/engine_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/error_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:26.892163 aikoai-2.2/aikoai/api_resources/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/experimental/completion_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/fine_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/api_resources/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38173 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:26.892163 aikoai-2.2/aikoai/datalib/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/datalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/datalib/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/datalib/numpy_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/datalib/pandas_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/embeddings_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/object_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:26.892163 aikoai-2.2/aikoai/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:26.892163 aikoai-2.2/aikoai/tests/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/asyncio/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/test_api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/test_file_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/test_long_examples_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/test_url_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/upload_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    34289 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-05-08 17:57:13.000000 aikoai-2.2/aikoai/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:26.888163 aikoai-2.2/aikoai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 17:57:26.000000 aikoai-2.2/aikoai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-08 17:57:26.000000 aikoai-2.2/aikoai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:57:26.000000 aikoai-2.2/aikoai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 17:57:26.000000 aikoai-2.2/aikoai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 17:57:26.000000 aikoai-2.2/aikoai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 17:57:26.000000 aikoai-2.2/aikoai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:57:26.000000 aikoai-2.2/aikoai.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-08 17:57:13.000000 aikoai-2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-08 17:57:26.892163 aikoai-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 17:57:13.000000 aikoai-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:31.860730 aikoai-3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 18:13:31.864730 aikoai-3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:31.856729 aikoai-3.1/aikoai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/_aikoai_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/aiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/aikoai_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/aikoai_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:31.860730 aikoai-3.1/aikoai/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:31.860730 aikoai-3.1/aikoai/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/abstract/api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/abstract/engine_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/error_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:31.860730 aikoai-3.1/aikoai/api_resources/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/experimental/completion_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/fine_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/api_resources/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38173 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:31.860730 aikoai-3.1/aikoai/datalib/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/datalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/datalib/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/datalib/numpy_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/datalib/pandas_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/embeddings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/object_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:31.860730 aikoai-3.1/aikoai/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:31.860730 aikoai-3.1/aikoai/tests/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/asyncio/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/test_api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/test_file_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/test_long_examples_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/test_url_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/upload_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34289 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-05-08 18:13:20.000000 aikoai-3.1/aikoai/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:13:31.856729 aikoai-3.1/aikoai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 18:13:31.000000 aikoai-3.1/aikoai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-08 18:13:31.000000 aikoai-3.1/aikoai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:13:31.000000 aikoai-3.1/aikoai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 18:13:31.000000 aikoai-3.1/aikoai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 18:13:31.000000 aikoai-3.1/aikoai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 18:13:31.000000 aikoai-3.1/aikoai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:13:31.000000 aikoai-3.1/aikoai.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-08 18:13:20.000000 aikoai-3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-08 18:13:31.864730 aikoai-3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:13:20.000000 aikoai-3.1/setup.py
```

### Comparing `aikoai-2.2/aikoai/__init__.py` & `aikoai-3.1/aikoai/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 # Originally forked from the MIT-licensed Stripe Python bindings.
 
 import os
 import sys
 from typing import TYPE_CHECKING, Optional, Union, Callable
 
 from contextvars import ContextVar
+import aiko
 
 if "pkg_resources" not in sys.modules:
-    # workaround for the following:
-    # https://github.com/benoitc/gunicorn/pull/2539
     sys.modules["pkg_resources"] = object()  # type: ignore[assignment]
     import aiohttp
 
     del sys.modules["pkg_resources"]
 
 from aikoai.api_resources import (
     Audio,
@@ -42,16 +41,16 @@
 api_key = 'sk-' + os.environ.get("AIKOAI_API_KEY")
 # Path of a file with an API key, whose contents can change. Supercedes
 # `api_key` if set.  The main use case is volume-mounted Kubernetes secrets,
 # which are updated automatically.
 api_key_path: Optional[str] = os.environ.get("AIKOAI_API_KEY_PATH")
 
 organization = os.environ.get("AIKOAI_ORGANIZATION")
-api_base = os.environ.get("AIKOAI_API_BASE", "https://api.openai.com/v1")
-api_type = os.environ.get("AIKOAI_API_TYPE", "open_ai")
+api_base = os.environ.get("AIKOAI_API_BASE", aiko.api_base)
+api_type = os.environ.get("AIKOAI_API_TYPE", aiko.api_type)
 api_version = os.environ.get(
     "AIKOAI_API_VERSION",
     ("2023-03-15-preview" if api_type in ("azure", "azure_ad", "azuread") else None),
 )
 verify_ssl_certs = True  # No effect. Certificates are always verified.
 proxy = None
 app_info = None
```

### Comparing `aikoai-2.2/aikoai/_aikoai_scripts.py` & `aikoai-3.1/aikoai/_aikoai_scripts.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/aikoai_object.py` & `aikoai-3.1/aikoai/aikoai_object.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/aikoai_response.py` & `aikoai-3.1/aikoai/aikoai_response.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_requestor.py` & `aikoai-3.1/aikoai/api_requestor.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/__init__.py` & `aikoai-3.1/aikoai/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/abstract/__init__.py` & `aikoai-3.1/aikoai/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/abstract/api_resource.py` & `aikoai-3.1/aikoai/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/abstract/createable_api_resource.py` & `aikoai-3.1/aikoai/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/abstract/deletable_api_resource.py` & `aikoai-3.1/aikoai/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/abstract/engine_api_resource.py` & `aikoai-3.1/aikoai/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/abstract/listable_api_resource.py` & `aikoai-3.1/aikoai/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/abstract/nested_resource_class_methods.py` & `aikoai-3.1/aikoai/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/abstract/updateable_api_resource.py` & `aikoai-3.1/aikoai/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/audio.py` & `aikoai-3.1/aikoai/api_resources/audio.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/chat_completion.py` & `aikoai-3.1/aikoai/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/completion.py` & `aikoai-3.1/aikoai/api_resources/completion.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/customer.py` & `aikoai-3.1/aikoai/api_resources/customer.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/deployment.py` & `aikoai-3.1/aikoai/api_resources/deployment.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/edit.py` & `aikoai-3.1/aikoai/api_resources/edit.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/embedding.py` & `aikoai-3.1/aikoai/api_resources/embedding.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/engine.py` & `aikoai-3.1/aikoai/api_resources/engine.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/error_object.py` & `aikoai-3.1/aikoai/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/file.py` & `aikoai-3.1/aikoai/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/fine_tune.py` & `aikoai-3.1/aikoai/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/image.py` & `aikoai-3.1/aikoai/api_resources/image.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/api_resources/moderation.py` & `aikoai-3.1/aikoai/api_resources/moderation.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/cli.py` & `aikoai-3.1/aikoai/cli.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/datalib/__init__.py` & `aikoai-3.1/aikoai/datalib/__init__.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/embeddings_utils.py` & `aikoai-3.1/aikoai/embeddings_utils.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/error.py` & `aikoai-3.1/aikoai/error.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/tests/asyncio/test_endpoints.py` & `aikoai-3.1/aikoai/tests/asyncio/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/tests/test_api_requestor.py` & `aikoai-3.1/aikoai/tests/test_api_requestor.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/tests/test_endpoints.py` & `aikoai-3.1/aikoai/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/tests/test_exceptions.py` & `aikoai-3.1/aikoai/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/tests/test_file_cli.py` & `aikoai-3.1/aikoai/tests/test_file_cli.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/tests/test_long_examples_validator.py` & `aikoai-3.1/aikoai/tests/test_long_examples_validator.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/tests/test_url_composition.py` & `aikoai-3.1/aikoai/tests/test_url_composition.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/tests/test_util.py` & `aikoai-3.1/aikoai/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/upload_progress.py` & `aikoai-3.1/aikoai/upload_progress.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/util.py` & `aikoai-3.1/aikoai/util.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/validators.py` & `aikoai-3.1/aikoai/validators.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai/wandb_logger.py` & `aikoai-3.1/aikoai/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `aikoai-2.2/aikoai.egg-info/SOURCES.txt` & `aikoai-3.1/aikoai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 pyproject.toml
 setup.cfg
 setup.py
 aikoai/__init__.py
 aikoai/_aikoai_scripts.py
+aikoai/aiko.py
 aikoai/aikoai_object.py
 aikoai/aikoai_response.py
 aikoai/api_requestor.py
 aikoai/cli.py
 aikoai/embeddings_utils.py
 aikoai/error.py
 aikoai/object_classes.py
```

### Comparing `aikoai-2.2/setup.cfg` & `aikoai-3.1/setup.cfg`

 * *Files identical despite different names*

