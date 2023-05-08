# Comparing `tmp/rcsb.utils.io-1.42.tar.gz` & `tmp/rcsb.utils.io-1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.io-1.42.tar", last modified: Thu Mar 16 13:31:23 2023, max compression
+gzip compressed data, was "rcsb.utils.io-1.43.tar", last modified: Mon May  8 14:04:43 2023, max compression
```

## Comparing `rcsb.utils.io-1.42.tar` & `rcsb.utils.io-1.43.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-16 13:31:23.638632 rcsb.utils.io-1.42/
--rw-r--r--   0 vsts      (1001) docker     (122)     9367 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1740 2023-03-16 13:31:23.638632 rcsb.utils.io-1.42/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1024 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-16 13:31:23.630632 rcsb.utils.io-1.42/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-16 13:31:23.630632 rcsb.utils.io-1.42/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-16 13:31:23.638632 rcsb.utils.io-1.42/rcsb/utils/io/
--rw-r--r--   0 vsts      (1001) docker     (122)     1828 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/CacheUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6185 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/CryptUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4635 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/ExecUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12022 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/FastaUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5604 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/FileLock.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25377 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/FileUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12683 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/FtpUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6281 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/GitUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1198 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/HashableDict.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6761 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/IndexUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    32305 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/IoUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/LogUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6341 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/MarshalUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5113 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/ProcessStatusUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6260 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/SftpUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)      796 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/SingletonClass.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1716 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/SplitJoin.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12245 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/StashUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11807 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/StashableBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3145 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14817 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/UrlRequestUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4495 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/rcsb/utils/io/decorators.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-16 13:31:23.630632 rcsb.utils.io-1.42/rcsb.utils.io.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1740 2023-03-16 13:31:23.000000 rcsb.utils.io-1.42/rcsb.utils.io.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      975 2023-03-16 13:31:23.000000 rcsb.utils.io-1.42/rcsb.utils.io.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-16 13:31:23.000000 rcsb.utils.io-1.42/rcsb.utils.io.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-16 13:26:21.000000 rcsb.utils.io-1.42/rcsb.utils.io.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      423 2023-03-16 13:31:23.000000 rcsb.utils.io-1.42/rcsb.utils.io.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-03-16 13:31:23.000000 rcsb.utils.io-1.42/rcsb.utils.io.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      389 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-03-16 13:31:23.638632 rcsb.utils.io-1.42/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2271 2023-03-16 13:23:59.000000 rcsb.utils.io-1.42/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.085972 rcsb.utils.io-1.43/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9456 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1740 2023-05-08 14:04:43.085972 rcsb.utils.io-1.43/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1024 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.081972 rcsb.utils.io-1.43/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.081972 rcsb.utils.io-1.43/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.085972 rcsb.utils.io-1.43/rcsb/utils/io/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1828 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/CacheUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6185 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/CryptUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4635 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/ExecUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12022 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/FastaUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5604 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/FileLock.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25377 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/FileUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12683 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/FtpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6281 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/GitUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1198 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/HashableDict.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6761 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/IndexUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    32305 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/IoUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/LogUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6341 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/MarshalUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5113 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/ProcessStatusUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6260 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/SftpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      796 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/SingletonClass.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1716 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/SplitJoin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12245 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/StashUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11807 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/StashableBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3145 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14760 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/UrlRequestUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4495 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/decorators.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.081972 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1740 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      975 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-08 13:59:52.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      423 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      389 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-08 14:04:43.085972 rcsb.utils.io-1.43/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2271 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/setup.py
```

### Comparing `rcsb.utils.io-1.42/HISTORY.txt` & `rcsb.utils.io-1.43/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -126,8 +126,9 @@
  6-Jun-2022  - V1.35 Resolve pylint issues in FastaUtil
  8-Sep-2022  - V1.36 Resolve pylint issues
  3-Oct-2022  - V1.37 Add options to UrlRequestUtil
  5-Dec-2022  - V1.38 Update UniProt fetching tests
 23-Dec-2022  - V1.39 Configuration changes to support tox 4
 13-Feb-2023  - V1.40 Resolve pylint issues
 14-Mar-2023  - V1.41 Make 'timeout' parameter a keyword argument for instantiating FileUtil object
-15-Mar-2023  - V1.42 Fix checking for remote branches by name in GitUtil()
+15-Mar-2023  - V1.42 Fix checking for remote branches by name in GitUtil()
+ 8-May-2023  - V1.43 Use allowed_methods instead of deprecated param in UrlRequestUtil()
```

### Comparing `rcsb.utils.io-1.42/LICENSE` & `rcsb.utils.io-1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/PKG-INFO` & `rcsb.utils.io-1.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.io
-Version: 1.42
+Version: 1.43
 Summary: RCSB Python I/O Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_io
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.io-1.42/README.md` & `rcsb.utils.io-1.43/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/CacheUtils.py` & `rcsb.utils.io-1.43/rcsb/utils/io/CacheUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/CryptUtils.py` & `rcsb.utils.io-1.43/rcsb/utils/io/CryptUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/ExecUtils.py` & `rcsb.utils.io-1.43/rcsb/utils/io/ExecUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/FastaUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/FastaUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/FileLock.py` & `rcsb.utils.io-1.43/rcsb/utils/io/FileLock.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/FileUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/FileUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/FtpUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/FtpUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/GitUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/GitUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/HashableDict.py` & `rcsb.utils.io-1.43/rcsb/utils/io/HashableDict.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/IndexUtils.py` & `rcsb.utils.io-1.43/rcsb/utils/io/IndexUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/IoUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/IoUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/LogUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/LogUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/MarshalUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/MarshalUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/ProcessStatusUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/ProcessStatusUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/SftpUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/SftpUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/SingletonClass.py` & `rcsb.utils.io-1.43/rcsb/utils/io/SingletonClass.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/SplitJoin.py` & `rcsb.utils.io-1.43/rcsb/utils/io/SplitJoin.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/StashUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/StashUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/StashableBase.py` & `rcsb.utils.io-1.43/rcsb/utils/io/StashableBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/TimeUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/UrlRequestUtil.py` & `rcsb.utils.io-1.43/rcsb/utils/io/UrlRequestUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Simple wrapper for URL request processing
 #
 # Updates:
 #  17-Mar-2019 jdw adjust return value to include response error code
 #  16-Dec-2019 jdw add HTTPException to retry()
 #  28-May-2019 jdw unwrapped methods now using requests module library.
 #   3-Oct-2022 dwp add flag to allow option of overwriting of User-Agent or not
