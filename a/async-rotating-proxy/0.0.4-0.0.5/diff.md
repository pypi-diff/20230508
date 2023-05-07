# Comparing `tmp/async_rotating_proxy-0.0.4.tar.gz` & `tmp/async_rotating_proxy-0.0.5.tar.gz`

## Comparing `async_rotating_proxy-0.0.4.tar` & `async_rotating_proxy-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/requirements.txt
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/src/async_rotating_proxy/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/src/async_rotating_proxy/browser.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/README.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/src/async_rotating_proxy/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/src/async_rotating_proxy/browser.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/PKG-INFO
```

### Comparing `async_rotating_proxy-0.0.4/src/async_rotating_proxy/__init__.py` & `async_rotating_proxy-0.0.5/src/async_rotating_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.4/src/async_rotating_proxy/browser.py` & `async_rotating_proxy-0.0.5/src/async_rotating_proxy/browser.py`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.4/LICENSE.txt` & `async_rotating_proxy-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.4/README.md` & `async_rotating_proxy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.4/pyproject.toml` & `async_rotating_proxy-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "async_rotating_proxy"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Greg Bizup", email="g.bizup@gmail.com" }
 ]
 description = "Run an API on your local machine that reroutes traffic through rotating proxies. Useful for pyppeteer proxy rotation."
 readme = "README.md"
 requires-python = ">3.10"
 classifiers = [
@@ -24,11 +24,12 @@
     "scraping",
 ]
 dependencies = [
     "aiohttp >= 3.8.4",
     "fastapi >= 0.95.1",
     "pyppeteer >= 1.0.2",
     "uvicorn >= 0.21.1",
+    "fake_headers >= 1.0.2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/gbiz123/async-rotating-proxy"
```

### Comparing `async_rotating_proxy-0.0.4/PKG-INFO` & `async_rotating_proxy-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: async_rotating_proxy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Run an API on your local machine that reroutes traffic through rotating proxies. Useful for pyppeteer proxy rotation.
 Project-URL: Homepage, https://github.com/gbiz123/async-rotating-proxy
 Author-email: Greg Bizup <g.bizup@gmail.com>
 License-File: LICENSE.txt
 Keywords: fastapi,proxy,pyppeteer,rotating proxy,scraping
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >3.10
 Requires-Dist: aiohttp>=3.8.4
+Requires-Dist: fake-headers>=1.0.2
 Requires-Dist: fastapi>=0.95.1
 Requires-Dist: pyppeteer>=1.0.2
 Requires-Dist: uvicorn>=0.21.1
 Description-Content-Type: text/markdown
 
 # async-rotating-proxy
 Run an API on your local machine that reroutes traffic through rotating proxies.
```

