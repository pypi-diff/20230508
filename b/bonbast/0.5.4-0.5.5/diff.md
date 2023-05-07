# Comparing `tmp/bonbast-0.5.4.tar.gz` & `tmp/bonbast-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonbast-0.5.4.tar", last modified: Sat Apr 15 17:25:37 2023, max compression
+gzip compressed data, was "bonbast-0.5.5.tar", last modified: Sun May  7 22:13:50 2023, max compression
```

## Comparing `bonbast-0.5.4.tar` & `bonbast-0.5.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-15 17:25:16.000000 bonbast-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-15 17:25:37.498376 bonbast-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-15 17:25:16.000000 bonbast-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-15 17:25:16.000000 bonbast-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 17:25:37.498376 bonbast-0.5.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-15 17:25:16.000000 bonbast-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.494376 bonbast-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.494376 bonbast-0.5.4/src/bonbast/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/src/bonbast/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/helpers/click_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/helpers/currency_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/src/bonbast/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/managers/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/managers/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/src/bonbast/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/gold.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/src/bonbast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.398656 bonbast-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-07 22:13:18.000000 bonbast-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-05-07 22:13:50.398656 bonbast-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-07 22:13:18.000000 bonbast-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-07 22:13:18.000000 bonbast-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 22:13:50.398656 bonbast-0.5.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-07 22:13:18.000000 bonbast-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.382656 bonbast-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.390656 bonbast-0.5.5/src/bonbast/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.394656 bonbast-0.5.5/src/bonbast/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/helpers/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/helpers/currency_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.394656 bonbast-0.5.5/src/bonbast/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/managers/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/managers/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.398656 bonbast-0.5.5/src/bonbast/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/gold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.390656 bonbast-0.5.5/src/bonbast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/top_level.txt
```

### Comparing `bonbast-0.5.4/LICENSE` & `bonbast-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/PKG-INFO` & `bonbast-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonbast
-Version: 0.5.4
+Version: 0.5.5
 Summary: Get currencies exchange rates for IRR from Bonbast.com
 Author-email: Amir Hossein SamadiPour <samadipoor2@gmail.com>, Alireza Azadi <alireza_azadi@hotmail.com>, Iliya Aghamajidi <dozheiny@gmail.com>, Parsa Shahmaleki <parsampsh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Amir Hossein SamadiPour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bonbast-0.5.4/README.md` & `bonbast-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/pyproject.toml` & `bonbast-0.5.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bonbast"
-version = "0.5.4"
+version = "0.5.5"
 description = "Get currencies exchange rates for IRR from Bonbast.com"
 readme = "README.md"
 authors = [
     { name = "Amir Hossein SamadiPour", email = "samadipoor2@gmail.com" },
     { name = "Alireza Azadi", email = "alireza_azadi@hotmail.com" },
     { name = "Iliya Aghamajidi", email = "dozheiny@gmail.com" },
     { name = "Parsa Shahmaleki", email = "parsampsh@gmail.com" },
@@ -37,15 +37,15 @@
 
 [project.urls]
 repository = "https://github.com/SamadiPour/bonbast"
 #documentation = ""
 
 
 [tool.bumpver]
-current_version = "0.5.4"
+current_version = "0.5.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `bonbast-0.5.4/src/bonbast/helpers/click_callbacks.py` & `bonbast-0.5.5/src/bonbast/helpers/click_callbacks.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast/helpers/currency_flags.py` & `bonbast-0.5.5/src/bonbast/helpers/currency_flags.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast/helpers/utils.py` & `bonbast-0.5.5/src/bonbast/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast/main.py` & `bonbast-0.5.5/src/bonbast/main.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast/managers/storage_manager.py` & `bonbast-0.5.5/src/bonbast/managers/storage_manager.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast/managers/token_manager.py` & `bonbast-0.5.5/src/bonbast/managers/token_manager.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast/models/coin.py` & `bonbast-0.5.5/src/bonbast/models/coin.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast/models/currency.py` & `bonbast-0.5.5/src/bonbast/models/currency.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast/models/gold.py` & `bonbast-0.5.5/src/bonbast/models/gold.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,35 @@
 
 class Gold:
     """ Gold model
     """
     VALUES = {
         'mithqal': 'Gold Mithqal',
         'gol18': 'Gold Gram',
+        'ounce': 'Ounce',
+        'bitcoin': 'Bitcoin',
     }
 
     def __init__(self, code: str, name: str, price: float):
         self.code = code
         self.name = name
         self.price = price
 
     @property
+    def price(self):
+        if self.code in ['mithqal', 'gol18']:
+            return int(self._price)
+        else:
+            return self._price
+
+    @price.setter
+    def price(self, value):
+        self._price = value
+
+    @property
     def formatted_price(self) -> str:
         return format_toman(self.price)
 
     def to_json(self) -> dict:
         return {
             self.code: {
                 'name': self.name,
```

### Comparing `bonbast-0.5.4/src/bonbast/models/token.py` & `bonbast-0.5.5/src/bonbast/models/token.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast/server.py` & `bonbast-0.5.5/src/bonbast/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             ))
 
     for gold in Gold.VALUES:
         if f'{gold}' in r:
             golds.append(Gold(
                 gold,
                 Gold.VALUES[gold],
-                price=int(r[gold])
+                price=float(r[gold])
             ))
 
     return currencies, coins, golds
 
 
 def get_graph_data(
         currency: str,
```

### Comparing `bonbast-0.5.4/src/bonbast/tables.py` & `bonbast-0.5.5/src/bonbast/tables.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.4/src/bonbast.egg-info/PKG-INFO` & `bonbast-0.5.5/src/bonbast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonbast
-Version: 0.5.4
+Version: 0.5.5
 Summary: Get currencies exchange rates for IRR from Bonbast.com
 Author-email: Amir Hossein SamadiPour <samadipoor2@gmail.com>, Alireza Azadi <alireza_azadi@hotmail.com>, Iliya Aghamajidi <dozheiny@gmail.com>, Parsa Shahmaleki <parsampsh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Amir Hossein SamadiPour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bonbast-0.5.4/src/bonbast.egg-info/SOURCES.txt` & `bonbast-0.5.5/src/bonbast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

