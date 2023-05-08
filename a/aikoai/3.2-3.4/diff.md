# Comparing `tmp/aikoai-3.2.tar.gz` & `tmp/aikoai-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikoai-3.2.tar", last modified: Mon May  8 18:22:38 2023, max compression
+gzip compressed data, was "aikoai-3.4.tar", last modified: Mon May  8 18:28:04 2023, max compression
```

## Comparing `aikoai-3.2.tar` & `aikoai-3.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:38.933910 aikoai-3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 18:22:38.933910 aikoai-3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:38.929909 aikoai-3.2/aikoai/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/_aikoai_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/aikoai_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/aikoai_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:38.929909 aikoai-3.2/aikoai/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:38.929909 aikoai-3.2/aikoai/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/abstract/api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/abstract/engine_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/error_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:38.929909 aikoai-3.2/aikoai/api_resources/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/experimental/completion_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/fine_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/api_resources/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38173 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:38.929909 aikoai-3.2/aikoai/datalib/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/datalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/datalib/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/datalib/numpy_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/datalib/pandas_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/embeddings_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/object_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:38.933910 aikoai-3.2/aikoai/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:38.933910 aikoai-3.2/aikoai/tests/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/asyncio/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/test_api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/test_file_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/test_long_examples_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/test_url_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/upload_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    34289 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-05-08 18:22:27.000000 aikoai-3.2/aikoai/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:22:38.929909 aikoai-3.2/aikoai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 18:22:38.000000 aikoai-3.2/aikoai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-08 18:22:38.000000 aikoai-3.2/aikoai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:22:38.000000 aikoai-3.2/aikoai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 18:22:38.000000 aikoai-3.2/aikoai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 18:22:38.000000 aikoai-3.2/aikoai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 18:22:38.000000 aikoai-3.2/aikoai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:22:38.000000 aikoai-3.2/aikoai.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-08 18:22:27.000000 aikoai-3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-08 18:22:38.933910 aikoai-3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:22:27.000000 aikoai-3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:28:04.154333 aikoai-3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 18:28:04.154333 aikoai-3.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:28:04.146333 aikoai-3.4/aikoai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/_aikoai_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/aikoai_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/aikoai_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:28:04.150333 aikoai-3.4/aikoai/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:28:04.154333 aikoai-3.4/aikoai/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/abstract/api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/abstract/engine_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/error_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:28:04.154333 aikoai-3.4/aikoai/api_resources/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/experimental/completion_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/fine_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/api_resources/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38173 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:28:04.154333 aikoai-3.4/aikoai/datalib/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/datalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/datalib/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/datalib/numpy_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/datalib/pandas_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/embeddings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/object_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:28:04.154333 aikoai-3.4/aikoai/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:28:04.154333 aikoai-3.4/aikoai/tests/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/asyncio/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/test_api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/test_file_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/test_long_examples_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/test_url_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/upload_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34289 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-05-08 18:27:51.000000 aikoai-3.4/aikoai/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:28:04.150333 aikoai-3.4/aikoai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 18:28:04.000000 aikoai-3.4/aikoai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-08 18:28:04.000000 aikoai-3.4/aikoai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:28:04.000000 aikoai-3.4/aikoai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 18:28:04.000000 aikoai-3.4/aikoai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 18:28:04.000000 aikoai-3.4/aikoai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 18:28:04.000000 aikoai-3.4/aikoai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:28:03.000000 aikoai-3.4/aikoai.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-08 18:27:51.000000 aikoai-3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-08 18:28:04.154333 aikoai-3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:27:51.000000 aikoai-3.4/setup.py
```

### Comparing `aikoai-3.2/aikoai/__init__.py` & `aikoai-3.4/aikoai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from aikoai.version import VERSION
 from aikoai.api_resources import BASE, TYPE
 
 if TYPE_CHECKING:
     import requests
     from aiohttp import ClientSession
 
