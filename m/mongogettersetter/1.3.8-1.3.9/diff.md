# Comparing `tmp/mongogettersetter-1.3.8.tar.gz` & `tmp/mongogettersetter-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.3.8.tar", last modified: Mon May  8 00:06:50 2023, max compression
+gzip compressed data, was "mongogettersetter-1.3.9.tar", last modified: Mon May  8 01:48:59 2023, max compression
```

## Comparing `mongogettersetter-1.3.8.tar` & `mongogettersetter-1.3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.8/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    26686 2023-05-08 00:03:05.000000 mongogettersetter-1.3.8/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-08 00:06:40.000000 mongogettersetter-1.3.8/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 01:48:59.487131 mongogettersetter-1.3.9/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-08 01:48:59.483131 mongogettersetter-1.3.9/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.9/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 01:48:59.483131 mongogettersetter-1.3.9/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    26777 2023-05-08 01:38:06.000000 mongogettersetter-1.3.9/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 01:48:59.483131 mongogettersetter-1.3.9/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-08 01:48:59.000000 mongogettersetter-1.3.9/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-08 01:48:59.000000 mongogettersetter-1.3.9/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-08 01:48:59.000000 mongogettersetter-1.3.9/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-08 01:48:59.000000 mongogettersetter-1.3.9/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-08 01:48:59.000000 mongogettersetter-1.3.9/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-08 01:48:59.487131 mongogettersetter-1.3.9/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-08 00:40:47.000000 mongogettersetter-1.3.9/setup.py
```

### Comparing `mongogettersetter-1.3.8/PKG-INFO` & `mongogettersetter-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.8
+Version: 1.3.9
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.8/README.md` & `mongogettersetter-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mongogettersetter-1.3.8/mongogettersetter/__init__.py` & `mongogettersetter-1.3.9/mongogettersetter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,23 +501,26 @@
             self.pull(None)
         self._data = self._collection.find_one(self._filter_query)
 
     def __delattr__(self, _key):
         """
         Delete the key in the array/string/object using del keyword
         """
-        path = ".".join(str(v) for v in self._keys)
+        path = ".".join(str(v) for v in self._keys + [_key])
         data = self.get()
         _key = str(_key)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
         if isinstance(data, list):
             self.pull(None)
         self._data = self._collection.find_one(self._filter_query)
+    
+    def __contains__(self, _key):
+        return _key in self.get()
 
     def delete(self):
         """
         Delete the nested object from the MongoDB Document using $unset
         """
         
         path = ".".join(str(v) for v in self._keys)
@@ -573,14 +576,15 @@
             self._data = self._collection.find_one(self._filter_query)
         
 
     def __getattr__(self, _key):
         """
         Get the value of the key in the dictionary.
         """
+        
         _key = str(_key)
         if _key in self.__dict__:
             return self.__dict__[_key]
         else:
             path = ".".join(str(v) for v in self._keys)
             # print(f"__getitem__ you are at: {path}")
             original_dict = self._data
```

### Comparing `mongogettersetter-1.3.8/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.3.9/mongogettersetter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.8
+Version: 1.3.9
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.8/setup.py` & `mongogettersetter-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.3.8',
+    version='1.3.9',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean realtime way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

