# Comparing `tmp/pytest-httpbin-2.0.0rc1.tar.gz` & `tmp/pytest-httpbin-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-httpbin-2.0.0rc1.tar", last modified: Wed Mar 16 15:16:48 2022, max compression
+gzip compressed data, was "pytest-httpbin-2.0.0rc2.tar", last modified: Mon May  8 19:31:07 2023, max compression
```

## Comparing `pytest-httpbin-2.0.0rc1.tar` & `pytest-httpbin-2.0.0rc2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 graingert  (1000) graingert  (1000)        0 2022-03-16 15:16:48.386725 pytest-httpbin-2.0.0rc1/
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     1170 2022-02-24 17:51:40.000000 pytest-httpbin-2.0.0rc1/DESCRIPTION.rst
--rw-rw-r--   0 graingert  (1000) graingert  (1000)      198 2022-02-24 17:51:40.000000 pytest-httpbin-2.0.0rc1/MANIFEST.in
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     2142 2022-03-16 15:16:48.386725 pytest-httpbin-2.0.0rc1/PKG-INFO
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     9556 2022-03-16 15:14:43.000000 pytest-httpbin-2.0.0rc1/README.md
-drwxrwxr-x   0 graingert  (1000) graingert  (1000)        0 2022-03-16 15:16:48.382725 pytest-httpbin-2.0.0rc1/pytest_httpbin/
--rw-rw-r--   0 graingert  (1000) graingert  (1000)      365 2022-03-16 15:11:08.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin/__init__.py
-drwxrwxr-x   0 graingert  (1000) graingert  (1000)        0 2022-03-16 15:16:48.386725 pytest-httpbin-2.0.0rc1/pytest_httpbin/certs/
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     1866 2022-02-24 17:51:40.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin/certs/cacert.pem
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     1606 2022-02-24 17:51:40.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin/certs/cert.pem
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     1675 2022-02-24 17:51:40.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin/certs/key.pem
--rw-rw-r--   0 graingert  (1000) graingert  (1000)      513 2022-03-16 15:11:08.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin/certs.py
--rw-rw-r--   0 graingert  (1000) graingert  (1000)      979 2022-03-16 15:11:08.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin/plugin.py
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     4348 2022-03-16 15:11:08.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin/serve.py
--rw-rw-r--   0 graingert  (1000) graingert  (1000)       25 2022-03-16 15:15:39.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin/version.py
-drwxrwxr-x   0 graingert  (1000) graingert  (1000)        0 2022-03-16 15:16:48.386725 pytest-httpbin-2.0.0rc1/pytest_httpbin.egg-info/
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     2142 2022-03-16 15:16:48.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin.egg-info/PKG-INFO
--rw-rw-r--   0 graingert  (1000) graingert  (1000)      578 2022-03-16 15:16:48.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin.egg-info/SOURCES.txt
--rw-rw-r--   0 graingert  (1000) graingert  (1000)        1 2022-03-16 15:16:48.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin.egg-info/dependency_links.txt
--rw-rw-r--   0 graingert  (1000) graingert  (1000)       43 2022-03-16 15:16:48.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin.egg-info/entry_points.txt
--rw-rw-r--   0 graingert  (1000) graingert  (1000)       36 2022-03-16 15:16:48.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin.egg-info/requires.txt
--rw-rw-r--   0 graingert  (1000) graingert  (1000)       15 2022-03-16 15:16:48.000000 pytest-httpbin-2.0.0rc1/pytest_httpbin.egg-info/top_level.txt
--rw-rw-r--   0 graingert  (1000) graingert  (1000)      313 2022-03-16 15:16:48.386725 pytest-httpbin-2.0.0rc1/setup.cfg
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     2116 2022-03-16 15:11:08.000000 pytest-httpbin-2.0.0rc1/setup.py
-drwxrwxr-x   0 graingert  (1000) graingert  (1000)        0 2022-03-16 15:16:48.386725 pytest-httpbin-2.0.0rc1/tests/
--rw-rw-r--   0 graingert  (1000) graingert  (1000)      124 2022-03-16 15:11:08.000000 pytest-httpbin-2.0.0rc1/tests/conftest.py
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     1589 2022-03-16 15:11:08.000000 pytest-httpbin-2.0.0rc1/tests/test_httpbin.py
--rw-rw-r--   0 graingert  (1000) graingert  (1000)     3741 2022-03-16 15:11:08.000000 pytest-httpbin-2.0.0rc1/tests/test_server.py
--rw-rw-r--   0 graingert  (1000) graingert  (1000)      642 2022-03-16 15:11:08.000000 pytest-httpbin-2.0.0rc1/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:31:07.833964 pytest-httpbin-2.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-08 19:31:07.833964 pytest-httpbin-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:31:07.833964 pytest-httpbin-2.0.0rc2/pytest_httpbin/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:31:07.833964 pytest-httpbin-2.0.0rc2/pytest_httpbin/certs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin/certs/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:31:07.833964 pytest-httpbin-2.0.0rc2/pytest_httpbin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-08 19:31:07.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-08 19:31:07.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:31:07.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 19:31:07.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 19:31:07.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 19:31:07.000000 pytest-httpbin-2.0.0rc2/pytest_httpbin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-08 19:31:07.833964 pytest-httpbin-2.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:31:07.833964 pytest-httpbin-2.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/tests/test_httpbin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-08 19:30:23.000000 pytest-httpbin-2.0.0rc2/tests/util.py
```

### Comparing `pytest-httpbin-2.0.0rc1/DESCRIPTION.rst` & `pytest-httpbin-2.0.0rc2/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `pytest-httpbin-2.0.0rc1/PKG-INFO` & `pytest-httpbin-2.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pytest-httpbin
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Easily test your HTTP library against a local copy of httpbin
 Home-page: https://github.com/kevin1024/pytest-httpbin
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Keywords: pytest-httpbin testing pytest httpbin
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 pytest-httpbin
 ==============
 
@@ -49,9 +49,7 @@
     def test_that_my_library_works_kinda_ok():
         assert requests.get('http://httpbin.org/get').status_code == 200
 
 pytest-httpbin also supports https and includes its own CA cert you can use.
 Check out `the full documentation`_ on the github page.
 
 .. _the full documentation: https://github.com/kevin1024/pytest-httpbin
-
-
```

