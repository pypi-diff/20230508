# Comparing `tmp/pulumi_minio-0.9.1a1681933919.tar.gz` & `tmp/pulumi_minio-0.9.1a1682440158.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_minio-0.9.1a1681933919.tar", last modified: Wed Apr 19 20:02:17 2023, max compression
+gzip compressed data, was "pulumi_minio-0.9.1a1682440158.tar", last modified: Tue Apr 25 16:33:27 2023, max compression
```

## Comparing `pulumi_minio-0.9.1a1681933919.tar` & `pulumi_minio-0.9.1a1682440158.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:02:17.215809 pulumi_minio-0.9.1a1681933919/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-19 20:02:17.211809 pulumi_minio-0.9.1a1681933919/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:02:17.211809 pulumi_minio-0.9.1a1681933919/pulumi_minio/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:02:17.211809 pulumi_minio-0.9.1a1681933919/pulumi_minio/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/get_iam_policy_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group_policy_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group_user_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_user_policy_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/ilm_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/s3_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/s3_bucket_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/s3_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/s3_bucket_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio/s3_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:02:17.211809 pulumi_minio-0.9.1a1681933919/pulumi_minio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-19 20:02:17.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 20:02:17.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:02:17.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:02:17.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 20:02:17.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 20:02:17.000000 pulumi_minio-0.9.1a1681933919/pulumi_minio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:02:17.215809 pulumi_minio-0.9.1a1681933919/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-19 20:02:16.000000 pulumi_minio-0.9.1a1681933919/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:27.199635 pulumi_minio-0.9.1a1682440158/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-25 16:33:27.199635 pulumi_minio-0.9.1a1682440158/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:27.199635 pulumi_minio-0.9.1a1682440158/pulumi_minio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:27.199635 pulumi_minio-0.9.1a1682440158/pulumi_minio/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/get_iam_policy_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_group_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_group_policy_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_group_user_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_user_policy_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/ilm_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_bucket_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_bucket_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:27.199635 pulumi_minio-0.9.1a1682440158/pulumi_minio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-25 16:33:27.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 16:33:27.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:33:27.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:33:27.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 16:33:27.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 16:33:27.000000 pulumi_minio-0.9.1a1682440158/pulumi_minio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:33:27.199635 pulumi_minio-0.9.1a1682440158/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-25 16:33:26.000000 pulumi_minio-0.9.1a1682440158/setup.py
```

### Comparing `pulumi_minio-0.9.1a1681933919/PKG-INFO` & `pulumi_minio-0.9.1a1682440158/pulumi_minio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi_minio
-Version: 0.9.1a1681933919
+Name: pulumi-minio
+Version: 0.9.1a1682440158
 Summary: A Pulumi package for creating and managing minio cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-minio
 Keywords: pulumi minio
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-minio/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-minio/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fminio.svg)](https://www.npmjs.com/package/@pulumi/minio)
 [![Python version](https://badge.fury.io/py/pulumi-minio.svg)](https://pypi.org/project/pulumi-minio)
 [![NuGet version](https://badge.fury.io/nu/pulumi.minio.svg)](https://badge.fury.io/nu/pulumi.minio)
```

### Comparing `pulumi_minio-0.9.1a1681933919/README.md` & `pulumi_minio-0.9.1a1682440158/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/__init__.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/_inputs.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/_utilities.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/config/vars.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/get_iam_policy_document.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/get_iam_policy_document.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group_membership.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group_policy.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_group_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group_policy_attachment.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_group_user_attachment.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,218 +5,192 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['IamGroupPolicyAttachmentArgs', 'IamGroupPolicyAttachment']
+__all__ = ['IamGroupUserAttachmentArgs', 'IamGroupUserAttachment']
 
 @pulumi.input_type
-class IamGroupPolicyAttachmentArgs:
+class IamGroupUserAttachmentArgs:
     def __init__(__self__, *,
                  group_name: pulumi.Input[str],
-                 policy_name: pulumi.Input[str]):
+                 user_name: pulumi.Input[str]):
         """
-        The set of arguments for constructing a IamGroupPolicyAttachment resource.
+        The set of arguments for constructing a IamGroupUserAttachment resource.
         """
         pulumi.set(__self__, "group_name", group_name)
-        pulumi.set(__self__, "policy_name", policy_name)
+        pulumi.set(__self__, "user_name", user_name)
 
     @property
     @pulumi.getter(name="groupName")
     def group_name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "group_name")
 
     @group_name.setter
     def group_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "group_name", value)
 
     @property
-    @pulumi.getter(name="policyName")
-    def policy_name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "policy_name")
-
-    @policy_name.setter
-    def policy_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "policy_name", value)
+    @pulumi.getter(name="userName")
+    def user_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "user_name")
+
+    @user_name.setter
+    def user_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "user_name", value)
 
 
 @pulumi.input_type
