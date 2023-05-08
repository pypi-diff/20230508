# Comparing `tmp/yuna-db-0.2.2.tar.gz` & `tmp/yuna-db-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuna-db-0.2.2.tar", last modified: Wed May  3 00:03:14 2023, max compression
+gzip compressed data, was "yuna-db-0.2.3.tar", last modified: Mon May  8 07:33:07 2023, max compression
```

## Comparing `yuna-db-0.2.2.tar` & `yuna-db-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.2.2/LICENSE
--rw-r--r--   0        0        0     1579 2023-04-27 18:41:03.641249 yuna-db-0.2.2/README.md
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.2/__init__.py
--rwxr-xr-x   0        0        0     3472 2023-05-03 00:01:55.987176 yuna-db-0.2.2/example.py
--rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.2.2/requirements.txt
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.2/src/__init__.py
--rw-r--r--   0        0        0    15394 2023-05-02 23:16:33.172343 yuna-db-0.2.2/src/yuna/__init__.py
--rw-r--r--   0        0        0     8917 2023-05-02 19:00:09.307489 yuna-db-0.2.2/src/yuna/lmdb_util.py
--rw-r--r--   0        0        0    31423 2023-05-03 00:01:23.886587 yuna-db-0.2.2/src/yuna/plugins.py
--rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.2.2/tests/__init__.py
--rwxr-xr-x   0        0        0     9470 2023-05-02 23:48:28.489421 yuna-db-0.2.2/tests/test_yuna.py
--rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.2.2/version.txt
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 yuna-db-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1615 2023-05-08 07:27:32.741832 yuna-db-0.2.3/README.md
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.3/__init__.py
+-rwxr-xr-x   0        0        0     3470 2023-05-08 07:32:52.780510 yuna-db-0.2.3/example.py
+-rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.2.3/requirements.txt
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.3/src/__init__.py
+-rw-r--r--   0        0        0    26645 2023-05-08 07:24:34.918122 yuna-db-0.2.3/src/yuna/__init__.py
+-rw-r--r--   0        0        0     8915 2023-05-08 05:34:13.855559 yuna-db-0.2.3/src/yuna/lmdb_util.py
+-rw-r--r--   0        0        0    31439 2023-05-08 06:49:57.398627 yuna-db-0.2.3/src/yuna/plugins.py
+-rwxr-xr-x   0        0        0     1066 2023-05-08 05:37:29.051656 yuna-db-0.2.3/src/yuna/yuna_repack
+-rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.2.3/tests/__init__.py
+-rwxr-xr-x   0        0        0     9470 2023-05-02 23:48:28.489421 yuna-db-0.2.3/tests/test_yuna.py
+-rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.2.3/version.txt
+-rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 yuna-db-0.2.3/PKG-INFO
```

### Comparing `yuna-db-0.2.2/LICENSE` & `yuna-db-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yuna-db-0.2.2/README.md` & `yuna-db-0.2.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 
 # Example
 
 ```
 from yuna import Yuna, SERIALIZE_JSON, SERIALIZE_STR
 
 with Yuna("/tmp/test.ydb", create=True) as db:
-	db.new_table("names", serialize=SERIALIZE_JSON)
+    db.new_table("names", serialize=SERIALIZE_JSON)
 
-	key = "feynman"
-	value = dict(first_name="Richard", last_name="Feynman")
-	db.tables.names.put(key, value)
-
-	temp = db.tables.names.get(key)
-	assert temp == value
-
-	db.new_table("abbrevs", serialize=SERIALIZE_STR)
-	key = "l8r"
-	value = "see you later"
-
-	db.tables.abbrevs.put(key, value)
-	temp = db.tables.abbrevs.get(key)
-	assert temp == value
+    key = "feynman"
+    value = dict(first_name="Richard", last_name="Feynman")
+    db.tables.names.put(key, value)
+
+    temp = db.tables.names.get(key)
+    assert temp == value
+
+    db.new_table("abbrevs", serialize=SERIALIZE_STR)
+    key = "l8r"
+    value = "see you later"
+
+    db.tables.abbrevs.put(key, value)
+    temp = db.tables.abbrevs.get(key)
+    assert temp == value
 ```
 
 # Planned new features to come:
 
 * Support integer keys with a .insert() method providing autoincrement
 * Finish the Zstandard compression support
 * Add docstrings to the iterators
```

### Comparing `yuna-db-0.2.2/example.py` & `yuna-db-0.2.3/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 # Hack sys.path so that this file will run against Yuna from this directory tree,
 # even if someone ran "pip install yuna-db" before running this.
 THIS_DIR = os.path.dirname(os.path.abspath(__file__))
 sys.path.insert(0, os.path.abspath(os.path.join(THIS_DIR, "src")))
 
 import yuna
 from yuna import Yuna
