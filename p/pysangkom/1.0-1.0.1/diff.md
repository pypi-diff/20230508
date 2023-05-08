# Comparing `tmp/pysangkom-1.0.tar.gz` & `tmp/pysangkom-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysangkom-1.0.tar", last modified: Mon May  8 10:23:55 2023, max compression
+gzip compressed data, was "pysangkom-1.0.1.tar", last modified: Mon May  8 10:27:11 2023, max compression
```

## Comparing `pysangkom-1.0.tar` & `pysangkom-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:23:55.901648 pysangkom-1.0/
--rw-r--r--   0 kang49     (501) staff       (20)      520 2023-05-08 10:23:55.901418 pysangkom-1.0/PKG-INFO
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:23:55.900109 pysangkom-1.0/pysangkom/
--rw-r--r--   0 kang49     (501) staff       (20)        0 2023-05-08 09:36:30.000000 pysangkom-1.0/pysangkom/__init__.py
--rw-r--r--   0 kang49     (501) staff       (20)    40090 2023-05-08 10:15:04.000000 pysangkom-1.0/pysangkom/main.py
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:23:55.901230 pysangkom-1.0/pysangkom.egg-info/
--rw-r--r--   0 kang49     (501) staff       (20)      520 2023-05-08 10:23:55.000000 pysangkom-1.0/pysangkom.egg-info/PKG-INFO
--rw-r--r--   0 kang49     (501) staff       (20)      212 2023-05-08 10:23:55.000000 pysangkom-1.0/pysangkom.egg-info/SOURCES.txt
--rw-r--r--   0 kang49     (501) staff       (20)        1 2023-05-08 10:23:55.000000 pysangkom-1.0/pysangkom.egg-info/dependency_links.txt
--rw-r--r--   0 kang49     (501) staff       (20)       31 2023-05-08 10:23:55.000000 pysangkom-1.0/pysangkom.egg-info/requires.txt
--rw-r--r--   0 kang49     (501) staff       (20)       10 2023-05-08 10:23:55.000000 pysangkom-1.0/pysangkom.egg-info/top_level.txt
--rw-r--r--   0 kang49     (501) staff       (20)       38 2023-05-08 10:23:55.901698 pysangkom-1.0/setup.cfg
--rw-r--r--   0 kang49     (501) staff       (20)      716 2023-05-08 10:22:35.000000 pysangkom-1.0/setup.py
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:27:11.859690 pysangkom-1.0.1/
+-rw-r--r--   0 kang49     (501) staff       (20)      522 2023-05-08 10:27:11.859568 pysangkom-1.0.1/PKG-INFO
+-rw-r--r--   0 kang49     (501) staff       (20)      532 2023-05-08 10:26:16.000000 pysangkom-1.0.1/README.md
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:27:11.858367 pysangkom-1.0.1/pysangkom/
+-rw-r--r--   0 kang49     (501) staff       (20)        0 2023-05-08 09:36:30.000000 pysangkom-1.0.1/pysangkom/__init__.py
+-rw-r--r--   0 kang49     (501) staff       (20)    40090 2023-05-08 10:15:04.000000 pysangkom-1.0.1/pysangkom/main.py
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:27:11.859383 pysangkom-1.0.1/pysangkom.egg-info/
+-rw-r--r--   0 kang49     (501) staff       (20)      522 2023-05-08 10:27:11.000000 pysangkom-1.0.1/pysangkom.egg-info/PKG-INFO
+-rw-r--r--   0 kang49     (501) staff       (20)      222 2023-05-08 10:27:11.000000 pysangkom-1.0.1/pysangkom.egg-info/SOURCES.txt
+-rw-r--r--   0 kang49     (501) staff       (20)        1 2023-05-08 10:27:11.000000 pysangkom-1.0.1/pysangkom.egg-info/dependency_links.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       31 2023-05-08 10:27:11.000000 pysangkom-1.0.1/pysangkom.egg-info/requires.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       10 2023-05-08 10:27:11.000000 pysangkom-1.0.1/pysangkom.egg-info/top_level.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       38 2023-05-08 10:27:11.859735 pysangkom-1.0.1/setup.cfg
+-rw-r--r--   0 kang49     (501) staff       (20)      718 2023-05-08 10:27:01.000000 pysangkom-1.0.1/setup.py
```

### Comparing `pysangkom-1.0/PKG-INFO` & `pysangkom-1.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysangkom
-Version: 1.0
+Version: 1.0.1
 Summary: This library is pysangkom, Please becareful
 Author: m_keen
 Author-email: vxfqkn8wtx@privaterelay.appleid.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pysangkom-1.0/pysangkom/main.py` & `pysangkom-1.0.1/pysangkom/main.py`

 * *Files identical despite different names*

### Comparing `pysangkom-1.0/pysangkom.egg-info/PKG-INFO` & `pysangkom-1.0.1/pysangkom.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysangkom
-Version: 1.0
+Version: 1.0.1
 Summary: This library is pysangkom, Please becareful
 Author: m_keen
 Author-email: vxfqkn8wtx@privaterelay.appleid.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pysangkom-1.0/setup.py` & `pysangkom-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pysangkom',
-    version='1.0',
+    version='1.0.1',
     packages=find_packages(),
     author='m_keen',
     author_email='vxfqkn8wtx@privaterelay.appleid.com',
     description='This library is pysangkom, Please becareful',
     install_requires=[
         'numpy>=1.24.0',
         'requests>=2.30.0'
```

