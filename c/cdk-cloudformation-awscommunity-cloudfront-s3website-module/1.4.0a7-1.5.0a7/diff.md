# Comparing `tmp/cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7.tar.gz` & `tmp/cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-cloudfront-s3website-module/dist/python/cd", last modified: Mon Apr 10 06:14:32 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-cloudfront-s3website-module/dist/python/cd", last modified: Mon May  8 06:12:53 2023, max compression
```

## Comparing `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7.tar` & `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-04-10 06:14:25.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-10 06:14:25.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2950 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1981 2023-04-10 06:14:25.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-04-10 06:14:25.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2030 2023-04-10 06:14:25.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    40837 2023-04-10 06:14:25.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      496 2023-04-10 06:14:25.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    22253 2023-04-10 06:14:25.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/_jsii/awscommunity-cloudfront-s3website-module@1.4.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-10 06:14:25.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2950 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      852 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       60 2023-04-10 06:14:32.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-05-08 06:12:47.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-05-08 06:12:47.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2950 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1981 2023-05-08 06:12:47.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-05-08 06:12:47.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2029 2023-05-08 06:12:47.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    40837 2023-05-08 06:12:47.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      496 2023-05-08 06:12:47.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    22251 2023-05-08 06:12:47.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/_jsii/awscommunity-cloudfront-s3website-module@1.5.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-08 06:12:47.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2950 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      852 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       60 2023-05-08 06:12:53.000000 cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/LICENSE` & `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/PKG-INFO` & `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-cloudfront-s3website-module
-Version: 1.4.0a7
+Version: 1.5.0a7
 Summary: Schema for Module Fragment of type AwsCommunity::CloudFront::S3Website::MODULE
 Home-page: https://github.com/cdklabs/cdk-cloudformation.git
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
 
 # awscommunity-cloudfront-s3website-module
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::CloudFront::S3Website::MODULE` v1.4.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::CloudFront::S3Website::MODULE` v1.5.0.
 
 ## Description
 
 Schema for Module Fragment of type AwsCommunity::CloudFront::S3Website::MODULE
 
 ## Usage
 
@@ -51,13 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::CloudFront::S3Website::MODULE`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-cloudfront-s3website-module+v1.4.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-cloudfront-s3website-module+v1.5.0).
 * Issues related to `AwsCommunity::CloudFront::S3Website::MODULE` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/README.md` & `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # awscommunity-cloudfront-s3website-module
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::CloudFront::S3Website::MODULE` v1.4.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::CloudFront::S3Website::MODULE` v1.5.0.
 
 ## Description
 
 Schema for Module Fragment of type AwsCommunity::CloudFront::S3Website::MODULE
 
 ## Usage
 
@@ -28,13 +28,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::CloudFront::S3Website::MODULE`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-cloudfront-s3website-module+v1.4.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-cloudfront-s3website-module+v1.5.0).
 * Issues related to `AwsCommunity::CloudFront::S3Website::MODULE` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/setup.py` & `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-awscommunity-cloudfront-s3website-module",
-    "version": "1.4.0.a7",
+    "version": "1.5.0.a7",
     "description": "Schema for Module Fragment of type AwsCommunity::CloudFront::S3Website::MODULE",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-cloudformation.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cdk_cloudformation_awscommunity_cloudfront_s3website_module",
         "cdk_cloudformation_awscommunity_cloudfront_s3website_module._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_awscommunity_cloudfront_s3website_module._jsii": [
-            "awscommunity-cloudfront-s3website-module@1.4.0-alpha.7.jsii.tgz"
+            "awscommunity-cloudfront-s3website-module@1.5.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_awscommunity_cloudfront_s3website_module": [
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

### Comparing `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/__init__.py` & `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # awscommunity-cloudfront-s3website-module
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::CloudFront::S3Website::MODULE` v1.4.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::CloudFront::S3Website::MODULE` v1.5.0.
 
 ## Description
 
 Schema for Module Fragment of type AwsCommunity::CloudFront::S3Website::MODULE
 
 ## Usage
 
@@ -29,15 +29,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::CloudFront::S3Website::MODULE`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-cloudfront-s3website-module+v1.4.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-cloudfront-s3website-module+v1.5.0).
 * Issues related to `AwsCommunity::CloudFront::S3Website::MODULE` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
```

### Comparing `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/PKG-INFO` & `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-cloudfront-s3website-module
-Version: 1.4.0a7
+Version: 1.5.0a7
 Summary: Schema for Module Fragment of type AwsCommunity::CloudFront::S3Website::MODULE
 Home-page: https://github.com/cdklabs/cdk-cloudformation.git
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
 
 # awscommunity-cloudfront-s3website-module
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::CloudFront::S3Website::MODULE` v1.4.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::CloudFront::S3Website::MODULE` v1.5.0.
 
 ## Description
 
 Schema for Module Fragment of type AwsCommunity::CloudFront::S3Website::MODULE
 
 ## Usage
 
@@ -51,13 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::CloudFront::S3Website::MODULE`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-cloudfront-s3website-module+v1.4.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-cloudfront-s3website-module+v1.5.0).
 * Issues related to `AwsCommunity::CloudFront::S3Website::MODULE` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.4.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/SOURCES.txt` & `cdk-cloudformation-awscommunity-cloudfront-s3website-module-1.5.0a7/src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/py.typed
 src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/PKG-INFO
 src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/SOURCES.txt
 src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/dependency_links.txt
 src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/requires.txt
 src/cdk_cloudformation_awscommunity_cloudfront_s3website_module.egg-info/top_level.txt
 src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/_jsii/__init__.py
-src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/_jsii/awscommunity-cloudfront-s3website-module@1.4.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_awscommunity_cloudfront_s3website_module/_jsii/awscommunity-cloudfront-s3website-module@1.5.0-alpha.7.jsii.tgz
```

