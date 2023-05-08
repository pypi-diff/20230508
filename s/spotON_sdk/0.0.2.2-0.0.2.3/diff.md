# Comparing `tmp/spotON_sdk-0.0.2.2.tar.gz` & `tmp/spotON_sdk-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.2.2.tar", last modified: Mon May  8 20:32:13 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.2.3.tar", last modified: Mon May  8 20:51:02 2023, max compression
```

## Comparing `spotON_sdk-0.0.2.2.tar` & `spotON_sdk-0.0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.2.2/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.2/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.2/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-08 20:32:08.469735 spotON_sdk-0.0.2.2/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.2/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.2/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2068 2023-05-08 20:31:55.757613 spotON_sdk-0.0.2.2/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.2/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0      251 2023-05-08 14:51:22.990857 spotON_sdk-0.0.2.2/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.2.3/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.3/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-08 20:50:56.475068 spotON_sdk-0.0.2.3/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.3/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.3/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.2.3/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.3/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.2.3/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.3/PKG-INFO
```

### Comparing `spotON_sdk-0.0.2.2/.gitignore` & `spotON_sdk-0.0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.2/LICENSE` & `spotON_sdk-0.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.2/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.2.3/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.2/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.2.3/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.2/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.2.3/spotON_sdk/constants/markets.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,37 +11,35 @@
 from .countries import *
 from .bidding_zones import bidding_zones
 
 @dataclass
 class Market():
     area:Area
     country :Country
+    area_code :str = field(init=False)
     country_code : str = field(init=False)
-    region_code : str = field(init=False)
+    region_code : str | None = field(init=False,default=None)
     cities : str = field(init=False)
 
-
     def __post_init__(self):
         self.area_code = self.area.name
         country_region = self.area_code.split("_")
         self.country_code = country_region[0]
         if len(country_region) >=2:
             self.region_code = country_region[1]
-        else:
-            self.region_code = ""
         print (self.area_code)
         try:
             city_List = bidding_zones[self.area_code]["cities"]
             my_string = ', '.join(city_List)
             self.cities = my_string
         except:
-            self.cities = "no city"
+            self.cities = ""
 
 
-        self.name = f"{self.country.emoji} {self.country.__class__.__name__} {self.area_code} {self.cities}"
+        self.name = f"{self.country.emoji} {self.country.country_name} {self.area_code} {self.cities}"
         #self.get_Market_by_area_code(self.area.name)
 
 dataclass
 class Markets():
     austria = Market(Area.AT,Austria)
     germany = Market(Area.DE_LU,Germany)
     luxembourg = Market(Area.DE_LU,Luxembourg)
```

### Comparing `spotON_sdk-0.0.2.2/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.2.3/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

