# Comparing `tmp/mongogettersetter-1.3.5.tar.gz` & `tmp/mongogettersetter-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.3.5.tar", last modified: Fri May  5 20:28:42 2023, max compression
+gzip compressed data, was "mongogettersetter-1.3.6.tar", last modified: Sun May  7 23:47:35 2023, max compression
```

## Comparing `mongogettersetter-1.3.5.tar` & `mongogettersetter-1.3.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.5/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24990 2023-05-05 20:23:21.000000 mongogettersetter-1.3.5/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-05 20:28:33.000000 mongogettersetter-1.3.5/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-07 23:47:35.857672 mongogettersetter-1.3.6/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-07 23:47:35.857672 mongogettersetter-1.3.6/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.6/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-07 23:47:35.857672 mongogettersetter-1.3.6/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    26326 2023-05-07 23:46:18.000000 mongogettersetter-1.3.6/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-07 23:47:35.857672 mongogettersetter-1.3.6/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-07 23:47:35.000000 mongogettersetter-1.3.6/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-07 23:47:35.000000 mongogettersetter-1.3.6/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-07 23:47:35.000000 mongogettersetter-1.3.6/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-07 23:47:35.000000 mongogettersetter-1.3.6/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-07 23:47:35.000000 mongogettersetter-1.3.6/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-07 23:47:35.857672 mongogettersetter-1.3.6/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-07 23:46:50.000000 mongogettersetter-1.3.6/setup.py
```

### Comparing `mongogettersetter-1.3.5/PKG-INFO` & `mongogettersetter-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.5
+Version: 1.3.6
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.5/README.md` & `mongogettersetter-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `mongogettersetter-1.3.5/mongogettersetter/__init__.py` & `mongogettersetter-1.3.6/mongogettersetter/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import json
-from .MongoDataWrapper import MongoDataWrapper
-from .MongoDictWrapper import MongoDictWrapper
-
 
 class MongoGetterSetter(type):
 
     """
     `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
     """
 
@@ -45,34 +42,34 @@
             """
             Return the value of the key in the array/string/object
             """
             data = self._collection.find_one(self._filter_query)
             if _key in data and isinstance(data[_key], dict):
                 dictwrapper = MongoDictWrapper(data[_key])
                 dictwrapper.prepare(
-                    [_key], self._collection, self._filter_query
+                    data, [_key], self._collection, self._filter_query
                 )
                 return dictwrapper
             else:
                 return MongoDataWrapper(data, [_key], self._collection, self._filter_query)
 
         def __getitem__(self, _key):
             """
             Return the value of the key in the array/string/object
             """
             #TODO: make sure the filter query runs only once
             data = self._collection.find_one(self._filter_query)
             if _key in data and isinstance(data[_key], dict):
                 dictwrapper = MongoDictWrapper(data)
                 dictwrapper.prepare(
-                    [_key], self._collection, self._filter_query
+                    data, [_key], self._collection, self._filter_query
                 )
                 return dictwrapper
             else:
-                return MongoDataWrapper([_key], self._collection, self._filter_query)
+                return MongoDataWrapper(data, [_key], self._collection, self._filter_query)
 
         def __setattr__(self, _key, value):
             """
             Set the value of the key in the array/string/object
             """
             _filter_query = self._filter_query
             self._collection.update_one(_filter_query, {"$set": {_key: value}})
@@ -158,31 +155,36 @@
     `MongoDataWrapper` is a subscriptable class, which wraps MongoDB document datatypes to provide MongoDB Array/List Operations over a simple, straightforward API to perform various operations on the MongoDB collection. Check the list of methods for the allowed operations.
     """
 
     def __init__(self, data, _key, _collection, _filter_query):
         self._data = data
         self._filter_query = _filter_query
         self._collection = _collection
-        self._key = _key[0]
         self._keys = _key
 
