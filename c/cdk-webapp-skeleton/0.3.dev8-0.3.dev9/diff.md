# Comparing `tmp/cdk_webapp_skeleton-0.3.dev8.tar.gz` & `tmp/cdk_webapp_skeleton-0.3.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.3.dev8.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.3.dev9.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.3.dev8.tar` & `cdk_webapp_skeleton-0.3.dev9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev8/README.md
--rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/auth_stack.py
--rw-r--r--   0        0        0     1544 2023-04-18 21:19:44.807699 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/react_website.py
--rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0     4334 2023-04-18 21:50:57.522135 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/webapp_lambda.py
--rw-r--r--   0        0        0      593 2023-04-18 21:51:50.214877 cdk_webapp_skeleton-0.3.dev8/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev9/README.md
+-rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     1544 2023-04-18 21:19:44.807699 cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     4442 2023-04-18 23:59:14.698730 cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0      593 2023-04-18 23:59:14.686730 cdk_webapp_skeleton-0.3.dev9/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev9/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/auth_stack.py` & `cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/auth_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/branch_config.py` & `cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/branch_config.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/react_website.py` & `cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/react_website.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/webapp_lambda.py` & `cdk_webapp_skeleton-0.3.dev9/cdk_webapp_skeleton/webapp_lambda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from aws_cdk import aws_apigateway as apigateway
 from aws_cdk import aws_certificatemanager as certificatemanager
 from aws_cdk import aws_cloudwatch as cloudwatch
 from aws_cdk import aws_codeguruprofiler as codeguruprofiler
 from aws_cdk import aws_lambda as _lambda
 from aws_cdk import aws_logs as logs
 from aws_cdk import aws_route53 as route53
@@ -15,16 +17,17 @@
     """Assumes a local folder called "webapp-backend" with a Dockerfile in it."""
 
     def __init__(
         self,
         scope: "Construct",
         _id: str,
         branch_config: BranchConfig,
-        lambda_runtime_environment=None,
         image_directory="webapp-backend",
+        lambda_runtime_environment=None,
+        memory_size: Optional[int] = 256,
     ):
         super().__init__(scope, _id)
         if lambda_runtime_environment is None:
             lambda_runtime_environment = {}
 
         profiling_group = codeguruprofiler.ProfilingGroup(
             scope,
@@ -39,14 +42,15 @@
         )
 
         self.webapp_lambda_func = _lambda.DockerImageFunction(
             scope,
             "FlaskLambda",
             code=_lambda.DockerImageCode.from_image_asset(directory=image_directory),
             environment=lambda_runtime_environment,
+            memory_size=memory_size,
             tracing=_lambda.Tracing.ACTIVE,
         )
         profiling_group.grant_publish(self.webapp_lambda_func)
 
         logs.MetricFilter(
             scope,
             "FlaskLambdaTimeouts",
```

### Comparing `cdk_webapp_skeleton-0.3.dev8/pyproject.toml` & `cdk_webapp_skeleton-0.3.dev9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdk-webapp-skeleton"
-version = "0.3.dev8"
+version = "0.3.dev9"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cdk_webapp_skeleton"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `cdk_webapp_skeleton-0.3.dev8/PKG-INFO` & `cdk_webapp_skeleton-0.3.dev9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.3.dev8
+Version: 0.3.dev9
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

