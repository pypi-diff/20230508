# Comparing `tmp/async_rotating_proxy-0.0.5.tar.gz` & `tmp/async_rotating_proxy-0.0.6.tar.gz`

## Comparing `async_rotating_proxy-0.0.5.tar` & `async_rotating_proxy-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/requirements.txt
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/src/async_rotating_proxy/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/src/async_rotating_proxy/browser.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.6/src/async_rotating_proxy/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.6/src/async_rotating_proxy/browser.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.6/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.6/PKG-INFO
```

### Comparing `async_rotating_proxy-0.0.5/src/async_rotating_proxy/__init__.py` & `async_rotating_proxy-0.0.6/src/async_rotating_proxy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         else:
             proxy = f"{proxy_scheme}://{proxy}"
 
         # Get the page and return HTML response
         async with aiohttp.ClientSession() as session:
             headers = Headers(headers=True).generate() if fake_headers else {}
 
+            headers["Accept-Encoding"] = "*" # Because aiohttp does not support Brotli
+
             async with session.get(url, proxy=proxy, headers=headers) as response:
                 html = await response.content.read()
                 return HTMLResponse(html.decode())
 
     return app
```

### Comparing `async_rotating_proxy-0.0.5/src/async_rotating_proxy/browser.py` & `async_rotating_proxy-0.0.6/src/async_rotating_proxy/browser.py`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.5/LICENSE.txt` & `async_rotating_proxy-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.5/README.md` & `async_rotating_proxy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.5/pyproject.toml` & `async_rotating_proxy-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "async_rotating_proxy"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="Greg Bizup", email="g.bizup@gmail.com" }
 ]
 description = "Run an API on your local machine that reroutes traffic through rotating proxies. Useful for pyppeteer proxy rotation."
 readme = "README.md"
 requires-python = ">3.10"
 classifiers = [
```

### Comparing `async_rotating_proxy-0.0.5/PKG-INFO` & `async_rotating_proxy-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_rotating_proxy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Run an API on your local machine that reroutes traffic through rotating proxies. Useful for pyppeteer proxy rotation.
 Project-URL: Homepage, https://github.com/gbiz123/async-rotating-proxy
 Author-email: Greg Bizup <g.bizup@gmail.com>
 License-File: LICENSE.txt
 Keywords: fastapi,proxy,pyppeteer,rotating proxy,scraping
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

