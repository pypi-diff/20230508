# Comparing `tmp/pamai-1.0.2.tar.gz` & `tmp/pamai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pamai-1.0.2.tar", last modified: Mon May  8 12:25:59 2023, max compression
+gzip compressed data, was "pamai-1.0.3.tar", last modified: Mon May  8 12:47:46 2023, max compression
```

## Comparing `pamai-1.0.2.tar` & `pamai-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:25:59.250713 pamai-1.0.2/
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     1082 2023-05-08 12:08:14.000000 pamai-1.0.2/LICENSE.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       99 2023-05-08 12:06:00.000000 pamai-1.0.2/MANIFEST.in
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-08 12:25:59.250936 pamai-1.0.2/PKG-INFO
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     8509 2023-05-08 12:16:21.000000 pamai-1.0.2/README.md
-drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:25:59.248526 pamai-1.0.2/pamai/
--rw-r--r--   0 chrisrauch193   (501) staff       (20)      103 2023-05-08 12:04:24.000000 pamai-1.0.2/pamai/__init__.py
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       21 2023-05-08 12:25:44.000000 pamai-1.0.2/pamai/version.py
-drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:25:59.250423 pamai-1.0.2/pamai.egg-info/
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/PKG-INFO
--rw-r--r--   0 chrisrauch193   (501) staff       (20)      246 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/SOURCES.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)        1 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/dependency_links.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)      323 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/requires.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)        6 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/top_level.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       76 2023-05-08 11:50:53.000000 pamai-1.0.2/pyproject.toml
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     1158 2023-05-08 12:25:59.252589 pamai-1.0.2/setup.cfg
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       97 2023-05-08 12:09:39.000000 pamai-1.0.2/setup.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:47:46.591180 pamai-1.0.3/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1082 2023-05-08 12:08:14.000000 pamai-1.0.3/LICENSE.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       99 2023-05-08 12:06:00.000000 pamai-1.0.3/MANIFEST.in
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-08 12:47:46.591877 pamai-1.0.3/PKG-INFO
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     8509 2023-05-08 12:16:21.000000 pamai-1.0.3/README.md
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:47:46.586347 pamai-1.0.3/pamai/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      103 2023-05-08 12:04:24.000000 pamai-1.0.3/pamai/__init__.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       21 2023-05-08 12:47:24.000000 pamai-1.0.3/pamai/version.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:47:46.590656 pamai-1.0.3/pamai.egg-info/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/PKG-INFO
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      246 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        1 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      323 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/requires.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        6 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/top_level.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       76 2023-05-08 11:50:53.000000 pamai-1.0.3/pyproject.toml
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1158 2023-05-08 12:47:46.595519 pamai-1.0.3/setup.cfg
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       97 2023-05-08 12:09:39.000000 pamai-1.0.3/setup.py
```

### Comparing `pamai-1.0.2/LICENSE.txt` & `pamai-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pamai-1.0.2/PKG-INFO` & `pamai-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pamai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for PAMAI written by Arthur Zucker and Chris Rauch.
 Home-page: https://github.com/ArthurZucker/PAMAI
-Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.2.tar.gz
+Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.3.tar.gz
 Author: Chris Rauch
 Author-email: chrisrauch193@gmail.com
 License: MIT
 Keywords: pamai,ai,audio,denet,arthur,zucker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pamai-1.0.2/README.md` & `pamai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pamai-1.0.2/pamai.egg-info/PKG-INFO` & `pamai-1.0.3/pamai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pamai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for PAMAI written by Arthur Zucker and Chris Rauch.
 Home-page: https://github.com/ArthurZucker/PAMAI
-Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.2.tar.gz
+Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.3.tar.gz
 Author: Chris Rauch
 Author-email: chrisrauch193@gmail.com
 License: MIT
 Keywords: pamai,ai,audio,denet,arthur,zucker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pamai-1.0.2/setup.cfg` & `pamai-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = Chris Rauch
 author_email = chrisrauch193@gmail.com
 keywords = pamai, ai, audio, denet, arthur, zucker
 description = Package for PAMAI written by Arthur Zucker and Chris Rauch.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ArthurZucker/PAMAI
-download_url = https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.2.tar.gz
+download_url = https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.3.tar.gz
 license = MIT
 license_files = LICENSE.txt
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Topic :: Software Development :: Build Tools
 	License :: OSI Approved :: MIT License
```

