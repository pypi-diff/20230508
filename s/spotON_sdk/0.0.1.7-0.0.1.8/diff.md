# Comparing `tmp/spotON_sdk-0.0.1.7.tar.gz` & `tmp/spotON_sdk-0.0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.1.7.tar", last modified: Mon May  8 08:25:01 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.1.8.tar", last modified: Mon May  8 09:21:08 2023, max compression
```

## Comparing `spotON_sdk-0.0.1.7.tar` & `spotON_sdk-0.0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.7/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.7/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.1.7/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-08 08:24:40.645545 spotON_sdk-0.0.1.7/spotON_sdk/__init__.py
--rw-r--r--   0        0        0     4801 2023-05-08 08:12:43.917785 spotON_sdk-0.0.1.7/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     1468 2023-05-08 08:21:51.312070 spotON_sdk-0.0.1.7/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.7/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0      138 2023-05-08 08:23:54.822670 spotON_sdk-0.0.1.7/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.8/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.8/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-08 09:20:48.635973 spotON_sdk-0.0.1.8/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0     4800 2023-05-08 09:11:38.492606 spotON_sdk-0.0.1.8/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     1594 2023-05-08 09:20:38.293918 spotON_sdk-0.0.1.8/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.8/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0      174 2023-05-08 09:11:24.703434 spotON_sdk-0.0.1.8/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.8/PKG-INFO
```

### Comparing `spotON_sdk-0.0.1.7/.gitignore` & `spotON_sdk-0.0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.7/LICENSE` & `spotON_sdk-0.0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.7/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.1.8/spotON_sdk/constants/countries.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
             print(f"{self.capital} not found in European capitals.")
             return None
 
     def __post_init__(self: Any) -> None:
         self.delta,self.UTC_time_difference = self.calculate_utc_time_difference()
         self.emoji = _country_code_to_emoji(self.country_code)
 
-
 @dataclass
 class Austria(Country):
     capital: str = "Europe/Vienna"
     country_code: str = "AT"
 
 
 @dataclass
```

### Comparing `spotON_sdk-0.0.1.7/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.1.8/spotON_sdk/constants/markets.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,18 @@
         self.name = f"{self.country.emoji} {self.country.__class__.__name__}"
         #self.get_Market_by_area_code(self.area.name)
 
 dataclass
 class Markets():
     austria = Market(Area.AT,Austria())
     germany = Market(Area.DE,Germany())
-    sweden = Market(Area.SE,Sweden())
+    sweden1 = Market(Area.SE_1,Sweden())
+    sweden2 = Market(Area.SE_2,Sweden())
+    sweden3 = Market(Area.SE_3,Sweden())
+    sweden4 = Market(Area.SE_4,Sweden())
     markets_List = [value for key, value in vars().items() if isinstance(value, Market)]
 
     @staticmethod
     def get_Market_by_area_code(area_code: str) -> Optional[Market]:
         for country in Markets.markets_List:
             if country.country_code == area_code:
                 return country
```

### Comparing `spotON_sdk-0.0.1.7/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.1.8/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

