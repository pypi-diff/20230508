# Comparing `tmp/aikoai-1.1.tar.gz` & `tmp/aikoai-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikoai-1.1.tar", last modified: Mon May  8 17:25:32 2023, max compression
+gzip compressed data, was "aikoai-2.1.tar", last modified: Mon May  8 17:50:58 2023, max compression
```

## Comparing `aikoai-1.1.tar` & `aikoai-2.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:32.000132 aikoai-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 17:25:32.000132 aikoai-1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:31.996132 aikoai-1.1/aikoai/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/_aikoai_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/aikoai_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/aikoai_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:32.000132 aikoai-1.1/aikoai/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:32.000132 aikoai-1.1/aikoai/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/abstract/api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/abstract/engine_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/error_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:32.000132 aikoai-1.1/aikoai/api_resources/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/experimental/completion_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/fine_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/api_resources/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38173 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:32.000132 aikoai-1.1/aikoai/datalib/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/datalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/datalib/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/datalib/numpy_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/datalib/pandas_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/embeddings_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/object_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:32.000132 aikoai-1.1/aikoai/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:32.000132 aikoai-1.1/aikoai/tests/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/asyncio/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/test_api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/test_file_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/test_long_examples_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/test_url_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/upload_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    34289 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-05-08 17:25:17.000000 aikoai-1.1/aikoai/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:25:31.996132 aikoai-1.1/aikoai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 17:25:31.000000 aikoai-1.1/aikoai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-08 17:25:31.000000 aikoai-1.1/aikoai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:25:31.000000 aikoai-1.1/aikoai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 17:25:31.000000 aikoai-1.1/aikoai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 17:25:31.000000 aikoai-1.1/aikoai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 17:25:31.000000 aikoai-1.1/aikoai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:25:31.000000 aikoai-1.1/aikoai.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-08 17:25:17.000000 aikoai-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-08 17:25:32.004133 aikoai-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 17:25:17.000000 aikoai-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:58.366010 aikoai-2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 17:50:58.366010 aikoai-2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:58.358010 aikoai-2.1/aikoai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/_aikoai_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/aikoai_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/aikoai_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:58.362010 aikoai-2.1/aikoai/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:58.362010 aikoai-2.1/aikoai/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/abstract/api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10015 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/abstract/engine_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/error_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:58.362010 aikoai-2.1/aikoai/api_resources/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/experimental/completion_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/fine_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/api_resources/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:58.362010 aikoai-2.1/aikoai/datalib/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/datalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/datalib/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/datalib/numpy_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/datalib/pandas_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/embeddings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/object_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:58.366010 aikoai-2.1/aikoai/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:58.366010 aikoai-2.1/aikoai/tests/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/asyncio/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/test_api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/test_file_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/test_long_examples_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/test_url_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/upload_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34275 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-08 17:50:37.000000 aikoai-2.1/aikoai/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:58.358010 aikoai-2.1/aikoai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 17:50:58.000000 aikoai-2.1/aikoai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-08 17:50:58.000000 aikoai-2.1/aikoai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:50:58.000000 aikoai-2.1/aikoai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 17:50:58.000000 aikoai-2.1/aikoai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 17:50:58.000000 aikoai-2.1/aikoai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 17:50:58.000000 aikoai-2.1/aikoai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:50:58.000000 aikoai-2.1/aikoai.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-08 17:50:37.000000 aikoai-2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-08 17:50:58.366010 aikoai-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 17:50:37.000000 aikoai-2.1/setup.py
```

### Comparing `aikoai-1.1/aikoai/__init__.py` & `aikoai-2.1/aikoai/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,32 +28,32 @@
     ErrorObject,
     File,
     FineTune,
     Image,
     Model,
     Moderation,
 )
-from aikoai.error import APIError, InvalidRequestError, AikoAIError
+from aikoai.error import APIError, InvalidRequestError, OpenAIError
 from aikoai.version import VERSION
 
 if TYPE_CHECKING:
     import requests
     from aiohttp import ClientSession
 
-api_key = 'sk-' + os.environ.get("AIKOAI_API_KEY")
+api_key = os.environ.get("OPENAI_API_KEY")
 # Path of a file with an API key, whose contents can change. Supercedes
 # `api_key` if set.  The main use case is volume-mounted Kubernetes secrets,
 # which are updated automatically.
-api_key_path: Optional[str] = os.environ.get("AIKOAI_API_KEY_PATH")
+api_key_path: Optional[str] = os.environ.get("OPENAI_API_KEY_PATH")
 
-organization = os.environ.get("AIKOAI_ORGANIZATION")
-api_base = os.environ.get("AIKOAI_API_BASE", "https://api.openai.com/v1")
-api_type = os.environ.get("AIKOAI_API_TYPE", "open_ai")
+organization = os.environ.get("OPENAI_ORGANIZATION")
+api_base = os.environ.get("OPENAI_API_BASE", "https://api.openai.com/v1")
+api_type = os.environ.get("OPENAI_API_TYPE", "open_ai")
 api_version = os.environ.get(
-    "AIKOAI_API_VERSION",
+    "OPENAI_API_VERSION",
     ("2023-03-15-preview" if api_type in ("azure", "azure_ad", "azuread") else None),
 )
 verify_ssl_certs = True  # No effect. Certificates are always verified.
 proxy = None
 app_info = None
 enable_telemetry = False  # Ignored; the telemetry feature was removed.
 ca_bundle_path = None  # No longer used, feature was removed
@@ -83,15 +83,15 @@
     "Engine",
     "ErrorObject",
     "File",
     "FineTune",
     "InvalidRequestError",
     "Model",
     "Moderation",
-    "AikoAIError",
+    "OpenAIError",
     "api_base",
     "api_key",
     "api_type",
     "api_key_path",
     "api_version",
     "app_info",
     "ca_bundle_path",
```

### Comparing `aikoai-1.1/aikoai/_aikoai_scripts.py` & `aikoai-2.1/aikoai/_aikoai_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             if proxy.startswith('https'):
                 aikoai.proxy['https'] = proxy
             elif proxy.startswith('http'):
                 aikoai.proxy['http'] = proxy
 
     try:
         args.func(args)
-    except aikoai.error.AikoAIError as e:
+    except aikoai.error.OpenAIError as e:
         display_error(e)
         return 1
     except KeyboardInterrupt:
         sys.stderr.write("\n")
         return 1
     return 0
```

### Comparing `aikoai-1.1/aikoai/aikoai_object.py` & `aikoai-2.1/aikoai/aikoai_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import json
 from copy import deepcopy
 from typing import Optional, Tuple, Union
 
 import aikoai
 from aikoai import api_requestor, util
-from aikoai.aikoai_response import AikoAIResponse
+from aikoai.aikoai_response import OpenAIResponse
 from aikoai.util import ApiType
 
 
-class AikoAIObject(dict):
+class OpenAIObject(dict):
     api_base_override = None
 
     def __init__(
         self,
         id=None,
         api_key=None,
         api_version=None,
         api_type=None,
         organization=None,
         response_ms: Optional[int] = None,
         api_base=None,
         engine=None,
         **params,
     ):
-        super(AikoAIObject, self).__init__()
+        super(OpenAIObject, self).__init__()
 
         if response_ms is not None and not isinstance(response_ms, int):
             raise TypeError(f"response_ms is a {type(response_ms).__name__}.")
         self._response_ms = response_ms
 
         self._retrieve_params = params
 
@@ -43,41 +43,41 @@
 
     @property
     def response_ms(self) -> Optional[int]:
         return self._response_ms
 
     def __setattr__(self, k, v):
         if k[0] == "_" or k in self.__dict__:
-            return super(AikoAIObject, self).__setattr__(k, v)
+            return super(OpenAIObject, self).__setattr__(k, v)
 
         self[k] = v
         return None
 
     def __getattr__(self, k):
         if k[0] == "_":
             raise AttributeError(k)
         try:
             return self[k]
         except KeyError as err:
             raise AttributeError(*err.args)
 
     def __delattr__(self, k):
         if k[0] == "_" or k in self.__dict__:
-            return super(AikoAIObject, self).__delattr__(k)
+            return super(OpenAIObject, self).__delattr__(k)
         else:
             del self[k]
 
     def __setitem__(self, k, v):
         if v == "":
             raise ValueError(
                 "You cannot set %s to an empty string. "
                 "We interpret empty strings as None in requests."
                 "You may set %s.%s = None to delete the property" % (k, str(self), k)
             )
-        super(AikoAIObject, self).__setitem__(k, v)
+        super(OpenAIObject, self).__setitem__(k, v)
 
     def __delitem__(self, k):
         raise NotImplementedError("del is not supported")
 
     # Custom unpickling method that uses `update` to update the dictionary
     # without calling __setitem__, which would fail if any value is an empty
     # string
@@ -142,16 +142,16 @@
         self.api_type = api_type or getattr(values, "api_type", None)
         self.organization = organization or getattr(values, "organization", None)
         self._response_ms = response_ms or getattr(values, "_response_ms", None)
 
         # Wipe old state before setting new.
         self.clear()
         for k, v in values.items():
-            super(AikoAIObject, self).__setitem__(
-                k, util.convert_to_aikoai_object(v, api_key, api_version, organization)
+            super(OpenAIObject, self).__setitem__(
+                k, util.convert_to_aikoai_response(v, api_key, api_version, organization)
             )
 
         self._previous = values
 
     @classmethod
     def api_base(cls):
         return None
@@ -183,27 +183,27 @@
             stream=stream,
             headers=headers,
             request_id=request_id,
             request_timeout=request_timeout,
         )
 
         if stream:
