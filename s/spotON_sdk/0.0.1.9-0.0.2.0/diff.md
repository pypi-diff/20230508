# Comparing `tmp/spotON_sdk-0.0.1.9.tar.gz` & `tmp/spotON_sdk-0.0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.1.9.tar", last modified: Mon May  8 09:33:00 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.2.0.tar", last modified: Mon May  8 10:30:35 2023, max compression
```

## Comparing `spotON_sdk-0.0.1.9.tar` & `spotON_sdk-0.0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.9/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.9/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.1.9/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-08 09:31:40.713773 spotON_sdk-0.0.1.9/spotON_sdk/__init__.py
--rw-r--r--   0        0        0     4800 2023-05-08 09:31:35.980158 spotON_sdk-0.0.1.9/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     1611 2023-05-08 09:29:58.120135 spotON_sdk-0.0.1.9/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.9/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0      249 2023-05-08 09:31:23.040049 spotON_sdk-0.0.1.9/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.2.0/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.0/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-08 10:30:14.925290 spotON_sdk-0.0.2.0/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.0/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4225 2023-05-08 10:07:05.374063 spotON_sdk-0.0.2.0/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2030 2023-05-08 10:21:43.909352 spotON_sdk-0.0.2.0/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.0/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0      287 2023-05-08 10:22:03.210055 spotON_sdk-0.0.2.0/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.0/PKG-INFO
```

### Comparing `spotON_sdk-0.0.1.9/.gitignore` & `spotON_sdk-0.0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.9/LICENSE` & `spotON_sdk-0.0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.9/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.2.0/spotON_sdk/constants/countries.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     return ''.join(chr(ord(c) + OFFSET) for c in country_code.upper())
 
 @dataclass
 class Country:
     capital: str
     country_code: str
     UTC_time_difference: int = field(init=False)
-
+    has_Bidding_Zones :bool = False
+    
     def calculate_utc_time_difference(self) -> Optional[pd.Timedelta]:
         try:
             local_tz = pytz.timezone(self.capital)
             utc_dt = pd.Timestamp.utcnow().to_pydatetime()
             local_dt = utc_dt.astimezone(local_tz)
             UTC_time_difference = (local_dt.utcoffset().total_seconds()) // 3600
             delta = pd.Timedelta(hours=UTC_time_difference)
@@ -34,14 +35,15 @@
         self.delta,self.UTC_time_difference = self.calculate_utc_time_difference()
         self.emoji = _country_code_to_emoji(self.country_code)
 
 @dataclass
 class Austria(Country):
     capital: str = "Europe/Vienna"
     country_code: str = "AT"
+    
 
 
 @dataclass
 class Belgium(Country):
     capital: str = "Europe/Brussels"
     country_code: str = "BE"
 
@@ -189,41 +191,17 @@
     country_code: str = "ES"
 
 
 @dataclass
 class Sweden(Country):
     capital: str = "Europe/Stockholm"
     country_code: str = "SE"
+    has_Bidding_Zones :bool = False
 
 
-'''@dataclass
-class Market():
-    area:Area
-    country :Country
-
-
-
-    def __post_init__(self):
-        self.area_code = self.area.name
-        country_region = self.area_code.split("_")
-        self.country_code = country_region[0]
-        if len(country_region) >=2:
-            self.region_code = country_region[1]
-        else:
-            self.region_code = ""
-        #self.get_Market_by_area_code(self.area.name)
-
-@dataclass
-class Markets():
-    austria = Market(Area.AT,Austria)
-    germany = Market(Area.DE,Germany)
-    sweden = Market(Area.SE,Sweden)
-    markets_List = [value for key, value in vars().items() if isinstance(value, Market)]
-
-'''
 
 def return_All_Areas(filterstring:str ="MBA"):
         
     result = []
     for area in Area:
         #print (area.name, area.meaning)
         if filterstring in area.meaning:
```

### Comparing `spotON_sdk-0.0.1.9/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.2.0/spotON_sdk/constants/markets.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,31 +5,43 @@
 import pandas as pd
 from dataclasses import dataclass, field
 from typing import Optional, Dict,Any
 import pytz
 
 from typing import List
 from .countries import *
+from .bidding_zones import bidding_zones
 
 @dataclass
 class Market():
     area:Area
     country :Country
-
+    country_code : str = field(init=False)
+    region_code : str = field(init=False)
+    cities : str = field(init=False)
 
 
     def __post_init__(self):
         self.area_code = self.area.name
         country_region = self.area_code.split("_")
         self.country_code = country_region[0]
         if len(country_region) >=2:
             self.region_code = country_region[1]
         else:
             self.region_code = ""
-        self.name = f"{self.country.emoji} {self.country.__class__.__name__} {self.area_code}"
+        print (self.area_code)
+        try:
+            city_List = bidding_zones[self.area_code]["cities"]
+            my_string = ', '.join(city_List)
+            self.cities = my_string
+        except:
+            self.cities = "no city"
+
+
+        self.name = f"{self.country.emoji} {self.country.__class__.__name__} {self.area_code} {self.cities}"
         #self.get_Market_by_area_code(self.area.name)
 
 dataclass
 class Markets():
     austria = Market(Area.AT,Austria())
     germany = Market(Area.DE,Germany())
     sweden1 = Market(Area.SE_1,Sweden())
```

### Comparing `spotON_sdk-0.0.1.9/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.2.0/spotON_sdk/logic/Config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import List
 
+from ..constants.markets import Market
 class Switchtypes():
     switch = "Switch"
     dimmer = "Dimmer"
 
 
 class PeriodTypes():
     wholeDay :str = "24h Hour Period"
@@ -21,14 +22,15 @@
 
 
 @dataclass
 class Config():
     switchtype :Switchtypes
     nr_of_Hours_On :int
     uninterrupted :bool
+    market : Market 
     timeframe :List[List[int]] 
     periodType : str = ""
     bestHour :str = ""
     week: int = 100
     timeFrameValidation = TimeFrameValidation(False)
 
     def __post_init__(self):
```

