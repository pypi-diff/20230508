# Comparing `tmp/dapla_statbank_client-1.0.2.tar.gz` & `tmp/dapla_statbank_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_statbank_client-1.0.2.tar", max compression
+gzip compressed data, was "dapla_statbank_client-1.0.4.tar", max compression
```

## Comparing `dapla_statbank_client-1.0.2.tar` & `dapla_statbank_client-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-04-13 09:20:19.222743 dapla_statbank_client-1.0.2/LICENSE
--rw-r--r--   0        0        0     8938 2023-04-13 09:20:37.138836 dapla_statbank_client-1.0.2/README.md
--rw-r--r--   0        0        0     1119 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      190 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/__init__.py
--rw-r--r--   0        0        0     5651 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/apidata.py
--rw-r--r--   0        0        0     3668 2023-04-13 09:20:19.226743 dapla_statbank_client-1.0.2/statbank/auth.py
--rw-r--r--   0        0        0    17539 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/client.py
--rw-r--r--   0        0        0    13609 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/transfer.py
--rw-r--r--   0        0        0    13611 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/uttrekk.py
--rw-r--r--   0        0        0    14153 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/uttrekk_validations.py
--rw-r--r--   0        0        0     9637 1970-01-01 00:00:00.000000 dapla_statbank_client-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/LICENSE
+-rw-r--r--   0        0        0     9087 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/README.md
+-rw-r--r--   0        0        0     1119 2023-05-08 06:04:56.424735 dapla_statbank_client-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      206 2023-05-08 06:04:56.424735 dapla_statbank_client-1.0.4/statbank/__init__.py
+-rw-r--r--   0        0        0     5651 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/statbank/apidata.py
+-rw-r--r--   0        0        0     3668 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/statbank/auth.py
+-rw-r--r--   0        0        0    17571 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/statbank/client.py
+-rw-r--r--   0        0        0    13617 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/statbank/transfer.py
+-rw-r--r--   0        0        0    13722 2023-05-08 06:04:34.728356 dapla_statbank_client-1.0.4/statbank/uttrekk.py
+-rw-r--r--   0        0        0    14153 2023-05-08 06:04:34.728356 dapla_statbank_client-1.0.4/statbank/uttrekk_validations.py
+-rw-r--r--   0        0        0     9786 1970-01-01 00:00:00.000000 dapla_statbank_client-1.0.4/PKG-INFO
```

### Comparing `dapla_statbank_client-1.0.2/LICENSE` & `dapla_statbank_client-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.2/README.md` & `dapla_statbank_client-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 filbesk_06339_new = stat_client.read_description_json("path.json")
 ```
 Some deeper data-structures, like the dataframes in the transfer will not be serialized and stored with the transfer-object in its json.
 
 ---
 
 ### Version history
+- 1.0.3 Fixing bug where empty codelists stops description initialization, Updating pyjstat to 2.4.0, changing imports to absolute from package root
 - 1.0.2 Doc-string style cleanup, a check on username and password on client init, changes to time and display of time, demo notebooks cleaned
 - 1.0.0 Finished going through initial issues, less complaining from verify on floats
 - 0.0.11 Statbank people wanted a user-agent-requesst-header to differentiate test from prod
 - 0.0.9 After further user-testing and requests
 - 0.0.5 Still some parameter issues
 - 0.0.4 More test coverage, some bugs fixed in rounding checks and parameter-passing
 - 0.0.3 Removed batches, stripping uttrekk from transfer, rounding function on uttrekk, data required in as a dict of dataframes, with "deltabell-navn". Tableid now works to transfer to instead of only "hovedtabellnavn"
```

