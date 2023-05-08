# Comparing `tmp/sheetcloud-0.1.0.post8.tar.gz` & `tmp/sheetcloud-0.1.0.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheetcloud-0.1.0.post8.tar", last modified: Fri May  5 13:28:32 2023, max compression
+gzip compressed data, was "sheetcloud-0.1.0.post9.tar", last modified: Mon May  8 07:59:26 2023, max compression
```

## Comparing `sheetcloud-0.1.0.post8.tar` & `sheetcloud-0.1.0.post9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.402811 sheetcloud-0.1.0.post8/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-05 13:28:32.398810 sheetcloud-0.1.0.post8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.394811 sheetcloud-0.1.0.post8/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/resources/endpoints.v1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/resources/template_red_sailfish.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:28:32.402811 sheetcloud-0.1.0.post8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.398810 sheetcloud-0.1.0.post8/sheetcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.398810 sheetcloud-0.1.0.post8/sheetcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.398810 sheetcloud-0.1.0.post8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/tests/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/tests/test_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:59:26.370483 sheetcloud-0.1.0.post9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-08 07:59:26.370483 sheetcloud-0.1.0.post9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:59:26.370483 sheetcloud-0.1.0.post9/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/resources/endpoints.v1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/resources/template_red_sailfish.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:59:26.370483 sheetcloud-0.1.0.post9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:59:26.370483 sheetcloud-0.1.0.post9/sheetcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/sheetcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:59:26.370483 sheetcloud-0.1.0.post9/sheetcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-08 07:59:26.000000 sheetcloud-0.1.0.post9/sheetcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 07:59:26.000000 sheetcloud-0.1.0.post9/sheetcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:59:26.000000 sheetcloud-0.1.0.post9/sheetcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 07:59:26.000000 sheetcloud-0.1.0.post9/sheetcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 07:59:26.000000 sheetcloud-0.1.0.post9/sheetcloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:59:26.370483 sheetcloud-0.1.0.post9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/tests/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 07:58:02.000000 sheetcloud-0.1.0.post9/tests/test_orm.py
```

### Comparing `sheetcloud-0.1.0.post8/LICENSE` & `sheetcloud-0.1.0.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post8/PKG-INFO` & `sheetcloud-0.1.0.post9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheetcloud
-Version: 0.1.0.post8
+Version: 0.1.0.post9
 Summary: Sheetcloud.de | Turn Spreadsheets into a Cloud Database | Account required
 Author-email: "sheetcloud.org" <contact@sheetcloud.org>
 Project-URL: Homepage, https://www.sheetcloud.org
 Project-URL: Tracker, https://github.com/sheetcloud/sheetcloud/issues
 Project-URL: Source, https://github.com/sheetcloud/sheetcloud
 Project-URL: Examples, https://github.com/sheetcloud
 Keywords: Spreadsheets,RAD,Database,Cloud
```

### Comparing `sheetcloud-0.1.0.post8/README.md` & `sheetcloud-0.1.0.post9/README.md`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post8/pyproject.toml` & `sheetcloud-0.1.0.post9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post8/resources/template_red_sailfish.json` & `sheetcloud-0.1.0.post9/resources/template_red_sailfish.json`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post8/sheetcloud/conn.py` & `sheetcloud-0.1.0.post9/sheetcloud/conn.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 import requests
 
 from typing import *
 
 from sheetcloud.utils import pw_obfuscator
 
 
+ENV_SHEETCLOUD_API_URL = os.environ.get('SHEETCLOUD_API_URL', 'https://api.sheetcloud.de')
 ENV_SHEETCLOUD_USERNAME = os.environ.get('SHEETCLOUD_USERNAME', 'missing')
 ENV_SHEETCLOUD_PASSWORD = os.environ.get('SHEETCLOUD_PASSWORD', 'missing')
-ENV_SHEETCLOUD_LICENSE = os.environ.get('SHEETCLOUD_LICENSE', 'missing')
+ENV_SHEETCLOUD_LICENSE = os.environ.get('SHEETCLOUD_LICENSE', None)
 
 
 ENV_SHEETCLOUD_DEV = str(os.environ.get('SHEETCLOUD_DEV', 'False')).strip().lower() == 'true'
