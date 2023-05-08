# Comparing `tmp/cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7.tar.gz` & `tmp/cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/newrelic-observability-dashboards/dist/python/cdk-cloud", last modified: Mon Apr 24 06:13:08 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/newrelic-observability-dashboards/dist/python/cdk-cloud", last modified: Mon May  8 06:13:30 2023, max compression
```

## Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7.tar` & `cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3115 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2124 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2017 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     9007 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      482 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    17384 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/newrelic-observability-dashboards@1.1.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3115 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      782 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       53 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-05-08 06:13:23.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-05-08 06:13:23.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3115 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2124 2023-05-08 06:13:23.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-05-08 06:13:23.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2016 2023-05-08 06:13:23.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     8895 2023-05-08 06:13:23.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      482 2023-05-08 06:13:23.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    17379 2023-05-08 06:13:23.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/newrelic-observability-dashboards@1.2.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-08 06:13:23.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3115 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      782 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       53 2023-05-08 06:13:30.000000 cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/LICENSE` & `cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/PKG-INFO` & `cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-newrelic-observability-dashboards
-Version: 1.1.0a7
+Version: 1.2.0a7
 Summary: CRUD operations for New Relic Dashboards via the NerdGraph API
 Home-page: https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # newrelic-observability-dashboards
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.1.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.2.0.
 
 ## Description
 
 CRUD operations for New Relic Dashboards via the NerdGraph API
 
 ## References
 
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Dashboards`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.1.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.2.0).
 * Issues related to `NewRelic::Observability::Dashboards` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/README.md` & `cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # newrelic-observability-dashboards
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.1.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.2.0.
 
 ## Description
 
 CRUD operations for New Relic Dashboards via the NerdGraph API
 
 ## References
 
@@ -32,13 +32,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Dashboards`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.1.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.2.0).
 * Issues related to `NewRelic::Observability::Dashboards` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/setup.py` & `cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-newrelic-observability-dashboards",
-    "version": "1.1.0.a7",
+    "version": "1.2.0.a7",
     "description": "CRUD operations for New Relic Dashboards via the NerdGraph API",
     "license": "Apache-2.0",
     "url": "https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cdk_cloudformation_newrelic_observability_dashboards",
         "cdk_cloudformation_newrelic_observability_dashboards._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_newrelic_observability_dashboards._jsii": [
-            "newrelic-observability-dashboards@1.1.0-alpha.7.jsii.tgz"
+            "newrelic-observability-dashboards@1.2.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_newrelic_observability_dashboards": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.72.1, <3.0.0",
-        "constructs>=10.1.302, <11.0.0",
+        "aws-cdk-lib>=2.78.0, <3.0.0",
+        "constructs>=10.2.17, <11.0.0",
         "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/__init__.py` & `cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # newrelic-observability-dashboards
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.1.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.2.0.
 
 ## Description
 
 CRUD operations for New Relic Dashboards via the NerdGraph API
 
 ## References
 
@@ -33,15 +33,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Dashboards`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.1.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.2.0).
 * Issues related to `NewRelic::Observability::Dashboards` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
@@ -74,34 +74,34 @@
     '''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        dashboard_input: typing.Optional[builtins.str] = None,
+        dashboard: typing.Optional[builtins.str] = None,
         list_query_filter: typing.Optional[builtins.str] = None,
         tags: typing.Any = None,
         variables: typing.Any = None,
     ) -> None:
         '''Create a new ``NewRelic::Observability::Dashboards``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
