# Comparing `tmp/py_auth_amqp_wrapper-0.0.3.tar.gz` & `tmp/py_auth_amqp_wrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_amqp_wrapper-0.0.3.tar", last modified: Mon Apr  3 15:08:37 2023, max compression
+gzip compressed data, was "py_auth_amqp_wrapper-0.0.5.tar", last modified: Mon May  8 12:34:51 2023, max compression
```

## Comparing `py_auth_amqp_wrapper-0.0.3.tar` & `py_auth_amqp_wrapper-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:08:37.011167 py_auth_amqp_wrapper-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-03 15:08:03.000000 py_auth_amqp_wrapper-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-03 15:08:37.011167 py_auth_amqp_wrapper-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-03 15:08:03.000000 py_auth_amqp_wrapper-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:08:37.011167 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-03 15:08:03.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-03 15:08:03.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-03 15:08:03.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/_getlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-03 15:08:03.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-03 15:08:03.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-03 15:08:03.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:08:37.011167 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-03 15:08:36.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-03 15:08:36.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 15:08:36.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-03 15:08:36.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-03 15:08:36.000000 py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-03 15:08:03.000000 py_auth_amqp_wrapper-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-03 15:08:37.011167 py_auth_amqp_wrapper-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_getlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 12:34:51.000000 py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 12:34:16.000000 py_auth_amqp_wrapper-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-08 12:34:51.174124 py_auth_amqp_wrapper-0.0.5/setup.cfg
```

### Comparing `py_auth_amqp_wrapper-0.0.3/LICENSE` & `py_auth_amqp_wrapper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.3/PKG-INFO` & `py_auth_amqp_wrapper-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_auth_amqp_wrapper
-Version: 0.0.3
+Version: 0.0.5
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_amqp_wrapper
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: AMQP
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/__main__.py` & `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,32 +6,35 @@
 from typing import Optional
 
 from ._version import __version__
 from ._load_config import load_config
 from ._runner import run
 
 
-
 def cli() -> Optional[str]:
     parser = argparse.ArgumentParser(
         prog="py_auth_amqp_wrapper",
         description="This will start an auth server based on py_auth_micro and connect it to an AMQP message Broker",
     )
-    parser.add_argument("--config","-c",help="path to the configuration file", default="./config.json",type=str)
-    parser.add_argument("--version","-v",help="displays the package version and quits",action="store_true")
-    parser.add_argument("--disable_existing_loggers","-d",help="disables existing loggers",action="store_true")
-    
+    parser.add_argument(
+        "--config", "-c", help="path to the configuration file", default="./config.json", type=str)
+    parser.add_argument(
+        "--version", "-v", help="displays the package version and quits", action="store_true")
+    parser.add_argument("--disable_existing_loggers", "-d",
+                        help="disables existing loggers", action="store_true")
+
     inputvars = parser.parse_args()
 
     if inputvars.version:
         print(f"py_auth_micro=={__version__}")
         return None
 
     return inputvars.config, inputvars.disable_existing_loggers
 
+
 if __name__ == "__main__":
     config, disable_existing_loggers = cli()
 
     if config is None:
         sys.exit(0)
 
         # configure DB
@@ -53,9 +56,8 @@
         config = load_config(config)
     except Exception as exc:
         print(exc)
         print("could not load config")
         sys.exit(78)
     print("loaded config")
     print("\n\nstarting up")
-    asyncio.run(run(**config,disable_existing_loggers=disable_existing_loggers))
-
+    asyncio.run(run(**config, disable_existing_loggers=disable_existing_loggers))
```

### Comparing `py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/_getlogger.py` & `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_getlogger.py`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/_load_config.py` & `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_load_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,27 +136,28 @@
             "DEBUG": logging.DEBUG,
             "INFO": logging.INFO,
             "WARNING": logging.WARNING,
             "ERROR": logging.ERROR,
             "CRITICAL": logging.CRITICAL,
         }
 
-        if log_settings.get("disable_aio_pika",False):
+        if log_settings.get("disable_aio_pika", False):
             pass
-            
-        if log_settings.get("disable_tortoise_orm",False):
+
+        if log_settings.get("disable_tortoise_orm", False):
             logging.getLogger("db_client").disabled = True
             logging.getLogger("tortoise").disabled = True
 
         level = LEVELMAP[log_settings.get("level", "INFO")]
         handler = log_settings.get("handler", None)
         handler_settings = log_settings.get("handler_settings", {})
 
         if handler_settings.get("amqp", None) is not None:
             amqp_settings = AMQPConfig(**handler_settings["amqp"])
-            handler_settings = {"amqp_config":amqp_settings}
+            handler_settings = {"amqp_config": amqp_settings}
+
+        config_dict["log_config"] = {
+            "log_level": level, "handler": handler, "handler_config": handler_settings}
 
-        config_dict["log_config"] = {"log_level":level,"handler":handler,"handler_config":handler_settings}
-    
     config_dict["queue_settings"] = default_queue_names
 
     return config_dict
```

### Comparing `py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper/_runner.py` & `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper/_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     logger = logging.getLogger("py_auth_amqp_wrapper")
     if log_config is not None:
         logger = getlogger(
             **log_config, disable_existing_loggers=disable_existing_loggers
         )
         logger.info("setup logger")
 
-    sessionwf = SessionWorkflow(ldap_config, jwt_encoder, jwt_validator, app_config)
+    sessionwf = SessionWorkflow(
+        ldap_config, jwt_encoder, jwt_validator, app_config)
     session_workflow_get_access_token = new_amqp_func(
         queue_settings["session_workflow_get_access_token"], sessionwf.get_access_token
     )
     session_workflow_login = new_amqp_func(
         queue_settings["session_workflow_login"], sessionwf.login
     )
     session_workflow_logout = new_amqp_func(
@@ -127,15 +128,15 @@
     @group_workflow_remove_user_from_group.exception_handler(Exception)
     @group_workflow_create_group.exception_handler(Exception)
     @group_workflow_delete_group.exception_handler(Exception)
     @session_workflow_logout.exception_handler(Exception)
     @session_workflow_login.exception_handler(Exception)
     @session_workflow_get_access_token.exception_handler(Exception)
     async def handle_exception(*args, exc: Exception, **kwargs):
-        logger.error(type(exc),exc)
+        logger.error(type(exc), exc)
         logger.error(str(kwargs))
         return {"resp_code": 500, "resp_data": {"msg": "something went wrong"}}
 
     service = await AMQPService().connect(amqp_config)
 
     await service.register_function(session_workflow_get_access_token)
     await service.register_function(session_workflow_login)
@@ -147,12 +148,10 @@
     await service.register_function(user_workflow_get_all)
     await service.register_function(user_workflow_get_user)
     await service.register_function(group_workflow_add_user_to_group)
     await service.register_function(group_workflow_remove_user_from_group)
     await service.register_function(group_workflow_create_group)
     await service.register_function(group_workflow_delete_group)
 
-    
-
     await service.serve()
 
     return
```

### Comparing `py_auth_amqp_wrapper-0.0.3/py_auth_amqp_wrapper.egg-info/PKG-INFO` & `py_auth_amqp_wrapper-0.0.5/py_auth_amqp_wrapper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-auth-amqp-wrapper
-Version: 0.0.3
+Version: 0.0.5
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_amqp_wrapper
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: AMQP
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_amqp_wrapper-0.0.3/setup.cfg` & `py_auth_amqp_wrapper-0.0.5/setup.cfg`

 * *Files identical despite different names*

