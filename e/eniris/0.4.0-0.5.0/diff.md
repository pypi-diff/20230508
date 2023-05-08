# Comparing `tmp/eniris-0.4.0.tar.gz` & `tmp/eniris-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eniris-0.4.0.tar", last modified: Wed May  3 12:16:05 2023, max compression
+gzip compressed data, was "eniris-0.5.0.tar", last modified: Mon May  8 08:36:20 2023, max compression
```

## Comparing `eniris-0.4.0.tar` & `eniris-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:16:05.508996 eniris-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-03 12:15:51.000000 eniris-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-03 12:16:05.508996 eniris-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-03 12:15:51.000000 eniris-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:16:05.508996 eniris-0.4.0/eniris/
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-03 12:15:51.000000 eniris-0.4.0/eniris/ApiDriver.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:15:51.000000 eniris-0.4.0/eniris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:16:05.508996 eniris-0.4.0/eniris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:16:05.508996 eniris-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-03 12:15:51.000000 eniris-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:36:20.823093 eniris-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 08:36:04.000000 eniris-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-08 08:36:20.823093 eniris-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-08 08:36:04.000000 eniris-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:36:20.823093 eniris-0.5.0/eniris/
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-05-08 08:36:04.000000 eniris-0.5.0/eniris/ApiDriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:36:04.000000 eniris-0.5.0/eniris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:36:20.823093 eniris-0.5.0/eniris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:36:20.823093 eniris-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 08:36:04.000000 eniris-0.5.0/setup.py
```

### Comparing `eniris-0.4.0/LICENSE` & `eniris-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eniris-0.4.0/PKG-INFO` & `eniris-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.4.0
+Version: 0.5.0
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.4.0.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.5.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -40,14 +40,15 @@
 - password (string, required)
 - authUrl (string, optional, default: 'https://authentication.eniris.be'): URL of authentication endpoint
 - apiUrl (string, optional, default: 'https://api.eniris.be'): URL of api endpoint
 - timeoutS (int, optional, default: 60): Request timeout in seconds
 - maximumRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
 - initialRetryDelayS (int, optional, default: 1): The initial delay between successive retries in seconds.
 - maximumRetryDelayS (int, optional, default: 60): The maximum delay between successive retries in seconds.
+- session (requests.Session, optional, default: requests.Session()): A session object to use for all API calls.
 
 Furthermore, the following methods are exposed:
 - get/delete: Send a HTTP GET/DELETE request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - params (dict, optional, default: None): URL query parameters
 - post/put: Send a HTTP POST or PUT request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
```

### Comparing `eniris-0.4.0/README.md` & `eniris-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 - password (string, required)
 - authUrl (string, optional, default: 'https://authentication.eniris.be'): URL of authentication endpoint
 - apiUrl (string, optional, default: 'https://api.eniris.be'): URL of api endpoint
 - timeoutS (int, optional, default: 60): Request timeout in seconds
 - maximumRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
 - initialRetryDelayS (int, optional, default: 1): The initial delay between successive retries in seconds.
 - maximumRetryDelayS (int, optional, default: 60): The maximum delay between successive retries in seconds.
+- session (requests.Session, optional, default: requests.Session()): A session object to use for all API calls.
 
 Furthermore, the following methods are exposed:
 - get/delete: Send a HTTP GET/DELETE request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - params (dict, optional, default: None): URL query parameters
 - post/put: Send a HTTP POST or PUT request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
```

### Comparing `eniris-0.4.0/eniris/ApiDriver.py` & `eniris-0.5.0/eniris/ApiDriver.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,82 +24,84 @@
     HTTPStatus.SERVICE_UNAVAILABLE
   }
   return response.status_code in RETRY_STATUS_CODES
 
 
 # Provide an easy interface to interact with the API, in the style of the requests library (https://docs.python-requests.org/en/master/)
 class ApiDriver:
