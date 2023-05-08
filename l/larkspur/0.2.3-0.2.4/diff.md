# Comparing `tmp/larkspur-0.2.3.tar.gz` & `tmp/larkspur-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "larkspur-0.2.3.tar", max compression
+gzip compressed data, was "larkspur-0.2.4.tar", max compression
```

## Comparing `larkspur-0.2.3.tar` & `larkspur-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2022-10-11 15:02:31.654877 larkspur-0.2.3/LICENSE
--rw-r--r--   0        0        0      105 2022-10-11 15:02:31.655146 larkspur-0.2.3/larkspur/__init__.py
--rwxr-xr-x   0        0        0     1598 2022-10-11 15:02:31.655220 larkspur-0.2.3/larkspur/benchmarks.py
--rw-r--r--   0        0        0    16781 2023-02-14 20:27:24.227231 larkspur-0.2.3/larkspur/larkspur.py
--rwxr-xr-x   0        0        0     4658 2023-02-14 20:27:24.229534 larkspur-0.2.3/larkspur/test_larkspur.py
--rw-r--r--   0        0        0      402 2023-02-14 20:27:24.232943 larkspur-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 larkspur-0.2.3/setup.py
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 larkspur-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-10-11 15:02:31.654877 larkspur-0.2.4/LICENSE
+-rw-r--r--   0        0        0      105 2022-10-11 15:02:31.655146 larkspur-0.2.4/larkspur/__init__.py
+-rwxr-xr-x   0        0        0     1598 2022-10-11 15:02:31.655220 larkspur-0.2.4/larkspur/benchmarks.py
+-rw-r--r--   0        0        0    16976 2023-05-08 19:05:14.093930 larkspur-0.2.4/larkspur/larkspur.py
+-rwxr-xr-x   0        0        0     5082 2023-05-08 19:05:14.094336 larkspur-0.2.4/larkspur/test_larkspur.py
+-rw-r--r--   0        0        0      402 2023-05-08 19:05:59.874746 larkspur-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 larkspur-0.2.4/setup.py
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 larkspur-0.2.4/PKG-INFO
```

### Comparing `larkspur-0.2.3/LICENSE` & `larkspur-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `larkspur-0.2.3/larkspur/benchmarks.py` & `larkspur-0.2.4/larkspur/benchmarks.py`

 * *Files identical despite different names*

### Comparing `larkspur-0.2.3/larkspur/larkspur.py` & `larkspur-0.2.4/larkspur/larkspur.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,19 @@
         self.error_rate = meta.get('error_rate') or error_rate
         self.scale = meta.get('scale') or scale
         self.ratio = meta.get('ratio') or ratio
         self.threshold_scale = meta.get('threshold_scale') or threshold_scale
         self.initial_capacity = meta.get('initial_capacity') or initial_capacity
         if not self.connection.exists(self.meta_name):
             self._create_meta()
