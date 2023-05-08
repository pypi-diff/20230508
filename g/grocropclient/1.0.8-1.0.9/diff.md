# Comparing `tmp/grocropclient-1.0.8.tar.gz` & `tmp/grocropclient-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grocropclient-1.0.8.tar", max compression
+gzip compressed data, was "grocropclient-1.0.9.tar", max compression
```

## Comparing `grocropclient-1.0.8.tar` & `grocropclient-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2022-08-04 17:08:26.375438 grocropclient-1.0.8/LICENSE
--rw-r--r--   0        0        0      503 2022-08-04 17:08:26.375733 grocropclient-1.0.8/README.md
--rw-r--r--   0        0        0     2913 2022-08-04 17:08:26.375985 grocropclient-1.0.8/grocropclient/TECH_DETAILS.md
--rw-r--r--   0        0        0       55 2022-08-04 17:08:26.376114 grocropclient-1.0.8/grocropclient/__init__.py
--rw-r--r--   0        0        0   138914 2022-08-16 16:11:38.512141 grocropclient-1.0.8/grocropclient/constants.py
--rw-r--r--   0        0        0     3775 2022-08-13 12:54:59.746252 grocropclient-1.0.8/grocropclient/crop_budgets.py
--rw-r--r--   0        0        0    15378 2022-08-08 15:42:31.563483 grocropclient-1.0.8/grocropclient/crop_budgets_data.py
--rw-r--r--   0        0        0    44041 2022-08-15 16:54:21.265720 grocropclient-1.0.8/grocropclient/gro_crop_client.py
--rw-r--r--   0        0        0      631 2022-08-16 16:11:38.513512 grocropclient-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1250 2022-08-16 16:11:52.017766 grocropclient-1.0.8/setup.py
--rw-r--r--   0        0        0     1241 2022-08-16 16:11:52.018087 grocropclient-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-08-04 17:08:26.375438 grocropclient-1.0.9/LICENSE
+-rw-r--r--   0        0        0      503 2022-08-04 17:08:26.375733 grocropclient-1.0.9/README.md
+-rw-r--r--   0        0        0     2913 2022-08-04 17:08:26.375985 grocropclient-1.0.9/grocropclient/TECH_DETAILS.md
+-rw-r--r--   0        0        0       55 2022-08-04 17:08:26.376114 grocropclient-1.0.9/grocropclient/__init__.py
+-rw-r--r--   0        0        0   138914 2022-08-17 19:26:06.312682 grocropclient-1.0.9/grocropclient/constants.py
+-rw-r--r--   0        0        0     3775 2022-08-13 12:54:59.746252 grocropclient-1.0.9/grocropclient/crop_budgets.py
+-rw-r--r--   0        0        0    15283 2022-08-17 19:26:06.313610 grocropclient-1.0.9/grocropclient/crop_budgets_data.py
+-rw-r--r--   0        0        0    45377 2022-08-17 19:26:06.315056 grocropclient-1.0.9/grocropclient/gro_crop_client.py
+-rw-r--r--   0        0        0      631 2022-08-17 19:26:50.920784 grocropclient-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1250 2022-08-17 19:27:59.375604 grocropclient-1.0.9/setup.py
+-rw-r--r--   0        0        0     1241 2022-08-17 19:27:59.375878 grocropclient-1.0.9/PKG-INFO
```

### Comparing `grocropclient-1.0.8/LICENSE` & `grocropclient-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grocropclient-1.0.8/grocropclient/TECH_DETAILS.md` & `grocropclient-1.0.9/grocropclient/TECH_DETAILS.md`

 * *Files identical despite different names*

### Comparing `grocropclient-1.0.8/grocropclient/constants.py` & `grocropclient-1.0.9/grocropclient/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 	SOYBEANS = 'soybeans'
 
 # Area Weighting Series
 class AreaWeightingSeriesList(Enum):
 	SOYBEANS_YIELD = '170037_270_yield_model'
 	CORN_YIELD = '170037_274_yield_model'
 	SOYBEANS_PRICE = '15851828_270_dtn_aggregated'
