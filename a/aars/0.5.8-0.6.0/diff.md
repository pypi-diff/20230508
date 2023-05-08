# Comparing `tmp/aars-0.5.8.tar.gz` & `tmp/aars-0.6.0.tar.gz`

## Comparing `aars-0.5.8.tar` & `aars-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.5.8/docs-requirements.txt
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aars-0.5.8/mkdocs.yml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.5.8/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.5.8/.github/workflows/mkdocs-gh-pages.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.5.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.5.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 aars-0.5.8/docs/FastAPI_Cookbook.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.8/docs/index.md -> ../README.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/Exceptions.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/utils.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/core/AARS.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/core/Index.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/core/Record.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/__init__.py
--rw-r--r--   0        0        0    38516 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/core.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/py.typed
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.8/tests/__init__.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 aars-0.5.8/tests/aars.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.5.8/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.5.8/LICENSE
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 aars-0.5.8/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 aars-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.6.0/docs-requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aars-0.6.0/mkdocs.yml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.6.0/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.6.0/.github/workflows/mkdocs-gh-pages.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aars-0.6.0/docs/FastAPI_Cookbook.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.6.0/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/Exceptions.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/utils.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/core/AARS.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/core/Index.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/core/Record.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/__init__.py
+-rw-r--r--   0        0        0    39589 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/core.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/py.typed
+-rw-r--r--   0        0        0    12223 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 aars-0.6.0/tests/aars.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 aars-0.6.0/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 aars-0.6.0/PKG-INFO
```

### Comparing `aars-0.5.8/mkdocs.yml` & `aars-0.6.0/mkdocs.yml`

 * *Files 22% similar despite different names*

```diff
@@ -20,11 +20,10 @@
             options:
               sort: attr,name
               show_root_heading: false
               selection:
                 members:
                   - public
                   - protected
-              show_source: true
               show_signature_annotations: true
               merge_init_into_class: true
               autodoc: true