-            assert not isinstance(response, AikoAIResponse)  # must be an iterator
+            assert not isinstance(response, OpenAIResponse)  # must be an iterator
             return (
-                util.convert_to_aikoai_object(
+                util.convert_to_aikoai_response(
                     line,
                     api_key,
                     self.api_version,
                     self.organization,
                     plain_old_data=plain_old_data,
                 )
                 for line in response
             )
         else:
-            return util.convert_to_aikoai_object(
+            return util.convert_to_aikoai_response(
                 response,
                 api_key,
                 self.api_version,
                 self.organization,
                 plain_old_data=plain_old_data,
             )
 
@@ -234,27 +234,27 @@
             stream=stream,
             headers=headers,
             request_id=request_id,
             request_timeout=request_timeout,
         )
 
         if stream:
-            assert not isinstance(response, AikoAIResponse)  # must be an iterator
+            assert not isinstance(response, OpenAIResponse)  # must be an iterator
             return (
-                util.convert_to_aikoai_object(
+                util.convert_to_aikoai_response(
                     line,
                     api_key,
                     self.api_version,
                     self.organization,
                     plain_old_data=plain_old_data,
                 )
                 for line in response
             )
         else:
-            return util.convert_to_aikoai_object(
+            return util.convert_to_aikoai_response(
                 response,
                 api_key,
                 self.api_version,
                 self.organization,
                 plain_old_data=plain_old_data,
             )
 
@@ -282,25 +282,25 @@
 
     def to_dict(self):
         return dict(self)
 
     def to_dict_recursive(self):
         d = dict(self)
         for k, v in d.items():
-            if isinstance(v, AikoAIObject):
+            if isinstance(v, OpenAIObject):
                 d[k] = v.to_dict_recursive()
             elif isinstance(v, list):
                 d[k] = [
-                    e.to_dict_recursive() if isinstance(e, AikoAIObject) else e
+                    e.to_dict_recursive() if isinstance(e, OpenAIObject) else e
                     for e in v
                 ]
         return d
 
     @property
-    def aikoai_id(self):
+    def openai_id(self):
         return self.id
 
     @property
     def typed_api_type(self):
         return (
             ApiType.from_str(self.api_type)
             if self.api_type
@@ -309,28 +309,28 @@
 
     # This class overrides __setitem__ to throw exceptions on inputs that it
     # doesn't like. This can cause problems when we try to copy an object
     # wholesale because some data that's returned from the API may not be valid
     # if it was set to be set manually. Here we override the class' copy
     # arguments so that we can bypass these possible exceptions on __setitem__.
     def __copy__(self):
-        copied = AikoAIObject(
+        copied = OpenAIObject(
             self.get("id"),
             self.api_key,
             api_version=self.api_version,
             api_type=self.api_type,
             organization=self.organization,
         )
 
         copied._retrieve_params = self._retrieve_params
 
         for k, v in self.items():
             # Call parent's __setitem__ to avoid checks that we've added in the
             # overridden version that can throw exceptions.
-            super(AikoAIObject, copied).__setitem__(k, v)
+            super(OpenAIObject, copied).__setitem__(k, v)
 
         return copied
 
     # This class overrides __setitem__ to throw exceptions on inputs that it
     # doesn't like. This can cause problems when we try to copy an object
     # wholesale because some data that's returned from the API may not be valid
     # if it was set to be set manually. Here we override the class' copy
@@ -338,10 +338,10 @@
     def __deepcopy__(self, memo):
         copied = self.__copy__()
         memo[id(self)] = copied
 
         for k, v in self.items():
             # Call parent's __setitem__ to avoid checks that we've added in the
             # overridden version that can throw exceptions.
-            super(AikoAIObject, copied).__setitem__(k, deepcopy(v, memo))
+            super(OpenAIObject, copied).__setitem__(k, deepcopy(v, memo))
 
         return copied
```

### Comparing `aikoai-1.1/aikoai/aikoai_response.py` & `aikoai-2.1/aikoai/aikoai_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Optional
 
 
-class AikoAIResponse:
+class OpenAIResponse:
     def __init__(self, data, headers):
         self._headers = headers
         self.data = data
 
     @property
     def request_id(self) -> Optional[str]:
         return self._headers.get("request-id")
 
     @property
     def organization(self) -> Optional[str]:
-        return self._headers.get("AikoAI-Organization")
+        return self._headers.get("OpenAI-Organization")
 
     @property
     def response_ms(self) -> Optional[int]:
-        h = self._headers.get("AikoAI-Processing-Ms")
+        h = self._headers.get("Openai-Processing-Ms")
         return None if h is None else round(float(h))
```

### Comparing `aikoai-1.1/aikoai/api_requestor.py` & `aikoai-2.1/aikoai/api_requestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 import aikoai
 from aikoai import error, util, version
-from aikoai.aikoai_response import AikoAIResponse
+from aikoai.aikoai_response import OpenAIResponse
 from aikoai.util import ApiType
 
 TIMEOUT_SECS = 600
 MAX_CONNECTION_RETRIES = 2
 
 # Has one attribute per thread, 'session'.
 _thread_context = threading.local()
@@ -53,39 +53,39 @@
         return None
     elif isinstance(proxy, str):
         return {"http": proxy, "https": proxy}
     elif isinstance(proxy, dict):
         return proxy.copy()
     else:
         raise ValueError(
-            "'aikoai.proxy' must be specified as either a string URL or a dict with string URL under the https and/or http keys."
+            "'openai.proxy' must be specified as either a string URL or a dict with string URL under the https and/or http keys."
         )
 
 
 def _aiohttp_proxies_arg(proxy) -> Optional[str]:
     """Returns a value suitable for the 'proxies' argument to 'aiohttp.ClientSession.request."""
     if proxy is None:
         return None
     elif isinstance(proxy, str):
         return proxy
     elif isinstance(proxy, dict):
         return proxy["https"] if "https" in proxy else proxy["http"]
     else:
         raise ValueError(
-            "'aikoai.proxy' must be specified as either a string URL or a dict with string URL under the https and/or http keys."
+            "'openai.proxy' must be specified as either a string URL or a dict with string URL under the https and/or http keys."
         )
 
 
 def _make_session() -> requests.Session:
     if aikoai.requestssession:
         if isinstance(aikoai.requestssession, requests.Session):
             return aikoai.requestssession
         return aikoai.requestssession()
     if not aikoai.verify_ssl_certs:
-        warnings.warn("verify_ssl_certs is ignored; aikoai always verifies.")
+        warnings.warn("verify_ssl_certs is ignored; openai always verifies.")
     s = requests.Session()
     proxies = _requests_proxies_arg(aikoai.proxy)
     if proxies:
         s.proxies = proxies
     s.mount(
         "https://",
         requests.adapters.HTTPAdapter(max_retries=MAX_CONNECTION_RETRIES),
@@ -156,71 +156,71 @@
         url,
         params,
         headers,
         files,
         stream: Literal[True],
         request_id: Optional[str] = ...,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = ...,
-    ) -> Tuple[Iterator[AikoAIResponse], bool, str]:
+    ) -> Tuple[Iterator[OpenAIResponse], bool, str]:
         pass
 
     @overload
     def request(
         self,
         method,
         url,
         params=...,
         headers=...,
         files=...,
         *,
         stream: Literal[True],
         request_id: Optional[str] = ...,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = ...,
-    ) -> Tuple[Iterator[AikoAIResponse], bool, str]:
+    ) -> Tuple[Iterator[OpenAIResponse], bool, str]:
         pass
 
     @overload
     def request(
         self,
         method,
         url,
         params=...,
         headers=...,
         files=...,
         stream: Literal[False] = ...,
         request_id: Optional[str] = ...,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = ...,
-    ) -> Tuple[AikoAIResponse, bool, str]:
+    ) -> Tuple[OpenAIResponse, bool, str]:
         pass
 
     @overload
     def request(
         self,
         method,
         url,
         params=...,
         headers=...,
         files=...,
         stream: bool = ...,
         request_id: Optional[str] = ...,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = ...,
-    ) -> Tuple[Union[AikoAIResponse, Iterator[AikoAIResponse]], bool, str]:
+    ) -> Tuple[Union[OpenAIResponse, Iterator[OpenAIResponse]], bool, str]:
         pass
 
     def request(
         self,
         method,
         url,
         params=None,
         headers=None,
         files=None,
         stream: bool = False,
         request_id: Optional[str] = None,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = None,
-    ) -> Tuple[Union[AikoAIResponse, Iterator[AikoAIResponse]], bool, str]:
+    ) -> Tuple[Union[OpenAIResponse, Iterator[OpenAIResponse]], bool, str]:
         result = self.request_raw(
             method.lower(),
             url,
             params=params,
             supplied_headers=headers,
             files=files,
             stream=stream,
@@ -237,71 +237,71 @@
         url,
         params,
         headers,
         files,
         stream: Literal[True],
         request_id: Optional[str] = ...,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = ...,
-    ) -> Tuple[AsyncGenerator[AikoAIResponse, None], bool, str]:
+    ) -> Tuple[AsyncGenerator[OpenAIResponse, None], bool, str]:
         pass
 
     @overload
     async def arequest(
         self,
         method,
         url,
         params=...,
         headers=...,
         files=...,
         *,
         stream: Literal[True],
         request_id: Optional[str] = ...,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = ...,
-    ) -> Tuple[AsyncGenerator[AikoAIResponse, None], bool, str]:
+    ) -> Tuple[AsyncGenerator[OpenAIResponse, None], bool, str]:
         pass
 
     @overload
     async def arequest(
         self,
         method,
         url,
         params=...,
         headers=...,
         files=...,
         stream: Literal[False] = ...,
         request_id: Optional[str] = ...,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = ...,
-    ) -> Tuple[AikoAIResponse, bool, str]:
+    ) -> Tuple[OpenAIResponse, bool, str]:
         pass
 
     @overload
     async def arequest(
         self,
         method,
         url,
         params=...,
         headers=...,
         files=...,
         stream: bool = ...,
         request_id: Optional[str] = ...,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = ...,
-    ) -> Tuple[Union[AikoAIResponse, AsyncGenerator[AikoAIResponse, None]], bool, str]:
+    ) -> Tuple[Union[OpenAIResponse, AsyncGenerator[OpenAIResponse, None]], bool, str]:
         pass
 
     async def arequest(
         self,
         method,
         url,
         params=None,
         headers=None,
         files=None,
         stream: bool = False,
         request_id: Optional[str] = None,
         request_timeout: Optional[Union[float, Tuple[float, float]]] = None,
-    ) -> Tuple[Union[AikoAIResponse, AsyncGenerator[AikoAIResponse, None]], bool, str]:
+    ) -> Tuple[Union[OpenAIResponse, AsyncGenerator[OpenAIResponse, None]], bool, str]:
         ctx = aiohttp_session()
         session = await ctx.__aenter__()
         try:
             result = await self.arequest_raw(
                 method.lower(),
                 url,
                 session,
@@ -342,15 +342,15 @@
                 resp,
             )
 
         if "internal_message" in error_data:
             error_data["message"] += "\n\n" + error_data["internal_message"]
 
         util.log_info(
-            "AikoAI API error received",
+            "OpenAI API error received",
             error_code=error_data.get("code"),
             error_type=error_data.get("type"),
             error_message=error_data.get("message"),
             error_param=error_data.get("param"),
             stream_error=stream_error,
         )
 
