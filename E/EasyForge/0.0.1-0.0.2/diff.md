# Comparing `tmp/EasyForge-0.0.1.tar.gz` & `tmp/EasyForge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyForge-0.0.1.tar", last modified: Mon May  8 06:46:54 2023, max compression
+gzip compressed data, was "EasyForge-0.0.2.tar", last modified: Mon May  8 07:09:25 2023, max compression
```

## Comparing `EasyForge-0.0.1.tar` & `EasyForge-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 06:46:54.638590 EasyForge-0.0.1/
--rw-rw-rw-   0        0        0    35825 2023-05-08 06:00:49.000000 EasyForge-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1578 2023-05-08 06:46:54.638590 EasyForge-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1121 2023-05-08 05:26:53.000000 EasyForge-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 06:46:54.639588 EasyForge-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-05-08 05:53:51.000000 EasyForge-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:46:54.600689 EasyForge-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 06:46:54.616649 EasyForge-0.0.1/src/EasyForge/
--rw-rw-rw-   0        0        0      980 2023-04-27 10:13:11.000000 EasyForge-0.0.1/src/EasyForge/Authentication.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:46:54.636595 EasyForge-0.0.1/src/EasyForge/DataManagement/
--rw-rw-rw-   0        0        0     2941 2023-05-08 06:44:39.000000 EasyForge-0.0.1/src/EasyForge/DataManagement/ACC.py
--rw-rw-rw-   0        0        0     5045 2023-05-08 06:44:39.000000 EasyForge-0.0.1/src/EasyForge/DataManagement/OSS.py
--rw-rw-rw-   0        0        0        0 2023-04-28 06:02:17.000000 EasyForge-0.0.1/src/EasyForge/DataManagement/__init__.py
--rw-rw-rw-   0        0        0      556 2023-05-08 06:44:09.000000 EasyForge-0.0.1/src/EasyForge/DesignAutomation.py
--rw-rw-rw-   0        0        0     5023 2023-05-08 06:44:09.000000 EasyForge-0.0.1/src/EasyForge/ModelDerivative.py
--rw-rw-rw-   0        0        0        0 2023-04-26 10:56:10.000000 EasyForge-0.0.1/src/EasyForge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:46:54.633603 EasyForge-0.0.1/src/EasyForge.egg-info/
--rw-rw-rw-   0        0        0     1578 2023-05-08 06:46:54.000000 EasyForge-0.0.1/src/EasyForge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-05-08 06:46:54.000000 EasyForge-0.0.1/src/EasyForge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 06:46:54.000000 EasyForge-0.0.1/src/EasyForge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-08 06:46:54.000000 EasyForge-0.0.1/src/EasyForge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 07:09:25.628766 EasyForge-0.0.2/
+-rw-rw-rw-   0        0        0    35825 2023-05-08 06:00:49.000000 EasyForge-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1562 2023-05-08 07:09:25.628766 EasyForge-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1105 2023-05-08 07:01:14.000000 EasyForge-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 07:09:25.629763 EasyForge-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-05-08 07:02:03.000000 EasyForge-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:09:25.597849 EasyForge-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 07:09:25.608820 EasyForge-0.0.2/src/EasyForge/
+-rw-rw-rw-   0        0        0      980 2023-04-27 10:13:11.000000 EasyForge-0.0.2/src/EasyForge/Authentication.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:09:25.626771 EasyForge-0.0.2/src/EasyForge/DataManagement/
+-rw-rw-rw-   0        0        0     2941 2023-05-08 06:44:39.000000 EasyForge-0.0.2/src/EasyForge/DataManagement/ACC.py
+-rw-rw-rw-   0        0        0     5045 2023-05-08 06:44:39.000000 EasyForge-0.0.2/src/EasyForge/DataManagement/OSS.py
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:02:17.000000 EasyForge-0.0.2/src/EasyForge/DataManagement/__init__.py
+-rw-rw-rw-   0        0        0      556 2023-05-08 06:44:09.000000 EasyForge-0.0.2/src/EasyForge/DesignAutomation.py
+-rw-rw-rw-   0        0        0     5023 2023-05-08 06:44:09.000000 EasyForge-0.0.2/src/EasyForge/ModelDerivative.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 10:56:10.000000 EasyForge-0.0.2/src/EasyForge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:09:25.622784 EasyForge-0.0.2/src/EasyForge.egg-info/
+-rw-rw-rw-   0        0        0     1562 2023-05-08 07:09:25.000000 EasyForge-0.0.2/src/EasyForge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-05-08 07:09:25.000000 EasyForge-0.0.2/src/EasyForge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 07:09:25.000000 EasyForge-0.0.2/src/EasyForge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 07:09:25.000000 EasyForge-0.0.2/src/EasyForge.egg-info/top_level.txt
```

### Comparing `EasyForge-0.0.1/LICENSE.txt` & `EasyForge-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EasyForge-0.0.1/PKG-INFO` & `EasyForge-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyForge
-Version: 0.0.1
+Version: 0.0.2
 Summary: To Make easy to use Forge (APS) by python
 Author: DKVG
 Author-email: gadellidk@gmail.com
 Keywords: EasyForge forge APS forge-python python-aps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,28 +19,28 @@
 
 In this Package the following Forge API:<br>
 1.Data Management API<br>
 2.Authentication API <br>
 3.ModelDerivative API<br>
 </p>
 <p>The Following are sample examples.</p>
