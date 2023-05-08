# Comparing `tmp/rispack-0.9.3.tar.gz` & `tmp/rispack-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rispack-0.9.3.tar", last modified: Sat Aug 20 11:57:37 2022, max compression
+gzip compressed data, was "rispack-0.9.4.tar", last modified: Sat Aug 20 12:10:55 2022, max compression
```

## Comparing `rispack-0.9.3.tar` & `rispack-0.9.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 11:57:37.845621 rispack-0.9.3/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2022-07-08 10:28:07.000000 rispack-0.9.3/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1144 2022-08-20 11:57:37.841621 rispack-0.9.3/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      537 2022-07-19 18:45:23.000000 rispack-0.9.3/README.md
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      693 2022-08-20 11:57:24.000000 rispack-0.9.3/pyproject.toml
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 11:57:37.837621 rispack-0.9.3/rispack/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       22 2022-08-20 11:57:24.000000 rispack-0.9.3/rispack/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      830 2022-08-15 21:22:06.000000 rispack-0.9.3/rispack/actions.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1115 2022-07-08 11:44:44.000000 rispack-0.9.3/rispack/aws.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2727 2022-08-03 13:11:06.000000 rispack-0.9.3/rispack/database.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      470 2022-08-15 20:19:30.000000 rispack-0.9.3/rispack/entities.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      393 2022-07-08 10:28:07.000000 rispack-0.9.3/rispack/entrypoint.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      293 2022-07-08 10:28:07.000000 rispack-0.9.3/rispack/errors.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2145 2022-07-08 23:55:13.000000 rispack-0.9.3/rispack/events.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 11:57:37.841621 rispack-0.9.3/rispack/handler/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      150 2022-07-08 10:28:07.000000 rispack-0.9.3/rispack/handler/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 11:57:37.841621 rispack-0.9.3/rispack/handler/interceptors/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       98 2022-08-03 13:11:06.000000 rispack-0.9.3/rispack/handler/interceptors/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1589 2022-08-20 11:57:24.000000 rispack-0.9.3/rispack/handler/interceptors/otp.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1286 2022-08-15 19:08:33.000000 rispack-0.9.3/rispack/handler/interceptors/pin.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      501 2022-07-12 16:30:02.000000 rispack-0.9.3/rispack/handler/interceptors/role.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      301 2022-07-08 10:28:07.000000 rispack-0.9.3/rispack/handler/job.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2029 2022-07-09 00:32:03.000000 rispack-0.9.3/rispack/handler/record.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1855 2022-07-12 16:30:02.000000 rispack-0.9.3/rispack/handler/request.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2088 2022-08-03 13:18:23.000000 rispack-0.9.3/rispack/handler/response.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2403 2022-08-03 13:11:06.000000 rispack-0.9.3/rispack/handler/route.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       60 2022-07-08 10:28:07.000000 rispack-0.9.3/rispack/logger.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      482 2022-07-12 16:30:02.000000 rispack-0.9.3/rispack/schemas.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1901 2022-08-20 11:57:24.000000 rispack-0.9.3/rispack/stores.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 11:57:37.841621 rispack-0.9.3/rispack.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1144 2022-08-20 11:57:37.000000 rispack-0.9.3/rispack.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      709 2022-08-20 11:57:37.000000 rispack-0.9.3/rispack.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2022-08-20 11:57:37.000000 rispack-0.9.3/rispack.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      124 2022-08-20 11:57:37.000000 rispack-0.9.3/rispack.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2022-08-20 11:57:37.000000 rispack-0.9.3/rispack.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2022-08-20 11:57:37.845621 rispack-0.9.3/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1148 2022-08-20 11:57:24.000000 rispack-0.9.3/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 12:10:55.345195 rispack-0.9.4/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2022-07-08 10:28:07.000000 rispack-0.9.4/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1144 2022-08-20 12:10:55.345195 rispack-0.9.4/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      537 2022-07-19 18:45:23.000000 rispack-0.9.4/README.md
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      693 2022-08-20 12:09:58.000000 rispack-0.9.4/pyproject.toml
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 12:10:55.341195 rispack-0.9.4/rispack/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       22 2022-08-20 12:09:50.000000 rispack-0.9.4/rispack/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      830 2022-08-15 21:22:06.000000 rispack-0.9.4/rispack/actions.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1115 2022-07-08 11:44:44.000000 rispack-0.9.4/rispack/aws.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2727 2022-08-03 13:11:06.000000 rispack-0.9.4/rispack/database.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      470 2022-08-15 20:19:30.000000 rispack-0.9.4/rispack/entities.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      393 2022-07-08 10:28:07.000000 rispack-0.9.4/rispack/entrypoint.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      293 2022-07-08 10:28:07.000000 rispack-0.9.4/rispack/errors.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2145 2022-07-08 23:55:13.000000 rispack-0.9.4/rispack/events.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 12:10:55.345195 rispack-0.9.4/rispack/handler/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      150 2022-07-08 10:28:07.000000 rispack-0.9.4/rispack/handler/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 12:10:55.345195 rispack-0.9.4/rispack/handler/interceptors/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       98 2022-08-03 13:11:06.000000 rispack-0.9.4/rispack/handler/interceptors/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1629 2022-08-20 12:09:43.000000 rispack-0.9.4/rispack/handler/interceptors/otp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1286 2022-08-15 19:08:33.000000 rispack-0.9.4/rispack/handler/interceptors/pin.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      501 2022-07-12 16:30:02.000000 rispack-0.9.4/rispack/handler/interceptors/role.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      301 2022-07-08 10:28:07.000000 rispack-0.9.4/rispack/handler/job.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2029 2022-07-09 00:32:03.000000 rispack-0.9.4/rispack/handler/record.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1855 2022-07-12 16:30:02.000000 rispack-0.9.4/rispack/handler/request.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2088 2022-08-03 13:18:23.000000 rispack-0.9.4/rispack/handler/response.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2403 2022-08-03 13:11:06.000000 rispack-0.9.4/rispack/handler/route.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       60 2022-07-08 10:28:07.000000 rispack-0.9.4/rispack/logger.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      482 2022-07-12 16:30:02.000000 rispack-0.9.4/rispack/schemas.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1901 2022-08-20 11:57:24.000000 rispack-0.9.4/rispack/stores.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-08-20 12:10:55.345195 rispack-0.9.4/rispack.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1144 2022-08-20 12:10:55.000000 rispack-0.9.4/rispack.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      709 2022-08-20 12:10:55.000000 rispack-0.9.4/rispack.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2022-08-20 12:10:55.000000 rispack-0.9.4/rispack.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      124 2022-08-20 12:10:55.000000 rispack-0.9.4/rispack.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2022-08-20 12:10:55.000000 rispack-0.9.4/rispack.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2022-08-20 12:10:55.345195 rispack-0.9.4/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1148 2022-08-20 12:09:54.000000 rispack-0.9.4/setup.py
```

### Comparing `rispack-0.9.3/LICENSE` & `rispack-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/PKG-INFO` & `rispack-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rispack
-Version: 0.9.3
+Version: 0.9.4
 Summary: Rispack - Pack of shared libraries from Rispar
 Home-page: https://github.com/risparfinance/rispack
 Author: Rispar
 Author-email: tecnologia@rispar.com.br
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rispack-0.9.3/README.md` & `rispack-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/pyproject.toml` & `rispack-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rispack"
-version = "0.9.3"
+version = "0.9.4"
 description = "Pack of shared libraries from Rispar"
 authors = ["Rispar <tecnologia@rispar.com.br>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 SQLAlchemy = "^1.4.36"
```

### Comparing `rispack-0.9.3/rispack/actions.py` & `rispack-0.9.4/rispack/actions.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack/aws.py` & `rispack-0.9.4/rispack/aws.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack/database.py` & `rispack-0.9.4/rispack/database.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack/events.py` & `rispack-0.9.4/rispack/events.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack/handler/interceptors/otp.py` & `rispack-0.9.4/rispack/handler/interceptors/otp.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,17 +39,18 @@
 
         payload = {"otp": otp, "profile_id": id}
 
 
         response = requests.post(self.endpoint, auth=get_signed_auth(), json=payload)
 
         logger.debug({
+            "endpoint": self.endpoint,
             "message": "debug otp interceptor",
             "payload": payload,
-            "reponse": response
+            "response": response
         })
 
         if response.status_code != HTTPStatus.OK:
             return Response.forbidden("Invalid OTP")
 
         return None
```

### Comparing `rispack-0.9.3/rispack/handler/interceptors/pin.py` & `rispack-0.9.4/rispack/handler/interceptors/pin.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack/handler/record.py` & `rispack-0.9.4/rispack/handler/record.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack/handler/request.py` & `rispack-0.9.4/rispack/handler/request.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack/handler/response.py` & `rispack-0.9.4/rispack/handler/response.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack/handler/route.py` & `rispack-0.9.4/rispack/handler/route.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack/stores.py` & `rispack-0.9.4/rispack/stores.py`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/rispack.egg-info/PKG-INFO` & `rispack-0.9.4/rispack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rispack
-Version: 0.9.3
+Version: 0.9.4
 Summary: Rispack - Pack of shared libraries from Rispar
 Home-page: https://github.com/risparfinance/rispack
 Author: Rispar
 Author-email: tecnologia@rispar.com.br
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rispack-0.9.3/rispack.egg-info/SOURCES.txt` & `rispack-0.9.4/rispack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rispack-0.9.3/setup.py` & `rispack-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 setuptools.setup(
     author="Rispar",
     author_email="tecnologia@rispar.com.br",
     url="https://github.com/risparfinance/rispack",
     name="rispack",
-    version="0.9.3",
+    version="0.9.4",
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     package_data={"rispack": ["LICENSE"]},
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Rispack - Pack of shared libraries from Rispar",
     license="Apache License 2.0",
```

