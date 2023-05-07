# Comparing `tmp/wynntilsresolver-0.1.4.tar.gz` & `tmp/wynntilsresolver-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wynntilsresolver-0.1.4.tar", last modified: Mon May  1 18:43:52 2023, max compression
+gzip compressed data, was "wynntilsresolver-0.1.5.tar", last modified: Sun May  7 21:59:07 2023, max compression
```

## Comparing `wynntilsresolver-0.1.4.tar` & `wynntilsresolver-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      982 2023-05-01 18:24:11.966738 wynntilsresolver-0.1.4/LICENSE
--rw-r--r--   0        0        0     1292 2023-05-01 18:43:52.197703 wynntilsresolver-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1282 2023-05-01 18:26:48.182426 wynntilsresolver-0.1.4/readme.md
--rw-r--r--   0        0        0      107 2023-05-01 18:00:33.720579 wynntilsresolver-0.1.4/src/wynntilsresolver/__init__.py
--rw-r--r--   0        0        0      614 2023-05-01 18:05:04.699504 wynntilsresolver-0.1.4/src/wynntilsresolver/__main__.py
--rw-r--r--   0        0        0      105 2023-05-01 14:01:24.386186 wynntilsresolver-0.1.4/src/wynntilsresolver/exceptions.py
--rw-r--r--   0        0        0     1376 2023-05-01 18:40:18.691900 wynntilsresolver-0.1.4/src/wynntilsresolver/model.py
--rw-r--r--   0        0        0     2513 2023-05-01 18:41:17.189668 wynntilsresolver-0.1.4/src/wynntilsresolver/resolver.py
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 wynntilsresolver-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0      982 2023-05-01 18:24:11.966738 wynntilsresolver-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0     1292 2023-05-07 21:59:07.135395 wynntilsresolver-0.1.5/pyproject.toml
+-rwxr-xr-x   0        0        0     1595 2023-05-07 21:57:59.122947 wynntilsresolver-0.1.5/readme.md
+-rwxr-xr-x   0        0        0      455 2023-05-07 21:42:32.114615 wynntilsresolver-0.1.5/src/wynntilsresolver/__init__.py
+-rwxr-xr-x   0        0        0      964 2023-05-07 21:42:27.218536 wynntilsresolver-0.1.5/src/wynntilsresolver/__main__.py
+-rwxr-xr-x   0        0        0      459 2023-05-07 21:42:22.729982 wynntilsresolver-0.1.5/src/wynntilsresolver/exceptions.py
+-rwxr-xr-x   0        0        0     1374 2023-05-07 21:56:38.495741 wynntilsresolver-0.1.5/src/wynntilsresolver/model.py
+-rwxr-xr-x   0        0        0     2439 2023-05-07 21:57:06.674456 wynntilsresolver-0.1.5/src/wynntilsresolver/resolver.py
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 wynntilsresolver-0.1.5/PKG-INFO
```

### Comparing `wynntilsresolver-0.1.4/LICENSE` & `wynntilsresolver-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-0.1.4/pyproject.toml` & `wynntilsresolver-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "WynntilsResolver"
-version = "0.1.4"
+version = "0.1.5"
 description = "A simple resolver to analyze wynntils' encoded equipment in chat."
 authors = [
     { name = "FYWinds", email = "i@windis.cn" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "readme.md"
```

### Comparing `wynntilsresolver-0.1.4/src/wynntilsresolver/model.py` & `wynntilsresolver-0.1.5/src/wynntilsresolver/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Author       : FYWinds i@windis.cn
 Date         : 2023-05-01 09:20:21
 LastEditors  : FYWinds i@windis.cn
-LastEditTime : 2023-05-01 14:40:10
+LastEditTime : 2023-05-07 17:56:38
 FilePath     : /src/wynntilsresolver/model.py
 
 Copyright (c) 2023 by FYWinds
 All Rights Reserved.
 Any modifications or distributions of the file
 should mark the original author's name.
 """
@@ -31,15 +31,15 @@
         return self.name
 
 
 @dataclasses.dataclass(frozen=True)
 class Item:
     name: str
     """The name of the item"""
-    ids: List[float]
+    ids: List[int]
     """The roll values of the item, sorted in wynntils' item identification order
     Can calculate by multiplying the id's base value"""
     powders: List[Powder]
     """Powders on the item, without tier"""
     rerolls: int
     """Rerolls of the item"""
```

### Comparing `wynntilsresolver-0.1.4/src/wynntilsresolver/resolver.py` & `wynntilsresolver-0.1.5/src/wynntilsresolver/resolver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Author       : FYWinds i@windis.cn
 Date         : 2023-05-01 09:08:08
 LastEditors  : FYWinds i@windis.cn
-LastEditTime : 2023-05-01 11:30:04
-FilePath     : /wynntilsresolver/resolver.py
+LastEditTime : 2023-05-07 17:56:51
+FilePath     : /src/wynntilsresolver/resolver.py
 
 Copyright (c) 2023 by FYWinds
 All Rights Reserved.
 Any modifications or distributions of the file
 should mark the original author's name.
 """
 import dataclasses
@@ -51,20 +51,19 @@
 
     def decode(self, text: str) -> Item:
         if m := self.pattern.match(text):
             name = m.group("Name")
             ids = self._decode_numbers(m.group("Ids"))
             powders = self._decode_numbers(m.group("Powders"))
             rerolls = self._decode_numbers(m.group("Rerolls"))[0]
-            ids = [((i / 4) + 30) / 100 for i in ids]  # id rolls from 0.3 to 1.3
             return Item(name, ids, self._decode_powders(powders), rerolls)
         else:
             raise ItemNotValidError(f"Given text {text} is not a valid encoded item.")
 
-    def decode_to_json(self, text) -> dict:
+    def decode_to_json(self, text: str) -> dict:
         return dataclasses.asdict(self.decode(text))
 
     def _decode_powders(self, powders: List[int]) -> List[Powder]:
         powders.reverse()
         plist = []
         for powderNum in powders:
             while powderNum > 0:
```

### Comparing `wynntilsresolver-0.1.4/PKG-INFO` & `wynntilsresolver-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wynntilsresolver
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple resolver to analyze wynntils' encoded equipment in chat.
 Keywords: wynntils resolver wynncraft
 Author-Email: FYWinds <i@windis.cn>
 License: GLWTPL
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -36,26 +36,38 @@
 
 Use as a package
 
 ```python
 from wynntilsresolver import resolver
 
 print(resolver.decode("󵿰Warp󵿲󵃨󵄴󵁤󵀠󵁤󵂄󵅥󵀀󵃌󵿲󵃗󵀄󵿱"))
-# Item(name='Warp', ids=[0.88, 1.07, 0.55, 0.38, 0.55, 0.63, 1.1925, 0.3, 0.81], powders=[AIR, AIR, AIR], rerolls=4)
+# Item(name='Warp', ids=[232, 308, 100, 32, 100, 132, 357, 0, 204], powders=[AIR, AIR, AIR], rerolls=4)
 print(resolver.decode_to_json("󵿰Warp󵿲󵃨󵄴󵁤󵀠󵁤󵂄󵅥󵀀󵃌󵿲󵃗󵀄󵿱"))
-# {'name': 'Warp', 'ids': [0.88, 1.07, 0.55, 0.38, 0.55, 0.63, 1.1925, 0.3, 0.81], 'powders': ['AIR', 'AIR', 'AIR'], 'rerolls': 4}
+# {'name': 'Warp', 'ids': [232, 308, 100, 32, 100, 132, 357, 0, 204], 'powders': ['AIR', 'AIR', 'AIR'], 'rerolls': 4}
+```
+
+> The calculation of the true roll value will rely on the identifications differ between the items.
+> Please calculate using the following algorithm:
+
+```python
+if baseValue > 100:
+    trueRoll = ((id/4 + 30) / 100) * baseValue
+else:
+    trueRoll = idRange.low + id/4
 ```
 
 Or initialite with your own match pattern
 ```python
 import re
 from wynntilsresolver import Resolver
 
 resolver = Resolver(pattern=re.compile(...))
 ```
 
 Use the cli
+
+This will defaulted decode the item into json format
 ```bash
 pip install wynntilsresolver[cli]
 python -m wynntilsresolver 󵿰Warp󵿲󵃨󵄴󵁤󵀠󵁤󵂄󵅥󵀀󵃌󵿲󵃗󵀄󵿱 
-# IN some terminal environment, you are not able to input some of the unicode string and will result in an ItemNotValidError
+# In some terminal environment, you are not able to input some of the unicode string and will result in an ItemNotValidError
 ```
```

