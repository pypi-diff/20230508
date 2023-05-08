# Comparing `tmp/taichu-serve-2.0.25.tar.gz` & `tmp/taichu-serve-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taichu-serve-2.0.25.tar", last modified: Mon May  8 10:23:35 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.9.tar", last modified: Wed Apr 19 02:34:49 2023, max compression
```

## Comparing `taichu-serve-2.0.25.tar` & `taichu-serve-2.0.9.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/
--rw-r--r--   0 caiyueliang   (501) staff       (20)      236 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/PKG-INFO
--rw-r--r--   0 caiyueliang   (501) staff       (20)     7397 2023-04-27 09:53:59.000000 taichu-serve-2.0.25/README.md
--rw-r--r--   0 caiyueliang   (501) staff       (20)       38 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/setup.cfg
--rw-r--r--   0 caiyueliang   (501) staff       (20)     1235 2023-05-08 10:18:24.000000 taichu-serve-2.0.25/setup.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve/
--rw-r--r--   0 caiyueliang   (501) staff       (20)     4130 2023-05-06 08:06:22.000000 taichu-serve-2.0.25/taichu_serve/__init__.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)    12994 2023-05-08 03:46:33.000000 taichu-serve-2.0.25/taichu_serve/app.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     8721 2023-05-08 06:16:05.000000 taichu-serve-2.0.25/taichu_serve/command.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      889 2023-04-25 06:18:51.000000 taichu-serve-2.0.25/taichu_serve/common.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     6712 2023-05-08 09:21:06.000000 taichu-serve-2.0.25/taichu_serve/dockerfile.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     1521 2023-04-23 10:26:19.000000 taichu-serve-2.0.25/taichu_serve/error_code.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     6336 2023-04-23 10:26:19.000000 taichu-serve-2.0.25/taichu_serve/grpc_predict_v2_pb2.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)    13010 2023-04-23 10:26:19.000000 taichu-serve-2.0.25/taichu_serve/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     6812 2023-05-08 10:03:05.000000 taichu-serve-2.0.25/taichu_serve/grpc_server.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     2316 2023-05-06 02:54:53.000000 taichu-serve-2.0.25/taichu_serve/log.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     5471 2023-05-06 08:06:22.000000 taichu-serve-2.0.25/taichu_serve/model_server.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      205 2023-04-23 10:26:19.000000 taichu-serve-2.0.25/taichu_serve/ratelimiter.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     3351 2023-05-06 08:17:59.000000 taichu-serve-2.0.25/taichu_serve/settings.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve/template/
--rw-r--r--   0 caiyueliang   (501) staff       (20)        0 2023-04-23 10:26:19.000000 taichu-serve-2.0.25/taichu_serve/template/__init__.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      848 2023-04-24 08:19:39.000000 taichu-serve-2.0.25/taichu_serve/template/model_service.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve/template/test/
--rw-r--r--   0 caiyueliang   (501) staff       (20)        0 2023-04-23 10:26:19.000000 taichu-serve-2.0.25/taichu_serve/template/test/__init__.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      691 2023-04-23 10:26:19.000000 taichu-serve-2.0.25/taichu_serve/template/test/grpc_client.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      286 2023-04-23 10:26:19.000000 taichu-serve-2.0.25/taichu_serve/template/test/http_client.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      932 2023-04-23 10:26:19.000000 taichu-serve-2.0.25/taichu_serve/template/test/stream_grpc_client.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve/third/
--rw-r--r--   0 caiyueliang   (501) staff       (20)        0 2023-05-08 01:45:25.000000 taichu-serve-2.0.25/taichu_serve/third/__init__.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     2676 2023-05-08 06:16:05.000000 taichu-serve-2.0.25/taichu_serve/third/tracer.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve.egg-info/
--rw-r--r--   0 caiyueliang   (501) staff       (20)      236 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 caiyueliang   (501) staff       (20)      894 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 caiyueliang   (501) staff       (20)        1 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 caiyueliang   (501) staff       (20)       58 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 caiyueliang   (501) staff       (20)      188 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 caiyueliang   (501) staff       (20)       13 2023-05-08 10:23:35.000000 taichu-serve-2.0.25/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.797402 taichu-serve-2.0.9/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:34:49.797253 taichu-serve-2.0.9/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-19 02:34:49.797443 taichu-serve-2.0.9/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      947 2023-04-19 02:34:18.000000 taichu-serve-2.0.9/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.793674 taichu-serve-2.0.9/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.9/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.9/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     5479 2023-04-19 02:05:09.000000 taichu-serve-2.0.9/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      934 2023-04-18 09:03:28.000000 taichu-serve-2.0.9/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     2118 2023-04-19 02:34:18.000000 taichu-serve-2.0.9/taichu_serve/dockerfile.py
+-rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.9/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.9/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.9/taichu_serve/log.py
+-rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.9/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.9/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     2253 2023-04-19 01:27:54.000000 taichu-serve-2.0.9/taichu_serve/settings.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.795889 taichu-serve-2.0.9/taichu_serve/template/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.9/taichu_serve/template/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      123 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/config.ini
+-rw-r--r--   0 chen       (501) staff       (20)      741 2023-04-18 03:02:30.000000 taichu-serve-2.0.9/taichu_serve/template/customize_service.py
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 03:02:30.000000 taichu-serve-2.0.9/taichu_serve/template/requirements.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.796946 taichu-serve-2.0.9/taichu_serve/template/test/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.9/taichu_serve/template/test/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      690 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/test/grpc_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      285 2023-04-18 08:45:26.000000 taichu-serve-2.0.9/taichu_serve/template/test/http_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      931 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/test/stream_grpc_client.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.794937 taichu-serve-2.0.9/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      900 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `taichu-serve-2.0.25/taichu_serve/__init__.py` & `taichu-serve-2.0.9/taichu_serve/model_server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,148 +1,204 @@
-__version__ = "1.0.4"
+"""`ModelService` defines an API for base model service.
+"""
+from __future__ import print_function
 
-import time
 import logging
-import typing
-
+import os
+import sys
+import traceback
 from abc import ABCMeta, abstractmethod
-from taichu_serve.model_server import BaseModelService
+import time
 
 logger = logging.getLogger(__name__)
 
 
-class ModelServer(BaseModelService):
-    '''SingleNodeModel defines abstraction for model service which loads a
-    single model.
+class BaseModelService(object):
+    '''ModelService wraps up all preprocessing, inference and postprocessing
+    functions used by model service. It is defined in a flexible manner to
+    be easily extended to support different frameworks.
     '''
+    __metaclass__ = ABCMeta
 
     def __init__(self, model_path):
-        super(ModelServer, self).__init__(model_path)
-        self._ready = False
-        self._ctx = {}
-
-    def warmup(self):
-        start_time = time.time()
-        self._warmup()
-        self._ready = True
-        logger.info('warmup time: ' + str((time.time() - start_time) * 1000) + 'ms')
-
-    def inference(self, data, request_id, stream=False):
-        """
-        Wrapper function to run preprocess, inference and postprocess functions.
-        """
-        logger.info('recv request: ' + request_id)
-
-        context = self._ctx.get(request_id)
-        if context is None:
-            context = {}
-            if stream:
-                logger.info('create context for request: ' + request_id)
-                self._ctx[request_id] = context
-
-        pre_start_time = time.time()
-        data = self._preprocess(data, context=context)
-        infer_start_time = time.time()
-
-        # Update preprocess latency metric
-        pre_time_in_ms = (infer_start_time - pre_start_time) * 1000
-        logger.info('preprocess time: ' + str(pre_time_in_ms) + 'ms')
-
-        data = self._inference(data, context=context)
-        infer_end_time = time.time()
-        infer_in_ms = (infer_end_time - infer_start_time) * 1000
-        logger.info('infer time: ' + str(infer_in_ms) + 'ms')
-
-        try:
-            # 判断是否是可迭代对象
-            data = self._postprocess(data, context=context)
-            is_stream = all([
-                hasattr(data, '__iter__'),
-                not isinstance(data, (str, bytes, list, tuple, typing.Mapping))
-            ])
-            if not is_stream:
-                yield data
-                return
-
-            for ret in data:
-                yield ret
-
-        finally:
-            post_time_in_ms = (time.time() - infer_end_time) * 1000
-            logger.info('postprocess time: ' + str(post_time_in_ms) + 'ms')
-            # Update inference latency metric
-            logger.info('latency: ' + str(pre_time_in_ms + infer_in_ms + post_time_in_ms) + 'ms')
+        self.ctx = None
 
     @abstractmethod
-    def _inference(self, data, context={}):
+    def inference(self, data, request_id):
         '''
-        Internal inference methods. Run forward computation and
-        return output.
+        Wrapper function to run preprocess, inference and postprocess functions.
 
         Parameters
         ----------
-        data : map of NDArray
-            Preprocessed inputs in NDArray format.
+        data : map of object
+            Raw input from request.
 
         Returns
         -------
-        list of NDArray
-            Inference output.
+        list of outputs to be sent back to client.
+            data to be sent back
         '''
-        return data
+        pass
 
     @abstractmethod
-    def _preprocess(self, data, context={}):
-        '''
-        Internal preprocess methods. Do transformation on raw
-        inputs and convert them to NDArray.
-
-        Parameters
-        ----------
-        data : map of object
-            Raw inputs from request.
+    def ping(self):
+        '''Ping to get system's health.
 
         Returns
         -------
-        list of NDArray
-            Processed inputs in NDArray format.
+        String
+            A message, "health": "healthy!", to show system is healthy.
         '''
-        return data
+        pass
 
     @abstractmethod
-    def _postprocess(self, data, context={}):
-        '''
-        Internal postprocess methods. Do transformation on inference output
-        and convert them to MIME type objects.
-
-        Parameters
-        ----------
-        data : map of NDArray
-            Inference output.
+    def signature(self):
+        '''Signiture for model service.
 
         Returns
         -------
-        list of object
-            list of outputs to be sent back.
+        Dict
+            Model service signiture.
         '''
-        return data
-
-    def destroy_context(self, request_id):
-        logger.info('destroy context for request: ' + request_id)
-        if request_id in self._ctx:
-            del self._ctx[request_id]
-
-    @abstractmethod
-    def _warmup(self):
         pass
 
-    @property
-    def model_version(self):
-        return '1'
-
-    @property
-    def ready(self):
-        return self._ready
-
-    def run(self, *args, **kwargs):
-        from taichu_serve.command import cli
-        cli(*args, **kwargs)
+
+# class SingleNodeService(BaseModelService):
+#     '''SingleNodeModel defines abstraction for model service which loads a
+#     single model.
+#     '''
+#
+#     def __init__(self, model_path):
+#         super(SingleNodeService, self).__init__(model_path)
+#         self._ready = False
+#
+#     def warmup(self):
+#         start_time = time.time()
+#         self._warmup()
+#         self._ready = True
+#         logger.info('warmup time: ' + str((time.time() - start_time) * 1000) + 'ms')
+#
+#     def inference(self, data, context={}):
+#         '''
+#         Wrapper function to run preprocess, inference and postprocess functions.
+#
+#         Parameters
+#         ----------
+#         data : map of object
+#             Raw input from request.
+#
+#         Returns
+#         -------
+#         list of outputs to be sent back to client.
+#             data to be sent back
+#         '''
+#         pre_start_time = time.time()
+#         data = self._preprocess(data, context=context)
+#         infer_start_time = time.time()
+#
+#         # Update preprocess latency metric
+#         pre_time_in_ms = (infer_start_time - pre_start_time) * 1000
+#         logger.info('preprocess time: ' + str(pre_time_in_ms) + 'ms')
+#
+#         data = self._inference(data, context=context)
+#         infer_end_time = time.time()
+#         infer_in_ms = (infer_end_time - infer_start_time) * 1000
+#
+#         logger.info('infer time: ' + str(infer_in_ms) + 'ms')
+#         data = self._postprocess(data, context=context)
+#
+#         # Update inference latency metric
+#         post_time_in_ms = (time.time() - infer_end_time) * 1000
+#         logger.info('postprocess time: ' + str(post_time_in_ms) + 'ms')
+#
+#         logger.info('latency: ' + str(pre_time_in_ms + infer_in_ms + post_time_in_ms) + 'ms')
+#         return data
+#
+#     @abstractmethod
+#     def _inference(self, data, context={}):
+#         '''
+#         Internal inference methods. Run forward computation and
+#         return output.
+#
+#         Parameters
+#         ----------
+#         data : map of NDArray
+#             Preprocessed inputs in NDArray format.
+#
+#         Returns
+#         -------
+#         list of NDArray
+#             Inference output.
+#         '''
+#         return data
+#
+#     @abstractmethod
+#     def _preprocess(self, data, context={}):
+#         '''
+#         Internal preprocess methods. Do transformation on raw
+#         inputs and convert them to NDArray.
+#
+#         Parameters
+#         ----------
+#         data : map of object
+#             Raw inputs from request.
+#
+#         Returns
+#         -------
+#         list of NDArray
+#             Processed inputs in NDArray format.
+#         '''
+#         return data
+#
+#     @abstractmethod
+#     def _postprocess(self, data, context={}):
+#         '''
+#         Internal postprocess methods. Do transformation on inference output
+#         and convert them to MIME type objects.
+#
+#         Parameters
+#         ----------
+#         data : map of NDArray
+#             Inference output.
+#
+#         Returns
+#         -------
+#         list of object
+#             list of outputs to be sent back.
+#         '''
+#         return data
+#
+#     @abstractmethod
+#     def _warmup(self):
+#         pass
+#
+#     @property
+#     def model_version(self):
+#         return '1'
+#
+#     @property
+#     def ready(self):
+#         return self._ready
+#
+
+def load_service(path, name=None):
+    sys.path.append(os.path.dirname(path))
+
+    try:
+        if not name:
+            name = os.path.splitext(os.path.basename(path))[0]
+
+        module = None
+        if sys.version_info[0] > 2:
+            import importlib
+            spec = importlib.util.spec_from_file_location(name, path)
+            module = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(module)
+
+        else:
+            import imp
+            module = imp.load_source(name, path)
+
+        return module
+    except Exception:
+        traceback.print_exc()
+        raise Exception('Incorrect or missing service file: ' + path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `taichu-serve-2.0.25/taichu_serve/common.py` & `taichu-serve-2.0.9/taichu_serve/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 Local = threading.local()
 logger = logging.getLogger(__name__)
 
 
 def grpc_interceptor(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
+        Local.request_id = str(uuid.uuid4())
         context = args[2]
         start_time = time.time()
         try:
             ret = func(*args, **kwargs)
         except ModelPredictError as e:
             logger.error('[grpc_interceptor] error: %s', e.message)
             context.set_code(grpc.StatusCode.INTERNAL)
```

### Comparing `taichu-serve-2.0.25/taichu_serve/error_code.py` & `taichu-serve-2.0.9/taichu_serve/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.25/taichu_serve/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.25/taichu_serve/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.25/taichu_serve/log.py` & `taichu-serve-2.0.9/taichu_serve/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,18 +53,14 @@
         for (k, v) in record.__dict__.items():
             if k not in exclude_fields:
                 data[k] = v
 
         return json.dumps(data, ensure_ascii=False)
 
 
-def init_logger(json_format: bool = False):
+def init_logger():
     logging.basicConfig(level=logging.INFO)
     logger = logging.getLogger()
     logger.handlers = []
     consoleHandler = logging.StreamHandler(stream=sys.stdout)
-    if json_format:
-        consoleHandler.setFormatter(JsonFormatter(datefmt='%Y-%m-%d %H:%M:%S'))
-    else:
-        consoleHandler.setFormatter(
-            logging.Formatter('%(asctime)s %(levelname)s %(pathname)s:%(lineno)d - [PID:%(process)d] %(message)s'))
+    consoleHandler.setFormatter(JsonFormatter(datefmt='%Y-%m-%d %H:%M:%S'))
     logger.addHandler(consoleHandler)
```

### Comparing `taichu-serve-2.0.25/taichu_serve/template/test/grpc_client.py` & `taichu-serve-2.0.9/taichu_serve/template/test/grpc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import grpc
 import taichu_serve.grpc_predict_v2_pb2 as grpc_predict_v2_pb2
 import taichu_serve.grpc_predict_v2_pb2_grpc as grpc_predict_v2_pb2_grpc
 
-model_name = "ModelService"
+model_name = "TestService"
 
 
 def run():
     conn = grpc.insecure_channel('localhost:8080')
     client = grpc_predict_v2_pb2_grpc.GRPCInferenceServiceStub(channel=conn)
 
     req = grpc_predict_v2_pb2.ModelInferRequest()
```

### Comparing `taichu-serve-2.0.25/taichu_serve/template/test/stream_grpc_client.py` & `taichu-serve-2.0.9/taichu_serve/template/test/stream_grpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import grpc
 import taichu_serve.grpc_predict_v2_pb2 as grpc_predict_v2_pb2
 import taichu_serve.grpc_predict_v2_pb2_grpc as grpc_predict_v2_pb2_grpc
 
-model_name = "ModelService"
+model_name = "TestService"
 
 
 def guide_list_features(stub):
     num = 5
 
     while True:
```

### Comparing `taichu-serve-2.0.25/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-2.0.9/taichu_serve.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.md
 setup.py
 taichu_serve/__init__.py
 taichu_serve/app.py
 taichu_serve/command.py
 taichu_serve/common.py
 taichu_serve/dockerfile.py
 taichu_serve/error_code.py
@@ -16,14 +15,14 @@
 taichu_serve.egg-info/PKG-INFO
 taichu_serve.egg-info/SOURCES.txt
 taichu_serve.egg-info/dependency_links.txt
 taichu_serve.egg-info/entry_points.txt
 taichu_serve.egg-info/requires.txt
 taichu_serve.egg-info/top_level.txt
 taichu_serve/template/__init__.py
-taichu_serve/template/model_service.py
+taichu_serve/template/config.ini
+taichu_serve/template/customize_service.py
+taichu_serve/template/requirements.txt
 taichu_serve/template/test/__init__.py
 taichu_serve/template/test/grpc_client.py
 taichu_serve/template/test/http_client.py
-taichu_serve/template/test/stream_grpc_client.py
-taichu_serve/third/__init__.py
-taichu_serve/third/tracer.py
+taichu_serve/template/test/stream_grpc_client.py
```

