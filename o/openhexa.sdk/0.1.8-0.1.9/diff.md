# Comparing `tmp/openhexa.sdk-0.1.8.tar.gz` & `tmp/openhexa.sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.sdk-0.1.8.tar", last modified: Tue May  2 12:08:29 2023, max compression
+gzip compressed data, was "openhexa.sdk-0.1.9.tar", last modified: Mon May  8 07:05:12 2023, max compression
```

## Comparing `openhexa.sdk-0.1.8.tar` & `openhexa.sdk-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:29.719538 openhexa.sdk-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-02 12:08:29.719538 openhexa.sdk-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:29.715538 openhexa.sdk-0.1.8/openhexa/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:29.715538 openhexa.sdk-0.1.8/openhexa/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/cli/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:29.719538 openhexa.sdk-0.1.8/openhexa/cli/skeleton/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/cli/skeleton/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/cli/skeleton/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/cli/skeleton/workspace.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:29.719538 openhexa.sdk-0.1.8/openhexa/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:29.719538 openhexa.sdk-0.1.8/openhexa/sdk/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/pipelines/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/pipelines/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/pipelines/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/pipelines/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/pipelines/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/pipelines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:29.719538 openhexa.sdk-0.1.8/openhexa/sdk/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/workspaces/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/openhexa/sdk/workspaces/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:29.715538 openhexa.sdk-0.1.8/openhexa.sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-02 12:08:29.000000 openhexa.sdk-0.1.8/openhexa.sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-02 12:08:29.000000 openhexa.sdk-0.1.8/openhexa.sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:08:29.000000 openhexa.sdk-0.1.8/openhexa.sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 12:08:29.000000 openhexa.sdk-0.1.8/openhexa.sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-02 12:08:29.000000 openhexa.sdk-0.1.8/openhexa.sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 12:08:29.000000 openhexa.sdk-0.1.8/openhexa.sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:08:18.000000 openhexa.sdk-0.1.8/openhexa.sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-02 12:08:29.719538 openhexa.sdk-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:29.719538 openhexa.sdk-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-02 12:08:15.000000 openhexa.sdk-0.1.8/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:05:12.016502 openhexa.sdk-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-08 07:05:12.016502 openhexa.sdk-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:05:12.012502 openhexa.sdk-0.1.9/openhexa/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:05:12.012502 openhexa.sdk-0.1.9/openhexa/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:05:12.012502 openhexa.sdk-0.1.9/openhexa/cli/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/cli/skeleton/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/cli/skeleton/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/cli/skeleton/workspace.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:05:12.012502 openhexa.sdk-0.1.9/openhexa/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:05:12.016502 openhexa.sdk-0.1.9/openhexa/sdk/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/pipelines/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/pipelines/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/pipelines/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/pipelines/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/pipelines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:05:12.016502 openhexa.sdk-0.1.9/openhexa/sdk/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/workspaces/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/openhexa/sdk/workspaces/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:05:12.012502 openhexa.sdk-0.1.9/openhexa.sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-08 07:05:12.000000 openhexa.sdk-0.1.9/openhexa.sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-08 07:05:12.000000 openhexa.sdk-0.1.9/openhexa.sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:05:12.000000 openhexa.sdk-0.1.9/openhexa.sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 07:05:12.000000 openhexa.sdk-0.1.9/openhexa.sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 07:05:12.000000 openhexa.sdk-0.1.9/openhexa.sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 07:05:12.000000 openhexa.sdk-0.1.9/openhexa.sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:05:01.000000 openhexa.sdk-0.1.9/openhexa.sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-08 07:05:12.016502 openhexa.sdk-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:05:12.016502 openhexa.sdk-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-08 07:04:58.000000 openhexa.sdk-0.1.9/tests/test_workspace.py
```

### Comparing `openhexa.sdk-0.1.8/LICENCE` & `openhexa.sdk-0.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/PKG-INFO` & `openhexa.sdk-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenHexa SDK
 Home-page: https://github.com/BLSQ/openhexa-sdk-python
 Author: Bluesquare
 Author-email: dev@bluesquarehub.com
 License: MIT License
 Keywords: openhexa,pipelines
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openhexa.sdk-0.1.8/README.md` & `openhexa.sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/openhexa/cli/api.py` & `openhexa.sdk-0.1.9/openhexa/cli/api.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/openhexa/cli/cli.py` & `openhexa.sdk-0.1.9/openhexa/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/openhexa/sdk/pipelines/parameter.py` & `openhexa.sdk-0.1.9/openhexa/sdk/pipelines/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import typing
 
 
 class ParameterValueError(Exception):
     pass
 
 
