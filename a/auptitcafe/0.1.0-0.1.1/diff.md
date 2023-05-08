# Comparing `tmp/auptitcafe-0.1.0.tar.gz` & `tmp/auptitcafe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auptitcafe-0.1.0.tar", max compression
+gzip compressed data, was "auptitcafe-0.1.1.tar", max compression
```

## Comparing `auptitcafe-0.1.0.tar` & `auptitcafe-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-06 07:28:28.056511 auptitcafe-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-06 07:28:28.056511 auptitcafe-0.1.0/auptitcafe/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-07 02:53:30.216593 auptitcafe-0.1.0/auptitcafe/menus.py
--rw-r--r--   0        0        0      279 2023-05-07 02:53:08.994686 auptitcafe-0.1.0/auptitcafe/plat.py
--rw-r--r--   0        0        0      402 2023-05-07 02:03:08.636590 auptitcafe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 auptitcafe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-05-07 09:18:31.419815 auptitcafe-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 09:19:13.604766 auptitcafe-0.1.1/auptitcafe/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-08 01:33:58.893072 auptitcafe-0.1.1/auptitcafe/menus.py
+-rw-r--r--   0        0        0      280 2023-05-08 01:32:24.031863 auptitcafe-0.1.1/auptitcafe/plat.py
+-rw-r--r--   0        0        0      441 2023-05-08 01:34:50.885782 auptitcafe-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 auptitcafe-0.1.1/PKG-INFO
```

### Comparing `auptitcafe-0.1.0/auptitcafe/menus.py` & `auptitcafe-0.1.1/auptitcafe/menus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import re
 import requests
+import pandas as pd
+
 from bs4 import BeautifulSoup
 
 from auptitcafe.plat import Plat
 
 class Menus:
     def __init__(self):
         self.menus_url = "http://auptitcafe.nc/menu/"
@@ -42,8 +44,14 @@
                         price = prix,
                         cat = category,
                         details = recette,
                         img_url = image)
             print("================================================================")
             out.append(plat)
         return out
+
+    def get_all_as_df(self):
+        df = pd.DataFrame.from_records([plat.to_dict() for plat in Menus.get_all(self)])
+        df
+        return df
+
```

