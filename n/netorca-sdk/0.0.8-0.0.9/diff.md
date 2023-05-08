# Comparing `tmp/netorca_sdk-0.0.8.tar.gz` & `tmp/netorca_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netorca_sdk-0.0.8.tar", last modified: Wed Feb 15 15:44:15 2023, max compression
+gzip compressed data, was "netorca_sdk-0.0.9.tar", last modified: Fri Feb 17 16:35:21 2023, max compression
```

## Comparing `netorca_sdk-0.0.8.tar` & `netorca_sdk-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:44:15.543969 netorca_sdk-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-02-15 15:43:47.000000 netorca_sdk-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      707 2023-02-15 15:44:15.542969 netorca_sdk-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-02-15 15:43:47.000000 netorca_sdk-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:44:15.542969 netorca_sdk-0.0.8/netorca_sdk/
--rw-rw-rw-   0 root         (0) root         (0)     5467 2023-02-15 15:43:47.000000 netorca_sdk-0.0.8/netorca_sdk/auth.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-15 15:43:47.000000 netorca_sdk-0.0.8/netorca_sdk/config.py
--rw-rw-rw-   0 root         (0) root         (0)     8180 2023-02-15 15:43:47.000000 netorca_sdk-0.0.8/netorca_sdk/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-02-15 15:43:47.000000 netorca_sdk-0.0.8/netorca_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:44:15.542969 netorca_sdk-0.0.8/netorca_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      707 2023-02-15 15:44:15.000000 netorca_sdk-0.0.8/netorca_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      307 2023-02-15 15:44:15.000000 netorca_sdk-0.0.8/netorca_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 15:44:15.000000 netorca_sdk-0.0.8/netorca_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-15 15:44:15.000000 netorca_sdk-0.0.8/netorca_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-15 15:44:15.000000 netorca_sdk-0.0.8/netorca_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-02-15 15:43:47.000000 netorca_sdk-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 15:44:15.543969 netorca_sdk-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-02-15 15:43:47.000000 netorca_sdk-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 16:35:21.404152 netorca_sdk-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      657 2023-02-17 16:35:21.404152 netorca_sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 16:35:21.404152 netorca_sdk-0.0.9/netorca_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8978 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9332 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/serviceowner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 16:35:21.404152 netorca_sdk-0.0.9/netorca_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      657 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      335 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-17 16:35:21.405153 netorca_sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/setup.py
```

### Comparing `netorca_sdk-0.0.8/LICENSE` & `netorca_sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netorca_sdk-0.0.8/PKG-INFO` & `netorca_sdk-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: netorca_sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
```

### Comparing `netorca_sdk-0.0.8/netorca_sdk/auth.py` & `netorca_sdk-0.0.9/netorca_sdk/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import requests
 
 from netorca_sdk.config import RETRY_TIMES, AUTH_ENDPOINT, TEAM_ENDPOINT
 from netorca_sdk.exceptions import NetorcaException
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
+
 class AbstractNetorcaAuth(ABC):
     @abstractmethod
     def get(self, *args, **kwargs):
         ...
 
     @abstractmethod
     def post(self, *args, **kwargs):
```

### Comparing `netorca_sdk-0.0.8/netorca_sdk/consumer.py` & `netorca_sdk-0.0.9/netorca_sdk/consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,28 @@
-"""
-- Config check
-- YAML Linting
-- get team
-- Submit for Validation
-"""
 import json
 import os
 from typing import Tuple
 
 import yaml
-from prettytable import PrettyTable, ALL
+from beautifultable import BeautifulTable
 
 from netorca_sdk.auth import AbstractNetorcaAuth, NetorcaAuth
 from netorca_sdk.config import VALIDATE_CONSUMER_REQUEST_ENDPOINT, SUBMIT_CONSUMER_REQUEST_ENDPOINT
 from netorca_sdk.exceptions import NetorcaException
 
 
 class ConsumerRequest:
     def __init__(self, netorca_api_key: str):
         self.netorca_api_key = netorca_api_key
 
         self.config = None
         self.consumer_request = None
         self.auth = None
