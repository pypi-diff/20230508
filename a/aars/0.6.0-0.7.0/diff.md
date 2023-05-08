# Comparing `tmp/aars-0.6.0.tar.gz` & `tmp/aars-0.7.0.tar.gz`

## Comparing `aars-0.6.0.tar` & `aars-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.6.0/docs-requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aars-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.6.0/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.6.0/.github/workflows/mkdocs-gh-pages.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.6.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.6.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aars-0.6.0/docs/FastAPI_Cookbook.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.6.0/docs/index.md -> ../README.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/Exceptions.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/utils.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/core/AARS.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/core/Index.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.6.0/docs/Code_Reference/core/Record.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/__init__.py
--rw-r--r--   0        0        0    39589 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/core.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/py.typed
--rw-r--r--   0        0        0    12223 2020-02-02 00:00:00.000000 aars-0.6.0/src/aars/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 aars-0.6.0/tests/aars.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.6.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.6.0/LICENSE
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 aars-0.6.0/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 aars-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.7.0/docs-requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aars-0.7.0/mkdocs.yml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.7.0/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.7.0/.github/workflows/mkdocs-gh-pages.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aars-0.7.0/docs/FastAPI_Cookbook.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.0/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.0/docs/Code_Reference/Exceptions.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.7.0/docs/Code_Reference/utils.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.7.0/docs/Code_Reference/core/AARS.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.0/docs/Code_Reference/core/Index.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.7.0/docs/Code_Reference/core/Record.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.7.0/src/aars/__init__.py
+-rw-r--r--   0        0        0    39717 2020-02-02 00:00:00.000000 aars-0.7.0/src/aars/core.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 aars-0.7.0/src/aars/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.0/src/aars/py.typed
+-rw-r--r--   0        0        0    12223 2020-02-02 00:00:00.000000 aars-0.7.0/src/aars/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 aars-0.7.0/tests/aars.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 aars-0.7.0/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 aars-0.7.0/PKG-INFO
```

### Comparing `aars-0.6.0/mkdocs.yml` & `aars-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aars-0.6.0/.github/workflows/mkdocs-gh-pages.yml` & `aars-0.7.0/.github/workflows/mkdocs-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `aars-0.6.0/.github/workflows/publish.yml` & `aars-0.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.6.0/.github/workflows/python-publish.yml` & `aars-0.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.6.0/docs/FastAPI_Cookbook.md` & `aars-0.7.0/docs/FastAPI_Cookbook.md`

 * *Files identical despite different names*

### Comparing `aars-0.6.0/src/aars/core.py` & `aars-0.7.0/src/aars/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,16 @@
         validate_assignment = True
 
     forgotten: bool = Field(
         default=False,
         alias="forgotten",
         description="Whether the record has been forgotten on Aleph",
     )
