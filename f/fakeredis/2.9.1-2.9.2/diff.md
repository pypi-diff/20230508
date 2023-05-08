# Comparing `tmp/fakeredis-2.9.1.tar.gz` & `tmp/fakeredis-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakeredis-2.9.1.tar", max compression
+gzip compressed data, was "fakeredis-2.9.2.tar", max compression
```

## Comparing `fakeredis-2.9.1.tar` & `fakeredis-2.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1571 2023-02-20 14:40:57.808951 fakeredis-2.9.1/LICENSE
--rw-r--r--   0        0        0     1728 2023-02-20 14:40:57.808951 fakeredis-2.9.1/README.md
--rw-r--r--   0        0        0      384 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/__init__.py
--rw-r--r--   0        0        0    11770 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/_basefakesocket.py
--rw-r--r--   0        0        0     4467 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/_command_args_parsing.py
--rw-r--r--   0        0        0    13701 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/_commands.py
--rw-r--r--   0        0        0     1402 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/_fakesocket.py
--rw-r--r--   0        0        0     6864 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/_helpers.py
--rw-r--r--   0        0        0     4340 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/_msgs.py
--rw-r--r--   0        0        0     6901 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/_server.py
--rw-r--r--   0        0        0     3293 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/_stream.py
--rw-r--r--   0        0        0     2690 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/_zset.py
--rw-r--r--   0        0        0     8353 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/aioredis.py
--rw-r--r--   0        0        0        0 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/__init__.py
--rw-r--r--   0        0        0     5476 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/bitmap_mixin.py
--rw-r--r--   0        0        0      835 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/connection_mixin.py
--rw-r--r--   0        0        0     8904 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/generic_mixin.py
--rw-r--r--   0        0        0     2859 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/hash_mixin.py
--rw-r--r--   0        0        0     7230 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/list_mixin.py
--rw-r--r--   0        0        0     5237 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/pubsub_mixin.py
--rw-r--r--   0        0        0    10053 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/scripting_mixin.py
--rw-r--r--   0        0        0     1809 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/server_mixin.py
--rw-r--r--   0        0        0     6324 2023-02-20 14:40:57.808951 fakeredis-2.9.1/fakeredis/commands_mixins/set_mixin.py
--rw-r--r--   0        0        0    16229 2023-02-20 14:40:57.812951 fakeredis-2.9.1/fakeredis/commands_mixins/sortedset_mixin.py
--rw-r--r--   0        0        0     2987 2023-02-20 14:40:57.812951 fakeredis-2.9.1/fakeredis/commands_mixins/streams_mixin.py
--rw-r--r--   0        0        0     9465 2023-02-20 14:40:57.812951 fakeredis-2.9.1/fakeredis/commands_mixins/string_mixin.py
--rw-r--r--   0        0        0     2963 2023-02-20 14:40:57.812951 fakeredis-2.9.1/fakeredis/commands_mixins/transactions_mixin.py
--rw-r--r--   0        0        0        0 2023-02-20 14:40:57.812951 fakeredis-2.9.1/fakeredis/py.typed
--rw-r--r--   0        0        0      322 2023-02-20 14:40:57.812951 fakeredis-2.9.1/fakeredis/stack/__init__.py
--rw-r--r--   0        0        0    16009 2023-02-20 14:40:57.812951 fakeredis-2.9.1/fakeredis/stack/_json_mixin.py
--rw-r--r--   0        0        0     2386 2023-02-20 14:40:57.812951 fakeredis-2.9.1/pyproject.toml
--rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 fakeredis-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1571 2023-02-20 17:17:34.706755 fakeredis-2.9.2/LICENSE
+-rw-r--r--   0        0        0     1728 2023-02-20 17:17:34.706755 fakeredis-2.9.2/README.md
+-rw-r--r--   0        0        0      384 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/__init__.py
+-rw-r--r--   0        0        0    11770 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/_basefakesocket.py
+-rw-r--r--   0        0        0     4467 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/_command_args_parsing.py
+-rw-r--r--   0        0        0    13701 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/_commands.py
+-rw-r--r--   0        0        0     1402 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/_fakesocket.py
+-rw-r--r--   0        0        0     6864 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/_helpers.py
+-rw-r--r--   0        0        0     4340 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/_msgs.py
+-rw-r--r--   0        0        0     6901 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/_server.py
+-rw-r--r--   0        0        0     3322 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/_stream.py
+-rw-r--r--   0        0        0     2690 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/_zset.py
+-rw-r--r--   0        0        0     8353 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/aioredis.py
+-rw-r--r--   0        0        0        0 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/commands_mixins/__init__.py
+-rw-r--r--   0        0        0     5476 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/commands_mixins/bitmap_mixin.py
+-rw-r--r--   0        0        0      835 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/commands_mixins/connection_mixin.py
+-rw-r--r--   0        0        0     8904 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/commands_mixins/generic_mixin.py
+-rw-r--r--   0        0        0     2859 2023-02-20 17:17:34.706755 fakeredis-2.9.2/fakeredis/commands_mixins/hash_mixin.py
+-rw-r--r--   0        0        0     7230 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/commands_mixins/list_mixin.py
+-rw-r--r--   0        0        0     5237 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/commands_mixins/pubsub_mixin.py
+-rw-r--r--   0        0        0    10053 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/commands_mixins/scripting_mixin.py
+-rw-r--r--   0        0        0     1809 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/commands_mixins/server_mixin.py
+-rw-r--r--   0        0        0     6324 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/commands_mixins/set_mixin.py
+-rw-r--r--   0        0        0    16229 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/commands_mixins/sortedset_mixin.py
+-rw-r--r--   0        0        0     2987 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/commands_mixins/streams_mixin.py
+-rw-r--r--   0        0        0     9465 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/commands_mixins/string_mixin.py
+-rw-r--r--   0        0        0     2963 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/commands_mixins/transactions_mixin.py
+-rw-r--r--   0        0        0        0 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/py.typed
+-rw-r--r--   0        0        0      322 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/stack/__init__.py
+-rw-r--r--   0        0        0    16009 2023-02-20 17:17:34.710755 fakeredis-2.9.2/fakeredis/stack/_json_mixin.py
+-rw-r--r--   0        0        0     2386 2023-02-20 17:17:34.710755 fakeredis-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 fakeredis-2.9.2/PKG-INFO
```

### Comparing `fakeredis-2.9.1/LICENSE` & `fakeredis-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/README.md` & `fakeredis-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/_basefakesocket.py` & `fakeredis-2.9.2/fakeredis/_basefakesocket.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/_command_args_parsing.py` & `fakeredis-2.9.2/fakeredis/_command_args_parsing.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/_commands.py` & `fakeredis-2.9.2/fakeredis/_commands.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/_fakesocket.py` & `fakeredis-2.9.2/fakeredis/_fakesocket.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/_helpers.py` & `fakeredis-2.9.2/fakeredis/_helpers.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/_msgs.py` & `fakeredis-2.9.2/fakeredis/_msgs.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/_server.py` & `fakeredis-2.9.2/fakeredis/_server.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/_stream.py` & `fakeredis-2.9.2/fakeredis/_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
     def find_index(self, id_str: str) -> Tuple[int, bool]:
         ts_seq = StreamRangeTest.parse_id(id_str)
         ind = bisect.bisect_left(list(map(lambda x: x[0], self._values)), ts_seq)
         return ind, self._values[ind][0] == ts_seq
 
     @staticmethod
     def _format_record(record):
