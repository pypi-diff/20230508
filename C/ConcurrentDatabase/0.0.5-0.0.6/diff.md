# Comparing `tmp/ConcurrentDatabase-0.0.5.tar.gz` & `tmp/ConcurrentDatabase-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConcurrentDatabase-0.0.5.tar", last modified: Sat May  6 21:49:01 2023, max compression
+gzip compressed data, was "ConcurrentDatabase-0.0.6.tar", last modified: Mon May  8 20:49:37 2023, max compression
```

## Comparing `ConcurrentDatabase-0.0.5.tar` & `ConcurrentDatabase-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/ConcurrentDatabase/
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/ColumnWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/Database.py
--rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/DynamicEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/DynamicTable.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-06 21:49:01.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-06 21:49:01.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:49:01.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-06 21:49:01.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:49:37.369824 ConcurrentDatabase-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:49:37.369824 ConcurrentDatabase-0.0.6/ConcurrentDatabase/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-08 20:49:26.000000 ConcurrentDatabase-0.0.6/ConcurrentDatabase/ColumnWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14289 2023-05-08 20:49:26.000000 ConcurrentDatabase-0.0.6/ConcurrentDatabase/Database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-05-08 20:49:26.000000 ConcurrentDatabase-0.0.6/ConcurrentDatabase/DynamicEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-05-08 20:49:26.000000 ConcurrentDatabase-0.0.6/ConcurrentDatabase/DynamicTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 20:49:26.000000 ConcurrentDatabase-0.0.6/ConcurrentDatabase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:49:37.369824 ConcurrentDatabase-0.0.6/ConcurrentDatabase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-08 20:49:37.000000 ConcurrentDatabase-0.0.6/ConcurrentDatabase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 20:49:37.000000 ConcurrentDatabase-0.0.6/ConcurrentDatabase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:49:37.000000 ConcurrentDatabase-0.0.6/ConcurrentDatabase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-08 20:49:37.000000 ConcurrentDatabase-0.0.6/ConcurrentDatabase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-08 20:49:37.369824 ConcurrentDatabase-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-08 20:49:26.000000 ConcurrentDatabase-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-08 20:49:26.000000 ConcurrentDatabase-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:49:37.369824 ConcurrentDatabase-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-08 20:49:26.000000 ConcurrentDatabase-0.0.6/setup.py
```

### Comparing `ConcurrentDatabase-0.0.5/ConcurrentDatabase/ColumnWrapper.py` & `ConcurrentDatabase-0.0.6/ConcurrentDatabase/ColumnWrapper.py`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.5/ConcurrentDatabase/Database.py` & `ConcurrentDatabase-0.0.6/ConcurrentDatabase/Database.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,18 @@
         self.child_key.attach_linked_table(self.parent_table, self.parent_key, child=True)
         self.parent_key.attach_linked_table(self.child_table, self.child_key)
 
         self.child_table.parent_tables.append(self.parent_table)
         self.parent_table.child_tables.append(self.child_table)
 
     def has_link(self, table1, table2):
-        return (self.parent_table == table1 and self.child_table == table2) or \
-               (self.child_table == table1 and self.parent_table == table2)
+        return (self.parent_table.table_name == table1.table_name and
+                self.child_table.table_name == table2.table_name) or \
+               (self.child_table.table_name == table1.table_name and
+                self.parent_table.table_name == table2.table_name)
 
     def get_foreign_key(self, table):
         if table == self.parent_table:
             return self.parent_key, self.child_key
         elif table == self.child_table:
             return self.child_key, self.parent_key
         else:
@@ -210,15 +212,16 @@
         # Check if the revision increment is only 1 more than the current version
         elif self.table_version_table.get_row(table_name=table_name)["version"] + 1 != version:
             raise ValueError(f"Table {table_name} version {version} is not 1 more than the current version "
                              f"{self.table_version_table.get_row(table_name=table_name)['version']}")
         # Check if the table exists
         if table_name not in self.tables:
             raise KeyError(f"Table {table_name} not found in database {self.database_name}")
-
+        logging.info(f"Upgrading table {table_name}"
+                     f" {self.table_version_table.get_row(table_name=table_name)['version']} -> {version}")
         # Update the table
         if update_query:
             for query in update_query:
                 self.run(query)
 
             # Update the table version
             self.table_version_table.update_or_add(table_name=table_name, version=version)
@@ -271,15 +274,15 @@
                     logging.error(f"Database Error: Commit failed {e}")
             self.lock.release()
         return cursor
 
     def batch_transaction(self, transactions: list, *args, **kwargs) -> sqlite3.Cursor:
         """
         Run a batch of queries on the database with thread safety.
-        :param sql: The SQL queries to run.
+        :param transactions: The SQL queries to run.
         :param args: The arguments to pass to the query.
         :param kwargs: The keyword arguments to pass to the query.
         :return: A cursor object, use cursor.fetchall() to get the results. (The cursor is not thread safe)
         """
         if not self.open:
             raise RuntimeError("Database is not open")
         self.lock.acquire(timeout=5)
```

