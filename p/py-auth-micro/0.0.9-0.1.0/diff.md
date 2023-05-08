# Comparing `tmp/py_auth_micro-0.0.9.tar.gz` & `tmp/py_auth_micro-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_micro-0.0.9.tar", last modified: Mon May  8 13:18:26 2023, max compression
+gzip compressed data, was "py_auth_micro-0.1.0.tar", last modified: Mon May  8 13:25:22 2023, max compression
```

## Comparing `py_auth_micro-0.0.9.tar` & `py_auth_micro-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.854654 py_auth_micro-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:18:26.854654 py_auth_micro-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/Config/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Config/_appconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Config/_dbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Config/_ldapconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Core/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Core/_ldap_interactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginbaseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginkerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginlocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/Models/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Models/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Models/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/Models/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_groupworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_sessionworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_userworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/py_auth_micro/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:18:26.850654 py_auth_micro-0.0.9/py_auth_micro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 13:18:26.000000 py_auth_micro-0.0.9/py_auth_micro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-08 13:18:26.854654 py_auth_micro-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 13:17:41.000000 py_auth_micro-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.400186 py_auth_micro-0.1.0/py_auth_micro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Config/_appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Config/_dbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Config/_ldapconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Core/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Core/_ldap_interactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginbaseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginkerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginlocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Models/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Models/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Models/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_groupworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_sessionworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_userworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.400186 py_auth_micro-0.1.0/py_auth_micro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/setup.py
```

### Comparing `py_auth_micro-0.0.9/LICENSE` & `py_auth_micro-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/PKG-INFO` & `py_auth_micro-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_auth_micro
-Version: 0.0.9
+Version: 0.1.0
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.0.9/README.rst` & `py_auth_micro-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/Config/_appconfig.py` & `py_auth_micro-0.1.0/py_auth_micro/Config/_appconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/Config/_dbconfig.py` & `py_auth_micro-0.1.0/py_auth_micro/Config/_dbconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/Config/_ldapconfig.py` & `py_auth_micro-0.1.0/py_auth_micro/Config/_ldapconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/Core/_ldap_interactions.py` & `py_auth_micro-0.1.0/py_auth_micro/Core/_ldap_interactions.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/LoginHandler/__init__.py` & `py_auth_micro-0.1.0/py_auth_micro/LoginHandler/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginbaseclass.py` & `py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginbaseclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from abc import ABC, abstractmethod
 
-from ..Models import User
-
 
 class LoginBaseClass(ABC):
     """Abstract Baseclass for Authenticating Users
 
     This Is an abstract baseclass describing all functions needed to be implemented by a generic LoginHandler.
     """
```

### Comparing `py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginldap.py` & `py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginldap.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/LoginHandler/_loginlocal.py` & `py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginlocal.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/Models/_token.py` & `py_auth_micro-0.1.0/py_auth_micro/Models/_token.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/Models/_user.py` & `py_auth_micro-0.1.0/py_auth_micro/Models/_user.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/__init__.py` & `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_groupworkflow.py` & `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_groupworkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,20 @@
         Raises:
             ValueError: Group already exists.
 
         Returns:
             dict: `resp_code` = 200 action was successfull, `resp_code` = 500 if it was not
         """
         # check groups Existence and Requesting Users Permission
-        if await self._perm_and_name_check(access_token, group_name) is not None:
+        if (
+            await self._perm_and_name_check(
+                access_token=access_token, group_name=group_name
+            )
+            is not None
+        ):
             raise ValueError("Group already exist")
 
         try:
             await Group.create(name=group_name)
         except Exception:
             return {
                 "resp_code": 500,
```

### Comparing `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_misc.py` & `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from jwt_helper import JWTValidator
 
 from ..Config import AppConfig
 
-def _get_info_from_token(jwt_validator:JWTValidator,app_cfg:AppConfig, access_token: str) -> tuple[str, bool]:
+
+def _get_info_from_token(
+    jwt_validator: JWTValidator, app_cfg: AppConfig, access_token: str
+) -> tuple[str, bool]:
     """This Function gets Information from an Access-Token.
 
     It will Return a Tuple with the username and if he is an administrator.
 
     Args:
         jwt_validator (JWTValidator): JWTValidator used to verify the Access Token.
         app_cfg (AppConfig): AppConfig containing the Admin Group name.
         access_token (str): The Access Token to validate.
     Raises:
         ValueError: The Token could not be verified.
 
     Returns:
         tuple[str, bool]: username, is_admin
     """
-        
+
     jwt_content = jwt_validator.get_jwt_as_dict(access_token)
 
     header: dict = jwt_content["headers"]
     user = jwt_content["payload"]["user"]
 
     is_admin = app_cfg.admin_group in header.get("aud", None)
 
-    return user, is_admin
+    return user, is_admin
```

### Comparing `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_sessionworkflow.py` & `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_sessionworkflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         Returns:
             dict: `resp_data` contains the id_token
         """
 
         if vhost is None:
             vhost = self.app_cfg.default_vhost
-            
+
         user: User = await login(username, password, self.ldap_cfg)
         token_obj = await user.create_id_token(
             self.jwt_encoder, self.app_cfg, vhost, ip
         )
         return {
             "resp_code": 200,
             "resp_data": {
```

### Comparing `py_auth_micro-0.0.9/py_auth_micro/WorkFlows/_userworkflow.py` & `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_userworkflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import bcrypt
 import re
 
 from dataclasses import dataclass
 from tortoise.exceptions import DoesNotExist
-from jwt_helper import JWTEncoder, JWTValidator
+from jwt_helper import JWTValidator
 from typing import Optional
 
 from ..Models import User
 from ..Exceptions import AlreadyExists
 from ..Config import AppConfig
 from ..Core import AuthSource
```

### Comparing `py_auth_micro-0.0.9/py_auth_micro.egg-info/PKG-INFO` & `py_auth_micro-0.1.0/py_auth_micro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-auth-micro
-Version: 0.0.9
+Version: 0.1.0
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.0.9/py_auth_micro.egg-info/SOURCES.txt` & `py_auth_micro-0.1.0/py_auth_micro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.0.9/setup.cfg` & `py_auth_micro-0.1.0/setup.cfg`

 * *Files identical despite different names*

