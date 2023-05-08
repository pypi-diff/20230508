# Comparing `tmp/embeddings-util-1.0.0.tar.gz` & `tmp/embeddings-util-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embeddings-util-1.0.0.tar", last modified: Mon May  8 10:49:56 2023, max compression
+gzip compressed data, was "embeddings-util-1.0.1.tar", last modified: Mon May  8 11:01:59 2023, max compression
```

## Comparing `embeddings-util-1.0.0.tar` & `embeddings-util-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-08 10:49:56.928036 embeddings-util-1.0.0/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1081 2023-05-08 09:39:13.000000 embeddings-util-1.0.0/LICENSE.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7532 2023-05-08 10:49:56.928036 embeddings-util-1.0.0/PKG-INFO
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6469 2023-05-08 10:49:18.000000 embeddings-util-1.0.0/README.md
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-08 10:49:56.928036 embeddings-util-1.0.0/embeddings_util/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       43 2023-05-08 10:47:57.000000 embeddings-util-1.0.0/embeddings_util/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6080 2023-05-08 10:47:43.000000 embeddings-util-1.0.0/embeddings_util/embeddings_util.py
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-08 10:49:56.928036 embeddings-util-1.0.0/embeddings_util.egg-info/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7532 2023-05-08 10:49:56.000000 embeddings-util-1.0.0/embeddings_util.egg-info/PKG-INFO
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      287 2023-05-08 10:49:56.000000 embeddings-util-1.0.0/embeddings_util.egg-info/SOURCES.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        1 2023-05-08 10:49:56.000000 embeddings-util-1.0.0/embeddings_util.egg-info/dependency_links.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       36 2023-05-08 10:49:56.000000 embeddings-util-1.0.0/embeddings_util.egg-info/requires.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       16 2023-05-08 10:49:56.000000 embeddings-util-1.0.0/embeddings_util.egg-info/top_level.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       38 2023-05-08 10:49:56.928036 embeddings-util-1.0.0/setup.cfg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1397 2023-05-08 10:36:34.000000 embeddings-util-1.0.0/setup.py
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-08 11:01:59.235618 embeddings-util-1.0.1/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1081 2023-05-08 09:39:13.000000 embeddings-util-1.0.1/LICENSE.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7532 2023-05-08 11:01:59.235618 embeddings-util-1.0.1/PKG-INFO
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6469 2023-05-08 10:49:18.000000 embeddings-util-1.0.1/README.md
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-08 11:01:59.235618 embeddings-util-1.0.1/embeddings_util/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       43 2023-05-08 10:47:57.000000 embeddings-util-1.0.1/embeddings_util/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6080 2023-05-08 10:47:43.000000 embeddings-util-1.0.1/embeddings_util/embeddings_util.py
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-08 11:01:59.235618 embeddings-util-1.0.1/embeddings_util.egg-info/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7532 2023-05-08 11:01:58.000000 embeddings-util-1.0.1/embeddings_util.egg-info/PKG-INFO
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      287 2023-05-08 11:01:59.000000 embeddings-util-1.0.1/embeddings_util.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)        1 2023-05-08 11:01:58.000000 embeddings-util-1.0.1/embeddings_util.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       36 2023-05-08 11:01:59.000000 embeddings-util-1.0.1/embeddings_util.egg-info/requires.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       16 2023-05-08 11:01:59.000000 embeddings-util-1.0.1/embeddings_util.egg-info/top_level.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       38 2023-05-08 11:01:59.235618 embeddings-util-1.0.1/setup.cfg
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1397 2023-05-08 11:00:50.000000 embeddings-util-1.0.1/setup.py
```

### Comparing `embeddings-util-1.0.0/LICENSE.txt` & `embeddings-util-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `embeddings-util-1.0.0/PKG-INFO` & `embeddings-util-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embeddings-util
-Version: 1.0.0
+Version: 1.0.1
 Summary: The embeddings package is a utility for generating question-answer pairs and embeddings from HTML pages or text input. It utilizes the OpenAI API to generate question-answer pairs and embeddings. This package is useful for generating training data for chatbots or question-answering models.
 Home-page: https://github.com/ChatClue/embedding-python
 Author: Osiris Development LLC
 Author-email: support@pagepixels.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `embeddings-util-1.0.0/README.md` & `embeddings-util-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `embeddings-util-1.0.0/embeddings_util/embeddings_util.py` & `embeddings-util-1.0.1/embeddings_util/embeddings_util.py`

 * *Files identical despite different names*

### Comparing `embeddings-util-1.0.0/embeddings_util.egg-info/PKG-INFO` & `embeddings-util-1.0.1/embeddings_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embeddings-util
-Version: 1.0.0
+Version: 1.0.1
 Summary: The embeddings package is a utility for generating question-answer pairs and embeddings from HTML pages or text input. It utilizes the OpenAI API to generate question-answer pairs and embeddings. This package is useful for generating training data for chatbots or question-answering models.
 Home-page: https://github.com/ChatClue/embedding-python
 Author: Osiris Development LLC
 Author-email: support@pagepixels.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `embeddings-util-1.0.0/setup.py` & `embeddings-util-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of the README.md file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='embeddings-util',
-    version='1.0.0',
+    version='1.0.1',
     description='The embeddings package is a utility for generating question-answer pairs and embeddings from HTML pages or text input. It utilizes the OpenAI API to generate question-answer pairs and embeddings. This package is useful for generating training data for chatbots or question-answering models.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Osiris Development LLC',
     author_email='support@pagepixels.com',
     url='https://github.com/ChatClue/embedding-python',
     packages=find_packages(),
```

