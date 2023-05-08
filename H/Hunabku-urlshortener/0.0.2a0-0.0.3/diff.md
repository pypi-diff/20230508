# Comparing `tmp/Hunabku_urlshortener-0.0.2a0.tar.gz` & `tmp/Hunabku_urlshortener-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_urlshortener-0.0.2a0.tar", last modified: Thu May  4 14:44:15 2023, max compression
+gzip compressed data, was "Hunabku_urlshortener-0.0.3.tar", last modified: Mon May  8 21:51:14 2023, max compression
```

## Comparing `Hunabku_urlshortener-0.0.2a0.tar` & `Hunabku_urlshortener-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:44:15.267946 Hunabku_urlshortener-0.0.2a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:44:15.267946 Hunabku_urlshortener-0.0.2a0/Hunabku_urlshortener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-04 14:44:15.000000 Hunabku_urlshortener-0.0.2a0/Hunabku_urlshortener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-04 14:44:15.000000 Hunabku_urlshortener-0.0.2a0/Hunabku_urlshortener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:44:15.000000 Hunabku_urlshortener-0.0.2a0/Hunabku_urlshortener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 14:44:15.000000 Hunabku_urlshortener-0.0.2a0/Hunabku_urlshortener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 14:44:15.000000 Hunabku_urlshortener-0.0.2a0/Hunabku_urlshortener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 14:43:55.000000 Hunabku_urlshortener-0.0.2a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-04 14:44:15.267946 Hunabku_urlshortener-0.0.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 14:43:55.000000 Hunabku_urlshortener-0.0.2a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:44:15.267946 Hunabku_urlshortener-0.0.2a0/hunabku_urlshortener/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:43:55.000000 Hunabku_urlshortener-0.0.2a0/hunabku_urlshortener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 14:43:55.000000 Hunabku_urlshortener-0.0.2a0/hunabku_urlshortener/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:44:15.267946 Hunabku_urlshortener-0.0.2a0/hunabku_urlshortener/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-04 14:43:55.000000 Hunabku_urlshortener-0.0.2a0/hunabku_urlshortener/endpoints/Shortener.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:44:15.267946 Hunabku_urlshortener-0.0.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-04 14:43:55.000000 Hunabku_urlshortener-0.0.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:51:14.500081 Hunabku_urlshortener-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:51:14.500081 Hunabku_urlshortener-0.0.3/Hunabku_urlshortener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-08 21:51:14.000000 Hunabku_urlshortener-0.0.3/Hunabku_urlshortener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-08 21:51:14.000000 Hunabku_urlshortener-0.0.3/Hunabku_urlshortener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:51:14.000000 Hunabku_urlshortener-0.0.3/Hunabku_urlshortener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 21:51:14.000000 Hunabku_urlshortener-0.0.3/Hunabku_urlshortener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 21:51:14.000000 Hunabku_urlshortener-0.0.3/Hunabku_urlshortener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 21:50:59.000000 Hunabku_urlshortener-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-08 21:51:14.500081 Hunabku_urlshortener-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-08 21:50:59.000000 Hunabku_urlshortener-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:51:14.500081 Hunabku_urlshortener-0.0.3/hunabku_urlshortener/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:50:59.000000 Hunabku_urlshortener-0.0.3/hunabku_urlshortener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 21:50:59.000000 Hunabku_urlshortener-0.0.3/hunabku_urlshortener/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:51:14.500081 Hunabku_urlshortener-0.0.3/hunabku_urlshortener/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-08 21:50:59.000000 Hunabku_urlshortener-0.0.3/hunabku_urlshortener/endpoints/Shortener.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:51:14.500081 Hunabku_urlshortener-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-08 21:50:59.000000 Hunabku_urlshortener-0.0.3/setup.py
```

### Comparing `Hunabku_urlshortener-0.0.2a0/Hunabku_urlshortener.egg-info/PKG-INFO` & `Hunabku_urlshortener-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Hunabku-urlshortener
-Version: 0.0.2a0
+Name: Hunabku_urlshortener
+Version: 0.0.3
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_urlshortener-0.0.2a0/PKG-INFO` & `Hunabku_urlshortener-0.0.3/Hunabku_urlshortener.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Hunabku_urlshortener
-Version: 0.0.2a0
+Name: Hunabku-urlshortener
+Version: 0.0.3
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_urlshortener-0.0.2a0/README.md` & `Hunabku_urlshortener-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Hunabku_urlshortener-0.0.2a0/hunabku_urlshortener/endpoints/Shortener.py` & `Hunabku_urlshortener-0.0.3/hunabku_urlshortener/endpoints/Shortener.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                     doc="MongoDB string connection")
 
     config += Param(db_name="urlshortener",
                     doc="Mongo DB name")
 
     config += Param(collection_name="records",
                     doc="Mongo DB collection name to save the records")
