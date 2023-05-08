# Comparing `tmp/py_auth_micro-0.1.0.tar.gz` & `tmp/py_auth_micro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_micro-0.1.0.tar", last modified: Mon May  8 13:25:22 2023, max compression
+gzip compressed data, was "py_auth_micro-0.1.1.tar", last modified: Mon May  8 13:46:29 2023, max compression
```

## Comparing `py_auth_micro-0.1.0.tar` & `py_auth_micro-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.400186 py_auth_micro-0.1.0/py_auth_micro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/Config/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Config/_appconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Config/_dbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Config/_ldapconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Core/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Core/_ldap_interactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginbaseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginkerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginlocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/Models/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Models/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Models/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/Models/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_groupworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_sessionworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_userworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/py_auth_micro/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:25:22.400186 py_auth_micro-0.1.0/py_auth_micro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 13:25:22.000000 py_auth_micro-0.1.0/py_auth_micro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-08 13:25:22.404187 py_auth_micro-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 13:24:43.000000 py_auth_micro-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.544164 py_auth_micro-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:46:29.544164 py_auth_micro-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Config/_appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Config/_dbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Config/_ldapconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Core/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Core/_ldap_interactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginbaseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginkerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginlocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Models/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Models/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Models/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_groupworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_sessionworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_userworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-08 13:46:29.544164 py_auth_micro-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/setup.py
```

### Comparing `py_auth_micro-0.1.0/LICENSE` & `py_auth_micro-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/PKG-INFO` & `py_auth_micro-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_auth_micro
-Version: 0.1.0
+Version: 0.1.1
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.1.0/README.rst` & `py_auth_micro-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/Config/_appconfig.py` & `py_auth_micro-0.1.1/py_auth_micro/Config/_appconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/Config/_dbconfig.py` & `py_auth_micro-0.1.1/py_auth_micro/Config/_dbconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/Config/_ldapconfig.py` & `py_auth_micro-0.1.1/py_auth_micro/Config/_ldapconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/Core/_ldap_interactions.py` & `py_auth_micro-0.1.1/py_auth_micro/Core/_ldap_interactions.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/LoginHandler/__init__.py` & `py_auth_micro-0.1.1/py_auth_micro/LoginHandler/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginbaseclass.py` & `py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginbaseclass.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginldap.py` & `py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginldap.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/LoginHandler/_loginlocal.py` & `py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginlocal.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/Models/_token.py` & `py_auth_micro-0.1.1/py_auth_micro/Models/_token.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/Models/_user.py` & `py_auth_micro-0.1.1/py_auth_micro/Models/_user.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/__init__.py` & `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_groupworkflow.py` & `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_groupworkflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,36 +17,36 @@
         app_cfg (AppConfig): Some miscellaneous settings regarding the Application.
     """
 
     jwt_validator: JWTValidator
     app_cfg: AppConfig
 
     async def _perm_and_name_check(
-        self, *, access_token: str, group_name: str, **kwargs
+        self, *, access_token: str, groupname: str, **kwargs
     ) -> Optional[Group]:
         """Will check the Permissions of the access Token and if the group already exists.
 
         Args:
             access_token (str): Access Token of the Request Sender.
-            group_name (str): Name of the Group to check for
+            groupname (str): Name of the Group to check for
 
         Raises:
             PermissionError: User Requesting the Action is not and Administrator.
 
         Returns:
             Optional[Group]: If the Group exists return it. None if it does not exist.
         """
         _, is_admin = _get_info_from_token(
             self.jwt_validator, self.app_cfg, access_token
         )
 
         if not is_admin:
             raise PermissionError("Not Authorized")
 
-        group = await Group.get_or_none(name=group_name)
+        group = await Group.get_or_none(name=groupname)
 
         if group is None:
             return None
 
         return group
 
     async def get_groups(self, *, access_token: str, **kwargs) -> dict:
@@ -70,150 +70,156 @@
             status_code = 204
         else:
             status_code = 200
 
         return {"resp_code": status_code, "resp_data": {"groups": groups}}
 
     async def create_group(
-        self, *, access_token: str, group_name: str, **kwargs
+        self, *, access_token: str, groupname: str, **kwargs
     ) -> dict:
         """Creates a Group with the specified Name
 
         Args:
             access_token (str): Access-Token of the Requesting User.
-            group_name (str): Name of the Group to create.
+            groupname (str): Name of the Group to create.
 
         Raises:
             ValueError: Group already exists.
 
         Returns:
             dict: `resp_code` = 200 action was successfull, `resp_code` = 500 if it was not
         """
         # check groups Existence and Requesting Users Permission
         if (
             await self._perm_and_name_check(
-                access_token=access_token, group_name=group_name
+                access_token=access_token, groupname=groupname
             )
             is not None
         ):
             raise ValueError("Group already exist")
 
         try:
-            await Group.create(name=group_name)
+            await Group.create(name=groupname)
         except Exception:
             return {
                 "resp_code": 500,
-                "resp_data": {"msg": f"could not create group {group_name}"},
+                "resp_data": {"msg": f"could not create group {groupname}"},
             }
 
-        return {"resp_code": 200, "resp_data": {"msg": f"created group {group_name}"}}
+        return {"resp_code": 200, "resp_data": {"msg": f"created group {groupname}"}}
 
     async def delete_group(
-        self, *, access_token: str, group_name: str, **kwargs
+        self, *, access_token: str, groupname: str, **kwargs
     ) -> dict:
         """Deletes the specified Group.
 
         Args:
             access_token (str): Access-Token of the Requesting User.
