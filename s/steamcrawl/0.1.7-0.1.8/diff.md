# Comparing `tmp/steamcrawl-0.1.7.tar.gz` & `tmp/steamcrawl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steamcrawl-0.1.7.tar", last modified: Sun May  7 13:53:09 2023, max compression
+gzip compressed data, was "steamcrawl-0.1.8.tar", last modified: Mon May  8 16:54:53 2023, max compression
```

## Comparing `steamcrawl-0.1.7.tar` & `steamcrawl-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 13:53:09.144461 steamcrawl-0.1.7/
--rw-rw-rw-   0        0        0     1085 2023-05-06 17:48:49.000000 steamcrawl-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      724 2023-05-07 13:53:09.144461 steamcrawl-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-05-07 13:50:42.000000 steamcrawl-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-07 13:53:09.144461 steamcrawl-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      656 2023-05-07 13:52:49.000000 steamcrawl-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:53:09.138476 steamcrawl-0.1.7/steamcrawl/
--rw-rw-rw-   0        0        0       28 2023-05-07 13:37:24.000000 steamcrawl-0.1.7/steamcrawl/__init__.py
--rw-rw-rw-   0        0        0      543 2023-05-05 21:51:45.000000 steamcrawl-0.1.7/steamcrawl/exceptions.py
--rw-rw-rw-   0        0        0    16867 2023-05-07 13:48:49.000000 steamcrawl-0.1.7/steamcrawl/request.py
--rw-rw-rw-   0        0        0        0 2023-05-07 11:37:40.000000 steamcrawl-0.1.7/steamcrawl/requestCounter.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:53:09.143464 steamcrawl-0.1.7/steamcrawl.egg-info/
--rw-rw-rw-   0        0        0      724 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 16:54:53.879324 steamcrawl-0.1.8/
+-rw-rw-rw-   0        0        0     1085 2023-05-06 17:48:49.000000 steamcrawl-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     3990 2023-05-08 16:54:53.879324 steamcrawl-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3580 2023-05-08 16:54:22.000000 steamcrawl-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:54:53.880321 steamcrawl-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      656 2023-05-08 16:52:48.000000 steamcrawl-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:54:53.854390 steamcrawl-0.1.8/steamcrawl/
+-rw-rw-rw-   0        0        0       28 2023-05-07 13:37:24.000000 steamcrawl-0.1.8/steamcrawl/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-05-07 15:13:15.000000 steamcrawl-0.1.8/steamcrawl/exceptions.py
+-rw-rw-rw-   0        0        0    17527 2023-05-08 16:42:05.000000 steamcrawl-0.1.8/steamcrawl/request.py
+-rw-rw-rw-   0        0        0        0 2023-05-07 11:37:40.000000 steamcrawl-0.1.8/steamcrawl/requestCounter.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:54:53.878325 steamcrawl-0.1.8/steamcrawl.egg-info/
+-rw-rw-rw-   0        0        0     3990 2023-05-08 16:54:53.000000 steamcrawl-0.1.8/steamcrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-08 16:54:53.000000 steamcrawl-0.1.8/steamcrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:54:53.000000 steamcrawl-0.1.8/steamcrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-08 16:54:53.000000 steamcrawl-0.1.8/steamcrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 16:54:53.000000 steamcrawl-0.1.8/steamcrawl.egg-info/top_level.txt
```

### Comparing `steamcrawl-0.1.7/LICENSE` & `steamcrawl-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `steamcrawl-0.1.7/setup.py` & `steamcrawl-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='steamcrawl',
-    version='0.1.7',
+    version='0.1.8',
     description='A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.',
     packages=["steamcrawl"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Hungreeee',
     author_email='hungmnguyen13102003@gmail.com',
     license='MIT',
```

### Comparing `steamcrawl-0.1.7/steamcrawl/exceptions.py` & `steamcrawl-0.1.8/steamcrawl/exceptions.py`

 * *Files identical despite different names*

### Comparing `steamcrawl-0.1.7/steamcrawl/request.py` & `steamcrawl-0.1.8/steamcrawl/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,31 @@
 from steamcrawl.exceptions import exception
 
 warnings.simplefilter(action = "ignore", category = RuntimeWarning)
 
 
 class Request:
 
