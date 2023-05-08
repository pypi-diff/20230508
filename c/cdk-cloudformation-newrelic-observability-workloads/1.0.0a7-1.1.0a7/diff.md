# Comparing `tmp/cdk-cloudformation-newrelic-observability-workloads-1.0.0a7.tar.gz` & `tmp/cdk-cloudformation-newrelic-observability-workloads-1.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/newrelic-observability-workloads/dist/python/cdk-cloudf", last modified: Fri Feb  3 16:13:13 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/newrelic-observability-workloads/dist/python/cdk-cloudf", last modified: Mon May  8 06:13:26 2023, max compression
```

## Comparing `cdk-cloudformation-newrelic-observability-workloads-1.0.0a7.tar` & `cdk-cloudformation-newrelic-observability-workloads-1.1.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-02-03 16:13:05.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-02-03 16:13:05.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3071 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2114 2023-02-03 16:13:05.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      236 2023-02-03 16:13:05.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1959 2023-02-03 16:13:05.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     9978 2023-02-03 16:13:05.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      480 2023-02-03 16:13:05.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    17427 2023-02-03 16:13:05.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads/_jsii/newrelic-observability-workloads@1.0.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:13:05.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3071 2023-02-03 16:13:12.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      772 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:13:12.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       52 2023-02-03 16:13:13.000000 cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:26.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-05-08 06:13:16.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-05-08 06:13:16.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3102 2023-05-08 06:13:26.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2114 2023-05-08 06:13:16.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-05-08 06:13:16.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-05-08 06:13:26.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2008 2023-05-08 06:13:16.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:26.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:26.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     8842 2023-05-08 06:13:16.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:26.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      480 2023-05-08 06:13:16.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    17306 2023-05-08 06:13:16.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads/_jsii/newrelic-observability-workloads@1.1.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-08 06:13:16.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:26.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3102 2023-05-08 06:13:25.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      772 2023-05-08 06:13:25.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-08 06:13:25.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-05-08 06:13:25.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       52 2023-05-08 06:13:25.000000 cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/LICENSE` & `cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/PKG-INFO` & `cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-newrelic-observability-workloads
-Version: 1.0.0a7
+Version: 1.1.0a7
 Summary: CRUD operations for New Relic Workloads via the NerdGraph API
 Home-page: https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-workloads
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # newrelic-observability-workloads
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Workloads` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Workloads` v1.1.0.
 
 ## Description
 
 CRUD operations for New Relic Workloads via the NerdGraph API
 
 ## References
 
@@ -55,15 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Workloads`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-workloads+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-workloads+v1.1.0).
 * Issues related to `NewRelic::Observability::Workloads` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-workloads).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/README.md` & `cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # newrelic-observability-workloads
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Workloads` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Workloads` v1.1.0.
 
 ## Description
 
 CRUD operations for New Relic Workloads via the NerdGraph API
 
 ## References
 
@@ -32,13 +32,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Workloads`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-workloads+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-workloads+v1.1.0).
 * Issues related to `NewRelic::Observability::Workloads` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-workloads).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/setup.py` & `cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-newrelic-observability-workloads",
-    "version": "1.0.0.a7",
+    "version": "1.1.0.a7",
     "description": "CRUD operations for New Relic Workloads via the NerdGraph API",
     "license": "Apache-2.0",
     "url": "https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-workloads",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_cloudformation_newrelic_observability_workloads",
         "cdk_cloudformation_newrelic_observability_workloads._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_newrelic_observability_workloads._jsii": [
-            "newrelic-observability-workloads@1.0.0-alpha.7.jsii.tgz"
+            "newrelic-observability-workloads@1.1.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_newrelic_observability_workloads": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.63.0, <3.0.0",
-        "constructs>=10.1.239, <11.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "aws-cdk-lib>=2.78.0, <3.0.0",
+        "constructs>=10.2.17, <11.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
 )
```

### Comparing `cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads/__init__.py` & `cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # newrelic-observability-workloads
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Workloads` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Workloads` v1.1.0.
 
 ## Description
 
 CRUD operations for New Relic Workloads via the NerdGraph API
 
 ## References
 
