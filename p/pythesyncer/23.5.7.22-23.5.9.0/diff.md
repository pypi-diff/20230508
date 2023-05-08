# Comparing `tmp/pythesyncer-23.5.7.22.tar.gz` & `tmp/pythesyncer-23.5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythesyncer-23.5.7.22.tar", last modified: Sun May  7 14:16:36 2023, max compression
+gzip compressed data, was "dist/pythesyncer-23.5.9.0.tar", last modified: Mon May  8 16:56:04 2023, max compression
```

## Comparing `pythesyncer-23.5.7.22.tar` & `pythesyncer-23.5.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 14:16:36.210061 pythesyncer-23.5.7.22/
--rw-rw-r--   0 tp03      (1000) tp03      (1000)      433 2023-05-07 14:16:36.210061 pythesyncer-23.5.7.22/PKG-INFO
--rw-r--r--   0 tp03      (1000) tp03      (1000)       76 2023-04-14 11:29:59.000000 pythesyncer-23.5.7.22/README.md
-drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 14:16:36.206061 pythesyncer-23.5.7.22/pythesyncer/
--rw-r--r--   0 tp03      (1000) tp03      (1000)     3539 2023-05-07 14:04:52.000000 pythesyncer-23.5.7.22/pythesyncer/__init__.py
--rw-r--r--   0 tp03      (1000) tp03      (1000)     1469 2023-05-07 14:15:58.000000 pythesyncer-23.5.7.22/pythesyncer/auth.py
-drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 14:16:36.210061 pythesyncer-23.5.7.22/pythesyncer.egg-info/
--rw-rw-r--   0 tp03      (1000) tp03      (1000)      433 2023-05-07 14:16:36.000000 pythesyncer-23.5.7.22/pythesyncer.egg-info/PKG-INFO
--rw-rw-r--   0 tp03      (1000) tp03      (1000)      274 2023-05-07 14:16:36.000000 pythesyncer-23.5.7.22/pythesyncer.egg-info/SOURCES.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-05-07 14:16:36.000000 pythesyncer-23.5.7.22/pythesyncer.egg-info/dependency_links.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       55 2023-05-07 14:16:36.000000 pythesyncer-23.5.7.22/pythesyncer.egg-info/entry_points.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       20 2023-05-07 14:16:36.000000 pythesyncer-23.5.7.22/pythesyncer.egg-info/requires.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       12 2023-05-07 14:16:36.000000 pythesyncer-23.5.7.22/pythesyncer.egg-info/top_level.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-05-07 14:16:36.210061 pythesyncer-23.5.7.22/setup.cfg
--rw-r--r--   0 tp03      (1000) tp03      (1000)      864 2023-04-14 11:58:13.000000 pythesyncer-23.5.7.22/setup.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-08 16:56:04.007358 pythesyncer-23.5.9.0/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      432 2023-05-08 16:56:04.003358 pythesyncer-23.5.9.0/PKG-INFO
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       76 2023-04-14 11:29:59.000000 pythesyncer-23.5.9.0/README.md
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-08 16:56:03.999359 pythesyncer-23.5.9.0/pythesyncer/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3539 2023-05-07 14:04:52.000000 pythesyncer-23.5.9.0/pythesyncer/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1469 2023-05-07 14:15:58.000000 pythesyncer-23.5.9.0/pythesyncer/auth.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-08 16:56:04.003358 pythesyncer-23.5.9.0/pythesyncer.egg-info/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      432 2023-05-08 16:56:03.000000 pythesyncer-23.5.9.0/pythesyncer.egg-info/PKG-INFO
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      274 2023-05-08 16:56:03.000000 pythesyncer-23.5.9.0/pythesyncer.egg-info/SOURCES.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-05-08 16:56:03.000000 pythesyncer-23.5.9.0/pythesyncer.egg-info/dependency_links.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       55 2023-05-08 16:56:03.000000 pythesyncer-23.5.9.0/pythesyncer.egg-info/entry_points.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       41 2023-05-08 16:56:03.000000 pythesyncer-23.5.9.0/pythesyncer.egg-info/requires.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       12 2023-05-08 16:56:03.000000 pythesyncer-23.5.9.0/pythesyncer.egg-info/top_level.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-05-08 16:56:04.007358 pythesyncer-23.5.9.0/setup.cfg
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      894 2023-05-08 16:50:16.000000 pythesyncer-23.5.9.0/setup.py
```

### Comparing `pythesyncer-23.5.7.22/pythesyncer/__init__.py` & `pythesyncer-23.5.9.0/pythesyncer/__init__.py`

 * *Files identical despite different names*

### Comparing `pythesyncer-23.5.7.22/pythesyncer/auth.py` & `pythesyncer-23.5.9.0/pythesyncer/auth.py`

 * *Files identical despite different names*

### Comparing `pythesyncer-23.5.7.22/setup.py` & `pythesyncer-23.5.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     url="https://github.com/private_repo/",
     packages=setuptools.find_packages(),
     package_data={
         setuptools.find_packages()[0]: [
             "bash/*"
         ]
     },
-    install_requires=['codefast', 'fire', 'boto3'],
+    install_requires=['codefast', 'fire', 'boto3', 'rich', 'aiohttp', 'simauth'],
     entry_points={
         'console_scripts': ["pysyncer=pythesyncer.__init__:main"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