-	CORN_PRICE = '15851828_780_dtn_aggregated'
+	CORN_PRICE = '15851828_274_dtn_aggregated'
 
 
 # lowercased custom regions
 # a dict was used as opposed to Enum class due to 
 # presence of '-', '.' and '&' characters in region names
 # outer keys are source_names, inner_keys are region_names
 CROP_BUDGET_REGIONS = {
```

### Comparing `grocropclient-1.0.8/grocropclient/crop_budgets.py` & `grocropclient-1.0.9/grocropclient/crop_budgets.py`

 * *Files identical despite different names*

### Comparing `grocropclient-1.0.8/grocropclient/crop_budgets_data.py` & `grocropclient-1.0.9/grocropclient/crop_budgets_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,19 @@
       "Crop Insurance Payments": {},
       "Government Payments": {
         "Government Payments, Other": [],
         "USDA Agricultural Risk and Price Loss Coverage Program Payments": []
       },
       "Production Revenue": {
         "Producer Prices": [],
-        "Yield": [
-          "Yield Assumption"
-        ]
+        "Yield": []
       },
       "Production Revenue, Projected": {
         "Producer Prices, Projected": [],
+        "Yield Assumption": [],
         "Yield, Historical Average": []
       },
       "Revenues, Other": {}
     },
     "Total Revenues, incl Govt Payments": {}
   },
   "Total Costs": {
@@ -131,14 +130,24 @@
           "Spray Fertilizer Expenses",
           "Spray Herbicide Application Expenses",
           "Spray Spring Burndown Herbicide Expenses",
           "Spread Fertilizer Application Expenses",
           "Straw Harvest Field Operations Expenses",
           "Sweep Plowing Expenses"
         ],
+        "Fuel and Machinery Expenses": [],
+        "Fuel Expenses": [
+          "Diesel Fuel Expenses, General Use Equipment",
+          "Diesel Fuel Expenses, Tractors",
+          "Fuel Expenses, General Use Equipment",
+          "Fuel Expenses, incl Electricity",
+          "Fuel Expenses, incl. Electricity",
+          "Fuel Expenses, Tractors",
+          "Vehicle Expenses"
+        ],
         "Fungicide Application Expenses": [],
         "Ginning and Hauling Expenses": [],
         "Ginning Expenses": [
           "Custom Ginning Expenses"
         ],
         "GinStar Defoliation Expenses": [],
         "Harvest Aid Application Expenses": [
@@ -216,14 +225,15 @@
           "Labor Expenses, Salaried",
           "Labor Expenses, Unallocated"
         ],
         "Machine Hire and Custom Work Expenses": [],
         "Machinery and Energy Expenses": [],
         "Marketing Expenses": [],
         "Operating Expenses, Other": [],
+        "Operating Interest Expenses": [],
         "Overage Expenses": [],
         "Pick and Module Expenses": [],
         "Picking Expenses": [],
         "Pickup Mileage Charge Expenses": [],
         "Planting Expenses": [
           "No-Till Planting Expenses"
         ],
@@ -296,25 +306,14 @@
           "Machinery Depreciation Expenses"
         ],
         "Electricity Expenses": [],
         "Establishment Cost, Equipment": [],
         "Fixed Labor Expenses": [],
         "Fixed Machine Hire Expenses": [],
         "Fixed Utility Expenses": [],
-        "Fuel and Machinery Expenses": [],
-        "Fuel Expenses": [
-          "Diesel Fuel Expenses, General Use Equipment",
-          "Diesel Fuel Expenses, Tractors",
-          "Fuel Expenses, Drying",
-          "Fuel Expenses, General Use Equipment",
-          "Fuel Expenses, incl Electricity",
-          "Fuel Expenses, incl. Electricity",
-          "Fuel Expenses, Tractors",
-          "Vehicle Expenses"
-        ],
         "General Management Expenses": [],
         "Insurance Premium Expenses": [
           "Building Insurance Premium Expenses",
           "Crop Insurance Premium Expenses, Hail",
           "Crop Insurance Premium Expenses, Herbicide Drift",
           "Miscellaneous Insurance Premium Expenses, SCO and STAX",
           "Multiple Peril Crop Insurance (MPCI) Premium Expenses",
@@ -323,17 +322,15 @@
           "Revenue Protection Crop Insurance Premium Expenses, 70%",
           "Revenue Protection Crop Insurance Premium Expenses, 70% SE",
           "Revenue Protection Crop Insurance Premium Expenses, 70% YA",
           "Revenue Protection Crop Insurance Premium Expenses, 70% YE",
           "STAX Crop Insurance Premium Expenses",
           "Supplemental Coverage Option (SCO) Insurance Premium Expenses"
         ],
-        "Interest Expenses": [
-          "Operating Interest Expenses"
-        ],
+        "Interest Expenses": [],
         "Land Opportunity Cost": [],
         "Land rent": [],
         "Land Rent and Lease Payment Expenses": [],
         "Machinery and Equipment Overhead Cost, General Use Equipment": [],
         "Machinery and Equipment Overhead Cost, Implements": [],
         "Machinery and Equipment Overhead Cost, Irrigation Equipment": [],
         "Machinery and Equipment Overhead Cost, Tractors": [],
@@ -366,11 +363,10 @@
   "Net Income": {
     "Net Profit": {},
     "Net Profit, excl Labor and Management Expenses": {},
     "Net Profit, excl Land Expenses": {},
     "Net Profit, excl Land, Labor and Management Expenses": {},
     "Net Profit, excl Overhead Costs": {},
     "Net Profit, Projected": {},
-    "Operating Profit": {},
-    "Operating Profit, incl Govt Payments": {}
+    "Operating Profit": {}
   }
 }
