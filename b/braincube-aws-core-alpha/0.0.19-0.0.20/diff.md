# Comparing `tmp/braincube-aws-core-alpha-0.0.19.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.19.tar", last modified: Mon May  8 06:57:23 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.20.tar", last modified: Mon May  8 10:41:21 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.19.tar` & `braincube-aws-core-alpha-0.0.20.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.891639 braincube-aws-core-alpha-0.0.19/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.19/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 06:57:23.891885 braincube-aws-core-alpha-0.0.19/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.19/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.19/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-08 06:57:23.892998 braincube-aws-core-alpha-0.0.19/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.19/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.878317 braincube-aws-core-alpha-0.0.19/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.883482 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.883983 braincube-aws-core-alpha-0.0.19/src/core/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.886187 braincube-aws-core-alpha-0.0.19/src/core/dal/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/data.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/database_errors.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2257 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/postgres_connection.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)    29861 2023-05-08 06:54:18.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.887803 braincube-aws-core-alpha-0.0.19/src/core/di/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/di/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/di/data.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3796 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.889804 braincube-aws-core-alpha-0.0.19/src/core/rest/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/rest/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2883 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/rest/app_controller.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3741 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/rest/app_module.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.891269 braincube-aws-core-alpha-0.0.19/src/core/utils/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/utils/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/utils/convert.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1437 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.832250 braincube-aws-core-alpha-0.0.20/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.20/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 10:41:21.832510 braincube-aws-core-alpha-0.0.20/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.20/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.20/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-08 10:41:21.833764 braincube-aws-core-alpha-0.0.20/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.20/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.814898 braincube-aws-core-alpha-0.0.20/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.819085 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-08 10:41:21.000000 braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.819552 braincube-aws-core-alpha-0.0.20/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.823083 braincube-aws-core-alpha-0.0.20/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-05 18:31:34.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2434 2023-05-08 10:25:13.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    29969 2023-05-08 09:06:16.000000 braincube-aws-core-alpha-0.0.20/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.825968 braincube-aws-core-alpha-0.0.20/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4099 2023-05-08 10:29:00.000000 braincube-aws-core-alpha-0.0.20/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.829450 braincube-aws-core-alpha-0.0.20/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2883 2023-05-03 16:48:18.000000 braincube-aws-core-alpha-0.0.20/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3741 2023-05-08 10:21:48.000000 braincube-aws-core-alpha-0.0.20/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 10:41:21.831613 braincube-aws-core-alpha-0.0.20/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.20/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-07 19:45:48.000000 braincube-aws-core-alpha-0.0.20/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1437 2023-05-04 08:51:42.000000 braincube-aws-core-alpha-0.0.20/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.19/LICENSE` & `braincube-aws-core-alpha-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.19/PKG-INFO` & `braincube-aws-core-alpha-0.0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.19
+Version: 0.0.20
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.19/README.md` & `braincube-aws-core-alpha-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.19/setup.cfg` & `braincube-aws-core-alpha-0.0.20/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.19
+version = 0.0.20
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.19
+Version: 0.0.20
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.20/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.20/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.20/src/core/dal/postgres_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,18 @@
     connection: Connection = await connect(user=user, password=password, database=database, host=host, port=port)
     await __init(connection)
     return connection
 
 
 async def get_pool(user: str = os.environ["PG_USER"], password: str = os.environ["PG_PASSWORD"],
                    database: str = os.environ["PG_DATABASE"], host: str = os.environ["PG_HOST"],
-                   port: int = os.environ["PG_PORT"], min_size: int = 0,
-                   max_size: int = 2, max_inactive_connection_lifetime: int = 2) -> Pool:
+                   port: int = os.environ["PG_PORT"], min_size: int = int(os.environ["PG_POOL_MIN_SIZE"]),
+                   max_size: int = int(os.environ["PG_POOL_MAX_SIZE"]),
+                   max_inactive_connection_lifetime: int = int(
+                       os.environ["PG_POOL_MAX_INACTIVE_CONNECTION_LIFETIME_SECONDS"])) -> Pool:
     """Retrieve a database connection pool.
     :param user: Database user.
     :param password: Database password.
     :param database: Database name.
     :param host: Database host.
     :param port: Database port number.
     :param min_size: Number of connection the pool will be initialized with.
```

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.20/src/core/dal/postgres_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,19 +295,22 @@
                         order: list[Order] | None = None,
                         connection: Connection | None = None) -> list[dict[str, any]]:
 
         q, _ = self._init_select_query(aliases, criterion, order)
 
         return await self._fetch(q, connection=connection)
 
-    async def _find_all_page(self, connection: Connection,
-                             aliases: list[str] | None = None,
-                             criterion: Criterion | None = None,
-                             page: Pageable = Pageable(),
-                             order: list[Order] | None = None) -> Page | Top:
+    async def _find_many(self, connection: Connection,
+                         aliases: list[str] | None = None,
+                         criterion: Criterion | None = None,
+                         page: Pageable = Pageable(),
+                         order: list[Order] | None = None) -> Page | Top | list[dict[str, any]]:
+
+        if page.top_size < 0:
+            return await self._find_all(aliases, criterion, order, connection)
 
         start = time.time()
 
         calc_top = page.top_size > 0
         q, cq = self._init_select_query(aliases, criterion, order, count_query=not calc_top)
 
         # top implementation
@@ -446,34 +449,34 @@
         if not keys:
             raise DatabaseError("no keys provided")
 
         criterion = Criterion.any([self._create_primary_key_criterion(key) for key in keys])
 
         return await self._find_all(aliases, criterion, order, connection)
 
-    async def find_all_page(self, aliases: list[str] | None = None,
-                            conditions: list[Condition] | None = None,
-                            page: Pageable = Pageable(),
-                            order: list[Order] | None = None,
-                            connection: Connection | None = None) -> Page | Top:
+    async def find_many(self, aliases: list[str] | None = None,
+                        conditions: list[Condition] | None = None,
+                        page: Pageable = Pageable(),
+                        order: list[Order] | None = None,
+                        connection: Connection | None = None) -> Page | Top | list[dict[str, any]]:
         """Find records from passed filters using paging.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param page: Limit and offset of the query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records wrapped by Page or Top dataclass.
         """
 
         criterion = self._conditions_to_criterion(conditions)
 
         if connection:
-            return await self._find_all_page(connection, aliases, criterion, page, order)
+            return await self._find_many(connection, aliases, criterion, page, order)
         async with self._pool.acquire() as connection_:
-            return await self._find_all_page(connection_, aliases, criterion, page, order)
+            return await self._find_many(connection_, aliases, criterion, page, order)
 
     async def insert(self, data: BaseModel | dict[str, any],
                      returning_aliases: list[str] | None = None,
                      connection: Connection | None = None) -> dict[str, any]:
         """Insert one record from dictionary.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
