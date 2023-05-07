# Comparing `tmp/ipfskvs-0.1.1.tar.gz` & `tmp/ipfskvs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.1.1.tar", max compression
+gzip compressed data, was "ipfskvs-0.1.2.tar", max compression
```

## Comparing `ipfskvs-0.1.1.tar` & `ipfskvs-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.1/LICENSE
--rw-r--r--   0        0        0     2015 2023-04-20 00:29:03.095803 ipfskvs-0.1.1/README.md
--rw-r--r--   0        0        0      114 2023-04-21 01:11:31.933487 ipfskvs-0.1.1/ipfskvs/__init__.py
--rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.1/ipfskvs/index.py
--rw-r--r--   0        0        0     9108 2023-04-23 19:08:07.056945 ipfskvs-0.1.1/ipfskvs/store.py
--rw-r--r--   0        0        0      434 2023-04-21 01:11:19.091616 ipfskvs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 ipfskvs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2015 2023-04-20 00:29:03.095803 ipfskvs-0.1.2/README.md
+-rw-r--r--   0        0        0      114 2023-05-07 22:58:52.420782 ipfskvs-0.1.2/ipfskvs/__init__.py
+-rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.2/ipfskvs/index.py
+-rw-r--r--   0        0        0     9170 2023-05-07 22:59:55.436372 ipfskvs-0.1.2/ipfskvs/store.py
+-rw-r--r--   0        0        0      434 2023-05-07 22:58:27.375758 ipfskvs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 ipfskvs-0.1.2/PKG-INFO
```

### Comparing `ipfskvs-0.1.1/LICENSE` & `ipfskvs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.1/README.md` & `ipfskvs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.1/ipfskvs/index.py` & `ipfskvs-0.1.2/ipfskvs/index.py`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.1/ipfskvs/store.py` & `ipfskvs-0.1.2/ipfskvs/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 __package__ = "ipfskvs"
 
 import errno
 import logging
 import os
-import time
 from dataclasses import dataclass
 from types import FunctionType
 from typing import Dict, Iterator, List, Self
 
 from google.protobuf.message import Message
 
 from ipfsclient.ipfs import Ipfs
@@ -237,15 +236,16 @@
 
         # list the files in the directory
         path = query_index.get_filename()
         response = ipfs.list_files(path)
 
         filenames = [
             file['Name'] for file in response['Entries']
-        ] if 'Entries' in response else []
+        ] if response and 'Entries' in response else []
+        LOG.debug("ipfs.list_files(%s): %s", path, response)
 
         for filename in filenames:
             # Listing the same file twice indicates the base case
             #   ex:
             #       path = `ls dir1/dir2` --> filenames = ["filename"]
             #       path = `ls dir1/dir2/filename` --> filenames = ["filename"]
             if filename in path:
```

### Comparing `ipfskvs-0.1.1/PKG-INFO` & `ipfskvs-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.1.1
+Version: 0.1.2
 Summary: IPFS Key Value Store
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (>=0.0.7,<0.0.8)
```