-        return [f'{record[0][0]}-{record[0][1]}'.encode(), list(record[1:])]
+        results = list(record[1:][0])
+        return [f'{record[0][0]}-{record[0][1]}'.encode(), results]
 
     def trim(self,
              maxlen: Optional[int] = None,
              minid: Optional[str] = None,
              limit: Optional[int] = None) -> int:
         if maxlen is not None and minid is not None:
             raise
```

### Comparing `fakeredis-2.9.1/fakeredis/_zset.py` & `fakeredis-2.9.2/fakeredis/_zset.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/aioredis.py` & `fakeredis-2.9.2/fakeredis/aioredis.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/bitmap_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/bitmap_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/connection_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/connection_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/generic_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/generic_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/hash_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/hash_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/list_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/list_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/pubsub_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/pubsub_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/scripting_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/scripting_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/server_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/server_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/set_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/set_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/sortedset_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/sortedset_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/streams_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/streams_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/string_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/string_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/commands_mixins/transactions_mixin.py` & `fakeredis-2.9.2/fakeredis/commands_mixins/transactions_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/fakeredis/stack/_json_mixin.py` & `fakeredis-2.9.2/fakeredis/stack/_json_mixin.py`

 * *Files identical despite different names*

### Comparing `fakeredis-2.9.1/pyproject.toml` & `fakeredis-2.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 [tool.poetry]
 name = "fakeredis"
 packages = [
     { include = "fakeredis" },
 ]
-version = "2.9.1"
+version = "2.9.2"
 description = "Fake implementation of redis API for testing purposes."
 readme = "README.md"
 keywords = ["redis", "rq", "django-rq", "RedisJson", ]
 authors = [
     "Daniel Moran <daniel.maruani@gmail.com>",
     "Bruce Merry <bmerry@ska.ac.za>",
     "James Saryerwinnie <js@jamesls.com>",
```

### Comparing `fakeredis-2.9.1/PKG-INFO` & `fakeredis-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakeredis
-Version: 2.9.1
+Version: 2.9.2
 Summary: Fake implementation of redis API for testing purposes.
 Home-page: https://github.com/cunla/fakeredis-py
 License: BSD-3-Clause
 Keywords: redis,rq,django-rq,RedisJson
 Author: Daniel Moran
 Author-email: daniel.maruani@gmail.com
 Maintainer: Daniel Moran
```

