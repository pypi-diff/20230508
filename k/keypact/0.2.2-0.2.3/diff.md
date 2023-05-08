# Comparing `tmp/keypact-0.2.2.tar.gz` & `tmp/keypact-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.2.2.tar", last modified: Tue May  2 21:34:01 2023, max compression
+gzip compressed data, was "keypact-0.2.3.tar", last modified: Mon May  8 20:06:35 2023, max compression
```

## Comparing `keypact-0.2.2.tar` & `keypact-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:34:01.680651 keypact-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-02 21:33:49.000000 keypact-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-02 21:34:01.680651 keypact-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-02 21:33:49.000000 keypact-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:34:01.680651 keypact-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-02 21:33:49.000000 keypact-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:34:01.676651 keypact-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:34:01.676651 keypact-0.2.2/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 21:33:49.000000 keypact-0.2.2/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-02 21:33:49.000000 keypact-0.2.2/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:34:01.680651 keypact-0.2.2/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:06:35.579814 keypact-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-08 20:06:25.000000 keypact-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 20:06:35.579814 keypact-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 20:06:25.000000 keypact-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:06:35.579814 keypact-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-08 20:06:25.000000 keypact-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:06:35.579814 keypact-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:06:35.579814 keypact-0.2.3/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 20:06:25.000000 keypact-0.2.3/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-08 20:06:25.000000 keypact-0.2.3/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:06:35.579814 keypact-0.2.3/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 20:06:35.000000 keypact-0.2.3/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 20:06:35.000000 keypact-0.2.3/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:06:35.000000 keypact-0.2.3/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 20:06:35.000000 keypact-0.2.3/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:06:35.000000 keypact-0.2.3/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 20:06:35.000000 keypact-0.2.3/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 20:06:35.000000 keypact-0.2.3/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.2.2/LICENSE` & `keypact-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.2.2/PKG-INFO` & `keypact-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.2.2
+Version: 0.2.3
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded.
```

### Comparing `keypact-0.2.2/README.md` & `keypact-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `keypact-0.2.2/setup.py` & `keypact-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.2.2',
+version='0.2.3',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `keypact-0.2.2/src/keypact/keypact.py` & `keypact-0.2.3/src/keypact/keypact.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import os
 from hashlib import sha256
 import pickle
 
 import fire
 
+import time
 
 class KeyPact:
 
     def __init__(self, name):
         self.name = name
         self.hashed_name = sha256(name.encode()).hexdigest()
         self.location = os.path.join(os.getcwd(), "kp-" + self.hashed_name)
@@ -34,45 +35,47 @@
         with open(os.path.join(self.location, key_location), "wb") as f:
             pickle.dump({"key":key,"value":value}, f)
 
     def get(self, key: str, custom_key_location: str = None):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest()) if custom_key_location == None else custom_key_location
 
         if not os.path.isfile(os.path.join(self.location, key_location)):
-            raise FileNotFoundError("Key not found")
+            return None
 
         total_result = None
         while total_result == None:
             try:
                 with open(os.path.join(self.location, key_location), "rb") as f:
                     result = pickle.load(f)
                     try:
                         total_result = result["value"]
                     except TypeError:
                         total_result = result
             except EOFError:
                 pass
+            time.sleep(0.1)
         return total_result
 
     def get_key(self, key_location: str):
        
 
         if not os.path.isfile(os.path.join(self.location, key_location)):
-            raise FileNotFoundError("Key not found")
+            return None
         total_result = None
         while total_result == None:
             try:
                 with open(os.path.join(self.location, key_location), "rb") as f:
                     result = pickle.load(f)
                     try:
                         total_result = result["key"]
                     except TypeError:
                         total_result = False
             except EOFError:
-                pass                        
+                pass
+            time.sleep(0.1)               
         return total_result
 
     def delete(self, key: str):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
 
         try:
             os.remove(os.path.join(self.location, key_location))
@@ -80,13 +83,16 @@
             pass
 
 
     def dict(self):
         result ={}
         for key in os.listdir(self.location):
             the_key = self.get_key(key)
-            if the_key != False:
-                result[the_key] = self.get(the_key)
+            if not the_key is None:
+                if the_key != False:
+                    result_of_key = self.get(the_key)
+                    if not result_of_key is None:
+                        result[the_key] = result_of_key
         return result
 
 def main():
     fire.Fire(KeyPact)
```

### Comparing `keypact-0.2.2/src/keypact.egg-info/PKG-INFO` & `keypact-0.2.3/src/keypact.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.2.2
+Version: 0.2.3
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded.
```

