# Comparing `tmp/pyelectroluxconnect-0.3.8.tar.gz` & `tmp/pyelectroluxconnect-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelectroluxconnect-0.3.8.tar", last modified: Wed Dec 28 20:12:19 2022, max compression
+gzip compressed data, was "pyelectroluxconnect-0.3.9.tar", last modified: Wed Dec 28 21:33:17 2022, max compression
```

## Comparing `pyelectroluxconnect-0.3.8.tar` & `pyelectroluxconnect-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-12-28 20:12:19.336132 pyelectroluxconnect-0.3.8/
--rw-rw-rw-   0        0        0    11524 2022-02-19 13:45:46.000000 pyelectroluxconnect-0.3.8/LICENSE
--rw-rw-rw-   0        0        0       30 2022-02-16 21:33:03.000000 pyelectroluxconnect-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6408 2022-12-28 20:12:19.628569 pyelectroluxconnect-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     5796 2022-05-14 20:02:30.000000 pyelectroluxconnect-0.3.8/README.md
--rw-rw-rw-   0        0        0      104 2021-11-24 22:35:42.000000 pyelectroluxconnect-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-28 20:12:19.635981 pyelectroluxconnect-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1045 2022-12-28 20:10:50.000000 pyelectroluxconnect-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-28 20:12:19.349132 pyelectroluxconnect-0.3.8/src/
-drwxrwxrwx   0        0        0        0 2022-12-28 20:12:19.349132 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect/
--rw-rw-rw-   0        0        0    46210 2022-12-28 20:04:56.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect/Session.py
--rw-rw-rw-   0        0        0      295 2022-06-14 10:30:57.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect/__init__.py
--rw-rw-rw-   0        0        0     4324 2021-11-24 22:21:14.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect/certificatechain.pem
--rw-rw-rw-   0        0        0     5613 2022-10-19 19:18:34.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect/urls.py
-drwxrwxrwx   0        0        0        0 2022-12-28 20:12:19.356132 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect.egg-info/
--rw-rw-rw-   0        0        0     6408 2022-12-28 20:12:19.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2022-12-28 20:12:19.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-28 20:12:19.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-02-19 15:17:45.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       38 2022-12-28 20:12:19.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-12-28 20:12:19.000000 pyelectroluxconnect-0.3.8/src/pyelectroluxconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-28 21:33:17.040427 pyelectroluxconnect-0.3.9/
+-rw-rw-rw-   0        0        0    11524 2022-02-19 13:45:46.000000 pyelectroluxconnect-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0       30 2022-02-16 21:33:03.000000 pyelectroluxconnect-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6408 2022-12-28 21:33:17.383962 pyelectroluxconnect-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5796 2022-05-14 20:02:30.000000 pyelectroluxconnect-0.3.9/README.md
+-rw-rw-rw-   0        0        0      104 2021-11-24 22:35:42.000000 pyelectroluxconnect-0.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-12-28 21:33:17.388252 pyelectroluxconnect-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2022-12-28 21:31:51.000000 pyelectroluxconnect-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-28 21:33:17.053427 pyelectroluxconnect-0.3.9/src/
+drwxrwxrwx   0        0        0        0 2022-12-28 21:33:17.053427 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect/
+-rw-rw-rw-   0        0        0    46163 2022-12-28 21:18:06.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect/Session.py
+-rw-rw-rw-   0        0        0      295 2022-06-14 10:30:57.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect/__init__.py
+-rw-rw-rw-   0        0        0     4324 2021-11-24 22:21:14.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect/certificatechain.pem
+-rw-rw-rw-   0        0        0     5613 2022-10-19 19:18:34.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect/urls.py
+drwxrwxrwx   0        0        0        0 2022-12-28 21:33:17.075427 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect.egg-info/
+-rw-rw-rw-   0        0        0     6408 2022-12-28 21:33:16.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2022-12-28 21:33:17.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-28 21:33:16.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-02-19 15:17:45.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       38 2022-12-28 21:33:16.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2022-12-28 21:33:16.000000 pyelectroluxconnect-0.3.9/src/pyelectroluxconnect.egg-info/top_level.txt
```

### Comparing `pyelectroluxconnect-0.3.8/LICENSE` & `pyelectroluxconnect-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyelectroluxconnect-0.3.8/PKG-INFO` & `pyelectroluxconnect-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyelectroluxconnect
-Version: 0.3.8
+Version: 0.3.9
 Summary: Interface for Electrolux Connectivity Platform API
 Home-page: https://github.com/tomeko12/pyelectroluxconnect
 Author: tomeko
 License: Apache Software License
 Keywords: home automation electrolux aeg frigidaire husqvarna
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyelectroluxconnect-0.3.8/README.md` & `pyelectroluxconnect-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyelectroluxconnect-0.3.8/setup.py` & `pyelectroluxconnect-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyelectroluxconnect',
-    version='0.3.8',
+    version='0.3.9',
     description='Interface for Electrolux Connectivity Platform API',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/tomeko12/pyelectroluxconnect',
     author='tomeko',
     license='Apache Software License',
     classifiers=[
```

### Comparing `pyelectroluxconnect-0.3.8/src/pyelectroluxconnect/Session.py` & `pyelectroluxconnect-0.3.9/src/pyelectroluxconnect/Session.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class Error(Exception):
     """ Session error """
     pass
 
 
-class HttpRequestError(Error):
+class RequestError(Error):
     """ Wrapped requests.exceptions.RequestException """
     pass
 
 class LoginError(Error):
     """ Login failed """
     pass
 
@@ -48,19 +48,19 @@
             "Invalid http response"
             ", status code: {0} - Data: {1}".format(
                 status_code,
                 text))
         self.status_code = status_code
         self.text = text
 
