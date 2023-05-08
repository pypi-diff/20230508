# Comparing `tmp/shady-island-0.0.8.tar.gz` & `tmp/shady-island-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shady-island-0.0.8.tar", last modified: Mon Aug  8 02:16:22 2022, max compression
+gzip compressed data, was "shady-island-0.0.9.tar", last modified: Fri Aug 12 15:07:39 2022, max compression
```

## Comparing `shady-island-0.0.8.tar` & `shady-island-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 02:16:22.246545 shady-island-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-08 02:16:08.000000 shady-island-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-08 02:16:08.000000 shady-island-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-08-08 02:16:22.246545 shady-island-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-08-08 02:16:08.000000 shady-island-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-08 02:16:08.000000 shady-island-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-08 02:16:22.246545 shady-island-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-08-08 02:16:08.000000 shady-island-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 02:16:22.246545 shady-island-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 02:16:22.246545 shady-island-0.0.8/src/shady_island/
--rw-r--r--   0 runner    (1001) docker     (121)    46357 2022-08-08 02:16:08.000000 shady-island-0.0.8/src/shady_island/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 02:16:22.246545 shady-island-0.0.8/src/shady_island/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-08-08 02:16:08.000000 shady-island-0.0.8/src/shady_island/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    48729 2022-08-08 02:16:08.000000 shady-island-0.0.8/src/shady_island/_jsii/shady-island@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 02:16:08.000000 shady-island-0.0.8/src/shady_island/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 02:16:22.246545 shady-island-0.0.8/src/shady_island.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-08-08 02:16:21.000000 shady-island-0.0.8/src/shady_island.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-08-08 02:16:22.000000 shady-island-0.0.8/src/shady_island.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 02:16:21.000000 shady-island-0.0.8/src/shady_island.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-08 02:16:22.000000 shady-island-0.0.8/src/shady_island.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-08 02:16:22.000000 shady-island-0.0.8/src/shady_island.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:07:39.781898 shady-island-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-12 15:07:22.000000 shady-island-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-12 15:07:22.000000 shady-island-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-08-12 15:07:39.781898 shady-island-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-08-12 15:07:22.000000 shady-island-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-12 15:07:22.000000 shady-island-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-12 15:07:39.781898 shady-island-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-08-12 15:07:22.000000 shady-island-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:07:39.781898 shady-island-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:07:39.781898 shady-island-0.0.9/src/shady_island/
+-rw-r--r--   0 runner    (1001) docker     (121)    47271 2022-08-12 15:07:22.000000 shady-island-0.0.9/src/shady_island/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:07:39.781898 shady-island-0.0.9/src/shady_island/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-08-12 15:07:22.000000 shady-island-0.0.9/src/shady_island/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50629 2022-08-12 15:07:22.000000 shady-island-0.0.9/src/shady_island/_jsii/shady-island@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 15:07:22.000000 shady-island-0.0.9/src/shady_island/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:07:39.781898 shady-island-0.0.9/src/shady_island.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-08-12 15:07:39.000000 shady-island-0.0.9/src/shady_island.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-08-12 15:07:39.000000 shady-island-0.0.9/src/shady_island.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 15:07:39.000000 shady-island-0.0.9/src/shady_island.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-12 15:07:39.000000 shady-island-0.0.9/src/shady_island.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-12 15:07:39.000000 shady-island-0.0.9/src/shady_island.egg-info/top_level.txt
```

### Comparing `shady-island-0.0.8/LICENSE` & `shady-island-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shady-island-0.0.8/PKG-INFO` & `shady-island-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shady-island
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities and constructs for the AWS CDK
 Home-page: https://libreworks.github.io/shady-island/
 Author: LibreWorks Contributors
 License: Apache-2.0
 Project-URL: Source, https://github.com:libreworks/shady-island.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `shady-island-0.0.8/README.md` & `shady-island-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shady-island-0.0.8/setup.py` & `shady-island-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "shady-island",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "Utilities and constructs for the AWS CDK",
     "license": "Apache-2.0",
     "url": "https://libreworks.github.io/shady-island/",
     "long_description_content_type": "text/markdown",
     "author": "LibreWorks Contributors",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "shady_island",
         "shady_island._jsii"
     ],
     "package_data": {
         "shady_island._jsii": [
-            "shady-island@0.0.8.jsii.tgz"
+            "shady-island@0.0.9.jsii.tgz"
         ],
         "shady_island": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `shady-island-0.0.8/src/shady_island/__init__.py` & `shady-island-0.0.9/src/shady_island/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,33 @@
         '''
         if __debug__:
             type_hints = typing.get_type_hints(Tier.__init__)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument label", value=label, expected_type=type_hints["label"])
         jsii.create(self.__class__, self, [id, label])
 
+    @jsii.member(jsii_name="parse") # type: ignore[misc]
+    @builtins.classmethod
+    def parse(cls, value: builtins.str) -> "Tier":
+        '''Return the deployment tier that corresponds to the provided value.
+
+        Production: "live", "prod", or "production".
+        Acceptance: "uat", "stage", "staging", or "acceptance".
+        Testing: "qc", "qa", "test", or "testing".
+        Development: anything else.
+
+        :param value: - The value to parse, case-insensitive.
+
+        :return: The matching deployment tier, or else ``DEVELOPMENT``.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Tier.parse)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        return typing.cast("Tier", jsii.sinvoke(cls, "parse", [value]))
+
     @jsii.member(jsii_name="applyTags")
     def apply_tags(self, construct: constructs.IConstruct) -> None:
         '''Adds the label of this tier as a tag to the provided construct.
 
         :param construct: -
         '''
         if __debug__:
@@ -592,14 +611,16 @@
               env: { account: '123456789012', region: 'us-east-1' },
             });
             const networkStack = exampleDev.createStack('Network', {});
             assert.strictEqual(networkStack.stackName, 'example-dev-network').
             
             You can override the `env` and `stackName` properties in the `props`
             argument if desired.
+            
+            The stack will have a `DeploymentTier` tag added, set to the tier label.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(Workload.create_stack)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = aws_cdk.StackProps(
             analytics_reporting=analytics_reporting,
             description=description,
```

### Comparing `shady-island-0.0.8/src/shady_island.egg-info/PKG-INFO` & `shady-island-0.0.9/src/shady_island.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shady-island
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities and constructs for the AWS CDK
 Home-page: https://libreworks.github.io/shady-island/
 Author: LibreWorks Contributors
 License: Apache-2.0
 Project-URL: Source, https://github.com:libreworks/shady-island.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

