# Comparing `tmp/merqube_client_lib-0.5.2.tar.gz` & `tmp/merqube_client_lib-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.5.2.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.5.3.tar", max compression
```

## Comparing `merqube_client_lib-0.5.2.tar` & `merqube_client_lib-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/LICENSE
--rw-r--r--   0        0        0      377 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/README.md
--rw-r--r--   0        0        0        0 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0      367 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0     1934 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/logging.py
--rw-r--r--   0        0        0     3022 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/mocker.py
--rw-r--r--   0        0        0        0 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/py.typed
--rw-r--r--   0        0        0        0 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/secapi/__init__.py
--rw-r--r--   0        0        0    12450 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/secapi/client.py
--rw-r--r--   0        0        0    11209 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/session.py
--rw-r--r--   0        0        0      351 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/types/__init__.py
--rw-r--r--   0        0        0      418 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/types/secapi.py
--rw-r--r--   0        0        0      677 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/util.py
--rw-r--r--   0        0        0     1713 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/LICENSE
+-rw-r--r--   0        0        0      377 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0      367 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0     3028 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/mocker.py
+-rw-r--r--   0        0        0        0 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0        0 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/secapi/__init__.py
+-rw-r--r--   0        0        0    12490 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/secapi/client.py
+-rw-r--r--   0        0        0    11209 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      351 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/types/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/types/secapi.py
+-rw-r--r--   0        0        0      677 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/util.py
+-rw-r--r--   0        0        0     1713 2023-05-08 16:36:12.896175 merqube_client_lib-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.5.3/PKG-INFO
```

### Comparing `merqube_client_lib-0.5.2/LICENSE` & `merqube_client_lib-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.2/merqube_client_lib/logging.py` & `merqube_client_lib-0.5.3/merqube_client_lib/logging.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.2/merqube_client_lib/mocker.py` & `merqube_client_lib-0.5.3/merqube_client_lib/mocker.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,14 @@
         # inside
 
         for method_name, func in method_name_function_map.items():
             if getattr(client, method_name) is None:
                 raise ValueError("Trying to patch a function that doesnt exist in the client")
             setattr(client, method_name, func)
 
-        def get_client(key: str = "unused"):
+        def get_client(*args: Any, **kwargs: Any):
             return client
 
         # now a get_client call from the main code will return this mocked client:
         monkeypatch.setattr(get_client_function_path, get_client)
 
     return mock_secapi
```

### Comparing `merqube_client_lib-0.5.2/merqube_client_lib/secapi/client.py` & `merqube_client_lib-0.5.3/merqube_client_lib/secapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 class _ClientBase:
     """
     base class that contains validation functions
     """
 
     def __init__(
         self,
-        session: Optional[MerqubeAPISession] = None,
+        user_session: Optional[MerqubeAPISession] = None,
         token: Optional[str] = None,
         **session_kwargs: Any,
     ):
-        self.session = session or get_merqube_session(token=token, **session_kwargs)
+        self.session = user_session or get_merqube_session(token=token, **session_kwargs)
         self.type_cache = TTLCache(1, ttl=DEFAULT_CACHE_TTL)  # type: ignore
 
     def _collection_helper(
         self,
         *,
         url: str,
         query_options: dict[str, str | Iterable[str] | None] | None = None,
@@ -128,19 +128,19 @@
 class SecAPIClient(_ClientBase):
     """
     Secapi client class
     """
 
     def __init__(
         self,
-        session: Optional[MerqubeAPISession] = None,
+        user_session: Optional[MerqubeAPISession] = None,
         token: Optional[str] = None,
         **session_kwargs: Any,
     ):
-        super().__init__(session=session, token=token, **session_kwargs)
+        super().__init__(user_session=user_session, token=token, **session_kwargs)
 
     def _get_security_metrics_helper(
         self,
         *,
         sec_type: str,
         metrics: str | Iterable[str],
         sec_names: str | Iterable[str] | None = None,
@@ -309,13 +309,13 @@
 
 
 secapi_client_cache: LRUCache = LRUCache(maxsize=256)  # type: ignore
 
 
 @cached(cache=secapi_client_cache)
 def get_client(
-    session: Optional[MerqubeAPISession] = None, token: Optional[str] = None, **session_kwargs: Any
+    user_session: Optional[MerqubeAPISession] = None, token: Optional[str] = None, **session_kwargs: Any
 ) -> SecAPIClient:
     """
     Cached; returns a secapi client for token
     """
-    return SecAPIClient(session=session, token=token, **session_kwargs)
+    return SecAPIClient(user_session=user_session, token=token, **session_kwargs)
```

### Comparing `merqube_client_lib-0.5.2/merqube_client_lib/session.py` & `merqube_client_lib-0.5.3/merqube_client_lib/session.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.2/merqube_client_lib/util.py` & `merqube_client_lib-0.5.3/merqube_client_lib/util.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.2/pyproject.toml` & `merqube_client_lib-0.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.5.2"
+version = "0.5.3"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
```

