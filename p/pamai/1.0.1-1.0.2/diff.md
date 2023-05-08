# Comparing `tmp/pamai-1.0.1.tar.gz` & `tmp/pamai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pamai-1.0.1.tar", last modified: Mon May  8 12:19:24 2023, max compression
+gzip compressed data, was "pamai-1.0.2.tar", last modified: Mon May  8 12:25:59 2023, max compression
```

## Comparing `pamai-1.0.1.tar` & `pamai-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:19:24.483700 pamai-1.0.1/
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     1082 2023-05-08 12:08:14.000000 pamai-1.0.1/LICENSE.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       99 2023-05-08 12:06:00.000000 pamai-1.0.1/MANIFEST.in
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     9420 2023-05-08 12:19:24.483971 pamai-1.0.1/PKG-INFO
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     8509 2023-05-08 12:16:21.000000 pamai-1.0.1/README.md
-drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:19:24.481207 pamai-1.0.1/pamai/
--rw-r--r--   0 chrisrauch193   (501) staff       (20)      103 2023-05-08 12:04:24.000000 pamai-1.0.1/pamai/__init__.py
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       21 2023-05-08 12:18:54.000000 pamai-1.0.1/pamai/version.py
-drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:19:24.483201 pamai-1.0.1/pamai.egg-info/
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     9420 2023-05-08 12:19:24.000000 pamai-1.0.1/pamai.egg-info/PKG-INFO
--rw-r--r--   0 chrisrauch193   (501) staff       (20)      246 2023-05-08 12:19:24.000000 pamai-1.0.1/pamai.egg-info/SOURCES.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)        1 2023-05-08 12:19:24.000000 pamai-1.0.1/pamai.egg-info/dependency_links.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)      323 2023-05-08 12:19:24.000000 pamai-1.0.1/pamai.egg-info/requires.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)        6 2023-05-08 12:19:24.000000 pamai-1.0.1/pamai.egg-info/top_level.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       76 2023-05-08 11:50:53.000000 pamai-1.0.1/pyproject.toml
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     1309 2023-05-08 12:19:24.485431 pamai-1.0.1/setup.cfg
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       97 2023-05-08 12:09:39.000000 pamai-1.0.1/setup.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:25:59.250713 pamai-1.0.2/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1082 2023-05-08 12:08:14.000000 pamai-1.0.2/LICENSE.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       99 2023-05-08 12:06:00.000000 pamai-1.0.2/MANIFEST.in
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-08 12:25:59.250936 pamai-1.0.2/PKG-INFO
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     8509 2023-05-08 12:16:21.000000 pamai-1.0.2/README.md
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:25:59.248526 pamai-1.0.2/pamai/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      103 2023-05-08 12:04:24.000000 pamai-1.0.2/pamai/__init__.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       21 2023-05-08 12:25:44.000000 pamai-1.0.2/pamai/version.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:25:59.250423 pamai-1.0.2/pamai.egg-info/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/PKG-INFO
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      246 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        1 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      323 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/requires.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        6 2023-05-08 12:25:59.000000 pamai-1.0.2/pamai.egg-info/top_level.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       76 2023-05-08 11:50:53.000000 pamai-1.0.2/pyproject.toml
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1158 2023-05-08 12:25:59.252589 pamai-1.0.2/setup.cfg
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       97 2023-05-08 12:09:39.000000 pamai-1.0.2/setup.py
```

### Comparing `pamai-1.0.1/LICENSE.txt` & `pamai-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pamai-1.0.1/PKG-INFO` & `pamai-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: pamai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for PAMAI written by Arthur Zucker and Chris Rauch.
 Home-page: https://github.com/ArthurZucker/PAMAI
-Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.2.tar.gz
 Author: Chris Rauch
 Author-email: chrisrauch193@gmail.com
 License: MIT
 Keywords: pamai,ai,audio,denet,arthur,zucker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: ==3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![wakatime](https://wakatime.com/badge/user/57d887d6-525a-4214-a78c-21863f2f88f7/project/93d14295-7eb1-438b-b391-744be6d71661.svg)](https://wakatime.com/badge/user/57d887d6-525a-4214-a78c-21863f2f88f7/project/93d14295-7eb1-438b-b391-744be6d71661)
 # DENet training code 
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pamai-1.0.1/README.md` & `pamai-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pamai-1.0.1/pamai.egg-info/PKG-INFO` & `pamai-1.0.2/pamai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: pamai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for PAMAI written by Arthur Zucker and Chris Rauch.
 Home-page: https://github.com/ArthurZucker/PAMAI
-Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.2.tar.gz
 Author: Chris Rauch
 Author-email: chrisrauch193@gmail.com
 License: MIT
 Keywords: pamai,ai,audio,denet,arthur,zucker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: ==3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![wakatime](https://wakatime.com/badge/user/57d887d6-525a-4214-a78c-21863f2f88f7/project/93d14295-7eb1-438b-b391-744be6d71661.svg)](https://wakatime.com/badge/user/57d887d6-525a-4214-a78c-21863f2f88f7/project/93d14295-7eb1-438b-b391-744be6d71661)
 # DENet training code 
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pamai-1.0.1/setup.cfg` & `pamai-1.0.2/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -4,27 +4,23 @@
 author = Chris Rauch
 author_email = chrisrauch193@gmail.com
 keywords = pamai, ai, audio, denet, arthur, zucker
 description = Package for PAMAI written by Arthur Zucker and Chris Rauch.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ArthurZucker/PAMAI
-download_url = https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.1.tar.gz
+download_url = https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.2.tar.gz
 license = MIT
 license_files = LICENSE.txt
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Topic :: Software Development :: Build Tools
 	License :: OSI Approved :: MIT License
-	Programming Language :: Python
 	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
 
 [options]
 install_requires = 
 	PyAudio==0.2.13
 	pybind11==2.10.4
 	Cython==0.29.34
 	numpy==1.23.5
@@ -40,13 +36,13 @@
 	scikit-learn==1.2.2
 	scipy==1.10.1
 	simple-parsing==0.1.2
 	torch==2.0.0
 	torchaudio==2.0.1
 	tqdm==4.65.0
 	wandb==0.15.0
-python_requires = >=3.8
+python_requires = ==3.8
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

