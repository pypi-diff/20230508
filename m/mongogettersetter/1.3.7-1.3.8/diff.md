# Comparing `tmp/mongogettersetter-1.3.7.tar.gz` & `tmp/mongogettersetter-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.3.7.tar", last modified: Sun May  7 23:57:54 2023, max compression
+gzip compressed data, was "mongogettersetter-1.3.8.tar", last modified: Mon May  8 00:06:50 2023, max compression
```

## Comparing `mongogettersetter-1.3.7.tar` & `mongogettersetter-1.3.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-07 23:57:54.235701 mongogettersetter-1.3.7/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-07 23:57:54.235701 mongogettersetter-1.3.7/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.7/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-07 23:57:54.235701 mongogettersetter-1.3.7/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    26674 2023-05-07 23:56:39.000000 mongogettersetter-1.3.7/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-07 23:57:54.235701 mongogettersetter-1.3.7/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-07 23:57:54.000000 mongogettersetter-1.3.7/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-07 23:57:54.000000 mongogettersetter-1.3.7/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-07 23:57:54.000000 mongogettersetter-1.3.7/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-07 23:57:54.000000 mongogettersetter-1.3.7/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-07 23:57:54.000000 mongogettersetter-1.3.7/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-07 23:57:54.235701 mongogettersetter-1.3.7/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-07 23:56:58.000000 mongogettersetter-1.3.7/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.8/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    26686 2023-05-08 00:03:05.000000 mongogettersetter-1.3.8/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-08 00:06:50.000000 mongogettersetter-1.3.8/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-08 00:06:50.062632 mongogettersetter-1.3.8/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-08 00:06:40.000000 mongogettersetter-1.3.8/setup.py
```

### Comparing `mongogettersetter-1.3.7/PKG-INFO` & `mongogettersetter-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.7
+Version: 1.3.8
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.7/README.md` & `mongogettersetter-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `mongogettersetter-1.3.7/mongogettersetter/__init__.py` & `mongogettersetter-1.3.8/mongogettersetter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,15 +593,15 @@
                 dictwrapper = MongoDictWrapper(nested_dict[_key])
                 dictwrapper.prepare(
                     original_dict, self._keys + [_key], self._collection, self._filter_query
                 )
                 return dictwrapper
             elif isinstance(nested_dict[_key], list):
                 datawrapper = MongoDataWrapper(
-                    original_dict + [_key], self._collection, self._filter_query
+                    original_dict, self._keys + [_key], self._collection, self._filter_query
                 )
                 return datawrapper
             else:
                 return nested_dict[_key]
 
     def __getitem__(self, _key):
         _key = str(_key)
```

### Comparing `mongogettersetter-1.3.7/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.3.8/mongogettersetter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.7
+Version: 1.3.8
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.7/setup.py` & `mongogettersetter-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.3.7',
+    version='1.3.8',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean realtime way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

