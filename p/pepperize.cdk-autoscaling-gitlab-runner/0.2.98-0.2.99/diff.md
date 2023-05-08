# Comparing `tmp/pepperize.cdk-autoscaling-gitlab-runner-0.2.98.tar.gz` & `tmp/pepperize.cdk-autoscaling-gitlab-runner-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperize.cdk-autoscaling-gitlab-runner-0.2.98.tar", last modified: Fri Jun 17 02:56:20 2022, max compression
+gzip compressed data, was "pepperize.cdk-autoscaling-gitlab-runner-0.2.99.tar", last modified: Fri Jun 17 03:03:22 2022, max compression
```

## Comparing `pepperize.cdk-autoscaling-gitlab-runner-0.2.98.tar` & `pepperize.cdk-autoscaling-gitlab-runner-0.2.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 02:56:20.812699 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-06-17 02:56:09.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-17 02:56:09.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    20115 2022-06-17 02:56:20.812699 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19099 2022-06-17 02:56:09.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-06-17 02:56:09.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 02:56:20.812699 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-06-17 02:56:09.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 02:56:20.808699 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 02:56:20.812699 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20115 2022-06-17 02:56:20.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-06-17 02:56:20.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 02:56:20.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-17 02:56:20.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-17 02:56:20.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 02:56:20.812699 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize_cdk_autoscaling_gitlab_runner/
--rw-r--r--   0 runner    (1001) docker     (121)   139243 2022-06-17 02:56:09.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize_cdk_autoscaling_gitlab_runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 02:56:20.812699 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize_cdk_autoscaling_gitlab_runner/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-06-17 02:56:09.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize_cdk_autoscaling_gitlab_runner/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   138723 2022-06-17 02:56:09.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize_cdk_autoscaling_gitlab_runner/_jsii/cdk-autoscaling-gitlab-runner@0.2.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 02:56:09.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize_cdk_autoscaling_gitlab_runner/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 03:03:22.174417 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-06-17 03:03:08.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-17 03:03:08.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    20115 2022-06-17 03:03:22.174417 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    19099 2022-06-17 03:03:08.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-06-17 03:03:08.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 03:03:22.174417 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-06-17 03:03:08.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 03:03:22.170416 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 03:03:22.170416 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    20115 2022-06-17 03:03:21.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-06-17 03:03:22.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 03:03:21.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-17 03:03:21.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-17 03:03:22.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 03:03:22.174417 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize_cdk_autoscaling_gitlab_runner/
+-rw-r--r--   0 runner    (1001) docker     (121)   139243 2022-06-17 03:03:08.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize_cdk_autoscaling_gitlab_runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 03:03:22.174417 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize_cdk_autoscaling_gitlab_runner/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-06-17 03:03:08.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize_cdk_autoscaling_gitlab_runner/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   138724 2022-06-17 03:03:08.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize_cdk_autoscaling_gitlab_runner/_jsii/cdk-autoscaling-gitlab-runner@0.2.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 03:03:08.000000 pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize_cdk_autoscaling_gitlab_runner/py.typed
```

### Comparing `pepperize.cdk-autoscaling-gitlab-runner-0.2.98/LICENSE` & `pepperize.cdk-autoscaling-gitlab-runner-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-autoscaling-gitlab-runner-0.2.98/PKG-INFO` & `pepperize.cdk-autoscaling-gitlab-runner-0.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-autoscaling-gitlab-runner
-Version: 0.2.98
+Version: 0.2.99
 Summary: AWS CDK GitLab Runner autoscaling on EC2 instances using docker+machine executor.
 Home-page: https://github.com/pepperize/cdk-autoscaling-gitlab-runner.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/cdk-autoscaling-gitlab-runner.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pepperize.cdk-autoscaling-gitlab-runner-0.2.98/README.md` & `pepperize.cdk-autoscaling-gitlab-runner-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-autoscaling-gitlab-runner-0.2.98/setup.py` & `pepperize.cdk-autoscaling-gitlab-runner-0.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pepperize.cdk-autoscaling-gitlab-runner",
-    "version": "0.2.98",
+    "version": "0.2.99",
     "description": "AWS CDK GitLab Runner autoscaling on EC2 instances using docker+machine executor.",
     "license": "MIT",
     "url": "https://github.com/pepperize/cdk-autoscaling-gitlab-runner.git",
     "long_description_content_type": "text/markdown",
     "author": "Patrick Florek<patrick.florek@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pepperize_cdk_autoscaling_gitlab_runner",
         "pepperize_cdk_autoscaling_gitlab_runner._jsii"
     ],
     "package_data": {
         "pepperize_cdk_autoscaling_gitlab_runner._jsii": [
-            "cdk-autoscaling-gitlab-runner@0.2.98.jsii.tgz"
+            "cdk-autoscaling-gitlab-runner@0.2.99.jsii.tgz"
         ],
         "pepperize_cdk_autoscaling_gitlab_runner": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/PKG-INFO` & `pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-autoscaling-gitlab-runner
-Version: 0.2.98
+Version: 0.2.99
 Summary: AWS CDK GitLab Runner autoscaling on EC2 instances using docker+machine executor.
 Home-page: https://github.com/pepperize/cdk-autoscaling-gitlab-runner.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/cdk-autoscaling-gitlab-runner.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/SOURCES.txt` & `pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/SOURCES.txt
 src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/dependency_links.txt
 src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/requires.txt
 src/pepperize.cdk_autoscaling_gitlab_runner.egg-info/top_level.txt
 src/pepperize_cdk_autoscaling_gitlab_runner/__init__.py
 src/pepperize_cdk_autoscaling_gitlab_runner/py.typed
 src/pepperize_cdk_autoscaling_gitlab_runner/_jsii/__init__.py
-src/pepperize_cdk_autoscaling_gitlab_runner/_jsii/cdk-autoscaling-gitlab-runner@0.2.98.jsii.tgz
+src/pepperize_cdk_autoscaling_gitlab_runner/_jsii/cdk-autoscaling-gitlab-runner@0.2.99.jsii.tgz
```

### Comparing `pepperize.cdk-autoscaling-gitlab-runner-0.2.98/src/pepperize_cdk_autoscaling_gitlab_runner/__init__.py` & `pepperize.cdk-autoscaling-gitlab-runner-0.2.99/src/pepperize_cdk_autoscaling_gitlab_runner/__init__.py`

 * *Files identical despite different names*

