# Comparing `tmp/umjunsik-2.0.1.tar.gz` & `tmp/umjunsik-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umjunsik-2.0.1.tar", last modified: Mon May  8 13:43:12 2023, max compression
+gzip compressed data, was "umjunsik-2.0.2.tar", last modified: Mon May  8 13:45:41 2023, max compression
```

## Comparing `umjunsik-2.0.1.tar` & `umjunsik-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-05-08 13:43:12.550579 umjunsik-2.0.1/
--rw-r--r--   0 hiyabye    (501) staff       (20)    18360 2023-05-08 13:43:12.550390 umjunsik-2.0.1/PKG-INFO
--rw-r--r--   0 hiyabye    (501) staff       (20)       38 2023-05-08 13:43:12.550632 umjunsik-2.0.1/setup.cfg
--rw-r--r--   0 hiyabye    (501) staff       (20)      912 2023-05-08 13:43:02.000000 umjunsik-2.0.1/setup.py
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-05-08 13:43:12.549366 umjunsik-2.0.1/umjunsik/
--rw-r--r--   0 hiyabye    (501) staff       (20)       30 2023-05-08 08:21:44.000000 umjunsik-2.0.1/umjunsik/__init__.py
--rw-r--r--   0 hiyabye    (501) staff       (20)      372 2023-05-08 13:41:41.000000 umjunsik-2.0.1/umjunsik/__main__.py
--rw-r--r--   0 hiyabye    (501) staff       (20)     3010 2023-05-08 13:41:53.000000 umjunsik-2.0.1/umjunsik/umjunsik.py
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-05-08 13:43:12.550170 umjunsik-2.0.1/umjunsik.egg-info/
--rw-r--r--   0 hiyabye    (501) staff       (20)    18360 2023-05-08 13:43:12.000000 umjunsik-2.0.1/umjunsik.egg-info/PKG-INFO
--rw-r--r--   0 hiyabye    (501) staff       (20)      234 2023-05-08 13:43:12.000000 umjunsik-2.0.1/umjunsik.egg-info/SOURCES.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)        1 2023-05-08 13:43:12.000000 umjunsik-2.0.1/umjunsik.egg-info/dependency_links.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)       64 2023-05-08 13:43:12.000000 umjunsik-2.0.1/umjunsik.egg-info/entry_points.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)        9 2023-05-08 13:43:12.000000 umjunsik-2.0.1/umjunsik.egg-info/top_level.txt
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-05-08 13:45:41.895593 umjunsik-2.0.2/
+-rw-r--r--   0 hiyabye    (501) staff       (20)    18360 2023-05-08 13:45:41.895408 umjunsik-2.0.2/PKG-INFO
+-rw-r--r--   0 hiyabye    (501) staff       (20)       38 2023-05-08 13:45:41.895631 umjunsik-2.0.2/setup.cfg
+-rw-r--r--   0 hiyabye    (501) staff       (20)      900 2023-05-08 13:45:24.000000 umjunsik-2.0.2/setup.py
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-05-08 13:45:41.894338 umjunsik-2.0.2/umjunsik/
+-rw-r--r--   0 hiyabye    (501) staff       (20)       30 2023-05-08 08:21:44.000000 umjunsik-2.0.2/umjunsik/__init__.py
+-rw-r--r--   0 hiyabye    (501) staff       (20)      372 2023-05-08 13:41:41.000000 umjunsik-2.0.2/umjunsik/__main__.py
+-rw-r--r--   0 hiyabye    (501) staff       (20)     3010 2023-05-08 13:41:53.000000 umjunsik-2.0.2/umjunsik/umjunsik.py
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-05-08 13:45:41.895130 umjunsik-2.0.2/umjunsik.egg-info/
+-rw-r--r--   0 hiyabye    (501) staff       (20)    18360 2023-05-08 13:45:41.000000 umjunsik-2.0.2/umjunsik.egg-info/PKG-INFO
+-rw-r--r--   0 hiyabye    (501) staff       (20)      234 2023-05-08 13:45:41.000000 umjunsik-2.0.2/umjunsik.egg-info/SOURCES.txt
+-rw-r--r--   0 hiyabye    (501) staff       (20)        1 2023-05-08 13:45:41.000000 umjunsik-2.0.2/umjunsik.egg-info/dependency_links.txt
+-rw-r--r--   0 hiyabye    (501) staff       (20)       52 2023-05-08 13:45:41.000000 umjunsik-2.0.2/umjunsik.egg-info/entry_points.txt
+-rw-r--r--   0 hiyabye    (501) staff       (20)        9 2023-05-08 13:45:41.000000 umjunsik-2.0.2/umjunsik.egg-info/top_level.txt
```

### Comparing `umjunsik-2.0.1/PKG-INFO` & `umjunsik-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umjunsik
-Version: 2.0.1
+Version: 2.0.2
 Summary: 어떻게 엄준식이 언어이름이냐🤣
 Home-page: https://github.com/rycont/umjunsik-lang
 Author: rycont
 Author-email: rycont@outlook.kr
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: umjunsik Version: 2.0.1 Summary: ì´ë»ê²
+Metadata-Version: 2.1 Name: umjunsik Version: 2.0.2 Summary: ì´ë»ê²
 ìì¤ìì´ ì¸ì´ì´ë¦ì´ëð¤£ Home-page: https://github.com/rycont/
 umjunsik-lang Author: rycont Author-email: rycont@outlook.kr Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown # ìë­
```

### Comparing `umjunsik-2.0.1/setup.py` & `umjunsik-2.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="umjunsik",
-    version="2.0.1",
+    version="2.0.2",
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'umjunsik-interpreter=umjunsik.__main__:main',
+            'umjunsik=umjunsik.__main__:main',
         ],
     },
     author="rycont",
     author_email="rycont@outlook.kr",
     description="어떻게 엄준식이 언어이름이냐🤣",
     long_description=open("../README.md", "r", encoding="UTF-8").read(),
     long_description_content_type="text/markdown",
```

### Comparing `umjunsik-2.0.1/umjunsik/umjunsik.py` & `umjunsik-2.0.2/umjunsik/umjunsik.py`

 * *Files identical despite different names*

### Comparing `umjunsik-2.0.1/umjunsik.egg-info/PKG-INFO` & `umjunsik-2.0.2/umjunsik.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umjunsik
-Version: 2.0.1
+Version: 2.0.2
 Summary: 어떻게 엄준식이 언어이름이냐🤣
 Home-page: https://github.com/rycont/umjunsik-lang
 Author: rycont
 Author-email: rycont@outlook.kr
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: umjunsik Version: 2.0.1 Summary: ì´ë»ê²
+Metadata-Version: 2.1 Name: umjunsik Version: 2.0.2 Summary: ì´ë»ê²
 ìì¤ìì´ ì¸ì´ì´ë¦ì´ëð¤£ Home-page: https://github.com/rycont/
 umjunsik-lang Author: rycont Author-email: rycont@outlook.kr Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown # ìë­
```

