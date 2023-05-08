# Comparing `tmp/cdk8s-jenkins-0.0.98.tar.gz` & `tmp/cdk8s-jenkins-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-jenkins-0.0.98.tar", last modified: Sun Oct 30 00:36:00 2022, max compression
+gzip compressed data, was "cdk8s-jenkins-0.0.99.tar", last modified: Mon Oct 31 00:36:16 2022, max compression
```

## Comparing `cdk8s-jenkins-0.0.98.tar` & `cdk8s-jenkins-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:36:00.770425 cdk8s-jenkins-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-30 00:35:48.000000 cdk8s-jenkins-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-30 00:35:48.000000 cdk8s-jenkins-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-10-30 00:36:00.770425 cdk8s-jenkins-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4560 2022-10-30 00:35:48.000000 cdk8s-jenkins-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-30 00:35:48.000000 cdk8s-jenkins-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-30 00:36:00.770425 cdk8s-jenkins-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-10-30 00:35:48.000000 cdk8s-jenkins-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:36:00.770425 cdk8s-jenkins-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:36:00.770425 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins/
--rw-r--r--   0 runner    (1001) docker     (121)    24117 2022-10-30 00:35:48.000000 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:36:00.770425 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-30 00:35:48.000000 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   143844 2022-10-30 00:35:48.000000 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins/_jsii/cdk8s-jenkins@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 00:35:48.000000 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 00:36:00.770425 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-10-30 00:36:00.000000 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-10-30 00:36:00.000000 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 00:36:00.000000 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-30 00:36:00.000000 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-30 00:36:00.000000 cdk8s-jenkins-0.0.98/src/cdk8s_jenkins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 00:36:16.170388 cdk8s-jenkins-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-31 00:36:04.000000 cdk8s-jenkins-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-31 00:36:04.000000 cdk8s-jenkins-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-10-31 00:36:16.166388 cdk8s-jenkins-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4560 2022-10-31 00:36:04.000000 cdk8s-jenkins-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-31 00:36:04.000000 cdk8s-jenkins-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 00:36:16.170388 cdk8s-jenkins-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-10-31 00:36:04.000000 cdk8s-jenkins-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 00:36:16.166388 cdk8s-jenkins-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 00:36:16.166388 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins/
+-rw-r--r--   0 runner    (1001) docker     (121)    24117 2022-10-31 00:36:04.000000 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 00:36:16.166388 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-31 00:36:04.000000 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   143843 2022-10-31 00:36:04.000000 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins/_jsii/cdk8s-jenkins@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 00:36:04.000000 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 00:36:16.166388 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-10-31 00:36:15.000000 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-10-31 00:36:16.000000 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 00:36:15.000000 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-31 00:36:16.000000 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-31 00:36:16.000000 cdk8s-jenkins-0.0.99/src/cdk8s_jenkins.egg-info/top_level.txt
```

### Comparing `cdk8s-jenkins-0.0.98/LICENSE` & `cdk8s-jenkins-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-jenkins-0.0.98/PKG-INFO` & `cdk8s-jenkins-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-jenkins
-Version: 0.0.98
+Version: 0.0.99
 Summary: Jenkins construct for CDK8s
 Home-page: https://github.com/cdk8s-team/cdk8s-jenkins
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-jenkins
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk8s-jenkins-0.0.98/README.md` & `cdk8s-jenkins-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-jenkins-0.0.98/setup.py` & `cdk8s-jenkins-0.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-jenkins",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "Jenkins construct for CDK8s",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-jenkins",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_jenkins",
         "cdk8s_jenkins._jsii"
     ],
     "package_data": {
         "cdk8s_jenkins._jsii": [
-            "cdk8s-jenkins@0.0.98.jsii.tgz"
+            "cdk8s-jenkins@0.0.99.jsii.tgz"
         ],
         "cdk8s_jenkins": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-jenkins-0.0.98/src/cdk8s_jenkins/__init__.py` & `cdk8s-jenkins-0.0.99/src/cdk8s_jenkins/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-jenkins-0.0.98/src/cdk8s_jenkins.egg-info/PKG-INFO` & `cdk8s-jenkins-0.0.99/src/cdk8s_jenkins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-jenkins
-Version: 0.0.98
+Version: 0.0.99
 Summary: Jenkins construct for CDK8s
 Home-page: https://github.com/cdk8s-team/cdk8s-jenkins
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-jenkins
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