```

### Comparing `aars-0.5.8/.github/workflows/mkdocs-gh-pages.yml` & `aars-0.6.0/.github/workflows/mkdocs-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.8/.github/workflows/publish.yml` & `aars-0.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.8/.github/workflows/python-publish.yml` & `aars-0.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.8/docs/FastAPI_Cookbook.md` & `aars-0.6.0/docs/FastAPI_Cookbook.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,149 @@
-# FastAPI Cookbook
-This cookbook will show you how to build and test an advanced FastAPI app using the full suite of AARS features:
-
-- Indexing for efficient querying
-- Built-in pagination for large result sets
-- Support for caching
-- Listening for new messages on Aleph
-
-## Basic setup
-Creating a [FastAPI](https://fastapi.tiangolo.com/) app with AARS is very simple.
-The following code snippet shows how to initialize AARS and add it to your FastAPI app.
-```python
-from fastapi import FastAPI
-
-from aleph.sdk.vm.app import AlephApp
-
-from aars import AARS, Record
-
-http_app = FastAPI()
-
-# Setup the Aleph app
-app = AlephApp(http_app=http_app)
-
-# Initialize AARS
-aars = AARS(
-    channel="MY_CHANNEL",
-)
-```
-Your app is now ready to use AARS. The next step is to define your data schema.
-
-## Interlude: Caching Aleph messages
-You can use a cache to speed up subsequent fetches of Aleph messages:
-```python
-from aleph.sdk.vm.cache import VmCache, TestVmCache
-from os import getenv
-TEST_CACHE = getenv("TEST_CACHE")
-if TEST_CACHE is not None and TEST_CACHE.lower() == "true":
-    cache = TestVmCache()
-else:
-    cache = VmCache()
-
-aars = AARS(
-    channel="MY_CHANNEL",
-    cache=cache
-)
-```
-In this example, setting the `TEST_CACHE` environment variable to `true` will use a cache that you can
-easily run locally with [Uvicorn](https://www.uvicorn.org/):
-```shell
-export TEST_CACHE=true
-python -m uvicorn aars.test_cache:app --reload
-```
-!!! note "Caches work well with Aleph messages, as they are immutable."
-    An exception to this are records that have been forgotten.
-    AARS will handle cache invalidation automatically, if you use the [`forget`][aars.core.Record.forget] method to forget a record.
-    But you should be aware that forgotten messages differ from the original message and other actors
-    thay may forget your message can invalidate your cache without AARS noticing.
-
-!!! tip "Use a cache whenever possible"
-
-## Defining a data schema
-Now that we have AARS initialized, we can create a record.
-```python
-from typing import Optional
-
-from aars import Index
-
-class User(Record):
-    username: str
-    display_name: str
-    bio: Optional[str]
-
-Index(User, 'username')
-```
-This code snippet creates a User record with three fields: `username`, `display_name`, and `bio`.
-The `Index` class creates an index on the `username` field. This is required for efficient querying.
-
-## Syncing indices
-We call `AARS.sync_indices()` to sync the indices with the Aleph VM. This is necessary if
-you have previously created records through AARS and want to query them using the indices.
-
-The correct way to handle syncing indices is to call `AARS.sync_indices()` on the ASGI startup sequence.
-This is the sequence of events that FastAPI runs when it starts up. You can read more about it
-[here](https://fastapi.tiangolo.com/advanced/events/#startup-event).
-```python
-import asyncio
-
-# IMPORTANT: app should be the AlephApp instance
-@app.on_event("startup")
-async def startup():
-    await asyncio.wait_for(AARS.sync_indices(), timeout=None)
-```
-Note that we are using `asyncio.wait_for` to wait for the indices to sync, as we can set the timeout to `None` for
-the possibly lengthy operation.
-
-!!! Warning
-
-    Calling `AARS.sync_indices()` scales linearly with the number of records in the VM. This means that
-    if you have 1000 records, it will take roughly `1000 / 50 = 20` API calls to sync the indices. This is why it is
-    recommended to call `AARS.sync_indices()` only once, after you have created all of your records and indices.
-    AARS will automatically add records to the indices as they are created.
-    
-
-## Creating and querying Records with FastAPI
-Now that we have a record, we can create a FastAPI endpoint to create and query records.
-
-### Creating a Record
-```python
-@app.post("/users")
-async def create_user(
-    username: str,
-    display_name: str,
-    bio: Optional[str] = None,
-) -> User:
-    user = User(
-        username=username,
-        display_name=display_name,
-        bio=bio,
-    )
-    return await user.save()
-```
-This endpoint will create a new user record and return it.
-
-### Fetching Records
-```python
-from typing import List
-@app.get("/users")
-async def get_users(
-    page: int = 1,
-    page_size: int = 20,
-) -> List[User]:
-    return await User.fetch_objects().page(page=page, page_size=page_size)
-```
-This endpoint will return a list of users, paginated by 20 users per page.
-
-### Using an Index to query Records
-```python
-@app.get("/users/{username}")
-async def get_user(
-    username: str,
-) -> User:
-    return await User.fetch_objects().where_eq(username=username).first()
-```
-This endpoint will return a single user, given their username.
-
-## Listening to Aleph Messages
-!!! warning "TODO"
+# FastAPI Cookbook
+This cookbook will show you how to build and test an advanced FastAPI app using the full suite of AARS features:
+
+- Indexing for efficient querying
+- Built-in pagination for large result sets
+- Support for caching
+- Listening for new messages on Aleph
+
+## Basic setup
+Creating a [FastAPI](https://fastapi.tiangolo.com/) app with AARS is very simple.
+The following code snippet shows how to initialize AARS and add it to your FastAPI app.
+```python
+from fastapi import FastAPI
+
+from aleph.sdk.vm.app import AlephApp
+
+from aars import AARS, Record
+
+http_app = FastAPI()
+
+# Setup the Aleph app
+app = AlephApp(http_app=http_app)
+
+# Initialize AARS
+aars = AARS(
+    channel="MY_CHANNEL",
+)
+```
+Your app is now ready to use AARS. The next step is to define your data schema.
+
+## Interlude: Caching Aleph messages
+You can use a cache to speed up subsequent fetches of Aleph messages:
+```python
+from aleph.sdk.vm.cache import VmCache, TestVmCache
+from os import getenv
+TEST_CACHE = getenv("TEST_CACHE")
+if TEST_CACHE is not None and TEST_CACHE.lower() == "true":
+    cache = TestVmCache()
+else:
+    cache = VmCache()
+
+aars = AARS(
+    channel="MY_CHANNEL",
+    cache=cache
+)
+```
+In this example, setting the `TEST_CACHE` environment variable to `true` will use a cache that you can
+easily run locally with [Uvicorn](https://www.uvicorn.org/):
+```shell
+export TEST_CACHE=true
+python -m uvicorn aars.test_cache:app --reload
+```
+!!! note "Caches work well with Aleph messages, as they are immutable."
+    An exception to this are records that have been forgotten.
+    AARS will handle cache invalidation automatically, if you use the [`forget`][aars.core.Record.forget] method to forget a record.
+    But you should be aware that forgotten messages differ from the original message and other actors
+    thay may forget your message can invalidate your cache without AARS noticing.
+
+!!! tip "Use a cache whenever possible"
+
+## Defining a data schema
+Now that we have AARS initialized, we can create a record.
+```python
+from typing import Optional
+
+from aars import Index
+
+class User(Record):
+    username: str
+    display_name: str
+    bio: Optional[str]
+
+Index(User, 'username')
+```
+This code snippet creates a User record with three fields: `username`, `display_name`, and `bio`.
+The `Index` class creates an index on the `username` field. This is required for efficient querying.
+
+## Syncing indices
+We call `AARS.sync_indices()` to sync the indices with the Aleph VM. This is necessary if
+you have previously created records through AARS and want to query them using the indices.
+
+The correct way to handle syncing indices is to call `AARS.sync_indices()` on the ASGI startup sequence.
+This is the sequence of events that FastAPI runs when it starts up. You can read more about it
+[here](https://fastapi.tiangolo.com/advanced/events/#startup-event).
+```python
+import asyncio
+
+# IMPORTANT: app should be the AlephApp instance
+@app.on_event("startup")
+async def startup():
+    await asyncio.wait_for(AARS.sync_indices(), timeout=None)
+```
+Note that we are using `asyncio.wait_for` to wait for the indices to sync, as we can set the timeout to `None` for
+the possibly lengthy operation.
+
+!!! Warning
+
+    Calling `AARS.sync_indices()` scales linearly with the number of records in the VM. This means that
+    if you have 1000 records, it will take roughly `1000 / 50 = 20` API calls to sync the indices. This is why it is
+    recommended to call `AARS.sync_indices()` only once, after you have created all of your records and indices.
+    AARS will automatically add records to the indices as they are created.
+    
+
+## Creating and querying Records with FastAPI
+Now that we have a record, we can create a FastAPI endpoint to create and query records.
+
+### Creating a Record
+```python
+@app.post("/users")
+async def create_user(
+    username: str,
+    display_name: str,
+    bio: Optional[str] = None,
+) -> User:
+    user = User(
+        username=username,
+        display_name=display_name,
+        bio=bio,
+    )
+    return await user.save()
+```
+This endpoint will create a new user record and return it.
+
+### Fetching Records
+```python
+from typing import List
+@app.get("/users")
+async def get_users(
+    page: int = 1,
+    page_size: int = 20,
+) -> List[User]:
+    return await User.fetch_objects().page(page=page, page_size=page_size)
+```
+This endpoint will return a list of users, paginated by 20 users per page.
+
+### Using an Index to query Records
+
+```python
+@app.get("/users/{username}")
+async def get_user(
+        username: str,
+) -> User:
+    return await User.fetch_objects().filter(username=username).first()
+```
+This endpoint will return a single user, given their username.
+
+## Listening to Aleph Messages
+!!! warning "TODO"
     This section is not yet complete.
```

### Comparing `aars-0.5.8/src/aars/core.py` & `aars-0.6.0/src/aars/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,45 +358,57 @@
 
         Returns:
             A pageable request object, which can be asynchronously iterated over.
         """
         return PageableRequest(AARS.fetch_records, record_type=cls)
 
     @classmethod
-    def where_eq(cls: Type[R], **kwargs) -> PageableResponse[R]:
+    def filter(cls: Type[R], **kwargs) -> PageableResponse[R]:
         """
         Queries an object by given properties through an index, in order to fetch applicable records.
-        An index name is defined as
-        ```python
-        "Class.property1.property2"
-        ```
-        and is initialized by creating an `Index` instance, targeting a BaseRecord class with a list of properties.
 
-        ```python
-        Index(MyRecord, ['property1', 'property2'])
-        ```
+        Example: What is an index?
+            An index name is defined as
+            ```python
+            "Class.property1.property2"
+            ```
+            and is initialized by creating an `Index` instance, targeting a BaseRecord class with a list of properties.
 
-        This will create an index named 'MyRecord.property1.property2' which can be queried with:
+            ```python
+            Index(MyRecord, ['property1', 'property2'])
+            ```
 
-        ```python
-        MyRecord.where_eq(property1='value1', property2='value2')
-        ```
+            This will create an index named 'MyRecord.property1.property2' which can be queried with:
 
-        If no index is defined for the given properties, an IndexError is raised.
+            ```python
+            MyRecord.filter(property1='value1', property2='value2')
+            ```
+
+        Similar to the Django ORM, it allows the `__in` operator to query for multiple values of a property.
+
+        Example: Querying for multiple values
+            ```python
+            MyRecord.filter(property1__in=['value1', 'value2'])
+            ```
+            This will return all records where `property1` is either `'value1'` or `'value2'`.
 
-        If only a part of the keys is indexed for the given query, a fallback index is used and locally filtered.
+        Note: Fallback indexes
+            If only a part of the keys is indexed for the given query, a fallback index is used and locally filtered.
 
         Args:
             **kwargs: The properties to query for.
         Returns:
             A pageable response object, which can be asynchronously iterated over.
+        Raises:
+            IndexError: If no index is defined for the given properties.
+            KeyError: If a given property does not exist.
         """
         query = IndexQuery(cls, **kwargs)
         index = cls.get_index(query.get_index_name())
-        generator = index.lookup(query)
+        generator = index.lookup_and_fetch(query)
         return PageableResponse(generator)
 
     @classmethod
     def add_index(cls: Type[R], index: "Index") -> None:
         """
         Adds an index to the class. This allows the index to be used for queries and will be automatically updated
         when records are created or updated.
@@ -505,20 +517,20 @@
 
 class Index(Record, Generic[R]):
     """
     An Index is a data structure that allows for fast lookup of records by their properties.
     It is used internally by the Record class and once created, is automatically updated when records are created or
     updated.
 
-    It is not recommended using the Index class directly, but rather through the `where_eq` method of the `Record`
+    It is not recommended using the Index class directly, but rather through the `filter` method of the `Record`
     class.
 
     Example:
         ```python
-        MyRecord.where_eq(foo='bar')
+        MyRecord.filter(foo='bar')
         ```
         If `MyRecord` has an index on the property `foo`, this will return all records of type `MyRecord` where `foo` is
         equal to `'bar'`.
     """
 
     record_type: Type[R]
     index_on: List[str]
@@ -556,64 +568,79 @@
 
     def __str__(self):
         return f"Index({self.record_type.__name__}.{'.'.join(self.index_on)})"
 
     def __repr__(self):
         return f"{self.record_type.__name__}.{'.'.join(self.index_on)}"
 
-    def lookup(self, query: IndexQuery) -> AsyncIterator[R]:
+    def lookup(self, query: IndexQuery) -> Tuple[Set[str], bool]:
+        """
+        Retrieves the item_hashes of all records that match the given query, without fetching the records themselves.
+        Args:
+            query: The query to execute.
+        Returns:
+            A tuple of the item_hashes of all records that match the query and a boolean indicating whether the query
+            needs filtering.
+        """
+        assert query.record_type == self.record_type
+        id_hashes: Set[str] = set()
+        needs_filtering = False
+
+        subquery = query
+        if repr(self) != query.get_index_name():
+            subquery = query.get_subquery(self.index_on)
+            needs_filtering = True
+
+        queries = list(subquery.get_unfolded_queries())
+
+        for q in queries:
+            id_hashes.update(self.hashmap.get(tuple(q.values()), set()))
+
+        if not id_hashes:
+            return set(), False
+
+        return id_hashes, needs_filtering
+
+    def lookup_and_fetch(self, query: IndexQuery) -> AsyncIterator[R]:
         """
         Fetches records with given values for the indexed properties.
 
         Example:
             ```python
             index = Index(MyRecord, 'foo')
             index_query = IndexQuery(MyRecord, **{'foo': 'bar'})
             index.lookup(index_query)
             ```
             Returns all records of type `MyRecord` where `foo` is equal to `'bar'`.
-            This is an anti-pattern, as the `IndexQuery` should be created by calling `MyRecord.where_eq(foo='bar')`
+            This is an anti-pattern, as the `IndexQuery` should be created by calling `MyRecord.filter(foo='bar')`
             instead.
 
         Args:
             query: The query to execute.
         Returns:
             An async iterator over the records.
         """
-        assert query.record_type == self.record_type
-        id_hashes: Optional[Set[str]]
-        needs_filtering = False
-
-        subquery = query
-        if repr(self) != query.get_index_name():
-            subquery = query.get_subquery(self.index_on)
-            needs_filtering = True
-        id_hashes = self.hashmap.get(tuple(subquery.values()))
+        id_hashes, needs_filtering = self.lookup(query)
 
-        if id_hashes is None:
+        if not id_hashes:
             return EmptyAsyncIterator()
 
         items = AARS.fetch_records(self.record_type, list(id_hashes))
 
         if needs_filtering:
             return self._filter_index_items(items, query)
         return items
 
     @classmethod
     async def _filter_index_items(
         cls, items: AsyncIterator[R], query: IndexQuery
     ) -> AsyncIterator[R]:
-        sorted_keys = query.keys()
         async for item in items:
-            # eliminate the item which does not fulfill the properties
-            class_properties = vars(item)
-            required_class_properties = {
-                key: class_properties.get(key) for key in sorted_keys
-            }
-            if required_class_properties == dict(query):
+            class_properties = item.content
+            if all(query.comparators[key].value(value, class_properties[key]) for key, value in query.items()):
                 yield item
 
     def add_record(self, obj: R):
         """Adds a record to the index."""
         assert issubclass(type(obj), Record)
         assert obj.id_hash is not None
         key = attrgetter(*self.index_on)(obj)
```

### Comparing `aars-0.5.8/src/aars/exceptions.py` & `aars-0.6.0/src/aars/exceptions.py`

 * *Files identical despite different names*

### Comparing `aars-0.5.8/src/aars/utils.py` & `aars-0.6.0/src/aars/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,34 +5,44 @@
 
 Also, it contains the [PageableResponse][aars.utils.PageableResponse] and
 [PageableRequest][aars.utils.PageableRequest] classes, which allow for
 easy pagination of queries and efficient retrieval of large amounts of data
 in the asynchronous environment of AARS.
 """
 import operator
+from enum import Enum
 from itertools import *
 from typing import (
     AsyncIterator,
     List,
     TypeVar,
     OrderedDict,
     Generic,
     Type,
     Optional,
     Awaitable,
     Callable,
     Tuple,
-    Dict,
+    Dict, Iterator,
 )
 
 from .exceptions import AlreadyUsedError
 
 T = TypeVar("T")
 
 
+class Comparator(Enum):
+    """
+    An enum for the different comparison operators.
+    """
+
+    EQ = operator.eq
+    IN = operator.contains
+
+
 class EmptyAsyncIterator(AsyncIterator[T]):
     """
     An async iterator that can be returned when there are no results.
     """
 
     async def __anext__(self) -> T:
         raise StopAsyncIteration
@@ -42,25 +52,44 @@
     """
     A query for a specific index. The keys are the index keys, and the values are the values to query for.
     It is an ordered dict in which the order is alphabetically determined by the keys, so that the same query
     will always have the same string representation. This is used to determine the index name.
     """
 
     record_type: Type[T]
+    comparators: Dict[str, Comparator]
 
     def __init__(self, record_type: Type[T], **kwargs):
         """
         Create a new IndexQuery.
+        Queries fields can use comparison suffixes to specify the type of comparison to use, like this:
+        ```python
+        IndexQuery(record_type=MyRecord, a__lt=1, b__in=[1, 2, 3])
+        ```
+        This would query for all records of type MyRecord where the field `a` is less than 1 and the field `b` is
+        contained in the list [1, 2, 3].
+
         Args:
             record_type: The type of record that this query is for.
             **kwargs: The keys and values to query for.
         """
-        super().__init__(
-            {item[0]: item[1] for item in sorted(kwargs.items()) if item[1] is not None}
-        )
+        # check if all kwargs are valid
+        self.comparators = {}
+        values = {}
+        for item in sorted(kwargs.items()):
+            if "__" in item[0]:
+                key, comparator = item[0].split("__")
+                self.comparators[key] = Comparator[comparator.upper()]
+            else:
+                key = item[0]
+                self.comparators[key] = Comparator.EQ
+            if key not in record_type.__annotations__:
+                raise KeyError(f"Invalid key '{key}' for record type {record_type.__name__}")
+            values[key] = item[1]
+        super().__init__(values)
         self.record_type = record_type
 
     def get_index_name(self) -> str:
         """
         Get the name of the index that this query would use.
         Returns:
             The name of the index to query.
@@ -78,17 +107,38 @@
             ```
         Args:
             keys: The keys to include in the subquery.
         Returns:
             The subquery.
         """
         return IndexQuery(
-            self.record_type, **{key: arg for key, arg in self.items() if key in keys}
+            self.record_type, **{key + "__" + self.comparators[key].name: arg for key, arg in self.items() if key in keys}
         )
 
+    def get_unfolded_queries(self) -> Iterator["IndexQuery"]:
+        """
+        Get all combinations of queries that arise from the IN comparators.
+        Example:
+            ```python
+            query = IndexQuery(record_type=MyRecord, a__in=[1, 2], b__in=[3, 4])
+            assert query.get_unfolded_queries() == [
+                IndexQuery(record_type=MyRecord, a=1, b=3),
+                IndexQuery(record_type=MyRecord, a=1, b=4),
+                IndexQuery(record_type=MyRecord, a=2, b=3),
+                IndexQuery(record_type=MyRecord, a=2, b=4),
+            ]
+            ```
+        """
+        for key, comparator in self.comparators.items():
+            if comparator == Comparator.IN:
+                for value in self[key]:
+                    yield from IndexQuery(self.record_type, **{key: value}).get_unfolded_queries()
+            else:
+                yield self
+
 
 class PageableResponse(AsyncIterator[T], Generic[T]):
     """
     A wrapper around an AsyncIterator that allows for easy pagination and iteration, while also preventing multiple
     iterations. This is mainly used for nicer syntax when not using the async generator syntax.
 
     Example: Iterate over all records
```

### Comparing `aars-0.5.8/tests/aars.py` & `aars-0.6.0/tests/aars.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,30 +61,42 @@
 
 @pytest.mark.asyncio
 async def test_store_and_index():
     new_book = await Book(title="Atlas Shrugged", author="Ayn Rand").save()
     assert new_book.title == "Atlas Shrugged"
     assert new_book.author == "Ayn Rand"
     await asyncio.sleep(1)
-    fetched_book = await Book.where_eq(title="Atlas Shrugged").first()
+    fetched_book = await Book.filter(title="Atlas Shrugged").first()
     assert new_book == fetched_book
 
 
 @pytest.mark.asyncio
 async def test_multi_index():
     new_book = await Book(title="Lila", author="Robert M. Pirsig", year=1991).save()
     # wait a few secs
     await asyncio.sleep(1)
-    should_be_none = await Book.where_eq(title="Lila", author="Yo Momma").all()
+    should_be_none = await Book.filter(title="Lila", author="Yo Momma").all()
     assert len(should_be_none) == 0
-    fetched_book = await Book.where_eq(title="Lila", author="Robert M. Pirsig").first()
+    fetched_book = await Book.filter(title="Lila", author="Robert M. Pirsig").first()
     assert new_book == fetched_book
 
 
 @pytest.mark.asyncio
+async def test_in_query():
+    books = await asyncio.gather(
+        Book(title="Siddhartha", author="Hermann Hesse", year=1922).save(),
+        Book(title="Fahrenheit 451", author="Ray Bradbury", year=1953).save(),
+    )
+    await asyncio.sleep(1)
+    fetched_books = await Book.filter(title__in=["Siddhartha", "Fahrenheit 451"], year__in=[1922, 1953]).all()
+    assert books[0] in fetched_books
+    assert books[1] in fetched_books
+
+
+@pytest.mark.asyncio
 async def test_amending_record():
     book = await Book(title="Neurodancer", author="William Gibson").save()
     assert book.current_revision == 0
     book.title = "Neuromancer"
     book = await book.save()
     assert book.title == "Neuromancer"
     assert len(book.revision_hashes) == 2
@@ -104,15 +116,15 @@
 async def test_store_and_index_record_of_records():
     books = await asyncio.gather(
         Book(title="Atlas Shrugged", author="Ayn Rand").save(),
         Book(title="The Martian", author="Andy Weir").save(),
     )
     new_library = await Library(name="The Library", books=books).save()
     await asyncio.sleep(1)
-    fetched_library = await Library.where_eq(name="The Library").first()
+    fetched_library = await Library.filter(name="The Library").first()
     assert new_library == fetched_library
 
 
 @pytest.mark.asyncio
 async def test_forget_object():
     forgettable_book = await Book(
         title="The Forgotten Book", author="Mechthild Gläser"
@@ -127,17 +139,16 @@
 
 
 @pytest.mark.asyncio
 async def test_store_and_wrong_where_eq():
     new_book = await Book(title="Atlas Shrugged", author="Ayn Rand").save()
     assert new_book.title == "Atlas Shrugged"
     assert new_book.author == "Ayn Rand"
-    with pytest.warns(UserWarning):
-        fetched_book = await Book.where_eq(title="Atlas Shrugged", foo="bar").all()
-    assert len(fetched_book) == 0
+    with pytest.raises(KeyError):
+        await Book.filter(title="Atlas Shrugged", foo="bar").all()
 
 
 @pytest.mark.asyncio
 async def test_fetch_all_pagination():
     page_one = await Book.fetch_objects().page(1, 1)
     page_two = await Book.fetch_objects().page(2, 1)
     assert len(page_one) == 1
@@ -150,14 +161,15 @@
     class BookWithDictAuthor(Record):
         title: str
         author: dict
 
     book = await BookWithDictAuthor(
         title="Test Book", author={"first": "John", "last": "Doe"}
     ).save()
+    await asyncio.sleep(1)
     fetched_book = await BookWithDictAuthor.fetch(book.id_hash).first()
     assert fetched_book.author == {"first": "John", "last": "Doe"}
 
 
 @pytest.mark.asyncio
 async def test_negative_limit_pagination():
     with pytest.raises(ValueError):
```

### Comparing `aars-0.5.8/.gitignore` & `aars-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aars-0.5.8/LICENSE` & `aars-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aars-0.5.8/README.md` & `aars-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 # Create a new user
 new_user = await User(username='chirpy_user', display_name='Chirpy User', bio='I love chirping!').save()
 
 # Create a new chirp
 new_chirp = await Chirp(author=new_user, content='Hello, Chirper!', likes=0, timestamp=int(time.time())).save()
 
 # Query chirps by author
-chirps_by_author = await Chirp.where_eq(author=new_user).all()
+chirps_by_author = await Chirp.filter(author=new_user).all()
 
 # Update a chirp
 new_chirp.likes += 1
 updated_chirp = await new_chirp.save()
 ```
 
 ## Documentation
```

### Comparing `aars-0.5.8/pyproject.toml` & `aars-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aars"
-version = "0.5.8"
+version = "0.6.0"
 authors = [
   { name="Mike Hukiewitz", email="mike.hukiewitz@robotter.ai" },
 ]
 description = "Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aars-0.5.8/PKG-INFO` & `aars-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aars
-Version: 0.5.8
+Version: 0.6.0
 Summary: Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im
 Project-URL: Homepage, https://github.com/aleph-im/active-record-sdk
 Project-URL: Bug Tracker, https://github.com/aleph-im/active-record-sdk/issues
 Author-email: Mike Hukiewitz <mike.hukiewitz@robotter.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -74,15 +74,15 @@
 # Create a new user
 new_user = await User(username='chirpy_user', display_name='Chirpy User', bio='I love chirping!').save()
 
 # Create a new chirp
 new_chirp = await Chirp(author=new_user, content='Hello, Chirper!', likes=0, timestamp=int(time.time())).save()
 
 # Query chirps by author
-chirps_by_author = await Chirp.where_eq(author=new_user).all()
+chirps_by_author = await Chirp.filter(author=new_user).all()
 
 # Update a chirp
 new_chirp.likes += 1
 updated_chirp = await new_chirp.save()
 ```
 
 ## Documentation
```

