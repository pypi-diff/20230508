# Comparing `tmp/kopia-0.1.4.tar.gz` & `tmp/kopia-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kopia-0.1.4.tar", max compression
+gzip compressed data, was "kopia-0.1.5.tar", max compression
```

## Comparing `kopia-0.1.4.tar` & `kopia-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      715 2023-05-08 10:15:22.340948 kopia-0.1.4/README.md
--rw-r--r--   0        0        0       22 2023-05-08 11:30:46.846593 kopia-0.1.4/kopia/__init__.py
--rw-r--r--   0        0        0      238 2023-04-04 18:02:57.290510 kopia-0.1.4/kopia/main.py
--rw-r--r--   0        0        0        0 2023-04-04 14:14:07.117800 kopia-0.1.4/kopia/mysqlc/__init__.py
--rw-r--r--   0        0        0     1406 2023-05-08 11:30:19.602874 kopia-0.1.4/kopia/mysqlc/app.py
--rw-r--r--   0        0        0        0 2023-04-04 14:15:33.606873 kopia-0.1.4/kopia/sqlite/__init__.py
--rw-r--r--   0        0        0      926 2023-05-08 11:21:47.806372 kopia-0.1.4/kopia/sqlite/app.py
--rw-r--r--   0        0        0      590 2023-05-08 11:30:49.954222 kopia-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 kopia-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      715 2023-05-08 10:15:22.340948 kopia-0.1.5/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 11:33:15.595821 kopia-0.1.5/kopia/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-04 18:02:57.290510 kopia-0.1.5/kopia/main.py
+-rw-r--r--   0        0        0        0 2023-04-04 14:14:07.117800 kopia-0.1.5/kopia/mysqlc/__init__.py
+-rw-r--r--   0        0        0     1412 2023-05-08 11:33:01.406782 kopia-0.1.5/kopia/mysqlc/app.py
+-rw-r--r--   0        0        0        0 2023-04-04 14:15:33.606873 kopia-0.1.5/kopia/sqlite/__init__.py
+-rw-r--r--   0        0        0      926 2023-05-08 11:21:47.806372 kopia-0.1.5/kopia/sqlite/app.py
+-rw-r--r--   0        0        0      590 2023-05-08 11:33:15.595726 kopia-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 kopia-0.1.5/PKG-INFO
```

### Comparing `kopia-0.1.4/README.md` & `kopia-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kopia-0.1.4/kopia/mysqlc/app.py` & `kopia-0.1.5/kopia/mysqlc/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         # Create a cursor object
         cursor = connection.cursor()
 
         # Execute the mysqldump command
 
         cursor.execute(
             "mysqldump"
-            f" --user {user}" if user else ""
-            f" --password {password}" if password else ""
-            f" --host {host}" if host else ""
+            f" --user='{user}'" if user else ""
+            f" --password='{password}'" if password else ""
+            f" --host='{host}'" if host else ""
             f" {database} > {output_file}"
         )
 
         # Close the cursor and connection
         cursor.close()
         connection.close()
```

### Comparing `kopia-0.1.4/kopia/sqlite/app.py` & `kopia-0.1.5/kopia/sqlite/app.py`

 * *Files identical despite different names*

### Comparing `kopia-0.1.4/pyproject.toml` & `kopia-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kopia"
-version = "0.1.4"
+version = "0.1.5"
 description = "CLI for creating database dumps"
 authors = ["Rasmus Nathanson <rasmus.nathanson@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 kopia = "kopia.main:app"
```

### Comparing `kopia-0.1.4/PKG-INFO` & `kopia-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kopia
-Version: 0.1.4
+Version: 0.1.5
 Summary: CLI for creating database dumps
 Author: Rasmus Nathanson
 Author-email: rasmus.nathanson@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