-        filter_names = sorted(list(self.connection.smembers(self.name)))
+        filter_names = list(self.connection.smembers(self.name))
+        # Sort the bloomfilters according to their bf# as they are in format NAME:bf0
+        filter_names.sort(
+            key=lambda bf_name: int(bf_name.decode("utf-8").split(":")[-1][2:])
+        )
         self.filters = [
             BloomFilter(connection, fn.decode('utf8'), self.initial_capacity)
             for fn in filter_names
         ]
 
     def _create_meta(self):
         self.connection.hmset(self.meta_name, {
```

### Comparing `larkspur-0.2.3/larkspur/test_larkspur.py` & `larkspur-0.2.4/larkspur/test_larkspur.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,16 @@
         self.r.flushdb()
 
 
 class TestBloomFilter(LarkspurTestCase):
 
     def test_add(self):
         bf = BloomFilter(self.r, 'test', capacity=1000, error_rate=0.001)
-        members = [str(ObjectId()) for x in range(1000)]
-        nonmembers = [str(ObjectId()) for x in range(10)]
+        members = [str(ObjectId()) for _ in range(1000)]
+        nonmembers = [str(ObjectId()) for _ in range(10)]
         for oid in members:
             bf.add(oid)
         margin = 0.002 * 1000
         assert(all([oid in bf for oid in members]))
         assert(len([
             result for result in
             [oid in bf for oid in nonmembers]
@@ -33,88 +33,88 @@
             bf.add(nonmembers[1])
             bf.add(nonmembers[2])
             bf.add(nonmembers[3])
         self.assertRaises(IndexError, add_too_many)
 
     def test_bulk_add(self):
         bf = BloomFilter(self.r, 'test', capacity=1000, error_rate=0.001)
-        members = [str(ObjectId()) for x in range(1000)]
-        nonmembers = [str(ObjectId()) for x in range(10)]
+        members = [str(ObjectId()) for _ in range(1000)]
+        nonmembers = [str(ObjectId()) for _ in range(10)]
         bf.bulk_add(members)
         margin = 0.002 * 1000
         assert(all([oid in bf for oid in members]))
         assert(len([
             result for result in
             [oid in bf for oid in nonmembers]
             if result]) <= margin)
 
     def test_flush(self):
         bf = BloomFilter(self.r, 'test', capacity=1000, error_rate=0.001)
-        members = [str(ObjectId()) for x in range(1000)]
+        members = [str(ObjectId()) for _ in range(1000)]
         bf.bulk_add(members)
         assert bf.count >= 990
         bf.flush(None)
         assert bf.count == 0
         assert(all([oid not in bf for oid in members]))
 
 
 class TestScalableBloomFilter(LarkspurTestCase):
     def test_add(self):
         sbf = ScalableBloomFilter(self.r, 'test', initial_capacity=1000, error_rate=0.001)
-        members = [str(ObjectId()) for x in range(6000)]
-        nonmembers = [str(ObjectId()) for x in range(10)]
+        members = [str(ObjectId()) for _ in range(6000)]
+        nonmembers = [str(ObjectId()) for _ in range(10)]
         for oid in members:
             sbf.add(oid)
         margin = 0.002 * 6000
         assert(all([oid in sbf for oid in members]))
         assert(len([
             result for result in
             [oid in sbf for oid in nonmembers]
             if result]) <= margin)
 
     def test_bulk_add(self):
         sbf = ScalableBloomFilter(self.r, 'test', initial_capacity=1000, error_rate=0.001)
-        members = [str(ObjectId()) for x in range(6000)]
-        nonmembers = [str(ObjectId()) for x in range(10)]
+        members = [str(ObjectId()) for _ in range(6000)]
+        nonmembers = [str(ObjectId()) for _ in range(10)]
         sbf.bulk_add(members)
         margin = 0.002 * 6000
         assert(all([oid in sbf for oid in members]))
         assert(len([
             result for result in
             [oid in sbf for oid in nonmembers]
             if result]) <= margin)
 
     def test_count(self):
         sbf = ScalableBloomFilter(self.r, 'test', initial_capacity=1000, error_rate=0.001)
-        members = [str(ObjectId()) for x in range(10000)]
+        members = [str(ObjectId()) for _ in range(10000)]
         for oid in members:
             sbf.add(oid)
         assert sbf.count >= 9980
 
     def test_clear(self):
         sbf = ScalableBloomFilter(self.r, 'test', initial_capacity=1000, error_rate=0.001)
-        members = [str(ObjectId()) for x in range(6000)]
+        members = [str(ObjectId()) for _ in range(6000)]
         sbf.bulk_add(members)
         assert sbf.count >= 5988
         sbf.flush()
         assert sbf.count == 0
         assert(all([oid not in sbf for oid in members]))
 
     def test_existing_filter(self):
         sbf = ScalableBloomFilter(self.r, 'test', initial_capacity=1000, error_rate=0.001)
-        members = [str(ObjectId()) for x in range(3000)]
+        members = [str(ObjectId()) for _ in range(3000)]
         sbf.bulk_add(members)
         sbf2 = ScalableBloomFilter(self.r, 'test')
         assert sbf2.count == sbf.count
         assert sbf2.error_rate == sbf.error_rate
         assert sbf2.capacity == sbf.capacity
 
     def test_expire(self):
         sbf = ScalableBloomFilter(self.r, 'test', initial_capacity=1000, error_rate=0.001)
-        members = [str(ObjectId()) for x in range(3000)]
+        members = [str(ObjectId()) for _ in range(3000)]
         sbf.bulk_add(members)
         sbf.expire(60)
         for bf in sbf.filters:
             assert self.r.ttl(bf.name) == 60
             assert self.r.ttl(bf.meta_name) == 60
         assert self.r.ttl(sbf.name) == 60
         assert self.r.ttl(sbf.meta_name) == 60
@@ -122,7 +122,15 @@
     def test_cardinality(self):
         sbf = ScalableBloomFilter(self.r, 'test', initial_capacity=1)
         member = str(ObjectId())
         # Create a new key
         assert not sbf.add(member)
         # Try to create the same key again
         assert sbf.add(member)
+
+    def test_sort(self):
+        sbf = ScalableBloomFilter(self.r, 'test', initial_capacity=1, scale=1)
+        # Create a keys until we have double digit BloomFilters
+        [sbf.add(str(ObjectId())) for _ in range(0, 11)]
+        # Reload and nsure the last filter is filter 10
+        sbf = ScalableBloomFilter(self.r, 'test', initial_capacity=1, scale=1)
+        assert sbf.filters[-1].meta_name == "bfmeta:test:bf10"
```

### Comparing `larkspur-0.2.3/setup.py` & `larkspur-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['redis>=3.5.3,<4.0.0']
 
 setup_kwargs = {
     'name': 'larkspur',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'a Redis-backed, scalable Bloom filter',
     'long_description': 'None',
     'author': 'Thomas R Storey',
     'author_email': 'orey.st@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

