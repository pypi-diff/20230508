# Comparing `tmp/terraform-backend-s3-bucket-0.0.8.tar.gz` & `tmp/terraform-backend-s3-bucket-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terraform-backend-s3-bucket-0.0.8.tar", last modified: Sat Apr 15 12:03:26 2023, max compression
+gzip compressed data, was "terraform-backend-s3-bucket-0.0.9.tar", last modified: Mon Apr 17 16:37:41 2023, max compression
```

## Comparing `terraform-backend-s3-bucket-0.0.8.tar` & `terraform-backend-s3-bucket-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:03:26.739992 terraform-backend-s3-bucket-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-15 12:03:13.000000 terraform-backend-s3-bucket-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-15 12:03:13.000000 terraform-backend-s3-bucket-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-15 12:03:26.739992 terraform-backend-s3-bucket-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-15 12:03:13.000000 terraform-backend-s3-bucket-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 12:03:13.000000 terraform-backend-s3-bucket-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:03:26.739992 terraform-backend-s3-bucket-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-15 12:03:13.000000 terraform-backend-s3-bucket-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:03:26.735992 terraform-backend-s3-bucket-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:03:26.739992 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-15 12:03:13.000000 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:03:26.739992 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 12:03:13.000000 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 12:03:13.000000 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 12:03:13.000000 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:03:26.739992 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-15 12:03:26.000000 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-15 12:03:26.000000 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 12:03:26.000000 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 12:03:26.000000 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-15 12:03:26.000000 terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:37:41.673604 terraform-backend-s3-bucket-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 16:37:29.000000 terraform-backend-s3-bucket-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 16:37:29.000000 terraform-backend-s3-bucket-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-17 16:37:41.673604 terraform-backend-s3-bucket-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-17 16:37:29.000000 terraform-backend-s3-bucket-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 16:37:29.000000 terraform-backend-s3-bucket-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:37:41.673604 terraform-backend-s3-bucket-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-17 16:37:29.000000 terraform-backend-s3-bucket-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:37:41.673604 terraform-backend-s3-bucket-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:37:41.673604 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-17 16:37:29.000000 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:37:41.673604 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-17 16:37:29.000000 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-04-17 16:37:29.000000 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:37:29.000000 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:37:41.673604 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-17 16:37:41.000000 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-17 16:37:41.000000 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:37:41.000000 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 16:37:41.000000 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 16:37:41.000000 terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket.egg-info/top_level.txt
```

### Comparing `terraform-backend-s3-bucket-0.0.8/LICENSE` & `terraform-backend-s3-bucket-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-0.0.8/PKG-INFO` & `terraform-backend-s3-bucket-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-backend-s3-bucket
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.
 Home-page: https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `terraform-backend-s3-bucket-0.0.8/README.md` & `terraform-backend-s3-bucket-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-0.0.8/setup.py` & `terraform-backend-s3-bucket-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "terraform-backend-s3-bucket",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.",
     "license": "Apache-2.0",
     "url": "https://github.com/stefanfreitag/terraform-backend-s3-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "terraform_backend_s3_bucket",
         "terraform_backend_s3_bucket._jsii"
     ],
     "package_data": {
         "terraform_backend_s3_bucket._jsii": [
-            "terraform-backend-s3-bucket@0.0.8.jsii.tgz"
+            "terraform-backend-s3-bucket@0.0.9.jsii.tgz"
         ],
         "terraform_backend_s3_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket/__init__.py` & `terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket.egg-info/PKG-INFO` & `terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-backend-s3-bucket
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.
 Home-page: https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `terraform-backend-s3-bucket-0.0.8/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt` & `terraform-backend-s3-bucket-0.0.9/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/terraform_backend_s3_bucket/py.typed
 src/terraform_backend_s3_bucket.egg-info/PKG-INFO
 src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
 src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
 src/terraform_backend_s3_bucket.egg-info/requires.txt
 src/terraform_backend_s3_bucket.egg-info/top_level.txt
 src/terraform_backend_s3_bucket/_jsii/__init__.py
-src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@0.0.8.jsii.tgz
+src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@0.0.9.jsii.tgz
```

