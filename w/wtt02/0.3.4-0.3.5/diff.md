# Comparing `tmp/wtt02-0.3.4.tar.gz` & `tmp/wtt02-0.3.5.tar.gz`

## Comparing `wtt02-0.3.4.tar` & `wtt02-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt02-0.3.4/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt02-0.3.4/tests/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wtt02-0.3.4/tests/test_load.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt02-0.3.4/wtt02/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt02-0.3.4/wtt02/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt02-0.3.4/wtt02/_env.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 wtt02-0.3.4/wtt02/main.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wtt02-0.3.4/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt02-0.3.4/LICENSE.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt02-0.3.4/README.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 wtt02-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt02-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt02-0.3.5/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt02-0.3.5/tests/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wtt02-0.3.5/tests/test_load.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt02-0.3.5/wtt02/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt02-0.3.5/wtt02/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt02-0.3.5/wtt02/_env.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 wtt02-0.3.5/wtt02/main.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wtt02-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt02-0.3.5/LICENSE.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt02-0.3.5/README.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 wtt02-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt02-0.3.5/PKG-INFO
```

### Comparing `wtt02-0.3.4/tests/test_load.py` & `wtt02-0.3.5/tests/test_load.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import wtt02.main as main
 
 HERE = pathlib.Path(__file__).parent
 
 
 def test_load(monkeypatch):
     """Test the extension can be loaded."""
-    monkeypatch.setenv("WTT_02_LICENSE", "test")
+    monkeypatch.setenv("ATOMDB_LICENSE", "test")
 
     con = main.get_connection()
 
     results = con.execute("SELECT calc_exact_mw('c1ccccc1');").fetchall()
     assert len(results) == 1
```

### Comparing `wtt02-0.3.4/wtt02/main.py` & `wtt02-0.3.5/wtt02/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 def get_connection(
     database: str = ":memory:",
     read_only: bool = False,
     config: Optional[dict] = None,
     file_path: Optional[Path] = None,
 ) -> duckdb.DuckDBPyConnection:
     """Return a connection with wtt02 loaded."""
-    if "WTT_02_LICENSE" not in os.environ:
+    if "ATOMDB_LICENSE" not in os.environ:
         raise WTT02ConfigurationException(
-            "WTT_02_LICENSE environment variable not set. "
+            "ATOMDB_LICENSE environment variable not set. "
             "Check the docs or email at help@wheretrue.com"
         )
 
     if config is None:
         config = {"allow_unsigned_extensions": True}
     else:
         config["allow_unsigned_extensions"] = True
```

### Comparing `wtt02-0.3.4/LICENSE.txt` & `wtt02-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wtt02-0.3.4/pyproject.toml` & `wtt02-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wtt02-0.3.4/PKG-INFO` & `wtt02-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtt02
-Version: 0.3.4
+Version: 0.3.5
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

