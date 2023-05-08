# Comparing `tmp/miniopy-async-1.8.tar.gz` & `tmp/miniopy-async-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniopy-async-1.8.tar", last modified: Thu Jul 14 02:51:32 2022, max compression
+gzip compressed data, was "miniopy-async-1.9.tar", last modified: Thu Jul 14 13:47:40 2022, max compression
```

## Comparing `miniopy-async-1.8.tar` & `miniopy-async-1.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:51:32.617194 miniopy-async-1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-14 02:51:22.000000 miniopy-async-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-07-14 02:51:32.617194 miniopy-async-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-07-14 02:51:22.000000 miniopy-async-1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:51:32.613194 miniopy-async-1.8/miniopy_async/
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   143050 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    15004 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/commonconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:51:32.617194 miniopy-async-1.8/miniopy_async/credentials/
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/credentials/credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)    21581 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/credentials/providers.py
--rw-r--r--   0 runner    (1001) docker     (121)    26576 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4909 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/deleteobjects.py
--rw-r--r--   0 runner    (1001) docker     (121)     4673 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/error.py
--rw-r--r--   0 runner    (1001) docker     (121)    20212 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/legalhold.py
--rw-r--r--   0 runner    (1001) docker     (121)    12365 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/lifecycleconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     9872 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/minioadmin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9846 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/notificationconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/objectlockconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)    15423 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/replicationconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/retention.py
--rw-r--r--   0 runner    (1001) docker     (121)    15063 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/select.py
--rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/signer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3431 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/sse.py
--rw-r--r--   0 runner    (1001) docker     (121)     3109 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/sseconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/tagging.py
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/versioningconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-07-14 02:51:22.000000 miniopy-async-1.8/miniopy_async/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:51:32.617194 miniopy-async-1.8/miniopy_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-07-14 02:51:32.000000 miniopy-async-1.8/miniopy_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-07-14 02:51:32.000000 miniopy-async-1.8/miniopy_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 02:51:32.000000 miniopy-async-1.8/miniopy_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-14 02:51:32.000000 miniopy-async-1.8/miniopy_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-14 02:51:32.000000 miniopy-async-1.8/miniopy_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-14 02:51:32.617194 miniopy-async-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-07-14 02:51:22.000000 miniopy-async-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 13:47:40.198425 miniopy-async-1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-14 13:47:29.000000 miniopy-async-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-07-14 13:47:40.198425 miniopy-async-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-07-14 13:47:29.000000 miniopy-async-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 13:47:40.198425 miniopy-async-1.9/miniopy_async/
+-rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   143084 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15004 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/commonconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 13:47:40.198425 miniopy-async-1.9/miniopy_async/credentials/
+-rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/credentials/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21581 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/credentials/providers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26576 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4909 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/deleteobjects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4673 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/error.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20212 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/legalhold.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12365 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/lifecycleconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9872 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/minioadmin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9846 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/notificationconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/objectlockconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4561 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15423 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/replicationconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/retention.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15063 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/select.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/signer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3431 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/sse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3109 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/sseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2886 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/versioningconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-07-14 13:47:29.000000 miniopy-async-1.9/miniopy_async/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 13:47:40.198425 miniopy-async-1.9/miniopy_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-07-14 13:47:40.000000 miniopy-async-1.9/miniopy_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-07-14 13:47:40.000000 miniopy-async-1.9/miniopy_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 13:47:40.000000 miniopy-async-1.9/miniopy_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-14 13:47:40.000000 miniopy-async-1.9/miniopy_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-14 13:47:40.000000 miniopy-async-1.9/miniopy_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-14 13:47:40.198425 miniopy-async-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-07-14 13:47:29.000000 miniopy-async-1.9/setup.py
```

### Comparing `miniopy-async-1.8/LICENSE` & `miniopy-async-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/PKG-INFO` & `miniopy-async-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniopy-async
-Version: 1.8
+Version: 1.9
 Summary: Asynchronous MinIO Python Client API
 Home-page: https://github.com/hlf20010508/miniopy-async
 Author: L-ING
 Author-email: hlf01@icloud.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: miniopy-async Version: 1.8 Summary: Asynchronous