### Comparing `ConcurrentDatabase-0.0.5/ConcurrentDatabase/DynamicEntry.py` & `ConcurrentDatabase-0.0.6/ConcurrentDatabase/DynamicEntry.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         self.table = table
         self.database = table.database
         self.primary_keys = table.primary_keys
         self._rowid = None
         self._values = {}
         self._previous_values = {}
         self._dirty = False
+        self._deleted = False
 
         if load_tuple is not None:
             for i in range(len(load_tuple)):
                 if i < len(self.columns):
                     self._values[self.columns[i].name] = load_tuple[i]
 
         for key in kwargs:
@@ -175,15 +176,15 @@
     def delete(self):
         """
         Deletes the entry from the database
         :return:
         """
         primary_key_values = [self._values[column.name] for column in self.columns if column.primary_key]
         sql = f"DELETE FROM {self.table.table_name} WHERE {self._entry_where_clause()}"
-        self.database.run(sql, tuple(primary_key_values))
+        result = self.database.run(sql, primary_key_values)
         del self
 
     def is_dirty(self):
         return self._dirty
 
     def _entry_where_clause(self):
         """
@@ -273,9 +274,9 @@
         else:
             raise TypeError(f"Cannot compare DynamicEntry to {type(other)}")
 
     def __del__(self):
         """
         Called when the DynamicEntry object is garbage collected, flushes the entry to the database to prevent data loss
         """
-        if self._dirty:
+        if self._dirty and not self._deleted:
             self.flush()
```

### Comparing `ConcurrentDatabase-0.0.5/ConcurrentDatabase/DynamicTable.py` & `ConcurrentDatabase-0.0.6/ConcurrentDatabase/DynamicTable.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     def get_row(self, **kwargs) -> typing.Optional[DynamicEntry]:
         """
         Get a row from the table.
         :param kwargs: The filters to apply to the query.
         :return: The row.
         """
         self._validate_columns(**kwargs)
-        self._contains_primary_keys(**kwargs)
+        # self._contains_primary_keys(**kwargs)
 
         # Check if the DynamicEntry is already loaded
         for entry in self.entries:
             if entry == kwargs:
                 return entry
 
         # Build the query
@@ -144,14 +144,16 @@
         :return: The rows.
         """
         db_load = self.database.get(f"SELECT * FROM {self.table_name} ORDER BY rowid {'DESC' if reverse else 'ASC'}")
         if db_load:  # Append any new entries to self.entries and don't overwrite pre-existing entries
             for entry in self.entries:
                 if entry not in db_load:
                     db_load.append(entry)
+            new_entries = [DynamicEntry(self, load_tuple=row) for row in db_load]
+            self.entries.extend(new_entries)
             return self.entries
         else:
             return []
 
     def get_related_entries(self, entry: DynamicEntry) -> List[DynamicEntry]:
         """
         Get all entries that reference the given entry in this table.
@@ -219,15 +221,15 @@
         """
         Add a row to the table.
         :param kwargs: The values of the entry
         :return: A DynamicEntry object representing the row.
         """
         # For each column validate that it is a valid column
         self._validate_columns(**kwargs)
-        self._contains_primary_keys(**kwargs)
+        # self._contains_primary_keys(**kwargs)
 
         # Build the query
         sql = f"INSERT INTO {self.table_name} ("
         for column in kwargs:
             sql += f"{column}, "
         sql = sql[:-2] + ") VALUES ("
         for _ in kwargs:
```

### Comparing `ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/PKG-INFO` & `ConcurrentDatabase-0.0.6/ConcurrentDatabase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.5
+Version: 0.0.6
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.5/PKG-INFO` & `ConcurrentDatabase-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.5
+Version: 0.0.6
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.5/README.md` & `ConcurrentDatabase-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.5/pyproject.toml` & `ConcurrentDatabase-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "ConcurrentDatabase"
 author = "Jay S"
 author_email = ""
-version = "0.0.5"
+version = "0.0.6"
 description = "A simple wrapper allow for treating an SQLite database as an object oriented structure"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `ConcurrentDatabase-0.0.5/setup.py` & `ConcurrentDatabase-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ConcurrentDatabase",
-    version="0.0.5",
+    version="0.0.6",
     author="Jay S",
     author_email="",
     description="A SQLite wrapper that allows for object oriented database access.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

