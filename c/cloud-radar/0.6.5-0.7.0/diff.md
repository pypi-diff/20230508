# Comparing `tmp/cloud_radar-0.6.5.tar.gz` & `tmp/cloud_radar-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_radar-0.6.5.tar", max compression
+gzip compressed data, was "cloud_radar-0.7.0.tar", max compression
```

## Comparing `cloud_radar-0.6.5.tar` & `cloud_radar-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-01 19:49:52.609153 cloud_radar-0.6.5/LICENSE.txt
--rw-r--r--   0        0        0    12792 2023-05-01 19:49:52.609153 cloud_radar-0.6.5/README.md
--rw-r--r--   0        0        0     1431 2023-05-01 19:50:07.737241 cloud_radar-0.6.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/__init__.py
--rw-r--r--   0        0        0       48 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/e2e/__init__.py
--rw-r--r--   0        0        0     1677 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/e2e/_stack.py
--rw-r--r--   0        0        0       57 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/unit/__init__.py
--rw-r--r--   0        0        0     8886 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/unit/_template.py
--rw-r--r--   0        0        0    24791 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/unit/functions.py
--rw-r--r--   0        0        0    13992 1970-01-01 00:00:00.000000 cloud_radar-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 13:56:13.907853 cloud_radar-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0    12786 2023-05-08 13:56:13.907853 cloud_radar-0.7.0/README.md
+-rw-r--r--   0        0        0     1431 2023-05-08 13:56:28.571994 cloud_radar-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/e2e/__init__.py
+-rw-r--r--   0        0        0     1677 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/e2e/_stack.py
+-rw-r--r--   0        0        0       57 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/__init__.py
+-rw-r--r--   0        0        0      711 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_condition.py
+-rw-r--r--   0        0        0     1822 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_output.py
+-rw-r--r--   0        0        0     3199 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_parameter.py
+-rw-r--r--   0        0        0     3872 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_resource.py
+-rw-r--r--   0        0        0     5230 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_stack.py
+-rw-r--r--   0        0        0     9167 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/_template.py
+-rw-r--r--   0        0        0    24791 2023-05-08 13:56:13.911853 cloud_radar-0.7.0/src/cloud_radar/cf/unit/functions.py
+-rw-r--r--   0        0        0    13986 1970-01-01 00:00:00.000000 cloud_radar-0.7.0/PKG-INFO
```

### Comparing `cloud_radar-0.6.5/LICENSE.txt` & `cloud_radar-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.6.5/README.md` & `cloud_radar-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -132,25 +132,25 @@
 
 # template_path can be a str or a Path object
 template = Template.from_yaml(template_path.resolve())
 
 params = {"BucketPrefix": "testing", "KeepBucket": "TRUE"}
 
 # parameters and region are optional arguments.
-result = template.render(params, region="us-west-2")
+stack = template.create_stack(params, region="us-west-2")
 
-assert "LogsBucket" not in result["Resources"]
+stack.no_resource("LogsBucket")
 
-bucket = result["Resources"]["RetainLogsBucket"]
+bucket = stack.get_resource("RetainLogsBucket")
 
 assert "DeletionPolicy" in bucket
 
 assert bucket["DeletionPolicy"] == "Retain"
 
-bucket_name = bucket["Properties"]["BucketName"]
+bucket_name = bucket.get_property_value("BucketName")
 
 assert "us-west-2" in bucket_name
 ```
 
 The AWS pseudo variables are all class attributes and can be modified before rendering a template.
 ```python
 # The value of 'AWS::AccountId' in !Sub "My AccountId is ${AWS::AccountId}" can be changed:
```

### Comparing `cloud_radar-0.6.5/pyproject.toml` & `cloud_radar-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-radar"
-version = "0.6.5"
+version = "0.7.0"
 description = "Run functional tests on cloudformation stacks."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/DontShaveTheYak/cloud-radar"
 keywords = ["aws", "cloudformation", "cloud-radar", "testing", "taskcat", "cloud", "radar"]
 classifiers = [
```

### Comparing `cloud_radar-0.6.5/src/cloud_radar/cf/e2e/_stack.py` & `cloud_radar-0.7.0/src/cloud_radar/cf/e2e/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.6.5/src/cloud_radar/cf/unit/_template.py` & `cloud_radar-0.7.0/src/cloud_radar/cf/unit/_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any, Callable, Dict, Optional, Union
 
 from cfn_tools import dump_yaml, load_yaml  # type: ignore
 
 import yaml
 
 from . import functions
+from ._stack import Stack
 
 IntrinsicFunc = Callable[["Template", Any], Any]
 
 
 class Template:
     """Loads a Cloudformation template file so that it's parameters
     and conditions can be rendered into their final form for testing.
@@ -121,14 +122,26 @@
 
             if not keep_resource:
                 del self.template["Resources"][r_name]
                 continue
 
         return self.template
 
+    def create_stack(
+        self, params: Optional[Dict[str, str]] = None, region: Optional[str] = None
+    ):
+        if region:
+            self.Region = region
+
+        self.render(params)
+
+        stack = Stack(self.template)
+
+        return stack
+
     def resolve_values(
         self,
         data: Any,
         allowed_func: functions.Dispatch,
     ) -> Any:
         """Recurses through a Cloudformation template. Solving all
         references and variables along the way.
```

### Comparing `cloud_radar-0.6.5/src/cloud_radar/cf/unit/functions.py` & `cloud_radar-0.7.0/src/cloud_radar/cf/unit/functions.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.6.5/PKG-INFO` & `cloud_radar-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-radar
-Version: 0.6.5
+Version: 0.7.0
 Summary: Run functional tests on cloudformation stacks.
 Home-page: https://github.com/DontShaveTheYak/cloud-radar
 License: Apache-2.0
 Keywords: aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -160,25 +160,25 @@
 
 # template_path can be a str or a Path object
 template = Template.from_yaml(template_path.resolve())
 
 params = {"BucketPrefix": "testing", "KeepBucket": "TRUE"}
 
 # parameters and region are optional arguments.
-result = template.render(params, region="us-west-2")
+stack = template.create_stack(params, region="us-west-2")
 
-assert "LogsBucket" not in result["Resources"]
+stack.no_resource("LogsBucket")
 
-bucket = result["Resources"]["RetainLogsBucket"]
+bucket = stack.get_resource("RetainLogsBucket")
 
 assert "DeletionPolicy" in bucket
 
 assert bucket["DeletionPolicy"] == "Retain"
 
-bucket_name = bucket["Properties"]["BucketName"]
+bucket_name = bucket.get_property_value("BucketName")
 
 assert "us-west-2" in bucket_name
 ```
 
 The AWS pseudo variables are all class attributes and can be modified before rendering a template.
 ```python
 # The value of 'AWS::AccountId' in !Sub "My AccountId is ${AWS::AccountId}" can be changed:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-radar Version: 0.6.5 Summary: Run functional
+Metadata-Version: 2.1 Name: cloud-radar Version: 0.7.0 Summary: Run functional
 tests on cloudformation stacks. Home-page: https://github.com/DontShaveTheYak/
 cloud-radar License: Apache-2.0 Keywords: aws,cloudformation,cloud-
 radar,testing,taskcat,cloud,radar Author: Levi Blaney Author-email:
 shadycuz@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -59,39 +59,39 @@
 expand) Using Cloud-Radar starts by importing it into your test file or
 framework. We will use this [Template](./tests/templates/log_bucket/
 log_bucket.yaml) as an example. ```python from pathlib import Path from
 cloud_radar.cf.unit import Template template_path = Path("tests/templates/
 log_bucket/log_bucket.yaml") # template_path can be a str or a Path object
 template = Template.from_yaml(template_path.resolve()) params =
 {"BucketPrefix": "testing", "KeepBucket": "TRUE"} # parameters and region are
-optional arguments. result = template.render(params, region="us-west-2") assert
-"LogsBucket" not in result["Resources"] bucket = result["Resources"]
-["RetainLogsBucket"] assert "DeletionPolicy" in bucket assert bucket
-["DeletionPolicy"] == "Retain" bucket_name = bucket["Properties"]["BucketName"]
-assert "us-west-2" in bucket_name ``` The AWS pseudo variables are all class
-attributes and can be modified before rendering a template. ```python # The
-value of 'AWS::AccountId' in !Sub "My AccountId is ${AWS::AccountId}" can be
-changed: Template.AccountId = '8675309' ``` _Note: Region should only be
-changed to change the default value. To change the region during testing pass
-the desired region to render(region='us-west-2')_ The default values for psedo
-variables: | Name | Default Value | | ---------------- | --------------- | |
-AccountId | "555555555555" | | NotificationARNs | [] | | **NoValue** | "" | |
-**Partition** | "aws" | | Region | "us-east-1" | | **StackId** | "" | |
-**StackName** | "" | | **URLSuffix** | "amazonaws.com" | _Note: Bold variables
-are not fully impletmented yet see the [Roadmap](#roadmap)_ A real unit testing
-example using Pytest can be seen [here](./tests/test_cf/test_examples/
-test_unit.py)   Functional Testing (Click to expand) Using Cloud-Radar starts
-by importing it into your test file or framework. ```python from pathlib import
-Path from cloud_radar.cf.e2e import Stack # Stack is a context manager that
-makes sure your stacks are deleted after testing. template_path = Path("tests/
-templates/log_bucket/log_bucket.yaml") params = {"BucketPrefix": "testing",
-"KeepBucket": "False"} regions = ['us-west-2'] # template_path can be a string
-or a Path object. # params can be optional if all your template params have
-default values # regions can be optional, default region is 'us-east-1' with
-Stack(template_path, params, regions) as stacks: # Stacks will be created and
+optional arguments. stack = template.create_stack(params, region="us-west-2")
+stack.no_resource("LogsBucket") bucket = stack.get_resource("RetainLogsBucket")
+assert "DeletionPolicy" in bucket assert bucket["DeletionPolicy"] == "Retain"
+bucket_name = bucket.get_property_value("BucketName") assert "us-west-2" in
+bucket_name ``` The AWS pseudo variables are all class attributes and can be
+modified before rendering a template. ```python # The value of 'AWS::AccountId'
+in !Sub "My AccountId is ${AWS::AccountId}" can be changed: Template.AccountId
+= '8675309' ``` _Note: Region should only be changed to change the default
+value. To change the region during testing pass the desired region to render
+(region='us-west-2')_ The default values for psedo variables: | Name | Default
+Value | | ---------------- | --------------- | | AccountId | "555555555555" | |
+NotificationARNs | [] | | **NoValue** | "" | | **Partition** | "aws" | | Region
+| "us-east-1" | | **StackId** | "" | | **StackName** | "" | | **URLSuffix** |
+"amazonaws.com" | _Note: Bold variables are not fully impletmented yet see the
+[Roadmap](#roadmap)_ A real unit testing example using Pytest can be seen
+[here](./tests/test_cf/test_examples/test_unit.py)   Functional Testing (Click
+to expand) Using Cloud-Radar starts by importing it into your test file or
+framework. ```python from pathlib import Path from cloud_radar.cf.e2e import
+Stack # Stack is a context manager that makes sure your stacks are deleted
+after testing. template_path = Path("tests/templates/log_bucket/
+log_bucket.yaml") params = {"BucketPrefix": "testing", "KeepBucket": "False"}
+regions = ['us-west-2'] # template_path can be a string or a Path object. #
+params can be optional if all your template params have default values #
+regions can be optional, default region is 'us-east-1' with Stack
+(template_path, params, regions) as stacks: # Stacks will be created and
 returned as a list in the stacks variable. for stack in stacks: # stack will be
 an instance of Taskcat's Stack class. # It has all the expected properties like
 parameters, outputs and resources print(f"Testing {stack.name}") bucket_name =
 "" for output in stack.outputs: if output.key == "LogsBucketName": bucket_name
 = output.value break assert "logs" in bucket_name assert stack.region.name in
 bucket_name print(f"Created bucket: {bucket_name}") # Once the test is over
 then all resources will be deleted from your AWS account. ``` You can use
```