@@ -28,15 +29,16 @@
         return True
 
     @staticmethod
     def normalize(value: typing.Any) -> typing.Any:
         """If appropriate, subclasses can override this method to normalize empty values to None.
 
         This can be used to handle empty values and normalize them to None, or to perform type conversions, allowing us
-        to allow multiple input types but still normalize everything to a single type."""
+        to allow multiple input types but still normalize everything to a single type.
+        """
 
         return value
 
     def validate(
         self, value: typing.Optional[typing.Any], allow_empty: bool = True
     ) -> typing.Optional[typing.Any]:
         """Validate the provided value for this type."""
@@ -145,14 +147,19 @@
         name: typing.Optional[str] = None,
         choices: typing.Optional[typing.Sequence] = None,
         help: typing.Optional[str] = None,
         default: typing.Optional[typing.Any] = None,
         required: bool = True,
         multiple: bool = False,
     ):
+        if re.match("^[a-z_][a-z_0-9]+$", code) is None:
+            raise InvalidParameterError(
+                f"Invalid parameter code provided ({code}). Parameter must start with a letter or an underscore, and can only contain lower case letters, numbers and underscores."
+            )
+
         self.code = code
 
         try:
             self.type = TYPES_BY_PYTHON_TYPE[type]()
         except KeyError:
             valid_parameter_types = [str(k) for k in TYPES_BY_PYTHON_TYPE.keys()]
             raise InvalidParameterError(
```

### Comparing `openhexa.sdk-0.1.8/openhexa/sdk/pipelines/pipeline.py` & `openhexa.sdk-0.1.9/openhexa/sdk/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/openhexa/sdk/pipelines/run.py` & `openhexa.sdk-0.1.9/openhexa/sdk/pipelines/run.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/openhexa/sdk/pipelines/runtime.py` & `openhexa.sdk-0.1.9/openhexa/sdk/pipelines/runtime.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/openhexa/sdk/pipelines/task.py` & `openhexa.sdk-0.1.9/openhexa/sdk/pipelines/task.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/openhexa/sdk/pipelines/utils.py` & `openhexa.sdk-0.1.9/openhexa/sdk/pipelines/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -124,7 +124,47 @@
                         ] = connection_config["database_name"]
                     except KeyError:
                         exception_message = (
                             "Invalid local workspace PostgreSQL connection config. Please make sure you provide "
                             "the following keys: url, username, password."
                         )
                         raise LocalWorkspaceConfigError(exception_message)
+                # S3 connections
+                elif connection_config["type"] == "s3":
+                    try:
+                        os.environ[
+                            f"{stringcase.constcase(slug)}_SECRET_ACCESS_KEY"
+                        ] = connection_config["secret_access_key"]
+                        os.environ[f"{stringcase.constcase(slug)}_ACCESS_KEY_ID"] = str(
+                            connection_config["access_key_id"]
+                        )
+                        os.environ[f"{stringcase.constcase(slug)}_BUCKET_NAME"] = str(
+                            connection_config["bucket_name"]
+                        )
+                    except KeyError:
+                        exception_message = (
+                            "Invalid local workspace S3 connection config. Please make sure you provide "
+                            "the following keys: secret_key, access_key_id, bucket_name."
+                        )
+                        raise LocalWorkspaceConfigError(exception_message)
+                # GCS connections
+                elif connection_config["type"] == "gcs":
+                    try:
+                        os.environ[
+                            f"{stringcase.constcase(slug)}_SERVICE_ACCOUNT_KEY"
+                        ] = connection_config["service_account_key"]
+                        os.environ[f"{stringcase.constcase(slug)}_BUCKET_NAME"] = str(
+                            connection_config["bucket_name"]
+                        )
+                    except KeyError:
+                        exception_message = (
+                            "Invalid local workspace GCS connection config. Please make sure you provide "
+                            "the following keys: service_account_key, bucket_name."
+                        )
+                        raise LocalWorkspaceConfigError(exception_message)
+                # Custom connection
+                else:
+                    for key, value in connection_config.items():
+                        if key != "type":
+                            os.environ[stringcase.constcase(f"{slug}_{key}")] = str(
+                                value
+                            )
```

### Comparing `openhexa.sdk-0.1.8/openhexa.sdk.egg-info/PKG-INFO` & `openhexa.sdk-0.1.9/openhexa.sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenHexa SDK
 Home-page: https://github.com/BLSQ/openhexa-sdk-python
 Author: Bluesquare
 Author-email: dev@bluesquarehub.com
 License: MIT License
 Keywords: openhexa,pipelines
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openhexa.sdk-0.1.8/openhexa.sdk.egg-info/SOURCES.txt` & `openhexa.sdk-0.1.9/openhexa.sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 openhexa/sdk/pipelines/task.py
 openhexa/sdk/pipelines/utils.py
 openhexa/sdk/workspaces/__init__.py
 openhexa/sdk/workspaces/connection.py
 openhexa/sdk/workspaces/workspace.py
 tests/__init__.py
 tests/test_parameter.py
-tests/test_pipeline.py
+tests/test_pipeline.py
+tests/test_workspace.py
```

### Comparing `openhexa.sdk-0.1.8/pyproject.toml` & `openhexa.sdk-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/setup.cfg` & `openhexa.sdk-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.8/tests/test_parameter.py` & `openhexa.sdk-0.1.9/tests/test_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,22 @@
 
 
 def test_parameter_init():
     # Wrong type
     with pytest.raises(InvalidParameterError):
         Parameter("arg", type="string")
 
+    # Wrong code
+    with pytest.raises(InvalidParameterError):
+        Parameter("-123", type=str)
+    with pytest.raises(InvalidParameterError):
+        Parameter("Abc", type=str)
+    with pytest.raises(InvalidParameterError):
+        Parameter("0_z", type=str)
+
     # Empty choices
     with pytest.raises(InvalidParameterError):
         Parameter("arg", type=str, choices=[])
 
     # Invalid choices
     with pytest.raises(InvalidParameterError):
         Parameter("arg", type=str, choices=[1, 2, 3])
```

### Comparing `openhexa.sdk-0.1.8/tests/test_pipeline.py` & `openhexa.sdk-0.1.9/tests/test_pipeline.py`

 * *Files identical despite different names*

