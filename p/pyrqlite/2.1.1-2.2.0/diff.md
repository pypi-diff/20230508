# Comparing `tmp/pyrqlite-2.1.1.tar.gz` & `tmp/pyrqlite-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrqlite-2.1.1.tar", last modified: Fri Dec 24 01:10:31 2021, max compression
+gzip compressed data, was "pyrqlite-2.2.0.tar", last modified: Mon May  8 13:26:15 2023, max compression
```

## Comparing `pyrqlite-2.1.1.tar` & `pyrqlite-2.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2021-12-24 01:10:31.159164 pyrqlite-2.1.1/
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1077 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/LICENSE
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      999 2021-12-24 01:10:31.159164 pyrqlite-2.1.1/PKG-INFO
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     2653 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/README.rst
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)       95 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/pyproject.toml
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)       38 2021-12-24 01:10:31.159164 pyrqlite-2.1.1/setup.cfg
--rwxr-xr-x   0 zmedico   (1000) zmedico   (1000)     3261 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/setup.py
-drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2021-12-24 01:10:31.156164 pyrqlite-2.1.1/src/
-drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2021-12-24 01:10:31.158164 pyrqlite-2.1.1/src/pyrqlite/
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)        0 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/src/pyrqlite/__init__.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     3284 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/src/pyrqlite/_ephemeral.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     5478 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/src/pyrqlite/connections.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      295 2021-12-24 01:09:59.000000 pyrqlite-2.1.1/src/pyrqlite/constants.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)    10885 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/src/pyrqlite/cursors.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1124 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/src/pyrqlite/dbapi2.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      207 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/src/pyrqlite/exceptions.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     7551 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/src/pyrqlite/extensions.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1080 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/src/pyrqlite/row.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      346 2021-12-24 01:09:23.000000 pyrqlite-2.1.1/src/pyrqlite/types.py
-drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2021-12-24 01:10:31.159164 pyrqlite-2.1.1/src/pyrqlite.egg-info/
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      999 2021-12-24 01:10:31.000000 pyrqlite-2.1.1/src/pyrqlite.egg-info/PKG-INFO
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      435 2021-12-24 01:10:31.000000 pyrqlite-2.1.1/src/pyrqlite.egg-info/SOURCES.txt
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)        1 2021-12-24 01:10:31.000000 pyrqlite-2.1.1/src/pyrqlite.egg-info/dependency_links.txt
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)        9 2021-12-24 01:10:31.000000 pyrqlite-2.1.1/src/pyrqlite.egg-info/top_level.txt
+drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-05-08 13:26:15.892583 pyrqlite-2.2.0/
+-rw-rw-r--   0 philip    (1000) philip    (1000)     1077 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/LICENSE
+-rw-rw-r--   0 philip    (1000) philip    (1000)      675 2023-05-08 13:26:15.892583 pyrqlite-2.2.0/PKG-INFO
+-rw-rw-r--   0 philip    (1000) philip    (1000)     2621 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/README.rst
+-rw-rw-r--   0 philip    (1000) philip    (1000)      624 2023-05-08 13:24:46.000000 pyrqlite-2.2.0/pyproject.toml
+-rw-rw-r--   0 philip    (1000) philip    (1000)       38 2023-05-08 13:26:15.892583 pyrqlite-2.2.0/setup.cfg
+-rwxrwxr-x   0 philip    (1000) philip    (1000)     3219 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/setup.py
+drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-05-08 13:26:15.888584 pyrqlite-2.2.0/src/
+drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-05-08 13:26:15.892583 pyrqlite-2.2.0/src/pyrqlite/
+-rw-rw-r--   0 philip    (1000) philip    (1000)        0 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/__init__.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)     3284 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/_ephemeral.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)     5963 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/connections.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)      273 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/constants.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)    11314 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/cursors.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)     1124 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/dbapi2.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)      207 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/exceptions.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)     7551 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/extensions.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)     1080 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/row.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)      346 2023-05-08 13:19:03.000000 pyrqlite-2.2.0/src/pyrqlite/types.py
+drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-05-08 13:26:15.892583 pyrqlite-2.2.0/src/pyrqlite.egg-info/
+-rw-rw-r--   0 philip    (1000) philip    (1000)      675 2023-05-08 13:26:15.000000 pyrqlite-2.2.0/src/pyrqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 philip    (1000) philip    (1000)      435 2023-05-08 13:26:15.000000 pyrqlite-2.2.0/src/pyrqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 philip    (1000) philip    (1000)        1 2023-05-08 13:26:15.000000 pyrqlite-2.2.0/src/pyrqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 philip    (1000) philip    (1000)        9 2023-05-08 13:26:15.000000 pyrqlite-2.2.0/src/pyrqlite.egg-info/top_level.txt
```

### Comparing `pyrqlite-2.1.1/LICENSE` & `pyrqlite-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.1.1/README.rst` & `pyrqlite-2.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 
 
 Installation
 ------------
 
 The last stable release is available on github and can be installed with ``pip``::
 