-from yuna.lmdb_util import _delete_file_or_dir
+from yuna.lmdb_util import delete_file_or_dir
 
 TEST_FILE = "/tmp/junk.ydb"
 
-_delete_file_or_dir(TEST_FILE)
+delete_file_or_dir(TEST_FILE)
 with Yuna(TEST_FILE, "test", 1, create=True) as db:
     db.new_table("a26", serialize=yuna.SERIALIZE_STR, compress=yuna.COMPRESS_LZ4)
     tbl_a26 = db.tables.a26
     tbl_a26.put("a", "1")
     tbl_a26.put("b", "2")
     #tbl_a26.put("c", "3")
     tbl_a26.put("d", "4")
```

### Comparing `yuna-db-0.2.2/src/yuna/lmdb_util.py` & `yuna-db-0.2.3/src/yuna/lmdb_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 YUNA_DEFAULT_MAX_TABLES = 100
 YUNA_DEFAULT_MAX_DB_SIZE = 2**40  # one tebibyte (binary terabyte): 1024**4
 
 _VALID_SAFETY_MODES = ('a', 'u')
 
 
-def _delete_file_or_dir(fname: str):
+def delete_file_or_dir(fname: str):
     # If it doesn't exist, we don't complain, similar to /bin/rm -f on Linux
     if not os.path.exists(fname):
         return
 
     # Something exists; delete it whether it is a file or a directory.
     try:
         os.remove(fname)
@@ -274,15 +274,15 @@
 
         if not os.path.exists(fname):
             raise FileNotFoundError(fname)
 
     # Create implies we want to be able to write.  Don't even check it, just make sure read_only is False.
     if create:
         read_only = False
-        _delete_file_or_dir(fname)
+        delete_file_or_dir(fname)
 
     try:
         kwargs = {
             "create": create,
             "map_size": max_db_file_size,
             "max_dbs": max_tables,
             "readonly": read_only,
```

### Comparing `yuna-db-0.2.2/src/yuna/plugins.py` & `yuna-db-0.2.3/src/yuna/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,15 @@
 ) -> Callable:
     key_plugins = get_serialize_plugins(key_serialize_tag)
     fn_key_serialize = key_plugins.serialize if key_plugins else _return_bytes_unchanged
 
     value_plugins = get_serialize_plugins(value_serialize_tag)
     fn_value_deserialize = value_plugins.deserialize
 
-    def get(self, key: str, default: object=_YUNA_NOT_PROVIDED) -> object:
+    def get(self, key: str, default: Any=_YUNA_NOT_PROVIDED) -> Any:
         bytes_key = fn_key_serialize(key)
         result = _lmdb_table_get(env, table, bytes_key, None)
         if result is None:
             if default is _YUNA_NOT_PROVIDED:
                 raise KeyError(key)
             else:
                 return default
@@ -314,15 +314,15 @@
 ) -> Callable:
     key_plugins = get_serialize_plugins(key_serialize_tag)
     fn_key_serialize = key_plugins.serialize if key_plugins else _return_bytes_unchanged
 
     value_plugins = get_compress_plugins(value_compress_tag)
     fn_value_decompress = value_plugins.decompress
 
-    def get(self, key: str, default: object=_YUNA_NOT_PROVIDED) -> object:
+    def get(self, key: str, default: Any=_YUNA_NOT_PROVIDED) -> Any:
         bytes_key = fn_key_serialize(key)
         result = _lmdb_table_get(env, table, bytes_key, None)
         if result is None:
             if default is _YUNA_NOT_PROVIDED:
                 raise KeyError(key)
             else:
                 return default
@@ -341,15 +341,15 @@
 
     value_serialize_plugins = get_serialize_plugins(value_serialize_tag)
     fn_value_deserialize = value_serialize_plugins.deserialize
 
     value_compress_plugins = get_compress_plugins(value_compress_tag)
     fn_value_decompress = value_compress_plugins.decompress
 
-    def get(self, key: str, default: object=_YUNA_NOT_PROVIDED) -> object:
+    def get(self, key: str, default: Any=_YUNA_NOT_PROVIDED) -> Any:
         bytes_key = fn_key_serialize(key)
         result = _lmdb_table_get(env, table, bytes_key, None)
         if result is None:
             if default is _YUNA_NOT_PROVIDED:
                 raise KeyError(key)
             else:
                 return default
