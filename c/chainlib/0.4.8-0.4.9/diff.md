# Comparing `tmp/chainlib-0.4.8.tar.gz` & `tmp/chainlib-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlib-0.4.8.tar", last modified: Tue Feb 14 06:44:25 2023, max compression
+gzip compressed data, was "chainlib-0.4.9.tar", last modified: Tue Feb 14 10:39:44 2023, max compression
```

## Comparing `chainlib-0.4.8.tar` & `chainlib-0.4.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 06:44:25.979941 chainlib-0.4.8/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:02:45.000000 chainlib-0.4.8/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       95 2022-11-14 07:11:06.000000 chainlib-0.4.8/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      726 2023-02-14 06:44:25.979941 chainlib-0.4.8/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     2776 2022-11-14 18:45:27.000000 chainlib-0.4.8/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      868 2022-11-14 07:03:32.000000 chainlib-0.4.8/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1621 2022-11-14 07:04:27.000000 chainlib-0.4.8/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 06:44:25.976607 chainlib-0.4.8/chainlib/
--rw-r--r--   0 lash      (1000) lash      (1000)      699 2021-10-10 10:19:14.000000 chainlib-0.4.8/chainlib/auth.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1341 2023-02-10 19:31:04.000000 chainlib-0.4.8/chainlib/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5667 2021-12-21 15:02:23.000000 chainlib-0.4.8/chainlib/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 06:44:25.979941 chainlib-0.4.8/chainlib/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      107 2022-11-04 07:26:52.000000 chainlib-0.4.8/chainlib/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6330 2023-02-13 06:37:30.000000 chainlib-0.4.8/chainlib/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4695 2023-02-13 06:37:30.000000 chainlib-0.4.8/chainlib/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1833 2023-02-14 06:42:51.000000 chainlib-0.4.8/chainlib/cli/gen.py
--rw-r--r--   0 lash      (1000) lash      (1000)      312 2023-02-14 06:42:51.000000 chainlib-0.4.8/chainlib/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)    12465 2022-11-12 13:30:44.000000 chainlib-0.4.8/chainlib/cli/man.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4594 2023-02-13 06:37:30.000000 chainlib-0.4.8/chainlib/cli/rpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4477 2022-11-03 17:13:57.000000 chainlib-0.4.8/chainlib/cli/wallet.py
--rw-r--r--   0 lash      (1000) lash      (1000)    13045 2022-12-28 13:36:25.000000 chainlib-0.4.8/chainlib/connection.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 06:44:25.973274 chainlib-0.4.8/chainlib/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 06:44:25.979941 chainlib-0.4.8/chainlib/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)      223 2022-10-13 13:02:39.000000 chainlib-0.4.8/chainlib/data/config/config.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 06:44:25.979941 chainlib-0.4.8/chainlib/data/env/
--rw-r--r--   0 lash      (1000) lash      (1000)     1198 2022-04-28 15:42:34.000000 chainlib-0.4.8/chainlib/data/env/env.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      290 2023-02-10 19:31:04.000000 chainlib-0.4.8/chainlib/dialect.py
--rw-r--r--   0 lash      (1000) lash      (1000)      962 2021-12-21 15:02:23.000000 chainlib-0.4.8/chainlib/encode.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1243 2022-10-13 13:02:39.000000 chainlib-0.4.8/chainlib/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)      216 2021-10-10 10:19:14.000000 chainlib-0.4.8/chainlib/fee.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1088 2021-10-10 10:19:14.000000 chainlib-0.4.8/chainlib/hash.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1150 2021-10-10 10:19:14.000000 chainlib-0.4.8/chainlib/http.py
--rw-r--r--   0 lash      (1000) lash      (1000)     8121 2021-10-10 10:19:14.000000 chainlib-0.4.8/chainlib/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4354 2021-10-10 10:19:14.000000 chainlib-0.4.8/chainlib/jsonrpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)      300 2022-10-13 13:12:24.000000 chainlib-0.4.8/chainlib/nonce.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 06:44:25.979941 chainlib-0.4.8/chainlib/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     3323 2023-02-14 06:42:51.000000 chainlib-0.4.8/chainlib/runnable/gen.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1781 2023-02-13 06:37:30.000000 chainlib-0.4.8/chainlib/settings.py
--rw-r--r--   0 lash      (1000) lash      (1000)      305 2021-10-10 10:19:14.000000 chainlib-0.4.8/chainlib/sign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1739 2023-02-11 11:42:28.000000 chainlib-0.4.8/chainlib/src.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1203 2021-10-10 10:19:14.000000 chainlib-0.4.8/chainlib/stat.py
--rw-r--r--   0 lash      (1000) lash      (1000)      184 2022-10-13 13:02:39.000000 chainlib-0.4.8/chainlib/status.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2188 2023-02-10 19:31:04.000000 chainlib-0.4.8/chainlib/tx.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 06:44:25.976607 chainlib-0.4.8/chainlib.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      726 2023-02-14 06:44:25.000000 chainlib-0.4.8/chainlib.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      903 2023-02-14 06:44:25.000000 chainlib-0.4.8/chainlib.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-02-14 06:44:25.000000 chainlib-0.4.8/chainlib.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       60 2023-02-14 06:44:25.000000 chainlib-0.4.8/chainlib.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       89 2023-02-14 06:44:25.000000 chainlib-0.4.8/chainlib.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-02-14 06:44:25.000000 chainlib-0.4.8/chainlib.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       70 2022-10-13 13:02:39.000000 chainlib-0.4.8/requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 06:44:25.979941 chainlib-0.4.8/scripts/
--rwxr-xr-x   0 lash      (1000) lash      (1000)     7382 2022-11-12 13:17:39.000000 chainlib-0.4.8/scripts/chainlib-man.py
--rw-r--r--   0 lash      (1000) lash      (1000)      712 2023-02-14 06:44:25.979941 chainlib-0.4.8/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      655 2023-02-14 06:42:51.000000 chainlib-0.4.8/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 10:39:44.006665 chainlib-0.4.9/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:02:45.000000 chainlib-0.4.9/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       95 2022-11-14 07:11:06.000000 chainlib-0.4.9/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      726 2023-02-14 10:39:44.006665 chainlib-0.4.9/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     2776 2022-11-14 18:45:27.000000 chainlib-0.4.9/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      868 2022-11-14 07:03:32.000000 chainlib-0.4.9/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1621 2022-11-14 07:04:27.000000 chainlib-0.4.9/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 10:39:44.003332 chainlib-0.4.9/chainlib/
+-rw-r--r--   0 lash      (1000) lash      (1000)      699 2021-10-10 10:19:14.000000 chainlib-0.4.9/chainlib/auth.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1341 2023-02-10 19:31:04.000000 chainlib-0.4.9/chainlib/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5667 2021-12-21 15:02:23.000000 chainlib-0.4.9/chainlib/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 10:39:44.006665 chainlib-0.4.9/chainlib/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      107 2022-11-04 07:26:52.000000 chainlib-0.4.9/chainlib/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6330 2023-02-13 06:37:30.000000 chainlib-0.4.9/chainlib/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4695 2023-02-13 06:37:30.000000 chainlib-0.4.9/chainlib/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1833 2023-02-14 06:42:51.000000 chainlib-0.4.9/chainlib/cli/gen.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      312 2023-02-14 06:42:51.000000 chainlib-0.4.9/chainlib/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    12465 2022-11-12 13:30:44.000000 chainlib-0.4.9/chainlib/cli/man.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4594 2023-02-13 06:37:30.000000 chainlib-0.4.9/chainlib/cli/rpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4477 2022-11-03 17:13:57.000000 chainlib-0.4.9/chainlib/cli/wallet.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    13045 2022-12-28 13:36:25.000000 chainlib-0.4.9/chainlib/connection.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 10:39:44.003332 chainlib-0.4.9/chainlib/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 10:39:44.006665 chainlib-0.4.9/chainlib/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)      223 2022-10-13 13:02:39.000000 chainlib-0.4.9/chainlib/data/config/config.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 10:39:44.006665 chainlib-0.4.9/chainlib/data/env/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1198 2022-04-28 15:42:34.000000 chainlib-0.4.9/chainlib/data/env/env.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      290 2023-02-10 19:31:04.000000 chainlib-0.4.9/chainlib/dialect.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      962 2021-12-21 15:02:23.000000 chainlib-0.4.9/chainlib/encode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1243 2022-10-13 13:02:39.000000 chainlib-0.4.9/chainlib/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      216 2021-10-10 10:19:14.000000 chainlib-0.4.9/chainlib/fee.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1088 2021-10-10 10:19:14.000000 chainlib-0.4.9/chainlib/hash.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1150 2021-10-10 10:19:14.000000 chainlib-0.4.9/chainlib/http.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     8121 2021-10-10 10:19:14.000000 chainlib-0.4.9/chainlib/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4354 2021-10-10 10:19:14.000000 chainlib-0.4.9/chainlib/jsonrpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      300 2022-10-13 13:12:24.000000 chainlib-0.4.9/chainlib/nonce.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 10:39:44.006665 chainlib-0.4.9/chainlib/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3323 2023-02-14 06:42:51.000000 chainlib-0.4.9/chainlib/runnable/gen.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1896 2023-02-14 10:39:30.000000 chainlib-0.4.9/chainlib/settings.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      305 2021-10-10 10:19:14.000000 chainlib-0.4.9/chainlib/sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1739 2023-02-11 11:42:28.000000 chainlib-0.4.9/chainlib/src.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1203 2021-10-10 10:19:14.000000 chainlib-0.4.9/chainlib/stat.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      184 2022-10-13 13:02:39.000000 chainlib-0.4.9/chainlib/status.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2188 2023-02-10 19:31:04.000000 chainlib-0.4.9/chainlib/tx.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 10:39:44.006665 chainlib-0.4.9/chainlib.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      726 2023-02-14 10:39:43.000000 chainlib-0.4.9/chainlib.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      903 2023-02-14 10:39:43.000000 chainlib-0.4.9/chainlib.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-02-14 10:39:43.000000 chainlib-0.4.9/chainlib.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       60 2023-02-14 10:39:43.000000 chainlib-0.4.9/chainlib.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       89 2023-02-14 10:39:43.000000 chainlib-0.4.9/chainlib.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-02-14 10:39:43.000000 chainlib-0.4.9/chainlib.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       70 2022-10-13 13:02:39.000000 chainlib-0.4.9/requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-14 10:39:44.006665 chainlib-0.4.9/scripts/
+-rwxr-xr-x   0 lash      (1000) lash      (1000)     7382 2022-11-12 13:17:39.000000 chainlib-0.4.9/scripts/chainlib-man.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      712 2023-02-14 10:39:44.006665 chainlib-0.4.9/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      655 2023-02-14 06:42:51.000000 chainlib-0.4.9/setup.py
```

### Comparing `chainlib-0.4.8/LICENSE` & `chainlib-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/PKG-INFO` & `chainlib-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlib
-Version: 0.4.8
+Version: 0.4.9
 Summary: Generic blockchain access library and tooling
 Home-page: https://git.defalsify.org/chainlib
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainlib-0.4.8/README.md` & `chainlib-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/WAIVER` & `chainlib-0.4.9/WAIVER`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/WAIVER.asc` & `chainlib-0.4.9/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/auth.py` & `chainlib-0.4.9/chainlib/auth.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/block.py` & `chainlib-0.4.9/chainlib/block.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/chain.py` & `chainlib-0.4.9/chainlib/chain.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/cli/arg.py` & `chainlib-0.4.9/chainlib/cli/arg.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/cli/config.py` & `chainlib-0.4.9/chainlib/cli/config.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/cli/gen.py` & `chainlib-0.4.9/chainlib/cli/gen.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/cli/man.py` & `chainlib-0.4.9/chainlib/cli/man.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/cli/rpc.py` & `chainlib-0.4.9/chainlib/cli/rpc.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/cli/wallet.py` & `chainlib-0.4.9/chainlib/cli/wallet.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/connection.py` & `chainlib-0.4.9/chainlib/connection.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/data/env/env.ini` & `chainlib-0.4.9/chainlib/data/env/env.ini`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/encode.py` & `chainlib-0.4.9/chainlib/encode.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/error.py` & `chainlib-0.4.9/chainlib/error.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/hash.py` & `chainlib-0.4.9/chainlib/hash.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/http.py` & `chainlib-0.4.9/chainlib/http.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/interface.py` & `chainlib-0.4.9/chainlib/interface.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/jsonrpc.py` & `chainlib-0.4.9/chainlib/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/runnable/gen.py` & `chainlib-0.4.9/chainlib/runnable/gen.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/settings.py` & `chainlib-0.4.9/chainlib/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -41,15 +41,20 @@
 def process_settings_common(settings, config):
     chain_spec = ChainSpec.from_chain_str(config.get('CHAIN_SPEC'))
     settings.set('CHAIN_SPEC', chain_spec)
     return settings
 
 
 def process_settings_signer_check(settings, config):
