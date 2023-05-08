# Comparing `tmp/pyCZDS-1.5.tar.gz` & `tmp/pyCZDS-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCZDS-1.5.tar", last modified: Sat Apr  1 20:13:01 2023, max compression
+gzip compressed data, was "pyCZDS-1.6.tar", last modified: Mon May  8 08:43:43 2023, max compression
```

## Comparing `pyCZDS-1.5.tar` & `pyCZDS-1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 20:13:01.150975 pyCZDS-1.5/
--rw-rw-rw-   0        0        0    35821 2022-12-16 18:23:26.000000 pyCZDS-1.5/LICENSE
--rw-rw-rw-   0        0        0     6344 2023-04-01 20:13:01.150975 pyCZDS-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5521 2023-04-01 20:11:25.000000 pyCZDS-1.5/README.md
--rw-rw-rw-   0        0        0      897 2023-04-01 20:12:28.000000 pyCZDS-1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-01 20:13:01.150975 pyCZDS-1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-01 20:13:01.117572 pyCZDS-1.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-01 20:13:01.142354 pyCZDS-1.5/src/pyCZDS.egg-info/
--rw-rw-rw-   0        0        0     6344 2023-04-01 20:13:01.000000 pyCZDS-1.5/src/pyCZDS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-04-01 20:13:01.000000 pyCZDS-1.5/src/pyCZDS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 20:13:01.000000 pyCZDS-1.5/src/pyCZDS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-01 20:13:01.000000 pyCZDS-1.5/src/pyCZDS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-01 20:13:01.146965 pyCZDS-1.5/src/pyczds/
--rw-rw-rw-   0        0        0        0 2022-12-16 18:10:39.000000 pyCZDS-1.5/src/pyczds/__init__.py
--rw-rw-rw-   0        0        0     2482 2022-12-16 19:05:34.000000 pyCZDS-1.5/src/pyczds/authentication.py
--rw-rw-rw-   0        0        0     4273 2023-04-01 20:10:43.000000 pyCZDS-1.5/src/pyczds/client.py
--rw-rw-rw-   0        0        0     2461 2022-12-26 15:53:53.000000 pyCZDS-1.5/src/pyczds/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-01 20:13:01.149972 pyCZDS-1.5/tests/
--rw-rw-rw-   0        0        0     3696 2022-12-16 22:05:49.000000 pyCZDS-1.5/tests/test_authentication.py
--rw-rw-rw-   0        0        0     3605 2022-12-17 09:18:40.000000 pyCZDS-1.5/tests/test_client.py
--rw-rw-rw-   0        0        0     2689 2022-12-26 18:04:19.000000 pyCZDS-1.5/tests/test_helpers.py
--rw-rw-rw-   0        0        0     1902 2022-12-26 18:04:45.000000 pyCZDS-1.5/tests/test_pyczds.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:43:43.848443 pyCZDS-1.6/
+-rw-rw-rw-   0        0        0    35821 2022-12-16 18:23:26.000000 pyCZDS-1.6/LICENSE
+-rw-rw-rw-   0        0        0     6519 2023-05-08 08:43:43.847038 pyCZDS-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5696 2023-05-08 08:41:44.000000 pyCZDS-1.6/README.md
+-rw-rw-rw-   0        0        0      897 2023-05-08 08:22:15.000000 pyCZDS-1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 08:43:43.848443 pyCZDS-1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 08:43:43.804876 pyCZDS-1.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 08:43:43.839017 pyCZDS-1.6/src/pyCZDS.egg-info/
+-rw-rw-rw-   0        0        0     6519 2023-05-08 08:43:43.000000 pyCZDS-1.6/src/pyCZDS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-05-08 08:43:43.000000 pyCZDS-1.6/src/pyCZDS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 08:43:43.000000 pyCZDS-1.6/src/pyCZDS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 08:43:43.000000 pyCZDS-1.6/src/pyCZDS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 08:43:43.843028 pyCZDS-1.6/src/pyczds/
+-rw-rw-rw-   0        0        0        0 2022-12-16 18:10:39.000000 pyCZDS-1.6/src/pyczds/__init__.py
+-rw-rw-rw-   0        0        0     2596 2023-05-08 08:22:46.000000 pyCZDS-1.6/src/pyczds/authentication.py
+-rw-rw-rw-   0        0        0     4357 2023-05-08 08:32:06.000000 pyCZDS-1.6/src/pyczds/client.py
+-rw-rw-rw-   0        0        0     2580 2023-05-08 08:24:16.000000 pyCZDS-1.6/src/pyczds/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:43:43.847038 pyCZDS-1.6/tests/
+-rw-rw-rw-   0        0        0     3696 2022-12-16 22:05:49.000000 pyCZDS-1.6/tests/test_authentication.py
+-rw-rw-rw-   0        0        0     3605 2022-12-17 09:18:40.000000 pyCZDS-1.6/tests/test_client.py
+-rw-rw-rw-   0        0        0     2689 2022-12-26 18:04:19.000000 pyCZDS-1.6/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     1902 2023-05-08 08:43:18.000000 pyCZDS-1.6/tests/test_pyczds.py
```

### Comparing `pyCZDS-1.5/LICENSE` & `pyCZDS-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCZDS-1.5/PKG-INFO` & `pyCZDS-1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCZDS
-Version: 1.5
+Version: 1.6
 Summary: An API client for ICANN's Centralized Zone Data Service (CZDS). Learn more under https://czds.icann.org/.
 Author-email: "Max M. Diez" <pyczds@xdiez.com>
 Project-URL: Homepage, https://github.com/mdiez/pyCZDS
 Project-URL: Bug Tracker, https://github.com/mdiez/pyCZDS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,17 @@
 *This package allows you to seamlessly interact with ICANN's CZDS and download zone files for participating Top-Level Domains.*
 
 > The Centralized Zone Data Service (CZDS) is an online portal where any interested party can request access to the Zone Files provided by participating generic Top-Level Domains (gTLDs).
 
 [Source](https://czds.icann.org/home)
 
 Relevant links:
+* [ICANN CZDS homepage](https://czds.icann.org/home)
 * pyCZDS on [PyPI](https://pypi.org/project/pyCZDS/)
-* pyCDZS repo on [GitHub](https://github.com/mdiez/pyCZDS)
+* pyCZDS repo on [GitHub](https://github.com/mdiez/pyCZDS)
 
 ## Installation
 
 This package requires Python 3 and has been tested with Python 3.10.8. It requires the `requests` package.
 The library implements a client against the official API documentation which can be found under this [link](https://github.com/icann/czds-api-client-java/blob/master/docs/ICANN_CZDS_api.pdf).
 
 Install pyCZDS with the command `pip install pyCZDS`.
@@ -62,29 +63,29 @@
     ...
     'https://czds-download-api.icann.org/czds/downloads/com.zone'
 ]
 ```
 Access to additional zone files can be requested online under this [link](https://czds.icann.org/zone-request/add).
 
 ### Requesting the headers for a zone file
-Using one of the links received via `get_zonefiles_list()`, the following command will retrieve the headers for a specified zonefile. It returns a `dict`:
+Using one of the links received via `get_zonefiles_list()`, the following command retrieves the headers for a specified zonefile. It returns a `dict` (more specifically, a `requests.models.CaseInsensitiveDict`):
 ```
 print(c.head_zonefile('https://czds-download-api.icann.org/czds/downloads/vision.zone'))
 # {
     'Date': 'Fri, 16 Dec 2022 19:42:58 GMT',
     ...
     'Last-Modified': 'Fri, 16 Dec 2022 01:29:08 GMT',
     ...
     'Content-Disposition': 'attachment;filename=vision.txt.gz',
     ...
     'Content-Length': '602034',
     ...
 }
 ```
-To facilitate further work with the metadata, the `dict` not only contains the raw HTTP headers, but also a subdict `parsed`, which contains a number of headers parsed in suitable data types:
+To facilitate further work with the metadata, the dictionary not only contains the raw HTTP headers, but also a subdict `parsed` (which is a `requests.models.CaseInsensitiveDict`, too), which contains a number of headers parsed in suitable data types:
 ```
 print(c.head_zonefile('https://czds-download-api.icann.org/czds/downloads/vision.zone'))
 # {
     'Last-Modified': 'Sat, 17 Dec 2022 00:17:25 GMT',
     'Content-Disposition': 'attachment;filename=net.txt.gz',
     'Content-Length': '481167941',
     ...
@@ -103,15 +104,15 @@
 ```
 Both parameters are optional.
 * `download_dir` sets the local directory where the file should be downloaded to. If it is not passed, the file will be downloaded to the working directory of your script.
 * `filename` sets the local filename of the downloaded file. If it is not passed, the filename will be set according to the value the API provides in the `Content-Disposition` header, e.g., `vision.tar.gz`.
 
 
 ## Troubleshooting
-Should you encounter errors, a good first step is to increase the logging level to `debug` and then analyze the output.
+Should you encounter any errors, a good first step is to increase the logging level to `debug` and then analyze the output.
 
 ```
 import logging
 
 from pyczds import client
 
 logger = logging.getLogger()
```

### Comparing `pyCZDS-1.5/README.md` & `pyCZDS-1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 *This package allows you to seamlessly interact with ICANN's CZDS and download zone files for participating Top-Level Domains.*
 
 > The Centralized Zone Data Service (CZDS) is an online portal where any interested party can request access to the Zone Files provided by participating generic Top-Level Domains (gTLDs).
 
 [Source](https://czds.icann.org/home)
 
 Relevant links:
+* [ICANN CZDS homepage](https://czds.icann.org/home)
 * pyCZDS on [PyPI](https://pypi.org/project/pyCZDS/)
-* pyCDZS repo on [GitHub](https://github.com/mdiez/pyCZDS)
+* pyCZDS repo on [GitHub](https://github.com/mdiez/pyCZDS)
 
 ## Installation
 
 This package requires Python 3 and has been tested with Python 3.10.8. It requires the `requests` package.
 The library implements a client against the official API documentation which can be found under this [link](https://github.com/icann/czds-api-client-java/blob/master/docs/ICANN_CZDS_api.pdf).
 
 Install pyCZDS with the command `pip install pyCZDS`.
@@ -44,29 +45,29 @@
     ...
     'https://czds-download-api.icann.org/czds/downloads/com.zone'
 ]
 ```
 Access to additional zone files can be requested online under this [link](https://czds.icann.org/zone-request/add).
 
 ### Requesting the headers for a zone file
-Using one of the links received via `get_zonefiles_list()`, the following command will retrieve the headers for a specified zonefile. It returns a `dict`:
+Using one of the links received via `get_zonefiles_list()`, the following command retrieves the headers for a specified zonefile. It returns a `dict` (more specifically, a `requests.models.CaseInsensitiveDict`):
 ```
 print(c.head_zonefile('https://czds-download-api.icann.org/czds/downloads/vision.zone'))
 # {
     'Date': 'Fri, 16 Dec 2022 19:42:58 GMT',
     ...
     'Last-Modified': 'Fri, 16 Dec 2022 01:29:08 GMT',
     ...
     'Content-Disposition': 'attachment;filename=vision.txt.gz',
     ...
     'Content-Length': '602034',
     ...
 }
 ```
-To facilitate further work with the metadata, the `dict` not only contains the raw HTTP headers, but also a subdict `parsed`, which contains a number of headers parsed in suitable data types:
+To facilitate further work with the metadata, the dictionary not only contains the raw HTTP headers, but also a subdict `parsed` (which is a `requests.models.CaseInsensitiveDict`, too), which contains a number of headers parsed in suitable data types:
 ```
 print(c.head_zonefile('https://czds-download-api.icann.org/czds/downloads/vision.zone'))
 # {
     'Last-Modified': 'Sat, 17 Dec 2022 00:17:25 GMT',
     'Content-Disposition': 'attachment;filename=net.txt.gz',
     'Content-Length': '481167941',
     ...
@@ -85,15 +86,15 @@
 ```
 Both parameters are optional.
 * `download_dir` sets the local directory where the file should be downloaded to. If it is not passed, the file will be downloaded to the working directory of your script.
 * `filename` sets the local filename of the downloaded file. If it is not passed, the filename will be set according to the value the API provides in the `Content-Disposition` header, e.g., `vision.tar.gz`.
 
 
 ## Troubleshooting
-Should you encounter errors, a good first step is to increase the logging level to `debug` and then analyze the output.
+Should you encounter any errors, a good first step is to increase the logging level to `debug` and then analyze the output.
 
 ```
 import logging
 
 from pyczds import client
 
 logger = logging.getLogger()
```

### Comparing `pyCZDS-1.5/pyproject.toml` & `pyCZDS-1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests", ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyCZDS"
-version = "1.5"
+version = "1.6"
 authors = [
   { name="Max M. Diez", email="pyczds@xdiez.com" },
 ]
 description = "An API client for ICANN's Centralized Zone Data Service (CZDS). Learn more under https://czds.icann.org/."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyCZDS-1.5/src/pyCZDS.egg-info/PKG-INFO` & `pyCZDS-1.6/src/pyCZDS.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCZDS
-Version: 1.5
+Version: 1.6
 Summary: An API client for ICANN's Centralized Zone Data Service (CZDS). Learn more under https://czds.icann.org/.
 Author-email: "Max M. Diez" <pyczds@xdiez.com>
 Project-URL: Homepage, https://github.com/mdiez/pyCZDS
 Project-URL: Bug Tracker, https://github.com/mdiez/pyCZDS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,17 @@
 *This package allows you to seamlessly interact with ICANN's CZDS and download zone files for participating Top-Level Domains.*
 
 > The Centralized Zone Data Service (CZDS) is an online portal where any interested party can request access to the Zone Files provided by participating generic Top-Level Domains (gTLDs).
 
 [Source](https://czds.icann.org/home)
 
 Relevant links:
+* [ICANN CZDS homepage](https://czds.icann.org/home)
 * pyCZDS on [PyPI](https://pypi.org/project/pyCZDS/)
-* pyCDZS repo on [GitHub](https://github.com/mdiez/pyCZDS)
+* pyCZDS repo on [GitHub](https://github.com/mdiez/pyCZDS)
 
 ## Installation
 
 This package requires Python 3 and has been tested with Python 3.10.8. It requires the `requests` package.
 The library implements a client against the official API documentation which can be found under this [link](https://github.com/icann/czds-api-client-java/blob/master/docs/ICANN_CZDS_api.pdf).
 
 Install pyCZDS with the command `pip install pyCZDS`.
@@ -62,29 +63,29 @@
     ...
     'https://czds-download-api.icann.org/czds/downloads/com.zone'
 ]
 ```
 Access to additional zone files can be requested online under this [link](https://czds.icann.org/zone-request/add).
 
 ### Requesting the headers for a zone file
-Using one of the links received via `get_zonefiles_list()`, the following command will retrieve the headers for a specified zonefile. It returns a `dict`:
+Using one of the links received via `get_zonefiles_list()`, the following command retrieves the headers for a specified zonefile. It returns a `dict` (more specifically, a `requests.models.CaseInsensitiveDict`):
 ```
 print(c.head_zonefile('https://czds-download-api.icann.org/czds/downloads/vision.zone'))
 # {
     'Date': 'Fri, 16 Dec 2022 19:42:58 GMT',
     ...
     'Last-Modified': 'Fri, 16 Dec 2022 01:29:08 GMT',
     ...
     'Content-Disposition': 'attachment;filename=vision.txt.gz',
     ...
     'Content-Length': '602034',
     ...
 }
 ```
-To facilitate further work with the metadata, the `dict` not only contains the raw HTTP headers, but also a subdict `parsed`, which contains a number of headers parsed in suitable data types:
+To facilitate further work with the metadata, the dictionary not only contains the raw HTTP headers, but also a subdict `parsed` (which is a `requests.models.CaseInsensitiveDict`, too), which contains a number of headers parsed in suitable data types:
 ```
 print(c.head_zonefile('https://czds-download-api.icann.org/czds/downloads/vision.zone'))
 # {
     'Last-Modified': 'Sat, 17 Dec 2022 00:17:25 GMT',
     'Content-Disposition': 'attachment;filename=net.txt.gz',
     'Content-Length': '481167941',
     ...
@@ -103,15 +104,15 @@
 ```
 Both parameters are optional.
 * `download_dir` sets the local directory where the file should be downloaded to. If it is not passed, the file will be downloaded to the working directory of your script.
 * `filename` sets the local filename of the downloaded file. If it is not passed, the filename will be set according to the value the API provides in the `Content-Disposition` header, e.g., `vision.tar.gz`.
 
 
 ## Troubleshooting
-Should you encounter errors, a good first step is to increase the logging level to `debug` and then analyze the output.
+Should you encounter any errors, a good first step is to increase the logging level to `debug` and then analyze the output.
 
 ```
 import logging
 
 from pyczds import client
 
 logger = logging.getLogger()
```

### Comparing `pyCZDS-1.5/src/pyczds/authentication.py` & `pyCZDS-1.6/src/pyczds/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 
 from .helpers import CZDSHelpers
 
 
 class CZDSAuthentication(CZDSHelpers):
     AUTH_URL = "https://account-api.icann.org/api/authenticate"
 
-    def __init__(self, username, password):
+    def __init__(self, username: str, password: str) -> None:
         if not isinstance(username, str) or len(username) == 0 or not self._is_email_address(username):
             raise ValueError('Username invalid.')
 
         if not isinstance(password, str) or len(password) == 0:
             raise ValueError('Password invalid.')
 
         self._username = username
         self._password = password
 
         self._token = str()
 
-    def _get_token_jwt_payload(self):
+    def _get_token_jwt_payload(self) -> json:
         logging.debug('Parsing JWT payload.')
 
         if len(self._token) == 0:
             raise ValueError('Authentication token is not set.')
 
         payload_b64 = self._token.split('.')[1]
         s = base64.b64decode(payload_b64)
         j = json.loads(s)
 
         logging.debug('JSON content of JWT payload: {}'.format(json.dumps(j)))
 
         return j
 
-    def _is_authenticated(self):
+    def _is_authenticated(self) -> bool:
         logging.debug('About to check if client is authenticated or not.')
 
         if len(self._token) > 0:
             j = self._get_token_jwt_payload()
 
             if j['exp'] > time.time():
                 logging.debug('Token is set and has not yet expired. Client is authenticated.')
@@ -50,15 +50,15 @@
             logging.debug('Not authenticated because token has expired.')
 
         else:
             logging.debug('Not authenticated because auth token is not set.')
 
         return False
 
-    def _authenticate(self):
+    def _authenticate(self) -> None:
         logging.debug('About to authenticate with username {}.'.format(self._username))
 
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
         }
 
@@ -74,8 +74,9 @@
         response = requests.Session().send(prepared_request)
         self._preprocess_response(response)
 
         token = response.json()['accessToken']
 
         logging.debug('Successfully authenticated. Received token {}.'.format(token))
 
-        self._token = token
+        token_padded = token + '=' * ((4 - len(token) % 4) % 4)
+        self._token = token_padded
```

### Comparing `pyCZDS-1.5/src/pyczds/client.py` & `pyCZDS-1.6/src/pyczds/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import sys
 import logging
 import os
 from urllib.parse import urljoin, urlparse, unquote
 from email.utils import parsedate_to_datetime
 from email.message import EmailMessage
-from importlib import metadata
 
 import requests
 
 from .authentication import CZDSAuthentication
 
 
 class CZDSClient(CZDSAuthentication):
     BASE_URL = 'https://czds-api.icann.org'
     ZONE_DOWNLOAD_LINKS_LIST_URL = urljoin(BASE_URL, '/czds/downloads/links')
 
-    def __init__(self, username, password):
+    def __init__(self, username: str, password: str) -> None:
         super().__init__(username=username, password=password)
 
-        if 'unittest' not in sys.modules.keys():
-            self._user_agent = '{} / {}'.format(
-                metadata.distribution('pyCZDS').name, metadata.distribution('pyCZDS').version
-            )
-        else:
-            self._user_agent = 'pyCZDS / test'
+        self._user_agent = '{} / {}'.format('pyCZDS', '1.6')
 
-    def _do_request(self, method, url, stream=False):
+        if 'unittest' in sys.modules.keys():
+            self._user_agent = '{} TEST'.format(self._user_agent)
+
+    def _do_request(self, method: str, url: str, stream: bool = False) -> requests.Response:
         if not self._is_authenticated():
             logging.debug('Not authenticated. Attempting authentication.')
             self._authenticate()
 
         headers = {
             'Authorization': 'Bearer {}'.format(self._token),
             'User-Agent': self._user_agent
@@ -40,48 +37,48 @@
         self._preprocess_request(prepared_request)
 
         response = requests.Session().send(prepared_request, stream=stream)
         self._preprocess_response(response, stream)
 
         return response
 
-    def _parse_headers(self, headers):
+    def _parse_headers(self, headers: requests.models.CaseInsensitiveDict) -> requests.models.CaseInsensitiveDict:
         parsed = requests.models.CaseInsensitiveDict()
 
         parsed['last-modified'] = parsedate_to_datetime(headers['last-modified'])
         parsed['content-length'] = int(headers['content-length'])
 
         msg = EmailMessage()
         msg['content-disposition'] = headers['content-disposition']
         filename = msg.get_filename()
         parsed['filename'] = filename
 
         headers['parsed'] = parsed
 
         return headers
 
-    def get_zonefiles_list(self):
+    def get_zonefiles_list(self) -> list:
         logging.debug('About to request zonefile URLs list.')
 
         url_list = self._do_request('get', self.ZONE_DOWNLOAD_LINKS_LIST_URL).json()
 
         if len(url_list) == 0:
             raise Exception('This account does not seem to have access to any zonefiles.')
 
         return url_list
 
-    def head_zonefile(self, zonefile_url):
+    def head_zonefile(self, zonefile_url: str) -> requests.models.CaseInsensitiveDict:
         logging.debug('About to request headers for zonefile {}.'.format(zonefile_url.split('/')[-1]))
 
         headers = self._do_request('head', zonefile_url).headers
         headers = self._parse_headers(headers)
 
         return headers
 
-    def get_zonefile(self, zonefile_url, download_dir='', filename=''):
+    def get_zonefile(self, zonefile_url: str, download_dir: str = '', filename: str = '') -> None:
         if not download_dir or (download_dir and len(str(download_dir)) == 0):
             download_dir = os.getcwd()
 
         url_parsed = urlparse(zonefile_url)
         remote_filename = unquote(os.path.basename(url_parsed.path))
 
         logging.debug('About to start download for zonefile {} to directory {}.'.format(
```

### Comparing `pyCZDS-1.5/src/pyczds/helpers.py` & `pyCZDS-1.6/src/pyczds/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import logging
 import re
 import os
+from typing import Match
 
 import requests
 
 
 class CZDSHelpers(object):
 
-    def _is_email_address(self, address_string):
+    def _is_email_address(self, address_string: str) -> Match:
         pat = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b'
         return re.match(pat, address_string)
 
-    def _preprocess_request(self, request):
+    def _preprocess_request(self, request: requests.Request) -> None:
         logging.debug(
             'About to send {} request to URL {} with headers {} and body {}.'.format(
                 request.method, request.url, request.headers, str(request.body)
             )
         )
 
-    def _preprocess_response(self, response, stream=False):
+    def _preprocess_response(self, response: requests.Response, stream: bool = False) -> None:
         logging.debug('Returned status code {}.'.format(response.status_code))
         logging.debug('Received headers {}.'.format(response.headers))
 
         if not stream:
             logging.debug('Received raw response {}.'.format(response.text))
 
         if response.status_code != 200:
@@ -42,15 +43,15 @@
             if response.status_code == 415:
                 raise requests.HTTPError('Unsupported content type header sent.')
             if response.status_code == 429:
                 raise requests.HTTPError('Too many authentication attempts from the same IP address.')
             if response.status_code == 500:
                 raise requests.HTTPError('Internal service error.')
 
-    def _check_file_size(self, file_path, size):
+    def _check_file_size(self, file_path: str, size: int) -> None:
         file_size = os.path.getsize(file_path)
 
         if file_size != size:
             raise Exception(
                 'The size of the file ({:,} bytes) differs from the size announced in the header ({:,} bytes).'.format(
                     file_size, size
                 )
```

### Comparing `pyCZDS-1.5/tests/test_authentication.py` & `pyCZDS-1.6/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `pyCZDS-1.5/tests/test_client.py` & `pyCZDS-1.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyCZDS-1.5/tests/test_helpers.py` & `pyCZDS-1.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyCZDS-1.5/tests/test_pyczds.py` & `pyCZDS-1.6/tests/test_pyczds.py`

 * *Files identical despite different names*

