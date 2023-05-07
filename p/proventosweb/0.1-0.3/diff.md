# Comparing `tmp/proventosweb-0.1.tar.gz` & `tmp/proventosweb-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.1.tar", last modified: Sun May  7 22:35:26 2023, max compression
+gzip compressed data, was "proventosweb-0.3.tar", last modified: Sun May  7 22:47:52 2023, max compression
```

## Comparing `proventosweb-0.1.tar` & `proventosweb-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 22:35:26.160446 proventosweb-0.1/
--rw-rw-rw-   0        0        0      268 2023-05-07 22:35:26.153466 proventosweb-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-07 22:35:26.150473 proventosweb-0.1/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      268 2023-05-07 22:35:25.000000 proventosweb-0.1/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-07 22:35:25.000000 proventosweb-0.1/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 22:35:25.000000 proventosweb-0.1/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.1/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       40 2023-05-07 22:35:25.000000 proventosweb-0.1/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-07 22:35:25.000000 proventosweb-0.1/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 22:35:26.160446 proventosweb-0.1/setup.cfg
--rw-rw-rw-   0        0        0      539 2023-05-03 22:00:27.000000 proventosweb-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 22:47:52.840120 proventosweb-0.3/
+-rw-rw-rw-   0        0        0      264 2023-05-07 22:47:52.838126 proventosweb-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-07 22:47:52.836130 proventosweb-0.3/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-05-07 22:47:52.000000 proventosweb-0.3/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-07 22:47:52.000000 proventosweb-0.3/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 22:47:52.000000 proventosweb-0.3/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.3/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-07 22:47:52.000000 proventosweb-0.3/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 22:47:52.000000 proventosweb-0.3/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 22:47:52.840120 proventosweb-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-05-07 22:41:19.000000 proventosweb-0.3/setup.py
```

### Comparing `proventosweb-0.1/setup.py` & `proventosweb-0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import setup
 
 setup(name='proventosweb',
-      version='0.1',
+      version='0.3',
       description='Uma biblioteca para buscar proventos de ações na plataforma Status Invest',
       url='https://github.com/rafaelpsampaio/proventosweb',
       author='Rafael Sampaio',
-      author_email='rafapsampaio@gmail.com.com',
+      author_email='rafapsampaio@gmail.com',
       packages=['proventosweb'],
       install_requires=[
           'pandas',
           'datetime',
-          'json',
           'requests',
           'bs4',
           'numpy'
       ],
       zip_safe=False)
```

