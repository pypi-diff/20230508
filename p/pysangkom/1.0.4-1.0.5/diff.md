# Comparing `tmp/pysangkom-1.0.4.tar.gz` & `tmp/pysangkom-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysangkom-1.0.4.tar", last modified: Mon May  8 10:38:47 2023, max compression
+gzip compressed data, was "pysangkom-1.0.5.tar", last modified: Mon May  8 10:45:55 2023, max compression
```

## Comparing `pysangkom-1.0.4.tar` & `pysangkom-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:38:47.819733 pysangkom-1.0.4/
--rw-r--r--   0 kang49     (501) staff       (20)     1099 2023-05-08 10:38:47.819542 pysangkom-1.0.4/PKG-INFO
--rw-r--r--   0 kang49     (501) staff       (20)      535 2023-05-08 10:29:19.000000 pysangkom-1.0.4/README.md
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:38:47.818331 pysangkom-1.0.4/pysangkom/
--rw-r--r--   0 kang49     (501) staff       (20)        0 2023-05-08 09:36:30.000000 pysangkom-1.0.4/pysangkom/__init__.py
--rw-r--r--   0 kang49     (501) staff       (20)    40090 2023-05-08 10:15:04.000000 pysangkom-1.0.4/pysangkom/forkyou.py
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:38:47.819350 pysangkom-1.0.4/pysangkom.egg-info/
--rw-r--r--   0 kang49     (501) staff       (20)     1099 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/PKG-INFO
--rw-r--r--   0 kang49     (501) staff       (20)      225 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/SOURCES.txt
--rw-r--r--   0 kang49     (501) staff       (20)        1 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/dependency_links.txt
--rw-r--r--   0 kang49     (501) staff       (20)       31 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/requires.txt
--rw-r--r--   0 kang49     (501) staff       (20)       10 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/top_level.txt
--rw-r--r--   0 kang49     (501) staff       (20)       38 2023-05-08 10:38:47.819783 pysangkom-1.0.4/setup.cfg
--rw-r--r--   0 kang49     (501) staff       (20)      902 2023-05-08 10:38:44.000000 pysangkom-1.0.4/setup.py
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:45:55.862416 pysangkom-1.0.5/
+-rw-r--r--   0 kang49     (501) staff       (20)     1175 2023-05-08 10:45:55.862185 pysangkom-1.0.5/PKG-INFO
+-rw-r--r--   0 kang49     (501) staff       (20)      608 2023-05-08 10:44:31.000000 pysangkom-1.0.5/README.md
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:45:55.860856 pysangkom-1.0.5/pysangkom/
+-rw-r--r--   0 kang49     (501) staff       (20)        0 2023-05-08 09:36:30.000000 pysangkom-1.0.5/pysangkom/__init__.py
+-rw-r--r--   0 kang49     (501) staff       (20)    40090 2023-05-08 10:15:04.000000 pysangkom-1.0.5/pysangkom/forkyou.py
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:45:55.861989 pysangkom-1.0.5/pysangkom.egg-info/
+-rw-r--r--   0 kang49     (501) staff       (20)     1175 2023-05-08 10:45:55.000000 pysangkom-1.0.5/pysangkom.egg-info/PKG-INFO
+-rw-r--r--   0 kang49     (501) staff       (20)      225 2023-05-08 10:45:55.000000 pysangkom-1.0.5/pysangkom.egg-info/SOURCES.txt
+-rw-r--r--   0 kang49     (501) staff       (20)        1 2023-05-08 10:45:55.000000 pysangkom-1.0.5/pysangkom.egg-info/dependency_links.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       31 2023-05-08 10:45:55.000000 pysangkom-1.0.5/pysangkom.egg-info/requires.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       10 2023-05-08 10:45:55.000000 pysangkom-1.0.5/pysangkom.egg-info/top_level.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       38 2023-05-08 10:45:55.862464 pysangkom-1.0.5/setup.cfg
+-rw-r--r--   0 kang49     (501) staff       (20)      905 2023-05-08 10:45:29.000000 pysangkom-1.0.5/setup.py
```

### Comparing `pysangkom-1.0.4/PKG-INFO` & `pysangkom-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pysangkom
-Version: 1.0.4
+Version: 1.0.5
 Summary: This library is pysangkom, Please becareful
-Author: m_keen
+Author: Meta_Keen
 Author-email: vxfqkn8wtx@privaterelay.appleid.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,7 +22,8 @@
 
 ## How to use
 <pre>
 from pysangkom.forkyou import pysangkom
 
 call = pysangkom.pysangkom()
 </pre>
+![Views](https://visitor-badge.glitch.me/badge?page_id=kang49.pysangkom)
```

### Comparing `pysangkom-1.0.4/pysangkom/forkyou.py` & `pysangkom-1.0.5/pysangkom/forkyou.py`

 * *Files identical despite different names*

### Comparing `pysangkom-1.0.4/pysangkom.egg-info/PKG-INFO` & `pysangkom-1.0.5/pysangkom.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pysangkom
-Version: 1.0.4
+Version: 1.0.5
 Summary: This library is pysangkom, Please becareful
-Author: m_keen
+Author: Meta_Keen
 Author-email: vxfqkn8wtx@privaterelay.appleid.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,7 +22,8 @@
 
 ## How to use
 <pre>
 from pysangkom.forkyou import pysangkom
 
 call = pysangkom.pysangkom()
 </pre>
+![Views](https://visitor-badge.glitch.me/badge?page_id=kang49.pysangkom)
```

### Comparing `pysangkom-1.0.4/setup.py` & `pysangkom-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='pysangkom',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
-    author='m_keen',
+    author='Meta_Keen',
     author_email='vxfqkn8wtx@privaterelay.appleid.com',
     description='This library is pysangkom, Please becareful',
     long_description=long_description,
     long_description_content_type='text/markdown',
     readme = "README.md",
     install_requires=[
         'numpy>=1.24.0',
```