-    $ cd
-    $ git clone https://github.com/rqlite/pyrqlite.git
-    $ pip install ./pyrqlite
+    $ pip install git+https://github.com/rqlite/pyrqlite.git
 
 Alternatively (e.g. if ``pip`` is not available), a tarball can be downloaded
 from GitHub and installed with Setuptools::
 
     $ # X.X is the desired pyrqlite version (e.g. 0.5 or 0.6).
     $ curl -L https://github.com/rqlite/tarball/pyrqlite-X.X | tar xz
     $ cd pyrqlite*
```

### Comparing `pyrqlite-2.1.1/setup.py` & `pyrqlite-2.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 )
 
 sys.path.insert(0, 'src')
 from pyrqlite.constants import (
     __author__,
     __email__,
     __license__,
-    __version__,
 )
 
 class PyTest(Command):
     user_options = [('match=', 'k', 'Run only tests that match the provided expressions')]
 
     def initialize_options(self):
         self.match = None
@@ -68,15 +67,14 @@
             "--msg-template='{C}:{msg_id}:{path}:{line:3d},{column}: {obj}: {msg} ({symbol})'"] +
             find_packages('src', exclude=['test']), cwd='./src')
         raise SystemExit(errno)
 
 
 setup(
     name="pyrqlite",
-    version=__version__,
     url='https://github.com/rqlite/pyrqlite/',
     author=__author__,
     author_email=__email__,
     maintainer=__author__,
     maintainer_email=__email__,
     description='python DB API 2.0 driver for rqlite',
     license=__license__,
```

### Comparing `pyrqlite-2.1.1/src/pyrqlite/_ephemeral.py` & `pyrqlite-2.2.0/src/pyrqlite/_ephemeral.py`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.1.1/src/pyrqlite/connections.py` & `pyrqlite-2.2.0/src/pyrqlite/connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,7 +150,23 @@
         if factory:
             return factory(self)
         else:
             return Cursor(self)
 
     def execute(self, *args, **kwargs):
         return self.cursor().execute(*args, **kwargs)
+
+    def ping(self, reconnect=True):
+        if self._connection.sock is None:
+            if reconnect:
+                self._connection = self._init_connection()
+            else:
+                raise self.Error("Already closed")
+        try: 
+            self.execute("SELECT 1")
+        except Exception:
+            if reconnect:
+                self._connection = self._init_connection()
+                self.ping(False)
+            else:
+                raise
+
```

### Comparing `pyrqlite-2.1.1/src/pyrqlite/cursors.py` & `pyrqlite-2.2.0/src/pyrqlite/cursors.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,14 +66,16 @@
             'request method: %s uri: %s headers: %s body: %s',
             method,
             uri,
             headers,
             body)
         response = self.connection._fetch_response(
             method, uri, body=body, headers=headers)