-  def __init__(self):
+  def __init__(self, steamLoginSecure: str):
     self.headers = {
       'Cookie': ''
     }
     self.__all_listings_api = 'https://steamcommunity.com/market/search/render/?search_descriptions=0&norender=1'
     self.__appid_api = 'https://api.steampowered.com/ISteamApps/GetAppList/v2/'
     self.__pricehistory_api = 'https://steamcommunity.com/market/pricehistory/'
     self.__item_overview_api = 'https://steamcommunity.com/market/priceoverview/'
     self.__listingshistory_api = 'https://steamcommunity.com/market/myhistory/render/?norender=1'
     self.__appdetails_api = 'https://store.steampowered.com/api/appdetails/'
 
+    exception('type', steamLoginSecure, str, "Input steamLoginSecure it not a valid string type.")
+    header = 'steamLoginSecure=' + steamLoginSecure + ';'
+    testApi = 'https://steamcommunity.com/market/pricehistory/?appid=730&market_hash_name=P90%20%7C%20Blind%20Spot%20(Field-Tested)'
+    requestObject = requests.get(testApi, headers={'Cookie': header}, timeout=1.0).content
+    exception('network', str(requestObject), 'b\'[]\'', "Input header it not an authorized cookie header.")
+    self.headers['Cookie'] = header
 
   def set_steam_auth(self, steamLoginSecure: str):
     """
     """
     exception('type', steamLoginSecure, str, "Input steamLoginSecure it not a valid string type.")
     header = 'steamLoginSecure=' + steamLoginSecure + ';'
     testApi = 'https://steamcommunity.com/market/pricehistory/?appid=730&market_hash_name=P90%20%7C%20Blind%20Spot%20(Field-Tested)'
@@ -36,16 +42,16 @@
   def __request_helper(self, api: str, params: dict, headers: dict, index: list):
     """
     """
     dfGather = []
     requestObject = requests.get(api, params=params, headers=headers, timeout=1.0)
     contentObject = json.loads(requestObject.content)
 
-    for i in contentObject:
-      if i in index:
+    for i in index:
+      if i in contentObject:
         if contentObject[i] != []:
           dfGather.append(contentObject[i])
 
     if 'success' in contentObject:
       isSuccess = contentObject['success']
       exception('network', isSuccess, False, "Steam cannot make this API call. Please double check your parameters and try again.")
     
@@ -318,26 +324,28 @@
           if str(request.url[34:53]) == 'itemordershistogram':
             api = request.url
             bodyObject = request.response.body
             break
 
     exception('network', api, "", "Steam cannot make this query. Please double check the item name and try again.")
     response = requests.get(api + '&norender=1', headers=self.headers, timeout=1.0)
-    contentObject = response.content
     exception('network', str(response.content), 'b\'null\'', "You have reached the request limit of Steam. Please try again later.")
-    dfSellGraph = pd.json_normalize(json.loads(contentObject), record_path=['sell_order_graph'])
-    dfBuyGraph = pd.json_normalize(json.loads(contentObject), record_path=['buy_order_graph'])
+    contentObject = json.loads(response.content)
+    dfSellGraph = pd.json_normalize(contentObject, record_path=['sell_order_graph'])
+    dfBuyGraph = pd.json_normalize(contentObject, record_path=['buy_order_graph'])
     
     dfSellGraph['type'] = 'sell'
     dfBuyGraph['type'] = 'buy'
     if 'success' in contentObject:
       isSuccess = contentObject['success']
       exception('network', isSuccess, False, "Steam cannot make this API call. Please double check your parameters and try again.")
     dfCombined = [dfSellGraph, dfBuyGraph]
-    return pd.concat(dfCombined, ignore_index=True)
+    dfCombined = pd.concat(dfCombined, ignore_index=True)
+    dfCombined = dfCombined.rename(columns={0: 'price', 1: 'orders', 2: 'description'})
+    return dfCombined
   
   def get_itemname_id(self, item_name: str, appid: str):
     """
     """
     exception('type', item_name, str, "Input item_name it not a valid string type.")
     exception('type', appid, str, "Input appid it not a valid string type.")
     exception('network', self.headers['Cookie'], '',
```

