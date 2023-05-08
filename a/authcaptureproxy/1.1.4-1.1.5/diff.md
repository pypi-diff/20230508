# Comparing `tmp/authcaptureproxy-1.1.4.tar.gz` & `tmp/authcaptureproxy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authcaptureproxy-1.1.4.tar", max compression
+gzip compressed data, was "authcaptureproxy-1.1.5.tar", max compression
```

## Comparing `authcaptureproxy-1.1.4.tar` & `authcaptureproxy-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     8489 2022-06-25 21:49:30.665280 authcaptureproxy-1.1.4/CHANGELOG.md
--rw-r--r--   0        0        0    10889 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/LICENSE.txt
--rw-r--r--   0        0        0     2512 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/README.md
--rw-r--r--   0        0        0     1885 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/authcaptureproxy/__init__.py
--rw-r--r--   0        0        0    28265 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/authcaptureproxy/auth_capture_proxy.py
--rw-r--r--   0        0        0     5979 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/authcaptureproxy/cli.py
--rw-r--r--   0        0        0      139 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/authcaptureproxy/const.py
--rw-r--r--   0        0        0       78 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/authcaptureproxy/examples/__init__.py
--rw-r--r--   0        0        0     8785 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/authcaptureproxy/examples/modifiers.py
--rw-r--r--   0        0        0     1406 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/authcaptureproxy/examples/testers.py
--rw-r--r--   0        0        0     8468 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/authcaptureproxy/helper.py
--rw-r--r--   0        0        0     1662 2022-06-25 21:49:29.637259 authcaptureproxy-1.1.4/authcaptureproxy/stackoverflow.py
--rw-r--r--   0        0        0    15394 2022-06-25 21:49:30.681280 authcaptureproxy-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3627 2022-06-25 21:49:41.109254 authcaptureproxy-1.1.4/setup.py
--rw-r--r--   0        0        0     4206 2022-06-25 21:49:41.109698 authcaptureproxy-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     8670 2023-05-07 08:11:09.231574 authcaptureproxy-1.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0    10889 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     2512 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/README.md
+-rw-r--r--   0        0        0     1885 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/authcaptureproxy/__init__.py
+-rw-r--r--   0        0        0    28304 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/authcaptureproxy/auth_capture_proxy.py
+-rw-r--r--   0        0        0     5979 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/authcaptureproxy/cli.py
+-rw-r--r--   0        0        0      139 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/authcaptureproxy/const.py
+-rw-r--r--   0        0        0       78 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/authcaptureproxy/examples/__init__.py
+-rw-r--r--   0        0        0     8824 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/authcaptureproxy/examples/modifiers.py
+-rw-r--r--   0        0        0     1406 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/authcaptureproxy/examples/testers.py
+-rw-r--r--   0        0        0     8468 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/authcaptureproxy/helper.py
+-rw-r--r--   0        0        0     1662 2023-05-07 08:11:08.383560 authcaptureproxy-1.1.5/authcaptureproxy/stackoverflow.py
+-rw-r--r--   0        0        0    15394 2023-05-07 08:11:09.239574 authcaptureproxy-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4357 1970-01-01 00:00:00.000000 authcaptureproxy-1.1.5/PKG-INFO
```

### Comparing `authcaptureproxy-1.1.4/CHANGELOG.md` & `authcaptureproxy-1.1.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog for auth_capture_proxy
 
 <!--next-version-placeholder-->
 