-        :param dashboard_input: 
+        :param dashboard: 
         :param list_query_filter: 
         :param tags: 
         :param variables: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__83e95e1c81e5cebb3699baa93ba5fa3ab2a7fe50fff55eea029f7df8749ddf31)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = CfnDashboardsProps(
-            dashboard_input=dashboard_input,
+            dashboard=dashboard,
             list_query_filter=list_query_filter,
             tags=tags,
             variables=variables,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
@@ -127,60 +127,60 @@
         return typing.cast("CfnDashboardsProps", jsii.get(self, "props"))
 
 
 @jsii.data_type(
     jsii_type="@cdk-cloudformation/newrelic-observability-dashboards.CfnDashboardsProps",
     jsii_struct_bases=[],
     name_mapping={
-        "dashboard_input": "dashboardInput",
+        "dashboard": "dashboard",
         "list_query_filter": "listQueryFilter",
         "tags": "tags",
         "variables": "variables",
     },
 )
 class CfnDashboardsProps:
     def __init__(
         self,
         *,
-        dashboard_input: typing.Optional[builtins.str] = None,
+        dashboard: typing.Optional[builtins.str] = None,
         list_query_filter: typing.Optional[builtins.str] = None,
         tags: typing.Any = None,
         variables: typing.Any = None,
     ) -> None:
         '''CRUD operations for New Relic Dashboards via the NerdGraph API.
 
-        :param dashboard_input: 
+        :param dashboard: 
         :param list_query_filter: 
         :param tags: 
         :param variables: 
 
         :schema: CfnDashboardsProps
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e8ec58d72d07b15ae7381ca0f66880525b482ca312572db04ef2a9c0fc7fd82b)
-            check_type(argname="argument dashboard_input", value=dashboard_input, expected_type=type_hints["dashboard_input"])
+            check_type(argname="argument dashboard", value=dashboard, expected_type=type_hints["dashboard"])
             check_type(argname="argument list_query_filter", value=list_query_filter, expected_type=type_hints["list_query_filter"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument variables", value=variables, expected_type=type_hints["variables"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if dashboard_input is not None:
-            self._values["dashboard_input"] = dashboard_input
+        if dashboard is not None:
+            self._values["dashboard"] = dashboard
         if list_query_filter is not None:
             self._values["list_query_filter"] = list_query_filter
         if tags is not None:
             self._values["tags"] = tags
         if variables is not None:
             self._values["variables"] = variables
 
     @builtins.property
-    def dashboard_input(self) -> typing.Optional[builtins.str]:
+    def dashboard(self) -> typing.Optional[builtins.str]:
         '''
-        :schema: CfnDashboardsProps#DashboardInput
+        :schema: CfnDashboardsProps#Dashboard
         '''
-        result = self._values.get("dashboard_input")
+        result = self._values.get("dashboard")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def list_query_filter(self) -> typing.Optional[builtins.str]:
         '''
         :schema: CfnDashboardsProps#ListQueryFilter
         '''
@@ -222,24 +222,24 @@
 
 publication.publish()
 
 def _typecheckingstub__83e95e1c81e5cebb3699baa93ba5fa3ab2a7fe50fff55eea029f7df8749ddf31(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
-    dashboard_input: typing.Optional[builtins.str] = None,
+    dashboard: typing.Optional[builtins.str] = None,
     list_query_filter: typing.Optional[builtins.str] = None,
     tags: typing.Any = None,
     variables: typing.Any = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__e8ec58d72d07b15ae7381ca0f66880525b482ca312572db04ef2a9c0fc7fd82b(
     *,
-    dashboard_input: typing.Optional[builtins.str] = None,
+    dashboard: typing.Optional[builtins.str] = None,
     list_query_filter: typing.Optional[builtins.str] = None,
     tags: typing.Any = None,
     variables: typing.Any = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO` & `cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-newrelic-observability-dashboards
-Version: 1.1.0a7
+Version: 1.2.0a7
 Summary: CRUD operations for New Relic Dashboards via the NerdGraph API
 Home-page: https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # newrelic-observability-dashboards
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.1.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.2.0.
 
 ## Description
 
 CRUD operations for New Relic Dashboards via the NerdGraph API
 
 ## References
 
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Dashboards`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.1.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.2.0).
 * Issues related to `NewRelic::Observability::Dashboards` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt` & `cdk-cloudformation-newrelic-observability-dashboards-1.2.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_newrelic_observability_dashboards/py.typed
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/dependency_links.txt
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/requires.txt
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/top_level.txt
 src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/__init__.py
-src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/newrelic-observability-dashboards@1.1.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/newrelic-observability-dashboards@1.2.0-alpha.7.jsii.tgz
```

