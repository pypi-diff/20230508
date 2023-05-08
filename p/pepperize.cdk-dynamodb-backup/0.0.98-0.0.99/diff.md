# Comparing `tmp/pepperize.cdk-dynamodb-backup-0.0.98.tar.gz` & `tmp/pepperize.cdk-dynamodb-backup-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperize.cdk-dynamodb-backup-0.0.98.tar", last modified: Tue Sep  6 14:01:32 2022, max compression
+gzip compressed data, was "pepperize.cdk-dynamodb-backup-0.0.99.tar", last modified: Tue Sep  6 14:07:57 2022, max compression
```

## Comparing `pepperize.cdk-dynamodb-backup-0.0.98.tar` & `pepperize.cdk-dynamodb-backup-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:01:32.516621 pepperize.cdk-dynamodb-backup-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-06 14:01:15.000000 pepperize.cdk-dynamodb-backup-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-06 14:01:15.000000 pepperize.cdk-dynamodb-backup-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-09-06 14:01:32.516621 pepperize.cdk-dynamodb-backup-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-09-06 14:01:15.000000 pepperize.cdk-dynamodb-backup-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-06 14:01:15.000000 pepperize.cdk-dynamodb-backup-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 14:01:32.516621 pepperize.cdk-dynamodb-backup-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-09-06 14:01:15.000000 pepperize.cdk-dynamodb-backup-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:01:32.516621 pepperize.cdk-dynamodb-backup-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:01:32.516621 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize.cdk_dynamodb_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-09-06 14:01:31.000000 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize.cdk_dynamodb_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-09-06 14:01:32.000000 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize.cdk_dynamodb_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 14:01:31.000000 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize.cdk_dynamodb_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-06 14:01:32.000000 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize.cdk_dynamodb_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-06 14:01:32.000000 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize.cdk_dynamodb_backup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:01:32.516621 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize_cdk_dynamodb_backup/
--rw-r--r--   0 runner    (1001) docker     (121)    23186 2022-09-06 14:01:15.000000 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize_cdk_dynamodb_backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:01:32.516621 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize_cdk_dynamodb_backup/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-06 14:01:15.000000 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize_cdk_dynamodb_backup/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29973 2022-09-06 14:01:15.000000 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize_cdk_dynamodb_backup/_jsii/cdk-dynamodb-backup@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 14:01:15.000000 pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize_cdk_dynamodb_backup/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:07:57.128368 pepperize.cdk-dynamodb-backup-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-06 14:07:41.000000 pepperize.cdk-dynamodb-backup-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-06 14:07:41.000000 pepperize.cdk-dynamodb-backup-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-09-06 14:07:57.128368 pepperize.cdk-dynamodb-backup-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-09-06 14:07:41.000000 pepperize.cdk-dynamodb-backup-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-06 14:07:41.000000 pepperize.cdk-dynamodb-backup-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 14:07:57.128368 pepperize.cdk-dynamodb-backup-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-09-06 14:07:41.000000 pepperize.cdk-dynamodb-backup-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:07:57.124368 pepperize.cdk-dynamodb-backup-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:07:57.128368 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize.cdk_dynamodb_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-09-06 14:07:56.000000 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize.cdk_dynamodb_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-09-06 14:07:57.000000 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize.cdk_dynamodb_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 14:07:56.000000 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize.cdk_dynamodb_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-06 14:07:56.000000 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize.cdk_dynamodb_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-06 14:07:56.000000 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize.cdk_dynamodb_backup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:07:57.128368 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize_cdk_dynamodb_backup/
+-rw-r--r--   0 runner    (1001) docker     (121)    23186 2022-09-06 14:07:41.000000 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize_cdk_dynamodb_backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 14:07:57.128368 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize_cdk_dynamodb_backup/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-06 14:07:41.000000 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize_cdk_dynamodb_backup/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29973 2022-09-06 14:07:41.000000 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize_cdk_dynamodb_backup/_jsii/cdk-dynamodb-backup@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 14:07:41.000000 pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize_cdk_dynamodb_backup/py.typed
```

### Comparing `pepperize.cdk-dynamodb-backup-0.0.98/LICENSE` & `pepperize.cdk-dynamodb-backup-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-dynamodb-backup-0.0.98/PKG-INFO` & `pepperize.cdk-dynamodb-backup-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-dynamodb-backup
-Version: 0.0.98
+Version: 0.0.99
 Summary: Backup and restore AWS DynamoDB Table to AWS S3 Bucket with AWS Data Pipeline.
 Home-page: https://github.com/patrick.florek/cdk-dynamodb-backup.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/patrick.florek/cdk-dynamodb-backup.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pepperize.cdk-dynamodb-backup-0.0.98/README.md` & `pepperize.cdk-dynamodb-backup-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-dynamodb-backup-0.0.98/setup.py` & `pepperize.cdk-dynamodb-backup-0.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pepperize.cdk-dynamodb-backup",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "Backup and restore AWS DynamoDB Table to AWS S3 Bucket with AWS Data Pipeline.",
     "license": "MIT",
     "url": "https://github.com/patrick.florek/cdk-dynamodb-backup.git",
     "long_description_content_type": "text/markdown",
     "author": "Patrick Florek<patrick.florek@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pepperize_cdk_dynamodb_backup",
         "pepperize_cdk_dynamodb_backup._jsii"
     ],
     "package_data": {
         "pepperize_cdk_dynamodb_backup._jsii": [
-            "cdk-dynamodb-backup@0.0.98.jsii.tgz"
+            "cdk-dynamodb-backup@0.0.99.jsii.tgz"
         ],
         "pepperize_cdk_dynamodb_backup": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize.cdk_dynamodb_backup.egg-info/PKG-INFO` & `pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize.cdk_dynamodb_backup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-dynamodb-backup
-Version: 0.0.98
+Version: 0.0.99
 Summary: Backup and restore AWS DynamoDB Table to AWS S3 Bucket with AWS Data Pipeline.
 Home-page: https://github.com/patrick.florek/cdk-dynamodb-backup.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/patrick.florek/cdk-dynamodb-backup.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize.cdk_dynamodb_backup.egg-info/SOURCES.txt` & `pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize.cdk_dynamodb_backup.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/pepperize.cdk_dynamodb_backup.egg-info/SOURCES.txt
 src/pepperize.cdk_dynamodb_backup.egg-info/dependency_links.txt
 src/pepperize.cdk_dynamodb_backup.egg-info/requires.txt
 src/pepperize.cdk_dynamodb_backup.egg-info/top_level.txt
 src/pepperize_cdk_dynamodb_backup/__init__.py
 src/pepperize_cdk_dynamodb_backup/py.typed
 src/pepperize_cdk_dynamodb_backup/_jsii/__init__.py
-src/pepperize_cdk_dynamodb_backup/_jsii/cdk-dynamodb-backup@0.0.98.jsii.tgz
+src/pepperize_cdk_dynamodb_backup/_jsii/cdk-dynamodb-backup@0.0.99.jsii.tgz
```

### Comparing `pepperize.cdk-dynamodb-backup-0.0.98/src/pepperize_cdk_dynamodb_backup/__init__.py` & `pepperize.cdk-dynamodb-backup-0.0.99/src/pepperize_cdk_dynamodb_backup/__init__.py`

 * *Files identical despite different names*

