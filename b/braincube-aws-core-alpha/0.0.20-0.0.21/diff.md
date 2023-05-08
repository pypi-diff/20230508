# Comparing `tmp/braincube-aws-core-alpha-0.0.20.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.20.tar", last modified: Mon May  8 10:41:21 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.21.tar", last modified: Mon May  8 13:09:23 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.20.tar` & `braincube-aws-core-alpha-0.0.21.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.832250 braincube-aws-core-alpha-0.0.20/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.20/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 10:41:21.832510 braincube-aws-core-alpha-0.0.20/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.20/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.20/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-08 10:41:21.833764 braincube-aws-core-alpha-0.0.20/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.20/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.814898 braincube-aws-core-alpha-0.0.20/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.819085 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.819552 braincube-aws-core-alpha-0.0.20/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.823083 braincube-aws-core-alpha-0.0.20/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-05 18:31:34.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2434 2023-05-08 10:25:13.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    29969 2023-05-08 09:06:16.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.825968 braincube-aws-core-alpha-0.0.20/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4099 2023-05-08 10:29:00.000000 braincube-aws-core-alpha-0.0.20/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.829450 braincube-aws-core-alpha-0.0.20/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2883 2023-05-03 16:48:18.000000 braincube-aws-core-alpha-0.0.20/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3741 2023-05-08 10:21:48.000000 braincube-aws-core-alpha-0.0.20/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.831613 braincube-aws-core-alpha-0.0.20/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-07 19:45:48.000000 braincube-aws-core-alpha-0.0.20/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1437 2023-05-04 08:51:42.000000 braincube-aws-core-alpha-0.0.20/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.212328 braincube-aws-core-alpha-0.0.21/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.21/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 13:09:23.213256 braincube-aws-core-alpha-0.0.21/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.21/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.21/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-08 13:09:23.217686 braincube-aws-core-alpha-0.0.21/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.21/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.191462 braincube-aws-core-alpha-0.0.21/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.196745 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.197131 braincube-aws-core-alpha-0.0.21/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.200358 braincube-aws-core-alpha-0.0.21/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-05 18:31:34.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2434 2023-05-08 10:25:13.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    30110 2023-05-08 12:48:30.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.203434 braincube-aws-core-alpha-0.0.21/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4099 2023-05-08 13:07:54.000000 braincube-aws-core-alpha-0.0.21/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.206872 braincube-aws-core-alpha-0.0.21/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2835 2023-05-08 12:13:01.000000 braincube-aws-core-alpha-0.0.21/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3741 2023-05-08 10:21:48.000000 braincube-aws-core-alpha-0.0.21/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.210346 braincube-aws-core-alpha-0.0.21/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-07 19:45:48.000000 braincube-aws-core-alpha-0.0.21/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1437 2023-05-04 08:51:42.000000 braincube-aws-core-alpha-0.0.21/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.20/LICENSE` & `braincube-aws-core-alpha-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/PKG-INFO` & `braincube-aws-core-alpha-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.20
+Version: 0.0.21
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.20/README.md` & `braincube-aws-core-alpha-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/setup.cfg` & `braincube-aws-core-alpha-0.0.21/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.20
+version = 0.0.21
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.20
+Version: 0.0.21
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.21/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.21/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.21/src/core/dal/postgres_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,19 +140,18 @@
         table = Table(self._master_table[1])
 
         for field, column in self._aliases_to_fields(returning_aliases, select=False):
             q = q.returning(table[field.name].as_(field.alias))
 
         return await self._fetch(q, False, connection)
 
-    def _create_primary_key_criterion(self, key: Key) -> Criterion:
-
-        return Criterion.all([
-            pk[0] == key.values[i] for i, pk in enumerate(self._master_primary_key.values())
-        ])
+    def _create_primary_key_criterion(self, key: Key, select: bool = True) -> Criterion:
+        return Criterion.all(
+            [pk[0] == key.values[i] if select else (Field(name=pk[1].name) == key.values[i]) for i, pk in
+             enumerate(self._master_primary_key.values())])
 
     def _aliases_to_fields(self, aliases: list[str] | None = None,
                            select: bool = True) -> list[tuple]:
 
         fields = list()
         accepted = self._schema_columns_fields if select else self._master_columns
         if aliases:
@@ -295,14 +294,15 @@
                         order: list[Order] | None = None,
                         connection: Connection | None = None) -> list[dict[str, any]]:
 
         q, _ = self._init_select_query(aliases, criterion, order)
 
         return await self._fetch(q, connection=connection)
 
+    # TODO: Optional connection
     async def _find_many(self, connection: Connection,
                          aliases: list[str] | None = None,
                          criterion: Criterion | None = None,
                          page: Pageable = Pageable(),
                          order: list[Order] | None = None) -> Page | Top | list[dict[str, any]]:
 
         if page.top_size < 0:
@@ -371,15 +371,15 @@
         dq = PostgreSQLQuery \
             .from_(self._master_table[1]) \
             .delete() \
             .where(criterion)
 
         return await self._execute(dq, returning_aliases, connection)
 