### Comparing `dapla_statbank_client-1.0.2/pyproject.toml` & `dapla_statbank_client-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "dapla-statbank-client"
-version = "1.0.2"
+version = "1.0.4"
 description = "Handles data transfer Statbank <-> Dapla for Statistics Norway"
 authors = ["Statistics Norway", "Carl F. Corneil <cfc@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "statbank"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^1.5.0"
 dapla-toolbelt = "^1.3.3"
 requests = "^2.28.1"
-pyjstat = "^2.3.0"
 ipywidgets = "^8.0.2"
 IPython = "^8.5.0"
+pyjstat = "^2.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.1.3"
 pre-commit = "^2.20.0"
 autoflake = "^1.7.6"
 pep8-naming = "^0.13.2"
 pyupgrade = "^3.1.0"
```

### Comparing `dapla_statbank_client-1.0.2/statbank/apidata.py` & `dapla_statbank_client-1.0.4/statbank/apidata.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.2/statbank/auth.py` & `dapla_statbank_client-1.0.4/statbank/auth.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.2/statbank/client.py` & `dapla_statbank_client-1.0.4/statbank/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import os
 from datetime import timedelta as td
 
 import ipywidgets as widgets
 import pandas as pd
 from IPython.display import display
 
-from .apidata import apidata, apidata_all, apidata_rotate
-from .auth import StatbankAuth
-from .transfer import StatbankTransfer
-from .uttrekk import StatbankUttrekksBeskrivelse
+from statbank.apidata import apidata, apidata_all, apidata_rotate
+from statbank.auth import StatbankAuth
+from statbank.transfer import StatbankTransfer
+from statbank.uttrekk import StatbankUttrekksBeskrivelse
 
 
 TOMORROW = datetime.datetime.now() + td(days=1)
 
 
 class StatbankClient(StatbankAuth):
     """
```

### Comparing `dapla_statbank_client-1.0.2/statbank/transfer.py` & `dapla_statbank_client-1.0.4/statbank/transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import urllib
 from datetime import datetime as dt
 from datetime import timedelta as td
 
 import pandas as pd
 import requests as r
 
-from .auth import StatbankAuth
+from statbank.auth import StatbankAuth
 
 
 class StatbankTransfer(StatbankAuth):
     """
     Class for talking with the "transfer-API",
     which actually recieves the data from the user and sends it to Statbank.
     ...
```

### Comparing `dapla_statbank_client-1.0.2/statbank/uttrekk.py` & `dapla_statbank_client-1.0.4/statbank/uttrekk.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import json
 from decimal import ROUND_HALF_UP, Decimal, localcontext
 
 import pandas as pd
 import requests as r
 from requests.exceptions import ConnectionError
 
-from .auth import StatbankAuth
-from .uttrekk_validations import StatbankUttrekkValidators
+from statbank.auth import StatbankAuth
+from statbank.uttrekk_validations import StatbankUttrekkValidators
 
 
 class StatbankUttrekksBeskrivelse(StatbankAuth, StatbankUttrekkValidators):
     """
     Class for talking with the "uttrekksbeskrivelses-API",
     which describes metadata about shape of data to be transferred.
     And metadata about the table itself in Statbankens system,
@@ -311,20 +311,21 @@
         self.tableid = self.filbeskrivelse["TabellId"]
         self.tablename = self.filbeskrivelse["Huvudtabell"]
         self.subtables = {
             x["Filnavn"]: x["Filtext"] for x in self.filbeskrivelse["DeltabellTitler"]
         }
         self.variables = self.filbeskrivelse["deltabller"]
         self.codelists = {}
-        for kodeliste in self.filbeskrivelse["kodelister"]:
-            new_kodeliste = {}
-            for kode in kodeliste["koder"]:
-                new_kodeliste[kode["kode"]] = kode["text"]
-            self.codelists[kodeliste["kodeliste"]] = {"koder": new_kodeliste}
-            remain_keys = list(kodeliste.keys())
-            remain_keys.remove("koder")
-            remain_keys.remove("kodeliste")
-            for k in remain_keys:
-                self.codelists[kodeliste["kodeliste"]][k] = kodeliste[k]
+        if "kodelister" in self.filbeskrivelse.keys():
+            for kodeliste in self.filbeskrivelse["kodelister"]:
+                new_kodeliste = {}
+                for kode in kodeliste["koder"]:
+                    new_kodeliste[kode["kode"]] = kode["text"]
+                self.codelists[kodeliste["kodeliste"]] = {"koder": new_kodeliste}
+                remain_keys = list(kodeliste.keys())
+                remain_keys.remove("koder")
+                remain_keys.remove("kodeliste")
+                for k in remain_keys:
+                    self.codelists[kodeliste["kodeliste"]][k] = kodeliste[k]
 
         if "null_prikk_missing_kodeliste" in self.filbeskrivelse.keys():
             self.suppression = self.filbeskrivelse["null_prikk_missing_kodeliste"]
```

### Comparing `dapla_statbank_client-1.0.2/statbank/uttrekk_validations.py` & `dapla_statbank_client-1.0.4/statbank/uttrekk_validations.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.2/PKG-INFO` & `dapla_statbank_client-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dapla-statbank-client
-Version: 1.0.2
+Version: 1.0.4
 Summary: Handles data transfer Statbank <-> Dapla for Statistics Norway
 License: MIT
 Author: Statistics Norway
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: IPython (>=8.5.0,<9.0.0)
 Requires-Dist: dapla-toolbelt (>=1.3.3,<2.0.0)
 Requires-Dist: ipywidgets (>=8.0.2,<9.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
-Requires-Dist: pyjstat (>=2.3.0,<3.0.0)
+Requires-Dist: pyjstat (>=2.4.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # dapla-statbank-client
 Used internally by SSB (Statistics Norway).
 Validates and transfers data from Dapla to Statbank.
 Gets data from public and internal statbank.
@@ -145,14 +145,15 @@
 filbesk_06339_new = stat_client.read_description_json("path.json")
 ```
 Some deeper data-structures, like the dataframes in the transfer will not be serialized and stored with the transfer-object in its json.
 
 ---
 
 ### Version history
+- 1.0.3 Fixing bug where empty codelists stops description initialization, Updating pyjstat to 2.4.0, changing imports to absolute from package root
 - 1.0.2 Doc-string style cleanup, a check on username and password on client init, changes to time and display of time, demo notebooks cleaned
 - 1.0.0 Finished going through initial issues, less complaining from verify on floats
 - 0.0.11 Statbank people wanted a user-agent-requesst-header to differentiate test from prod
 - 0.0.9 After further user-testing and requests
 - 0.0.5 Still some parameter issues
 - 0.0.4 More test coverage, some bugs fixed in rounding checks and parameter-passing
 - 0.0.3 Removed batches, stripping uttrekk from transfer, rounding function on uttrekk, data required in as a dict of dataframes, with "deltabell-navn". Tableid now works to transfer to instead of only "hovedtabellnavn"
```

