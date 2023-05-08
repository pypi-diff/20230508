# Comparing `tmp/aioxmlrpc-0.6.5.tar.gz` & `tmp/aioxmlrpc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxmlrpc-0.6.5.tar", max compression
+gzip compressed data, was "aioxmlrpc-0.7.0.tar", max compression
```

## Comparing `aioxmlrpc-0.6.5.tar` & `aioxmlrpc-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1525 2022-06-02 06:43:48.349040 aioxmlrpc-0.6.5/LICENSE
--rw-r--r--   0        0        0     1390 2022-06-02 06:43:48.349040 aioxmlrpc-0.6.5/README.rst
--rw-r--r--   0        0        0      498 2023-04-27 08:33:37.381595 aioxmlrpc-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      129 2022-06-02 06:43:48.352373 aioxmlrpc-0.6.5/src/aioxmlrpc/__init__.py
--rw-r--r--   0        0        0     4741 2022-06-02 06:43:48.352373 aioxmlrpc-0.6.5/src/aioxmlrpc/client.py
--rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 aioxmlrpc-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1525 2022-06-02 06:43:48.349040 aioxmlrpc-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1464 2023-05-08 09:36:16.556811 aioxmlrpc-0.7.0/README.rst
+-rw-r--r--   0        0        0      498 2023-05-08 10:01:12.579757 aioxmlrpc-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      129 2022-06-02 06:43:48.352373 aioxmlrpc-0.7.0/src/aioxmlrpc/__init__.py
+-rw-r--r--   0        0        0     4844 2023-05-08 09:47:19.208644 aioxmlrpc-0.7.0/src/aioxmlrpc/client.py
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 aioxmlrpc-0.7.0/PKG-INFO
```

### Comparing `aioxmlrpc-0.6.5/LICENSE` & `aioxmlrpc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxmlrpc-0.6.5/README.rst` & `aioxmlrpc-0.7.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,14 @@
    :target: https://github.com/mardiros/aioxmlrpc/actions/workflows/main.yml
 
 
 .. image:: https://codecov.io/gh/mardiros/aioxmlrpc/branch/master/graph/badge.svg?token=BR3KttC9uJ
    :target: https://codecov.io/gh/mardiros/aioxmlrpc
 
 
-Getting Started
-===============
-
 Asyncio version of the standard lib ``xmlrpc``
 
 Currently only ``aioxmlrpc.client``, which works like ``xmlrpc.client`` but
 with coroutine is implemented.
 
 Fill free to fork me if you want to implement the server part.
 
@@ -24,21 +21,24 @@
 ``aioxmlrpc`` is based on ``httpx`` for the transport, and just patch
 the necessary from the python standard library to get it working.
 
 
 Installation
 ------------
 
+aioxmlrpc is available on PyPI, it can simply be installed with your favorite
+tool, example with pip here.
+
 ::
 
     pip install aioxmlrpc
 
 
-Example of usage
-----------------
+Getting Started
+---------------
 
 This example show how to print the current version of the Gandi XML-RPC api.
 
 
 ::
 
     import asyncio
@@ -58,7 +58,8 @@
 
 
 Run the example
 
 ::
 
     poetry run examples/gandi_api_version.py
+
```

### Comparing `aioxmlrpc-0.6.5/src/aioxmlrpc/client.py` & `aioxmlrpc-0.7.0/src/aioxmlrpc/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,27 +126,30 @@
         uri,
         encoding=None,
         verbose=False,
         allow_none=False,
         use_datetime=False,
         use_builtin_types=False,
         auth=None,
+        *,
         headers=None,
+        context=None,
         timeout=5.0,
         session=None,
     ):
 
         if not headers:
             headers = {
                 "User-Agent": "python/aioxmlrpc",
                 "Accept": "text/xml",
                 "Content-Type": "text/xml",
             }
-
-        self._session = session or httpx.AsyncClient(headers=headers)
+        if context is None:
+            context = True
+        self._session = session or httpx.AsyncClient(headers=headers, verify=context)
         transport = AioTransport(
             use_https=uri.startswith("https://"),
             session=self._session,
             auth=auth,
             timeout=timeout,
             use_datetime=use_datetime,
             use_builtin_types=use_builtin_types,
```

### Comparing `aioxmlrpc-0.6.5/PKG-INFO` & `aioxmlrpc-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxmlrpc
-Version: 0.6.5
+Version: 0.7.0
 Summary: XML-RPC client for asyncio
 Home-page: https://github.com/mardiros/aioxmlrpc
 License: BSD-3-Clause License
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -25,17 +25,14 @@
    :target: https://github.com/mardiros/aioxmlrpc/actions/workflows/main.yml
 
 
 .. image:: https://codecov.io/gh/mardiros/aioxmlrpc/branch/master/graph/badge.svg?token=BR3KttC9uJ
    :target: https://codecov.io/gh/mardiros/aioxmlrpc
 
 
-Getting Started
-===============
-
 Asyncio version of the standard lib ``xmlrpc``
 
 Currently only ``aioxmlrpc.client``, which works like ``xmlrpc.client`` but
 with coroutine is implemented.
 
 Fill free to fork me if you want to implement the server part.
 
@@ -43,21 +40,24 @@
 ``aioxmlrpc`` is based on ``httpx`` for the transport, and just patch
 the necessary from the python standard library to get it working.
 
 
 Installation
 ------------
 
+aioxmlrpc is available on PyPI, it can simply be installed with your favorite
+tool, example with pip here.
+
 ::
 
     pip install aioxmlrpc
 
 
-Example of usage
-----------------
+Getting Started
+---------------
 
 This example show how to print the current version of the Gandi XML-RPC api.
 
 
 ::
 
     import asyncio
@@ -78,7 +78,8 @@
 
 Run the example
 
 ::
 
     poetry run examples/gandi_api_version.py
 
+
```