@@ -407,36 +407,36 @@
         )
         ua = {
             "bindings_version": version.VERSION,
             "httplib": "requests",
             "lang": "python",
             "lang_version": platform.python_version(),
             "platform": platform.platform(),
-            "publisher": "aikoai",
+            "publisher": "openai",
             "uname": uname_without_node,
         }
         if aikoai.app_info:
             ua["application"] = aikoai.app_info
 
         headers = {
-            "X-AikoAI-Client-User-Agent": json.dumps(ua),
+            "X-OpenAI-Client-User-Agent": json.dumps(ua),
             "User-Agent": user_agent,
         }
 
         headers.update(util.api_key_to_header(self.api_type, self.api_key))
 
         if self.organization:
-            headers["AikoAI-Organization"] = self.organization
+            headers["OpenAI-Organization"] = self.organization
 
         if self.api_version is not None and self.api_type == ApiType.OPEN_AI:
-            headers["AikoAI-Version"] = self.api_version
+            headers["OpenAI-Version"] = self.api_version
         if request_id is not None:
             headers["X-Request-Id"] = request_id
         if aikoai.debug:
-            headers["AikoAI-Debug"] = "true"
+            headers["OpenAI-Debug"] = "true"
         headers.update(extra)
 
         return headers
 
     def _validate_headers(
         self, supplied_headers: Optional[Dict[str, str]]
     ) -> Dict[str, str]:
@@ -483,21 +483,21 @@
                 data = params
             if params and not files:
                 data = json.dumps(params).encode()
                 headers["Content-Type"] = "application/json"
         else:
             raise error.APIConnectionError(
                 "Unrecognized HTTP method %r. This may indicate a bug in the "
-                "AikoAI bindings. Please contact us through our help center at help.aikocute.tech for "
+                "AikoAI bindings. Please contact us through our help center at help.aikocute.tech"
                 "assistance." % (method,)
             )
 
         headers = self.request_headers(method, headers, request_id)
 
-        util.log_debug("Request to AikoAI API", method=method, path=abs_url)
+        util.log_debug("Request to OpenAI API", method=method, path=abs_url)
         util.log_debug("Post details", data=data, api_version=self.api_version)
 
         return abs_url, headers, data
 
     def request_raw(
         self,
         method,
@@ -527,21 +527,21 @@
                 timeout=request_timeout if request_timeout else TIMEOUT_SECS,
                 proxies=_thread_context.session.proxies,
             )
         except requests.exceptions.Timeout as e:
             raise error.Timeout("Request timed out: {}".format(e)) from e
         except requests.exceptions.RequestException as e:
             raise error.APIConnectionError(
-                "Error communicating with AikoAI: {}".format(e)
+                "Error communicating with OpenAI: {}".format(e)
             ) from e
         util.log_debug(
-            "AikoAI API response",
+            "OpenAI API response",
             path=abs_url,
             response_code=result.status_code,
-            processing_ms=result.headers.get("AikoAI-Processing-Ms"),
+            processing_ms=result.headers.get("OpenAI-Processing-Ms"),
             request_id=result.headers.get("X-Request-Id"),
         )
         # Don't read the whole stream for debug logging unless necessary.
         if aikoai.log == "debug":
             util.log_debug(
                 "API response body", body=result.content, headers=result.headers
             )
@@ -587,34 +587,34 @@
             "data": data,
             "proxy": _aiohttp_proxies_arg(aikoai.proxy),
             "timeout": timeout,
         }
         try:
             result = await session.request(**request_kwargs)
             util.log_info(
-                "AikoAI API response",
+                "OpenAI API response",
                 path=abs_url,
                 response_code=result.status,
-                processing_ms=result.headers.get("AikoAI-Processing-Ms"),
+                processing_ms=result.headers.get("OpenAI-Processing-Ms"),
                 request_id=result.headers.get("X-Request-Id"),
             )
             # Don't read the whole stream for debug logging unless necessary.
             if aikoai.log == "debug":
                 util.log_debug(
                     "API response body", body=result.content, headers=result.headers
                 )
             return result
         except (aiohttp.ServerTimeoutError, asyncio.TimeoutError) as e:
             raise error.Timeout("Request timed out") from e
         except aiohttp.ClientError as e:
-            raise error.APIConnectionError("Error communicating with AikoAI") from e
+            raise error.APIConnectionError("Error communicating with OpenAI") from e
 
     def _interpret_response(
         self, result: requests.Response, stream: bool
-    ) -> Tuple[Union[AikoAIResponse, Iterator[AikoAIResponse]], bool]:
+    ) -> Tuple[Union[OpenAIResponse, Iterator[OpenAIResponse]], bool]:
         """Returns the response(s) and a bool indicating whether it is a stream."""
         if stream and "text/event-stream" in result.headers.get("Content-Type", ""):
             return (
                 self._interpret_response_line(
                     line, result.status_code, result.headers, stream=True
                 )
                 for line in parse_stream(result.iter_lines())
@@ -628,15 +628,15 @@
                     stream=False,
                 ),
                 False,
             )
 
     async def _interpret_async_response(
         self, result: aiohttp.ClientResponse, stream: bool
-    ) -> Tuple[Union[AikoAIResponse, AsyncGenerator[AikoAIResponse, None]], bool]:
+    ) -> Tuple[Union[OpenAIResponse, AsyncGenerator[OpenAIResponse, None]], bool]:
         """Returns the response(s) and a bool indicating whether it is a stream."""
         if stream and "text/event-stream" in result.headers.get("Content-Type", ""):
             return (
                 self._interpret_response_line(
                     line, result.status, result.headers, stream=True
                 )
                 async for line in parse_stream_async(result.content)
@@ -654,18 +654,18 @@
                     stream=False,
                 ),
                 False,
             )
 
     def _interpret_response_line(
         self, rbody: str, rcode: int, rheaders, stream: bool
-    ) -> AikoAIResponse:
+    ) -> OpenAIResponse:
         # HTTP 204 response code does not have any content in the body.
         if rcode == 204:
-            return AikoAIResponse(None, rheaders)
+            return OpenAIResponse(None, rheaders)
 
         if rcode == 503:
             raise error.ServiceUnavailableError(
                 "The server is overloaded or not ready yet.",
                 rbody,
                 rcode,
                 headers=rheaders,
@@ -675,15 +675,15 @@
                 data = rbody
             else:
                 data = json.loads(rbody)
         except (JSONDecodeError, UnicodeDecodeError) as e:
             raise error.APIError(
                 f"HTTP code {rcode} from API ({rbody})", rbody, rcode, headers=rheaders
             ) from e
-        resp = AikoAIResponse(data, rheaders)
+        resp = OpenAIResponse(data, rheaders)
         # In the future, we might add a "status" parameter to errors
         # to better handle the "error while streaming" case.
         stream_error = stream and "error" in resp.data
         if stream_error or not 200 <= rcode < 300:
             raise self.handle_error_response(
                 rbody, rcode, resp.data, rheaders, stream_error=stream_error
             )
```

### Comparing `aikoai-1.1/aikoai/api_resources/__init__.py` & `aikoai-2.1/aikoai/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/api_resources/abstract/__init__.py` & `aikoai-2.1/aikoai/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/api_resources/abstract/api_resource.py` & `aikoai-2.1/aikoai/api_resources/abstract/api_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from urllib.parse import quote_plus
 
 import aikoai
 from aikoai import api_requestor, error, util
-from aikoai.aikoai_object import AikoAIObject
+from aikoai.aikoai_object import OpenAIObject
 from aikoai.util import ApiType
 from typing import Optional
 
 
-class APIResource(AikoAIObject):
+class APIResource(OpenAIObject):
     api_prefix = ""
-    azure_api_prefix = "aikoai"
+    azure_api_prefix = "openai"
     azure_deployments_prefix = "deployments"
 
     @classmethod
     def retrieve(
         cls, id, api_key=None, request_id=None, request_timeout=None, **params
     ):
         instance = cls(id=id, api_key=api_key, **params)
@@ -126,15 +126,15 @@
             organization=organization,
             api_base=api_base,
             api_type=api_type,
         )
         response, _, api_key = requestor.request(
             method_, url_, params, request_id=request_id
         )
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     async def _astatic_request(
         cls,
         method_,
```

### Comparing `aikoai-1.1/aikoai/api_resources/abstract/createable_api_resource.py` & `aikoai-2.1/aikoai/api_resources/abstract/createable_api_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             organization,
         )
 
         response, _, api_key = requestor.request(
             "post", url, params, request_id=request_id
         )
 
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response,
             api_key,
             api_version,
             organization,
             plain_old_data=cls.plain_old_data,
         )
 
@@ -85,14 +85,14 @@
             organization,
         )
 
         response, _, api_key = await requestor.arequest(
             "post", url, params, request_id=request_id
         )
 
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response,
             api_key,
             api_version,
             organization,
             plain_old_data=cls.plain_old_data,
         )
```

### Comparing `aikoai-1.1/aikoai/api_resources/abstract/deletable_api_resource.py` & `aikoai-2.1/aikoai/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/api_resources/abstract/engine_api_resource.py` & `aikoai-2.1/aikoai/api_resources/abstract/engine_api_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pydoc import apropos
 from typing import Optional
 from urllib.parse import quote_plus
 
 import aikoai
 from aikoai import api_requestor, error, util
 from aikoai.api_resources.abstract.api_resource import APIResource
-from aikoai.aikoai_response import AikoAIResponse
+from aikoai.aikoai_response import OpenAIResponse
 from aikoai.util import ApiType
 
 MAX_TIMEOUT = 20
 
 
 class EngineAPIResource(APIResource):
     plain_old_data = False
@@ -35,15 +35,15 @@
         if typed_api_type in (ApiType.AZURE, ApiType.AZURE_AD):
             if not api_version:
                 raise error.InvalidRequestError(
                     "An API version is required for the Azure API type."
                 )
             if engine is None:
                 raise error.InvalidRequestError(
-                    "You must provide the deployment name in the 'engine' parameter to access the Azure AikoAI service"
+                    "You must provide the deployment name in the 'engine' parameter to access the Azure OpenAI service"
                 )
             extn = quote_plus(engine)
             return "/%s/%s/%s/%s?api-version=%s" % (
                 cls.azure_api_prefix,
                 cls.azure_deployments_prefix,
                 extn,
                 base,
@@ -158,28 +158,28 @@
             stream=stream,
             request_id=request_id,
             request_timeout=request_timeout,
         )
 
         if stream:
             # must be an iterator