+        if response.code != 200:
+            raise Error("received unexpected http status: %d" % response.code)
         logger.debug(
             "status: %s reason: %s",
             response.status,
             response.reason)
         response_text = response.read().decode('utf-8')
         logger.debug("raw response: %s", response_text)
         response_json = json.loads(
@@ -99,23 +101,23 @@
 
         qmark_matches = qmark_re.findall(operation)
         named_matches = named_re.findall(operation)
         param_matches = len(qmark_matches) + len(named_matches)
 
         # Matches but no parameters
         if param_matches > 0 and parameters is None:
-            raise ProgrammingError('paramater required but not given: %s' %
+            raise ProgrammingError('parameter required but not given: %s' %
                                    operation)
 
         # No regex matches and no parameters.
         if parameters is None:
             return operation
 
         if len(qmark_matches) > 0 and len(named_matches) > 0:
-            raise ProgrammingError('different paramater types in operation not'
+            raise ProgrammingError('different parameter types in operation not'
                                    'permitted: %s %s' % 
                                    (operation, parameters))
 
         if isinstance(parameters, dict):
             # parameters is a dict or a dict subclass
             if len(qmark_matches) > 0:
                 raise ProgrammingError('Unamed binding used, but you supplied '
@@ -148,27 +150,32 @@
             operation = ''.join(subst)
 
         return operation
 
     def _get_sql_command(self, sql_str):
         return sql_str.split(None, 1)[0].upper()
 
-    def execute(self, operation, parameters=None):
+    def execute(self, operation, parameters=None, queue=False, wait=False):
         if not isinstance(operation, basestring):
             raise ValueError(
                              "argument must be a string, not '{}'".format(type(operation).__name__))
 
         operation = self._substitute_params(operation, parameters)
 
         command = self._get_sql_command(operation)
         if command in ('SELECT', 'PRAGMA'):
             payload = self._request("GET",
                                     "/db/query?" + _urlencode({'q': operation}))
         else:
-            payload = self._request("POST", "/db/execute?transaction",
+            path = "/db/execute?transaction"
+            if queue:
+                path = path + "&queue"
+            if wait:
+                path = path +"&wait"
+            payload = self._request("POST", path,
                                     headers={'Content-Type': 'application/json'}, body=json.dumps([operation]))
 
         last_insert_id = None
         rows_affected = -1
         payload_rows = {}
         try:
             results = payload["results"]
@@ -238,23 +245,29 @@
             # rowcount for each update, and _emit_delete_statements
             # warns unless rowcount matches
             self.rowcount = rows_affected
         else:
             self.rowcount = len(self._rows)
         return self
 
-    def executemany(self, operation, seq_of_parameters=None):
+    def executemany(self, operation, seq_of_parameters=None, queue=False, wait=False):
         if not isinstance(operation, basestring):
             raise ValueError(
                 "argument must be a string, not '{}'".format(type(operation).__name__))
 
         statements = []
         for parameters in seq_of_parameters:
             statements.append(self._substitute_params(operation, parameters))
-        payload = self._request("POST", "/db/execute?transaction",
+
+        path = "/db/execute?transaction"
+        if queue:
+            path = path + "&queue"
+        if wait:
+            path = path +"&wait"
+        payload = self._request("POST", path,
                                 headers={'Content-Type': 'application/json'},
                                 body=json.dumps(statements))
         rows_affected = -1
         try:
             results = payload["results"]
         except KeyError:
             pass
```

### Comparing `pyrqlite-2.1.1/src/pyrqlite/dbapi2.py` & `pyrqlite-2.2.0/src/pyrqlite/dbapi2.py`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.1.1/src/pyrqlite/extensions.py` & `pyrqlite-2.2.0/src/pyrqlite/extensions.py`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.1.1/src/pyrqlite/row.py` & `pyrqlite-2.2.0/src/pyrqlite/row.py`

 * *Files identical despite different names*

