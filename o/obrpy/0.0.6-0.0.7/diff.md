# Comparing `tmp/obrpy-0.0.6.tar.gz` & `tmp/obrpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obrpy-0.0.6.tar", last modified: Thu Feb 23 12:43:04 2023, max compression
+gzip compressed data, was "obrpy-0.0.7.tar", last modified: Mon May  8 16:22:43 2023, max compression
```

## Comparing `obrpy-0.0.6.tar` & `obrpy-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 12:43:04.536464 obrpy-0.0.6/
--rw-rw-rw-   0        0        0      283 2023-02-23 12:43:04.536464 obrpy-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-23 12:43:04.524463 obrpy-0.0.6/obrpy/
--rw-rw-rw-   0        0        0     1341 2023-02-23 12:03:19.000000 obrpy-0.0.6/obrpy/PathSelector.py
--rw-rw-rw-   0        0        0     3112 2023-02-23 12:42:48.000000 obrpy-0.0.6/obrpy/__init__.py
--rw-rw-rw-   0        0        0      420 2023-02-23 12:35:18.000000 obrpy-0.0.6/obrpy/load.py
--rw-rw-rw-   0        0        0      928 2023-02-23 12:35:04.000000 obrpy-0.0.6/obrpy/save.py
-drwxrwxrwx   0        0        0        0 2023-02-23 12:43:04.534464 obrpy-0.0.6/obrpy.egg-info/
--rw-rw-rw-   0        0        0      283 2023-02-23 12:43:04.000000 obrpy-0.0.6/obrpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-02-23 12:43:04.000000 obrpy-0.0.6/obrpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 12:43:04.000000 obrpy-0.0.6/obrpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-02-23 12:43:04.000000 obrpy-0.0.6/obrpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-23 12:43:04.000000 obrpy-0.0.6/obrpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-23 12:43:04.536464 obrpy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-02-23 12:42:59.000000 obrpy-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-23 12:43:04.535465 obrpy-0.0.6/test/
--rw-rw-rw-   0        0        0      171 2023-02-23 12:35:33.000000 obrpy-0.0.6/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:22:43.881211 obrpy-0.0.7/
+-rw-rw-rw-   0        0        0      283 2023-05-08 16:22:43.881211 obrpy-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 16:22:43.854033 obrpy-0.0.7/obrpy/
+-rw-rw-rw-   0        0        0     1341 2023-02-23 12:03:19.000000 obrpy-0.0.7/obrpy/PathSelector.py
+-rw-rw-rw-   0        0        0     5304 2023-05-04 14:08:11.000000 obrpy-0.0.7/obrpy/__init__.py
+-rw-rw-rw-   0        0        0     2022 2023-05-03 10:35:47.000000 obrpy-0.0.7/obrpy/load.py
+-rw-rw-rw-   0        0        0     8391 2023-04-26 14:25:18.000000 obrpy-0.0.7/obrpy/obr.py
+-rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.0.7/obrpy/obrsdk.py
+-rw-rw-rw-   0        0        0     2663 2023-04-26 14:11:20.000000 obrpy-0.0.7/obrpy/save.py
+-rw-rw-rw-   0        0        0     3729 2023-04-26 15:09:07.000000 obrpy-0.0.7/obrpy/settings.py
+-rw-rw-rw-   0        0        0     3425 2023-05-03 08:58:35.000000 obrpy-0.0.7/obrpy/take_a_look.py
+-rw-rw-rw-   0        0        0     1930 2023-04-26 12:15:31.000000 obrpy-0.0.7/obrpy/update.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:22:43.874187 obrpy-0.0.7/obrpy.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:22:43.881211 obrpy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-05-08 16:19:00.000000 obrpy-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:22:43.880217 obrpy-0.0.7/test/
+-rw-rw-rw-   0        0        0      697 2023-05-04 15:23:53.000000 obrpy-0.0.7/test/test.py
```

### Comparing `obrpy-0.0.6/obrpy/PathSelector.py` & `obrpy-0.0.7/obrpy/PathSelector.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.6/setup.py` & `obrpy-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.6' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.0.7' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'obrpy' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Andres Pedraza Rodriguez' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'a.pedraza@upm.es' #Modificar con vuestros datos
 URL = 'https://github.com/temisAP' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = "This library is aimed for using Luna's OBR-4600 with Python." #Descripción corta
```