-    def get(self, _key=None):
+    def get(self, _key=None, realtime=False):
         """
         Get the original representation of the document as it exists without MongoGetterSetter Wrappers.
-                If no arguments are passed, then return the whole data.
-                If _key is passed, it will return the specific value w.r.t the key.
+        If no arguments are passed, then return the whole data.
+        If _key is passed, it will return the specific value w.r.t the key.
+        If realtime is set to true, the data is fetched from MongoDB in realtime
 
-                Args:
-                    _key (any|None, optional):  Defaults to None.
+        Args:
+            _key (any|None, optional):  Defaults to None.
+            realtime (bool, optional): Defaults to False
 
-                Returns:
-                    any: Original Data without Wrapper
+        Returns:
+            any: Original Data without Wrapper
 
         """
-        nested_dict = self._collection.find_one(self._filter_query)
+        if realtime:
+            self._data = nested_dict = self._collection.find_one(self._filter_query)
+        else:
+            nested_dict = self._data
+
         for k in self._keys:
             nested_dict = nested_dict[k]
         if _key is None:
             return nested_dict
         else:
             return nested_dict[_key]
 
@@ -195,103 +197,101 @@
         return self._collection.find_one({path: {"$in": [value]}})
 
     def append(self, *value):
         """
         Append the value to the array. Returns True if the value is appended, else False.
         """
 
-        return self.push(*value)
+        result = self.push(*value)
+        self._data = self._collection.find_one(self._filter_query)
+        return result
 
     def push(self, *values, maximum=0):
         """
         Push the value to the array. Returns True if the value is pushed, else False.
         """
 
         path = ".".join(str(v) for v in self._keys)
         if maximum == 0:
