# Comparing `tmp/pyacmi-1.0.0.tar.gz` & `tmp/pyacmi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacmi-1.0.0.tar", last modified: Mon May  8 11:11:50 2023, max compression
+gzip compressed data, was "pyacmi-1.0.1.tar", last modified: Mon May  8 11:38:52 2023, max compression
```

## Comparing `pyacmi-1.0.0.tar` & `pyacmi-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 11:11:50.725544 pyacmi-1.0.0/
--rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 10:54:45.000000 pyacmi-1.0.0/LICENSE
--rw-r--r--   0 wangtong   (501) staff       (20)      749 2023-05-08 11:11:50.725414 pyacmi-1.0.0/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      103 2023-05-08 11:07:30.000000 pyacmi-1.0.0/README.md
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 11:11:50.724617 pyacmi-1.0.0/pyacmi/
--rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 09:42:33.000000 pyacmi-1.0.0/pyacmi/__init__.py
--rw-r--r--   0 wangtong   (501) staff       (20)    17604 2023-05-08 10:59:36.000000 pyacmi-1.0.0/pyacmi/acmi.py
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 11:11:50.725231 pyacmi-1.0.0/pyacmi.egg-info/
--rw-r--r--   0 wangtong   (501) staff       (20)      749 2023-05-08 11:11:50.000000 pyacmi-1.0.0/pyacmi.egg-info/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-08 11:11:50.000000 pyacmi-1.0.0/pyacmi.egg-info/SOURCES.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-08 11:11:50.000000 pyacmi-1.0.0/pyacmi.egg-info/dependency_links.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       17 2023-05-08 11:11:50.000000 pyacmi-1.0.0/pyacmi.egg-info/requires.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-08 11:11:50.000000 pyacmi-1.0.0/pyacmi.egg-info/top_level.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-08 11:11:50.725594 pyacmi-1.0.0/setup.cfg
--rw-r--r--   0 wangtong   (501) staff       (20)      959 2023-05-08 11:10:59.000000 pyacmi-1.0.0/setup.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 11:38:52.213270 pyacmi-1.0.1/
+-rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 10:54:45.000000 pyacmi-1.0.1/LICENSE
+-rw-r--r--   0 wangtong   (501) staff       (20)     1116 2023-05-08 11:38:52.213145 pyacmi-1.0.1/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      438 2023-05-08 11:36:11.000000 pyacmi-1.0.1/README.md
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 11:38:52.212327 pyacmi-1.0.1/pyacmi/
+-rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 09:42:33.000000 pyacmi-1.0.1/pyacmi/__init__.py
+-rw-r--r--   0 wangtong   (501) staff       (20)    17604 2023-05-08 10:59:36.000000 pyacmi-1.0.1/pyacmi/acmi.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 11:38:52.212967 pyacmi-1.0.1/pyacmi.egg-info/
+-rw-r--r--   0 wangtong   (501) staff       (20)     1116 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       17 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/requires.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/top_level.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-08 11:38:52.213315 pyacmi-1.0.1/setup.cfg
+-rw-r--r--   0 wangtong   (501) staff       (20)     1022 2023-05-08 11:38:32.000000 pyacmi-1.0.1/setup.py
```

### Comparing `pyacmi-1.0.0/LICENSE` & `pyacmi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacmi-1.0.0/pyacmi/acmi.py` & `pyacmi-1.0.1/pyacmi/acmi.py`

 * *Files identical despite different names*

### Comparing `pyacmi-1.0.0/setup.py` & `pyacmi-1.0.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from setuptools import setup
 
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
         name="pyacmi",
-        version='1.0.0',
+        version='1.0.1',
         description="ACMI flight record file parser",
-        long_description="ACMI is a file used by tacview for creating flight recording from simulators or real world.",
+        long_description=long_description,
+        long_description_content_type='text/markdown',
         url='https://github.com/wangtong2015/pyacmi',
         author="Wang Tong",
         author_email="astroboythu@gmail.com",
         license="MIT",
         classifiers=[
             'Development Status :: 3 - Alpha',
             'Topic :: Games/Entertainment :: Simulation',
```

