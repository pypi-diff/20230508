# Comparing `tmp/yeref-0.1.57.tar.gz` & `tmp/yeref-0.1.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.57.tar", last modified: Mon May  8 10:57:19 2023, max compression
+gzip compressed data, was "yeref-0.1.58.tar", last modified: Mon May  8 11:57:34 2023, max compression
```

## Comparing `yeref-0.1.57.tar` & `yeref-0.1.58.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 10:57:19.553101 yeref-0.1.57/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 10:57:19.553365 yeref-0.1.57/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-08 10:57:19.554601 yeref-0.1.57/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-08 10:57:07.000000 yeref-0.1.57/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 10:57:19.547007 yeref-0.1.57/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.57/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   508331 2023-05-07 13:42:35.000000 yeref-0.1.57/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   198722 2023-05-08 10:48:49.000000 yeref-0.1.57/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 10:57:19.552324 yeref-0.1.57/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 10:57:19.000000 yeref-0.1.57/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-08 10:57:19.000000 yeref-0.1.57/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-08 10:57:19.000000 yeref-0.1.57/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-08 10:57:19.000000 yeref-0.1.57/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 11:57:34.528570 yeref-0.1.58/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 11:57:34.528793 yeref-0.1.58/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-08 11:57:34.529463 yeref-0.1.58/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-08 11:57:19.000000 yeref-0.1.58/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 11:57:34.522898 yeref-0.1.58/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.58/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   508331 2023-05-08 11:56:43.000000 yeref-0.1.58/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   198722 2023-05-08 10:48:49.000000 yeref-0.1.58/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 11:57:34.528005 yeref-0.1.58/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 11:57:34.000000 yeref-0.1.58/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-08 11:57:34.000000 yeref-0.1.58/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-08 11:57:34.000000 yeref-0.1.58/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-08 11:57:34.000000 yeref-0.1.58/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.57/setup.py` & `yeref-0.1.58/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.57',
+      version='0.1.58',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,15 +39,15 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.57-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.58-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.57/yeref/l_.py` & `yeref-0.1.58/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.57/yeref/yeref.py` & `yeref-0.1.58/yeref/yeref.py`

 * *Files identical despite different names*