-class _IamGroupPolicyAttachmentState:
+class _IamGroupUserAttachmentState:
     def __init__(__self__, *,
                  group_name: Optional[pulumi.Input[str]] = None,
-                 policy_name: Optional[pulumi.Input[str]] = None):
+                 user_name: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering IamGroupPolicyAttachment resources.
+        Input properties used for looking up and filtering IamGroupUserAttachment resources.
         """
         if group_name is not None:
             pulumi.set(__self__, "group_name", group_name)
-        if policy_name is not None:
-            pulumi.set(__self__, "policy_name", policy_name)
+        if user_name is not None:
+            pulumi.set(__self__, "user_name", user_name)
 
     @property
     @pulumi.getter(name="groupName")
     def group_name(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "group_name")
 
     @group_name.setter
     def group_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group_name", value)
 
     @property
-    @pulumi.getter(name="policyName")
-    def policy_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "policy_name")
+    @pulumi.getter(name="userName")
+    def user_name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "user_name")
 
-    @policy_name.setter
-    def policy_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "policy_name", value)
+    @user_name.setter
+    def user_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_name", value)
 
 
-class IamGroupPolicyAttachment(pulumi.CustomResource):
+class IamGroupUserAttachment(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  group_name: Optional[pulumi.Input[str]] = None,
-                 policy_name: Optional[pulumi.Input[str]] = None,
+                 user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_minio as minio
 
         developer_iam_group = minio.IamGroup("developerIamGroup")
-        test_policy = minio.IamGroupPolicy("testPolicy", policy=\"\"\"{
-          "Version":"2012-10-17",
-          "Statement": [
-            {
-              "Sid":"ListAllBucket",
-              "Effect": "Allow",
-              "Action": ["s3:PutObject"],
-              "Principal":"*",
-              "Resource": "arn:aws:s3:::state-terraform-s3/*"
-            }
-          ]
-        }
-
-        \"\"\")
-        developer_iam_group_policy_attachment = minio.IamGroupPolicyAttachment("developerIamGroupPolicyAttachment",
+        user_one = minio.IamUser("userOne")
+        developer_iam_group_user_attachment = minio.IamGroupUserAttachment("developerIamGroupUserAttachment",
             group_name=minio_iam_group["group"]["name"],
-            policy_name=minio_iam_policy["test_policy"]["id"])
-        pulumi.export("minioName", developer_iam_group_policy_attachment.id)
-        pulumi.export("minioUsers", developer_iam_group_policy_attachment.group_name)
-        pulumi.export("minioGroup", developer_iam_group_policy_attachment.policy_name)
+            user_name=user_one.name)
+        pulumi.export("minioName", developer_iam_group_user_attachment.id)
+        pulumi.export("minioUsers", developer_iam_group_user_attachment.group_name)
+        pulumi.export("minioGroup", developer_iam_group_user_attachment.user_name)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: IamGroupPolicyAttachmentArgs,
+                 args: IamGroupUserAttachmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_minio as minio
 
         developer_iam_group = minio.IamGroup("developerIamGroup")
-        test_policy = minio.IamGroupPolicy("testPolicy", policy=\"\"\"{
-          "Version":"2012-10-17",
-          "Statement": [
-            {
-              "Sid":"ListAllBucket",
-              "Effect": "Allow",
-              "Action": ["s3:PutObject"],
-              "Principal":"*",
-              "Resource": "arn:aws:s3:::state-terraform-s3/*"
-            }
-          ]
-        }
-
-        \"\"\")
-        developer_iam_group_policy_attachment = minio.IamGroupPolicyAttachment("developerIamGroupPolicyAttachment",
+        user_one = minio.IamUser("userOne")
+        developer_iam_group_user_attachment = minio.IamGroupUserAttachment("developerIamGroupUserAttachment",
             group_name=minio_iam_group["group"]["name"],
-            policy_name=minio_iam_policy["test_policy"]["id"])
-        pulumi.export("minioName", developer_iam_group_policy_attachment.id)
-        pulumi.export("minioUsers", developer_iam_group_policy_attachment.group_name)
-        pulumi.export("minioGroup", developer_iam_group_policy_attachment.policy_name)
+            user_name=user_one.name)
+        pulumi.export("minioName", developer_iam_group_user_attachment.id)
+        pulumi.export("minioUsers", developer_iam_group_user_attachment.group_name)
+        pulumi.export("minioGroup", developer_iam_group_user_attachment.user_name)
         ```
 
         :param str resource_name: The name of the resource.
-        :param IamGroupPolicyAttachmentArgs args: The arguments to use to populate this resource's properties.
+        :param IamGroupUserAttachmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(IamGroupPolicyAttachmentArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(IamGroupUserAttachmentArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  group_name: Optional[pulumi.Input[str]] = None,
-                 policy_name: Optional[pulumi.Input[str]] = None,
+                 user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = IamGroupPolicyAttachmentArgs.__new__(IamGroupPolicyAttachmentArgs)
+            __props__ = IamGroupUserAttachmentArgs.__new__(IamGroupUserAttachmentArgs)
 
             if group_name is None and not opts.urn:
                 raise TypeError("Missing required property 'group_name'")
             __props__.__dict__["group_name"] = group_name
-            if policy_name is None and not opts.urn:
-                raise TypeError("Missing required property 'policy_name'")
-            __props__.__dict__["policy_name"] = policy_name
-        super(IamGroupPolicyAttachment, __self__).__init__(
-            'minio:index/iamGroupPolicyAttachment:IamGroupPolicyAttachment',
+            if user_name is None and not opts.urn:
+                raise TypeError("Missing required property 'user_name'")
+            __props__.__dict__["user_name"] = user_name
+        super(IamGroupUserAttachment, __self__).__init__(
+            'minio:index/iamGroupUserAttachment:IamGroupUserAttachment',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             group_name: Optional[pulumi.Input[str]] = None,
-            policy_name: Optional[pulumi.Input[str]] = None) -> 'IamGroupPolicyAttachment':
+            user_name: Optional[pulumi.Input[str]] = None) -> 'IamGroupUserAttachment':
         """
