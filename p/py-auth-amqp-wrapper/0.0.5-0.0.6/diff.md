# Comparing `tmp/py_auth_amqp_wrapper-0.0.5.tar.gz` & `tmp/py_auth_amqp_wrapper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_amqp_wrapper-0.0.5.tar", last modified: Mon May  8 12:34:51 2023, max compression
+gzip compressed data, was "py_auth_amqp_wrapper-0.0.6.tar", last modified: Mon May  8 12:52:44 2023, max compression
```

## Comparing `py_auth_amqp_wrapper-0.0.5.tar` & `py_auth_amqp_wrapper-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_getlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_getlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/setup.cfg
```

### Comparing `py_auth_amqp_wrapper-0.0.5/LICENSE` & `py_auth_amqp_wrapper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.5/PKG-INFO` & `py_auth_amqp_wrapper-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_auth_amqp_wrapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_amqp_wrapper
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: AMQP
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/__main__.py` & `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_getlogger.py` & `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_getlogger.py`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_load_config.py` & `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_load_config.py`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_runner.py` & `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import asyncio
 import logging
+import traceback
 
 from tortoise import Tortoise
-from aio_pika import connect_robust
-from aio_pika.patterns import JsonRPC
 
 from jwt_helper import JWTEncoder, JWTValidator
 from amqp_helper import AMQPConfig, AMQPService, new_amqp_func
 from py_auth_micro.Config import DBConfig, AppConfig, LDAPConfig
 from py_auth_micro.WorkFlows import SessionWorkflow, UserWorkflow, GroupWorkflow
 
 from ._getlogger import getlogger
@@ -53,16 +51,15 @@
     logger = logging.getLogger("py_auth_amqp_wrapper")
     if log_config is not None:
         logger = getlogger(
             **log_config, disable_existing_loggers=disable_existing_loggers
         )
         logger.info("setup logger")
 
-    sessionwf = SessionWorkflow(
-        ldap_config, jwt_encoder, jwt_validator, app_config)
+    sessionwf = SessionWorkflow(ldap_config, jwt_encoder, jwt_validator, app_config)
     session_workflow_get_access_token = new_amqp_func(
         queue_settings["session_workflow_get_access_token"], sessionwf.get_access_token
     )
     session_workflow_login = new_amqp_func(
         queue_settings["session_workflow_login"], sessionwf.login
     )
     session_workflow_logout = new_amqp_func(
@@ -104,22 +101,20 @@
         queue_settings["group_workflow_delete_group"], groupwf.delete_group
     )
 
     @session_workflow_logout.exception_handler(TypeError)
     @session_workflow_login.exception_handler(TypeError)
     @session_workflow_get_access_token.exception_handler(TypeError)
     async def handle_exception(*args, exc: Exception, **kwargs):
-        print(type(exc), exc)
-        print(args)
-        print(kwargs)
+        logger.exception(exc, kwargs)
         return {"resp_code": 400, "resp_data": {"msg": "Invalid Data"}}
 
     @session_workflow_login.exception_handler(ValueError, PermissionError)
     async def handle_login_fail(*args, exc: Exception, **kwargs):
-        print(type(exc), exc)
+        logger.exception(exc, kwargs)
         return {"resp_code": 401, "resp_data": {"msg": "Could not login"}}
 
     @user_workflow_admin_create_user.exception_handler(Exception)
     @user_workflow_register_user.exception_handler(Exception)
     @user_workflow_delete_user.exception_handler(Exception)
     @user_workflow_change_user.exception_handler(Exception)
     @user_workflow_get_all.exception_handler(Exception)
@@ -128,17 +123,16 @@
     @group_workflow_remove_user_from_group.exception_handler(Exception)
     @group_workflow_create_group.exception_handler(Exception)
     @group_workflow_delete_group.exception_handler(Exception)
     @session_workflow_logout.exception_handler(Exception)
     @session_workflow_login.exception_handler(Exception)
     @session_workflow_get_access_token.exception_handler(Exception)
     async def handle_exception(*args, exc: Exception, **kwargs):
-        logger.error(type(exc), exc)
-        logger.error(str(kwargs))
-        return {"resp_code": 500, "resp_data": {"msg": "something went wrong"}}
+        logger.exception(exc, kwargs)
+        return {"resp_code": 500, "resp_data": {"msg": f"something went wrong! {exc}"}}
 
     service = await AMQPService().connect(amqp_config)
 
     await service.register_function(session_workflow_get_access_token)
     await service.register_function(session_workflow_login)
     await service.register_function(session_workflow_logout)
     await service.register_function(user_workflow_admin_create_user)
```

### Comparing `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/PKG-INFO` & `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-auth-amqp-wrapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_amqp_wrapper
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: AMQP
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_amqp_wrapper-0.0.5/setup.cfg` & `py_auth_amqp_wrapper-0.0.6/setup.cfg`

 * *Files identical despite different names*