+## v1.1.5 (2023-05-07)
+### Fix
+* **access_url:** Do not add port if 0 ([`ba9acb4`](https://github.com/alandtse/auth_capture_proxy/commit/ba9acb49f106a76c32f95ef3ef871444309597e0))
+
 ## v1.1.4 (2022-06-25)
 ### Fix
 * Fix swap_url for http converted urls ([`2b672fa`](https://github.com/alandtse/auth_capture_proxy/commit/2b672fa3a9c86ecf4dd64d7fc7d66a8a7fa1d5ff))
 
 ## v1.1.3 (2022-02-25)
 ### Fix
 * Bump multidict ([`bf8c7c1`](https://github.com/alandtse/auth_capture_proxy/commit/bf8c7c13252d2042f07a8ad2de1e6aba188e6985))
```

### Comparing `authcaptureproxy-1.1.4/LICENSE.txt` & `authcaptureproxy-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.4/README.md` & `authcaptureproxy-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.4/authcaptureproxy/__init__.py` & `authcaptureproxy-1.1.5/authcaptureproxy/__init__.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.4/authcaptureproxy/auth_capture_proxy.py` & `authcaptureproxy-1.1.5/authcaptureproxy/auth_capture_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         """
         self.refresh_modifiers()  # refresh in case of pending change
         self._old_modifiers = self._modifiers
         self._modifiers = value
 
     def access_url(self) -> URL:
         """Return access url for proxy with port."""
-        return self._proxy_url.with_port(self.port)
+        return self._proxy_url.with_port(self.port) if self.port != 0 else self._proxy_url
 
     async def change_host_url(self, new_url: URL) -> None:
         """Change the host url of the proxy.
 
         This will also reset all stored data.
 
         Args:
```

### Comparing `authcaptureproxy-1.1.4/authcaptureproxy/cli.py` & `authcaptureproxy-1.1.5/authcaptureproxy/cli.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.4/authcaptureproxy/examples/modifiers.py` & `authcaptureproxy-1.1.5/authcaptureproxy/examples/modifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,17 @@
     if not base_url:
         _LOGGER.debug("No base_url specified")
         return html
     return await find_urls_bs4(partial(prepend_url, base_url), search={}, exceptions={}, html=html)
 
 
 async def find_regex_urls(
-    modifier: Optional[Callable] = None, patterns: Dict[Text, Text] = None, html: Text = ""
+    modifier: Optional[Callable] = None,
+    patterns: Optional[Dict[Text, Text]] = None,
+    html: Text = "",
 ) -> Text:
     """Find urls for based on regex.
 
     Seen in Tesla login with MFA enabled.
 
     Args:
         modifier (Optional[Callable], optional): The function to call. It will take in the html_tag, tag, and attribute and modify the html_tag. Defaults to None.
@@ -151,16 +153,16 @@
             _LOGGER.debug("Replacing %s -> %s", url_string, str(new_url))
             html = re.sub(re.escape(url_string), str(new_url), html, re.IGNORECASE)
     return html
 
 
 async def find_urls_bs4(
     modifier: Optional[Callable] = None,
-    search: Dict[Text, Text] = None,
-    exceptions: Dict[Text, List[Text]] = None,
+    search: Optional[Dict[Text, Text]] = None,
+    exceptions: Optional[Dict[Text, List[Text]]] = None,
     html: Text = "",
 ) -> Text:
     """Find urls in html using bs4.
 
     This function will search using beautifulsoup.find_all() and then apply the modifier function to the found url.
 
     Args:
```

### Comparing `authcaptureproxy-1.1.4/authcaptureproxy/examples/testers.py` & `authcaptureproxy-1.1.5/authcaptureproxy/examples/testers.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.4/authcaptureproxy/helper.py` & `authcaptureproxy-1.1.5/authcaptureproxy/helper.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.4/authcaptureproxy/stackoverflow.py` & `authcaptureproxy-1.1.5/authcaptureproxy/stackoverflow.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.4/pyproject.toml` & `authcaptureproxy-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # This is the version of your project. Keep it up-to-date and follow semantic versioning.
 # It's used in the PyPi, wheels, Docker, and Github packages.
 # Also make sure to use exactly this version when creating a Github release,
 # but prefix a "v" to the Github release.
 # E.g. This might be "1.2.13", and the Github release will be "v1.2.13".
 # Although semantic versioning allows for build tags (metadata),
 # not all tools are compatible with it, so avoid it if you can.
-version = "1.1.4"
+version = "1.1.5"
 
 description = "A Python project to create a proxy to capture authentication information from a webpage. This is useful to capture oauth login details without access to a third-party oauth."
 keywords = [""]
 authors = ["Alan D. Tse"]
 maintainers = ["Alan D. Tse"]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `authcaptureproxy-1.1.4/PKG-INFO` & `authcaptureproxy-1.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: authcaptureproxy
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python project to create a proxy to capture authentication information from a webpage. This is useful to capture oauth login details without access to a third-party oauth.
 Home-page: https://github.com/alandtse/auth_capture_proxy
 License: Apache-2.0
 Author: Alan D. Tse
 Maintainer: Alan D. Tse
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Requires-Dist: aiohttp (>=3,<4)
 Requires-Dist: beautifulsoup4 (>=4,<5)
 Requires-Dist: httpx
 Requires-Dist: importlib-metadata (>=3.4.0)
 Requires-Dist: multidict (>=6,<7)
```