+#   8-May-2023 aae Use allowed_methods instead of deprecated param
 #
 ##
 
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
@@ -222,15 +223,15 @@
         exceptionsCatch = kwargs.get("exceptionsCatch", (HTTPError))
         httpCodesCatch = kwargs.get("httpCodesCatch", [])
         returnContentType = kwargs.get("returnContentType", None)
         timeOutSeconds = kwargs.get("timeOut", 5)
         retries = kwargs.get("retries", 3)
         statusForcelist = (429, 500, 502, 503, 504)
         backoffFactor = 5
-        methodWhitelist = ("HEAD", "GET", "PUT", "DELETE", "OPTIONS", "TRACE", "POST")
+        allowedMethods = ("HEAD", "GET", "PUT", "DELETE", "OPTIONS", "TRACE", "POST")
         if returnContentType == "JSON":
             if "Accept" not in headerD:
                 headerD["Accept"] = "application/json"
         #
         if overwriteUserAgent:
             headerD.update({"User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36"})
         #
@@ -242,16 +243,15 @@
                 with requests.Session() as session:
                     thisRetry = Retry(
                         total=retries,
                         read=retries,
                         connect=retries,
                         backoff_factor=backoffFactor,
                         status_forcelist=statusForcelist,
-                        # allowed_methods=methodWhitelist,
-                        method_whitelist=methodWhitelist,
+                        allowed_methods=allowedMethods,
                     )
                     adapter = HTTPAdapter(max_retries=thisRetry)
                     session.mount("http://", adapter)
                     session.mount("https://", adapter)
                     # session = self.__requestsRetrySession(retries=3, backoffFactor=5, statusForcelist=(429, 500, 502, 503, 504))
                     req = session.get(urlPath, params=paramD, headers=headerD, **optD)
             else:
@@ -290,15 +290,15 @@
         exceptionsCatch = kwargs.get("exceptionsCatch", (HTTPError))
         httpCodesCatch = kwargs.get("httpCodesCatch", [])
         returnContentType = kwargs.get("returnContentType", None)
         sendContentType = kwargs.get("sendContentType", None)
         timeOutSeconds = kwargs.get("timeOut", 5)
         retries = kwargs.get("retries", 3)
         statusForcelist = (429, 500, 502, 503, 504)
-        methodWhitelist = ("HEAD", "GET", "PUT", "DELETE", "OPTIONS", "TRACE", "POST")
+        allowedMethods = ("HEAD", "GET", "PUT", "DELETE", "OPTIONS", "TRACE", "POST")
         backoffFactor = 5
         if returnContentType in ["JSON", "application/json"]:
             if "Accept" not in headerD:
                 headerD["Accept"] = "application/json"
         if sendContentType is not None:
             if "Content-Type" not in headerD:
                 headerD["Content-Type"] = sendContentType
@@ -312,16 +312,15 @@
                 with requests.Session() as session:
                     thisRetry = Retry(
                         total=retries,
                         read=retries,
                         connect=retries,
                         backoff_factor=backoffFactor,
                         status_forcelist=statusForcelist,
-                        # allowed_methods=methodWhitelist,
-                        method_whitelist=methodWhitelist,
+                        allowed_methods=allowedMethods,
                     )
                     adapter = HTTPAdapter(max_retries=thisRetry)
                     session.mount("http://", adapter)
                     session.mount("https://", adapter)
                     # session = self.__requestsRetrySession(retries=retries, backoffFactor=5, statusForcelist=(429, 500, 502, 504))
                     if sendContentType == "application/json":
                         req = session.post(urlPath, json=paramD, headers=headerD, **optD)
```

### Comparing `rcsb.utils.io-1.42/rcsb/utils/io/decorators.py` & `rcsb.utils.io-1.43/rcsb/utils/io/decorators.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/rcsb.utils.io.egg-info/PKG-INFO` & `rcsb.utils.io-1.43/rcsb.utils.io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.io
-Version: 1.42
+Version: 1.43
 Summary: RCSB Python I/O Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_io
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.io-1.42/rcsb.utils.io.egg-info/SOURCES.txt` & `rcsb.utils.io-1.43/rcsb.utils.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.42/setup.py` & `rcsb.utils.io-1.43/setup.py`

 * *Files identical despite different names*