-        Get an existing IamGroupPolicyAttachment resource's state with the given name, id, and optional extra
+        Get an existing IamGroupUserAttachment resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _IamGroupPolicyAttachmentState.__new__(_IamGroupPolicyAttachmentState)
+        __props__ = _IamGroupUserAttachmentState.__new__(_IamGroupUserAttachmentState)
 
         __props__.__dict__["group_name"] = group_name
-        __props__.__dict__["policy_name"] = policy_name
-        return IamGroupPolicyAttachment(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["user_name"] = user_name
+        return IamGroupUserAttachment(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="groupName")
     def group_name(self) -> pulumi.Output[str]:
         return pulumi.get(self, "group_name")
 
     @property
-    @pulumi.getter(name="policyName")
-    def policy_name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "policy_name")
+    @pulumi.getter(name="userName")
+    def user_name(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "user_name")
```

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_group_user_attachment.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_user_policy_attachment.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,192 +5,222 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['IamGroupUserAttachmentArgs', 'IamGroupUserAttachment']
+__all__ = ['IamUserPolicyAttachmentArgs', 'IamUserPolicyAttachment']
 
 @pulumi.input_type
-class IamGroupUserAttachmentArgs:
+class IamUserPolicyAttachmentArgs:
     def __init__(__self__, *,
-                 group_name: pulumi.Input[str],
+                 policy_name: pulumi.Input[str],
                  user_name: pulumi.Input[str]):
         """
-        The set of arguments for constructing a IamGroupUserAttachment resource.
+        The set of arguments for constructing a IamUserPolicyAttachment resource.
         """
-        pulumi.set(__self__, "group_name", group_name)
+        pulumi.set(__self__, "policy_name", policy_name)
         pulumi.set(__self__, "user_name", user_name)
 
     @property
-    @pulumi.getter(name="groupName")
-    def group_name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "group_name")
-
-    @group_name.setter
-    def group_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "group_name", value)
+    @pulumi.getter(name="policyName")
+    def policy_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "policy_name")
+
+    @policy_name.setter
+    def policy_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "policy_name", value)
 
     @property
     @pulumi.getter(name="userName")
     def user_name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "user_name")
 
     @user_name.setter
     def user_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "user_name", value)
 
 
 @pulumi.input_type
-class _IamGroupUserAttachmentState:
+class _IamUserPolicyAttachmentState:
     def __init__(__self__, *,
-                 group_name: Optional[pulumi.Input[str]] = None,
+                 policy_name: Optional[pulumi.Input[str]] = None,
                  user_name: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering IamGroupUserAttachment resources.
+        Input properties used for looking up and filtering IamUserPolicyAttachment resources.
         """
-        if group_name is not None:
-            pulumi.set(__self__, "group_name", group_name)
+        if policy_name is not None:
+            pulumi.set(__self__, "policy_name", policy_name)
         if user_name is not None:
             pulumi.set(__self__, "user_name", user_name)
 
     @property
-    @pulumi.getter(name="groupName")
-    def group_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "group_name")
-
-    @group_name.setter
-    def group_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group_name", value)
+    @pulumi.getter(name="policyName")
+    def policy_name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "policy_name")
+
+    @policy_name.setter
+    def policy_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "policy_name", value)
 
     @property
     @pulumi.getter(name="userName")
     def user_name(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "user_name")
 
     @user_name.setter
     def user_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_name", value)
 
 
-class IamGroupUserAttachment(pulumi.CustomResource):
+class IamUserPolicyAttachment(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 group_name: Optional[pulumi.Input[str]] = None,
+                 policy_name: Optional[pulumi.Input[str]] = None,
                  user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_minio as minio
 
-        developer_iam_group = minio.IamGroup("developerIamGroup")
-        user_one = minio.IamUser("userOne")
-        developer_iam_group_user_attachment = minio.IamGroupUserAttachment("developerIamGroupUserAttachment",
-            group_name=minio_iam_group["group"]["name"],
-            user_name=user_one.name)
-        pulumi.export("minioName", developer_iam_group_user_attachment.id)
-        pulumi.export("minioUsers", developer_iam_group_user_attachment.group_name)
-        pulumi.export("minioGroup", developer_iam_group_user_attachment.user_name)
+        test_user = minio.IamUser("testUser")
+        test_policy = minio.IamPolicy("testPolicy", policy=\"\"\"{
+          "Version":"2012-10-17",
+          "Statement": [
+            {
+              "Sid":"ListAllBucket",
+              "Effect": "Allow",
+              "Action": ["s3:PutObject"],
+              "Principal":"*",
+              "Resource": "arn:aws:s3:::state-terraform-s3/*"
+            }
+          ]
+        }
+        \"\"\")
+        developer_iam_user_policy_attachment = minio.IamUserPolicyAttachment("developerIamUserPolicyAttachment",
+            user_name=test_user.id,
+            policy_name=test_policy.id)
+        pulumi.export("minioName", developer_iam_user_policy_attachment.id)
+        pulumi.export("minioUsers", developer_iam_user_policy_attachment.user_name)
+        pulumi.export("minioGroup", developer_iam_user_policy_attachment.policy_name)
+        developer_index_iam_user_policy_attachment_iam_user_policy_attachment = minio.IamUserPolicyAttachment("developerIndex/iamUserPolicyAttachmentIamUserPolicyAttachment",
+            user_name="CN=My User,OU=Unit,DC=example,DC=com",
+            policy_name=test_policy.id)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: IamGroupUserAttachmentArgs,
+                 args: IamUserPolicyAttachmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_minio as minio
 
-        developer_iam_group = minio.IamGroup("developerIamGroup")
-        user_one = minio.IamUser("userOne")
-        developer_iam_group_user_attachment = minio.IamGroupUserAttachment("developerIamGroupUserAttachment",
-            group_name=minio_iam_group["group"]["name"],
-            user_name=user_one.name)
-        pulumi.export("minioName", developer_iam_group_user_attachment.id)
-        pulumi.export("minioUsers", developer_iam_group_user_attachment.group_name)
-        pulumi.export("minioGroup", developer_iam_group_user_attachment.user_name)
+        test_user = minio.IamUser("testUser")
+        test_policy = minio.IamPolicy("testPolicy", policy=\"\"\"{
+          "Version":"2012-10-17",
+          "Statement": [
+            {
+              "Sid":"ListAllBucket",
+              "Effect": "Allow",
+              "Action": ["s3:PutObject"],
+              "Principal":"*",
+              "Resource": "arn:aws:s3:::state-terraform-s3/*"
+            }
+          ]
+        }
+        \"\"\")
+        developer_iam_user_policy_attachment = minio.IamUserPolicyAttachment("developerIamUserPolicyAttachment",
+            user_name=test_user.id,
+            policy_name=test_policy.id)
+        pulumi.export("minioName", developer_iam_user_policy_attachment.id)
+        pulumi.export("minioUsers", developer_iam_user_policy_attachment.user_name)
+        pulumi.export("minioGroup", developer_iam_user_policy_attachment.policy_name)
+        developer_index_iam_user_policy_attachment_iam_user_policy_attachment = minio.IamUserPolicyAttachment("developerIndex/iamUserPolicyAttachmentIamUserPolicyAttachment",
+            user_name="CN=My User,OU=Unit,DC=example,DC=com",
+            policy_name=test_policy.id)
         ```
 
         :param str resource_name: The name of the resource.
