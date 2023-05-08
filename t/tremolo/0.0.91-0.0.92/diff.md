# Comparing `tmp/tremolo-0.0.91.tar.gz` & `tmp/tremolo-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.91.tar", last modified: Sun May  7 12:36:52 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.92.tar", last modified: Mon May  8 04:30:19 2023, max compression
```

## Comparing `tremolo-0.0.91.tar` & `tremolo-0.0.92.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-07 11:58:36.000000 tremolo-0.0.91/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-07 12:36:52.000000 tremolo-0.0.91/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     3143 2023-05-07 11:58:36.000000 tremolo-0.0.91/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-07 12:36:52.000000 tremolo-0.0.91/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-07 12:04:23.000000 tremolo-0.0.91/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     5356 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/contexts.py
--rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/__init__.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/tremolo/lib/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-07 11:24:03.000000 tremolo-0.0.91/tremolo/lib/h1parser/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-04-16 22:37:48.000000 tremolo-0.0.91/tremolo/lib/h1parser/parse_header.py
--rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-07 12:02:00.000000 tremolo-0.0.91/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     9307 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    10924 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/http_response.py
--rw-r--r--   0 tux       (1000) users      (100)      844 2023-05-07 11:23:12.000000 tremolo-0.0.91/tremolo/lib/object_pool.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-07 11:18:03.000000 tremolo-0.0.91/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-07 12:36:51.000000 tremolo-0.0.91/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-07 12:36:51.000000 tremolo-0.0.91/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-07 12:36:51.000000 tremolo-0.0.91/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-07 12:36:51.000000 tremolo-0.0.91/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 04:30:19.000000 tremolo-0.0.92/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.92/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-08 04:30:19.000000 tremolo-0.0.92/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     3143 2023-05-08 03:43:30.000000 tremolo-0.0.92/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 04:30:19.000000 tremolo-0.0.92/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-08 04:09:48.000000 tremolo-0.0.92/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 04:30:19.000000 tremolo-0.0.92/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     5391 2023-05-08 03:47:27.000000 tremolo-0.0.92/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/contexts.py
+-rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 04:30:19.000000 tremolo-0.0.92/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/__init__.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 04:30:19.000000 tremolo-0.0.92/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/h1parser/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     9307 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    10924 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)      844 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/object_pool.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-08 03:43:30.000000 tremolo-0.0.92/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 04:30:19.000000 tremolo-0.0.92/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-08 04:30:19.000000 tremolo-0.0.92/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-08 04:30:19.000000 tremolo-0.0.92/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-08 04:30:19.000000 tremolo-0.0.92/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-08 04:30:19.000000 tremolo-0.0.92/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.91/LICENSE.txt` & `tremolo-0.0.92/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/PKG-INFO` & `tremolo-0.0.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.91
+Version: 0.0.92
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.91/README.md` & `tremolo-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/setup.py` & `tremolo-0.0.92/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/h1parser/*']},
-    version='0.0.91',
+    version='0.0.92',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.91/tremolo/__main__.py` & `tremolo-0.0.92/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/asgi_lifespan.py` & `tremolo-0.0.92/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/asgi_server.py` & `tremolo-0.0.92/tremolo/asgi_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,23 +100,25 @@
                 self._response.set_status(data['status'], HTTPStatus(data['status']).phrase)
                 self._response.append_header(b'Date: %s\r\nServer: %s\r\n' % (
                                              datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
                                              self.options['server_name']))
 
                 if 'headers' in data:
                     for header in data['headers']:
-                        if header[0] == b'content-type':
+                        name = header[0].lower()
+
+                        if name == b'content-type':
                             self._response.set_content_type(header[1])
                             continue
 
-                        if header[0] in (b'connection', b'date', b'server', b'transfer-encoding'):
+                        if name in (b'connection', b'date', b'server', b'transfer-encoding'):
                             # disallow apps from changing them, as they are managed by Tremolo
                             continue
 
-                        if header[0] == b'content-length':
+                        if name == b'content-length':
                             # will disable http chunked in the self._response.write()
                             self._request.http_keepalive = False
 
                         self._response.append_header(b'%s: %s\r\n' % header)
             elif data['type'] == 'http.response.body':
                 if 'body' in data:
                     await self._response.write(data['body'])
```

### Comparing `tremolo-0.0.91/tremolo/contexts.py` & `tremolo-0.0.92/tremolo/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/exceptions.py` & `tremolo-0.0.92/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/http_server.py` & `tremolo-0.0.92/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/lib/h1parser/parse_header.py` & `tremolo-0.0.92/tremolo/lib/h1parser/parse_header.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/lib/http_exception.py` & `tremolo-0.0.92/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/lib/http_protocol.py` & `tremolo-0.0.92/tremolo/lib/http_protocol.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/lib/http_request.py` & `tremolo-0.0.92/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/lib/http_response.py` & `tremolo-0.0.92/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/lib/object_pool.py` & `tremolo-0.0.92/tremolo/lib/object_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/lib/request.py` & `tremolo-0.0.92/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/lib/response.py` & `tremolo-0.0.92/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo/tremolo.py` & `tremolo-0.0.92/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.91/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.92/tremolo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.91
+Version: 0.0.92
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.91/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.92/tremolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

