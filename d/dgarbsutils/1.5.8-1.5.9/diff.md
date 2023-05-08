# Comparing `tmp/dgarbsutils-1.5.8.tar.gz` & `tmp/dgarbsutils-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgarbsutils-1.5.8.tar", last modified: Tue Feb  7 14:20:10 2023, max compression
+gzip compressed data, was "dgarbsutils-1.5.9.tar", last modified: Tue Feb 21 14:54:33 2023, max compression
```

## Comparing `dgarbsutils-1.5.8.tar` & `dgarbsutils-1.5.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-07 14:20:10.758400 dgarbsutils-1.5.8/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1072 2022-06-10 11:14:25.000000 dgarbsutils-1.5.8/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      913 2023-02-07 14:20:10.762400 dgarbsutils-1.5.8/PKG-INFO
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      419 2022-06-14 21:50:35.000000 dgarbsutils-1.5.8/README.md
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       84 2022-06-13 13:28:13.000000 dgarbsutils-1.5.8/pyproject.toml
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      693 2023-02-07 14:20:10.762400 dgarbsutils-1.5.8/setup.cfg
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-07 14:20:10.750400 dgarbsutils-1.5.8/src/
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-07 14:20:10.758400 dgarbsutils-1.5.8/src/dgarbsutils/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     2312 2022-08-10 12:24:46.000000 dgarbsutils-1.5.8/src/dgarbsutils/Cloudwatch.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5600 2022-09-20 17:39:03.000000 dgarbsutils-1.5.8/src/dgarbsutils/DynamoDB.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2069 2022-12-05 15:01:17.000000 dgarbsutils-1.5.8/src/dgarbsutils/EventBridge.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5153 2023-02-07 14:19:45.000000 dgarbsutils-1.5.8/src/dgarbsutils/GraphMail.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-06-13 13:28:13.000000 dgarbsutils-1.5.8/src/dgarbsutils/__init__.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5991 2023-01-17 18:38:11.000000 dgarbsutils-1.5.8/src/dgarbsutils/awsUtils.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5839 2023-01-20 20:04:01.000000 dgarbsutils-1.5.8/src/dgarbsutils/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-07 14:20:10.758400 dgarbsutils-1.5.8/src/dgarbsutils.egg-info/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      913 2023-02-07 14:20:10.000000 dgarbsutils-1.5.8/src/dgarbsutils.egg-info/PKG-INFO
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      455 2023-02-07 14:20:10.000000 dgarbsutils-1.5.8/src/dgarbsutils.egg-info/SOURCES.txt
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        1 2023-02-07 14:20:10.000000 dgarbsutils-1.5.8/src/dgarbsutils.egg-info/dependency_links.txt
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       31 2023-02-07 14:20:10.000000 dgarbsutils-1.5.8/src/dgarbsutils.egg-info/requires.txt
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       12 2023-02-07 14:20:10.000000 dgarbsutils-1.5.8/src/dgarbsutils.egg-info/top_level.txt
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-07 14:20:10.758400 dgarbsutils-1.5.8/tests/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1782 2022-07-16 22:59:17.000000 dgarbsutils-1.5.8/tests/test_utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1072 2022-06-10 11:14:25.000000 dgarbsutils-1.5.9/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      913 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/PKG-INFO
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      419 2022-06-14 21:50:35.000000 dgarbsutils-1.5.9/README.md
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       84 2022-06-13 13:28:13.000000 dgarbsutils-1.5.9/pyproject.toml
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      693 2023-02-21 14:54:33.814099 dgarbsutils-1.5.9/setup.cfg
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.806100 dgarbsutils-1.5.9/src/
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/src/dgarbsutils/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     2312 2022-08-10 12:24:46.000000 dgarbsutils-1.5.9/src/dgarbsutils/Cloudwatch.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5610 2023-02-21 14:53:27.000000 dgarbsutils-1.5.9/src/dgarbsutils/DynamoDB.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2069 2022-12-05 15:01:17.000000 dgarbsutils-1.5.9/src/dgarbsutils/EventBridge.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5153 2023-02-07 14:19:45.000000 dgarbsutils-1.5.9/src/dgarbsutils/GraphMail.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-06-13 13:28:13.000000 dgarbsutils-1.5.9/src/dgarbsutils/__init__.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5991 2023-01-17 18:38:11.000000 dgarbsutils-1.5.9/src/dgarbsutils/awsUtils.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5839 2023-01-20 20:04:01.000000 dgarbsutils-1.5.9/src/dgarbsutils/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      913 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/PKG-INFO
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      455 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/SOURCES.txt
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        1 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/dependency_links.txt
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       31 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/requires.txt
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       12 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/top_level.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/tests/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1782 2022-07-16 22:59:17.000000 dgarbsutils-1.5.9/tests/test_utils.py
```

### Comparing `dgarbsutils-1.5.8/LICENSE` & `dgarbsutils-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.5.8/PKG-INFO` & `dgarbsutils-1.5.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgarbsutils
-Version: 1.5.8
+Version: 1.5.9
 Summary: A set of curated utils
 Home-page: https://github.com/dgarbalo/py-utils
 Author: Devon Garbalosa
 Author-email: dgarbalo@gmail.com
 Project-URL: Bug Tracker, https://github.com/dgarbalo/py-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dgarbsutils-1.5.8/setup.cfg` & `dgarbsutils-1.5.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dgarbsutils
