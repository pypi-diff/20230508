# Comparing `tmp/clubscore-0.1.2.tar.gz` & `tmp/clubscore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clubscore-0.1.2.tar", last modified: Sat May  6 09:47:48 2023, max compression
+gzip compressed data, was "dist/clubscore-0.1.3.tar", last modified: Mon May  8 11:59:06 2023, max compression
```

## Comparing `clubscore-0.1.2.tar` & `clubscore-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:47:48.000000 clubscore-0.1.2/
--rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.2/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-06 09:47:48.000000 clubscore-0.1.2/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.1.2/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore/
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.2/clubscore/__init__.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore/objects/
--rw-r--r--   0 dave       (501) staff       (20)     4792 2023-05-06 08:35:20.000000 clubscore-0.1.2/clubscore/objects/CONTAINER.py
--rw-r--r--   0 dave       (501) staff       (20)     2204 2023-05-06 08:35:20.000000 clubscore-0.1.2/clubscore/objects/IMG.py
--rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.1.2/clubscore/objects/RECTANGLE.py
--rw-r--r--   0 dave       (501) staff       (20)     3899 2023-05-06 08:35:20.000000 clubscore-0.1.2/clubscore/objects/TEXT.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.2/clubscore/objects/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     3209 2023-04-06 23:23:45.000000 clubscore-0.1.2/clubscore/utils.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      374 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-06 09:47:48.000000 clubscore-0.1.2/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-06 09:41:10.000000 clubscore-0.1.2/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 11:59:06.000000 clubscore-0.1.3/
+-rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.3/LICENSE
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-08 11:59:06.000000 clubscore-0.1.3/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.1.3/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 11:59:06.000000 clubscore-0.1.3/clubscore/
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.3/clubscore/__init__.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 11:59:06.000000 clubscore-0.1.3/clubscore/objects/
+-rw-r--r--   0 dave       (501) staff       (20)     4792 2023-05-06 08:35:20.000000 clubscore-0.1.3/clubscore/objects/CONTAINER.py
+-rw-r--r--   0 dave       (501) staff       (20)     2204 2023-05-06 08:35:20.000000 clubscore-0.1.3/clubscore/objects/IMG.py
+-rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.1.3/clubscore/objects/RECTANGLE.py
+-rw-r--r--   0 dave       (501) staff       (20)     3926 2023-05-08 11:56:58.000000 clubscore-0.1.3/clubscore/objects/TEXT.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.3/clubscore/objects/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     3332 2023-05-06 21:57:49.000000 clubscore-0.1.3/clubscore/utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 11:59:06.000000 clubscore-0.1.3/clubscore.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-08 11:59:06.000000 clubscore-0.1.3/clubscore.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      394 2023-05-08 11:59:06.000000 clubscore-0.1.3/clubscore.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-08 11:59:06.000000 clubscore-0.1.3/clubscore.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-08 11:59:06.000000 clubscore-0.1.3/clubscore.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-08 11:59:06.000000 clubscore-0.1.3/clubscore.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-08 11:59:06.000000 clubscore-0.1.3/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-08 11:58:04.000000 clubscore-0.1.3/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 11:59:06.000000 clubscore-0.1.3/tests/
+-rw-r--r--   0 dave       (501) staff       (20)     1353 2023-05-07 10:14:30.000000 clubscore-0.1.3/tests/test_utils.py
```

### Comparing `clubscore-0.1.2/LICENSE` & `clubscore-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.2/PKG-INFO` & `clubscore-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.1.2/clubscore/objects/CONTAINER.py` & `clubscore-0.1.3/clubscore/objects/CONTAINER.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.2/clubscore/objects/IMG.py` & `clubscore-0.1.3/clubscore/objects/IMG.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.2/clubscore/objects/RECTANGLE.py` & `clubscore-0.1.3/clubscore/objects/RECTANGLE.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.2/clubscore/objects/TEXT.py` & `clubscore-0.1.3/clubscore/objects/TEXT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from PIL import ImageDraw, ImageFont
-from clubscore import utils as u
-
+from PIL import Image, ImageDraw, ImageFont
+import utils as u
 
 class TEXT:
 
     """
     image: immagine di background di riferimento
     test: testo da scrivere
     font_path: font di riferimento  da utilizzare (fornire path)
@@ -61,25 +60,26 @@
 
     """
     costruttore a partire da dizionario XML dell'oggetto
     """
     @staticmethod
     def initiate(image, root, dict, lines):
 
-        if "testo" in dict and "*" in dict["testo"]:
+        if "testo" in dict:
+            if "*" in dict["testo"]:
 
-            testo = lines.pop(0).strip()
+                testo = lines.pop(0).strip()
 
-            if "match_word" in dict and "True" in dict["match_word"]:
-                testo = u.matchWord(testo, u.getTeams("graphics/teams/squadre.txt"))
+                if "match_word" in dict and "True" in dict["match_word"]:
+                    testo = u.matchWord(testo, u.getTeams("graphics/teams/squadre.txt"))
 
-            if "upper" in dict and "True" in dict["upper"]:
-                testo = testo.upper()
+                if "upper" in dict and "True" in dict["upper"]:
+                    testo = testo.upper()
 
-            dict["testo"] = dict["testo"].replace("*", testo)
+                dict["testo"] = dict["testo"].replace("*", testo)
 
             final_text = dict["testo"]
 
         elif "concatenation" in dict:
             print("concatenation", lines)
             for i in range(len(lines)):
                 repl = "{%s}" % str(i)
```

### Comparing `clubscore-0.1.2/clubscore/utils.py` & `clubscore-0.1.3/clubscore/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from PIL import Image, ImageDraw, ImageFont
 import xml.etree.ElementTree as ET
 import difflib
 import os
 import requests
+import logging
 from bs4 import BeautifulSoup
 
+
+# set the logging level (e.g. DEBUG, INFO, WARNING, ERROR)
+logging.basicConfig(level=logging.INFO)
+
 """
 Prende un file in formato PNG e lo colora completamente di
 un colore specifico in rgb.
 Colore di default è bianco
 """
 
 
@@ -82,15 +87,15 @@
     arr = [x.lower() for x in arr]
     s = s.lower()
 
     match = difflib.get_close_matches(s, arr, n=1, cutoff=0.3)
     if match:
         return match[0]
     else:
-        print("non ho trovato")
+        logging.INFO("Non ho trovato")
         raise Exception("Non ho trovato una squadra")
 
 
 """
 Recupera la lista delle squadre di cui si hanno le grafiche
 """
```

### Comparing `clubscore-0.1.2/clubscore.egg-info/PKG-INFO` & `clubscore-0.1.3/clubscore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.1.2/setup.py` & `clubscore-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clubscore',
-    version='0.1.2',
+    version='0.1.3',
     author='Davide Gimondo',
     author_email='davegimo@gmail.com',
     description='A package for creating customizable templates in XML',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davegimo/clubscore',
     packages=find_packages(),
```

