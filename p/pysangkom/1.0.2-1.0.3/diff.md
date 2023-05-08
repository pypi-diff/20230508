# Comparing `tmp/pysangkom-1.0.2.tar.gz` & `tmp/pysangkom-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysangkom-1.0.2.tar", last modified: Mon May  8 10:29:47 2023, max compression
+gzip compressed data, was "pysangkom-1.0.3.tar", last modified: Mon May  8 10:32:13 2023, max compression
```

## Comparing `pysangkom-1.0.2.tar` & `pysangkom-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:29:47.908106 pysangkom-1.0.2/
--rw-r--r--   0 kang49     (501) staff       (20)      522 2023-05-08 10:29:47.907881 pysangkom-1.0.2/PKG-INFO
--rw-r--r--   0 kang49     (501) staff       (20)      535 2023-05-08 10:29:19.000000 pysangkom-1.0.2/README.md
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:29:47.906676 pysangkom-1.0.2/pysangkom/
--rw-r--r--   0 kang49     (501) staff       (20)        0 2023-05-08 09:36:30.000000 pysangkom-1.0.2/pysangkom/__init__.py
--rw-r--r--   0 kang49     (501) staff       (20)    40090 2023-05-08 10:15:04.000000 pysangkom-1.0.2/pysangkom/forkyou.py
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:29:47.907690 pysangkom-1.0.2/pysangkom.egg-info/
--rw-r--r--   0 kang49     (501) staff       (20)      522 2023-05-08 10:29:47.000000 pysangkom-1.0.2/pysangkom.egg-info/PKG-INFO
--rw-r--r--   0 kang49     (501) staff       (20)      225 2023-05-08 10:29:47.000000 pysangkom-1.0.2/pysangkom.egg-info/SOURCES.txt
--rw-r--r--   0 kang49     (501) staff       (20)        1 2023-05-08 10:29:47.000000 pysangkom-1.0.2/pysangkom.egg-info/dependency_links.txt
--rw-r--r--   0 kang49     (501) staff       (20)       31 2023-05-08 10:29:47.000000 pysangkom-1.0.2/pysangkom.egg-info/requires.txt
--rw-r--r--   0 kang49     (501) staff       (20)       10 2023-05-08 10:29:47.000000 pysangkom-1.0.2/pysangkom.egg-info/top_level.txt
--rw-r--r--   0 kang49     (501) staff       (20)       38 2023-05-08 10:29:47.908162 pysangkom-1.0.2/setup.cfg
--rw-r--r--   0 kang49     (501) staff       (20)      718 2023-05-08 10:29:45.000000 pysangkom-1.0.2/setup.py
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:32:13.269567 pysangkom-1.0.3/
+-rw-r--r--   0 kang49     (501) staff       (20)      522 2023-05-08 10:32:13.269354 pysangkom-1.0.3/PKG-INFO
+-rw-r--r--   0 kang49     (501) staff       (20)      535 2023-05-08 10:29:19.000000 pysangkom-1.0.3/README.md
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:32:13.267880 pysangkom-1.0.3/pysangkom/
+-rw-r--r--   0 kang49     (501) staff       (20)        0 2023-05-08 09:36:30.000000 pysangkom-1.0.3/pysangkom/__init__.py
+-rw-r--r--   0 kang49     (501) staff       (20)    40090 2023-05-08 10:15:04.000000 pysangkom-1.0.3/pysangkom/forkyou.py
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:32:13.269131 pysangkom-1.0.3/pysangkom.egg-info/
+-rw-r--r--   0 kang49     (501) staff       (20)      522 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/PKG-INFO
+-rw-r--r--   0 kang49     (501) staff       (20)      225 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/SOURCES.txt
+-rw-r--r--   0 kang49     (501) staff       (20)        1 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/dependency_links.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       31 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/requires.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       10 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/top_level.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       38 2023-05-08 10:32:13.269617 pysangkom-1.0.3/setup.cfg
+-rw-r--r--   0 kang49     (501) staff       (20)      744 2023-05-08 10:32:08.000000 pysangkom-1.0.3/setup.py
```

### Comparing `pysangkom-1.0.2/PKG-INFO` & `pysangkom-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysangkom
-Version: 1.0.2
+Version: 1.0.3
 Summary: This library is pysangkom, Please becareful
 Author: m_keen
 Author-email: vxfqkn8wtx@privaterelay.appleid.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pysangkom-1.0.2/README.md` & `pysangkom-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pysangkom-1.0.2/pysangkom/forkyou.py` & `pysangkom-1.0.3/pysangkom/forkyou.py`

 * *Files identical despite different names*

### Comparing `pysangkom-1.0.2/pysangkom.egg-info/PKG-INFO` & `pysangkom-1.0.3/pysangkom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysangkom
-Version: 1.0.2
+Version: 1.0.3
 Summary: This library is pysangkom, Please becareful
 Author: m_keen
 Author-email: vxfqkn8wtx@privaterelay.appleid.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pysangkom-1.0.2/setup.py` & `pysangkom-1.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pysangkom',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(),
     author='m_keen',
     author_email='vxfqkn8wtx@privaterelay.appleid.com',
     description='This library is pysangkom, Please becareful',
+    readme = "README.md",
     install_requires=[
         'numpy>=1.24.0',
         'requests>=2.30.0'
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