-            group_name (str): Name of the Group to delete.
+            groupname (str): Name of the Group to delete.
 
         Raises:
             ValueError: Group does not exist
 
         Returns:
             dict: `resp_code` = 200 action was successfull, `resp_code` = 500 if it was not
         """
         # check groups Existence and Requesting Users Permission
-        group = await self._perm_and_name_check(access_token, group_name)
+        group = await self._perm_and_name_check(
+            access_token=access_token, groupname=groupname
+        )
 
         if group is None:
             raise ValueError("Group does not exist")
 
         try:
             await group.delete()
         except Exception:
             return {
                 "resp_code": 500,
-                "resp_data": {"msg": f"could not delete group {group_name}"},
+                "resp_data": {"msg": f"could not delete group {groupname}"},
             }
 
-        return {"resp_code": 200, "resp_data": {"msg": f"deleted group {group_name}"}}
+        return {"resp_code": 200, "resp_data": {"msg": f"deleted group {groupname}"}}
 
     async def add_user_to_group(
-        self, *, access_token: str, group_name: str, user_name: str, **kwargs
+        self, *, access_token: str, groupname: str, username: str, **kwargs
     ) -> dict:
         """Adds a User to a group
 
         Args:
             access_token (str): Access Token of the Requesting User.
-            group_name (str): Name of the Group to add the User to.
-            user_name (str): Name of the User to add to the Group.
+            groupname (str): Name of the Group to add the User to.
+            username (str): Name of the User to add to the Group.
 
         Raises:
             ValueError: Group does not exist.
 
         Returns:
             dict: `resp_code` = 200 action was successfull, `resp_code` = 500 if it was not
         """
 
         # check groups Existence and Requesting Users Permission
-        group = await self._perm_and_name_check(access_token, group_name)
+        group = await self._perm_and_name_check(
+            access_token=access_token, groupname=groupname
+        )
 
         if group is None:
             raise ValueError("Group does not exist")
 
-        user = await User.get(username=user_name)
+        user = await User.get(username=username)
 
         try:
             await group.users.add(user)
         except Exception:
             return {
                 "resp_code": 500,
                 "resp_data": {
-                    "msg": f"could not add user {user_name} to group {group_name}"
+                    "msg": f"could not add user {username} to group {groupname}"
                 },
             }
 
         return {
             "resp_code": 200,
-            "resp_data": {"msg": f"added user {user_name} to group {group_name}"},
+            "resp_data": {"msg": f"added user {username} to group {groupname}"},
         }
 
     async def remove_user_from_group(
-        self, *, access_token: str, group_name: str, user_name: str, **kwargs
+        self, *, access_token: str, groupname: str, username: str, **kwargs
     ) -> dict:
         """Removes a User from a group
 
         Args:
             access_token (str): Access Token of the Requesting User.
-            group_name (str): Name of the Group to remove the User from.
-            user_name (str): Name of the User to remove the Group.
+            groupname (str): Name of the Group to remove the User from.
+            username (str): Name of the User to remove the Group.
 
         Raises:
             ValueError: Group does not exist.
 
         Returns:
             dict: `resp_code` = 200 action was successfull, `resp_code` = 500 if it was not
         """
 
         # check groups Existence and Requesting Users Permission
-        group = await self._perm_and_name_check(access_token, group_name)
+        group = await self._perm_and_name_check(
+            access_token=access_token, groupname=groupname
+        )
 
         if group is None:
             raise ValueError("Group does not exist")
 
-        user = await User.get(username=user_name)
+        user = await User.get(username=username)
 
         try:
             await group.users.remove(user)
         except Exception:
             return {
                 "resp_code": 500,
                 "resp_data": {
-                    "msg": f"could not remove user {user_name} to group {group_name}"
+                    "msg": f"could not remove user {username} to group {groupname}"
                 },
             }
 
         return {
             "resp_code": 200,
-            "resp_data": {"msg": f"removed user {user_name} to group {group_name}"},
+            "resp_data": {"msg": f"removed user {username} to group {groupname}"},
         }
```

### Comparing `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_misc.py` & `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_misc.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_sessionworkflow.py` & `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_sessionworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro/WorkFlows/_userworkflow.py` & `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_userworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/py_auth_micro.egg-info/PKG-INFO` & `py_auth_micro-0.1.1/py_auth_micro.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-auth-micro
-Version: 0.1.0
+Version: 0.1.1
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.1.0/py_auth_micro.egg-info/SOURCES.txt` & `py_auth_micro-0.1.1/py_auth_micro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.0/setup.cfg` & `py_auth_micro-0.1.1/setup.cfg`

 * *Files identical despite different names*

