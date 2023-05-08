# Comparing `tmp/CreateAI-0.8.2.tar.gz` & `tmp/CreateAI-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CreateAI-0.8.2.tar", last modified: Mon May  8 12:25:55 2023, max compression
+gzip compressed data, was "CreateAI-0.9.3.tar", last modified: Mon May  8 12:34:47 2023, max compression
```

## Comparing `CreateAI-0.8.2.tar` & `CreateAI-0.9.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 12:25:55.894458 CreateAI-0.8.2/
-drwxrwxrwx   0        0        0        0 2023-05-08 12:25:55.892467 CreateAI-0.8.2/CreateAI.egg-info/
--rw-rw-rw-   0        0        0     2244 2023-05-08 12:25:55.000000 CreateAI-0.8.2/CreateAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-08 12:25:55.000000 CreateAI-0.8.2/CreateAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 12:25:55.000000 CreateAI-0.8.2/CreateAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-08 12:25:55.000000 CreateAI-0.8.2/CreateAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1097 2023-05-05 14:50:25.000000 CreateAI-0.8.2/LICENCE
--rw-rw-rw-   0        0        0       48 2023-05-08 12:25:54.000000 CreateAI-0.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2244 2023-05-08 12:25:55.894458 CreateAI-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     1799 2023-05-08 12:23:43.000000 CreateAI-0.8.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 12:25:55.896029 CreateAI-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-05-08 12:25:54.000000 CreateAI-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:34:46.995071 CreateAI-0.9.3/
+drwxrwxrwx   0        0        0        0 2023-05-08 12:34:46.994067 CreateAI-0.9.3/CreateAI.egg-info/
+-rw-rw-rw-   0        0        0     2244 2023-05-08 12:34:46.000000 CreateAI-0.9.3/CreateAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-08 12:34:46.000000 CreateAI-0.9.3/CreateAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:34:46.000000 CreateAI-0.9.3/CreateAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-08 12:34:46.000000 CreateAI-0.9.3/CreateAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1097 2023-05-05 14:50:25.000000 CreateAI-0.9.3/LICENCE
+-rw-rw-rw-   0        0        0       48 2023-05-08 12:34:46.000000 CreateAI-0.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2244 2023-05-08 12:34:46.996062 CreateAI-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1799 2023-05-08 12:26:30.000000 CreateAI-0.9.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:34:46.997062 CreateAI-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-05-08 12:34:46.000000 CreateAI-0.9.3/setup.py
```

### Comparing `CreateAI-0.8.2/CreateAI.egg-info/PKG-INFO` & `CreateAI-0.9.3/CreateAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CreateAI
-Version: 0.8.2
+Version: 0.9.3
 Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CreateAI-0.8.2/LICENCE` & `CreateAI-0.9.3/LICENCE`

 * *Files identical despite different names*

### Comparing `CreateAI-0.8.2/PKG-INFO` & `CreateAI-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CreateAI
-Version: 0.8.2
+Version: 0.9.3
 Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CreateAI-0.8.2/README.md` & `CreateAI-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `CreateAI-0.8.2/setup.py` & `CreateAI-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open(r'C:\MyUse\code\python\EasyPack\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='CreateAI',
-	version='0.8.2',
+	version='0.9.3',
 	author='R0fael',
 	author_email='roslobodchikov@gmail.com',
 	description='Easy tool for creating AI in python',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/R0fael/CreateAI',
 	packages=['C:\MyUse\code\python\EasyPack\CreateAI'],
```