-<label>
+<p>
 Example 1 (To create Authenticate Token): <br>
 from forge.Authentication import Authenticate<br>
 def GenerateToken():<br>
     app_client_id = 'YOUR_FORGE_CLIENT_ID'<br>
     app_client_secret = 'YOUR_FORGE_CLIENT_SECRET'<br>
     access_token = Authenticate(forge_client_id=app_client_id, forge_client_secret=app_client_secret,authenticate_scopes='viewables:read')<br>
     return access_token
-</label>
+</p>
 <br>
 <br>
 
-<label>
+<p>
 Example 2  (To create Bucket): <br>
 def createBucket():<br>
     app_client_id = 'YOUR_FORGE_CLIENT_ID'<br>
     app_client_secret = 'YOUR_FORGE_CLIENT_SECRET'<br>
     BUCKET_KEY = 'YOUR_BUCKET_NAME'
     bucketCreation = CreateBucket(forge_client_id=app_client_id, forge_client_secret=app_client_secret,bucket_key=BUCKET_KEY)<br>
     return bucketCreation<br>
-</label>
+</p>
```

### Comparing `EasyForge-0.0.1/README.md` & `EasyForge-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 In this Package the following Forge API:<br>
 1.Data Management API<br>
 2.Authentication API <br>
 3.ModelDerivative API<br>
 </p>
 <p>The Following are sample examples.</p>
-<label>
+<p>
 Example 1 (To create Authenticate Token): <br>
 from forge.Authentication import Authenticate<br>
 def GenerateToken():<br>
     app_client_id = 'YOUR_FORGE_CLIENT_ID'<br>
     app_client_secret = 'YOUR_FORGE_CLIENT_SECRET'<br>
     access_token = Authenticate(forge_client_id=app_client_id, forge_client_secret=app_client_secret,authenticate_scopes='viewables:read')<br>
     return access_token
-</label>
+</p>
 <br>
 <br>
 
-<label>
+<p>
 Example 2  (To create Bucket): <br>
 def createBucket():<br>
     app_client_id = 'YOUR_FORGE_CLIENT_ID'<br>
     app_client_secret = 'YOUR_FORGE_CLIENT_SECRET'<br>
     BUCKET_KEY = 'YOUR_BUCKET_NAME'
     bucketCreation = CreateBucket(forge_client_id=app_client_id, forge_client_secret=app_client_secret,bucket_key=BUCKET_KEY)<br>
     return bucketCreation<br>
-</label>
+</p>
```

### Comparing `EasyForge-0.0.1/setup.py` & `EasyForge-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EasyForge",
-    version="0.0.1",
+    version="0.0.2",
     author="DKVG",
     author_email="gadellidk@gmail.com",
     description="To Make easy to use Forge (APS) by python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `EasyForge-0.0.1/src/EasyForge/Authentication.py` & `EasyForge-0.0.2/src/EasyForge/Authentication.py`

 * *Files identical despite different names*

### Comparing `EasyForge-0.0.1/src/EasyForge/DataManagement/ACC.py` & `EasyForge-0.0.2/src/EasyForge/DataManagement/ACC.py`

 * *Files identical despite different names*

### Comparing `EasyForge-0.0.1/src/EasyForge/DataManagement/OSS.py` & `EasyForge-0.0.2/src/EasyForge/DataManagement/OSS.py`

 * *Files identical despite different names*

### Comparing `EasyForge-0.0.1/src/EasyForge/DesignAutomation.py` & `EasyForge-0.0.2/src/EasyForge/DesignAutomation.py`

 * *Files identical despite different names*

### Comparing `EasyForge-0.0.1/src/EasyForge/ModelDerivative.py` & `EasyForge-0.0.2/src/EasyForge/ModelDerivative.py`

 * *Files identical despite different names*

### Comparing `EasyForge-0.0.1/src/EasyForge.egg-info/PKG-INFO` & `EasyForge-0.0.2/src/EasyForge.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyForge
-Version: 0.0.1
+Version: 0.0.2
 Summary: To Make easy to use Forge (APS) by python
 Author: DKVG
 Author-email: gadellidk@gmail.com
 Keywords: EasyForge forge APS forge-python python-aps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,28 +19,28 @@
 
 In this Package the following Forge API:<br>
 1.Data Management API<br>
 2.Authentication API <br>
 3.ModelDerivative API<br>
 </p>
 <p>The Following are sample examples.</p>
-<label>
+<p>
 Example 1 (To create Authenticate Token): <br>
 from forge.Authentication import Authenticate<br>
 def GenerateToken():<br>
     app_client_id = 'YOUR_FORGE_CLIENT_ID'<br>
     app_client_secret = 'YOUR_FORGE_CLIENT_SECRET'<br>
     access_token = Authenticate(forge_client_id=app_client_id, forge_client_secret=app_client_secret,authenticate_scopes='viewables:read')<br>
     return access_token
-</label>
+</p>
 <br>
 <br>
 
-<label>
+<p>
 Example 2  (To create Bucket): <br>
 def createBucket():<br>
     app_client_id = 'YOUR_FORGE_CLIENT_ID'<br>
     app_client_secret = 'YOUR_FORGE_CLIENT_SECRET'<br>
     BUCKET_KEY = 'YOUR_BUCKET_NAME'
     bucketCreation = CreateBucket(forge_client_id=app_client_id, forge_client_secret=app_client_secret,bucket_key=BUCKET_KEY)<br>
     return bucketCreation<br>
-</label>
+</p>
```