-            return (
-                self._collection.update_one(
-                    self._filter_query, {"$push": {path: {"$each": values}}}
-                ).modified_count
-                > 0
+            result = self._collection.update_one(
+                self._filter_query, {"$push": {path: {"$each": values}}}
             )
+            self._data = self._collection.find_one(self._filter_query)
+            return result.modified_count > 0
         else:
             update_operation = {"$push": {path: {"$each": values, "$slice": -maximum}}}
 
-            return (
-                self._collection.update_one(
-                    self._filter_query, update_operation
-                ).modified_count
-                > 0
-            )
+            result = self._collection.update_one(
+                self._filter_query, update_operation
+            ).modified_count
+            self._data = self._collection.find_one(self._filter_query)
+            return result.modified_count > 0
 
     def addToSet(self, value):
         """
         Add the value to the array if it does not exist. Returns True if the value is added, else False.
         """
 
         path = ".".join(str(v) for v in self._keys)
-        return (
-            self._collection.update_one(
-                self._filter_query, {"$addToSet": {path: value}}
-            ).modified_count
-            > 0
+        result = self._collection.update_one(
+            self._filter_query, {"$addToSet": {path: value}}
         )
+        self._data = self._collection.find_one(self._filter_query)
+        return result.modified_count > 0
 
     def pop(self, direction=1):
         """
         Pop the value from the array. Returns True if the value is popped, else False. direction=1 for popping from the end, direction=-1 for popping from the beginning.
         """
 
         path = ".".join(str(v) for v in self._keys)
-        return (
-            self._collection.update_one(
-                self._filter_query, {"$pop": {path: direction}}
-            ).modified_count
-            > 0
+        result = self._collection.update_one(
+            self._filter_query, {"$pop": {path: direction}}
         )
+        self._data = self._collection.find_one(self._filter_query)
+        return result.modified_count > 0
 
     def remove(self, item):
         """
         Remove the value from the array. Returns True if the value is removed, else False.
         """
 
-        return self.pull(item)
+        result = self.pull(item)
+        self._data = self._collection.find_one(self._filter_query)
+        return result
 
     def count(self):
         """
         Return the length of the array/string/object
         """
 
         return self.__len__()
 
     def pull(self, value):
         """
         Remove the value from the array. Returns True if the value is removed, else False.
         """
-
+        
         path = ".".join(str(v) for v in self._keys)
-        return (
-            self._collection.update_one(
-                self._filter_query, {"$pull": {path: value}}
-            ).modified_count
-            > 0
+        result = self._collection.update_one(
+            self._filter_query, {"$pull": {path: value}}
         )
+        self._data = self._collection.find_one(self._filter_query)
+        return result.modified_count > 0
 
     def insert(self, index, value):
         """
         Insert the value at the index in the array. Returns True if the value is inserted, else False.
         """
 
         path = ".".join(str(v) for v in self._keys)
         insert_query = {"$push": {path: {"$each": [value], "$position": index}}}
-        return (
-            self._collection.update_one(self._filter_query, insert_query).modified_count
-            > 0
-        )
+        result = self._collection.update_one(self._filter_query, insert_query)
+        self._data = self._collection.find_one(self._filter_query)
+        return result.modified_count > 0
         
     def index(self, value):
         """
         Find the index of the value in array. If the value is not present, you will get -1.
         """
         path = ".".join(str(v) for v in self._keys)
         # print(path)
@@ -312,20 +312,19 @@
 
     def pullAll(self, *values):
         """
         Remove all the (given) values from the array. Returns True if the value is removed, else False.
         """
 
         path = ".".join(str(v) for v in self._keys)
-        return (
-            self._collection.update_one(
-                self._filter_query, {"$pullAll": {path: values}}
-            ).modified_count
-            > 0
+        result = self._collection.update_one(
+            self._filter_query, {"$pullAll": {path: values}}
         )
+        self._data = self._collection.find_one(self._filter_query)
+        return result.modified_count > 0
 
     def matchSize(self, value):
         """
         Check if the array has the given size. Returns True if the array has the given size, else False.
         """
 
         path = ".".join(str(v) for v in self._keys)
@@ -354,23 +353,22 @@
 
         path = ".".join(str(v) for v in self._keys)
         _filter_query = dict(self._filter_query)
         update_query = {
             path + f".$[elem]." + _key: value for _key, value in kvalues.items()
         }
         _filter_query[path + "." + field] = match
-        return (
-            self._collection.update_one(
-                self._filter_query,
-                {"$set": update_query},
-                array_filters=[{f"elem.{field}": match}],
-                upsert=True,
-            ).modified_count
-            > 0
+        result = self._collection.update_one(
+            self._filter_query,
+            {"$set": update_query},
+            array_filters=[{f"elem.{field}": match}],
+            upsert=True,
         )
+        self._data = self._collection.find_one(self._filter_query)
+        return result.modified_count > 0
 
     def __len__(self):
         """
         Return the length of the array/string/object
         """
 
         return len(self.get())
@@ -426,174 +424,179 @@
         return bool(nested_dict)
 
     def __getitem__(self, _key):
         """
         Return the value of the key in the array/string/object
         """
 
-        data = self.get(_key)
+        data = self.get(_key, realtime=True)
         # return data[_key]
         if isinstance(data, dict):
             dictwrapper = MongoDictWrapper(data)
             dictwrapper.prepare(
-                self._keys + [_key], self._collection, self._filter_query
+                self._data, self._keys + [_key], self._collection, self._filter_query
             )
             return dictwrapper
-        elif isinstance(data, list):
+        else:
             datawrapper = MongoDataWrapper(
-                data, self._keys + [_key], self._collection, self._filter_query
+                self._data, self._keys + [_key], self._collection, self._filter_query
             )
             return datawrapper
-        else:
-            return data
 
     def __getattr__(self, _key):
         """
         Return the value of the key in the array/string/object
         """
 
         if _key in self.__dict__:
             return self.__dict__[_key]
         else:
-            data = self.get(_key)
+            data = self.get(_key, realtime=True)
             # return data[_key]
             if isinstance(data, dict):
                 dictwrapper = MongoDictWrapper(data)
                 dictwrapper.prepare(
-                    data, self._keys + [_key], self._collection, self._filter_query
+                    self._data, self._keys + [_key], self._collection, self._filter_query
                 )
                 return dictwrapper
-            elif isinstance(data, list):
+            else:
                 datawrapper = MongoDataWrapper(
-                    data, self._keys + [_key], self._collection, self._filter_query
+                    self._data, self._keys + [_key], self._collection, self._filter_query
                 )
                 return datawrapper
-            else:
-                return data
 
     def __setattr__(self, _key, value):
         """
         Set the value of the key in the array/string/object
         """
         _key = str(_key)
-        if _key in ["_filter_query", "_collection", "_key", "_keys", "_data"]:
+        if _key in ["_filter_query", "_collection", "_keys", "_data"]:
             self.__dict__[_key] = value
         else:
             path = ".".join(str(v) for v in self._keys)
             self._collection.update_one(
                 self._filter_query, {"$set": {path + "." + _key: value}}
             )
-            # # print("__setattr__", _key, value)
+            self._data = self._collection.find_one(self._filter_query)
 
     def __setitem__(self, index, value):
         """
         Set the value of the key in the array/string/object
         """
         path = ".".join(str(v) for v in self._keys)
         update_query = {path + "." + str(index): value}
         self._collection.update_one(self._filter_query, {"$set": update_query})
+        self._data = self._collection.find_one(self._filter_query)
 
     def __delitem__(self, _key):
         """
         Delete the key in the array/string/object using del keyword
         """
         path = ".".join(str(v) for v in self._keys)
         data = self.get()
         _key = str(_key)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
         if isinstance(data, list):
             self.pull(None)
+        self._data = self._collection.find_one(self._filter_query)
 
     def __delattr__(self, _key):
         """
         Delete the key in the array/string/object using del keyword
         """
         path = ".".join(str(v) for v in self._keys)
         data = self.get()
         _key = str(_key)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
         if isinstance(data, list):
             self.pull(None)
-    
+        self._data = self._collection.find_one(self._filter_query)
+
     def delete(self):
         """
         Delete the nested object from the MongoDB Document using $unset
         """
         
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path: ""}}
         )
-        
-
+        self._data = self._collection.find_one(self._filter_query)
+    
+    def refresh(self):
+        self._data = self._collection.find_one(self._filter_query)
 
 class MongoDictWrapper(dict):
     """
     MongoDictWrapper is a wrapper around the dictionary object to provide the functionality of updating the database when the dictionary is updated. It is used to wrap the dictionary object in the MongoGetterSetter class. It is not meant to be used directly.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+    
+    def refresh(self):
+        self._data = self._collection.find_one(self._filter_query)
 
-    def prepare(self, _key, _collection, _filter_query):
+    def prepare(self, _data, _keys, _collection, _filter_query):
         """
         Prepare the MongoDictWrapper object to be used. This method is called by the MongoGetterSetter class when the object is created.
         """
-
+        self._data = _data
         self._filter_query = _filter_query
         self._collection = _collection
-        self._key = _key[0]
-        self._keys = _key
+        self._keys = _keys
         # path = '.'.join(str(v) for v in self._keys)
         # print(f"__prepare__ you are at: {path}")
 
     def __setattr__(self, _key, value):
         _key = str(_key)
         """
         Set the value of the key in the dictionary and update the database.
         """
-        if _key in ["_filter_query", "_collection", "_key", "_keys"]:
+        if _key in ["_filter_query", "_collection", "_keys", "_data"]:
             self.__dict__[_key] = value
         else:
             # Call the parent __setitem__ method to actually set the value in the dictionary
             path = ".".join(str(v) for v in self._keys)
             # Execute your function here
             # # print(f"Dictionary updated: {path}.{_key}={value}")
             update = {"$set": {"{}.{}".format(path, _key): value}}
             result = self._collection.update_one(self._filter_query, update)
             nested_dict = self._collection.find_one(self._filter_query)
             for k in self._keys:
                 nested_dict = nested_dict[k]
             # print(f"__setitem__ {str(nested_dict)}")
             super().update(nested_dict)
+            self._data = self._collection.find_one(self._filter_query)
+        
 
     def __getattr__(self, _key):
         """
         Get the value of the key in the dictionary.
         """
         _key = str(_key)
         if _key in self.__dict__:
             return self.__dict__[_key]
         else:
             path = ".".join(str(v) for v in self._keys)
             # print(f"__getitem__ you are at: {path}")
-            original_dict = self._collection.find_one(self._filter_query)
-            nested_dict = original_dict
+            original_dict = self._data
+            nested_dict = dict(original_dict)
             for k in self._keys:
                 nested_dict = nested_dict[k]
             super().update(nested_dict)
             # print(f"__getitem__ {str(nested_dict)}")
             if isinstance(nested_dict[_key], dict):
                 dictwrapper = MongoDictWrapper(nested_dict[_key])
                 dictwrapper.prepare(
-                    self._keys + [_key], self._collection, self._filter_query
+                    original_dict, self._keys + [_key], self._collection, self._filter_query
                 )
                 return dictwrapper
             elif isinstance(nested_dict[_key], list):
                 datawrapper = MongoDataWrapper(
                     original_dict + [_key], self._collection, self._filter_query
                 )
                 return datawrapper
@@ -603,29 +606,29 @@
     def __getitem__(self, _key):
         _key = str(_key)
         """
         Get the value of the key in the dictionary.
         """
         path = ".".join(str(v) for v in self._keys)
         # print(f"__getitem__ you are at: {path}")
-        original_dict = self._collection.find_one(self._filter_query)
-        nested_dict = original_dict
+        original_dict = self._data
+        nested_dict = dict(original_dict)
         for k in self._keys:
             nested_dict = nested_dict[k]
         super().update(nested_dict)
         # print(f"__getitem__ {str(nested_dict)}")
         if isinstance(nested_dict[_key], dict):
             dictwrapper = MongoDictWrapper(nested_dict[_key])
             dictwrapper.prepare(
-                self._keys + [_key], self._collection, self._filter_query
+                original_dict, self._keys + [_key], self._collection, self._filter_query
             )
             return dictwrapper
         elif isinstance(nested_dict[_key], list):
             datawrapper = MongoDataWrapper(
-                self._keys + [_key], self._collection, self._filter_query
+                original_dict, self._keys + [_key], self._collection, self._filter_query
             )
             return datawrapper
         else:
             return nested_dict[_key]
 
     def __setitem__(self, _key, value):
         _key = str(_key)
@@ -634,15 +637,15 @@
         """
         # Call the parent __setitem__ method to actually set the value in the dictionary
         path = ".".join(str(v) for v in self._keys)
         # Execute your function here
         # # print(f"Dictionary updated: {path}.{_key}={value}")
         update = {"$set": {"{}.{}".format(path, _key): value}}
         result = self._collection.update_one(self._filter_query, update)
-        nested_dict = self._collection.find_one(self._filter_query)
+        self._data = nested_dict = self._collection.find_one(self._filter_query)
         for k in self._keys:
             nested_dict = nested_dict[k]
         # print(f"__setitem__ {str(nested_dict)}")
         super().update(nested_dict)
 
     def __delitem__(self, _key):
         _key = str(_key)
@@ -650,35 +653,38 @@
         Delete the item from the dictionary and update the database.
         """
         super().__delitem__(_key)
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
+        self._data = self._collection.find_one(self._filter_query)
 
     def __delattr_(self, _key):
         _key = str(_key)
         """
         Delete the item from the dictionary and update the database.
         """
         super().__delitem__(_key)
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
+        self._data = self._collection.find_one(self._filter_query)
     
     def delete(self):
         """
         Delete the nested object from the MongoDB Document using $unset
         """
         
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path: ""}}
         )
+        self._data = self._collection.find_one(self._filter_query)
 
     def get(self, _key=None, default=None):
         """
         Get the value of the key from the dictionary. If the key is not present, return the default value.
         """
         if _key is None:
             return dict(self)
```

### Comparing `mongogettersetter-1.3.5/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.3.6/mongogettersetter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.5
+Version: 1.3.6
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.5/setup.py` & `mongogettersetter-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.3.5',
+    version='1.3.6',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean realtime way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

