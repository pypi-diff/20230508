# Comparing `tmp/proventosweb-0.4.tar.gz` & `tmp/proventosweb-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.4.tar", last modified: Mon May  8 12:55:04 2023, max compression
+gzip compressed data, was "proventosweb-0.5.tar", last modified: Mon May  8 13:12:33 2023, max compression
```

## Comparing `proventosweb-0.4.tar` & `proventosweb-0.5.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 12:55:04.964903 proventosweb-0.4/
--rw-rw-rw-   0        0        0      314 2023-05-08 12:55:04.964903 proventosweb-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 12:55:04.964903 proventosweb-0.4/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      314 2023-05-08 12:55:04.000000 proventosweb-0.4/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-08 12:55:04.000000 proventosweb-0.4/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 12:55:04.000000 proventosweb-0.4/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.4/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-08 12:55:04.000000 proventosweb-0.4/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 12:55:04.000000 proventosweb-0.4/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 12:55:04.964903 proventosweb-0.4/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-05-08 12:52:05.000000 proventosweb-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:12:33.031374 proventosweb-0.5/
+-rw-rw-rw-   0        0        0      314 2023-05-08 13:12:33.031374 proventosweb-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 13:12:32.993971 proventosweb-0.5/proventosweb/
+-rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.5/proventosweb/__init__.py
+-rw-rw-rw-   0        0        0    11029 2023-05-08 12:51:57.000000 proventosweb-0.5/proventosweb/proventosweb.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:12:33.031374 proventosweb-0.5/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      314 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.5/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:12:33.031374 proventosweb-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-05-08 13:01:52.000000 proventosweb-0.5/setup.py
```

### Comparing `proventosweb-0.4/setup.py` & `proventosweb-0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='proventosweb',
-      version='0.4',
+      version='0.5',
       description='Uma biblioteca para buscar proventos de ações na plataforma Status Invest',
       url='https://github.com/rafaelpsampaio/proventosweb',
       author='Rafael Sampaio',
       author_email='rafapsampaio@gmail.com',
       packages=['proventosweb'],
       install_requires=[
           'pandas',
```

