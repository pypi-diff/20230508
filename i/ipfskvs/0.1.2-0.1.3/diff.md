# Comparing `tmp/ipfskvs-0.1.2.tar.gz` & `tmp/ipfskvs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.1.2.tar", max compression
+gzip compressed data, was "ipfskvs-0.1.3.tar", max compression
```

## Comparing `ipfskvs-0.1.2.tar` & `ipfskvs-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.2/LICENSE
--rw-r--r--   0        0        0     2015 2023-04-20 00:29:03.095803 ipfskvs-0.1.2/README.md
--rw-r--r--   0        0        0      114 2023-05-07 22:58:52.420782 ipfskvs-0.1.2/ipfskvs/__init__.py
--rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.2/ipfskvs/index.py
--rw-r--r--   0        0        0     9170 2023-05-07 22:59:55.436372 ipfskvs-0.1.2/ipfskvs/store.py
--rw-r--r--   0        0        0      434 2023-05-07 22:58:27.375758 ipfskvs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 ipfskvs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2015 2023-04-20 00:29:03.095803 ipfskvs-0.1.3/README.md
+-rw-r--r--   0        0        0      114 2023-05-07 23:05:31.024049 ipfskvs-0.1.3/ipfskvs/__init__.py
+-rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.3/ipfskvs/index.py
+-rw-r--r--   0        0        0     9256 2023-05-07 23:06:38.029248 ipfskvs-0.1.3/ipfskvs/store.py
+-rw-r--r--   0        0        0      434 2023-05-07 23:05:39.619866 ipfskvs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 ipfskvs-0.1.3/PKG-INFO
```

### Comparing `ipfskvs-0.1.2/LICENSE` & `ipfskvs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.2/README.md` & `ipfskvs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.2/ipfskvs/index.py` & `ipfskvs-0.1.3/ipfskvs/index.py`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.2/ipfskvs/store.py` & `ipfskvs-0.1.3/ipfskvs/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,19 +233,20 @@
                 into a list of Index objects
         """
         result = []
 
         # list the files in the directory
         path = query_index.get_filename()
         response = ipfs.list_files(path)
+        LOG.debug("ipfs.list_files(%s): %s", path, response)
 
         filenames = [
             file['Name'] for file in response['Entries']
-        ] if response and 'Entries' in response else []
-        LOG.debug("ipfs.list_files(%s): %s", path, response)
+        ] if response and 'Entries' in response and response['Entries'] else []
+        LOG.debug("ipfs.list_files filenames: %s", filenames)
 
         for filename in filenames:
             # Listing the same file twice indicates the base case
             #   ex:
             #       path = `ls dir1/dir2` --> filenames = ["filename"]
             #       path = `ls dir1/dir2/filename` --> filenames = ["filename"]
             if filename in path:
```

### Comparing `ipfskvs-0.1.2/PKG-INFO` & `ipfskvs-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.1.2
+Version: 0.1.3
 Summary: IPFS Key Value Store
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (>=0.0.7,<0.0.8)
```