-  def __init__(self, username:str, password:str, authUrl:str = 'https://authentication.eniris.be', apiUrl:str = 'https://api.eniris.be', timeoutS:int = 60, maximumRetries:int = 4, initialRetryDelayS:int=1, maximumRetryDelayS:int=60):
+  def __init__(self, username:str, password:str, authUrl:str = 'https://authentication.eniris.be', apiUrl:str = 'https://api.eniris.be', timeoutS:int = 60, maximumRetries:int = 4, initialRetryDelayS:int=1, maximumRetryDelayS:int=60, session: requests.Session=None):
     """Constructor. You must specify at least username and password or a credentialsPath where they are stored as a json of the form {'login': USERNAME, 'password': PASSWORD}
 
     Args:
         username (str, optional): Insights username
         password (str, optional): Insights password of the user
         authUrl (str, optional): Url of authentication endpoint. Defaults to https://authentication.eniris.be
         apiUrl (str, optional): Url of api endpoint. Defaults to https://api.eniris.be
-        timeoutS (int, optional): API timeout in seconds. Defaults to 60.
-        maximumRetries (int, optional): How many times to try again in case of a failure. Defaults to 4.
-        initialRetryDelayS (int, optional): The initial delay between successive retries in seconds. Defaults to 1.
-        maximumRetryDelayS (int, optional): The maximum delay between successive retries in seconds. Defaults to 60.
+        timeoutS (int, optional): API timeout in seconds. Defaults to 60
+        maximumRetries (int, optional): How many times to try again in case of a failure. Defaults to 4
+        initialRetryDelayS (int, optional): The initial delay between successive retries in seconds. Defaults to 1
+        maximumRetryDelayS (int, optional): The maximum delay between successive retries in seconds. Defaults to 60
+        session (requests.Session, optional): A session object to use for all API calls. If None, a requests.Session without extra options is created. Defaults to None
 
     Raises:
         Exception: _description_
     """
     self.username = username
     self.password = password
     self.authUrl = authUrl
     self.apiUrl = apiUrl
     self.timeoutS = timeoutS
     self.maximumRetries = maximumRetries
     self.initialRetryDelayS = initialRetryDelayS
     self.maximumRetryDelayS = maximumRetryDelayS
     self.refreshDtAndToken = None
     self.accessDtAndToken = None
+    self.session = requests.Session() if session is None else session
     
   def _authenticate(self):
     dt = datetime.datetime.now()
     if self.refreshDtAndToken is None or (dt - self.refreshDtAndToken[0]).total_seconds() > 13*24*60*60: # 13 days
       data = { "username": self.username, "password": self.password }
-      resp = requests.post(self.authUrl + '/auth/login', json = data, timeout=self.timeoutS)
+      resp = self.session.post(self.authUrl + '/auth/login', json = data, timeout=self.timeoutS)
       if resp.status_code != 200:
         raise AuthenticationFailure("login failed: " + resp.text)
       self.refreshDtAndToken = (dt, resp.text)
     elif (dt - self.refreshDtAndToken[0]).total_seconds() > 7*24*60*60: # 7 days