@@ -33,15 +33,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Workloads`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-workloads+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-workloads+v1.1.0).
 * Issues related to `NewRelic::Observability::Workloads` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-workloads).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
@@ -74,38 +74,35 @@
     '''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        duplicate_name: typing.Optional[builtins.str] = None,
         list_query_filter: typing.Optional[builtins.str] = None,
-        source_guid: typing.Optional[builtins.str] = None,
+        tags: typing.Any = None,
         variables: typing.Any = None,
         workload: typing.Optional[builtins.str] = None,
     ) -> None:
         '''Create a new ``NewRelic::Observability::Workloads``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
-        :param duplicate_name: 
         :param list_query_filter: 
-        :param source_guid: 
+        :param tags: 
         :param variables: 
         :param workload: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__84822ac3c31b0d667a407c07951ba064e049dc2d6db5015d05df2378f09702df)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = CfnWorkloadsProps(
-            duplicate_name=duplicate_name,
             list_query_filter=list_query_filter,
-            source_guid=source_guid,
+            tags=tags,
             variables=variables,
             workload=workload,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.python.classproperty
@@ -130,83 +127,69 @@
         return typing.cast("CfnWorkloadsProps", jsii.get(self, "props"))
 
 
 @jsii.data_type(
     jsii_type="@cdk-cloudformation/newrelic-observability-workloads.CfnWorkloadsProps",
     jsii_struct_bases=[],
     name_mapping={
-        "duplicate_name": "duplicateName",
         "list_query_filter": "listQueryFilter",
-        "source_guid": "sourceGuid",
+        "tags": "tags",
         "variables": "variables",
         "workload": "workload",
     },
 )
 class CfnWorkloadsProps:
     def __init__(
         self,
         *,
-        duplicate_name: typing.Optional[builtins.str] = None,
         list_query_filter: typing.Optional[builtins.str] = None,
-        source_guid: typing.Optional[builtins.str] = None,
+        tags: typing.Any = None,
         variables: typing.Any = None,
         workload: typing.Optional[builtins.str] = None,
     ) -> None:
         '''CRUD operations for New Relic Workloads via the NerdGraph API.
 
-        :param duplicate_name: 
         :param list_query_filter: 
-        :param source_guid: 
+        :param tags: 
         :param variables: 
         :param workload: 
 
         :schema: CfnWorkloadsProps
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__282ab5bf2b30c52830b65bfbbec7234cd95397e6f378010a0ab8fbffca622624)
-            check_type(argname="argument duplicate_name", value=duplicate_name, expected_type=type_hints["duplicate_name"])
             check_type(argname="argument list_query_filter", value=list_query_filter, expected_type=type_hints["list_query_filter"])
-            check_type(argname="argument source_guid", value=source_guid, expected_type=type_hints["source_guid"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument variables", value=variables, expected_type=type_hints["variables"])
             check_type(argname="argument workload", value=workload, expected_type=type_hints["workload"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if duplicate_name is not None:
-            self._values["duplicate_name"] = duplicate_name
         if list_query_filter is not None:
             self._values["list_query_filter"] = list_query_filter
-        if source_guid is not None:
-            self._values["source_guid"] = source_guid
+        if tags is not None:
+            self._values["tags"] = tags
         if variables is not None:
             self._values["variables"] = variables
         if workload is not None:
             self._values["workload"] = workload
 
     @builtins.property
-    def duplicate_name(self) -> typing.Optional[builtins.str]:
-        '''
-        :schema: CfnWorkloadsProps#DuplicateName
-        '''
-        result = self._values.get("duplicate_name")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
     def list_query_filter(self) -> typing.Optional[builtins.str]:
         '''
         :schema: CfnWorkloadsProps#ListQueryFilter
         '''
         result = self._values.get("list_query_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def source_guid(self) -> typing.Optional[builtins.str]:
+    def tags(self) -> typing.Any:
         '''
-        :schema: CfnWorkloadsProps#SourceGuid
+        :schema: CfnWorkloadsProps#Tags
         '''
-        result = self._values.get("source_guid")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("tags")
+        return typing.cast(typing.Any, result)
 
     @builtins.property
     def variables(self) -> typing.Any:
         '''
         :schema: CfnWorkloadsProps#Variables
         '''
         result = self._values.get("variables")
@@ -239,26 +222,24 @@
 
 publication.publish()
 
 def _typecheckingstub__84822ac3c31b0d667a407c07951ba064e049dc2d6db5015d05df2378f09702df(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
-    duplicate_name: typing.Optional[builtins.str] = None,
     list_query_filter: typing.Optional[builtins.str] = None,
-    source_guid: typing.Optional[builtins.str] = None,
+    tags: typing.Any = None,
     variables: typing.Any = None,
     workload: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__282ab5bf2b30c52830b65bfbbec7234cd95397e6f378010a0ab8fbffca622624(
     *,
-    duplicate_name: typing.Optional[builtins.str] = None,
     list_query_filter: typing.Optional[builtins.str] = None,
-    source_guid: typing.Optional[builtins.str] = None,
+    tags: typing.Any = None,
     variables: typing.Any = None,
     workload: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/PKG-INFO` & `cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-newrelic-observability-workloads
-Version: 1.0.0a7
+Version: 1.1.0a7
 Summary: CRUD operations for New Relic Workloads via the NerdGraph API
 Home-page: https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-workloads
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # newrelic-observability-workloads
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Workloads` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Workloads` v1.1.0.
 
 ## Description
 
 CRUD operations for New Relic Workloads via the NerdGraph API
 
 ## References
 
@@ -55,15 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Workloads`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-workloads+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-workloads+v1.1.0).
 * Issues related to `NewRelic::Observability::Workloads` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-workloads).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-newrelic-observability-workloads-1.0.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/SOURCES.txt` & `cdk-cloudformation-newrelic-observability-workloads-1.1.0a7/src/cdk_cloudformation_newrelic_observability_workloads.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_newrelic_observability_workloads/py.typed
 src/cdk_cloudformation_newrelic_observability_workloads.egg-info/PKG-INFO
 src/cdk_cloudformation_newrelic_observability_workloads.egg-info/SOURCES.txt
 src/cdk_cloudformation_newrelic_observability_workloads.egg-info/dependency_links.txt
 src/cdk_cloudformation_newrelic_observability_workloads.egg-info/requires.txt
 src/cdk_cloudformation_newrelic_observability_workloads.egg-info/top_level.txt
 src/cdk_cloudformation_newrelic_observability_workloads/_jsii/__init__.py
-src/cdk_cloudformation_newrelic_observability_workloads/_jsii/newrelic-observability-workloads@1.0.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_newrelic_observability_workloads/_jsii/newrelic-observability-workloads@1.1.0-alpha.7.jsii.tgz
```