### Comparing `pytest-httpbin-2.0.0rc1/README.md` & `pytest-httpbin-2.0.0rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,16 @@
 
 ```bash
 pip install tox
 tox
 ```
 
 ## Changelog
-
+- 2.0.0rc2
+  - Add support for Python 3.11 and 3.12, drop dependency on six (#76)
 - 2.0.0rc1
   - Drop support for Python 2.6, 2.7, 3.4, 3.5 and 3.6 (#68)
   - Add support for Python 3.7, 3.8, 3.9 and 3.10 (#68)
   - Avoid deprecation warnings and resource warnings (#71)
 - 1.0.2
   - Switch from travis to github actions
   - This will be the last release to support Python 2.6, 2.7 or 3.6
```

### Comparing `pytest-httpbin-2.0.0rc1/pytest_httpbin/certs/cacert.pem` & `pytest-httpbin-2.0.0rc2/pytest_httpbin/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `pytest-httpbin-2.0.0rc1/pytest_httpbin/certs/cert.pem` & `pytest-httpbin-2.0.0rc2/pytest_httpbin/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytest-httpbin-2.0.0rc1/pytest_httpbin/certs/key.pem` & `pytest-httpbin-2.0.0rc2/pytest_httpbin/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytest-httpbin-2.0.0rc1/pytest_httpbin/certs.py` & `pytest-httpbin-2.0.0rc2/pytest_httpbin/certs.py`

 * *Files identical despite different names*

### Comparing `pytest-httpbin-2.0.0rc1/pytest_httpbin/plugin.py` & `pytest-httpbin-2.0.0rc2/pytest_httpbin/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-httpbin-2.0.0rc1/pytest_httpbin/serve.py` & `pytest-httpbin-2.0.0rc2/pytest_httpbin/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import os
 import ssl
 import threading
+from urllib.parse import urljoin
 from wsgiref.handlers import SimpleHandler
 from wsgiref.simple_server import WSGIRequestHandler, WSGIServer, make_server
 
-from six.moves.urllib.parse import urljoin
-
 CERT_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "certs")
 
 
 class ServerHandler(SimpleHandler):
-
     server_software = "Pytest-HTTPBIN/0.1.0"
     http_version = "1.1"
 
     def cleanup_headers(self):
         SimpleHandler.cleanup_headers(self)
         self.headers["Connection"] = "Close"
```

### Comparing `pytest-httpbin-2.0.0rc1/pytest_httpbin.egg-info/PKG-INFO` & `pytest-httpbin-2.0.0rc2/pytest_httpbin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pytest-httpbin
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Easily test your HTTP library against a local copy of httpbin
 Home-page: https://github.com/kevin1024/pytest-httpbin
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Keywords: pytest-httpbin testing pytest httpbin
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 pytest-httpbin
 ==============
 
@@ -49,9 +49,7 @@
     def test_that_my_library_works_kinda_ok():
         assert requests.get('http://httpbin.org/get').status_code == 200
 
 pytest-httpbin also supports https and includes its own CA cert you can use.
 Check out `the full documentation`_ on the github page.
 
 .. _the full documentation: https://github.com/kevin1024/pytest-httpbin
-
-
```

### Comparing `pytest-httpbin-2.0.0rc1/pytest_httpbin.egg-info/SOURCES.txt` & `pytest-httpbin-2.0.0rc2/pytest_httpbin.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 DESCRIPTION.rst
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 pytest_httpbin/__init__.py
 pytest_httpbin/certs.py
 pytest_httpbin/plugin.py
 pytest_httpbin/serve.py
 pytest_httpbin/version.py
```

### Comparing `pytest-httpbin-2.0.0rc1/setup.py` & `pytest-httpbin-2.0.0rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,22 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     # What does your project relate to?
     keywords="pytest-httpbin testing pytest httpbin",
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     include_package_data=True,  # include files listed in MANIFEST.in
-    install_requires=["httpbin", "six"],
-    extras_require={"test": ["requests", "pytest"]},
+    install_requires=["httpbin"],
+    extras_require={"test": ["requests", "pytest", "werkzeug<2.1.0"]},
     python_requires=">=3.7",
     # the following makes a plugin available to pytest
     entry_points={
         "pytest11": [
             "httpbin = pytest_httpbin.plugin",
         ]
     },
```

### Comparing `pytest-httpbin-2.0.0rc1/tests/test_httpbin.py` & `pytest-httpbin-2.0.0rc2/tests/test_httpbin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import ssl
+import sys
 import unittest
 
-import requests
+import pytest
+import requests.exceptions
 
 import pytest_httpbin
 
 
 def test_httpbin_gets_injected(httpbin):
     assert httpbin.url
 
@@ -39,16 +42,25 @@
     assert httpbin.join("foo") == httpbin.url + "/foo"
 
 
 def test_httpbin_str(httpbin):
     assert httpbin + "/foo" == httpbin.url + "/foo"
 
 
-def test_chunked_encoding(httpbin_both):
-    assert requests.get(httpbin_both.url + "/stream/20").status_code == 200
+def test_chunked_encoding(httpbin):
+    assert requests.get(httpbin.url + "/stream/20").status_code == 200
+
+
+@pytest.mark.xfail(
+    condition=sys.version_info < (3, 8) and ssl.OPENSSL_VERSION_INFO >= (3, 0, 0),
+    reason="fails on python3.7 openssl 3+",
+    raises=requests.exceptions.SSLError,
+)
+def test_chunked_encoding_secure(httpbin_secure):
+    assert requests.get(httpbin_secure.url + "/stream/20").status_code == 200
 
 
 @pytest_httpbin.use_class_based_httpbin
 @pytest_httpbin.use_class_based_httpbin_secure
 class TestClassBassedTests(unittest.TestCase):
     def test_http(self):
         assert requests.get(self.httpbin.url + "/get").status_code == 200
```

### Comparing `pytest-httpbin-2.0.0rc1/tests/test_server.py` & `pytest-httpbin-2.0.0rc2/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,8 +117,8 @@
 def test_redirect_location_is_https_for_secure_server(httpbin_secure):
     assert httpbin_secure.url.startswith("https://")
     response = requests.get(
         httpbin_secure + "/redirect-to?url=/html", allow_redirects=False
     )
     assert response.status_code == 302
     assert response.headers.get("Location")
-    assert response.headers["Location"].startswith("https://")
+    assert response.headers["Location"] == "/html"
```

### Comparing `pytest-httpbin-2.0.0rc1/tests/util.py` & `pytest-httpbin-2.0.0rc2/tests/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import socket
 
 
 def get_raw_http_response(host, port, path):
-
     CRLF = b"\r\n"
 
     request = [
         b"GET " + path.encode("ascii") + b" HTTP/1.1",
         b"Host: " + host.encode("ascii"),
         b"Connection: Close",
         b"",
```

