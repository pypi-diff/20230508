# Comparing `tmp/detabase-0.2.1.tar.gz` & `tmp/detabase-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detabase-0.2.1.tar", max compression
+gzip compressed data, was "detabase-0.2.2.tar", max compression
```

## Comparing `detabase-0.2.1.tar` & `detabase-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,18 @@
--rw-r--r--   0        0        0       30 2023-02-18 04:20:02.724322 detabase-0.2.1/detabase/__init__.py
--rw-r--r--   0        0        0     5986 2023-02-26 01:51:26.703025 detabase-0.2.1/detabase/engine.py
--rw-r--r--   0        0        0      354 2023-02-26 01:53:17.624943 detabase-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      613 2023-02-26 01:53:23.900100 detabase-0.2.1/setup.py
--rw-r--r--   0        0        0      376 2023-02-26 01:53:23.900293 detabase-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      408 2023-05-07 12:41:54.704060 detabase-0.2.2/detabase/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-07 02:23:49.679517 detabase-0.2.2/detabase/base_models.py
+-rw-r--r--   0        0        0     4592 2023-05-07 14:57:05.715206 detabase-0.2.2/detabase/casting.py
+-rw-r--r--   0        0        0     4419 2023-05-06 16:53:36.189206 detabase-0.2.2/detabase/config.py
+-rw-r--r--   0        0        0     3229 2023-05-07 22:59:19.779776 detabase-0.2.2/detabase/constants.py
+-rw-r--r--   0        0        0     2297 2023-05-07 22:24:17.389745 detabase-0.2.2/detabase/context.py
+-rw-r--r--   0        0        0     8376 2023-05-07 18:26:36.406632 detabase-0.2.2/detabase/descriptor.py
+-rw-r--r--   0        0        0    10149 2023-05-07 22:33:57.443611 detabase-0.2.2/detabase/deta_model.py
+-rw-r--r--   0        0        0     5487 2023-05-07 22:32:30.399216 detabase-0.2.2/detabase/engine.py
+-rw-r--r--   0        0        0     1346 2023-05-07 23:00:35.871930 detabase-0.2.2/detabase/enums.py
+-rw-r--r--   0        0        0     1078 2023-05-07 22:37:24.714167 detabase-0.2.2/detabase/form.py
+-rw-r--r--   0        0        0     1589 2023-05-07 02:26:17.056907 detabase-0.2.2/detabase/json_encoder.py
+-rw-r--r--   0        0        0      520 2023-05-06 19:28:05.417332 detabase-0.2.2/detabase/protocols.py
+-rw-r--r--   0        0        0     3005 2023-05-07 22:50:49.459643 detabase-0.2.2/detabase/regex.py
+-rw-r--r--   0        0        0     3793 2023-05-07 02:39:12.720415 detabase-0.2.2/detabase/types.py
+-rw-r--r--   0        0        0      480 2023-05-07 23:10:18.609285 detabase-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      768 2023-05-07 23:20:35.471364 detabase-0.2.2/setup.py
+-rw-r--r--   0        0        0      586 2023-05-07 23:20:35.471563 detabase-0.2.2/PKG-INFO
```

### Comparing `detabase-0.2.1/detabase/engine.py` & `detabase-0.2.2/detabase/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 __all__ = [
-		'DetaBase'
+		'DetaBase',
 ]
 
-import datetime
 from typing import Union, Optional
 from deta import Deta
+from detabase.types import *
 
-import os.path
+# import os.path
+#
+# from starlette.config import Config
 
-from starlette.config import Config
+from detabase.config import DetaConfig
 
-JsonPrimitive = Union[str, float, int, bool, None]
-DetaData = Union[dict, list, str, float, int, bool]
-DetaKey = Union[str, None]
-ExpireIn = Union[str, None]
-ExpireAt = Union[datetime.datetime, int, float, None]
-JsonSequence = list[JsonPrimitive]
-JsonDict = dict[str, Union[JsonSequence, JsonPrimitive]]
-Jsonable = Union[JsonDict, JsonSequence, JsonPrimitive]
-DetaQuery = Union[dict[str, JsonPrimitive], list[dict[str, JsonPrimitive]]]
 
-config = Config(os.path.join(os.getcwd(), '.env'))
+config = DetaConfig()
 
 
 class DetaBase:
 	
 	def __init__(self, table: str, project_key: str = None):
 		self.table = table
 		self.project_key = project_key
 	
 	def async_base(self):
-		return Deta(self.project_key or config.get("DETABASE_PROJECT_KEY", default='DETA_PROJECT_KEY', cast=str)).AsyncBase(self.table)
+		return Deta(self.project_key or config.detabase_project_key).AsyncBase(self.table)
 	
 	async def put_many(self, items: list[Jsonable], expire_in: ExpireIn = None, expire_at: ExpireAt = None):
 		base = self.async_base()
 		processed = dict(items=list())
 		failed = dict(items=list())
 		try:
 			loops = (len(items) - (len(items) % 20)) / 20
 			gen = (item for item in items)
 			while loops > 0:
 				result = await base.put_many(items=[next(gen) for _ in range(20)], expire_in=expire_in,
 				                             expire_at=expire_at)
-				processed['items'].extend(result.get('processed', {}).get('items', list()))
-				failed['items'].extend(result.get('failed', {}).get('items', list()))
+				processed['items'].extend(result.get('processed').get('items'))
+				failed['items'].extend(result.get('failed').get('items'))
 				loops -= 1
 			missing = list(gen)
 			if len(missing) > 0:
 				result = await base.put_many(items=list(gen), expire_in=expire_in, expire_at=expire_at)
-				processed['items'].extend(result.get('processed', {}).get('items', list()))
-				failed['items'].extend(result.get('failed', {}).get('items', list()))
+				processed['items'].extend(result.get('processed').get('items'))
+				failed['items'].extend(result.get('failed').get('items'))
 			return {'processed': processed, 'failed': failed}
 		except StopIteration:
 			pass
 		finally:
 			await base.close()
 			
 	async def put(self, data: DetaData, key: DetaKey = None, expire_in: ExpireIn = None, expire_at: ExpireAt = None):
```

