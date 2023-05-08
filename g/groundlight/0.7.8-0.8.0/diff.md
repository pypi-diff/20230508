# Comparing `tmp/groundlight-0.7.8.tar.gz` & `tmp/groundlight-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundlight-0.7.8.tar", max compression
+gzip compressed data, was "groundlight-0.8.0.tar", max compression
```

## Comparing `groundlight-0.7.8.tar` & `groundlight-0.8.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1071 2023-04-19 00:35:48.490143 groundlight-0.7.8/LICENSE
--rw-r--r--   0        0        0     1770 2023-04-19 00:35:48.490143 groundlight-0.7.8/README.md
--rw-r--r--   0        0        0     3597 2023-04-19 00:35:48.494143 groundlight-0.7.8/generated/model.py
--rw-r--r--   0        0        0      721 2023-04-19 00:35:48.494143 groundlight-0.7.8/generated/openapi_client/__init__.py
--rw-r--r--   0        0        0      220 2023-04-19 00:35:48.494143 groundlight-0.7.8/generated/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    14018 2023-04-19 00:35:48.494143 groundlight-0.7.8/generated/openapi_client/api/detectors_api.py
--rw-r--r--   0        0        0    14322 2023-04-19 00:35:48.494143 groundlight-0.7.8/generated/openapi_client/api/image_queries_api.py
--rw-r--r--   0        0        0    35591 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/api_client.py
--rw-r--r--   0        0        0      537 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/apis/__init__.py
--rw-r--r--   0        0        0    17643 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/configuration.py
--rw-r--r--   0        0        0     4979 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/exceptions.py
--rw-r--r--   0        0        0      348 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/__init__.py
--rw-r--r--   0        0        0    11870 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/classification_result.py
--rw-r--r--   0        0        0    13623 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/detector.py
--rw-r--r--   0        0        0    13486 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/detector_creation_input.py
--rw-r--r--   0        0        0    11288 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/detector_type_enum.py
--rw-r--r--   0        0        0    13847 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/image_query.py
--rw-r--r--   0        0        0    11330 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/image_query_type_enum.py
--rw-r--r--   0        0        0    12129 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/paginated_detector_list.py
--rw-r--r--   0        0        0    12150 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/paginated_image_query_list.py
--rw-r--r--   0        0        0    11438 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model/result_type_enum.py
--rw-r--r--   0        0        0    79719 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/model_utils.py
--rw-r--r--   0        0        0     1007 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/models/__init__.py
--rw-r--r--   0        0        0    14005 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/openapi_client/rest.py
--rw-r--r--   0        0        0      955 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/setup.py
--rw-r--r--   0        0        0        0 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/__init__.py
--rw-r--r--   0        0        0      779 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_classification_result.py
--rw-r--r--   0        0        0      813 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_detector.py
--rw-r--r--   0        0        0      787 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_detector_creation_input.py
--rw-r--r--   0        0        0      752 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_detector_type_enum.py
--rw-r--r--   0        0        0      828 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_detectors_api.py
--rw-r--r--   0        0        0      864 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_image_queries_api.py
--rw-r--r--   0        0        0     1080 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_image_query.py
--rw-r--r--   0        0        0      767 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_image_query_type_enum.py
--rw-r--r--   0        0        0      872 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_paginated_detector_list.py
--rw-r--r--   0        0        0      896 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_paginated_image_query_list.py
--rw-r--r--   0        0        0      738 2023-04-19 00:35:48.498143 groundlight-0.7.8/generated/test/test_result_type_enum.py
--rw-r--r--   0        0        0     1804 2023-04-19 00:35:48.502143 groundlight-0.7.8/pyproject.toml
--rw-r--r--   0        0        0      535 2023-04-19 00:35:48.502143 groundlight-0.7.8/src/groundlight/__init__.py
--rw-r--r--   0        0        0     1806 2023-04-19 00:35:48.502143 groundlight-0.7.8/src/groundlight/binary_labels.py
--rw-r--r--   0        0        0    10518 2023-04-19 00:35:48.502143 groundlight-0.7.8/src/groundlight/client.py
--rw-r--r--   0        0        0      271 2023-04-19 00:35:48.502143 groundlight-0.7.8/src/groundlight/config.py
--rw-r--r--   0        0        0     2074 2023-04-19 00:35:48.502143 groundlight-0.7.8/src/groundlight/images.py
--rw-r--r--   0        0        0     5757 2023-04-19 00:35:48.502143 groundlight-0.7.8/src/groundlight/internalapi.py
--rw-r--r--   0        0        0     1778 2023-04-19 00:35:48.502143 groundlight-0.7.8/src/groundlight/optional_imports.py
--rw-r--r--   0        0        0      308 2023-04-19 00:35:48.502143 groundlight-0.7.8/src/groundlight/status_codes.py
--rw-r--r--   0        0        0     2751 1970-01-01 00:00:00.000000 groundlight-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 18:55:30.181203 groundlight-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1868 2023-05-08 18:55:30.181203 groundlight-0.8.0/README.md
+-rw-r--r--   0        0        0     3597 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/model.py
+-rw-r--r--   0        0        0      721 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    14018 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/api/detectors_api.py
+-rw-r--r--   0        0        0    14322 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/api/image_queries_api.py
+-rw-r--r--   0        0        0    35591 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/api_client.py
+-rw-r--r--   0        0        0      537 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/apis/__init__.py
+-rw-r--r--   0        0        0    17643 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/configuration.py
+-rw-r--r--   0        0        0     4979 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/exceptions.py
+-rw-r--r--   0        0        0      348 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/__init__.py
+-rw-r--r--   0        0        0    11870 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/classification_result.py
+-rw-r--r--   0        0        0    13623 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/detector.py
+-rw-r--r--   0        0        0    13486 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/detector_creation_input.py
+-rw-r--r--   0        0        0    11288 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/detector_type_enum.py
+-rw-r--r--   0        0        0    13847 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/image_query.py
+-rw-r--r--   0        0        0    11330 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/image_query_type_enum.py
+-rw-r--r--   0        0        0    12129 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/paginated_detector_list.py
+-rw-r--r--   0        0        0    12150 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/paginated_image_query_list.py
+-rw-r--r--   0        0        0    11438 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/result_type_enum.py
+-rw-r--r--   0        0        0    79719 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model_utils.py
+-rw-r--r--   0        0        0     1007 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0    14005 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/rest.py
+-rw-r--r--   0        0        0      955 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/setup.py
+-rw-r--r--   0        0        0        0 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_classification_result.py
+-rw-r--r--   0        0        0      813 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_detector.py
+-rw-r--r--   0        0        0      787 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_detector_creation_input.py
+-rw-r--r--   0        0        0      752 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_detector_type_enum.py
+-rw-r--r--   0        0        0      828 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_detectors_api.py
+-rw-r--r--   0        0        0      864 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_image_queries_api.py
+-rw-r--r--   0        0        0     1080 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_image_query.py
+-rw-r--r--   0        0        0      767 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_image_query_type_enum.py
+-rw-r--r--   0        0        0      872 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_paginated_detector_list.py
+-rw-r--r--   0        0        0      896 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_paginated_image_query_list.py
+-rw-r--r--   0        0        0      738 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_result_type_enum.py
+-rw-r--r--   0        0        0     1804 2023-05-08 18:55:30.193203 groundlight-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      568 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/__init__.py
+-rw-r--r--   0        0        0     2692 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/binary_labels.py
+-rw-r--r--   0        0        0    11267 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/client.py
+-rw-r--r--   0        0        0      271 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/config.py
+-rw-r--r--   0        0        0     2135 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/images.py
+-rw-r--r--   0        0        0     5759 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/internalapi.py
+-rw-r--r--   0        0        0     1778 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/optional_imports.py
+-rw-r--r--   0        0        0      308 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/status_codes.py
+-rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 groundlight-0.8.0/PKG-INFO
```

### Comparing `groundlight-0.7.8/LICENSE` & `groundlight-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/README.md` & `groundlight-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -26,11 +26,11 @@
 
 _Note: The SDK is currently in "beta" phase. Interfaces are subject to change in future versions. We will follow [semver](https://semver.org/) semantics for breaking changes._
 
 ## Learn more
 
 Some more resources you might like:
 
-- [Code Documentation](https://code.groundlight.ai/)
-- [Python SDK](https://pypi.org/project/groundlight/)
+- [Code Documentation](https://code.groundlight.ai/python-sdk/docs/getting-started)
+- [Python SDK on PyPi](https://pypi.org/project/groundlight/) or [GitHub](https://github.com/groundlight/python-sdk)
 - [Company](https://www.groundlight.ai/)
-- [Login to Groundlight](https://app.groundlight.ai/)
+- [Login to Groundlight App](https://app.groundlight.ai/)
```

### Comparing `groundlight-0.7.8/generated/model.py` & `groundlight-0.8.0/generated/model.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/__init__.py` & `groundlight-0.8.0/generated/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/api/detectors_api.py` & `groundlight-0.8.0/generated/openapi_client/api/detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/api/image_queries_api.py` & `groundlight-0.8.0/generated/openapi_client/api/image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/api_client.py` & `groundlight-0.8.0/generated/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/apis/__init__.py` & `groundlight-0.8.0/generated/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/configuration.py` & `groundlight-0.8.0/generated/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/exceptions.py` & `groundlight-0.8.0/generated/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model/classification_result.py` & `groundlight-0.8.0/generated/openapi_client/model/classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model/detector.py` & `groundlight-0.8.0/generated/openapi_client/model/detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model/detector_creation_input.py` & `groundlight-0.8.0/generated/openapi_client/model/detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model/detector_type_enum.py` & `groundlight-0.8.0/generated/openapi_client/model/detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model/image_query.py` & `groundlight-0.8.0/generated/openapi_client/model/image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model/image_query_type_enum.py` & `groundlight-0.8.0/generated/openapi_client/model/image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model/paginated_detector_list.py` & `groundlight-0.8.0/generated/openapi_client/model/paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model/paginated_image_query_list.py` & `groundlight-0.8.0/generated/openapi_client/model/paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model/result_type_enum.py` & `groundlight-0.8.0/generated/openapi_client/model/result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/model_utils.py` & `groundlight-0.8.0/generated/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/models/__init__.py` & `groundlight-0.8.0/generated/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/openapi_client/rest.py` & `groundlight-0.8.0/generated/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/setup.py` & `groundlight-0.8.0/generated/setup.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_classification_result.py` & `groundlight-0.8.0/generated/test/test_classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_detector.py` & `groundlight-0.8.0/generated/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_detector_creation_input.py` & `groundlight-0.8.0/generated/test/test_detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_detector_type_enum.py` & `groundlight-0.8.0/generated/test/test_detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_detectors_api.py` & `groundlight-0.8.0/generated/test/test_detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_image_queries_api.py` & `groundlight-0.8.0/generated/test/test_image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_image_query.py` & `groundlight-0.8.0/generated/test/test_image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_image_query_type_enum.py` & `groundlight-0.8.0/generated/test/test_image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_paginated_detector_list.py` & `groundlight-0.8.0/generated/test/test_paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_paginated_image_query_list.py` & `groundlight-0.8.0/generated/test/test_paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/generated/test/test_result_type_enum.py` & `groundlight-0.8.0/generated/test/test_result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/pyproject.toml` & `groundlight-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = "MIT"
 name = "groundlight"
 packages = [
     {include = "**/*.py", from = "generated"},
     {include = "**/*.py", from = "src"},
 ]
 readme = "README.md"
-version = "0.7.8"
+version = "0.8.0"
 
 [tool.poetry.dependencies]
 certifi = "^2021.10.8"
 frozendict = "^2.3.2"
 pillow = "^9.0.0" # TODO: We may want to mark pillow (and numpy) as extra (https://python-poetry.org/docs/master/pyproject#extras)
 pydantic = "^1.7.4"
 python = ">=3.7.0,<4.0"
```

### Comparing `groundlight-0.7.8/src/groundlight/__init__.py` & `groundlight-0.8.0/src/groundlight/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # ruff: noqa
 # Add useful imports from the generated code here at the top level, as a convenience.
 from openapi_client import ApiException
 
 # Imports from our code
 from .client import Groundlight
+from .binary_labels import Label
 
 try:
     import importlib.metadata
 
     # Copy the version number from where it's set in pyproject.toml
     __version__ = importlib.metadata.version("groundlight")
 except ModuleNotFoundError:
```

### Comparing `groundlight-0.7.8/src/groundlight/binary_labels.py` & `groundlight-0.8.0/src/groundlight/binary_labels.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,76 @@
-"""Defines the possible values for binary class labels like Yes/No or PASS/FAIL.
+"""Defines the possible values for binary class labels like YES/NO.
 Provides methods to convert between them.
 
 This part of the API is kinda ugly right now.  So we'll encapsulate the ugliness in one place.
 """
 import logging
-from typing import List, Union
+from enum import Enum
+from typing import Union
 
 from model import Detector, ImageQuery
 
-logger = logging.getLogger("groundlight.sdk")
+logger = logging.getLogger(__name__)
 
 
-def internal_labels_for_detector(
-    context: Union[ImageQuery, Detector, str],  # pylint: disable=unused-argument
-) -> List[str]:
-    """Returns an ordered list of class labels as strings.
-    These are the versions of labels that the API demands.
-    :param context: Can be an ImageQuery, a Detector, or a string-id for one of them.
-    """
-    # NOTE: At some point this will need to be an API call, because these will be defined per-detector
-    return ["PASS", "FAIL"]
+class Label(str, Enum):
+    YES = "YES"
+    NO = "NO"
+    UNSURE = "UNSURE"
+
+
+VALID_DISPLAY_LABELS = {Label.YES, Label.NO, Label.UNSURE}
+
+
+class DeprecatedLabel(str, Enum):
+    PASS = "PASS"
+    FAIL = "FAIL"
+    NEEDS_REVIEW = "NEEDS_REVIEW"
+
+
+DEPRECATED_LABEL_NAMES = {DeprecatedLabel.PASS, DeprecatedLabel.FAIL, DeprecatedLabel.NEEDS_REVIEW}
 
 
 def convert_internal_label_to_display(
     context: Union[ImageQuery, Detector, str],  # pylint: disable=unused-argument
     label: str,
-) -> str:
+) -> Union[Label, str]:
+    """Convert a label that comes from our API into the label string enum that we show to the user.
+
+    NOTE: We return UPPERCASE label strings to the user, unless there is a custom label (which
+    shouldn't be happening at this time).
+    """
     # NOTE: Someday we will do nothing here, when the server provides properly named classes.
+    if not isinstance(label, str):
+        raise ValueError(f"Expected a string label, but got {label} of type {type(label)}")
     upper = label.upper()
-    if upper == "PASS":
-        return "YES"
-    if upper == "FAIL":
-        return "NO"
-    if upper in ["YES", "NO"]:
-        return label
-    logger.warning(f"Unrecognized internal label {label} - leaving alone.")
+    if upper in {Label.YES, DeprecatedLabel.PASS}:
+        return Label.YES
+    if upper in {Label.NO, DeprecatedLabel.FAIL}:
+        return Label.NO
+    if upper in {Label.UNSURE, DeprecatedLabel.NEEDS_REVIEW}:
+        return Label.UNSURE
+
+    logger.warning(f"Unrecognized internal label {label} - leaving it alone as a string.")
     return label
 
 
 def convert_display_label_to_internal(
     context: Union[ImageQuery, Detector, str],  # pylint: disable=unused-argument
-    label: str,
+    label: Union[Label, str],
 ) -> str:
+    """Convert a label that comes from the user into the label string that we send to the server. We
+    are strict here, and only allow YES/NO.
+
+    NOTE: We accept case-insensitive label strings from the user, but we send UPPERCASE labels to
+    the server. E.g., user inputs "yes" -> the label is returned as "YES".
+    """
     # NOTE: In the future we should validate against actually supported labels for the detector
+    if not isinstance(label, str):
+        raise ValueError(f"Expected a string label, but got {label} of type {type(label)}")
     upper = label.upper()
-    if upper in {"PASS", "YES"}:
-        return "PASS"
-    if upper in {"FAIL", "NO"}:
-        return "FAIL"
-    raise ValueError(f'Invalid label string "{label}".  Must be one of YES,NO,PASS,FAIL')
+    if upper == Label.YES:
+        return DeprecatedLabel.PASS.value
+    if upper == Label.NO:
+        return DeprecatedLabel.FAIL.value
+
+    raise ValueError(f"Invalid label string '{label}'.  Must be one of '{Label.YES.value}','{Label.NO.value}'.")
```

### Comparing `groundlight-0.7.8/src/groundlight/client.py` & `groundlight-0.8.0/src/groundlight/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from model import Detector, ImageQuery, PaginatedDetectorList, PaginatedImageQueryList
 from openapi_client import Configuration
 from openapi_client.api.detectors_api import DetectorsApi
 from openapi_client.api.image_queries_api import ImageQueriesApi
 from openapi_client.model.detector_creation_input import DetectorCreationInput
 
-from groundlight.binary_labels import convert_display_label_to_internal
+from groundlight.binary_labels import Label, convert_display_label_to_internal, convert_internal_label_to_display
 from groundlight.config import API_TOKEN_VARIABLE_NAME, API_TOKEN_WEB_URL
 from groundlight.images import parse_supported_image_types
 from groundlight.internalapi import GroundlightApiClient, NotFoundError, sanitize_endpoint_url
 from groundlight.optional_imports import Image, np
 
 logger = logging.getLogger("groundlight.sdk")
 
@@ -35,16 +35,15 @@
     iq = gl.submit_image_query(d, image)
     print(iq.result)
     ```
     """
 
     DEFAULT_WAIT: float = 30.0
 
-    BEFORE_POLLING_DELAY = 3.0  # Expected minimum time for a label to post
-    POLLING_INITIAL_DELAY = 0.5
+    POLLING_INITIAL_DELAY = 0.25
     POLLING_EXPONENTIAL_BACKOFF = 1.3  # This still has the nice backoff property that the max number of requests
     # is O(log(time)), but with 1.3 the guarantee is that the call will return no more than 30% late
 
     def __init__(self, endpoint: Optional[str] = None, api_token: Optional[str] = None) -> None:
         """:param endpoint: optionally specify a different endpoint
         :param api_token: use this API token for your API calls. If unset, fallback to the
             environment variable "GROUNDLIGHT_API_TOKEN".
@@ -68,14 +67,23 @@
 
         configuration.api_key["ApiToken"] = api_token
 
         self.api_client = GroundlightApiClient(configuration)
         self.detectors_api = DetectorsApi(self.api_client)
         self.image_queries_api = ImageQueriesApi(self.api_client)
 
+    @classmethod
+    def _post_process_image_query(cls, iq: ImageQuery) -> ImageQuery:
+        """Post-process the image query so we don't use confusing internal labels.
+
+        TODO: Get rid of this once we clean up the mapping logic server-side.
+        """
+        iq.result.label = convert_internal_label_to_display(iq, iq.result.label)
+        return iq
+
     def get_detector(self, id: Union[str, Detector]) -> Detector:  # pylint: disable=redefined-builtin
         if isinstance(id, Detector):
             # Short-circuit
             return id
         obj = self.detectors_api.get_detector(id=id)
         return Detector.parse_obj(obj.to_dict())
 
@@ -99,62 +107,78 @@
             detector_creation_input.confidence_threshold = confidence_threshold
         if config_name is not None:
             detector_creation_input.config_name = config_name
         obj = self.detectors_api.create_detector(detector_creation_input)
         return Detector.parse_obj(obj.to_dict())
 
     def get_or_create_detector(
-        self, name: str, query: str, *, confidence_threshold: Optional[float] = None, config_name: Optional[str] = None
+        self,
+        name: str,
+        query: str,
+        *,
+        confidence_threshold: Optional[float] = None,
+        config_name: Optional[str] = None,
     ) -> Detector:
         """Tries to look up the detector by name.  If a detector with that name, query, and
         confidence exists, return it. Otherwise, create a detector with the specified query and
         config.
         """
         try:
             existing_detector = self.get_detector_by_name(name)
         except NotFoundError:
             logger.debug(f"We could not find a detector with name='{name}'. So we will create a new detector ...")
             return self.create_detector(
-                name=name, query=query, confidence_threshold=confidence_threshold, config_name=config_name
+                name=name,
+                query=query,
+                confidence_threshold=confidence_threshold,
+                config_name=config_name,
             )
 
         # TODO: We may soon allow users to update the retrieved detector's fields.
         if existing_detector.query != query:
             raise ValueError(
-                f"Found existing detector with name={name} (id={existing_detector.id}) but the queries don't match."
-                f" The existing query is '{existing_detector.query}'."
+                (
+                    f"Found existing detector with name={name} (id={existing_detector.id}) but the queries don't match."
+                    f" The existing query is '{existing_detector.query}'."
+                ),
             )
         if confidence_threshold is not None and existing_detector.confidence_threshold != confidence_threshold:
             raise ValueError(
-                f"Found existing detector with name={name} (id={existing_detector.id}) but the confidence"
-                " thresholds don't match. The existing confidence threshold is"
-                f" {existing_detector.confidence_threshold}."
+                (
+                    f"Found existing detector with name={name} (id={existing_detector.id}) but the confidence"
+                    " thresholds don't match. The existing confidence threshold is"
+                    f" {existing_detector.confidence_threshold}."
+                ),
             )
         return existing_detector
 
     def get_image_query(self, id: str) -> ImageQuery:  # pylint: disable=redefined-builtin
         obj = self.image_queries_api.get_image_query(id=id)
-        return ImageQuery.parse_obj(obj.to_dict())
+        iq = ImageQuery.parse_obj(obj.to_dict())
+        return self._post_process_image_query(iq)
 
     def list_image_queries(self, page: int = 1, page_size: int = 10) -> PaginatedImageQueryList:
         obj = self.image_queries_api.list_image_queries(page=page, page_size=page_size)
-        return PaginatedImageQueryList.parse_obj(obj.to_dict())
+        image_queries = PaginatedImageQueryList.parse_obj(obj.to_dict())
+        if image_queries.results is not None:
+            image_queries.results = [self._post_process_image_query(iq) for iq in image_queries.results]
+        return image_queries
 
     def submit_image_query(
         self,
         detector: Union[Detector, str],
         image: Union[str, bytes, Image.Image, BytesIO, BufferedReader, np.ndarray],
         wait: Optional[float] = None,
     ) -> ImageQuery:
         """Evaluates an image with Groundlight.
         :param detector: the Detector object, or string id of a detector like `det_12345`
         :param image: The image, in several possible formats:
           - filename (string) of a jpeg file
           - byte array or BytesIO or BufferedReader with jpeg bytes
-          - numpy array with values 0-255 and dimensions (H,W,3) in RGB order
+          - numpy array with values 0-255 and dimensions (H,W,3) in BGR order
             (Note OpenCV uses BGR not RGB. `img[:, :, ::-1]` will reverse the channels)
           - PIL Image
           Any binary format must be JPEG-encoded already.  Any pixel format will get
           converted to JPEG at high quality before sending to service.
         :param wait: How long to wait (in seconds) for a confident answer.
         """
         if wait is None:
@@ -163,15 +187,15 @@
         image_bytesio: Union[BytesIO, BufferedReader] = parse_supported_image_types(image)
 
         raw_image_query = self.image_queries_api.submit_image_query(detector_id=detector_id, body=image_bytesio)
         image_query = ImageQuery.parse_obj(raw_image_query.to_dict())
         if wait:
             threshold = self.get_detector(detector).confidence_threshold
             image_query = self.wait_for_confident_result(image_query, confidence_threshold=threshold, timeout_sec=wait)
-        return image_query
+        return self._post_process_image_query(image_query)
 
     def wait_for_confident_result(
         self,
         image_query: ImageQuery,
         confidence_threshold: float,
         timeout_sec: float = 30.0,
     ) -> ImageQuery:
@@ -179,15 +203,14 @@
         Currently this is done by polling with an exponential back-off.
         :param image_query: An ImageQuery object to poll
         :param confidence_threshold: The minimum confidence level required to return before the timeout.
         :param timeout_sec: The maximum number of seconds to wait.
         """
         # TODO: Add support for ImageQuery id instead of object.
         timeout_time = time.time() + timeout_sec
-        time.sleep(self.BEFORE_POLLING_DELAY)
         delay = self.POLLING_INITIAL_DELAY
         while time.time() < timeout_time:
             current_confidence = image_query.result.confidence
             if current_confidence is None:
                 logging.debug("Image query with None confidence implies human label (for now)")
                 break
             if current_confidence >= confidence_threshold:
@@ -201,19 +224,19 @@
             )
             time_left = max(0, time.time() - timeout_time)
             time.sleep(min(delay, time_left))
             delay *= self.POLLING_EXPONENTIAL_BACKOFF
             image_query = self.get_image_query(image_query.id)
         return image_query
 
-    def add_label(self, image_query: Union[ImageQuery, str], label: str):
+    def add_label(self, image_query: Union[ImageQuery, str], label: Union[Label, str]):
         """A new label to an image query.  This answers the detector's question.
         :param image_query: Either an ImageQuery object (returned from `submit_image_query`) or
         an image_query id as a string.
-        :param label: The string "Yes" or the string "No" in answer to the query.
+        :param label: The string "YES" or the string "NO" in answer to the query.
         """
         if isinstance(image_query, ImageQuery):
             image_query_id = image_query.id
         else:
             image_query_id = str(image_query)
             # Some old imagequery id's started with "chk_"
             if not image_query_id.startswith(("chk_", "iq_")):
```

### Comparing `groundlight-0.7.8/src/groundlight/images.py` & `groundlight-0.8.0/src/groundlight/images.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         image.save(bytesio, "jpeg", quality=jpeg_quality)
         bytesio.seek(0)
         return bytesio
     if isinstance(image, (BytesIO, BufferedReader)):
         # Already in the right format
         return image
     if isinstance(image, np.ndarray):
-        return BytesIO(jpeg_from_numpy(image, jpeg_quality=jpeg_quality))
+        # Assume it is in BGR format from opencv
+        return BytesIO(jpeg_from_numpy(image[:, :, ::-1], jpeg_quality=jpeg_quality))
     raise TypeError(
         (
             "Unsupported type for image. Must be PIL, numpy (H,W,3) RGB, or a JPEG as a filename (str), bytes,"
             " BytesIO, or BufferedReader."
         ),
     )
```

### Comparing `groundlight-0.7.8/src/groundlight/internalapi.py` & `groundlight-0.8.0/src/groundlight/internalapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,19 +129,19 @@
         """
         url = f"{self.configuration.host}/v1/detectors?name={name}"
         headers = self._headers()
         response = requests.request("GET", url, headers=headers)
 
         if not is_ok(response.status_code):
             raise InternalApiError(
-                f"Error getting detector by name '{name}' (status={response.status_code}): {response.text}"
+                f"Error getting detector by name '{name}' (status={response.status_code}): {response.text}",
             )
 
         parsed = response.json()
 
         if parsed["count"] == 0:
             raise NotFoundError(f"Detector with name={name} not found.")
         if parsed["count"] > 1:
             raise RuntimeError(
-                f"We found multiple ({parsed['count']}) detectors with the same name. This shouldn't happen."
+                f"We found multiple ({parsed['count']}) detectors with the same name. This shouldn't happen.",
             )
         return Detector.parse_obj(parsed["results"][0])
```

### Comparing `groundlight-0.7.8/src/groundlight/optional_imports.py` & `groundlight-0.8.0/src/groundlight/optional_imports.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.8/PKG-INFO` & `groundlight-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groundlight
-Version: 0.7.8
+Version: 0.8.0
 Summary: Build computer vision systems from natural language with Groundlight
 Home-page: https://code.groundlight.ai/python-sdk
 License: MIT
 Author: Groundlight AI
 Author-email: support@groundlight.ai
 Requires-Python: >=3.7.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -51,12 +51,12 @@
 
 _Note: The SDK is currently in "beta" phase. Interfaces are subject to change in future versions. We will follow [semver](https://semver.org/) semantics for breaking changes._
 
 ## Learn more
 
 Some more resources you might like:
 
-- [Code Documentation](https://code.groundlight.ai/)
-- [Python SDK](https://pypi.org/project/groundlight/)
+- [Code Documentation](https://code.groundlight.ai/python-sdk/docs/getting-started)
+- [Python SDK on PyPi](https://pypi.org/project/groundlight/) or [GitHub](https://github.com/groundlight/python-sdk)
 - [Company](https://www.groundlight.ai/)
-- [Login to Groundlight](https://app.groundlight.ai/)
+- [Login to Groundlight App](https://app.groundlight.ai/)
```

