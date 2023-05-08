# Comparing `tmp/authcaptureproxy-1.1.6.tar.gz` & `tmp/authcaptureproxy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authcaptureproxy-1.1.6.tar", max compression
+gzip compressed data, was "authcaptureproxy-1.2.0.tar", max compression
```

## Comparing `authcaptureproxy-1.1.6.tar` & `authcaptureproxy-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     8844 2023-05-08 03:06:59.791533 authcaptureproxy-1.1.6/CHANGELOG.md
--rw-r--r--   0        0        0    10889 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/LICENSE.txt
--rw-r--r--   0        0        0     2512 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/README.md
--rw-r--r--   0        0        0     1885 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/authcaptureproxy/__init__.py
--rw-r--r--   0        0        0    28304 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/authcaptureproxy/auth_capture_proxy.py
--rw-r--r--   0        0        0     5979 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/authcaptureproxy/cli.py
--rw-r--r--   0        0        0      139 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/authcaptureproxy/const.py
--rw-r--r--   0        0        0       78 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/authcaptureproxy/examples/__init__.py
--rw-r--r--   0        0        0     8824 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/authcaptureproxy/examples/modifiers.py
--rw-r--r--   0        0        0     1406 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/authcaptureproxy/examples/testers.py
--rw-r--r--   0        0        0     8468 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/authcaptureproxy/helper.py
--rw-r--r--   0        0        0     1662 2023-05-08 03:06:58.935522 authcaptureproxy-1.1.6/authcaptureproxy/stackoverflow.py
--rw-r--r--   0        0        0    15394 2023-05-08 03:06:59.803533 authcaptureproxy-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 authcaptureproxy-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     9012 2023-05-08 03:27:30.469634 authcaptureproxy-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10889 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2512 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/README.md
+-rw-r--r--   0        0        0     1885 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/authcaptureproxy/__init__.py
+-rw-r--r--   0        0        0    28304 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/authcaptureproxy/auth_capture_proxy.py
+-rw-r--r--   0        0        0     5979 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/authcaptureproxy/cli.py
+-rw-r--r--   0        0        0      139 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/authcaptureproxy/const.py
+-rw-r--r--   0        0        0       78 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/authcaptureproxy/examples/__init__.py
+-rw-r--r--   0        0        0     8824 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/authcaptureproxy/examples/modifiers.py
+-rw-r--r--   0        0        0     1406 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/authcaptureproxy/examples/testers.py
+-rw-r--r--   0        0        0     8468 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/authcaptureproxy/helper.py
+-rw-r--r--   0        0        0     1662 2023-05-08 03:27:29.605630 authcaptureproxy-1.2.0/authcaptureproxy/stackoverflow.py
+-rw-r--r--   0        0        0    15395 2023-05-08 03:27:30.477634 authcaptureproxy-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4208 1970-01-01 00:00:00.000000 authcaptureproxy-1.2.0/PKG-INFO
```

### Comparing `authcaptureproxy-1.1.6/CHANGELOG.md` & `authcaptureproxy-1.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog for auth_capture_proxy
 
 <!--next-version-placeholder-->
 
+## v1.2.0 (2023-05-08)
+### Feature
+* Require python 3.10 ([`9ede8e1`](https://github.com/alandtse/auth_capture_proxy/commit/9ede8e1961d9cd3ee188bd8145810c1003a004a3))
+
 ## v1.1.6 (2023-05-08)
 ### Fix
 * Require python 3.9 or greater ([`5ba1afd`](https://github.com/alandtse/auth_capture_proxy/commit/5ba1afdaf2cbdf16a82c7f40d2d56d145b8b369f))
 
 ## v1.1.5 (2023-05-07)
 ### Fix
 * **access_url:** Do not add port if 0 ([`ba9acb4`](https://github.com/alandtse/auth_capture_proxy/commit/ba9acb49f106a76c32f95ef3ef871444309597e0))
```

### Comparing `authcaptureproxy-1.1.6/LICENSE.txt` & `authcaptureproxy-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.6/README.md` & `authcaptureproxy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.6/authcaptureproxy/__init__.py` & `authcaptureproxy-1.2.0/authcaptureproxy/__init__.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.6/authcaptureproxy/auth_capture_proxy.py` & `authcaptureproxy-1.2.0/authcaptureproxy/auth_capture_proxy.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.6/authcaptureproxy/cli.py` & `authcaptureproxy-1.2.0/authcaptureproxy/cli.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.6/authcaptureproxy/examples/modifiers.py` & `authcaptureproxy-1.2.0/authcaptureproxy/examples/modifiers.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.6/authcaptureproxy/examples/testers.py` & `authcaptureproxy-1.2.0/authcaptureproxy/examples/testers.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.6/authcaptureproxy/helper.py` & `authcaptureproxy-1.2.0/authcaptureproxy/helper.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.6/authcaptureproxy/stackoverflow.py` & `authcaptureproxy-1.2.0/authcaptureproxy/stackoverflow.py`

 * *Files identical despite different names*

### Comparing `authcaptureproxy-1.1.6/pyproject.toml` & `authcaptureproxy-1.2.0/pyproject.toml`

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
-version = "1.1.6"
+version = "1.2.0"
 
 description = "A Python project to create a proxy to capture authentication information from a webpage. This is useful to capture oauth login details without access to a third-party oauth."
 keywords = [""]
 authors = ["Alan D. Tse"]
 maintainers = ["Alan D. Tse"]
 license = "Apache-2.0"
 readme = "README.md"
@@ -82,15 +82,15 @@
 # TODO Is your code a script?
 # Set the name of the Python module followed by a colon, followed by the name of the function
 auth_capture_proxy = "authcaptureproxy.cli:cli"
 
 [tool.poetry.dependencies]
 # TODO Add and remove dependencies here
 # These are dependencies that are included in the main package
-python                   = "^3.9"
+python                   = "^3.10"
 typer                    = ">=0.3, <1.0"
 aiohttp = "^3"
 multidict = "^6"
 yarl = "^1"
 importlib-metadata = ">=3.4.0"
 beautifulsoup4 = "^4"
 httpx = "*"
```

### Comparing `authcaptureproxy-1.1.6/PKG-INFO` & `authcaptureproxy-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: authcaptureproxy
-Version: 1.1.6
+Version: 1.2.0
 Summary: A Python project to create a proxy to capture authentication information from a webpage. This is useful to capture oauth login details without access to a third-party oauth.
 Home-page: https://github.com/alandtse/auth_capture_proxy
 License: Apache-2.0
 Author: Alan D. Tse
 Maintainer: Alan D. Tse
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
```

