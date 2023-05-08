# Comparing `tmp/vortex_api-1.0.2.tar.gz` & `tmp/vortex_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-_x8faosk/vortex_api-1.0.2.tar", last modified: Wed May  3 19:51:36 2023, max compression
+gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-qw9lo195/vortex_api-1.0.3.tar", last modified: Mon May  8 08:09:04 2023, max compression
```

## Comparing `vortex_api-1.0.2.tar` & `vortex_api-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-03 19:51:36.902295 vortex_api-1.0.2/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.2/LICENSE
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1513 2023-05-03 19:51:36.902408 vortex_api-1.0.2/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      657 2023-05-03 18:53:00.000000 vortex_api-1.0.2/README.md
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-03 19:51:36.902787 vortex_api-1.0.2/setup.cfg
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1385 2023-05-03 15:16:34.000000 vortex_api-1.0.2/setup.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-03 19:51:36.900043 vortex_api-1.0.2/vortex_api/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1311 2023-05-03 18:26:27.000000 vortex_api-1.0.2/vortex_api/__init__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      336 2023-05-03 18:51:41.000000 vortex_api-1.0.2/vortex_api/__version__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    15719 2023-05-03 19:45:13.000000 vortex_api-1.0.2/vortex_api/api.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-03 19:51:36.901938 vortex_api-1.0.2/vortex_api.egg-info/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1513 2023-05-03 19:51:36.000000 vortex_api-1.0.2/vortex_api.egg-info/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      272 2023-05-03 19:51:36.000000 vortex_api-1.0.2/vortex_api.egg-info/SOURCES.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-03 19:51:36.000000 vortex_api-1.0.2/vortex_api.egg-info/dependency_links.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       17 2023-05-03 19:51:36.000000 vortex_api-1.0.2/vortex_api.egg-info/requires.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-03 19:51:36.000000 vortex_api-1.0.2/vortex_api.egg-info/top_level.txt
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-08 08:09:04.049893 vortex_api-1.0.3/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.3/LICENSE
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1513 2023-05-08 08:09:04.049975 vortex_api-1.0.3/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      657 2023-05-03 18:53:00.000000 vortex_api-1.0.3/README.md
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-08 08:09:04.050223 vortex_api-1.0.3/setup.cfg
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1385 2023-05-03 15:16:34.000000 vortex_api-1.0.3/setup.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-08 08:09:04.048591 vortex_api-1.0.3/vortex_api/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1311 2023-05-03 18:26:27.000000 vortex_api-1.0.3/vortex_api/__init__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      336 2023-05-08 08:08:06.000000 vortex_api-1.0.3/vortex_api/__version__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    18143 2023-05-08 06:54:13.000000 vortex_api-1.0.3/vortex_api/api.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-08 08:09:04.049752 vortex_api-1.0.3/vortex_api.egg-info/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1513 2023-05-08 08:09:04.000000 vortex_api-1.0.3/vortex_api.egg-info/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      272 2023-05-08 08:09:04.000000 vortex_api-1.0.3/vortex_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-08 08:09:04.000000 vortex_api-1.0.3/vortex_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       17 2023-05-08 08:09:04.000000 vortex_api-1.0.3/vortex_api.egg-info/requires.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-08 08:09:04.000000 vortex_api-1.0.3/vortex_api.egg-info/top_level.txt
```

### Comparing `vortex_api-1.0.2/LICENSE` & `vortex_api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.2/PKG-INFO` & `vortex_api-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `vortex_api-1.0.2/README.md` & `vortex_api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.2/setup.py` & `vortex_api-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.2/vortex_api/__init__.py` & `vortex_api-1.0.3/vortex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.2/vortex_api/api.py` & `vortex_api-1.0.3/vortex_api/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
 import csv
+import datetime
 
 class AsthaTradeVortexAPI:
 
     #Constants 
 
     #Exchanges
     EXCHANGE_NSE_FO = "NSE_FO"
@@ -26,15 +27,18 @@
     VALIDITY_FULL_DAY = "DAY"
     VALIDITY_IMMEDIATE_OR_CANCEL = "IOC"
     VALIDITY_AFTER_MARKET = "AMO"
 
     # Transaction type
     TRANSACTION_TYPE_BUY = "BUY"
     TRANSACTION_TYPE_SELL = "SELL"
-    
+
+    QUOTE_MODE_LTP = "ltp"
+    QUOTE_MODE_FULL = "full"
+    QUOTE_MODE_OHLC = "ohlc"
 
     def __init__(self, api_key: str, application_id: str, base_url: str = "https://vortex.restapi.asthatrade.com") -> None:
         """
         Constructor method for AsthaTradeAPI class.
 
         Args:
             api_key (str): API key for the Astha Trade API.
@@ -42,15 +46,15 @@
             base_url (str, optional): Base URL for the Astha Trade API. Defaults to "https://vortex.restapi.asthatrade.com".
         """
         self.api_key = api_key
         self.application_id = application_id
         self.base_url = base_url
         self.access_token = None
 
-    def _make_api_request(self, method: str, endpoint: str, data: dict = None) -> dict:
+    def _make_api_request(self, method: str, endpoint: str, data: dict = None, params=None) -> dict:
         """
         Private method to make HTTP requests to the Astha Trade API.
 
         Args:
             method (str): HTTP method for the request (e.g. "GET", "POST", "PUT", "DELETE").
             endpoint (str): API endpoint for the request.
             data (dict, optional): Payload data for the request. Defaults to None.
@@ -62,15 +66,15 @@
             op = {}
             op["status"]= "error"
             op["message"] = "please login first"
             return op
         bearer_token = f"Bearer {self.access_token}"
         headers = {"Content-Type": "application/json", "Authorization": bearer_token}
         url = self.base_url + endpoint
-        response = requests.request(method, url, headers=headers, json=data)
+        response = requests.request(method, url, headers=headers, json=data,params=params)
 
         response.raise_for_status()
         return response.json()
     
     def _make_unauth_request(self, method: str, endpoint: str, data: dict = None) -> dict:
         """
         Private method to make HTTP requests to the Astha Trade API.
@@ -324,14 +328,59 @@
             "validity": validity,
             "validity_days": validity_days,
             "mode": mode,
             "is_amo": is_amo
         }
         return self._make_api_request("POST", endpoint, data=data)
     
+    def quotes(self, *instruments, mode: str)-> dict: 
+        """
+        Gets quotes of up to 1000 instruments at a time. 
+
+        Args: 
+            instrument(list): List of instruments. The items should be like ( "NSE_EQ-22", "NSE_FO-1234")
+
+        Returns 
+            dict: JSON response containing quotes. It is possible that not all the symbol identifiers you passed had a quote available. Those inputs will be missing from the response.
+            Also, the order of output might be different than the order of input
+        """
+        endpoint = "/data/quotes"
+        i = list(instruments)
+        params = {"q": instruments,"mode": mode}
+        return self._make_api_request("GET", endpoint, data=None,params=params)
+    
+    def historical_candles(self, exchange: str, token: int, to: datetime.datetime , start: datetime.datetime, resolution: str): 
+        """
+        Gets historical candle data of a particular instrument. 
+
+        Args: 
+            exchange (str): Possible values: [NSE_EQ, NSE_FO, NSE_CD or MCX_FO]
+            token (int): Security token of the scrip. It can be found in the scripmaster file
+            to(datetime): datetime up till when you want to receive candles 
+            start(datetime): datetime from when you want to receive candles 
+            resolution(str): resoulution of the candle. can be "1", "2", "3", "4", "5", "10", "15", "30", "45", "60", "120", "180", "240", "1D", "1W", "1M"
+        """
+
+        if not isinstance(exchange, str):
+            raise TypeError("exchange must be a string")
+        if not isinstance(token, int):
+            raise TypeError("token must be an integer")
+        if not isinstance(to,datetime.datetime): 
+            raise TypeError("to must be a datetime")
+        if not isinstance(start,datetime.datetime): 
+            raise TypeError("start must be a datetime")
+        if not isinstance(resolution,str): 
+            raise TypeError("resolution must be string")
+
+        endpoint = "/data/history"
+        params = {"exchange": exchange,"token": token , "to": int(to.timestamp()), "from": int(start.timestamp()), "resolution": resolution}
+        print(params)
+        return self._make_api_request("GET", endpoint, data=None,params=params)
+
+    
     def _setup_client_code(self, login_object: dict) -> bool: 
         """ 
         Sets up access token after login
 
         Args: 
             login_object(dict): Login object received
```

### Comparing `vortex_api-1.0.2/vortex_api.egg-info/PKG-INFO` & `vortex_api-1.0.3/vortex_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```