-if ENV_SHEETCLOUD_DEV:
-    SHEETCLOUD_API_URL = 'https://localhost:8080'
-    logger.debug(f'Development mode enabled. API is now {SHEETCLOUD_API_URL}.')
-else:
-    SHEETCLOUD_API_URL = 'https://api.sheetcloud.de'
+if ENV_SHEETCLOUD_DEV is not None:
+    logger.debug(f'Development mode enabled. API is {ENV_SHEETCLOUD_API_URL}.')
+
 
 logger.info(f'Environment variable SHEETCLOUD_USERNAME is {ENV_SHEETCLOUD_USERNAME}.')
 logger.info(f'Environment variable SHEETCLOUD_PASSWORD is {pw_obfuscator(ENV_SHEETCLOUD_PASSWORD, "missing")}.')
-logger.info(f'(Optional) Environment variable SHEETCLOUD_LICENSE is {pw_obfuscator(ENV_SHEETCLOUD_LICENSE, "missing")}.')
+if ENV_SHEETCLOUD_LICENSE is not None:
+    logger.info(f'(Optional) Environment variable SHEETCLOUD_LICENSE is {pw_obfuscator(ENV_SHEETCLOUD_LICENSE, "missing")}.')
 
 _sheetcloud_auth_token: str = None
 
 
 class SheetcloudAuthorizationFailed(Exception):
     msg = """ Raised when authorization failed. Please check your user name and password as well as your internet connection. """
     def __str__(self) -> str:
@@ -58,17 +58,17 @@
     
     payload = None
     if data is not None:
         payload = json.dumps(data)
 
     while num_retries > 0:
         if method == 'post':
-            response = requests.post(f'{SHEETCLOUD_API_URL}{path}', data=payload, params=params, files=files, headers=headers, timeout=100, verify=not ENV_SHEETCLOUD_DEV)
+            response = requests.post(f'{ENV_SHEETCLOUD_API_URL}{path}', data=payload, params=params, files=files, headers=headers, timeout=100, verify=not ENV_SHEETCLOUD_DEV)
         else:
-            response = requests.get(f'{SHEETCLOUD_API_URL}{path}', data=payload, params=params, files=files, headers=headers, timeout=100, verify=not ENV_SHEETCLOUD_DEV)
+            response = requests.get(f'{ENV_SHEETCLOUD_API_URL}{path}', data=payload, params=params, files=files, headers=headers, timeout=100, verify=not ENV_SHEETCLOUD_DEV)
 
         if response.status_code in [401, 404]:
             logger.debug('Request new authorization token.')
             _sheetcloud_auth_token = request_auth_token()
             if _sheetcloud_auth_token is None:
                 raise SheetcloudAuthorizationFailed()
             headers['Authorization'] = f'Bearer {_sheetcloud_auth_token}'
@@ -98,15 +98,15 @@
 
 def request_auth_token(num_retries: int=3) -> Optional[str]:
     headers = {
         'accept': 'application/json', 
         'Content-Type': 'application/x-www-form-urlencoded'}
     data = f'grant_type=&username={ENV_SHEETCLOUD_USERNAME}&password={ENV_SHEETCLOUD_PASSWORD}&scope=&client_id=&client_secret='
     while num_retries > 0:
-        response = requests.post(f'{SHEETCLOUD_API_URL}/token', data, headers=headers, timeout=100, verify=not ENV_SHEETCLOUD_DEV)
+        response = requests.post(f'{ENV_SHEETCLOUD_API_URL}/token', data, headers=headers, timeout=100, verify=not ENV_SHEETCLOUD_DEV)
         if response.status_code == 200:
             response_data_dict = response.json()
             access_token = response_data_dict['access_token']
             return access_token
         else:
             if response.status_code == 401:
                 logger.error(f'Authorization failed. Check your user name and password again.')
```

### Comparing `sheetcloud-0.1.0.post8/sheetcloud/drive.py` & `sheetcloud-0.1.0.post9/sheetcloud/drive.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,82 @@
 import logging
 logger = logging.getLogger('SHEETCLOUD DRIVE')
 logging.basicConfig(format='\x1b[38;5;224m %(levelname)8s \x1b[0m | \x1b[38;5;39m %(name)s \x1b[0m | %(message)s', level=logging.DEBUG)
 
 import io
-import json
 import pandas as pd
 
-from datetime import datetime
 from typing import *
 
 from sheetcloud.conn import service
 
 
