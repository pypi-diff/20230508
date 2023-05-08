# Comparing `tmp/spotON_sdk-0.0.2.1.tar.gz` & `tmp/spotON_sdk-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.2.1.tar", last modified: Mon May  8 15:05:47 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.2.2.tar", last modified: Mon May  8 20:32:13 2023, max compression
```

## Comparing `spotON_sdk-0.0.2.1.tar` & `spotON_sdk-0.0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.2.1/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.1/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-08 15:05:34.172222 spotON_sdk-0.0.2.1/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.1/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.1/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2018 2023-05-08 14:51:04.730672 spotON_sdk-0.0.2.1/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.1/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0      251 2023-05-08 14:51:22.990857 spotON_sdk-0.0.2.1/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.2.2/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.2/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-08 20:32:08.469735 spotON_sdk-0.0.2.2/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.2/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.2/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2068 2023-05-08 20:31:55.757613 spotON_sdk-0.0.2.2/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.2/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0      251 2023-05-08 14:51:22.990857 spotON_sdk-0.0.2.2/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.2/PKG-INFO
```

### Comparing `spotON_sdk-0.0.2.1/.gitignore` & `spotON_sdk-0.0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.1/LICENSE` & `spotON_sdk-0.0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.1/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.2.2/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.1/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.2.2/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.1/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.2.2/spotON_sdk/constants/markets.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 
         self.name = f"{self.country.emoji} {self.country.__class__.__name__} {self.area_code} {self.cities}"
         #self.get_Market_by_area_code(self.area.name)
 
 dataclass
 class Markets():
     austria = Market(Area.AT,Austria)
-    germany = Market(Area.DE,Germany)
+    germany = Market(Area.DE_LU,Germany)
+    luxembourg = Market(Area.DE_LU,Luxembourg)
     sweden1 = Market(Area.SE_1,Sweden)
     sweden2 = Market(Area.SE_2,Sweden)
     sweden3 = Market(Area.SE_3,Sweden)
     sweden4 = Market(Area.SE_4,Sweden)
     markets_List = [value for key, value in vars().items() if isinstance(value, Market)]
 
     @staticmethod
```

### Comparing `spotON_sdk-0.0.2.1/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.2.2/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