-version = 1.5.8
+version = 1.5.9
 author = Devon Garbalosa
 author_email = dgarbalo@gmail.com
 description = A set of curated utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dgarbalo/py-utils
 project_urls =
```

### Comparing `dgarbsutils-1.5.8/src/dgarbsutils/Cloudwatch.py` & `dgarbsutils-1.5.9/src/dgarbsutils/Cloudwatch.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.5.8/src/dgarbsutils/DynamoDB.py` & `dgarbsutils-1.5.9/src/dgarbsutils/DynamoDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,21 @@
         data_type = str(type(data))
 
         if data_type == "<class 'str'>":
             if " ".join(data.split()) == "":
                 return {"NULL": True}
             return {"S": " ".join(data.split())}
         if data_type in ["<class 'int'>", "<class 'float'>", "<class 'complex'>"]:
-            return {"N": data}
+            return {"N": str(data)}
         if data_type == "<class 'list'>":
             return {"L": [self.dynamodb_translate_data_type(item) for item in data]}
         if data_type == "<class 'dict'>":
             return {"M": {key: self.dynamodb_translate_data_type(value) for key, value in data.items()}}
         if data_type == "<class 'bool'>":
-            return {"BOOL": data}
+            return {"BOOL": str(data)}
         if data_type == "<class 'NoneType'>":
             return {"NULL": True}
         return None
 
     def dynamodb_convert_to_json(self, data):
         """converts the dynamodb json to a python json"""
         output = {}
```

### Comparing `dgarbsutils-1.5.8/src/dgarbsutils/EventBridge.py` & `dgarbsutils-1.5.9/src/dgarbsutils/EventBridge.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.5.8/src/dgarbsutils/GraphMail.py` & `dgarbsutils-1.5.9/src/dgarbsutils/GraphMail.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.5.8/src/dgarbsutils/awsUtils.py` & `dgarbsutils-1.5.9/src/dgarbsutils/awsUtils.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.5.8/src/dgarbsutils/utils.py` & `dgarbsutils-1.5.9/src/dgarbsutils/utils.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.5.8/src/dgarbsutils.egg-info/PKG-INFO` & `dgarbsutils-1.5.9/src/dgarbsutils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgarbsutils
-Version: 1.5.8
+Version: 1.5.9
 Summary: A set of curated utils
 Home-page: https://github.com/dgarbalo/py-utils
 Author: Devon Garbalosa
 Author-email: dgarbalo@gmail.com
 Project-URL: Bug Tracker, https://github.com/dgarbalo/py-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dgarbsutils-1.5.8/tests/test_utils.py` & `dgarbsutils-1.5.9/tests/test_utils.py`

 * *Files identical despite different names*

