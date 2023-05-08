# Comparing `tmp/nure-2023.4.30.tar.gz` & `tmp/nure-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nure-2023.4.30.tar", last modified: Sun Apr 30 02:30:15 2023, max compression
+gzip compressed data, was "nure-2023.5.8.tar", last modified: Mon May  8 06:17:02 2023, max compression
```

## Comparing `nure-2023.4.30.tar` & `nure-2023.5.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:15.631868 nure-2023.4.30/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    35149 2021-05-21 04:50:18.000000 nure-2023.4.30/LICENSE
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-04-30 02:30:15.632721 nure-2023.4.30/PKG-INFO
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       30 2021-05-21 04:25:06.000000 nure-2023.4.30/README.md
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:12.644657 nure-2023.4.30/nure/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:41:00.000000 nure-2023.4.30/nure/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2523 2021-11-20 09:30:50.000000 nure-2023.4.30/nure/archive.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2379 2021-11-30 04:05:06.000000 nure-2023.4.30/nure/array.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:12.911885 nure-2023.4.30/nure/code/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       62 2021-07-13 10:11:18.000000 nure-2023.4.30/nure/code/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1353 2021-07-13 16:16:01.000000 nure-2023.4.30/nure/code/label_coder.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     4912 2022-07-29 07:41:08.000000 nure-2023.4.30/nure/dataframe.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1263 2021-07-21 05:24:39.000000 nure-2023.4.30/nure/datetime.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      106 2021-05-21 06:28:06.000000 nure-2023.4.30/nure/debug.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1325 2022-11-14 10:39:27.000000 nure-2023.4.30/nure/dict.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      487 2021-11-30 04:03:48.000000 nure-2023.4.30/nure/func.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:13.560700 nure-2023.4.30/nure/image/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2022-04-14 09:32:11.000000 nure-2023.4.30/nure/image/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    10331 2022-04-14 09:44:09.000000 nure-2023.4.30/nure/image/annotate.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6438 2022-04-14 09:32:48.000000 nure-2023.4.30/nure/image/func.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6060 2023-04-29 16:36:51.000000 nure-2023.4.30/nure/image/pil.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1457 2022-03-22 08:57:21.000000 nure-2023.4.30/nure/meta.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      445 2021-05-21 04:25:40.000000 nure-2023.4.30/nure/path.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:14.592020 nure-2023.4.30/nure/sync/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:53:57.000000 nure-2023.4.30/nure/sync/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      457 2021-05-21 09:16:57.000000 nure-2023.4.30/nure/sync/bigquery.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1628 2021-11-30 04:09:01.000000 nure-2023.4.30/nure/sync/cache.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3249 2021-07-23 06:18:01.000000 nure-2023.4.30/nure/sync/googlesheet.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      706 2021-05-21 09:17:03.000000 nure-2023.4.30/nure/sync/postgre.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3481 2023-04-29 16:38:30.000000 nure-2023.4.30/nure/sync/s3.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1806 2022-09-18 04:11:30.000000 nure-2023.4.30/nure/sync/sql.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1450 2021-09-17 11:26:33.000000 nure-2023.4.30/nure/sync/suffix.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2872 2021-11-05 14:16:28.000000 nure-2023.4.30/nure/volatitle.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:14.982812 nure-2023.4.30/nure.egg-info/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-04-30 02:30:08.000000 nure-2023.4.30/nure.egg-info/PKG-INFO
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      842 2023-04-30 02:30:10.000000 nure-2023.4.30/nure.egg-info/SOURCES.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        1 2023-04-30 02:30:08.000000 nure-2023.4.30/nure.egg-info/dependency_links.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      145 2023-04-30 02:30:09.000000 nure-2023.4.30/nure.egg-info/requires.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        5 2023-04-30 02:30:09.000000 nure-2023.4.30/nure.egg-info/top_level.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      103 2021-05-21 04:28:28.000000 nure-2023.4.30/pyproject.toml
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      849 2023-04-30 02:30:15.644622 nure-2023.4.30/setup.cfg
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:15.560696 nure-2023.4.30/tests/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1011 2021-11-20 09:51:16.000000 nure-2023.4.30/tests/test_archive.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1225 2021-09-17 11:28:32.000000 nure-2023.4.30/tests/test_bigquery.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2890 2021-07-13 16:25:33.000000 nure-2023.4.30/tests/test_coder.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      792 2021-07-23 06:18:01.000000 nure-2023.4.30/tests/test_googlesheet.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3698 2021-11-30 04:05:08.000000 nure-2023.4.30/tests/test_parallel.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      708 2021-09-17 11:49:25.000000 nure-2023.4.30/tests/test_postgre.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      655 2021-10-08 07:11:48.000000 nure-2023.4.30/tests/test_s3.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:17:02.550119 nure-2023.5.8/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    35149 2021-05-21 04:50:18.000000 nure-2023.5.8/LICENSE
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      611 2023-05-08 06:17:02.551459 nure-2023.5.8/PKG-INFO
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       30 2021-05-21 04:25:06.000000 nure-2023.5.8/README.md
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:06.754092 nure-2023.5.8/nure/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:41:00.000000 nure-2023.5.8/nure/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2523 2021-11-20 09:30:50.000000 nure-2023.5.8/nure/archive.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2379 2023-05-08 05:52:06.000000 nure-2023.5.8/nure/array.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:06.792652 nure-2023.5.8/nure/code/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       62 2021-07-13 10:11:18.000000 nure-2023.5.8/nure/code/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1353 2021-07-13 16:16:01.000000 nure-2023.5.8/nure/code/label_coder.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     4912 2022-07-29 07:41:08.000000 nure-2023.5.8/nure/dataframe.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1263 2021-07-21 05:24:39.000000 nure-2023.5.8/nure/datetime.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      106 2021-05-21 06:28:06.000000 nure-2023.5.8/nure/debug.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1416 2023-05-08 06:16:05.000000 nure-2023.5.8/nure/dict.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      487 2021-11-30 04:03:48.000000 nure-2023.5.8/nure/func.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:06.891279 nure-2023.5.8/nure/image/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2022-04-14 09:32:11.000000 nure-2023.5.8/nure/image/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    10331 2022-04-14 09:44:09.000000 nure-2023.5.8/nure/image/annotate.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6438 2022-04-14 09:32:48.000000 nure-2023.5.8/nure/image/func.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6060 2023-04-29 16:36:51.000000 nure-2023.5.8/nure/image/pil.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1457 2022-03-22 08:57:21.000000 nure-2023.5.8/nure/meta.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      445 2021-05-21 04:25:40.000000 nure-2023.5.8/nure/path.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:07.041371 nure-2023.5.8/nure/sync/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:53:57.000000 nure-2023.5.8/nure/sync/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      457 2021-05-21 09:16:57.000000 nure-2023.5.8/nure/sync/bigquery.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1628 2021-11-30 04:09:01.000000 nure-2023.5.8/nure/sync/cache.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3249 2021-07-23 06:18:01.000000 nure-2023.5.8/nure/sync/googlesheet.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      706 2021-05-21 09:17:03.000000 nure-2023.5.8/nure/sync/postgre.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3481 2023-04-29 16:38:30.000000 nure-2023.5.8/nure/sync/s3.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1806 2022-09-18 04:11:30.000000 nure-2023.5.8/nure/sync/sql.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1450 2021-09-17 11:26:33.000000 nure-2023.5.8/nure/sync/suffix.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2872 2021-11-05 14:16:28.000000 nure-2023.5.8/nure/volatitle.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:07.111087 nure-2023.5.8/nure.egg-info/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      611 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/PKG-INFO
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      842 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        1 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      145 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/requires.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        5 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/top_level.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      103 2021-05-21 04:28:28.000000 nure-2023.5.8/pyproject.toml
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      849 2023-05-08 06:17:02.556865 nure-2023.5.8/setup.cfg
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:17:02.532619 nure-2023.5.8/tests/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1011 2021-11-20 09:51:16.000000 nure-2023.5.8/tests/test_archive.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1225 2021-09-17 11:28:32.000000 nure-2023.5.8/tests/test_bigquery.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2890 2021-07-13 16:25:33.000000 nure-2023.5.8/tests/test_coder.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      792 2021-07-23 06:18:01.000000 nure-2023.5.8/tests/test_googlesheet.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3698 2021-11-30 04:05:08.000000 nure-2023.5.8/tests/test_parallel.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      708 2021-09-17 11:49:25.000000 nure-2023.5.8/tests/test_postgre.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      655 2021-10-08 07:11:48.000000 nure-2023.5.8/tests/test_s3.py
```

### Comparing `nure-2023.4.30/LICENSE` & `nure-2023.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/PKG-INFO` & `nure-2023.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2023.4.30
+Version: 2023.5.8
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2023.4.30/nure/archive.py` & `nure-2023.5.8/nure/archive.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/array.py` & `nure-2023.5.8/nure/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import concurrent.futures
 import os
