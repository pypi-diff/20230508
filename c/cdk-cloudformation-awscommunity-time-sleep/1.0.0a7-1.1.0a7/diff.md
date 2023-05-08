# Comparing `tmp/cdk-cloudformation-awscommunity-time-sleep-1.0.0a7.tar.gz` & `tmp/cdk-cloudformation-awscommunity-time-sleep-1.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-time-sleep/dist/python/cdk-cloudformation-", last modified: Mon Apr 10 06:14:30 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-time-sleep/dist/python/cdk-cloudformation-", last modified: Mon May  8 06:13:00 2023, max compression
```

## Comparing `cdk-cloudformation-awscommunity-time-sleep-1.0.0a7.tar` & `cdk-cloudformation-awscommunity-time-sleep-1.1.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:30.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-04-10 06:14:23.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-10 06:14:23.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2992 2023-04-10 06:14:30.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2018 2023-04-10 06:14:23.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-04-10 06:14:23.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-10 06:14:30.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1950 2023-04-10 06:14:23.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:30.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:30.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    10561 2023-04-10 06:14:23.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:30.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      462 2023-04-10 06:14:23.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    17812 2023-04-10 06:14:23.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep/_jsii/awscommunity-time-sleep@1.0.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-10 06:14:23.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:30.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2992 2023-04-10 06:14:29.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      682 2023-04-10 06:14:30.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-10 06:14:29.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-04-10 06:14:29.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       43 2023-04-10 06:14:29.000000 cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-05-08 06:12:54.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-05-08 06:12:54.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3002 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2026 2023-05-08 06:12:54.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-05-08 06:12:54.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1951 2023-05-08 06:12:54.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    10577 2023-05-08 06:12:54.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      462 2023-05-08 06:12:54.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    17841 2023-05-08 06:12:54.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep/_jsii/awscommunity-time-sleep@1.1.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-08 06:12:54.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3002 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      682 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       43 2023-05-08 06:13:00.000000 cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/LICENSE` & `cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/PKG-INFO` & `cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,18 @@
-Metadata-Version: 2.1
-Name: cdk-cloudformation-awscommunity-time-sleep
-Version: 1.0.0a7
-Summary: An example resource schema demonstrating some basic constructs and validation rules.
-Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git
-Author: Amazon Web Services
-License: Apache-2.0
-Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # awscommunity-time-sleep
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Time::Sleep` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Time::Sleep` v1.1.0.
 
 ## Description
 
-An example resource schema demonstrating some basic constructs and validation rules.
+Sleep a provided number of seconds between create, update, or delete operations.
 
 ## References
 
-* [Source](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git)
+* [Source](https://github.com/aws-cloudformation/community-registry-extensions.git)
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -55,13 +32,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Time::Sleep`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-time-sleep+v1.0.0).
-* Issues related to `AwsCommunity::Time::Sleep` should be reported to the [publisher](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-time-sleep+v1.1.0).
+* Issues related to `AwsCommunity::Time::Sleep` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/README.md` & `cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,41 @@
+Metadata-Version: 2.1
+Name: cdk-cloudformation-awscommunity-time-sleep
+Version: 1.1.0a7
+Summary: Sleep a provided number of seconds between create, update, or delete operations.
+Home-page: https://github.com/aws-cloudformation/community-registry-extensions.git
+Author: Amazon Web Services
+License: Apache-2.0
+Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Classifier: License :: OSI Approved
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # awscommunity-time-sleep
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Time::Sleep` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Time::Sleep` v1.1.0.
 
 ## Description
 
-An example resource schema demonstrating some basic constructs and validation rules.
+Sleep a provided number of seconds between create, update, or delete operations.
 
 ## References
 
-* [Source](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git)
+* [Source](https://github.com/aws-cloudformation/community-registry-extensions.git)
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -32,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Time::Sleep`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-time-sleep+v1.0.0).
-* Issues related to `AwsCommunity::Time::Sleep` should be reported to the [publisher](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-time-sleep+v1.1.0).
+* Issues related to `AwsCommunity::Time::Sleep` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/setup.py` & `cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-awscommunity-time-sleep",
-    "version": "1.0.0.a7",
-    "description": "An example resource schema demonstrating some basic constructs and validation rules.",
+    "version": "1.1.0.a7",
+    "description": "Sleep a provided number of seconds between create, update, or delete operations.",
     "license": "Apache-2.0",