-    
+
     config += Param(maxtries=3,
                     doc="Number of times to try generating a new short code if the insertion fails")
 
     def __init__(self, hunabku):
         super().__init__(hunabku)
         self.dbclient = MongoClient(self.config.db_uri)
         self.db = self.dbclient[self.config.db_name]
@@ -34,86 +34,94 @@
     def validate_url(self, url):
         validation = validators.url(url)
         if validation:
             return True
         else:
             return False
 
-
     def generate_code(self):
         """
         Generate a short code for a URL based on the current timestamp.
 
         Returns:
             A string with the short code for the URL.
+            The timestamp at which the code was generated.
         """
 
         curr_secs = int(datetime.datetime.now().timestamp())
 
         self.counter += 1
 
         if curr_secs != self.last_sec:
             self.last_sec = curr_secs
             self.counter = 0
-            
-        #generate short code using base62 encoding
+
+        # generate short code using base62 encoding
         short_code = base62.encode(int(f"{curr_secs}{self.counter}"))
 
-        return short_code    
-    
-   
+        return short_code, curr_secs
+
     def insert_url(self, url):
         """
         Insert a URL and its corresponding short code in the MongoDB collection.
 
         Args:
             url: A string with the URL to be shortened.
         """
         tries = 0
-        
+
         while tries < self.config.maxtries:
-            short_code = self.generate_code()
+            short_code, curr_secs = self.generate_code()
             try:
-                self.collection.insert_one({'_id': short_code, 'url': url})
+                self.collection.insert_one({'_id': short_code,
+                                            'url': url,
+                                            'timestamp': curr_secs,
+                                            'calls': 0})
                 return short_code
-            
+
             except errors.DuplicateKeyError:
                 tries += 1
 
         response = self.app.response_class(
-            response = self.json.dumps(
+            response=self.json.dumps(
                 {"error": "Could not generate a unique short code"}),
             status=500,
             mimetype='application/json'
         )
         return response
 
-
     @endpoint('/<url_code>', methods=['GET', 'POST'])
     def url_id_end(self, url_code):
         """
         @api {get} /<url_code> URL code resolver
         @apiDescription Redirects to an URL given a shortened code
         @apiName resolver
         @apiGroup URLShortener
 
         @apiSuccess  redirect to the website 
         """
         x = self.collection.find_one({"_id": url_code})
         if x:
+            # add counter or number of calls in the redirect and save date of last call
+            now = int(datetime.datetime.now().timestamp())
+            self.collection.update_one(
+                {'_id': url_code},
+                {'$inc': {'calls': 1},
+                 '$set': {'last_call': now}}
+            )
+
             return redirect(x["url"])
         else:
             response = self.app.response_class(
                 response=self.json.dumps({"error": "url_code not found"}),
                 status=404,
                 mimetype='application/json'
             )
             return response
 
-
     @endpoint('/create', methods=['GET', 'POST'])
     def url_create_end(self):
         """
         @api {get} /create  Create a shortened URL
         @apiDescription Creates a unique shortened code
         @apiName create
         @apiGroup URLShortener
@@ -138,18 +146,17 @@
             response = self.app.response_class(
                 response=self.json.dumps(
                     {"error": "Bad request, invalid URL"}),
                 status=400,
                 mimetype='application/json'
             )
             return response
-    
 
         url = args["url"]
-        short_code = self.insert_url(url)        
+        short_code = self.insert_url(url)
         data = {"url_code": str(short_code)}
         response = self.app.response_class(
             response=self.json.dumps(data),
             status=200,
             mimetype='application/json'
         )
-        return response
+        return response
```

### Comparing `Hunabku_urlshortener-0.0.2a0/setup.py` & `Hunabku_urlshortener-0.0.3/setup.py`

 * *Files identical despite different names*