-        :param IamGroupUserAttachmentArgs args: The arguments to use to populate this resource's properties.
+        :param IamUserPolicyAttachmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(IamGroupUserAttachmentArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(IamUserPolicyAttachmentArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 group_name: Optional[pulumi.Input[str]] = None,
+                 policy_name: Optional[pulumi.Input[str]] = None,
                  user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = IamGroupUserAttachmentArgs.__new__(IamGroupUserAttachmentArgs)
+            __props__ = IamUserPolicyAttachmentArgs.__new__(IamUserPolicyAttachmentArgs)
 
-            if group_name is None and not opts.urn:
-                raise TypeError("Missing required property 'group_name'")
-            __props__.__dict__["group_name"] = group_name
+            if policy_name is None and not opts.urn:
+                raise TypeError("Missing required property 'policy_name'")
+            __props__.__dict__["policy_name"] = policy_name
             if user_name is None and not opts.urn:
                 raise TypeError("Missing required property 'user_name'")
             __props__.__dict__["user_name"] = user_name
-        super(IamGroupUserAttachment, __self__).__init__(
-            'minio:index/iamGroupUserAttachment:IamGroupUserAttachment',
+        super(IamUserPolicyAttachment, __self__).__init__(
+            'minio:index/iamUserPolicyAttachment:IamUserPolicyAttachment',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            group_name: Optional[pulumi.Input[str]] = None,
-            user_name: Optional[pulumi.Input[str]] = None) -> 'IamGroupUserAttachment':
+            policy_name: Optional[pulumi.Input[str]] = None,
+            user_name: Optional[pulumi.Input[str]] = None) -> 'IamUserPolicyAttachment':
         """
-        Get an existing IamGroupUserAttachment resource's state with the given name, id, and optional extra
+        Get an existing IamUserPolicyAttachment resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _IamGroupUserAttachmentState.__new__(_IamGroupUserAttachmentState)
+        __props__ = _IamUserPolicyAttachmentState.__new__(_IamUserPolicyAttachmentState)
 
-        __props__.__dict__["group_name"] = group_name
+        __props__.__dict__["policy_name"] = policy_name
         __props__.__dict__["user_name"] = user_name
-        return IamGroupUserAttachment(resource_name, opts=opts, __props__=__props__)
+        return IamUserPolicyAttachment(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="groupName")
-    def group_name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "group_name")
+    @pulumi.getter(name="policyName")
+    def policy_name(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "policy_name")
 
     @property
     @pulumi.getter(name="userName")
     def user_name(self) -> pulumi.Output[str]:
         return pulumi.get(self, "user_name")
```

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_policy.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_service_account.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_user.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/iam_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/iam_user_policy_attachment.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_bucket_policy.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,218 +5,206 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['IamUserPolicyAttachmentArgs', 'IamUserPolicyAttachment']
+__all__ = ['S3BucketPolicyArgs', 'S3BucketPolicy']
 
 @pulumi.input_type
-class IamUserPolicyAttachmentArgs:
+class S3BucketPolicyArgs:
     def __init__(__self__, *,
-                 policy_name: pulumi.Input[str],
-                 user_name: pulumi.Input[str]):
+                 bucket: pulumi.Input[str],
+                 policy: pulumi.Input[str]):
         """
-        The set of arguments for constructing a IamUserPolicyAttachment resource.
+        The set of arguments for constructing a S3BucketPolicy resource.
         """
-        pulumi.set(__self__, "policy_name", policy_name)
-        pulumi.set(__self__, "user_name", user_name)
+        pulumi.set(__self__, "bucket", bucket)
+        pulumi.set(__self__, "policy", policy)
 
     @property
-    @pulumi.getter(name="policyName")
-    def policy_name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "policy_name")
+    @pulumi.getter
+    def bucket(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "bucket")
 
-    @policy_name.setter
-    def policy_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "policy_name", value)
+    @bucket.setter
+    def bucket(self, value: pulumi.Input[str]):
+        pulumi.set(self, "bucket", value)
 
     @property
-    @pulumi.getter(name="userName")
-    def user_name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "user_name")
+    @pulumi.getter
+    def policy(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "policy")
 
-    @user_name.setter
-    def user_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "user_name", value)
+    @policy.setter
+    def policy(self, value: pulumi.Input[str]):
+        pulumi.set(self, "policy", value)
 
 
 @pulumi.input_type
-class _IamUserPolicyAttachmentState:
+class _S3BucketPolicyState:
     def __init__(__self__, *,
-                 policy_name: Optional[pulumi.Input[str]] = None,
-                 user_name: Optional[pulumi.Input[str]] = None):
+                 bucket: Optional[pulumi.Input[str]] = None,
+                 policy: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering IamUserPolicyAttachment resources.
+        Input properties used for looking up and filtering S3BucketPolicy resources.
         """
-        if policy_name is not None:
-            pulumi.set(__self__, "policy_name", policy_name)
-        if user_name is not None:
-            pulumi.set(__self__, "user_name", user_name)
+        if bucket is not None:
+            pulumi.set(__self__, "bucket", bucket)
+        if policy is not None:
+            pulumi.set(__self__, "policy", policy)
 
     @property
-    @pulumi.getter(name="policyName")
-    def policy_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "policy_name")
+    @pulumi.getter
+    def bucket(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "bucket")
 
-    @policy_name.setter
-    def policy_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "policy_name", value)
+    @bucket.setter
+    def bucket(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "bucket", value)
 
     @property