```

### Comparing `grocropclient-1.0.8/grocropclient/gro_crop_client.py` & `grocropclient-1.0.9/grocropclient/gro_crop_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,26 +69,41 @@
         if ItemNameCategoryList.CORN.value in word.lower():
             return ItemNameCategoryList.CORN.value
         elif ItemNameCategoryList.SOYBEANS.value in word.lower():
             return ItemNameCategoryList.SOYBEANS.value
 
 class GroCropClient(object):
 
-    def __init__(self, api_host=API_HOST, access_token=None):
+    def __init__(self, api_host=API_HOST, access_token=None, proxy_host=None, proxy_port=None,
+                 proxy_username=None, proxy_pass=None):
         """Construct a GroCropClient instance.
         Parameters
         ----------
         api_host : string, optional
             api_host : string
             The API host's url, excluding 'https://', to be consistent with groclient/lib.py
             ex. 'api.gro-intelligence.com'
         access_token : string, optional
             Your Gro API authentication token. If not specified, the
             :code:`$GROAPI_TOKEN` environment variable is used. See
             :doc:`authentication`.
+        proxy_host : string, optional
+            If you're instantiating the GroCropClient behind a proxy, you'll need to 
+            provide the proxy_host to properly send requests using the groclient 
+            library.
+        proxy_port : int, optional
+            If you're instantiating the GroCropClient behind a proxy, you'll need to 
+            provide the proxy_port to properly send requests using the groclient 
+            library.
+        proxy_username : string, optional 
+            If you're instantiating the GroCropClient behind a proxy, and your proxy 
+            requires a username and password, you'll need to provide the proxy_username.
+        proxy_pass : string optional
+            Password for your proxy username.
+        
         Raises
         ------
             RuntimeError
                 Raised when neither the :code:`access_token` parameter nor
                 :code:`$GROAPI_TOKEN` environment variable are set.
         Examples
         --------
@@ -99,15 +114,25 @@
         if access_token is None:
             access_token = os.environ.get("GROAPI_TOKEN")
             if access_token is None:
                 raise RuntimeError("GROAPI_TOKEN environment variable must be set when "
                                    "Your Gro Client is constructed without the access_token argument")
         self._api_host = api_host
         self._access_token = access_token
-        self._client = GroClient(self._api_host, self._access_token)
+        self._proxy_host = proxy_host
+        self._proxy_port = proxy_port
+        self._proxy_username = proxy_username
+        self._proxy_pass = proxy_pass
+
+        self._client = GroClient(api_host = self._api_host, 
+                                 access_token = self._access_token, 
+                                 proxy_host = self._proxy_host,
+                                 proxy_port = self._proxy_port,
+                                 proxy_username = self._proxy_username,
+                                 proxy_pass = self._proxy_pass)
 
     def get_sources(self):
         """Returns a list of all US Crop sources, as JSON.
             The schema for our US crop sources is:
             ['description',
             'fileFormat',
             'historicalStartDate',
```

### Comparing `grocropclient-1.0.8/pyproject.toml` & `grocropclient-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grocropclient"
-version = "1.0.8"
+version = "1.0.9"
 description = "Python client library for accessing Gro Intelligence's US crop insights"
 authors = ["Gro Intelligence developers <dev@gro-intelligence.com>"]
 readme = "README.md"
 homepage = "https://www.gro-intelligence.com"
 repository = ""
 documentation = ""
 license = "MIT"
```

### Comparing `grocropclient-1.0.8/setup.py` & `grocropclient-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['fuzzywuzzy', 'groclient', 'numpy', 'pandas']
 
 setup_kwargs = {
     'name': 'grocropclient',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': "Python client library for accessing Gro Intelligence's US crop insights",
     'long_description': 'The Gro US Crop API Client is a Python library to help with the discovery and retrieval of data series related to US crops.\n\nThe library is written on top of the [Gro Python Client API](https://github.com/gro-intelligence/api-client)\nand offers a set of convenience methods and constants to make the use of the Gro API faster and simpler.\n\nThe use of the Gro US Crop API Client requires a Gro account with API access.\nVisit our [website](https://gro-intelligence.com/platform/api) for more information.\n',
     'author': 'Gro Intelligence developers',
     'author_email': 'dev@gro-intelligence.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.gro-intelligence.com',
```

### Comparing `grocropclient-1.0.8/PKG-INFO` & `grocropclient-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grocropclient
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python client library for accessing Gro Intelligence's US crop insights
 Home-page: https://www.gro-intelligence.com
 License: MIT
 Author: Gro Intelligence developers
 Author-email: dev@gro-intelligence.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