-from collections import Iterable, deque
-from typing import Callable, List
+from collections import deque
+from typing import Callable, Iterable, List
 
 _DEFAULT_N_WORKERS_ = os.cpu_count() or 4
 
 
 def parallelize_iterable(iterable: Iterable, func: Callable, *args, preserve_order=True,
                          executor: concurrent.futures.Executor = None,
                          n_workers: int = _DEFAULT_N_WORKERS_, use_process: bool = False,
```

### Comparing `nure-2023.4.30/nure/code/label_coder.py` & `nure-2023.5.8/nure/code/label_coder.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/dataframe.py` & `nure-2023.5.8/nure/dataframe.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/datetime.py` & `nure-2023.5.8/nure/datetime.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/dict.py` & `nure-2023.5.8/nure/dict.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,34 +6,42 @@
         if isinstance(v, collections.abc.Mapping):
             default[k] = update(default.get(k, {}), v)
         else:
             default[k] = v
     return default
 
 
-def get(obj, key, sep='.', default=None, suppress_error=True):
+def get(obj, key: str, sep='.', default=None, suppress_error=True):
     l_key = key.split(sep)
     for k in l_key:
-        if not isinstance(obj, collections.abc.Mapping) or k not in obj:
-            if suppress_error:
-                return default
+        try:
+            obj = obj[k]
+        except Exception:
+            try:
+                obj = obj[int(k)]
+            except Exception:
+                if suppress_error:
+                    return default
 
-            raise KeyError(f'{k} is not in {obj}')
-        obj = obj[k]
+                raise KeyError(f'{k} is not in {obj}')
 
     return obj
 
 
 def set(obj, key, value, sep='.'):
     l_key = key.split(sep)
     for k in l_key[:-1]:
-        assert isinstance(obj, collections.abc.MutableMapping), ValueError(f'{obj} is not a MutableMapping')
-        if k not in obj:
-            obj[k] = dict()
-        obj = obj[k]
+        try:
+            obj = obj[k]
+        except Exception:
+            try:
+                obj = obj[int(k)]
+            except Exception:
+                obj[k] = dict()
+                obj = obj[k]
 
     obj[l_key[-1]] = value
 
 
 def delete(obj, key, sep='.', suppress_error=False):
     l_key = key.split(sep)
     pre_obj = obj
```

### Comparing `nure-2023.4.30/nure/image/annotate.py` & `nure-2023.5.8/nure/image/annotate.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/image/func.py` & `nure-2023.5.8/nure/image/func.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/image/pil.py` & `nure-2023.5.8/nure/image/pil.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/meta.py` & `nure-2023.5.8/nure/meta.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/sync/cache.py` & `nure-2023.5.8/nure/sync/cache.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/sync/googlesheet.py` & `nure-2023.5.8/nure/sync/googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/sync/postgre.py` & `nure-2023.5.8/nure/sync/postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/sync/s3.py` & `nure-2023.5.8/nure/sync/s3.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/sync/sql.py` & `nure-2023.5.8/nure/sync/sql.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/sync/suffix.py` & `nure-2023.5.8/nure/sync/suffix.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure/volatitle.py` & `nure-2023.5.8/nure/volatitle.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/nure.egg-info/PKG-INFO` & `nure-2023.5.8/nure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2023.4.30
+Version: 2023.5.8
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2023.4.30/nure.egg-info/SOURCES.txt` & `nure-2023.5.8/nure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/setup.cfg` & `nure-2023.5.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nure
-version = 2023.04.30
+version = 2023.05.08
 author = Trung Tran
 author_email = tranduytrung@outlook.com
 description = Data Science Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tranduytrung/nure
 project_urls =
```

### Comparing `nure-2023.4.30/tests/test_archive.py` & `nure-2023.5.8/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/tests/test_bigquery.py` & `nure-2023.5.8/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/tests/test_coder.py` & `nure-2023.5.8/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/tests/test_googlesheet.py` & `nure-2023.5.8/tests/test_googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/tests/test_parallel.py` & `nure-2023.5.8/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/tests/test_postgre.py` & `nure-2023.5.8/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.30/tests/test_s3.py` & `nure-2023.5.8/tests/test_s3.py`

 * *Files identical despite different names*