+Metadata-Version: 2.1 Name: miniopy-async Version: 1.9 Summary: Asynchronous
 MinIO Python Client API Home-page: https://github.com/hlf20010508/miniopy-async
 Author: L-ING Author-email: hlf01@icloud.com License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `miniopy-async-1.8/README.md` & `miniopy-async-1.9/README.md`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/__init__.py` & `miniopy-async-1.9/miniopy_async/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 :Copyright © 2022 L-ING.
 :license: Apache 2.0, see LICENSE for more details.
 """
 
 __title__ = "miniopy-async"
 __author__ = "L-ING."
-__version__ = "1.8"
+__version__ = "1.9"
 __license__ = "Apache 2.0"
 __copyright__ = "(C) 2022 L-ING <hlf01@icloud.com>"
 
 import threading
 
 __LOCALE_LOCK__ = threading.Lock()
```

### Comparing `miniopy-async-1.8/miniopy_async/api.py` & `miniopy-async-1.9/miniopy_async/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,14 +261,15 @@
         async with aiohttp.ClientSession() as session:
             response = await session.request(
                 method,
                 urlunsplit(url),
                 data=body,
                 headers=headers
             )
+            await response.read()
 
         if response.status in [200, 204, 206]:
             return response
 
         response_data = await response.text()
         content_types = response.headers.get("content-type", "").split(";")
         if method != "HEAD" and "application/xml" not in content_types:
```

### Comparing `miniopy-async-1.8/miniopy_async/commonconfig.py` & `miniopy-async-1.9/miniopy_async/commonconfig.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/credentials/__init__.py` & `miniopy-async-1.9/miniopy_async/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/credentials/credentials.py` & `miniopy-async-1.9/miniopy_async/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/credentials/providers.py` & `miniopy-async-1.9/miniopy_async/credentials/providers.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/datatypes.py` & `miniopy-async-1.9/miniopy_async/datatypes.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/deleteobjects.py` & `miniopy-async-1.9/miniopy_async/deleteobjects.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/error.py` & `miniopy-async-1.9/miniopy_async/error.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/helpers.py` & `miniopy-async-1.9/miniopy_async/helpers.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/legalhold.py` & `miniopy-async-1.9/miniopy_async/legalhold.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/lifecycleconfig.py` & `miniopy-async-1.9/miniopy_async/lifecycleconfig.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/minioadmin.py` & `miniopy-async-1.9/miniopy_async/minioadmin.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/notificationconfig.py` & `miniopy-async-1.9/miniopy_async/notificationconfig.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/objectlockconfig.py` & `miniopy-async-1.9/miniopy_async/objectlockconfig.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/progress.py` & `miniopy-async-1.9/miniopy_async/progress.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/replicationconfig.py` & `miniopy-async-1.9/miniopy_async/replicationconfig.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/retention.py` & `miniopy-async-1.9/miniopy_async/retention.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/select.py` & `miniopy-async-1.9/miniopy_async/select.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/signer.py` & `miniopy-async-1.9/miniopy_async/signer.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/sse.py` & `miniopy-async-1.9/miniopy_async/sse.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/sseconfig.py` & `miniopy-async-1.9/miniopy_async/sseconfig.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/tagging.py` & `miniopy-async-1.9/miniopy_async/tagging.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/time.py` & `miniopy-async-1.9/miniopy_async/time.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/versioningconfig.py` & `miniopy-async-1.9/miniopy_async/versioningconfig.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async/xml.py` & `miniopy-async-1.9/miniopy_async/xml.py`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/miniopy_async.egg-info/PKG-INFO` & `miniopy-async-1.9/miniopy_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniopy-async
-Version: 1.8
+Version: 1.9
 Summary: Asynchronous MinIO Python Client API
 Home-page: https://github.com/hlf20010508/miniopy-async
 Author: L-ING
 Author-email: hlf01@icloud.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: miniopy-async Version: 1.8 Summary: Asynchronous
+Metadata-Version: 2.1 Name: miniopy-async Version: 1.9 Summary: Asynchronous
 MinIO Python Client API Home-page: https://github.com/hlf20010508/miniopy-async
 Author: L-ING Author-email: hlf01@icloud.com License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `miniopy-async-1.8/miniopy_async.egg-info/SOURCES.txt` & `miniopy-async-1.9/miniopy_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miniopy-async-1.8/setup.py` & `miniopy-async-1.9/setup.py`

 * *Files identical despite different names*

