# Comparing `tmp/ipfskvs-0.1.4.tar.gz` & `tmp/ipfskvs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.1.4.tar", max compression
+gzip compressed data, was "ipfskvs-0.1.5.tar", max compression
```

## Comparing `ipfskvs-0.1.4.tar` & `ipfskvs-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.4/LICENSE
--rw-r--r--   0        0        0     2015 2023-04-20 00:29:03.095803 ipfskvs-0.1.4/README.md
--rw-r--r--   0        0        0      114 2023-05-08 00:15:16.638037 ipfskvs-0.1.4/ipfskvs/__init__.py
--rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.4/ipfskvs/index.py
--rw-r--r--   0        0        0     9292 2023-05-08 00:14:51.008473 ipfskvs-0.1.4/ipfskvs/store.py
--rw-r--r--   0        0        0      434 2023-05-08 00:15:13.471247 ipfskvs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 ipfskvs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2015 2023-04-20 00:29:03.095803 ipfskvs-0.1.5/README.md
+-rw-r--r--   0        0        0      114 2023-05-08 00:33:40.917518 ipfskvs-0.1.5/ipfskvs/__init__.py
+-rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.5/ipfskvs/index.py
+-rw-r--r--   0        0        0     9352 2023-05-08 00:33:31.002191 ipfskvs-0.1.5/ipfskvs/store.py
+-rw-r--r--   0        0        0      434 2023-05-08 00:33:37.775338 ipfskvs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 ipfskvs-0.1.5/PKG-INFO
```

### Comparing `ipfskvs-0.1.4/LICENSE` & `ipfskvs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.4/README.md` & `ipfskvs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.4/ipfskvs/index.py` & `ipfskvs-0.1.5/ipfskvs/index.py`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.4/ipfskvs/store.py` & `ipfskvs-0.1.5/ipfskvs/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,12 +281,13 @@
             ipfs (Ipfs): The IPFS client.
             reader (Message): _description_
 
         Yields:
             Iterator[Store]: The list of matching Store objects with
                 file content loaded into the `reader` attribute
         """
+        LOG.debug("query index: %s", query_index.to_dict())
         for response_index in Store.query_indexes(query_index, ipfs):
             reader = type(reader)()
             store = Store(index=response_index, reader=reader, ipfs=ipfs)
             store.read()
             yield store
```

### Comparing `ipfskvs-0.1.4/PKG-INFO` & `ipfskvs-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.1.4
+Version: 0.1.5
 Summary: IPFS Key Value Store
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (>=0.0.7,<0.0.8)
```

