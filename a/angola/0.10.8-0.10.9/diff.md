# Comparing `tmp/angola-0.10.8.tar.gz` & `tmp/angola-0.10.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.10.8.tar", last modified: Tue Feb 21 03:15:31 2023, max compression
+gzip compressed data, was "angola-0.10.9.tar", last modified: Tue Feb 21 06:27:33 2023, max compression
```

## Comparing `angola-0.10.8.tar` & `angola-0.10.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 03:15:31.311493 angola-0.10.8/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2022-05-25 02:30:17.000000 angola-0.10.8/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.10.8/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-02-21 03:15:31.311547 angola-0.10.8/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.10.8/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-02-21 03:15:31.311767 angola-0.10.8/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-02-21 03:14:33.000000 angola-0.10.8/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 03:15:31.307243 angola-0.10.8/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 03:15:31.309519 angola-0.10.8/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      294 2023-02-05 09:35:54.000000 angola-0.10.8/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    45028 2023-02-21 03:14:28.000000 angola-0.10.8/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    13878 2023-01-21 20:17:47.000000 angola-0.10.8/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.10.8/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    16475 2023-02-02 00:30:34.000000 angola-0.10.8/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    16563 2023-02-21 03:11:29.000000 angola-0.10.8/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 03:15:31.310173 angola-0.10.8/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-02-21 03:15:31.000000 angola-0.10.8/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-02-21 03:15:31.000000 angola-0.10.8/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-02-21 03:15:31.000000 angola-0.10.8/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-02-21 03:15:31.000000 angola-0.10.8/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-02-21 03:15:31.000000 angola-0.10.8/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 03:15:31.311408 angola-0.10.8/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.10.8/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.10.8/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.10.8/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.10.8/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.10.8/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.841214 angola-0.10.9/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2022-05-25 02:30:17.000000 angola-0.10.9/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.10.9/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-02-21 06:27:33.841283 angola-0.10.9/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.10.9/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-02-21 06:27:33.841517 angola-0.10.9/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-02-21 06:26:54.000000 angola-0.10.9/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.835954 angola-0.10.9/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.838616 angola-0.10.9/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      294 2023-02-05 09:35:54.000000 angola-0.10.9/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    45123 2023-02-21 06:18:00.000000 angola-0.10.9/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    13878 2023-01-21 20:17:47.000000 angola-0.10.9/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.10.9/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    16435 2023-02-21 06:17:43.000000 angola-0.10.9/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    16563 2023-02-21 03:11:29.000000 angola-0.10.9/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.839678 angola-0.10.9/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.841113 angola-0.10.9/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.10.9/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.10.9/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.10.9/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.10.9/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.10.9/tests/test_query.py
```

### Comparing `angola-0.10.8/LICENSE` & `angola-0.10.9/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.10.8/PKG-INFO` & `angola-0.10.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.10.8
+Version: 0.10.9
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.10.8/README.md` & `angola-0.10.9/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.10.8/setup.py` & `angola-0.10.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.10.8"
+VERSION = "0.10.9"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.10.8/src/angola/database.py` & `angola-0.10.9/src/angola/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,31 +76,34 @@
     def __getattr__(self, __name: str, *a, **kw):
       return self._item.__getattribute__(__name, *a, **kw)
 
 class QueryResult(object):
     def __init__(self, cursor, pager, data_mapper=None):
         self.cursor = cursor
         stats = cursor.statistics()
-        current_count = self.cursor.count()
-        self.count = stats["fullCount"]
-        self.pagination = lib.gen_pagination(total_count=self.count,
-                                            count=current_count,
+        self.count = self.cursor.count() # current count
+        self.size = stats["fullCount"] # total count
+        self.pagination = lib.gen_pagination(
+                                            size=self.size,
+                                            count=self.count,
                                             page=pager[0],
                                             per_page=pager[1])
 
         def _default_data_mapper_cb(item): return item 
     
         self._data_mapper = _default_data_mapper_cb if not data_mapper else data_mapper
 
     def __iter__(self):
         for item in self.cursor:
             yield self._data_mapper(item)
 
     def __len__(self):
-        return self.count
+        """Get the total count """
+        return self.size
+
 
 class Item_Impl(dict):
     NAMESPACE = None
  
     def _make_path(self, path):
         # if self.NAMESPACE:
         #     return "%s.%s" % (self.NAMESPACE, path)
```

### Comparing `angola-0.10.8/src/angola/dict_mutator.py` & `angola-0.10.9/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.10.8/src/angola/dict_query.py` & `angola-0.10.9/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.10.8/src/angola/lib.py` & `angola-0.10.9/src/angola/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,42 +539,42 @@
         - page:int - the current page
         - per_page:int - items per page
     Returns: int 
     """
     return 0 if page < 1 else (page - 1) * per_page
 
 
-def gen_pagination(total_count: int, count: int, page: int, per_page: int) -> dict:
+def gen_pagination(size: int, count: int, page: int, per_page: int) -> dict:
     """
     Create pagination data based on some basic info
 
     Args:
-        - total_count:int - The total items
+        - size:int - The total items
         - count:int - the current count for the subset
         - page:int - the current page
         - per_page:int - total items per page
 
     Returns: dict
         - page:int - The current page
         - per_page:int - total items per page
-        - count:int - total items
-        - page_count:int - the current count for the page
+        - size:int - total items
+        - count:int - the current count for the page
         - page_showing_start:int|None - data start, ie: showing *1 to 10
         - page_showing_end:int|None - data end, ie: showing 1 to *10
         - total_pages:int - total pages
         - has_prev:bool - If it has prev page
         - prev_page:int|None - the prev page # or None
         - has_next:bool - If it has next page
         - next_page:int|None - the next page # or None
 
     """
     per_page = int(round(per_page))
     if per_page < 1:
         per_page = 10
-    total_pages = math.ceil(total_count / per_page)
+    total_pages = math.ceil(size / per_page)
     page = int(round(page))
     if page < 1:
         page = 1
     elif page > total_pages:
         page = total_pages
     has_prev = page > 1 and page <= total_pages
     has_next = page < total_pages
@@ -584,22 +584,22 @@
     if total_pages == 0:
         page_showing_start = 0
         page_showing_end = 0
         
     return {
         "page": page,
         "per_page": per_page,
-        "count": total_count,
+        "count": count,
+        "size": size,
         "total_pages": total_pages,
         "has_prev": has_prev,
         "prev_page": page - 1 if has_prev else None,
         "has_next": has_next,
         "next_page": page + 1 if has_next else None,
         "last_page": total_pages,
-        "page_count": count,
         "page_showing_start": page_showing_start,
         "page_showing_end": page_showing_end
     }
 
 
 def render_template(source: str, data={}, is_data_flatten=False) -> str:
     """
```

### Comparing `angola-0.10.8/src/angola/lib_xql.py` & `angola-0.10.9/src/angola/lib_xql.py`

 * *Files identical despite different names*

### Comparing `angola-0.10.8/src/angola.egg-info/PKG-INFO` & `angola-0.10.9/src/angola.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.10.8
+Version: 0.10.9
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.10.8/tests/test_database.py` & `angola-0.10.9/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.10.8/tests/test_dict_mutator.py` & `angola-0.10.9/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.10.8/tests/test_lib.py` & `angola-0.10.9/tests/test_lib.py`

 * *Files identical despite different names*