```

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.20/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.20/src/core/di/injector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import List, Optional, TypeVar, Type
 from inspect import signature, isfunction, iscoroutinefunction
 from .data import Dependency, Scope, qualifier_to_data
 
+from ..dal.postgres_connection import Pool, get_pool
+
 T = TypeVar("T")
 
 
 class _Injector:
     """Module that used in order to resolve dependencies from components or route functions."""
 
     dependencies: List[Dependency] = list()
@@ -27,24 +29,32 @@
                 _Injector.dependencies.append(Dependency(scope, component, params, name))
             return component
 
         return _inject
 
     @staticmethod
     async def provide(cls: Type[T], name: Optional[str] = None) -> T:
+
         matched = list(filter(lambda d: (d.cls is cls or issubclass(d.cls, cls)) and
                                         (d.name == name if name else d.name is None), _Injector.dependencies))
+
+        if not matched and cls is Pool:
+            instance = await get_pool()
+            _Injector.dependencies.append(Dependency(Scope.singleton, Pool, instance=instance))
+            return instance
+
         if not matched:
             raise ValueError(f"component name:'{name}', class:'{cls}' not found.")
         if len(matched) > 1:
             raise ValueError(f"multiple matching components have been found for class: '{cls}'")
         if not matched[0].instance:
             nested = list()
-            for param in matched[0].params:
-                nested.append(await _Injector.provide(param[0], param[1]))  # noqa
+            if matched[0].params:
+                for param in matched[0].params:
+                    nested.append(await _Injector.provide(param[0], param[1]))  # noqa
             if matched[0].factory:
                 instance = await matched[0].factory(*nested) \
                     if iscoroutinefunction(matched[0].factory) else matched[0].factory(*nested)
             else:
                 instance = matched[0].cls(*nested)
             if matched[0].scope is Scope.request:
                 return instance
```

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.20/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.20/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.20/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.20/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.19/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.20/src/core/utils/data.py`

 * *Files identical despite different names*