+
 def list_my_csvs() -> List[Dict]:
+    """ Returns a list of dict containing properties of all CSVs in the target account.
+        Properties:
+        - mimeType: str
+        - parents (List of ids)
+        - size 
+        - id
+        - name
+        - modifiedTime
+        - url
+
+    Returns:
+        List[Dict]: List of CSV properties
+    """
     res = service('/drive/list/csv', method='post')
     if 'csvs' in res:
         logger.info(f'List contains a total of {len(res["csvs"])} CSVs.')
         return res['csvs']
     return list()
 
 
 def read_csv(file_id: str) -> pd.DataFrame:
+    """ Read a specific CSV file with ID `file_id`.
+
+    Args:
+        file_id (str): The id of the CSV file to read.
+
+    Returns:
+        pd.DataFrame: DataFrame containing the data of the CSV file.
+    """
     headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/octet-stream',
     }
     params = {'file_id': file_id}
     content = service('/drive/read/csv', params=params, headers=headers, method='post', return_dict=False)
     df = pd.read_parquet(io.BytesIO(content), engine='pyarrow', use_nullable_dtypes=True)
     return df
 
 
-def write_csv(name: str, df: pd.DataFrame, cache: bool=True) -> None:
+def write_csv(name: str, df: pd.DataFrame) -> None:
+    """ Write a pandas DataFrame to a CSV file with name `name` in the target account.
+
+    Args:
+        name (str): Name of the file (not ID)
+        df (pd.DataFrame): DataFrame containing the data.
+    """
     with io.BytesIO() as memory_buffer:
         df.to_parquet(
             memory_buffer,
             compression='gzip',
             engine='pyarrow'
         )
         memory_buffer.seek(0)
         # need to send files separately
         files = {
             'file': ('Test', memory_buffer, 'application/octet-stream')
         }
         params = {'name': name}
         endpoint = '/drive/write/csv'
-        resp = service(endpoint, params=params, files=files, method='post')
-        print(resp)
+        _ = service(endpoint, params=params, files=files, method='post')
+        
 
 
 
 
 if __name__ == "__main__":
     print('Start connecting...')
     print(list_my_csvs())
```

### Comparing `sheetcloud-0.1.0.post8/sheetcloud/env.py` & `sheetcloud-0.1.0.post9/sheetcloud/env.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post8/sheetcloud/fun.py` & `sheetcloud-0.1.0.post9/sheetcloud/fun.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 from typing import *
 
 from sheetcloud import sheets
 from sheetcloud import templates
 
 
+def there_is_no_fun_here_yet():
+    raise Exception('Ohhhhhh, no fun :(')
+
 # def write_image(sheet_url_or_name: str, worksheet_name: str, img, cache: bool=True) -> None:
 
 #     sheets.write(sheet_url_or_name, worksheet_name, df, cache=cache)
 
 #     fmts = [('A:A', {'width': 250}), ('B:B', {'width': 500}), ('A1:B1', formats.header_blue), ('A2:A', formats.index_column_blue)]
 #     sheets.format_spreadsheet(sheet_url_or_name, worksheet_name, a1range_format_list=fmts, auto_resize=False)
```

### Comparing `sheetcloud-0.1.0.post8/sheetcloud/orm.py` & `sheetcloud-0.1.0.post9/sheetcloud/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     module = cls.__module__
     name = cls.__qualname__
     if module is not None and module != "__builtin__":
         name = module + "." + name
     return name
 
 
-def build_object(class_name: str, content: Dict, name_to_class: Dict) -> Any:
+def _build_object(class_name: str, content: Dict, name_to_class: Dict) -> Any:
     obj = None
     my_cls = name_to_class.get(class_name, None)
     if my_cls is not None:
         decoded_params = dict()
         for k, v in content.items():
             if v is not None:
                 decoded_params[k] = json.loads(v)
@@ -36,21 +36,21 @@
         obj = my_cls(**decoded_params)
     return obj
 
 
 def read(sheet_url_or_name: str, prefix_id: str, classes: List[Any], cache: bool=True) -> Optional[List]:
     res = None
     try:
-        res = build_dc_list_from_sheets(sheet_url_or_name=sheet_url_or_name, prefix_id=prefix_id, classes=classes, cache=cache)
+        res = _build_dc_list_from_sheets(sheet_url_or_name=sheet_url_or_name, prefix_id=prefix_id, classes=classes, cache=cache)
     except BaseException as e:
         logger.error(f'There was a problem loading {prefix_id} worksheets from {sheet_url_or_name} and building the list of dataclasses. Please double check the inputs and consult the documentation in order to not run into limitations.')
     return res
 
 
-def build_dc_list_from_sheets(sheet_url_or_name: str, prefix_id: str, classes: List[Any], cache: bool=True) -> Optional[List]:
+def _build_dc_list_from_sheets(sheet_url_or_name: str, prefix_id: str, classes: List[Any], cache: bool=True) -> Optional[List]:
     name_to_class = dict()
     for c in classes:
         name_to_class[c.__name__] = c
 
     names = sheets.list_worksheets_in_spreadsheet(sheet_url_or_name)
 
     query_by_uuid = dict()
@@ -63,15 +63,15 @@
             for i in range(df.shape[0]):
                 content = df.iloc[i].to_dict()
                 uuid = content.pop('uuid', None)
                 parent_uuid = content.pop('parent_uuid', None)
                 parent_field = content.pop('parent_field', None)
                 parent_class = content.pop('parent_class', None)
         
-                obj = build_object(class_name, content, name_to_class)
+                obj = _build_object(class_name, content, name_to_class)
         
                 query_by_uuid[uuid] = obj
                 if parent_uuid not in query_by_parent_uuuid_and_field:
                     query_by_parent_uuuid_and_field[parent_uuid] = dict()
                 if parent_field not in query_by_parent_uuuid_and_field[parent_uuid]:
                     query_by_parent_uuuid_and_field[parent_uuid][parent_field] = list()
                 query_by_parent_uuuid_and_field[parent_uuid][parent_field].append(obj)
@@ -84,15 +84,15 @@
         else:
             for f, f_list in fields.items():
                 parent.__setattr__(f, f_list)
 
     return obj_list
 
 
-def build_dfs_from_dc_table(dc_table: List) -> Dict[str, pd.DataFrame]:
+def _build_dfs_from_dc_table(dc_table: List) -> Dict[str, pd.DataFrame]:
     df = pd.DataFrame.from_records(dc_table, columns=['parent', 'parent_class', 'parent_field', 'obj_class', 'obj', 'parent_uuid', 'obj_uuid'])
     
     table_names = df['parent_class'].unique().tolist()
     omit_vars = dict()
     for pc in table_names:
         omit_vars[pc] = df[df.parent_class == pc]['parent_field'].unique().tolist()
     print(omit_vars)
@@ -119,31 +119,31 @@
 
     dfs = dict()
     for name, tbl in tables.items():
         dfs[name] = pd.DataFrame.from_dict(tbl)
     return dfs
 
 
-def build_dc_table(dataclass_list: List, res_list: List, parent: Any, parent_field: str, parent_uuid: str) -> List:
+def _build_dc_table(dataclass_list: List, res_list: List, parent: Any, parent_field: str, parent_uuid: str) -> List:
     for dc in dataclass_list:
         if is_dataclass(dc):
             dc_uuid = uuid.uuid4()
             parent_class = None if parent is None else type(parent).__name__
             res_list.append( (parent, parent_class, parent_field, type(dc).__name__, dc, parent_uuid, dc_uuid) )
 
             for f in fields(dc):
                 if isinstance(vars(dc)[f.name], list):
-                    res_list = build_dc_table(vars(dc)[f.name], res_list, dc, f.name, dc_uuid)
+                    res_list = _build_dc_table(vars(dc)[f.name], res_list, dc, f.name, dc_uuid)
     return res_list
 
 
-def write(sheet_url_or_name: str, dataclass_list: List, prefix_id: str, template_name: Optional[str]=None, cache: bool=True) -> None:
-    dc_table = build_dc_table(dataclass_list, list(), parent=None, parent_field=None, parent_uuid=None)
+def write(sheet_url_or_name: str, dataclass_list: List, prefix_id: str, cache: bool=True) -> None:
+    dc_table = _build_dc_table(dataclass_list, list(), parent=None, parent_field=None, parent_uuid=None)
     try:
-        dfs = build_dfs_from_dc_table(dc_table)
+        dfs = _build_dfs_from_dc_table(dc_table)
     except BaseException as e:
         logging.error(f'Error while encoding dataclasses. Please consult the documentation to ensure not running into limitations.')
         return None
 
     for tbl_name, tbl_df in dfs.items():
         worksheet_name = f'{prefix_id}_{tbl_name}'
         sheets.write(sheet_url_or_name, worksheet_name, tbl_df, cache=cache)
```

### Comparing `sheetcloud-0.1.0.post8/sheetcloud/sheets.py` & `sheetcloud-0.1.0.post9/sheetcloud/sheets.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post8/sheetcloud/templates.py` & `sheetcloud-0.1.0.post9/sheetcloud/templates.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post8/sheetcloud/user.py` & `sheetcloud-0.1.0.post9/sheetcloud/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import logging
 logger = logging.getLogger('SHEETCLOUD USER')
 logging.basicConfig(format='\x1b[38;5;224m %(levelname)8s \x1b[0m | \x1b[38;5;39m %(name)s \x1b[0m | %(message)s', level=logging.DEBUG)
 
 
 from typing import *
 
-from sheetcloud.conn import service, ENV_SHEETCLOUD_USERNAME, ENV_SHEETCLOUD_PASSWORD
+from sheetcloud.conn import service, ENV_SHEETCLOUD_USERNAME, ENV_SHEETCLOUD_LICENSE
+
 
 
 def request_recovery_token(email: str=None) -> None:
     if email is None:
         email = ENV_SHEETCLOUD_USERNAME
     logger.info(f'Requesting password recovery token for account {email}.')
     _ = service('/users/password/recovery', params={'email': email}, method='post')
@@ -27,21 +28,25 @@
     if 'password_updated' in response:
         logging.info(f'Password updated {response["password_updated"]}.')
 
 
 def activate_license_key(key: str) -> None:
     response = service('/users/license/update', params={'key': key}, method='post')
     if 'is_valid' in response:
-        logging.info(f'License is valid = {response["is_valid"]}.')
+        logging.info(f'License is valid: {response["is_valid"]}.')
 
 
 def open_sheetcloud_website() -> None:
     webbrowser.open(f'https://sheetcloud.org')
 
 
+if ENV_SHEETCLOUD_LICENSE is not None:
+    logger.info(f'License found. Attempting to verify. Note: This only has to be done once.')
+    activate_license_key(ENV_SHEETCLOUD_LICENSE)
+
 
 if __name__ == "__main__":
     print('Test user connection...')
     # open_sheetcloud_website()
     # password_reset('jkdhsfjklasjhjkdfh', 'abb')
     activate_license_key('dskljklasfjd')
```

### Comparing `sheetcloud-0.1.0.post8/sheetcloud/utils.py` & `sheetcloud-0.1.0.post9/sheetcloud/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 def load_endpoint_config(version_name: str) -> Dict:
     return load_json(f'resources/endpoints.{version_name}.json')
 
 
 def pw_obfuscator(pw: str, exception: str=None) -> str:
-    obf = '******' if len(pw) < 5 else f'{pw[:3]}****'
+    obf = '******' if pw is None or len(pw) < 5 else f'{pw[:3]}****'
     if exception == pw:
         obf = pw
     return obf
 
 
 def int2a1(number: int) -> str:
     out = ''
```

### Comparing `sheetcloud-0.1.0.post8/sheetcloud.egg-info/PKG-INFO` & `sheetcloud-0.1.0.post9/sheetcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheetcloud
-Version: 0.1.0.post8
+Version: 0.1.0.post9
 Summary: Sheetcloud.de | Turn Spreadsheets into a Cloud Database | Account required
 Author-email: "sheetcloud.org" <contact@sheetcloud.org>
 Project-URL: Homepage, https://www.sheetcloud.org
 Project-URL: Tracker, https://github.com/sheetcloud/sheetcloud/issues
 Project-URL: Source, https://github.com/sheetcloud/sheetcloud
 Project-URL: Examples, https://github.com/sheetcloud
 Keywords: Spreadsheets,RAD,Database,Cloud
```

### Comparing `sheetcloud-0.1.0.post8/sheetcloud.egg-info/SOURCES.txt` & `sheetcloud-0.1.0.post9/sheetcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post8/tests/test_orm.py` & `sheetcloud-0.1.0.post9/tests/test_orm.py`

 * *Files identical despite different names*