-class ApiResponseError(Error):
+class ResponseError(Error):
     """ Unexcpected response """
 
     def __init__(self, status_code, message):
-        super(ApiResponseError, self).__init__(
+        super(ResponseError, self).__init__(
             "Invalid API response: {1} ({0})".format(
                 status_code,
                 message))
         self.status_code = status_code
         self.message = message
 
 
@@ -165,19 +165,19 @@
             try:
                 if(not os.path.exists(os.path.expanduser("~/.pyelectroluxconnect/"))):
                     os.mkdir(os.path.expanduser("~/.pyelectroluxconnect/"))
                 with open(self._tokenFileName, "w") as tokenFile:
                     tokenFile.write(self._sessionToken)
             except OSError as err:
                 _LOGGER.error(f'Unable to write session token to file {self._tokenFileName}. {err.text}')
-        except ApiResponseError as err:
+        except ResponseError as err:
             if(err.status_code == 401 or err.status_code in ("AER0802", "ECP0108")): 
                 raise LoginError(f'{err.message} ({err.status_code})') from None
             else:
-                raise ApiResponseError(err.status_code, err.message) from None
+                raise ResponseError(err.status_code, err.message) from None
         except Exception as err:
             _LOGGER.error(err)
             raise
 
     def _getAppliancesList(self):
         """ 
         Get user registered appliances list
@@ -236,15 +236,15 @@
                         _json[0]["configuration_file"][applianceConfigFileName]["digest"])):
                     try:
                         _zipFile = self._requestHttp(
                             urls.getApplianceConfigurationFile(deviceConfigId))
                         open(applianceConfigFilePath, "wb").write(
                             _zipFile.content)
                     except requests.exceptions.RequestException as ex:
-                        raise HttpRequestError(ex)
+                        raise RequestError(ex)
 
                 if(os.path.exists(applianceConfigFilePath)
                    and f'md5-{hashlib.md5(open(applianceConfigFilePath,"rb").read()).hexdigest()}' ==
                         _json[0]["configuration_file"][applianceConfigFileName]["digest"]):
 
                     with zipfile.ZipFile(applianceConfigFilePath, "r") as archive:
                         result["Translations"] = {}
@@ -756,63 +756,63 @@
 
             _LOGGER.debug(f"HTTP Respose body: {response.text}")
 
             if 2 != response.status_code // 100:
                 raise HttpResponseError(response.status_code, response.text) from None
 
         except requests.exceptions.RequestException as ex:
-            raise HttpRequestError(ex) from None
+            raise RequestError(ex) from None
 
         return response
     
     
     def _requestApi(self, operation, payload=None):
         """
         Request to API
         returns JSON response
         """
         try:
             jsonresponse =  json.loads(self._requestHttp(
                         operation, payload).text)
             if(jsonresponse["status"] != "OK"):
-                raise ApiResponseError(jsonresponse["code"], jsonresponse["message"]) from None
+                raise ResponseError(jsonresponse["code"], jsonresponse["message"]) from None
             return jsonresponse["data"]
         
-        except HttpRequestError as err:
+        except RequestError as err:
             _LOGGER.error(f'API request error: {err}')
             raise Exception(err) from None
-        except ApiResponseError as err:
+        except ResponseError as err:
             if(err.status_code in ("ECP0105", "ECP2004")):
                 _LOGGER.warn(f'API token error {err.status_code}: {err.message}')
                 try:
                     self._createToken()
                     return json.loads(self._requestHttp(
                             operation, payload).text)["data"]
                 except LoginError as err:
                     raise LoginError(err) from None
                 except AuthError(err):
                     raise AuthError(err) from None
             else:
                 _LOGGER.error(f'API response error {err.status_code}: {err.message}')
-                raise ApiResponseError(err.status_code, err.message) from None
+                raise ResponseError(err.status_code, err.message) from None
         except HttpResponseError as err:
             message = err.text
             errcode = err.status_code
             
             try:
                 message = json.loads(err.text)
                 if("code" in message):
                     errcode = message["code"]
                 if("message" in message):
                     message = message["message"]
-                raise ApiResponseError(errcode, message) from None
+                raise ResponseError(errcode, message) from None
             except ValueError:
                 _LOGGER.error(f'HTTP response error {err.status_code}: {err.text}')
                 raise HttpResponseError(err.status_code, err.text) from None
-            raise HttpResponseError(err.status_code, err.text) from None
+            raise ResponseError(err.status_code, err.text) from None
         except Exception as err:
             _LOGGER.error(f'API request error: {err}')
             raise
         
             
         
 
@@ -1047,15 +1047,15 @@
         DeviceToken - Token required to authentication
                         for IBM broker, use 'use-token-auth' as username, 
                         DeviceToken as password
 
         """
         try:
             _json = self._requestApi(urls.registerMQTT(), None)
-        except ApiResponseError as err:
+        except ResponseError as err:
             if(err.status_code == "ECP0206"):
                 """ Device registered already, unregister first to get new token """
                 _LOGGER.warn(f"Device registered already in Electrolux MQTT broker, unregistering to get new token")
                 self.unregisterMQTT()
                 _json = self._requestApi(
                     urls.registerMQTT(), None)
             else:
```

### Comparing `pyelectroluxconnect-0.3.8/src/pyelectroluxconnect/certificatechain.pem` & `pyelectroluxconnect-0.3.9/src/pyelectroluxconnect/certificatechain.pem`

 * *Files identical despite different names*

### Comparing `pyelectroluxconnect-0.3.8/src/pyelectroluxconnect/urls.py` & `pyelectroluxconnect-0.3.9/src/pyelectroluxconnect/urls.py`

 * *Files identical despite different names*

### Comparing `pyelectroluxconnect-0.3.8/src/pyelectroluxconnect.egg-info/PKG-INFO` & `pyelectroluxconnect-0.3.9/src/pyelectroluxconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyelectroluxconnect
-Version: 0.3.8
+Version: 0.3.9
 Summary: Interface for Electrolux Connectivity Platform API
 Home-page: https://github.com/tomeko12/pyelectroluxconnect
 Author: tomeko
 License: Apache Software License
 Keywords: home automation electrolux aeg frigidaire husqvarna
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