-    @pulumi.getter(name="userName")
-    def user_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "user_name")
+    @pulumi.getter
+    def policy(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "policy")
 
-    @user_name.setter
-    def user_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "user_name", value)
+    @policy.setter
+    def policy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "policy", value)
 
 
-class IamUserPolicyAttachment(pulumi.CustomResource):
+class S3BucketPolicy(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 policy_name: Optional[pulumi.Input[str]] = None,
-                 user_name: Optional[pulumi.Input[str]] = None,
+                 bucket: Optional[pulumi.Input[str]] = None,
+                 policy: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_minio as minio
 
-        test_user = minio.IamUser("testUser")
-        test_policy = minio.IamPolicy("testPolicy", policy=\"\"\"{
-          "Version":"2012-10-17",
+        bucket_s3_bucket = minio.S3Bucket("bucketS3Bucket", bucket="example-bucket")
+        bucket_s3_bucket_policy = minio.S3BucketPolicy("bucketS3BucketPolicy",
+            bucket=bucket_s3_bucket.bucket,
+            policy=bucket_s3_bucket.bucket.apply(lambda bucket: f\"\"\"{{
+          "Version": "2012-10-17",
           "Statement": [
-            {
-              "Sid":"ListAllBucket",
+            {{
               "Effect": "Allow",
-              "Action": ["s3:PutObject"],
-              "Principal":"*",
-              "Resource": "arn:aws:s3:::state-terraform-s3/*"
-            }
+             "Principal": {{"AWS": ["*"]}},
+              "Resource": ["arn:aws:s3:::{bucket}"],
+             "Action": ["s3:ListBucket"]
+            }}
           ]
-        }
-
-        \"\"\")
-        developer = minio.IamUserPolicyAttachment("developer",
-            policy_name=test_policy.id,
-            user_name=test_user.id)
-        pulumi.export("minioName", developer.id)
-        pulumi.export("minioUsers", developer.user_name)
-        pulumi.export("minioGroup", developer.policy_name)
+        }}
+        \"\"\"))
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: IamUserPolicyAttachmentArgs,
+                 args: S3BucketPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_minio as minio
 
-        test_user = minio.IamUser("testUser")
-        test_policy = minio.IamPolicy("testPolicy", policy=\"\"\"{
-          "Version":"2012-10-17",
+        bucket_s3_bucket = minio.S3Bucket("bucketS3Bucket", bucket="example-bucket")
+        bucket_s3_bucket_policy = minio.S3BucketPolicy("bucketS3BucketPolicy",
+            bucket=bucket_s3_bucket.bucket,
+            policy=bucket_s3_bucket.bucket.apply(lambda bucket: f\"\"\"{{
+          "Version": "2012-10-17",
           "Statement": [
-            {
-              "Sid":"ListAllBucket",
+            {{
               "Effect": "Allow",
-              "Action": ["s3:PutObject"],
-              "Principal":"*",
-              "Resource": "arn:aws:s3:::state-terraform-s3/*"
-            }
+             "Principal": {{"AWS": ["*"]}},
+              "Resource": ["arn:aws:s3:::{bucket}"],
+             "Action": ["s3:ListBucket"]
+            }}
           ]
-        }
-
-        \"\"\")
-        developer = minio.IamUserPolicyAttachment("developer",
-            policy_name=test_policy.id,
-            user_name=test_user.id)
-        pulumi.export("minioName", developer.id)
-        pulumi.export("minioUsers", developer.user_name)
-        pulumi.export("minioGroup", developer.policy_name)
+        }}
+        \"\"\"))
         ```
 
         :param str resource_name: The name of the resource.
-        :param IamUserPolicyAttachmentArgs args: The arguments to use to populate this resource's properties.
+        :param S3BucketPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(IamUserPolicyAttachmentArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(S3BucketPolicyArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 policy_name: Optional[pulumi.Input[str]] = None,
-                 user_name: Optional[pulumi.Input[str]] = None,
+                 bucket: Optional[pulumi.Input[str]] = None,
+                 policy: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = IamUserPolicyAttachmentArgs.__new__(IamUserPolicyAttachmentArgs)
+            __props__ = S3BucketPolicyArgs.__new__(S3BucketPolicyArgs)
 
-            if policy_name is None and not opts.urn:
-                raise TypeError("Missing required property 'policy_name'")
-            __props__.__dict__["policy_name"] = policy_name
-            if user_name is None and not opts.urn:
-                raise TypeError("Missing required property 'user_name'")
-            __props__.__dict__["user_name"] = user_name
-        super(IamUserPolicyAttachment, __self__).__init__(
-            'minio:index/iamUserPolicyAttachment:IamUserPolicyAttachment',
+            if bucket is None and not opts.urn:
+                raise TypeError("Missing required property 'bucket'")
+            __props__.__dict__["bucket"] = bucket
+            if policy is None and not opts.urn:
+                raise TypeError("Missing required property 'policy'")
+            __props__.__dict__["policy"] = policy
+        super(S3BucketPolicy, __self__).__init__(
+            'minio:index/s3BucketPolicy:S3BucketPolicy',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            policy_name: Optional[pulumi.Input[str]] = None,
-            user_name: Optional[pulumi.Input[str]] = None) -> 'IamUserPolicyAttachment':
+            bucket: Optional[pulumi.Input[str]] = None,
+            policy: Optional[pulumi.Input[str]] = None) -> 'S3BucketPolicy':
         """
-        Get an existing IamUserPolicyAttachment resource's state with the given name, id, and optional extra
+        Get an existing S3BucketPolicy resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _IamUserPolicyAttachmentState.__new__(_IamUserPolicyAttachmentState)
+        __props__ = _S3BucketPolicyState.__new__(_S3BucketPolicyState)
 
-        __props__.__dict__["policy_name"] = policy_name
-        __props__.__dict__["user_name"] = user_name
-        return IamUserPolicyAttachment(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["bucket"] = bucket
+        __props__.__dict__["policy"] = policy
+        return S3BucketPolicy(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="policyName")
-    def policy_name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "policy_name")
+    @pulumi.getter
+    def bucket(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "bucket")
 
     @property
-    @pulumi.getter(name="userName")
-    def user_name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "user_name")
+    @pulumi.getter
+    def policy(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "policy")
```

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/ilm_policy.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/ilm_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/outputs.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/provider.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/s3_bucket.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/s3_bucket_notification.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/s3_bucket_versioning.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio/s3_object.py` & `pulumi_minio-0.9.1a1682440158/pulumi_minio/s3_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio.egg-info/PKG-INFO` & `pulumi_minio-0.9.1a1682440158/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi-minio
-Version: 0.9.1a1681933919
+Name: pulumi_minio
+Version: 0.9.1a1682440158
 Summary: A Pulumi package for creating and managing minio cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-minio
 Keywords: pulumi minio
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-minio/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-minio/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fminio.svg)](https://www.npmjs.com/package/@pulumi/minio)
 [![Python version](https://badge.fury.io/py/pulumi-minio.svg)](https://pypi.org/project/pulumi-minio)
 [![NuGet version](https://badge.fury.io/nu/pulumi.minio.svg)](https://badge.fury.io/nu/pulumi.minio)
```

### Comparing `pulumi_minio-0.9.1a1681933919/pulumi_minio.egg-info/SOURCES.txt` & `pulumi_minio-0.9.1a1682440158/pulumi_minio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1681933919/setup.py` & `pulumi_minio-0.9.1a1682440158/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.1a1681933919"
-PLUGIN_VERSION = "0.9.1-alpha.1681933919+5b28112c"
+VERSION = "0.9.1a1682440158"
+PLUGIN_VERSION = "0.9.1-alpha.1682440158+b5bae86b"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'minio', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "minio Pulumi Package - Development Version"
 
 
 setup(name='pulumi_minio',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing minio cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

