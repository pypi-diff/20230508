# Comparing `tmp/spotON_sdk-0.0.1.8.tar.gz` & `tmp/spotON_sdk-0.0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.1.8.tar", last modified: Mon May  8 09:21:08 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.1.9.tar", last modified: Mon May  8 09:33:00 2023, max compression
```

## Comparing `spotON_sdk-0.0.1.8.tar` & `spotON_sdk-0.0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.8/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.8/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.1.8/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-08 09:20:48.635973 spotON_sdk-0.0.1.8/spotON_sdk/__init__.py
--rw-r--r--   0        0        0     4800 2023-05-08 09:11:38.492606 spotON_sdk-0.0.1.8/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     1594 2023-05-08 09:20:38.293918 spotON_sdk-0.0.1.8/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.8/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0      174 2023-05-08 09:11:24.703434 spotON_sdk-0.0.1.8/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.9/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.9/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-08 09:31:40.713773 spotON_sdk-0.0.1.9/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0     4800 2023-05-08 09:31:35.980158 spotON_sdk-0.0.1.9/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     1611 2023-05-08 09:29:58.120135 spotON_sdk-0.0.1.9/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.9/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0      249 2023-05-08 09:31:23.040049 spotON_sdk-0.0.1.9/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.9/PKG-INFO
```

### Comparing `spotON_sdk-0.0.1.8/.gitignore` & `spotON_sdk-0.0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.8/LICENSE` & `spotON_sdk-0.0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.8/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.1.9/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.8/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.1.9/spotON_sdk/constants/markets.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.area_code = self.area.name
         country_region = self.area_code.split("_")
         self.country_code = country_region[0]
         if len(country_region) >=2:
             self.region_code = country_region[1]
         else:
             self.region_code = ""
-        self.name = f"{self.country.emoji} {self.country.__class__.__name__}"
+        self.name = f"{self.country.emoji} {self.country.__class__.__name__} {self.area_code}"
         #self.get_Market_by_area_code(self.area.name)
 
 dataclass
 class Markets():
     austria = Market(Area.AT,Austria())
     germany = Market(Area.DE,Germany())
     sweden1 = Market(Area.SE_1,Sweden())
```

### Comparing `spotON_sdk-0.0.1.8/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.1.9/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