-api_key = 'sk-' + os.environ.get("AIKOAI_API_KEY")
+api_key = os.environ.get("AIKOAI_API_KEY")
 # Path of a file with an API key, whose contents can change. Supercedes
 # `api_key` if set.  The main use case is volume-mounted Kubernetes secrets,
 # which are updated automatically.
 api_key_path: Optional[str] = os.environ.get("AIKOAI_API_KEY_PATH")
 
 organization = os.environ.get("AIKOAI_ORGANIZATION")
 api_base = os.environ.get("AIKOAI_API_BASE", BASE)
```

### Comparing `aikoai-3.2/aikoai/_aikoai_scripts.py` & `aikoai-3.4/aikoai/_aikoai_scripts.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/aikoai_object.py` & `aikoai-3.4/aikoai/aikoai_object.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/aikoai_response.py` & `aikoai-3.4/aikoai/aikoai_response.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_requestor.py` & `aikoai-3.4/aikoai/api_requestor.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/__init__.py` & `aikoai-3.4/aikoai/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/abstract/__init__.py` & `aikoai-3.4/aikoai/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/abstract/api_resource.py` & `aikoai-3.4/aikoai/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/abstract/createable_api_resource.py` & `aikoai-3.4/aikoai/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/abstract/deletable_api_resource.py` & `aikoai-3.4/aikoai/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/abstract/engine_api_resource.py` & `aikoai-3.4/aikoai/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/abstract/listable_api_resource.py` & `aikoai-3.4/aikoai/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/abstract/nested_resource_class_methods.py` & `aikoai-3.4/aikoai/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/abstract/updateable_api_resource.py` & `aikoai-3.4/aikoai/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/audio.py` & `aikoai-3.4/aikoai/api_resources/audio.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/chat_completion.py` & `aikoai-3.4/aikoai/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/completion.py` & `aikoai-3.4/aikoai/api_resources/completion.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/customer.py` & `aikoai-3.4/aikoai/api_resources/customer.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/deployment.py` & `aikoai-3.4/aikoai/api_resources/deployment.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/edit.py` & `aikoai-3.4/aikoai/api_resources/edit.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/embedding.py` & `aikoai-3.4/aikoai/api_resources/embedding.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/engine.py` & `aikoai-3.4/aikoai/api_resources/engine.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/error_object.py` & `aikoai-3.4/aikoai/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/file.py` & `aikoai-3.4/aikoai/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/fine_tune.py` & `aikoai-3.4/aikoai/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/image.py` & `aikoai-3.4/aikoai/api_resources/image.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/api_resources/moderation.py` & `aikoai-3.4/aikoai/api_resources/moderation.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/cli.py` & `aikoai-3.4/aikoai/cli.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/datalib/__init__.py` & `aikoai-3.4/aikoai/datalib/__init__.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/embeddings_utils.py` & `aikoai-3.4/aikoai/embeddings_utils.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/error.py` & `aikoai-3.4/aikoai/error.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/tests/asyncio/test_endpoints.py` & `aikoai-3.4/aikoai/tests/asyncio/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/tests/test_api_requestor.py` & `aikoai-3.4/aikoai/tests/test_api_requestor.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/tests/test_endpoints.py` & `aikoai-3.4/aikoai/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/tests/test_exceptions.py` & `aikoai-3.4/aikoai/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/tests/test_file_cli.py` & `aikoai-3.4/aikoai/tests/test_file_cli.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/tests/test_long_examples_validator.py` & `aikoai-3.4/aikoai/tests/test_long_examples_validator.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/tests/test_url_composition.py` & `aikoai-3.4/aikoai/tests/test_url_composition.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/tests/test_util.py` & `aikoai-3.4/aikoai/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/upload_progress.py` & `aikoai-3.4/aikoai/upload_progress.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/util.py` & `aikoai-3.4/aikoai/util.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/validators.py` & `aikoai-3.4/aikoai/validators.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai/wandb_logger.py` & `aikoai-3.4/aikoai/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/aikoai.egg-info/SOURCES.txt` & `aikoai-3.4/aikoai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aikoai-3.2/setup.cfg` & `aikoai-3.4/setup.cfg`

 * *Files identical despite different names*

