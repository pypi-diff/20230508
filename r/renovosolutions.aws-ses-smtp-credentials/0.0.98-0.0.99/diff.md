# Comparing `tmp/renovosolutions.aws-ses-smtp-credentials-0.0.98.tar.gz` & `tmp/renovosolutions.aws-ses-smtp-credentials-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-ses-smtp-credentials-0.0.98.tar", last modified: Mon Jan 30 13:40:24 2023, max compression
+gzip compressed data, was "renovosolutions.aws-ses-smtp-credentials-0.0.99.tar", last modified: Wed Feb  8 20:09:22 2023, max compression
```

## Comparing `renovosolutions.aws-ses-smtp-credentials-0.0.98.tar` & `renovosolutions.aws-ses-smtp-credentials-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:40:24.874233 renovosolutions.aws-ses-smtp-credentials-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-30 13:40:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-30 13:40:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-01-30 13:40:24.874233 renovosolutions.aws-ses-smtp-credentials-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-30 13:40:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-30 13:40:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 13:40:24.874233 renovosolutions.aws-ses-smtp-credentials-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-01-30 13:40:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:40:24.870233 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:40:24.874233 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/renovosolutions.aws_ses_smtp_credentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-01-30 13:40:24.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/renovosolutions.aws_ses_smtp_credentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-01-30 13:40:24.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/renovosolutions.aws_ses_smtp_credentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 13:40:24.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/renovosolutions.aws_ses_smtp_credentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-30 13:40:24.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/renovosolutions.aws_ses_smtp_credentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-30 13:40:24.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/renovosolutions.aws_ses_smtp_credentials.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:40:24.874233 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/ses-smtp-credentials/
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-01-30 13:40:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/ses-smtp-credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:40:24.874233 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/ses-smtp-credentials/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-01-30 13:40:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/ses-smtp-credentials/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-01-30 13:40:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/ses-smtp-credentials/_jsii/cdk-library-aws-ses-smtp-credentials@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 13:40:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.98/src/ses-smtp-credentials/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:09:22.817911 renovosolutions.aws-ses-smtp-credentials-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-08 20:09:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-08 20:09:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-08 20:09:22.817911 renovosolutions.aws-ses-smtp-credentials-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-08 20:09:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-08 20:09:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 20:09:22.817911 renovosolutions.aws-ses-smtp-credentials-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-02-08 20:09:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:09:22.817911 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:09:22.817911 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/renovosolutions.aws_ses_smtp_credentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-08 20:09:22.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/renovosolutions.aws_ses_smtp_credentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-08 20:09:22.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/renovosolutions.aws_ses_smtp_credentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:09:22.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/renovosolutions.aws_ses_smtp_credentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-08 20:09:22.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/renovosolutions.aws_ses_smtp_credentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-08 20:09:22.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/renovosolutions.aws_ses_smtp_credentials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:09:22.817911 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/ses-smtp-credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-02-08 20:09:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/ses-smtp-credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:09:22.817911 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/ses-smtp-credentials/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-08 20:09:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/ses-smtp-credentials/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26148 2023-02-08 20:09:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/ses-smtp-credentials/_jsii/cdk-library-aws-ses-smtp-credentials@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:09:09.000000 renovosolutions.aws-ses-smtp-credentials-0.0.99/src/ses-smtp-credentials/py.typed
```

### Comparing `renovosolutions.aws-ses-smtp-credentials-0.0.98/LICENSE` & `renovosolutions.aws-ses-smtp-credentials-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-ses-smtp-credentials-0.0.98/PKG-INFO` & `renovosolutions.aws-ses-smtp-credentials-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-ses-smtp-credentials
-Version: 0.0.98
+Version: 0.0.99
 Summary: AWS CDK Construct Library for generating SMTP credentials for SES and storing them in Secrets Manager
 Home-page: https://github.com/brandon/cdk-library-aws-ses-smtp-credentials.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/brandon/cdk-library-aws-ses-smtp-credentials.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-ses-smtp-credentials-0.0.98/README.md` & `renovosolutions.aws-ses-smtp-credentials-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-ses-smtp-credentials-0.0.98/setup.py` & `renovosolutions.aws-ses-smtp-credentials-0.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-ses-smtp-credentials",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "AWS CDK Construct Library for generating SMTP credentials for SES and storing them in Secrets Manager",
     "license": "Apache-2.0",
     "url": "https://github.com/brandon/cdk-library-aws-ses-smtp-credentials.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "ses-smtp-credentials",
         "ses-smtp-credentials._jsii"
     ],
     "package_data": {
         "ses-smtp-credentials._jsii": [
-            "cdk-library-aws-ses-smtp-credentials@0.0.98.jsii.tgz"
+            "cdk-library-aws-ses-smtp-credentials@0.0.99.jsii.tgz"
         ],
         "ses-smtp-credentials": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `renovosolutions.aws-ses-smtp-credentials-0.0.98/src/renovosolutions.aws_ses_smtp_credentials.egg-info/PKG-INFO` & `renovosolutions.aws-ses-smtp-credentials-0.0.99/src/renovosolutions.aws_ses_smtp_credentials.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-ses-smtp-credentials
-Version: 0.0.98
+Version: 0.0.99
 Summary: AWS CDK Construct Library for generating SMTP credentials for SES and storing them in Secrets Manager
 Home-page: https://github.com/brandon/cdk-library-aws-ses-smtp-credentials.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/brandon/cdk-library-aws-ses-smtp-credentials.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-ses-smtp-credentials-0.0.98/src/renovosolutions.aws_ses_smtp_credentials.egg-info/SOURCES.txt` & `renovosolutions.aws-ses-smtp-credentials-0.0.99/src/renovosolutions.aws_ses_smtp_credentials.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/renovosolutions.aws_ses_smtp_credentials.egg-info/SOURCES.txt
 src/renovosolutions.aws_ses_smtp_credentials.egg-info/dependency_links.txt
 src/renovosolutions.aws_ses_smtp_credentials.egg-info/requires.txt
 src/renovosolutions.aws_ses_smtp_credentials.egg-info/top_level.txt
 src/ses-smtp-credentials/__init__.py
 src/ses-smtp-credentials/py.typed
 src/ses-smtp-credentials/_jsii/__init__.py
-src/ses-smtp-credentials/_jsii/cdk-library-aws-ses-smtp-credentials@0.0.98.jsii.tgz
+src/ses-smtp-credentials/_jsii/cdk-library-aws-ses-smtp-credentials@0.0.99.jsii.tgz
```

### Comparing `renovosolutions.aws-ses-smtp-credentials-0.0.98/src/ses-smtp-credentials/__init__.py` & `renovosolutions.aws-ses-smtp-credentials-0.0.99/src/ses-smtp-credentials/__init__.py`

 * *Files identical despite different names*