-    async def find_by_id(self, key: Key,
+    async def find_by_pk(self, key: Key,
                          aliases: list[str] | None = None,
                          connection: Connection | None = None) -> dict[str, any] | None:
         """Find the record from passed key.
         :param key: Record identifier.
         :param aliases: List of fields that will be selected by the query.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record as dictionary.
@@ -387,24 +387,24 @@
 
         criterion = self._create_primary_key_criterion(key)
 
         q, _ = self._init_select_query(aliases, criterion, set_order=False)
 
         return await self._fetch_one(q, connection=connection)
 
-    async def exists_by_id(self, key: Key, connection: Connection | None = None) -> bool:
+    async def exists_by_pk(self, key: Key, connection: Connection | None = None) -> bool:
         """Find if record exists from passed key.
         :param key: Record identifier.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record existence.
         """
 
         aliases = [column.alias for field, column in self._master_primary_key.values()]
 
-        return await self.find_by_id(key, aliases, connection) is not None
+        return await self.find_by_pk(key, aliases, connection) is not None
 
     async def find_one(self, aliases: list[str] | None = None,
                        conditions: list[Condition] | None = None,
                        order: list[Order] | None = None,
                        connection: Connection | None = None) -> dict[str, any] | None:
         """Find one record from passed filters.
         :param aliases: List of fields that will be selected by the query.
@@ -430,15 +430,15 @@
         :return: Records as dictionary list.
         """
 
         criterion = self._conditions_to_criterion(conditions)
 
         return await self._find_all(aliases, criterion, order, connection)
 
-    async def find_all_by_id(self, keys: list[Key],
+    async def find_all_by_pk(self, keys: list[Key],
                              aliases: list[str] | None = None,
                              order: list[Order] | None = None,
                              connection: Connection | None = None) -> list[dict[str, any]]:
         """Find all records from passed keys.
         :param keys: Records identifiers.
         :param aliases: List of fields that will be selected by the query.
         :param order: Order in which the records will be returned.
@@ -576,28 +576,28 @@
         :return: Execution results as dictionary list.
         """
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._update(data, criterion, returning_aliases, connection)
 
-    async def update_by_id(self, key: Key,
+    async def update_by_pk(self, key: Key,
                            data: BaseModel | dict[str, any],
                            returning_aliases: list[str] | None = None,
                            connection: Connection | None = None) -> dict[str, any] | None:
         """Update record with new data according to passed key.
         :param key: Record identifier.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution result as dictionary.
         """
 
-        criterion = self._create_primary_key_criterion(key)
+        criterion = self._create_primary_key_criterion(key, select=False)
 
         records = await self._update(data, criterion, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
 
     async def update_data(self, data: BaseModel | dict[str, any],
                           conditions: list[Condition],
@@ -612,28 +612,28 @@
         :return: Execution results with returning type.
         """
 
         results = await self.update(data, conditions, self.__base_model_aliases(returning), connection)
 
         return [returning(**r) for r in results] if results else None
 
-    async def update_data_by_id(self, key: Key,
+    async def update_data_by_pk(self, key: Key,
                                 data: BaseModel | dict[str, any],
                                 returning: type[T],
                                 connection: Connection | None = None) -> T | None:
         """Update record with new data according to passed key using model.
         :param key: Record identifier.
         :param data: Model which contains master table column properties.
         :param returning: Result type.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution result with returning type.
         """
 
-        result = await self.update_by_id(key, data, self.__base_model_aliases(returning), connection)
+        result = await self.update_by_pk(key, data, self.__base_model_aliases(returning), connection)
 
         return returning(**result) if result else None
 
     async def delete(self, conditions: list[Condition],
                      returning_aliases: list[str] | None = None,
                      connection: Connection | None = None) -> list[dict[str, any]] | None:
         """Delete records according conditions.
@@ -644,23 +644,23 @@
         :return: Execution results as dictionary list.
         """
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._delete(criterion, returning_aliases, connection)
 
-    async def delete_by_id(self, key: Key,
+    async def delete_by_pk(self, key: Key,
                            returning_aliases: list[str] | None = None,
                            connection: Connection | None = None) -> dict[str, any] | None:
         """Delete records according to passed key.
         :param key: Record identifier.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When conditions are empty.
         :return: Execution results as dictionary.
         """
 
-        criterion = self._create_primary_key_criterion(key)
+        criterion = self._create_primary_key_criterion(key, select=False)
 
         records = await self._delete(criterion, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
```

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.21/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.21/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.21/src/core/rest/app_controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from typing import Optional
-
-
 class AppController:
     """Module with which you can define endpoints.
     :param base_path: base resource url.
     """
 
     def __init__(self, base_path: str):
         self.routes = dict()
         self._base_url = base_path
 
-    def route(self, path: str, method: str, qualifier: Optional[str] = None):
+    def route(self, path: str, method: str, qualifier: str | None = None):
         """Function that represents an endpoint.
         :param path: Resource url.
         :param method: HTTP method.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
@@ -23,51 +20,51 @@
             if path_ not in self.routes:
                 self.routes[path_] = dict()
             self.routes[path_][method] = func, qualifier
             return func
 
         return _route
 
-    def get(self, path: str = "", qualifier: Optional[str] = None):
+    def get(self, path: str = "", qualifier: str | None = None):
         """Function that represents an HTTP GET method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "GET", qualifier)
 
-    def post(self, path: str = "", qualifier: Optional[str] = None):
+    def post(self, path: str = "", qualifier: str | None = None):
         """Function that represents an HTTP POST method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "POST", qualifier)
 
-    def patch(self, path: str = "", qualifier: Optional[str] = None):
+    def patch(self, path: str = "", qualifier: str | None = None):
         """Function that represents an HTTP PATCH method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "PATCH", qualifier)
 
-    def delete(self, path: str = "", qualifier: Optional[str] = None):
+    def delete(self, path: str = "", qualifier: str | None = None):
         """Function that represents an HTTP DELETE method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "DELETE", qualifier)
 
-    def put(self, path: str = "", qualifier: Optional[str] = None):
+    def put(self, path: str = "", qualifier: str | None = None):
         """Function that represents an HTTP PUT method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "PUT", qualifier)
```

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.21/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.21/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.21/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.20/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.21/src/core/utils/data.py`

 * *Files identical despite different names*

