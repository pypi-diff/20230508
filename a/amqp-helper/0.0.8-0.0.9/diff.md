# Comparing `tmp/amqp_helper-0.0.8.tar.gz` & `tmp/amqp_helper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp_helper-0.0.8.tar", last modified: Thu Nov 10 13:45:01 2022, max compression
+gzip compressed data, was "amqp_helper-0.0.9.tar", last modified: Wed Mar  1 14:47:35 2023, max compression
```

## Comparing `amqp_helper-0.0.8.tar` & `amqp_helper-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:45:01.896455 amqp_helper-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-10 13:44:12.000000 amqp_helper-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-11-10 13:45:01.896455 amqp_helper-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-11-10 13:44:12.000000 amqp_helper-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:45:01.892455 amqp_helper-0.0.8/amqp_helper/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-11-10 13:44:12.000000 amqp_helper-0.0.8/amqp_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-11-10 13:44:12.000000 amqp_helper-0.0.8/amqp_helper/_amqpconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     3974 2022-11-10 13:44:12.000000 amqp_helper-0.0.8/amqp_helper/_amqploghandler.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-10 13:44:12.000000 amqp_helper-0.0.8/amqp_helper/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:45:01.896455 amqp_helper-0.0.8/amqp_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-11-10 13:45:01.000000 amqp_helper-0.0.8/amqp_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-10 13:45:01.000000 amqp_helper-0.0.8/amqp_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 13:45:01.000000 amqp_helper-0.0.8/amqp_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-10 13:45:01.000000 amqp_helper-0.0.8/amqp_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-10 13:45:01.000000 amqp_helper-0.0.8/amqp_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-11-10 13:45:01.896455 amqp_helper-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-11-10 13:44:12.000000 amqp_helper-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:47:35.688901 amqp_helper-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-01 14:47:35.688901 amqp_helper-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:47:35.688901 amqp_helper-0.0.9/amqp_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/amqp_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/amqp_helper/_amqpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/amqp_helper/_amqpconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/amqp_helper/_amqpfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/amqp_helper/_amqploghandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/amqp_helper/_amqpservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/amqp_helper/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:47:35.688901 amqp_helper-0.0.9/amqp_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-01 14:47:35.000000 amqp_helper-0.0.9/amqp_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-01 14:47:35.000000 amqp_helper-0.0.9/amqp_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:47:35.000000 amqp_helper-0.0.9/amqp_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-01 14:47:35.000000 amqp_helper-0.0.9/amqp_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-01 14:47:35.000000 amqp_helper-0.0.9/amqp_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-01 14:47:35.688901 amqp_helper-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-01 14:47:00.000000 amqp_helper-0.0.9/setup.py
```

### Comparing `amqp_helper-0.0.8/LICENSE` & `amqp_helper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp_helper-0.0.8/README.rst` & `amqp_helper-0.0.9/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -44,8 +44,75 @@
     async def main():
 
         connection = await connect_robust(**amqp_config.aio_pika())
 
         # do some amqp stuff
 
     if __name__ == "__main__":
+        asyncio.run(main())
+
+Example RPC over AMQP
+======================
+
+Server code
+------------
+The Server code is quite simple
+
+.. code-block:: python
+
+    import asyncio
+    from amqp_helper import AMQPConfig, AMQPService, new_amqp_func
+
+    amqp_config = AMQPConfig(username="test",password="testpw",vhost="testvhost")
+
+    async def testfunc(throw_value_error = False,throw_key_error = False, throw_exception = False*args, **kwargs):
+        if throw_value_error:
+            raise ValueError()
+        if throw_key_error:
+            raise KeyError()
+        if throw_exception:
+            raise Exception()
+
+        return {"result": "sync stuff"}
+
+    rpc_fun = new_amqp_func("test1", test1234)
+
+
+    @rpc_fun.exception_handler(ValueError, KeyError)
+    async def handle_value_error(*args, **kwargs):
+        retrun "got ValueError or KeyError"
+
+    @rpc_fun.exception_handler(Exception)
+    async def handle_value_error(*args, **kwargs):
+        return "got Exception"
+
+    async def main():
+
+        service = await AMQPService().connect(amqp_config)
+        await service.register_function(rpc_fun)
+
+        await service.serve()
+
+        # do some amqp stuff
+
+    if __name__ == "__main__":
+        asyncio.run(main())
+
+
+Client
+------------
+
+.. code-block:: python
+
+    import asyncio
+    from amqp_helper import AMQPConfig, AMQPClient
+
+    amqp_config = AMQPConfig(username="test",password="testpw",vhost="testvhost")
+
+    async def main():
+
+        client = await AMQPClient().connect(amqp_config)
+
+        print(await client.call(None,"test1"))
+
+    if __name__ == "__main__":
         asyncio.run(main())
```

### Comparing `amqp_helper-0.0.8/amqp_helper/_amqpconfig.py` & `amqp_helper-0.0.9/amqp_helper/_amqpconfig.py`

 * *Files identical despite different names*

### Comparing `amqp_helper-0.0.8/amqp_helper/_amqploghandler.py` & `amqp_helper-0.0.9/amqp_helper/_amqploghandler.py`

 * *Files identical despite different names*

### Comparing `amqp_helper-0.0.8/setup.cfg` & `amqp_helper-0.0.9/setup.cfg`

 * *Files identical despite different names*

