# Comparing `tmp/py_auth_micro-0.0.8.tar.gz` & `tmp/py_auth_micro-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_micro-0.0.8.tar", last modified: Wed Apr  5 09:22:49 2023, max compression
+gzip compressed data, was "py_auth_micro-0.0.9.tar", last modified: Mon May  8 13:18:26 2023, max compression
```

## Comparing `py_auth_micro-0.0.8.tar` & `py_auth_micro-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:22:49.840618 py_auth_micro-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-05 09:22:49.840618 py_auth_micro-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:22:49.836618 py_auth_micro-0.0.8/py_auth_micro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:22:49.836618 py_auth_micro-0.0.8/py_auth_micro/Config/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Config/_appconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Config/_dbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Config/_ldapconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:22:49.836618 py_auth_micro-0.0.8/py_auth_micro/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Core/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Core/_ldap_interactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:22:49.836618 py_auth_micro-0.0.8/py_auth_micro/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:22:49.836618 py_auth_micro-0.0.8/py_auth_micro/LoginHandler/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/LoginHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/LoginHandler/_loginbaseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/LoginHandler/_loginkerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/LoginHandler/_loginldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/LoginHandler/_loginlocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:22:49.836618 py_auth_micro-0.0.8/py_auth_micro/Models/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Models/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Models/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/Models/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:22:49.840618 py_auth_micro-0.0.8/py_auth_micro/WorkFlows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/WorkFlows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/WorkFlows/_groupworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/WorkFlows/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/WorkFlows/_sessionworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/WorkFlows/_userworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/py_auth_micro/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:22:49.836618 py_auth_micro-0.0.8/py_auth_micro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-05 09:22:49.000000 py_auth_micro-0.0.8/py_auth_micro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-05 09:22:49.000000 py_auth_micro-0.0.8/py_auth_micro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:22:49.000000 py_auth_micro-0.0.8/py_auth_micro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-05 09:22:49.000000 py_auth_micro-0.0.8/py_auth_micro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-05 09:22:49.000000 py_auth_micro-0.0.8/py_auth_micro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-05 09:22:49.840618 py_auth_micro-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-05 09:22:00.000000 py_auth_micro-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.854654 py_auth_micro-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:18:26.854654 py_auth_micro-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Config/_appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Config/_dbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Config/_ldapconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Core/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Core/_ldap_interactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginbaseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginkerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginlocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Models/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Models/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Models/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_groupworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_sessionworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_userworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-08 13:18:26.854654 py_auth_micro-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/setup.py
```

### Comparing `py_auth_micro-0.0.8/LICENSE` & `py_auth_micro-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/PKG-INFO` & `py_auth_micro-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_auth_micro
-Version: 0.0.8
+Version: 0.0.9
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.0.8/README.rst` & `py_auth_micro-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/Config/_appconfig.py` & `py_auth_micro-0.0.9/py_auth_micro/Config/_appconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/Config/_dbconfig.py` & `py_auth_micro-0.0.9/py_auth_micro/Config/_dbconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/Config/_ldapconfig.py` & `py_auth_micro-0.0.9/py_auth_micro/Config/_ldapconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/Core/_ldap_interactions.py` & `py_auth_micro-0.0.9/py_auth_micro/Core/_ldap_interactions.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/LoginHandler/__init__.py` & `py_auth_micro-0.0.9/py_auth_micro/LoginHandler/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/LoginHandler/_loginbaseclass.py` & `py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginbaseclass.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/LoginHandler/_loginldap.py` & `py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginldap.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/LoginHandler/_loginlocal.py` & `py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginlocal.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/Models/_token.py` & `py_auth_micro-0.0.9/py_auth_micro/Models/_token.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/Models/_user.py` & `py_auth_micro-0.0.9/py_auth_micro/Models/_user.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/WorkFlows/__init__.py` & `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/WorkFlows/_groupworkflow.py` & `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_groupworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/WorkFlows/_misc.py` & `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_misc.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/WorkFlows/_sessionworkflow.py` & `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_sessionworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/py_auth_micro/WorkFlows/_userworkflow.py` & `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_userworkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,18 @@
             dict: `resp_code` 200 if operation was successfull
         """
 
         if password != password_confirm:
             raise ValueError("passwords do not match")
 
         user_created = await self._create_user(
-            username, password, email, self.app_cfg.auto_activate_accounts
+            username=username,
+            password=password,
+            email=email,
+            activated=self.app_cfg.auto_activate_accounts,
         )
 
         if user_created:
             return {"resp_code": 201, "resp_data": {"msg": f"created user {username}"}}
 
         return {
             "resp_code": 400,
@@ -219,15 +222,17 @@
         _, is_admin = _get_info_from_token(
             self.jwt_validator, self.app_cfg, access_token
         )
 
         if not is_admin:
             raise PermissionError("Missing Permissions")
 
-        created = await self._create_user(username, password, email, True)
+        created = await self._create_user(
+            username=username, password=password, email=email, activated=True
+        )
 
         if created:
             return {"resp_code": 201, "resp_data": {"msg": f"created user {username}"}}
 
         return {
             "resp_code": 400,
             "resp_data": {"msg": f"could not create user {username}"},
```

### Comparing `py_auth_micro-0.0.8/py_auth_micro.egg-info/PKG-INFO` & `py_auth_micro-0.0.9/py_auth_micro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-auth-micro
-Version: 0.0.8
+Version: 0.0.9
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.0.8/py_auth_micro.egg-info/SOURCES.txt` & `py_auth_micro-0.0.9/py_auth_micro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.8/setup.cfg` & `py_auth_micro-0.0.9/setup.cfg`

 * *Files identical despite different names*