-        
-    def load_from_repository(self, repository_path: str) -> Tuple[bool, str]:
+
+    def load_from_repository(self, repository_path: str) -> None:
         """
             Check if valid and load request and config from consumer's repository.
             Repository must contain `.netorca` directory and `config.yaml` file.
             Note: Only one allowed extensions in `.netorca` directory is `*.yaml`
 
             Args:
                 repository_path: str    path to consumer repository
@@ -54,15 +48,15 @@
                     raise NetorcaException(
                         "No `netorca_global.base_url` provided.")
 
                 self.config = config
                 self.auth = self.get_auth()
             except yaml.YAMLError as exc:
                 raise NetorcaException(
-                    f"Error while parsing file: `{filename}`. Exception: {exc.problem}")
+                    f"Error while parsing file: `config.yml`. Exception: {exc.problem}")
 
         _tmp_consumer_request = {}
         # check and load consumer request
         for filename in os.listdir(dotnetorca_path):
             if filename == "config.yaml":
                 continue
 
@@ -82,15 +76,15 @@
                 for key in app.keys():
                     if key in _tmp_consumer_request:
                         raise NetorcaException(
                             f"Application with name `{key}` already exists in different `.yaml` declaration.")
 
                 _tmp_consumer_request.update(app)
         self.consumer_request = _tmp_consumer_request
-        
+
     def get_auth(self) -> AbstractNetorcaAuth:
         if not self.config:
             raise NetorcaException(f"Cannot authenticate before loading repository config.")
 
         netorca_fqdn = self.config.get("netorca_global", {}).get("base_url")
         self.auth = NetorcaAuth(fqdn=netorca_fqdn, api_key=self.netorca_api_key)
         return self.auth
@@ -126,74 +120,94 @@
                 Tuple[bool, str]    ->  is_valid, validation_errors
         """
         if not (self.config and self.consumer_request and self.auth):
             raise NetorcaException(f"Use `load_from_repository(repository_path)` method to load configuration.")
         VALIDATE_REQUEST_PATH = f"{self.auth.fqdn}{VALIDATE_CONSUMER_REQUEST_ENDPOINT}"
         full_request = self.prepare_request()
 
-        response = self.auth.post(url=VALIDATE_REQUEST_PATH, data=json.dumps(full_request), authentication_required=True)
+        response = self.auth.post(url=VALIDATE_REQUEST_PATH, data=json.dumps(full_request),
+                                  authentication_required=True)
 
         response = response.json()
         if response.get("is_valid"):
             return True, {}
-
         errors = response.get("errors")
+
         if pretty_print:
             ConsumerRequest.pretty_print_errors(errors)
         return False, errors
 
     def submit(self) -> Tuple[bool, str]:
         """
             Validate and submit consumer request.
             NOTE: Data must be first imported with `load_from_repository` method
 
             Returns:
-                bool    ->  submisson successful
+                bool, str    ->  submission successful, submission messages
         """
         is_valid = self.validate(pretty_print=True)
         if not is_valid[0]:
             return False, "Consumer request is invalid and cannot be submitted."
-            
+
         SUBMIT_REQUEST_PATH = f"{self.auth.fqdn}{SUBMIT_CONSUMER_REQUEST_ENDPOINT}"
         full_request = self.prepare_request()
-        response = self.auth.post(url=SUBMIT_REQUEST_PATH, data=json.dumps(full_request), authentication_required=True)
+        response = self.auth.post(url=SUBMIT_REQUEST_PATH, data=json.dumps(full_request),
+                                  authentication_required=True)
         if response.status_code == 201:
             return True, "Submitted successfuly."
         return False, response.text
 
-
     @staticmethod
     def pretty_print_errors(errors: dict) -> None:
         """
             Pretty print errors
-
             #TODO: this should be refactored to cleaner code (probably recursive)
         """
-        table = PrettyTable()
-        table.field_names = ["Team", "Application",
-                             "Service", "Field", "Reason"]
-        table.hrules = ALL
+
+        table = BeautifulTable(maxwidth=100)
+        table.set_style(BeautifulTable.STYLE_SEPARATED)
+        table.columns.header = ["Team", "Field", "Reason"]
         for item1, value1 in errors.items():