-      resp = requests.get(self.authUrl + '/auth/refreshtoken', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
+      resp = self.session.get(self.authUrl + '/auth/refreshtoken', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
       if resp.status_code == 200:
         self.refreshDtAndToken = (dt, resp.text)
       else:
         # Not the biggest problem, sice the refresh token will still be valid for a while, but we should log an exception
         logging.warning("Unable to renew the refresh token: " + resp.text)
     if self.accessDtAndToken is None or (dt - self.accessDtAndToken[0]).total_seconds() > 2*60: # 2 minutes
-      resp = requests.get(self.authUrl + '/auth/accesstoken', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
+      resp = self.session.get(self.authUrl + '/auth/accesstoken', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
       if resp.status_code != 200:
         raise AuthenticationFailure("accesstoken failed: " + resp.text)
       self.accessDtAndToken = (dt, resp.text)
       
   def close(self):
     """Log out from the API
     """
     dt = datetime.datetime.now()
     if self.refreshDtAndToken is None or (dt - self.refreshDtAndToken[0]).total_seconds() > 14*24*60*60: # 14 days
       # The refresh token did already expire, there is no reason to log out
       return
-    resp = requests.post(self.authUrl + '/auth/logout', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
+    resp = self.session.post(self.authUrl + '/auth/logout', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
     if resp.status_code == 204 or resp.status_code == 401:
       # The refresh token was either succesfully added to the deny list, or it was already invalid
       self.refreshDtAndToken = None
       self.accessDtAndToken = None 
     else:
       raise AuthenticationFailure("logout failed: " + resp.text)
   
   def __retry(self, requests_function:Callable, path:str, retryNr = 0, **req_function_kwargs) -> requests.Response:
     """Execute the given requests_function with the provided req_function_kwargs keyword arguments. If the function fails, it will try again until the amount of retries has exceeded.
 
     Args:
-        requests_function (Callable): Requests function to use. Can be requests.get, requests.post, requests.put or requests.delete
+        requests_function (Callable): Requests function to use. Can be self.session.get, self.session.post, self.session.put or self.session.delete
         path (str): Path relative to the apiUrl.
         retryNr (int, optional): How often the call has been tried already. Defaults to 0.
         req_function_kwargs (dict): Keyword arguments for the requests_function.
 
     Returns:
         requests.Response: HTTP response
     """
@@ -128,49 +130,49 @@
         path (str): Path relative to the apiUrl.
         params (dict, optional): URL parameters. Defaults to None.
 
     Returns:
         requests.Response: API call response
     """
     self._authenticate()
-    return self.__retry(requests.get, path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
+    return self.__retry(self.session.get, path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
 
   def post(self, path:str, json = None, params = None, data = None, **kwargs) -> requests.Response:
     """API POST call()
 
     Args:
         path (str): Path relative to the apiUrl.
         json (dict, optional): JSON body. Defaults to None.
         params (dict, optional): URL parameters. Defaults to None.
 
     Returns:
         requests.Response: API call response
     """
     self._authenticate()
-    return self.__retry(requests.post, path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
+    return self.__retry(self.session.post, path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
     
   def put(self, path:str, json = None, params = None, data = None, **kwargs) -> requests.Response:
     """API PUT call
 
     Args:
         path (str): Path relative to the apiUrl.
         json (dict, optional): JSON body. Defaults to None.
         params (dict, optional): URL parameters. Defaults to None.
 
     Returns:
         requests.Response: API call response
     """
     self._authenticate()
-    return self.__retry(requests.put, path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
+    return self.__retry(self.session.put, path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
   
   def delete(self, path:str, params = None, **kwargs) -> requests.Response:
     """API DELETE call
 
     Args:
         path (str): Path relative to the baseUrl.
         params (dict, optional): URL parameters. Defaults to None.
 
     Returns:
         requests.Response: API call response
     """
     self._authenticate()
-    return self.__retry(requests.delete, path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
+    return self.__retry(self.session.delete, path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
```

### Comparing `eniris-0.4.0/eniris.egg-info/PKG-INFO` & `eniris-0.5.0/eniris.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.4.0
+Version: 0.5.0
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.4.0.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.5.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -40,14 +40,15 @@
 - password (string, required)
 - authUrl (string, optional, default: 'https://authentication.eniris.be'): URL of authentication endpoint
 - apiUrl (string, optional, default: 'https://api.eniris.be'): URL of api endpoint
 - timeoutS (int, optional, default: 60): Request timeout in seconds
 - maximumRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
 - initialRetryDelayS (int, optional, default: 1): The initial delay between successive retries in seconds.
 - maximumRetryDelayS (int, optional, default: 60): The maximum delay between successive retries in seconds.
+- session (requests.Session, optional, default: requests.Session()): A session object to use for all API calls.
 
 Furthermore, the following methods are exposed:
 - get/delete: Send a HTTP GET/DELETE request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - params (dict, optional, default: None): URL query parameters
 - post/put: Send a HTTP POST or PUT request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
```

### Comparing `eniris-0.4.0/setup.py` & `eniris-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 with open("README.md", 'r') as f:
     long_description = f.read()
     
 setup(
   name = 'eniris',
   packages = ['eniris'],
-  version = '0.4.0',
+  version = '0.5.0',
   description = 'Eniris API driver for Python',
   license='MIT',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Enris BV',
   author_email = 'info@eniris.be',
   url = 'https://github.com/eniris-international/eniris-api-python-driver',
-  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.4.0.tar.gz',
+  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.5.0.tar.gz',
   keywords = ['eniris', 'api', 'rest'],   # Keywords that define your package best
   install_requires=[
     'requests',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
```