-    "url": "https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git",
+    "url": "https://github.com/aws-cloudformation/community-registry-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
     },
     "project_urls": {
         "Source": "https://github.com/cdklabs/cdk-cloudformation.git"
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cdk_cloudformation_awscommunity_time_sleep",
         "cdk_cloudformation_awscommunity_time_sleep._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_awscommunity_time_sleep._jsii": [
-            "awscommunity-time-sleep@1.0.0-alpha.7.jsii.tgz"
+            "awscommunity-time-sleep@1.1.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_awscommunity_time_sleep": [
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

### Comparing `cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep/__init__.py` & `cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 '''
 # awscommunity-time-sleep
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Time::Sleep` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Time::Sleep` v1.1.0.
 
 ## Description
 
-An example resource schema demonstrating some basic constructs and validation rules.
+Sleep a provided number of seconds between create, update, or delete operations.
 
 ## References
 
-* [Source](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git)
+* [Source](https://github.com/aws-cloudformation/community-registry-extensions.git)
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -33,16 +33,16 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Time::Sleep`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-time-sleep+v1.0.0).
-* Issues related to `AwsCommunity::Time::Sleep` should be reported to the [publisher](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-time-sleep+v1.1.0).
+* Issues related to `AwsCommunity::Time::Sleep` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
 import builtins
@@ -66,15 +66,15 @@
     _aws_cdk_ceddda9d.CfnResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdk-cloudformation/awscommunity-time-sleep.CfnSleep",
 ):
     '''A CloudFormation ``AwsCommunity::Time::Sleep``.
 
     :cloudformationResource: AwsCommunity::Time::Sleep
-    :link: https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git
+    :link: https://github.com/aws-cloudformation/community-registry-extensions.git
     '''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
@@ -115,15 +115,15 @@
         return typing.cast(builtins.str, jsii.sget(cls, "CFN_RESOURCE_TYPE_NAME"))
 
     @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> builtins.str:
         '''Attribute ``AwsCommunity::Time::Sleep.Id``.
 
-        :link: https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git
+        :link: https://github.com/aws-cloudformation/community-registry-extensions.git
         '''
         return typing.cast(builtins.str, jsii.get(self, "attrId"))
 
     @builtins.property
     @jsii.member(jsii_name="props")
     def props(self) -> "CfnSleepProps":
         '''Resource props.'''
@@ -147,15 +147,15 @@
         *,
         seconds: jsii.Number,
         sleep_on_create: typing.Optional[builtins.bool] = None,
         sleep_on_delete: typing.Optional[builtins.bool] = None,
         sleep_on_update: typing.Optional[builtins.bool] = None,
         triggers: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
-        '''An example resource schema demonstrating some basic constructs and validation rules.
+        '''Sleep a provided number of seconds between create, update, or delete operations.
 
         :param seconds: The number of seconds to sleep for.
         :param sleep_on_create: If we should sleep on a create.
         :param sleep_on_delete: If we should sleep on a delete.
         :param sleep_on_update: If we should sleep on an update.
         :param triggers: A value to represent when a sleep should occur. Any time this is updated this resource will sleep.
```

### Comparing `cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/PKG-INFO` & `cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-time-sleep
-Version: 1.0.0a7
-Summary: An example resource schema demonstrating some basic constructs and validation rules.
-Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git
+Version: 1.1.0a7
+Summary: Sleep a provided number of seconds between create, update, or delete operations.
+Home-page: https://github.com/aws-cloudformation/community-registry-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -19,23 +19,23 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # awscommunity-time-sleep
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Time::Sleep` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Time::Sleep` v1.1.0.
 
 ## Description
 
-An example resource schema demonstrating some basic constructs and validation rules.
+Sleep a provided number of seconds between create, update, or delete operations.
 
 ## References
 
-* [Source](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git)
+* [Source](https://github.com/aws-cloudformation/community-registry-extensions.git)
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Time::Sleep`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-time-sleep+v1.0.0).
-* Issues related to `AwsCommunity::Time::Sleep` should be reported to the [publisher](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-time-sleep+v1.1.0).
+* Issues related to `AwsCommunity::Time::Sleep` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-time-sleep-1.0.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/SOURCES.txt` & `cdk-cloudformation-awscommunity-time-sleep-1.1.0a7/src/cdk_cloudformation_awscommunity_time_sleep.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_awscommunity_time_sleep/py.typed
 src/cdk_cloudformation_awscommunity_time_sleep.egg-info/PKG-INFO
 src/cdk_cloudformation_awscommunity_time_sleep.egg-info/SOURCES.txt
 src/cdk_cloudformation_awscommunity_time_sleep.egg-info/dependency_links.txt
 src/cdk_cloudformation_awscommunity_time_sleep.egg-info/requires.txt
 src/cdk_cloudformation_awscommunity_time_sleep.egg-info/top_level.txt
 src/cdk_cloudformation_awscommunity_time_sleep/_jsii/__init__.py
-src/cdk_cloudformation_awscommunity_time_sleep/_jsii/awscommunity-time-sleep@1.0.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_awscommunity_time_sleep/_jsii/awscommunity-time-sleep@1.1.0-alpha.7.jsii.tgz
```

