# Comparing `tmp/bevy-2.0.0b5.tar.gz` & `tmp/bevy-2.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bevy-2.0.0b5.tar", max compression
+gzip compressed data, was "bevy-2.0.0b6.tar", max compression
```

## Comparing `bevy-2.0.0b5.tar` & `bevy-2.0.0b6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-05-07 16:20:11.686032 bevy-2.0.0b5/LICENSE
--rw-r--r--   0        0        0     5859 2023-05-07 16:20:11.686032 bevy-2.0.0b5/README.md
--rw-r--r--   0        0        0      213 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/__init__.py
--rw-r--r--   0        0        0     1463 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/contextvar.py
--rw-r--r--   0        0        0     1692 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/injectors/classes.py
--rw-r--r--   0        0        0     2244 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/injectors/functions.py
--rw-r--r--   0        0        0     2717 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/options.py
--rw-r--r--   0        0        0      164 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/providers/__init__.py
--rw-r--r--   0        0        0     1631 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/providers/annotated_provider.py
--rw-r--r--   0        0        0     3423 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/providers/provider.py
--rw-r--r--   0        0        0     1153 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/providers/type_provider.py
--rw-r--r--   0        0        0     6559 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/repository.py
--rw-r--r--   0        0        0      296 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/repository_cache.py
--rw-r--r--   0        0        0      866 2023-05-07 16:20:11.686032 bevy-2.0.0b5/pyproject.toml
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 bevy-2.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-07 17:21:08.196076 bevy-2.0.0b6/LICENSE
+-rw-r--r--   0        0        0     5859 2023-05-07 17:21:08.196076 bevy-2.0.0b6/README.md
+-rw-r--r--   0        0        0      213 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/__init__.py
+-rw-r--r--   0        0        0     1463 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/contextvar.py
+-rw-r--r--   0        0        0     1692 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/injectors/classes.py
+-rw-r--r--   0        0        0     2244 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/injectors/functions.py
+-rw-r--r--   0        0        0     2717 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/options.py
+-rw-r--r--   0        0        0      164 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/providers/__init__.py
+-rw-r--r--   0        0        0     1631 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/providers/annotated_provider.py
+-rw-r--r--   0        0        0     3423 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/providers/provider.py
+-rw-r--r--   0        0        0     1153 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/providers/type_provider.py
+-rw-r--r--   0        0        0     6625 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/repository.py
+-rw-r--r--   0        0        0      296 2023-05-07 17:21:08.196076 bevy-2.0.0b6/bevy/repository_cache.py
+-rw-r--r--   0        0        0      866 2023-05-07 17:21:08.196076 bevy-2.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 bevy-2.0.0b6/PKG-INFO
```

### Comparing `bevy-2.0.0b5/LICENSE` & `bevy-2.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b5/README.md` & `bevy-2.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b5/bevy/contextvar.py` & `bevy-2.0.0b6/bevy/contextvar.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b5/bevy/injectors/classes.py` & `bevy-2.0.0b6/bevy/injectors/classes.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b5/bevy/injectors/functions.py` & `bevy-2.0.0b6/bevy/injectors/functions.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b5/bevy/options.py` & `bevy-2.0.0b6/bevy/options.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b5/bevy/providers/annotated_provider.py` & `bevy-2.0.0b6/bevy/providers/annotated_provider.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b5/bevy/providers/provider.py` & `bevy-2.0.0b6/bevy/providers/provider.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b5/bevy/providers/type_provider.py` & `bevy-2.0.0b6/bevy/providers/type_provider.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b5/bevy/repository.py` & `bevy-2.0.0b6/bevy/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,21 +50,22 @@
     ):
         self._parent = parent or _NullRepository()
         self._providers: dict[Provider[_K, _V], _RepositoryCache[_K, _V]] = {}
 
         self.add_providers(*providers)
 
     def add_providers(self, *providers: Provider[_K, _V]):
-        """Adds providers to the repository. These providers will be used to lookup and create instances that will be
-        stored and returned by the repository."""
-        self._providers.update(
-            (provider, _RepositoryCache(self))
+        """Adds providers to the repository at a higher priority than existing providers. These providers will be used
+        to lookup and create instances that will be stored and returned by the repository.
+        """
+        self._providers = {
+            provider: _RepositoryCache(self)
             for provider in providers
             if provider not in self._providers
-        )
+        } | self._providers
 
     def branch(self) -> "Repository[_K, _V]":
         """Creates a new repository that inherits the providers from the current repository. Dependencies not found on
         the new repository can be propagated to the branched parent repository. This allows the branch repository to
         inherit dependencies from the parent repository and protects the parent from changes to the branch.
         """
         return type(self)(parent=self, providers=(*self._providers,))
```

### Comparing `bevy-2.0.0b5/pyproject.toml` & `bevy-2.0.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Bevy"
-version = "2.0.0b5"
+version = "2.0.0b6"
 description = "Python Dependency Inversion made simple so you can focus on creating amazing code."
 authors = ["Zech Zimmerman <hi@zech.codes>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ZechCodes/Bevy"
 repository = "https://github.com/ZechCodes/Bevy"
 documentation = "https://github.com/ZechCodes/Bevy/blob/master/README.md"
```

### Comparing `bevy-2.0.0b5/PKG-INFO` & `bevy-2.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bevy
-Version: 2.0.0b5
+Version: 2.0.0b6
 Summary: Python Dependency Inversion made simple so you can focus on creating amazing code.
 Home-page: https://github.com/ZechCodes/Bevy
 License: MIT
 Keywords: dependency,injection,annotations,types
 Author: Zech Zimmerman
 Author-email: hi@zech.codes
 Requires-Python: >=3.10,<4.0
```