-    id_hash: Optional[Union[ItemHash, str]] = Field(
-        default=None, alias="id_hash", description="The hash of the record's ID"
+    item_hash: Optional[Union[ItemHash, str]] = Field(
+        default=None, alias="item_hash", description="The hash of the record's ID"
     )
     current_revision: Optional[int] = Field(
         default=0,
         alias="current_revision",
         description="The current revision number of the record",
     )
     revision_hashes: List[ItemHash] = Field(
@@ -116,45 +116,45 @@
     __indexed_items: ClassVar[Set[str]] = set()
     __indices: ClassVar[Dict[str, "Index"]] = {}
 
     def __init__(self, **data: Any):
         super().__init__(**data)
 
     def __repr__(self):
-        return f"{type(self).__name__}({self.id_hash})"
+        return f"{type(self).__name__}({self.item_hash})"
 
     def __str__(self):
         return f"{type(self).__name__} {self.__dict__}"
 
     def __eq__(self, other):
         return (
-            str(self.id_hash) == str(other.id_hash)
-            and self.current_revision == other.current_revision
-            and self.revision_hashes == other.revision_hashes
-            and self.forgotten == other.forgotten
-            and self.content == other.content
-            and self.signer == other.signer
-            and self.changed == other.changed
+                str(self.item_hash) == str(other.item_hash)
+                and self.current_revision == other.current_revision
+                and self.revision_hashes == other.revision_hashes
+                and self.forgotten == other.forgotten
+                and self.content == other.content
+                and self.signer == other.signer
+                and self.changed == other.changed
             # do not compare timestamps, they can deviate on Aleph between commitment and finalization
         )
 
     def __setattr__(self, key, value):
-        if self.changed is False and key != "changed" and self.id_hash is not None:
+        if self.changed is False and key != "changed" and self.item_hash is not None:
             self.changed = True
         return super().__setattr__(key, value)
 
     @property
     def content(self) -> Dict[str, Any]:
         """
         Returns:
             A dictionary of the object's content, as it is to be stored on Aleph inside the `content` property of the POST message.
         """
         return self.dict(
             exclude={
-                "id_hash",
+                "item_hash",
                 "current_revision",
                 "revision_hashes",
                 "forgotten",
                 "timestamp",
                 "signer",
                 "changed",
             }
@@ -163,17 +163,17 @@
     async def update_revision_hashes(self: R) -> R:
         """
         Updates the list of available revision hashes, in order to fetch these.
 
         Returns:
             The object with the updated revision hashes.
         """
-        assert self.id_hash is not None
-        self.revision_hashes = [self.id_hash] + await async_iterator_to_list(
-            AARS.fetch_revisions(type(self), ref=self.id_hash)
+        assert self.item_hash is not None
+        self.revision_hashes = [self.item_hash] + await async_iterator_to_list(
+            AARS.fetch_revisions(type(self), ref=self.item_hash)
         )
         if self.current_revision is None:
             # latest revision
             self.current_revision = len(self.revision_hashes) - 1
         return self
 
     async def fetch_revision(
@@ -185,15 +185,15 @@
         Args:
             rev_no: The revision number of the revision to fetch. Negative numbers are allowed and count from the end.
             rev_hash: The hash of the revision to fetch.
 
         Returns:
             The object with the given revision.
         """
-        if self.id_hash is None:
+        if self.item_hash is None:
             raise NotStoredError(self)
 
         if rev_no is not None:
             if rev_no < 0:
                 rev_no = len(self.revision_hashes) + rev_no
             if self.current_revision == rev_no:
                 return self
@@ -228,15 +228,15 @@
     async def save(self: R) -> R:
         """
         Posts a new item to Aleph or amends it, if it was already posted. Will add new items to local indices.
         For indices to be persisted on Aleph, you need to call `save()` on the index itself or `cls.save_indices()`.
         Returns:
             The updated object itself.
         """
-        if not self.changed and self.id_hash is not None:
+        if not self.changed and self.item_hash is not None:
             return self
         if self.forgotten:
             raise AlreadyForgottenError(self)
         await AARS.post_or_amend_object(self)
         if self.current_revision == 0:
             self._index()
         self.changed = False
@@ -246,44 +246,44 @@
         """
         Adds the object to all indices it is supposed to be in.
         Returns:
             The object itself for chaining.
         """
         for index in self.get_indices():
             index.add_record(self)
-        self.__indexed_items.add(self.id_hash)
+        self.__indexed_items.add(self.item_hash)
 
     @classmethod
-    def is_indexed(cls: Type[R], id_hash: Union[ItemHash, str]) -> bool:
+    def is_indexed(cls: Type[R], item_hash: Union[ItemHash, str]) -> bool:
         """
         Checks if a given object is indexed.
         Args:
-            id_hash: The hash of the object to check.
+            item_hash: The hash of the object to check.
         Returns:
             True if the object is indexed, False otherwise.
         """
-        return id_hash in cls.__indexed_items
+        return item_hash in cls.__indexed_items
 
     async def forget(self: R) -> R:
         """
         Orders Aleph to forget a specific object with all its revisions. Will remove the object from all indices.
         The content of all POST messages will be deleted, but the hashes and timestamps will remain.
         !!! note "The forgotten object should be deleted afterwards, as it is useless now."
         Raises:
             NotStoredError: If the object is not stored on Aleph.
             AlephPermissionError: If the object is not owned by the current account.
             AlreadyForgottenError: If the object was already forgotten.
         """
 
         if not self.forgotten:
-            if self.id_hash is None:
+            if self.item_hash is None:
                 raise NotStoredError(self)
             if self.signer != AARS.account.get_address():
                 raise AlephPermissionError(
-                    AARS.account.get_address(), self.id_hash, self.signer
+                    AARS.account.get_address(), self.item_hash, self.signer
                 )
             await AARS.forget_objects([self])
             [index.remove_record(self) for index in self.get_indices()]
             self.forgotten = True
             return self
         else:
             raise AlreadyForgottenError(self)
@@ -295,25 +295,25 @@
         Args:
             post: The PostMessage to initialize from.
         Returns:
             The initialized object.
         """
         obj: R = cls(**post.content.content)
         if post.content.ref is None:
-            obj.id_hash = post.item_hash
+            obj.item_hash = post.item_hash
         else:
             if isinstance(post.content.ref, str):
-                obj.id_hash = ItemHash(post.content.ref)
+                obj.item_hash = ItemHash(post.content.ref)
             elif isinstance(post.content.ref, ChainRef):
-                obj.id_hash = post.content.ref.item_hash
+                obj.item_hash = post.content.ref.item_hash
             else:
                 raise TypeError(f"Unknown type of ref: {type(post.content.ref)}")
         await obj.update_revision_hashes()
-        assert obj.id_hash is not None
-        obj.current_revision = obj.revision_hashes.index(obj.id_hash)
+        assert obj.item_hash is not None
+        obj.current_revision = obj.revision_hashes.index(obj.item_hash)
         obj.timestamp = post.time
         obj.signer = post.sender
         return obj
 
     @classmethod
     async def from_dict(cls: Type[R], post: Dict[str, Any]) -> R:
         """
@@ -321,20 +321,20 @@
         Args:
             post: The raw Aleph data to initialize from.
         Returns:
             The initialized object.
         """
         obj = cls(**post["content"])
         if post.get("ref") is None:
-            obj.id_hash = ItemHash(post["item_hash"])
+            obj.item_hash = ItemHash(post["item_hash"])
         else:
-            obj.id_hash = ItemHash(post["ref"])
+            obj.item_hash = ItemHash(post["ref"])
         await obj.update_revision_hashes()
-        assert obj.id_hash is not None
-        obj.current_revision = obj.revision_hashes.index(obj.id_hash)
+        assert obj.item_hash is not None
+        obj.current_revision = obj.revision_hashes.index(obj.item_hash)
         obj.timestamp = post["time"]
         obj.signer = post["sender"]
         return obj
 
     @classmethod
     def fetch(
         cls: Type[R], hashes: Union[Union[str, ItemHash], List[Union[str, ItemHash]]]
@@ -501,19 +501,19 @@
         i = 0
         async for record in response:
             if record.signer != AARS.account.get_address():
                 continue
             record_batch.append(record)
             i += 1
             if i % 50 == 0:
-                item_hashes.extend([record.id_hash for record in record_batch])
+                item_hashes.extend([record.item_hash for record in record_batch])
                 await AARS.forget_objects(record_batch)
                 record_batch = []
         if record_batch:
-            item_hashes.extend([record.id_hash for record in record_batch])
+            item_hashes.extend([record.item_hash for record in record_batch])
             await AARS.forget_objects(record_batch)
 
         return item_hashes
 
 
 class Index(Record, Generic[R]):
     """
@@ -578,31 +578,31 @@
         Args:
             query: The query to execute.
         Returns:
             A tuple of the item_hashes of all records that match the query and a boolean indicating whether the query
             needs filtering.
         """
         assert query.record_type == self.record_type
-        id_hashes: Set[str] = set()
+        item_hashes: Set[str] = set()
         needs_filtering = False
 
         subquery = query
         if repr(self) != query.get_index_name():
             subquery = query.get_subquery(self.index_on)
             needs_filtering = True
 
         queries = list(subquery.get_unfolded_queries())
 
         for q in queries:
-            id_hashes.update(self.hashmap.get(tuple(q.values()), set()))
+            item_hashes.update(self.hashmap.get(tuple(q.values()), set()))
 
-        if not id_hashes:
+        if not item_hashes:
             return set(), False
 
-        return id_hashes, needs_filtering
+        return item_hashes, needs_filtering
 
     def lookup_and_fetch(self, query: IndexQuery) -> AsyncIterator[R]:
         """
         Fetches records with given values for the indexed properties.
 
         Example:
             ```python
@@ -615,20 +615,20 @@
             instead.
 
         Args:
             query: The query to execute.
         Returns:
             An async iterator over the records.
         """
-        id_hashes, needs_filtering = self.lookup(query)
+        item_hashes, needs_filtering = self.lookup(query)
 
-        if not id_hashes:
+        if not item_hashes:
             return EmptyAsyncIterator()
 
-        items = AARS.fetch_records(self.record_type, list(id_hashes))
+        items = AARS.fetch_records(self.record_type, list(item_hashes))
 
         if needs_filtering:
             return self._filter_index_items(items, query)
         return items
 
     @classmethod
     async def _filter_index_items(
@@ -638,32 +638,32 @@
             class_properties = item.content
             if all(query.comparators[key].value(value, class_properties[key]) for key, value in query.items()):
                 yield item
 
     def add_record(self, obj: R):
         """Adds a record to the index."""
         assert issubclass(type(obj), Record)
-        assert obj.id_hash is not None
+        assert obj.item_hash is not None
         key = attrgetter(*self.index_on)(obj)
         if isinstance(key, str):
             key = (key,)
         if isinstance(key, list):
             key = tuple(key)
         if key not in self.hashmap:
             self.hashmap[key] = set()
-        self.hashmap[key].add(obj.id_hash)
+        self.hashmap[key].add(obj.item_hash)
 
     def remove_record(self, obj: R):
         """Removes a record from the index, i.e. when it is forgotten."""
-        assert obj.id_hash is not None
+        assert obj.item_hash is not None
         key = attrgetter(*self.index_on)(obj)
         if isinstance(key, str):
             key = (key,)
         if key in self.hashmap:
-            self.hashmap[key].remove(obj.id_hash)
+            self.hashmap[key].remove(obj.item_hash)
 
     def regenerate(self, items: List[R]):
         """Regenerates the index with given items."""
         self.hashmap = {}
         for item in items:
             self.add_record(item)
 
@@ -735,31 +735,31 @@
             channel: The channel to post the object to. If None, will use the configured default channel.
         Returns:
             The object with the updated revision hashes and revision number.
         """
         if channel is None:
             channel = cls.channel
         assert isinstance(obj, Record)
-        post_type = type(obj).__name__ if obj.id_hash is None else "amend"
+        post_type = type(obj).__name__ if obj.item_hash is None else "amend"
         if (
-            obj.id_hash is not None
+            obj.item_hash is not None
             and obj.signer is not None
             and obj.signer != cls.account.get_address()
         ):
             raise AlephPermissionError(
-                cls.account.get_address(), obj.id_hash, obj.signer
+                cls.account.get_address(), obj.item_hash, obj.signer
             )
         message, status = await cls.session.create_post(
             post_content=obj.content,
             post_type=post_type,
             channel=channel,
-            ref=obj.id_hash,
+            ref=obj.item_hash,
         )
-        if obj.id_hash is None:
-            obj.id_hash = message.item_hash
+        if obj.item_hash is None:
+            obj.item_hash = message.item_hash
         obj.revision_hashes.append(message.item_hash)
         obj.current_revision = len(obj.revision_hashes) - 1
         obj.timestamp = message.time
         obj.signer = message.sender
         if cls.cache:
             await cls.cache.set(message.item_hash, obj.json())
         return obj
@@ -776,21 +776,21 @@
             objs: The objects to forget.
             channel: The channel to delete the object from. If None, will use the configured default channel.
         """
         if channel is None:
             channel = cls.channel
         hashes = []
         for obj in objs:
-            if obj.id_hash is None:
+            if obj.item_hash is None:
                 raise ValueError("Cannot forget an object that has not been posted.")
             if obj.signer != cls.account.get_address():
                 raise AlephPermissionError(
-                    obj.signer, obj.id_hash, cls.account.get_address()
+                    obj.signer, obj.item_hash, cls.account.get_address()
                 )
-            hashes += [obj.id_hash] + obj.revision_hashes
+            hashes += [obj.item_hash] + obj.revision_hashes
         forget_task = cls.session.forget(
             hashes=hashes,
             reason=None,
             channel=channel,
         )
         if cls.cache:
             await asyncio.gather(forget_task, *[cls.cache.delete(h) for h in hashes])
@@ -831,15 +831,15 @@
         returned_records = 0
 
         if cls.cache and item_hashes is not None:
             # TODO: Add some kind of caching for channels and owners or add recent item_hashes endpoint to the Aleph API
             records = await cls._fetch_records_from_cache(record_type, item_hashes)
             cached_ids = []
             for record in records:
-                cached_ids.append(record.id_hash)
+                cached_ids.append(record.item_hash)
                 record.changed = False
                 yield record
                 if page:
                     # If we are fetching a specific page, we need to track the number of records returned
                     # as the cache does not know about the pagination
                     returned_records += 1
                     if returned_records >= page_size:
```

### Comparing `aars-0.6.0/src/aars/exceptions.py` & `aars-0.7.0/src/aars/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     def __init__(
         self,
         content,
         message="Object '{0}' has already been forgotten. It is recommended to delete the "
         "called object locally.",
     ):
-        self.item_hash = content.id_hash
+        self.item_hash = content.item_hash
         self.message = f"{message.format(self.item_hash)}"
         super().__init__(self.message)
 
 
 class PostTypeIsNoClassError(AlephError):
     """Exception raised when a received post_type is not resolvable to any python class in current runtime."""
```

### Comparing `aars-0.6.0/src/aars/utils.py` & `aars-0.7.0/src/aars/utils.py`

 * *Files identical despite different names*

### Comparing `aars-0.6.0/tests/aars.py` & `aars-0.7.0/tests/aars.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
     book = await Book(title="Neurodancer", author="William Gibson").save()
     assert book.current_revision == 0
     book.title = "Neuromancer"
     book = await book.save()
     assert book.title == "Neuromancer"
     assert len(book.revision_hashes) == 2
     assert book.current_revision == 1
-    assert book.revision_hashes[0] == book.id_hash
-    assert book.revision_hashes[1] != book.id_hash
+    assert book.revision_hashes[0] == book.item_hash
+    assert book.revision_hashes[1] != book.item_hash
     await asyncio.sleep(1)
     old_book = await book.fetch_revision(rev_no=0)
     old_timestamp = old_book.timestamp
     assert old_book.title == "Neurodancer"
     new_book = await book.fetch_revision(rev_no=1)
     assert new_book.title == "Neuromancer"
     assert new_book.timestamp > old_timestamp
@@ -129,15 +129,15 @@
     forgettable_book = await Book(
         title="The Forgotten Book", author="Mechthild Gläser"
     ).save()  # I'm sorry.
     await asyncio.sleep(1)
     await forgettable_book.forget()
     assert forgettable_book.forgotten is True
     await asyncio.sleep(1)
-    assert len(await Book.fetch(forgettable_book.id_hash).all()) == 0
+    assert len(await Book.fetch(forgettable_book.item_hash).all()) == 0
     with pytest.raises(AlreadyForgottenError):
         await forgettable_book.forget()
 
 
 @pytest.mark.asyncio
 async def test_store_and_wrong_where_eq():
     new_book = await Book(title="Atlas Shrugged", author="Ayn Rand").save()
@@ -162,15 +162,15 @@
         title: str
         author: dict
 
     book = await BookWithDictAuthor(
         title="Test Book", author={"first": "John", "last": "Doe"}
     ).save()
     await asyncio.sleep(1)
-    fetched_book = await BookWithDictAuthor.fetch(book.id_hash).first()
+    fetched_book = await BookWithDictAuthor.fetch(book.item_hash).first()
     assert fetched_book.author == {"first": "John", "last": "Doe"}
 
 
 @pytest.mark.asyncio
 async def test_negative_limit_pagination():
     with pytest.raises(ValueError):
         await Book.fetch_objects().page(1, -1)
```

### Comparing `aars-0.6.0/.gitignore` & `aars-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aars-0.6.0/LICENSE` & `aars-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aars-0.6.0/README.md` & `aars-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aars-0.6.0/pyproject.toml` & `aars-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aars"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="Mike Hukiewitz", email="mike.hukiewitz@robotter.ai" },
 ]
 description = "Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aars-0.6.0/PKG-INFO` & `aars-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aars
-Version: 0.6.0
+Version: 0.7.0
 Summary: Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im
 Project-URL: Homepage, https://github.com/aleph-im/active-record-sdk
 Project-URL: Bug Tracker, https://github.com/aleph-im/active-record-sdk/issues
 Author-email: Mike Hukiewitz <mike.hukiewitz@robotter.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