-            assert not isinstance(response, AikoAIResponse)
+            assert not isinstance(response, OpenAIResponse)
             return (
-                util.convert_to_aikoai_object(
+                util.convert_to_aikoai_response(
                     line,
                     api_key,
                     api_version,
                     organization,
                     engine=engine,
                     plain_old_data=cls.plain_old_data,
                 )
                 for line in response
             )
         else:
-            obj = util.convert_to_aikoai_object(
+            obj = util.convert_to_aikoai_response(
                 response,
                 api_key,
                 api_version,
                 organization,
                 engine=engine,
                 plain_old_data=cls.plain_old_data,
             )
@@ -222,28 +222,28 @@
             stream=stream,
             request_id=request_id,
             request_timeout=request_timeout,
         )
 
         if stream:
             # must be an iterator
-            assert not isinstance(response, AikoAIResponse)
+            assert not isinstance(response, OpenAIResponse)
             return (
-                util.convert_to_aikoai_object(
+                util.convert_to_aikoai_response(
                     line,
                     api_key,
                     api_version,
                     organization,
                     engine=engine,
                     plain_old_data=cls.plain_old_data,
                 )
                 async for line in response
             )
         else:
-            obj = util.convert_to_aikoai_object(
+            obj = util.convert_to_aikoai_response(
                 response,
                 api_key,
                 api_version,
                 organization,
                 engine=engine,
                 plain_old_data=cls.plain_old_data,
             )
```

### Comparing `aikoai-1.1/aikoai/api_resources/abstract/listable_api_resource.py` & `aikoai-2.1/aikoai/api_resources/abstract/listable_api_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,19 +56,19 @@
             api_base,
             api_type,
         )
 
         response, _, api_key = requestor.request(
             "get", url, params, request_id=request_id
         )
-        aikoai_object = util.convert_to_aikoai_object(
+        aikoai_response = util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
-        aikoai_object._retrieve_params = params
-        return aikoai_object
+        aikoai_response._retrieve_params = params
+        return aikoai_response
 
     @classmethod
     async def alist(
         cls,
         api_key=None,
         request_id=None,
         api_version=None,
@@ -84,12 +84,12 @@
             api_base,
             api_type,
         )
 
         response, _, api_key = await requestor.arequest(
             "get", url, params, request_id=request_id
         )
-        aikoai_object = util.convert_to_aikoai_object(
+        aikoai_response = util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
-        aikoai_object._retrieve_params = params
-        return aikoai_object
+        aikoai_response._retrieve_params = params
+        return aikoai_response
```

### Comparing `aikoai-1.1/aikoai/api_resources/abstract/nested_resource_class_methods.py` & `aikoai-2.1/aikoai/api_resources/abstract/nested_resource_class_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         ):
             requestor = api_requestor.APIRequestor(
                 api_key, api_version=api_version, organization=organization
             )
             response, _, api_key = requestor.request(
                 method, url, params, request_id=request_id
             )
-            return util.convert_to_aikoai_object(
+            return util.convert_to_aikoai_response(
                 response, api_key, api_version, organization
             )
 
         async def anested_resource_request(
             cls,
             method,
             url,
@@ -59,15 +59,15 @@
         ):
             requestor = api_requestor.APIRequestor(
                 api_key, api_version=api_version, organization=organization
             )
             response, _, api_key = await requestor.arequest(
                 method, url, params, request_id=request_id
             )
-            return util.convert_to_aikoai_object(
+            return util.convert_to_aikoai_response(
                 response, api_key, api_version, organization
             )
 
         resource_request_method = "%ss_request" % resource
         setattr(
             cls,
             resource_request_method,
```

### Comparing `aikoai-1.1/aikoai/api_resources/abstract/updateable_api_resource.py` & `aikoai-2.1/aikoai/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/api_resources/audio.py` & `aikoai-2.1/aikoai/api_resources/audio.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             api_key=api_key,
             api_base=api_base,
             api_type=api_type,
             **params,
         )
         url = cls._get_url("transcriptions")
         response, _, api_key = requestor.request("post", url, files=files, params=data)
-        return util.convert_to_aikoaii_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     def translate(
         cls,
         model,
@@ -86,15 +86,15 @@
             api_key=api_key,
             api_base=api_base,
             api_type=api_type,
             **params,
         )
         url = cls._get_url("translations")
         response, _, api_key = requestor.request("post", url, files=files, params=data)
-        return util.convert_to_aikoaii_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     def transcribe_raw(
         cls,
         model,
@@ -114,15 +114,15 @@
             api_key=api_key,
             api_base=api_base,
             api_type=api_type,
             **params,
         )
         url = cls._get_url("transcriptions")
         response, _, api_key = requestor.request("post", url, files=files, params=data)
-        return util.convert_to_aikoaii_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     def translate_raw(
         cls,
         model,
@@ -142,15 +142,15 @@
             api_key=api_key,
             api_base=api_base,
             api_type=api_type,
             **params,
         )
         url = cls._get_url("translations")
         response, _, api_key = requestor.request("post", url, files=files, params=data)
-        return util.convert_to_aikoaii_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     async def atranscribe(
         cls,
         model,
@@ -171,15 +171,15 @@
             api_type=api_type,
             **params,
         )
         url = cls._get_url("transcriptions")
         response, _, api_key = await requestor.arequest(
             "post", url, files=files, params=data
         )
-        return util.convert_to_aikoaii_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     async def atranslate(
         cls,
         model,
@@ -200,15 +200,15 @@
             api_type=api_type,
             **params,
         )
         url = cls._get_url("translations")
         response, _, api_key = await requestor.arequest(
             "post", url, files=files, params=data
         )
-        return util.convert_to_aikoaii_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     async def atranscribe_raw(
         cls,
         model,
@@ -230,15 +230,15 @@
             api_type=api_type,
             **params,
         )
         url = cls._get_url("transcriptions")
         response, _, api_key = await requestor.arequest(
             "post", url, files=files, params=data
         )
-        return util.convert_to_aikoaii_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     async def atranslate_raw(
         cls,
         model,
@@ -260,10 +260,10 @@
             api_type=api_type,
             **params,
         )
         url = cls._get_url("translations")
         response, _, api_key = await requestor.arequest(
             "post", url, files=files, params=data
         )
-        return util.convert_to_aikoaii_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
```

### Comparing `aikoai-1.1/aikoai/api_resources/chat_completion.py` & `aikoai-2.1/aikoai/api_resources/completion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import time
 
 from aikoai import util
+from aikoai.api_resources.abstract import DeletableAPIResource, ListableAPIResource
 from aikoai.api_resources.abstract.engine_api_resource import EngineAPIResource
 from aikoai.error import TryAgain
 
 
-class ChatCompletion(EngineAPIResource):
-    engine_required = False
-    OBJECT_NAME = "chat.completions"
+class Completion(EngineAPIResource):
+    OBJECT_NAME = "completions"
 
     @classmethod
     def create(cls, *args, **kwargs):
         """
-        Creates a new chat completion for the provided messages and parameters.
+        Creates a new completion for the provided prompt and parameters.
 
-        See https://platform.aikocute.tech/docs/api-reference/chat-completions/create
-        for a list of valid parameters.
+        See https://platform.openai.com/docs/api-reference/completions/create for a list
+        of valid parameters.
         """
         start = time.time()
         timeout = kwargs.pop("timeout", None)
 
         while True:
             try:
                 return super().create(*args, **kwargs)
@@ -28,18 +28,18 @@
                     raise
 
                 util.log_info("Waiting for model to warm up", error=e)
 
     @classmethod
     async def acreate(cls, *args, **kwargs):
         """
-        Creates a new chat completion for the provided messages and parameters.
+        Creates a new completion for the provided prompt and parameters.
 
-        See https://platform.aikocute.tech/docs/api-reference/chat-completions/create
-        for a list of valid parameters.
+        See https://platform.openai.com/docs/api-reference/completions/create for a list
+        of valid parameters.
         """
         start = time.time()
         timeout = kwargs.pop("timeout", None)
 
         while True:
             try:
                 return await super().acreate(*args, **kwargs)
```

### Comparing `aikoai-1.1/aikoai/api_resources/completion.py` & `aikoai-2.1/aikoai/api_resources/chat_completion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import time
 
 from aikoai import util
-from aikoai.api_resources.abstract import DeletableAPIResource, ListableAPIResource
 from aikoai.api_resources.abstract.engine_api_resource import EngineAPIResource
 from aikoai.error import TryAgain
 
 
-class Completion(EngineAPIResource):
-    OBJECT_NAME = "completions"
+class ChatCompletion(EngineAPIResource):
+    engine_required = False
+    OBJECT_NAME = "chat.completions"
 
     @classmethod
     def create(cls, *args, **kwargs):
         """
-        Creates a new completion for the provided prompt and parameters.
+        Creates a new chat completion for the provided messages and parameters.
 
-        See https://platform.aikocute.tech/docs/api-reference/completions/create for a list
-        of valid parameters.
+        See https://platform.openai.com/docs/api-reference/chat-completions/create
+        for a list of valid parameters.
         """
         start = time.time()
         timeout = kwargs.pop("timeout", None)
 
         while True:
             try:
                 return super().create(*args, **kwargs)
@@ -28,18 +28,18 @@
                     raise
 
                 util.log_info("Waiting for model to warm up", error=e)
 
     @classmethod
     async def acreate(cls, *args, **kwargs):
         """
-        Creates a new completion for the provided prompt and parameters.
+        Creates a new chat completion for the provided messages and parameters.
 
-        See https://platform.aikocute.tech/docs/api-reference/completions/create for a list
-        of valid parameters.
+        See https://platform.openai.com/docs/api-reference/chat-completions/create
+        for a list of valid parameters.
         """
         start = time.time()
         timeout = kwargs.pop("timeout", None)
 
         while True:
             try:
                 return await super().acreate(*args, **kwargs)
```

### Comparing `aikoai-1.1/aikoai/api_resources/customer.py` & `aikoai-2.1/aikoai/api_resources/customer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from aikoai.aikoai_object import AikoAIObject
+from aikoai.aikoai_object import OpenAIObject
 
 
-class Customer(AikoAIObject):
+class Customer(OpenAIObject):
     @classmethod
     def get_url(cls, customer, endpoint):
         return f"/customer/{customer}/{endpoint}"
 
     @classmethod
     def create(cls, customer, endpoint, **params):
         instance = cls()
```

### Comparing `aikoai-1.1/aikoai/api_resources/deployment.py` & `aikoai-2.1/aikoai/api_resources/deployment.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/api_resources/edit.py` & `aikoai-2.1/aikoai/api_resources/edit.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         start = time.time()
         timeout = kwargs.pop("timeout", None)
 
         api_type = kwargs.pop("api_type", None)
         typed_api_type = cls._get_api_type_and_version(api_type=api_type)[0]
         if typed_api_type in (util.ApiType.AZURE, util.ApiType.AZURE_AD):
             raise error.InvalidAPIType(
-                "This operation is not supported by the Azure AikoAI API yet."
+                "This operation is not supported by the Azure OpenAI API yet."
             )
 
         while True:
             try:
                 return super().create(*args, **kwargs)
             except TryAgain as e:
                 if timeout is not None and time.time() > start + timeout:
@@ -40,15 +40,15 @@
         start = time.time()
         timeout = kwargs.pop("timeout", None)
 
         api_type = kwargs.pop("api_type", None)
         typed_api_type = cls._get_api_type_and_version(api_type=api_type)[0]
         if typed_api_type in (util.ApiType.AZURE, util.ApiType.AZURE_AD):
             raise error.InvalidAPIType(
-                "This operation is not supported by the Azure AikoAI API yet."
+                "This operation is not supported by the Azure OpenAI API yet."
             )
 
         while True:
             try:
                 return await super().acreate(*args, **kwargs)
             except TryAgain as e:
                 if timeout is not None and time.time() > start + timeout:
```

### Comparing `aikoai-1.1/aikoai/api_resources/embedding.py` & `aikoai-2.1/aikoai/api_resources/embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     OBJECT_NAME = "embeddings"
 
     @classmethod
     def create(cls, *args, **kwargs):
         """
         Creates a new embedding for the provided input and parameters.
 
-        See https://platform.aikocute.tech/docs/api-reference/embeddings for a list
+        See https://platform.openai.com/docs/api-reference/embeddings for a list
         of valid parameters.
         """
         start = time.time()
         timeout = kwargs.pop("timeout", None)
 
         user_provided_encoding_format = kwargs.get("encoding_format", None)
 
@@ -52,15 +52,15 @@
                 util.log_info("Waiting for model to warm up", error=e)
 
     @classmethod
     async def acreate(cls, *args, **kwargs):
         """
         Creates a new embedding for the provided input and parameters.
 
-        See https://platform.aikocute.tech/docs/api-reference/embeddings for a list
+        See https://platform.openai.com/docs/api-reference/embeddings for a list
         of valid parameters.
         """
         start = time.time()
         timeout = kwargs.pop("timeout", None)
 
         user_provided_encoding_format = kwargs.get("encoding_format", None)
```

### Comparing `aikoai-1.1/aikoai/api_resources/engine.py` & `aikoai-2.1/aikoai/api_resources/engine.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/api_resources/error_object.py` & `aikoai-2.1/aikoai/api_resources/error_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
-from aikoai.aikoai_object import AikoAIObject
+from aikoai.aikoai_object import OpenAIObject
 from aikoai.util import merge_dicts
 
 
-class ErrorObject(AikoAIObject):
+class ErrorObject(OpenAIObject):
     def refresh_from(
         self,
         values,
         api_key=None,
         api_version=None,
         api_type=None,
         organization=None,
```

### Comparing `aikoai-1.1/aikoai/api_resources/file.py` & `aikoai-2.1/aikoai/api_resources/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             api_base,
             api_type,
             api_version,
             organization,
             user_provided_filename,
         )
         response, _, api_key = requestor.request("post", url, files=files)
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     async def acreate(
         cls,
         file,
@@ -107,15 +107,15 @@
             api_base,
             api_type,
             api_version,
             organization,
             user_provided_filename,
         )
         response, _, api_key = await requestor.arequest("post", url, files=files)
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     def __prepare_file_download(
         cls,
         id,
```

### Comparing `aikoai-1.1/aikoai/api_resources/fine_tune.py` & `aikoai-2.1/aikoai/api_resources/fine_tune.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from aikoai import api_requestor, util, error
 from aikoai.api_resources.abstract import (
     CreateableAPIResource,
     ListableAPIResource,
     nested_resource_class_methods,
 )
 from aikoai.api_resources.abstract.deletable_api_resource import DeletableAPIResource
-from aikoai.aikoai_response import AikoAIResponse
+from aikoai.aikoai_response import OpenAIResponse
 from aikoai.util import ApiType
 
 
 @nested_resource_class_methods("event", operations=["list"])
 class FineTune(ListableAPIResource, CreateableAPIResource, DeletableAPIResource):
     OBJECT_NAME = "fine-tunes"
 
@@ -150,17 +150,17 @@
             **params,
         )
 
         response, _, api_key = requestor.request(
             "get", url, params, stream=True, request_id=request_id
         )
 
-        assert not isinstance(response, AikoAIResponse)  # must be an iterator
+        assert not isinstance(response, OpenAIResponse)  # must be an iterator
         return (
-            util.convert_to_aikoai_object(
+            util.convert_to_aikoai_response(
                 line,
                 api_key,
                 api_version,
                 organization,
             )
             for line in response
         )
@@ -188,17 +188,17 @@
             **params,
         )
 
         response, _, api_key = await requestor.arequest(
             "get", url, params, stream=True, request_id=request_id
         )
 
-        assert not isinstance(response, AikoAIResponse)  # must be an iterator
+        assert not isinstance(response, OpenAIResponse)  # must be an iterator
         return (
-            util.convert_to_aikoai_object(
+            util.convert_to_aikoai_response(
                 line,
                 api_key,
                 api_version,
                 organization,
             )
             async for line in response
         )
```

### Comparing `aikoai-1.1/aikoai/api_resources/image.py` & `aikoai-2.1/aikoai/api_resources/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         _, api_version = cls._get_api_type_and_version(api_type, api_version)
 
         response, _, api_key = requestor.request(
             "post", cls._get_url("generations"), params
         )
 
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     async def acreate(
         cls,
         api_key=None,
@@ -62,15 +62,15 @@
 
         _, api_version = cls._get_api_type_and_version(api_type, api_version)
 
         response, _, api_key = await requestor.arequest(
             "post", cls._get_url("generations"), params
         )
 
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     def _prepare_create_variation(
         cls,
         image,
@@ -117,15 +117,15 @@
             api_version,
             organization,
             **params,
         )
 
         response, _, api_key = requestor.request("post", url, files=files)
 
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     async def acreate_variation(
         cls,
         image,
@@ -144,15 +144,15 @@
             api_version,
             organization,
             **params,
         )
 
         response, _, api_key = await requestor.arequest("post", url, files=files)
 
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     def _prepare_create_edit(
         cls,
         image,
@@ -204,15 +204,15 @@
             api_version,
             organization,
             **params,
         )
 
         response, _, api_key = requestor.request("post", url, files=files)
 
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
 
     @classmethod
     async def acreate_edit(
         cls,
         image,
@@ -233,10 +233,10 @@
             api_version,
             organization,
             **params,
         )
 
         response, _, api_key = await requestor.arequest("post", url, files=files)
 
-        return util.convert_to_aikoai_object(
+        return util.convert_to_aikoai_response(
             response, api_key, api_version, organization
         )
```

### Comparing `aikoai-1.1/aikoai/api_resources/moderation.py` & `aikoai-2.1/aikoai/api_resources/moderation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional, Union
 
-from aikoai.aikoai_object import AikoAIObject
+from aikoai.aikoai_object import OpenAIObject
 
 
-class Moderation(AikoAIObject):
+class Moderation(OpenAIObject):
     VALID_MODEL_NAMES: List[str] = ["text-moderation-stable", "text-moderation-latest"]
 
     @classmethod
     def get_url(cls):
         return "/moderations"
 
     @classmethod
```

### Comparing `aikoai-1.1/aikoai/cli.py` & `aikoai-2.1/aikoai/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     @classmethod
     def generate(cls, args):
         warnings.warn(
             "Engine.generate is deprecated, use Completion.create", DeprecationWarning
         )
         if args.completions and args.completions > 1 and args.stream:
-            raise ValueError("Can't stream multiple completions with AikoAI CLI")
+            raise ValueError("Can't stream multiple completions with openai CLI")
 
         kwargs = {}
         if args.model is not None:
             kwargs["model"] = args.model
         resp = aikoai.Engine(id=args.id).generate(
             completions=args.completions,
             context=args.context,
@@ -496,19 +496,19 @@
         result_file = aikoai.FineTune.retrieve(id=args.id)["result_files"][0]
         resp = aikoai.File.download(id=result_file["id"])
         print(resp.decode("utf-8"))
 
     @classmethod
     def events(cls, args):
         if args.stream:
-            raise aikoai.error.AikoAIError(
+            raise aikoai.error.OpenAIError(
                 message=(
                     "The --stream parameter is deprecated, use fine_tunes.follow "
                     "instead:\n\n"
-                    "  aikoai api fine_tunes.follow -i {id}\n".format(id=args.id)
+                    "  openai api fine_tunes.follow -i {id}\n".format(id=args.id)
                 ),
             )
 
         resp = aikoai.FineTune.list_events(id=args.id)  # type: ignore
         print(resp)
 
     @classmethod
@@ -518,17 +518,17 @@
     @classmethod
     def _stream_events(cls, job_id):
         def signal_handler(sig, frame):
             status = aikoai.FineTune.retrieve(job_id).status
             sys.stdout.write(
                 "\nStream interrupted. Job is still {status}.\n"
                 "To resume the stream, run:\n\n"
-                "  aikoai api fine_tunes.follow -i {job_id}\n\n"
+                "  openai api fine_tunes.follow -i {job_id}\n\n"
                 "To cancel your job, run:\n\n"
-                "  aikoai api fine_tunes.cancel -i {job_id}\n\n".format(
+                "  openai api fine_tunes.cancel -i {job_id}\n\n".format(
                     status=status, job_id=job_id
                 )
             )
             sys.exit(0)
 
         signal.signal(signal.SIGINT, signal_handler)
 
@@ -545,31 +545,31 @@
                 )
                 sys.stdout.write("\n")
                 sys.stdout.flush()
         except Exception:
             sys.stdout.write(
                 "\nStream interrupted (client disconnected).\n"
                 "To resume the stream, run:\n\n"
-                "  aikoai api fine_tunes.follow -i {job_id}\n\n".format(job_id=job_id)
+                "  openai api fine_tunes.follow -i {job_id}\n\n".format(job_id=job_id)
             )
             return
 
         resp = aikoai.FineTune.retrieve(id=job_id)
         status = resp["status"]
         if status == "succeeded":
             sys.stdout.write("\nJob complete! Status: succeeded 🎉")
             sys.stdout.write(
                 "\nTry out your fine-tuned model:\n\n"
-                "aikoai api completions.create -m {model} -p <YOUR_PROMPT>".format(
+                "openai api completions.create -m {model} -p <YOUR_PROMPT>".format(
                     model=resp["fine_tuned_model"]
                 )
             )
         elif status == "failed":
             sys.stdout.write(
-                "\nJob failed. Please contact us through our help center at help.aikoai.com if you need assistance."
+                "\nJob failed. Please contact us through our help center at help.aikocute.techif you need assistance."
             )
         sys.stdout.write("\n")
 
     @classmethod
     def cancel(cls, args):
         resp = aikoai.FineTune.cancel(id=args.id)
         print(resp)
@@ -725,15 +725,15 @@
         required=True,
     )
 
     group = opt.add_mutually_exclusive_group()
     group.add_argument(
         "-e",
         "--engine",
-        help="The engine to use. See https://learn.microsoft.com/en-us/azure/cognitive-services/aikoai/chatgpt-quickstart?pivots=programming-language-python for more about what engines are available.",
+        help="The engine to use. See https://learn.microsoft.com/en-us/azure/cognitive-services/openai/chatgpt-quickstart?pivots=programming-language-python for more about what engines are available.",
     )
     group.add_argument(
         "-m",
         "--model",
         help="The model to use.",
     )
 
@@ -772,15 +772,15 @@
     sub.set_defaults(func=ChatCompletion.create)
 
     # Completions
     sub = subparsers.add_parser("completions.create")
     sub.add_argument(
         "-e",
         "--engine",
-        help="The engine to use. See https://platform.aikocute.tech/docs/engines for more about what engines are available.",
+        help="The engine to use. See https://platform.openai.com/docs/engines for more about what engines are available.",
     )
     sub.add_argument(
         "-m",
         "--model",
         help="The model to use. At most one of `engine` or `model` should be specified.",
     )
     sub.add_argument(
@@ -859,15 +859,15 @@
         "--file",
         required=True,
         help="File to upload",
     )
     sub.add_argument(
         "-p",
         "--purpose",
-        help="Why are you uploading this file? (see https://platform.aikoai.com/docs/api-reference/ for purposes)",
+        help="Why are you uploading this file? (see https://platform.openai.com/docs/api-reference/ for purposes)",
         required=True,
     )
     sub.set_defaults(func=File.create)
 
     sub = subparsers.add_parser("files.get")
     sub.add_argument("-i", "--id", required=True, help="The files ID")
     sub.set_defaults(func=File.get)
@@ -885,22 +885,22 @@
 
     sub = subparsers.add_parser("fine_tunes.create")
     sub.add_argument(
         "-t",
         "--training_file",
         required=True,
         help="JSONL file containing prompt-completion examples for training. This can "
-        "be the ID of a file uploaded through the AikoAI API (e.g. file-abcde12345), "
+        "be the ID of a file uploaded through the OpenAI API (e.g. file-abcde12345), "
         'a local file path, or a URL that starts with "http".',
     )
     sub.add_argument(
         "-v",
         "--validation_file",
         help="JSONL file containing prompt-completion examples for validation. This can "
-        "be the ID of a file uploaded through the AikoAI API (e.g. file-abcde12345), "
+        "be the ID of a file uploaded through the OpenAI API (e.g. file-abcde12345), "
         'a local file path, or a URL that starts with "http".',
     )
     sub.add_argument(
         "--no_check_if_files_exist",
         dest="check_if_files_exist",
         action="store_false",
         help="If this argument is set and training_file or validation_file are file paths, immediately upload them. If this argument is not set, check if they may be duplicates of already uploaded files before uploading, based on file name and file size.",
@@ -913,15 +913,15 @@
     sub.add_argument(
         "--suffix",
         help="If set, this argument can be used to customize the generated fine-tuned model name."
         "All punctuation and whitespace in `suffix` will be replaced with a "
         "single dash, and the string will be lower cased. The max "
         "length of `suffix` is 40 chars. "
         "The generated name will match the form `{base_model}:ft-{org-title}:{suffix}-{timestamp}`. "
-        'For example, `AikoAI api fine_tunes.create -t test.jsonl -m ada --suffix "custom model name" '
+        'For example, `openai api fine_tunes.create -t test.jsonl -m ada --suffix "custom model name" '
         "could generate a model with the name "
         "ada:ft-your-org:custom-model-name-2022-02-15-04-21-04",
     )
     sub.add_argument(
         "--no_follow",
         action="store_true",
         help="If set, returns immediately after creating the job. Otherwise, streams events and waits for the job to complete.",
```

### Comparing `aikoai-1.1/aikoai/datalib/__init__.py` & `aikoai-2.1/aikoai/datalib/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 This module helps make data libraries like `numpy` and `pandas` optional dependencies.
 
 The libraries add up to 130MB+, which makes it challenging to deploy applications
 using this library in environments with code size constraints, like AWS Lambda.
 
 This module serves as an import proxy and provides a few utilities for dealing with the optionality.
 
-Since the primary use case of this library (talking to the aikoai API) doesn't generally require data libraries,
+Since the primary use case of this library (talking to the OpenAI API) doesn't generally require data libraries,
 it's safe to make them optional. The rare case when data libraries are needed in the client is handled through
 assertions with instructive error messages.
 
 See also `setup.py`.
 """
```

### Comparing `aikoai-1.1/aikoai/embeddings_utils.py` & `aikoai-2.1/aikoai/embeddings_utils.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/error.py` & `aikoai-2.1/aikoai/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import aikoai
 
 
-class AikoAIError(Exception):
+class OpenAIError(Exception):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
-        super(AikoAIError, self).__init__(message)
+        super(OpenAIError, self).__init__(message)
 
         if http_body and hasattr(http_body, "decode"):
             try:
                 http_body = http_body.decode("utf-8")
             except BaseException:
                 http_body = (
                     "<Could not decode body as utf-8. "
-                    "Please contact us through our help center at help.aikocute.tech.>"
+                    "Please contact us through our help center at help.openai.com.>"
                 )
 
         self._message = message
         self.http_body = http_body
         self.http_status = http_status
         self.json_body = json_body
         self.headers = headers or {}
         self.code = code
         self.request_id = self.headers.get("request-id", None)
         self.error = self.construct_error_object()
-        self.organization = self.headers.get("aikoai-organization", None)
+        self.organization = self.headers.get("openai-organization", None)
 
     def __str__(self):
         msg = self._message or "<empty message>"
         if self.request_id is not None:
             return "Request {0}: {1}".format(self.request_id, msg)
         else:
             return msg
 
     # Returns the underlying `Exception` (base class) message, which is usually
-    # the raw message returned by aikoai's API. This was previously available
+    # the raw message returned by OpenAI's API. This was previously available
     # in python2 via `error.message`. Unlike `str(error)`, it omits "Request
     # req_..." from the beginning of the string.
     @property
     def user_message(self):
         return self._message
 
     def __repr__(self):
@@ -65,27 +65,27 @@
             return None
 
         return aikoai.api_resources.error_object.ErrorObject.construct_from(
             self.json_body["error"]
         )
 
 
-class APIError(AikoAIError):
+class APIError(OpenAIError):
     pass
 
 
-class TryAgain(AikoAIError):
+class TryAgain(OpenAIError):
     pass
 
 
-class Timeout(AikoAIError):
+class Timeout(OpenAIError):
     pass
 
 
-class APIConnectionError(AikoAIError):
+class APIConnectionError(OpenAIError):
     def __init__(
         self,
         message,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
@@ -94,15 +94,15 @@
     ):
         super(APIConnectionError, self).__init__(
             message, http_body, http_status, json_body, headers, code
         )
         self.should_retry = should_retry
 
 
-class InvalidRequestError(AikoAIError):
+class InvalidRequestError(OpenAIError):
     def __init__(
         self,
         message,
         param,
         code=None,
         http_body=None,
         http_status=None,
@@ -132,35 +132,35 @@
             self.http_body,
             self.http_status,
             self.json_body,
             self.headers,
         )
 
 
-class AuthenticationError(AikoAIError):
+class AuthenticationError(OpenAIError):
     pass
 
 
-class PermissionError(AikoAIError):
+class PermissionError(OpenAIError):
     pass
 
 
-class RateLimitError(AikoAIError):
+class RateLimitError(OpenAIError):
     pass
 
 
-class ServiceUnavailableError(AikoAIError):
+class ServiceUnavailableError(OpenAIError):
     pass
 
 
-class InvalidAPIType(AikoAIError):
+class InvalidAPIType(OpenAIError):
     pass
 
 
-class SignatureVerificationError(AikoAIError):
+class SignatureVerificationError(OpenAIError):
     def __init__(self, message, sig_header, http_body=None):
         super(SignatureVerificationError, self).__init__(message, http_body)
         self.sig_header = sig_header
 
     def __reduce__(self):
         return type(self), (
             self._message,
```

### Comparing `aikoai-1.1/aikoai/tests/asyncio/test_endpoints.py` & `aikoai-2.1/aikoai/tests/asyncio/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/tests/test_api_requestor.py` & `aikoai-2.1/aikoai/tests/test_api_requestor.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/tests/test_endpoints.py` & `aikoai-2.1/aikoai/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/tests/test_exceptions.py` & `aikoai-2.1/aikoai/tests/test_exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         message="message",
         code=400,
         http_body={"test": "test1"},
         http_status="fail",
         json_body={"text": "iono some text"},
         headers={"request-id": "asasd"},
     ),
-    aikoai.error.AikoAIError(),
+    aikoai.error.OpenAIError(),
 ]
 
 
 class TestExceptions:
     @pytest.mark.parametrize("error", EXCEPTION_TEST_CASES)
     def test_exceptions_are_pickleable(self, error) -> None:
         assert error.__repr__() == pickle.loads(pickle.dumps(error)).__repr__()
```

### Comparing `aikoai-1.1/aikoai/tests/test_file_cli.py` & `aikoai-2.1/aikoai/tests/test_file_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 def test_file_cli() -> None:
     contents = json.dumps({"prompt": "1 + 3 =", "completion": "4"}) + "\n"
     with NamedTemporaryFile(suffix=".jsonl", mode="wb") as train_file:
         train_file.write(contents.encode("utf-8"))
         train_file.flush()
         create_output = subprocess.check_output(
-            ["aikoai", "api", "files.create", "-f", train_file.name, "-p", "fine-tune"]
+            ["openai", "api", "files.create", "-f", train_file.name, "-p", "fine-tune"]
         )
     file_obj = json.loads(create_output)
     assert file_obj["bytes"] == len(contents)
     file_id: str = file_obj["id"]
     assert file_id.startswith("file-")
     start_time = time.time()
     while True:
         delete_result = subprocess.run(
-            ["aikoai", "api", "files.delete", "-i", file_id],
+            ["openai", "api", "files.delete", "-i", file_id],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             encoding="utf-8",
         )
         if delete_result.returncode == 0:
             break
         elif STILL_PROCESSING in delete_result.stderr:
```

### Comparing `aikoai-1.1/aikoai/tests/test_long_examples_validator.py` & `aikoai-2.1/aikoai/tests/test_long_examples_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     with NamedTemporaryFile(suffix=".jsonl", mode="w") as training_data:
         print(training_data.name)
         for prompt_completion_row in unprepared_training_data:
             training_data.write(json.dumps(prompt_completion_row) + "\n")
             training_data.flush()
 
         prepared_data_cmd_output = subprocess.run(
-            [f"aikoai tools fine_tunes.prepare_data -f {training_data.name}"],
+            [f"openai tools fine_tunes.prepare_data -f {training_data.name}"],
             stdout=subprocess.PIPE,
             text=True,
             input="y\ny\ny\ny\ny",  # apply all recommendations, one at a time
             stderr=subprocess.PIPE,
             encoding="utf-8",
             shell=True,
         )
```

### Comparing `aikoai-1.1/aikoai/tests/test_url_composition.py` & `aikoai-2.1/aikoai/tests/test_url_composition.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 
 @pytest.mark.url
 def test_completions_url_composition_azure() -> None:
     url = Completion.class_url("test_engine", "azure", "2021-11-01-preview")
     assert (
         url
-        == "/aikoai/deployments/test_engine/completions?api-version=2021-11-01-preview"
+        == "/openai/deployments/test_engine/completions?api-version=2021-11-01-preview"
     )
 
 
 @pytest.mark.url
 def test_completions_url_composition_azure_ad() -> None:
     url = Completion.class_url("test_engine", "azure_ad", "2021-11-01-preview")
     assert (
         url
-        == "/aikoai/deployments/test_engine/completions?api-version=2021-11-01-preview"
+        == "/openai/deployments/test_engine/completions?api-version=2021-11-01-preview"
     )
 
 
 @pytest.mark.url
 def test_completions_url_composition_default() -> None:
     url = Completion.class_url("test_engine")
     assert url == "/engines/test_engine/completions"
@@ -49,30 +49,30 @@
         engine="test_engine",
         api_type="azure",
         api_version="2021-11-01-preview",
     )
     url = completion.instance_url()
     assert (
         url
-        == "/aikoai/deployments/test_engine/completions/test_id?api-version=2021-11-01-preview"
+        == "/openai/deployments/test_engine/completions/test_id?api-version=2021-11-01-preview"
     )
 
 
 @pytest.mark.url
 def test_completions_url_composition_instance_url_azure_ad() -> None:
     completion = Completion(
         id="test_id",
         engine="test_engine",
         api_type="azure_ad",
         api_version="2021-11-01-preview",
     )
     url = completion.instance_url()
     assert (
         url
-        == "/aikoai/deployments/test_engine/completions/test_id?api-version=2021-11-01-preview"
+        == "/openai/deployments/test_engine/completions/test_id?api-version=2021-11-01-preview"
     )
 
 
 @pytest.mark.url
 def test_completions_url_composition_instance_url_azure_no_version() -> None:
     completion = Completion(
         id="test_id", engine="test_engine", api_type="azure", api_version=None
@@ -115,47 +115,47 @@
         api_type="azure",
         api_version="2021-11-01-preview",
     )
     completion["timeout"] = 12
     url = completion.instance_url()
     assert (
         url
-        == "/aikoai/deployments/test_engine/completions/test_id?api-version=2021-11-01-preview&timeout=12"
+        == "/openai/deployments/test_engine/completions/test_id?api-version=2021-11-01-preview&timeout=12"
     )
 
 
 @pytest.mark.url
-def test_completions_url_composition_instance_url_timeout_aikoai() -> None:
+def test_completions_url_composition_instance_url_timeout_openai() -> None:
     completion = Completion(id="test_id", engine="test_engine", api_type="open_ai")
     completion["timeout"] = 12
     url = completion.instance_url()
     assert url == "/engines/test_engine/completions/test_id?timeout=12"
 
 
 @pytest.mark.url
 def test_engine_search_url_composition_azure() -> None:
     engine = Engine(id="test_id", api_type="azure", api_version="2021-11-01-preview")
     assert engine.api_type == "azure"
     assert engine.typed_api_type == ApiType.AZURE
     url = engine.instance_url("test_operation")
     assert (
         url
-        == "/aikoai/deployments/test_id/test_operation?api-version=2021-11-01-preview"
+        == "/openai/deployments/test_id/test_operation?api-version=2021-11-01-preview"
     )
 
 
 @pytest.mark.url
 def test_engine_search_url_composition_azure_ad() -> None:
     engine = Engine(id="test_id", api_type="azure_ad", api_version="2021-11-01-preview")
     assert engine.api_type == "azure_ad"
     assert engine.typed_api_type == ApiType.AZURE_AD
     url = engine.instance_url("test_operation")
     assert (
         url
-        == "/aikoai/deployments/test_id/test_operation?api-version=2021-11-01-preview"
+        == "/openai/deployments/test_id/test_operation?api-version=2021-11-01-preview"
     )
 
 
 @pytest.mark.url
 def test_engine_search_url_composition_azure_no_version() -> None:
     engine = Engine(id="test_id", api_type="azure", api_version=None)
     assert engine.api_type == "azure"
@@ -167,15 +167,15 @@
 @pytest.mark.url
 def test_engine_search_url_composition_azure_no_operation() -> None:
     engine = Engine(id="test_id", api_type="azure", api_version="2021-11-01-preview")
     assert engine.api_type == "azure"
     assert engine.typed_api_type == ApiType.AZURE
     assert (
         engine.instance_url()
-        == "/aikoai/engines/test_id?api-version=2021-11-01-preview"
+        == "/openai/engines/test_id?api-version=2021-11-01-preview"
     )
 
 
 @pytest.mark.url
 def test_engine_search_url_composition_default() -> None:
     engine = Engine(id="test_id")
     assert engine.api_type == None
```

### Comparing `aikoai-1.1/aikoai/tests/test_util.py` & `aikoai-2.1/aikoai/tests/test_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from aikoai import util
 
 
 @pytest.fixture(scope="function")
 def api_key_file():
     saved_path = aikoai.api_key_path
     try:
-        with NamedTemporaryFile(prefix="aikoai-api-key", mode="wt") as tmp:
+        with NamedTemporaryFile(prefix="openai-api-key", mode="wt") as tmp:
             aikoai.api_key_path = tmp.name
             yield tmp
     finally:
         aikoai.api_key_path = saved_path
 
 
-def test_aikoai_api_key_path(api_key_file) -> None:
+def test_openai_api_key_path(api_key_file) -> None:
     print("sk-foo", file=api_key_file)
     api_key_file.flush()
     assert util.default_api_key() == "sk-foo"
 
 
-def test_aikoai_api_key_path_with_malformed_key(api_key_file) -> None:
+def test_openai_api_key_path_with_malformed_key(api_key_file) -> None:
     print("malformed-api-key", file=api_key_file)
     api_key_file.flush()
     with pytest.raises(ValueError, match="Malformed API key"):
         util.default_api_key()
```

### Comparing `aikoai-1.1/aikoai/upload_progress.py` & `aikoai-2.1/aikoai/upload_progress.py`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/aikoai/util.py` & `aikoai-2.1/aikoai/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import re
 import sys
 from enum import Enum
 from typing import Optional
 
 import aikoai
 
-AIKOAI_LOG = os.environ.get("AIKOAI_LOG")
+OPENAI_LOG = os.environ.get("OPENAI_LOG")
 
-logger = logging.getLogger("aikoai")
+logger = logging.getLogger("openai")
 
 __all__ = [
     "log_info",
     "log_debug",
     "log_warn",
     "logfmt",
 ]
@@ -32,27 +32,27 @@
 
     @staticmethod
     def from_str(label):
         if label.lower() == "azure":
             return ApiType.AZURE
         elif label.lower() in ("azure_ad", "azuread"):
             return ApiType.AZURE_AD
-        elif label.lower() in ("open_ai", "aikoai"):
+        elif label.lower() in ("open_ai", "openai"):
             return ApiType.OPEN_AI
         else:
             raise aikoai.error.InvalidAPIType(
                 "The API type provided in invalid. Please select one of the supported API types: 'azure', 'azure_ad', 'open_ai'"
             )
 
 
 def _console_log_level():
     if aikoai.log in ["debug", "info"]:
         return aikoai.log
-    elif AIKOAI_LOG in ["debug", "info"]:
-        return AIKOAI_LOG
+    elif OPENAI_LOG in ["debug", "info"]:
+        return OPENAI_LOG
     else:
         return None
 
 
 def log_debug(message, **params):
     msg = logfmt(dict(message=message, **params))
     if _console_log_level() == "debug":
@@ -94,75 +94,75 @@
 def get_object_classes():
     # This is here to avoid a circular dependency
     from aikoai.object_classes import OBJECT_CLASSES
 
     return OBJECT_CLASSES
 
 
-def convert_to_aikoai_object(
+def convert_to_aikoai_response(
     resp,
     api_key=None,
     api_version=None,
     organization=None,
     engine=None,
     plain_old_data=False,
 ):
-    # If we get a AikoAIResponse, we'll want to return a AikoAIObject.
+    # If we get a OpenAIResponse, we'll want to return a OpenAIObject.
 
     response_ms: Optional[int] = None
-    if isinstance(resp, aikoai.aikoai_response.AikoAIResponse):
+    if isinstance(resp, aikoai.aikoai_response.OpenAIResponse):
         organization = resp.organization
         response_ms = resp.response_ms
         resp = resp.data
 
     if plain_old_data:
         return resp
     elif isinstance(resp, list):
         return [
-            convert_to_aikoai_object(
+            convert_to_aikoai_response(
                 i, api_key, api_version, organization, engine=engine
             )
             for i in resp
         ]
     elif isinstance(resp, dict) and not isinstance(
-        resp, aikoai.aikoai_object.AikoAIObject
+        resp, aikoai.aikoai_response.OpenAIObject
     ):
         resp = resp.copy()
         klass_name = resp.get("object")
         if isinstance(klass_name, str):
             klass = get_object_classes().get(
-                klass_name, aikoai.aikoai_object.AikoAIObject
+                klass_name, aikoai.aikoai_response.OpenAIObject
             )
         else:
-            klass = aikoai.aikoai_object.AikoAIObject
+            klass = aikoai.aikoai_response.OpenAIObject
 
         return klass.construct_from(
             resp,
             api_key=api_key,
             api_version=api_version,
             organization=organization,
             response_ms=response_ms,
             engine=engine,
         )
     else:
         return resp
 
 
 def convert_to_dict(obj):
-    """Converts a AikoAIObject back to a regular dict.
+    """Converts a OpenAIObject back to a regular dict.
 
-    Nested AikoAIObjects are also converted back to regular dicts.
+    Nested OpenAIObjects are also converted back to regular dicts.
 
-    :param obj: The AikoAIObject to convert.
+    :param obj: The OpenAIObject to convert.
 
-    :returns: The AikoAIObject as a dict.
+    :returns: The OpenAIObject as a dict.
     """
     if isinstance(obj, list):
         return [convert_to_dict(i) for i in obj]
-    # This works by virtue of the fact that AikoAIObjects _are_ dicts. The dict
+    # This works by virtue of the fact that OpenAIObjects _are_ dicts. The dict
     # comprehension returns a regular dict and recursively applies the
     # conversion to each value.
     elif isinstance(obj, dict):
         return {k: convert_to_dict(v) for k, v in obj.items()}
     else:
         return obj
 
@@ -180,9 +180,9 @@
             if not api_key.startswith("sk-"):
                 raise ValueError(f"Malformed API key in {aikoai.api_key_path}.")
             return api_key
     elif aikoai.api_key is not None:
         return aikoai.api_key
     else:
         raise aikoai.error.AuthenticationError(
-            "No API key provided. You can set your API key in code using 'aikoai.api_key = <API-KEY>', or you can set the environment variable AIIKOAI_API_KEY=<API-KEY>). If your API key is stored in a file, you can point the aikoai module at it with 'aikoai.api_key_path = <PATH>'. You can generate API keys in the AikoAI web interface. See https://platform.aikocute.tech/account/api-keys for details."
+            "No API key provided. You can set your API key in code using 'aikoai.api_key = <API-KEY>', or you can set the environment variable OPENAI_API_KEY=<API-KEY>). If your API key is stored in a file, you can point the aikoai module at it with 'aikoai.api_key_path = <PATH>'. You can generate API keys in the OpenAI web interface. See https://platform.aikocute.tech/account/api-keys for details."
         )
```

### Comparing `aikoai-1.1/aikoai/validators.py` & `aikoai-2.1/aikoai/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
             df.prompt.str[: -len(common_suffix)]
             .str.contains(common_suffix, regex=False)
             .any()
         ):
             immediate_msg += f"\n  WARNING: Some of your prompts contain the suffix `{common_suffix}` more than once. We strongly suggest that you review your prompts and add a unique suffix"
 
     else:
-        immediate_msg = "\n- Your data does not contain a common separator at the end of your prompts. Having a separator string appended to the end of the prompt makes it clearer to the fine-tuned model where the completion should begin. See https://platform.aikocute.tech/docs/guides/fine-tuning/preparing-your-dataset for more detail and examples. If you intend to do open-ended generation, then you should leave the prompts empty"
+        immediate_msg = "\n- Your data does not contain a common separator at the end of your prompts. Having a separator string appended to the end of the prompt makes it clearer to the fine-tuned model where the completion should begin. See https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset for more detail and examples. If you intend to do open-ended generation, then you should leave the prompts empty"
 
     if common_suffix == "":
         optional_msg = (
             f"Add a suffix separator `{display_suggested_suffix}` to all prompts"
         )
 
         def optional_fn(x):
@@ -393,15 +393,15 @@
             df.completion.str[: -len(common_suffix)]
             .str.contains(common_suffix, regex=False)
             .any()
         ):
             immediate_msg += f"\n  WARNING: Some of your completions contain the suffix `{common_suffix}` more than once. We suggest that you review your completions and add a unique ending"
 
     else:
-        immediate_msg = "\n- Your data does not contain a common ending at the end of your completions. Having a common ending string appended to the end of the completion makes it clearer to the fine-tuned model where the completion should end. See https://platform.aikocute.tech/docs/guides/fine-tuning/preparing-your-dataset for more detail and examples."
+        immediate_msg = "\n- Your data does not contain a common ending at the end of your completions. Having a common ending string appended to the end of the completion makes it clearer to the fine-tuned model where the completion should end. See https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset for more detail and examples."
 
     if common_suffix == "":
         optional_msg = (
             f"Add a suffix ending `{display_suggested_suffix}` to all completions"
         )
 
         def optional_fn(x):
@@ -428,15 +428,15 @@
         return x
 
     optional_msg = None
     optional_fn = None
     immediate_msg = None
 
     if df.completion.str[:1].nunique() != 1 or df.completion.values[0][0] != " ":
-        immediate_msg = "\n- The completion should start with a whitespace character (` `). This tends to produce better results due to the tokenization we use. See https://platform.aikocute.tech/docs/guides/fine-tuning/preparing-your-dataset for more details"
+        immediate_msg = "\n- The completion should start with a whitespace character (` `). This tends to produce better results due to the tokenization we use. See https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset for more details"
         optional_msg = "Add a whitespace character to the beginning of the completion"
         optional_fn = add_space_start
     return Remediation(
         name="completion_space_start",
         immediate_msg=immediate_msg,
         optional_msg=optional_msg,
         optional_fn=optional_fn,
@@ -462,15 +462,15 @@
         .apply(lambda x: sum(1 for c in x if c.isalpha() and c.islower()))
         .sum()
     )
 
     if count_upper * 2 > count_lower:
         return Remediation(
             name="lower_case",
-            immediate_msg=f"\n- More than a third of your `{column}` column/key is uppercase. Uppercase {column}s tends to perform worse than a mixture of case encountered in normal language. We recommend to lower case the data if that makes sense in your domain. See https://platform.aikocute.tech/docs/guides/fine-tuning/preparing-your-dataset for more details",
+            immediate_msg=f"\n- More than a third of your `{column}` column/key is uppercase. Uppercase {column}s tends to perform worse than a mixture of case encountered in normal language. We recommend to lower case the data if that makes sense in your domain. See https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset for more details",
             optional_msg=f"Lowercase all your data in column/key `{column}`",
             optional_fn=lower_case,
         )
 
 
 def read_any_format(fname, fields=["prompt", "completion"]):
     """
@@ -692,15 +692,15 @@
         else ""
     )
 
     input_text = "\n\nYour data will be written to a new JSONL file. Proceed [Y/n]: "
 
     if not any_remediations and not split:
         sys.stdout.write(
-            f'\nYou can use your file for fine-tuning:\n> aikoaii api fine_tunes.create -t "{fname}"{additional_params}\n\nAfter you’ve fine-tuned a model, remember that your prompt has to end with the indicator string `{common_prompt_suffix_new_line_handled}` for the model to start generating completions, rather than continuing with the prompt.{optional_ending_string}\n'
+            f'\nYou can use your file for fine-tuning:\n> openai api fine_tunes.create -t "{fname}"{additional_params}\n\nAfter you’ve fine-tuned a model, remember that your prompt has to end with the indicator string `{common_prompt_suffix_new_line_handled}` for the model to start generating completions, rather than continuing with the prompt.{optional_ending_string}\n'
         )
         estimate_fine_tuning_time(df)
 
     elif accept_suggestion(input_text, auto_accept):
         fnames = get_outfnames(fname, split)
         if split:
             assert len(fnames) == 2 and "train" in fnames[0] and "valid" in fnames[1]
@@ -732,15 +732,15 @@
         valid_string = f' -v "{fnames[1]}"' if split else ""
         separator_reminder = (
             ""
             if len(common_prompt_suffix_new_line_handled) == 0
             else f"After you’ve fine-tuned a model, remember that your prompt has to end with the indicator string `{common_prompt_suffix_new_line_handled}` for the model to start generating completions, rather than continuing with the prompt."
         )
         sys.stdout.write(
-            f'\nWrote modified file{files_string}`\nFeel free to take a look!\n\nNow use that file when fine-tuning:\n> aikoaii api fine_tunes.create -t "{fnames[0]}"{valid_string}{additional_params}\n\n{separator_reminder}{optional_ending_string}\n'
+            f'\nWrote modified file{files_string}`\nFeel free to take a look!\n\nNow use that file when fine-tuning:\n> openai api fine_tunes.create -t "{fnames[0]}"{valid_string}{additional_params}\n\n{separator_reminder}{optional_ending_string}\n'
         )
         estimate_fine_tuning_time(df)
     else:
         sys.stdout.write("Aborting... did not write the file\n")
 
 
 def infer_task_type(df):
```

### Comparing `aikoai-1.1/aikoai/wandb_logger.py` & `aikoai-2.1/aikoai/wandb_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from aikoai import File, FineTune
     from aikoai.datalib.numpy_helper import numpy as np
     from aikoai.datalib.pandas_helper import pandas as pd
 
 
 class WandbLogger:
     """
-    Log fine-tunes to [Weights & Biases](https://wandb.me/aikoaii-docs)
+    Log fine-tunes to [Weights & Biases](https://wandb.me/openai-docs)
     """
 
     if not WANDB_AVAILABLE:
         print("Logging requires wandb to be installed. Run `pip install wandb`.")
     else:
         _wandb_api = None
         _logged_in = False
```

### Comparing `aikoai-1.1/aikoai.egg-info/SOURCES.txt` & `aikoai-2.1/aikoai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aikoai-1.1/setup.cfg` & `aikoai-2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = aikoai
 version = attr: aikoai.version.VERSION
 description = Python client library for the AikoAI API
 long_description = file: README.md
 long_description_content_type = text/markdown
-author = AikoAI
+author = AikoCute
 author_email = support@aikocute.tech
 url = https://github.com/Github-Aiko/aikoai-python
 license_files = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