@@ -397,15 +397,15 @@
 ) -> Callable:
     key_plugins = get_serialize_plugins(key_serialize_tag)
     fn_key_serialize = key_plugins.serialize if key_plugins else _return_bytes_unchanged
 
     value_plugins = get_serialize_plugins(value_serialize_tag)
     fn_value_serialize = value_plugins.serialize
 
-    def put(self, key: str, value: object) -> object:
+    def put(self, key: str, value: Any) -> None:
         bytes_key = fn_key_serialize(key)
         bytes_value = fn_value_serialize(value)
         _lmdb_table_put(env, table, bytes_key, bytes_value)
     return put
 
 def _put_table_compress_factory(
     env: lmdb.Environment,
@@ -415,15 +415,15 @@
 ) -> Callable:
     key_plugins = get_serialize_plugins(key_serialize_tag)
     fn_key_serialize = key_plugins.serialize if key_plugins else _return_bytes_unchanged
 
     value_plugins = get_compress_plugins(value_compress_tag)
     fn_value_compress = value_plugins.compress
 
-    def put(self, key: str, value: object) -> object:
+    def put(self, key: str, value: Any) -> None:
         bytes_key = fn_key_serialize(key)
         bytes_value = fn_value_compress(result)
         _lmdb_table_put(env, table, bytes_key, bytes_value)
     return put
 
 def _put_table_serialize_compress_factory(
     env: lmdb.Environment,
@@ -437,15 +437,15 @@
 
     value_serialize_plugins = get_serialize_plugins(value_serialize_tag)
     fn_value_serialize = value_serialize_plugins.serialize
 
     value_compress_plugins = get_compress_plugins(value_compress_tag)
     fn_value_compress = value_compress_plugins.compress
 
-    def put(self, key: str, value: object) -> object:
+    def put(self, key: str, value: Any) -> None:
         bytes_key = fn_key_serialize(key)
         bytes_value = fn_value_compress(fn_value_serialize(value))
         _lmdb_table_put(env, table, bytes_key, bytes_value)
     return put
 
 def put_factory(
     env: lmdb.Environment,
@@ -476,14 +476,15 @@
 
     def delete(self, key: str) -> None:
         bytes_key = fn_key_serialize(key)
         _lmdb_table_delete(env, table, bytes_key)
     return delete
 
 
+# TODO: change the types on keys from str to Any
 def keys_factory(
     env: lmdb.Environment,
     table: lmdb._Database,
     key_serialize_tag: Optional[str]
 ) -> Callable:
     key_plugins = get_serialize_plugins(key_serialize_tag)
     fn_key_serialize = key_plugins.serialize if key_plugins else _return_bytes_unchanged
```

### Comparing `yuna-db-0.2.2/tests/test_yuna.py` & `yuna-db-0.2.3/tests/test_yuna.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.2.2/PKG-INFO` & `yuna-db-0.2.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuna-db
-Version: 0.2.2
+Version: 0.2.3
 Summary: Yuna DB: dict-like semantics for LMDB
 Author-email: "Steve R. Hastings" <steve@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: lmdb >=1.4.1,<2
 
@@ -32,30 +32,30 @@
 
 # Example
 
 ```
 from yuna import Yuna, SERIALIZE_JSON, SERIALIZE_STR
 
 with Yuna("/tmp/test.ydb", create=True) as db:
-	db.new_table("names", serialize=SERIALIZE_JSON)
+    db.new_table("names", serialize=SERIALIZE_JSON)
 
-	key = "feynman"
-	value = dict(first_name="Richard", last_name="Feynman")
-	db.tables.names.put(key, value)
-
-	temp = db.tables.names.get(key)
-	assert temp == value
-
-	db.new_table("abbrevs", serialize=SERIALIZE_STR)
-	key = "l8r"
-	value = "see you later"
-
-	db.tables.abbrevs.put(key, value)
-	temp = db.tables.abbrevs.get(key)
-	assert temp == value
+    key = "feynman"
+    value = dict(first_name="Richard", last_name="Feynman")
+    db.tables.names.put(key, value)
+
+    temp = db.tables.names.get(key)
+    assert temp == value
+
+    db.new_table("abbrevs", serialize=SERIALIZE_STR)
+    key = "l8r"
+    value = "see you later"
+
+    db.tables.abbrevs.put(key, value)
+    temp = db.tables.abbrevs.get(key)
+    assert temp == value
 ```
 
 # Planned new features to come:
 
 * Support integer keys with a .insert() method providing autoincrement
 * Finish the Zstandard compression support
 * Add docstrings to the iterators
```

