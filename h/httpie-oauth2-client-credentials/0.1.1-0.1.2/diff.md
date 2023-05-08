# Comparing `tmp/httpie-oauth2-client-credentials-0.1.1.tar.gz` & `tmp/httpie-oauth2-client-credentials-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpie-oauth2-client-credentials-0.1.1.tar", last modified: Thu Oct  7 04:21:59 2021, max compression
+gzip compressed data, was "httpie-oauth2-client-credentials-0.1.2.tar", last modified: Mon May  8 16:10:48 2023, max compression
```

## Comparing `httpie-oauth2-client-credentials-0.1.1.tar` & `httpie-oauth2-client-credentials-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 04:21:59.583502 httpie-oauth2-client-credentials-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-10-07 04:21:45.000000 httpie-oauth2-client-credentials-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2021-10-07 04:21:59.583502 httpie-oauth2-client-credentials-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2021-10-07 04:21:45.000000 httpie-oauth2-client-credentials-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 04:21:59.583502 httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2021-10-07 04:21:59.000000 httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-10-07 04:21:59.000000 httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-07 04:21:59.000000 httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-10-07 04:21:59.000000 httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-07 04:21:59.000000 httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-07 04:21:59.000000 httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4778 2021-10-07 04:21:45.000000 httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-07 04:21:59.583502 httpie-oauth2-client-credentials-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2021-10-07 04:21:45.000000 httpie-oauth2-client-credentials-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:10:48.127634 httpie-oauth2-client-credentials-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 16:10:37.000000 httpie-oauth2-client-credentials-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-08 16:10:48.127634 httpie-oauth2-client-credentials-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-08 16:10:37.000000 httpie-oauth2-client-credentials-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:10:48.127634 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-08 16:10:37.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:10:48.127634 httpie-oauth2-client-credentials-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-08 16:10:37.000000 httpie-oauth2-client-credentials-0.1.2/setup.py
```

### Comparing `httpie-oauth2-client-credentials-0.1.1/LICENSE` & `httpie-oauth2-client-credentials-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `httpie-oauth2-client-credentials-0.1.1/PKG-INFO` & `httpie-oauth2-client-credentials-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: httpie-oauth2-client-credentials
-Version: 0.1.1
+Version: 0.1.2
 Summary: httpie auth plugin for OAuth2.0 client credentials flow.
 Home-page: https://github.com/satodoc/httpie-oauth2-client-credentials
+Download-URL: https://github.com/satodoc/httpie-oauth2-client-credentials
 Author: satdoc
 Author-email: satodoc-develop-public@outlook.com
 License: MIT
-Download-URL: https://github.com/satodoc/httpie-oauth2-client-credentials
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hca-httpie-auth
 
-As an auth plugin for httpie, it obtains a token with the OAuth2.0 client_credentials flow before executing http, and adds the `Authorzaion: Bearer ${token}` header to the executed request.  
+As an auth plugin for httpie, it obtains a token with the OAuth2.0 client_credentials flow before executing http, and adds the `Authorization: Bearer ${token}` header to the executed request.  
 
 ## Token request patterns
 
 Token request patterns are supported for the following:
 
 ## Installation
 
@@ -144,9 +143,7 @@
     "expires_in": 3599
 }
 ```
 
 ### Caution
 
 This plugin does not have a function to cache the token until "expires_in", so it will send a token request every time you execute the http command.
-
-
```

### Comparing `httpie-oauth2-client-credentials-0.1.1/README.md` & `httpie-oauth2-client-credentials-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # hca-httpie-auth
 
-As an auth plugin for httpie, it obtains a token with the OAuth2.0 client_credentials flow before executing http, and adds the `Authorzaion: Bearer ${token}` header to the executed request.  
+As an auth plugin for httpie, it obtains a token with the OAuth2.0 client_credentials flow before executing http, and adds the `Authorization: Bearer ${token}` header to the executed request.  
 
 ## Token request patterns
 
 Token request patterns are supported for the following:
 
 ## Installation
```

### Comparing `httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.egg-info/PKG-INFO` & `httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: httpie-oauth2-client-credentials
-Version: 0.1.1
+Version: 0.1.2
 Summary: httpie auth plugin for OAuth2.0 client credentials flow.
 Home-page: https://github.com/satodoc/httpie-oauth2-client-credentials
+Download-URL: https://github.com/satodoc/httpie-oauth2-client-credentials
 Author: satdoc
 Author-email: satodoc-develop-public@outlook.com
 License: MIT
-Download-URL: https://github.com/satodoc/httpie-oauth2-client-credentials
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hca-httpie-auth
 
-As an auth plugin for httpie, it obtains a token with the OAuth2.0 client_credentials flow before executing http, and adds the `Authorzaion: Bearer ${token}` header to the executed request.  
+As an auth plugin for httpie, it obtains a token with the OAuth2.0 client_credentials flow before executing http, and adds the `Authorization: Bearer ${token}` header to the executed request.  
 
 ## Token request patterns
 
 Token request patterns are supported for the following:
 
 ## Installation
 
@@ -144,9 +143,7 @@
     "expires_in": 3599
 }
 ```
 
 ### Caution
 
 This plugin does not have a function to cache the token until "expires_in", so it will send a token request every time you execute the http command.
-
-
```

### Comparing `httpie-oauth2-client-credentials-0.1.1/httpie_oauth2_client_credentials.py` & `httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         if self.scope:
             post_params['scope'] = self.scope
         
         post_data = None
         if self.token_request_type == 'basic':
             credentials = u'%s:%s' % (self.client_id, self.client_secret)
             token = b64encode(credentials.encode('utf8')).strip().decode('latin1')
-            req_headers['Authorzaion'] = 'Basic %s' % token
+            req_headers['Authorization'] = 'Basic %s' % token
             post_data = urlencode(post_params).encode()
 
         else:
             post_params['client_id'] = self.client_id
             post_params['client_secret'] = self.client_secret
             if self.token_request_type == 'form':
                 post_data = urlencode(post_params).encode()
```

### Comparing `httpie-oauth2-client-credentials-0.1.1/setup.py` & `httpie-oauth2-client-credentials-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 setup(
     name="httpie-oauth2-client-credentials",
     description="httpie auth plugin for OAuth2.0 client credentials flow.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
-    version="0.1.1",
+    version="0.1.2",
     author='satdoc',
     author_email='satodoc-develop-public@outlook.com',
     license='MIT',
     url='https://github.com/satodoc/httpie-oauth2-client-credentials',
     download_url='https://github.com/satodoc/httpie-oauth2-client-credentials',
     py_modules=['httpie_oauth2_client_credentials'],
     install_requires=['httpie>=2.0.0'],
```

