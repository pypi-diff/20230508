# Comparing `tmp/strangeworks_python_core-0.1.6.tar.gz` & `tmp/strangeworks_python_core-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_python_core-0.1.6.tar", max compression
+gzip compressed data, was "strangeworks_python_core-0.1.7.tar", max compression
```

## Comparing `strangeworks_python_core-0.1.6.tar` & `strangeworks_python_core-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      655 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/README.md
--rw-r--r--   0        0        0      726 2023-03-10 18:41:09.336812 strangeworks_python_core-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       19 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/__init__.py
--rw-r--r--   0        0        0       19 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/config/__init__.py
--rw-r--r--   0        0        0      647 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/config/base.py
--rw-r--r--   0        0        0     3340 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/config/config.py
--rw-r--r--   0        0        0      874 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/config/defaults.py
--rw-r--r--   0        0        0     1846 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/config/env.py
--rw-r--r--   0        0        0     6262 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/config/file.py
--rw-r--r--   0        0        0       19 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/errors/__init__.py
--rw-r--r--   0        0        0     2613 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/errors/error.py
--rw-r--r--   0        0        0       19 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/platform/__init__.py
--rw-r--r--   0        0        0     2457 2023-03-10 18:40:52.813068 strangeworks_python_core-0.1.6/strangeworks_core/platform/auth.py
--rw-r--r--   0        0        0     4842 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/platform/gql.py
--rw-r--r--   0        0        0    10844 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/platform/rest_client.py
--rw-r--r--   0        0        0     3275 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/platform/transport.py
--rw-r--r--   0        0        0       19 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/types/__init__.py
--rw-r--r--   0        0        0     3572 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/types/backend.py
--rw-r--r--   0        0        0     2024 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/types/file.py
--rw-r--r--   0        0        0     5748 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/types/job.py
--rw-r--r--   0        0        0     1088 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/types/product.py
--rw-r--r--   0        0        0     2162 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/types/resource.py
--rw-r--r--   0        0        0      553 2023-03-10 18:40:52.817068 strangeworks_python_core-0.1.6/strangeworks_core/utils.py
--rw-r--r--   0        0        0     1392 1970-01-01 00:00:00.000000 strangeworks_python_core-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      655 2023-05-08 21:46:50.603784 strangeworks_python_core-0.1.7/README.md
+-rw-r--r--   0        0        0      725 2023-05-08 21:47:06.275983 strangeworks_python_core-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       19 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/__init__.py
+-rw-r--r--   0        0        0       19 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/config/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/config/base.py
+-rw-r--r--   0        0        0     3340 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/config/config.py
+-rw-r--r--   0        0        0      874 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/config/defaults.py
+-rw-r--r--   0        0        0     1846 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/config/env.py
+-rw-r--r--   0        0        0     6262 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/config/file.py
+-rw-r--r--   0        0        0       19 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/errors/__init__.py
+-rw-r--r--   0        0        0     2613 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/errors/error.py
+-rw-r--r--   0        0        0       19 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/platform/__init__.py
+-rw-r--r--   0        0        0     2457 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/platform/auth.py
+-rw-r--r--   0        0        0     4842 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/platform/gql.py
+-rw-r--r--   0        0        0    10844 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/platform/rest_client.py
+-rw-r--r--   0        0        0     3275 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/platform/transport.py
+-rw-r--r--   0        0        0       19 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/types/__init__.py
+-rw-r--r--   0        0        0     3572 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/types/backend.py
+-rw-r--r--   0        0        0     2024 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/types/file.py
+-rw-r--r--   0        0        0     5748 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/types/job.py
+-rw-r--r--   0        0        0     1088 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/types/product.py
+-rw-r--r--   0        0        0     2420 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/types/resource.py
+-rw-r--r--   0        0        0      553 2023-05-08 21:46:50.607784 strangeworks_python_core-0.1.7/strangeworks_core/utils.py
+-rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 strangeworks_python_core-0.1.7/PKG-INFO
```

### Comparing `strangeworks_python_core-0.1.6/README.md` & `strangeworks_python_core-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/pyproject.toml` & `strangeworks_python_core-0.1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "strangeworks-python-core"
-version = "0.1.6"
+version = "0.1.7"
 description = "Strangeworks Core provides the infrastructure to interact with the platform."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_core"}]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.2"
 tomlkit = "^0.11.6"
 gql = "^3.4.0"
-requests-toolbelt = "^0.10.1"
+requests-toolbelt = "^1.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
```

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/config/base.py` & `strangeworks_python_core-0.1.7/strangeworks_core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/config/config.py` & `strangeworks_python_core-0.1.7/strangeworks_core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/config/defaults.py` & `strangeworks_python_core-0.1.7/strangeworks_core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/config/env.py` & `strangeworks_python_core-0.1.7/strangeworks_core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/config/file.py` & `strangeworks_python_core-0.1.7/strangeworks_core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/errors/error.py` & `strangeworks_python_core-0.1.7/strangeworks_core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/platform/auth.py` & `strangeworks_python_core-0.1.7/strangeworks_core/platform/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/platform/gql.py` & `strangeworks_python_core-0.1.7/strangeworks_core/platform/gql.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/platform/rest_client.py` & `strangeworks_python_core-0.1.7/strangeworks_core/platform/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/platform/transport.py` & `strangeworks_python_core-0.1.7/strangeworks_core/platform/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/types/backend.py` & `strangeworks_python_core-0.1.7/strangeworks_core/types/backend.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/types/file.py` & `strangeworks_python_core-0.1.7/strangeworks_core/types/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/types/job.py` & `strangeworks_python_core-0.1.7/strangeworks_core/types/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/types/product.py` & `strangeworks_python_core-0.1.7/strangeworks_core/types/product.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/types/resource.py` & `strangeworks_python_core-0.1.7/strangeworks_core/types/resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,20 +59,25 @@
 
         Return
         ------
         An intance of the Resource object.
         """
         return cls(**d)
 
-    def proxy_url(self) -> str:
+    def proxy_url(self, path: Optional[str] = None) -> str:
         """Return the proxy URL for the resource.
 
         Parameters
         ----------
-        None
+        path: Optional[str]
+            additional path to append to the proxy url. Defaults to None.
 
         Returns
         ------
         str:
            url that the proxy will use to make calls to the resource.
         """
-        return f"/products/{self.product.slug}/resource/{self.slug}/"
+        return (
+            f"/products/{self.product.slug}/resource/{self.slug}/"
+            if path is None
+            else f"/products/{self.product.slug}/resource/{self.slug}/{path.strip('/')}"
+        )
```

### Comparing `strangeworks_python_core-0.1.6/strangeworks_core/utils.py` & `strangeworks_python_core-0.1.7/strangeworks_core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_python_core-0.1.6/PKG-INFO` & `strangeworks_python_core-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strangeworks-python-core
-Version: 0.1.6
+Version: 0.1.7
 Summary: Strangeworks Core provides the infrastructure to interact with the platform.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
 Description-Content-Type: text/markdown
 
 # Strangeworks Python Core Library
 
 The Strangeworks Python Core Library provides commonly used things.
```