-            table.add_row([item1, "", "", "", ""])
             if isinstance(value1, str) or isinstance(value1, list):
-                table.add_row([item1, "", "", "", value1])
+                table.rows.append([item1, "", value1])
             elif isinstance(value1, dict):
                 for item2, value2 in value1.items():
                     if isinstance(value2, str) or isinstance(value2, list):
-                        table.add_row([item1, "", "", item2, value2])
-                    elif isinstance(value2, dict):
-                        table.add_row(["", item2, "", "", ""])
+                        table.rows.append([item1, item2, value2])
+
+                        if table.rows:
+                            print("-" * 100)
+                            print(f"Team: {item1} validation errors")
+                            print("-" * 100)
+                            print(table)
+                            print()
+                        break
+
+        for item1, value1 in errors.items():
+            if isinstance(value1, dict):
+                for item2, value2 in value1.items():
+                    table = BeautifulTable(maxwidth=100)
+                    table.set_style(BeautifulTable.STYLE_SEPARATED)
+                    table.columns.header = ["Application", "Service", "ServiceItem", "Field", "Reason"]
+
+                    if isinstance(value2, dict):
                         for item3, value3 in value2.items():
-                            if isinstance(value3, str) or isinstance(value3, list):
-                                table.add_row(["", item2, "", item3, value3])
+                            if isinstance(value3, str):
+                                table.rows.append([item2, "", "", item3, value3])
+                            elif isinstance(value3, list):
+                                for err in value3:
+                                    table.rows.append([item2, "", "", item3, err])
                             elif isinstance(value3, dict):
                                 for item4, value4 in value3.items():
                                     if isinstance(value4, str) or isinstance(value4, list):
-                                        table.add_row(
-                                            ["", "", item3, item4, value4])
+                                        table.rows.append(["", item3, "", item4, value4])
                                     elif isinstance(value4, dict):
-                                        table.add_row(["", "", item4, "", ""])
                                         for item5, value5 in value4.items():
                                             if isinstance(value5, str) or isinstance(value5, list):
-                                                table.add_row(
-                                                    ["", "", "", item5, value5])
-        print(table)
+                                                table.rows.append(["", item3, item4, item5, value5])
+
+                        if table.rows:
+                            print("-" * 100)
+                            print(f"Application: `{item2}` validation errors")
+                            print("-" * 100)
+                            print(table)
+                            print()
```

### Comparing `netorca_sdk-0.0.8/netorca_sdk.egg-info/PKG-INFO` & `netorca_sdk-0.0.9/netorca_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: netorca-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
```

### Comparing `netorca_sdk-0.0.8/setup.py` & `netorca_sdk-0.0.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from distutils.core import setup
+
 setup(
-  name = 'netorca_sdk',
-  packages = ['netorca_sdk'],
-  version = '0.0.8',
-  license='MIT',
-  description = 'A package for interacting with the NetOrca API',
-  author = 'Scott Rowlandson',
-  author_email = 'scott@netautomate.org',
-  url = 'https://gitlab.com/netorca_public/netorca_sdk/',
-  keywords = ['netorca', 'orchestration', 'netautomate'],
-  install_requires=[
-          'requests', 'prettytable', 'pyyaml'
-      ],
-  classifiers=[
-    'Development Status :: 3 - Alpha',
-    'Intended Audience :: Developers',
-    'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-  ],
-)
+    name='netorca_sdk',
+    packages=['netorca_sdk'],
+    version='0.0.9',
+    license='MIT',
+    description='A package for interacting with the NetOrca API',
+    author='Scott Rowlandson',
+    author_email='scott@netautomate.org',
+    url='https://gitlab.com/netorca_public/netorca_sdk/',
+    keywords=['netorca', 'orchestration', 'netautomate'],
+    install_requires=[
+        'beautifultable',
+        'pyyaml',
+        'requests',
+    ],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ],
+)
```