-    if config.get('WALLET_KEY_FILE') != None and config.get('_UNSIGNED_SENDER_ADDRESS') != None:
+    unsigned_address = None
+    try:
+        unsigned_address = config.get('_UNSIGNED_SENDER_ADDRESS')
+    except KeyError:
+        pass
+    if config.get('WALLET_KEY_FILE') != None and unsigned_address != None:
         logg.warning('misconfigured client has both wallet key file and signed sender options set')
     return settings
 
 
 def process_settings_value(settings, config):
     value = None
     try:
```

### Comparing `chainlib-0.4.8/chainlib/src.py` & `chainlib-0.4.9/chainlib/src.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/stat.py` & `chainlib-0.4.9/chainlib/stat.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib/tx.py` & `chainlib-0.4.9/chainlib/tx.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/chainlib.egg-info/PKG-INFO` & `chainlib-0.4.9/chainlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlib
-Version: 0.4.8
+Version: 0.4.9
 Summary: Generic blockchain access library and tooling
 Home-page: https://git.defalsify.org/chainlib
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainlib-0.4.8/chainlib.egg-info/SOURCES.txt` & `chainlib-0.4.9/chainlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/scripts/chainlib-man.py` & `chainlib-0.4.9/scripts/chainlib-man.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.4.8/setup.cfg` & `chainlib-0.4.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = chainlib
 license = AGPLv3+
 author_email = dev@holbrook.no
 description = Generic blockchain access library and tooling
-version = 0.4.8
+version = 0.4.9
 url = https://git.defalsify.org/chainlib
 author = Louis Holbrook
 keywords = 
 	dlt
 	blockchain
 	cryptocurrency
 classifiers =
```

### Comparing `chainlib-0.4.8/setup.py` & `chainlib-0.4.9/setup.py`

 * *Files identical despite different names*

