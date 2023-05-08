# Comparing `tmp/qbandas-1.1.1.tar.gz` & `tmp/qbandas-1.2.0.tar.gz`

## Comparing `qbandas-1.1.1.tar` & `qbandas-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qbandas-1.1.1/requirements.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qbandas-1.1.1/requirements_dev.txt
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/__main__.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/headers.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/pack.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/records.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/schema.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/util.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/data/field_types.json
--rwxr-xr-x   0        0        0      108 2020-02-02 00:00:00.000000 qbandas-1.1.1/scripts/build.bat
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 qbandas-1.1.1/scripts/doc-build.bat
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 qbandas-1.1.1/test/test_headers.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 qbandas-1.1.1/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.1.1/LICENSE
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 qbandas-1.1.1/README.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 qbandas-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 qbandas-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qbandas-1.2.0/requirements.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qbandas-1.2.0/requirements_dev.txt
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/__main__.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/data/address-fields.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/data/config.ini
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/data/field_types.json
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/profiles/__init__.py
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/profiles/profiles.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/records/__init__.py
+-rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/records/_pack.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/records/records.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/schemas/__init__.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/schemas/schemas.py
+-rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 qbandas-1.2.0/scripts/build.bat
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 qbandas-1.2.0/scripts/doc-build.bat
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 qbandas-1.2.0/test/test_headers.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 qbandas-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 qbandas-1.2.0/README.md
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 qbandas-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 qbandas-1.2.0/PKG-INFO
```

### Comparing `qbandas-1.1.1/qbandas/pack.py` & `qbandas-1.2.0/qbandas/records/_pack.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-"""
-Functions for converting data from Python's representation to QuickBase's representation.
-"""
-
-from datetime import datetime
-from typing import Any, Callable
+'''
+Functions for converting data from Python's representation to 
+QuickBase's representation.
+'''
+
+import datetime as dt
+import re
+from typing import Any
 
 import pandas as pd
 
 
 def _pack_default(x: Any) -> dict|None:
-    """
+    '''
     Pack a value into the default QuickBase API format.
 
     Parameters
     ----------
     x : Any
         The value to pack
 
@@ -25,22 +27,22 @@
     --------
     >>> import qbandas
     >>> qbandas.pack._pack_default('Object')
     {'value': 'Object'}
     >>> qbandas.pack._pack_default(None) == None
     True
 
-    """
+    '''
 
     if pd.isna(x):
         return None
     return {'value':x}
 
 def _pack_duration(x: float|int|str|None, unit: str = 'seconds') -> dict|None:
-    """
+    '''
     Pack a number into duration format for the QuickBase API
     
     Parameters
     ----------
     x : float | int | str | None
         The value to pack.
     unit : str
@@ -57,15 +59,15 @@
     >>> qbandas.pack._pack_duration(15)
     {'value': 15000}
     >>> qbandas.pack._pack_duration(15, unit = 'milliseconds')
     {'value': 15}
     >>> qbandas.pack._pack_duration(None) == None
     True
 
-    """
+    '''
 
     if pd.isna(x):
         return None
 
     x = int(x)
 
     if unit == 'seconds':
@@ -75,16 +77,16 @@
     else:
         raise Exception(f"'{unit}' is not a valid duration unit for value {x} of type {type(x)}")
 
     return {'value':x}
 
 
     
-def _pack_date(x: datetime|str|None, format: str = "%m.%d.%Y") -> dict|None:
-    """
+def _pack_date(x: dt.datetime|str|None, format: str = "%m.%d.%Y") -> dict|None:
+    '''
     Pack a date into the date format for the QuickBase API
 
     Parameters
     ----------
     x :  datetime | str | None
         The value to pack
     format : str
@@ -103,29 +105,28 @@
     >>> qbandas.pack._pack_date(dt(day=10, month=5, year=1754))
     {'value': '1754-05-10'}
     >>> qbandas.pack._pack_date('Friday, Nov 11, 2022', format='%A, %b %d, %Y')
     {'value': '2022-11-11'}
     >>> qbandas.pack._pack_date(None) == None
     True
 
-    """
+    '''
     if pd.isna(x):
         return None
 
-    if not isinstance(x, (datetime, str)):
+    if not isinstance(x, (dt.datetime, str)):
         raise Exception(f"value {x} of type {type(x)} cannot be coerced to date")
     elif isinstance(x, str):
-        x = datetime.strptime(x, format)
+        x = dt.datetime.strptime(x, format)
 
     return {'value':x.strftime('%Y-%m-%d')}
 
-    
-
-def _pack_datetime(x: datetime|str|None, format: str = '%d%b%Y:%H:%M:%S.%f') -> dict|None:
-    """
+def _pack_datetime(x: dt.datetime|str|None, 
+                   format: str = '%d%b%Y:%H:%M:%S.%f') -> dict|None:
+    '''
     Pack a datetime into the datetime format for the QuickBase API
     
     Parameters
     ----------
     x : datetime | str | None
         The value to pack
     format : str
@@ -145,82 +146,61 @@
     >>> qbandas.pack._pack_datetime(dt(day=10, month=5, year=1754, minute=24))
     {'value': '1754-05-10T00:24:00Z'}
     >>> qbandas.pack._pack_datetime('Friday, Nov 11, 2022 at 9:30 AM', format='%A, %b %d, %Y at %H:%M %p')
     {'value': '2022-11-11T09:30:00Z'}
     >>> qbandas.pack._pack_datetime(None) == None
     True
 
-    """
+    '''
     
     if pd.isna(x):
         return None
 
-    if not isinstance(x, (datetime, str)):
+    if not isinstance(x, (dt.datetime, str)):
         raise Exception(f"'{type(x)}' cannot be coerced to datetime")
     elif isinstance(x, str):
-        x = datetime.strptime(x, format)
+        x = dt.datetime.strptime(x, format)
     
     return {'value':x.strftime('%Y-%m-%dT%H:%M:%SZ')}
 
-   
-
-def _pack_phonenum(x: None|str, format: str = "##########") -> dict|None:
-    """
+def _pack_phonenum(x: None|str|float|int) -> dict|None:
+    '''
     Pack a phone string into the phone format for the QuickBase API
     
     Parameters
     ----------
-    x : None | str
-        The value to pack. It should be a string
-    format : str
-        the format string for reading the phone number. The phone number 
-        "(123) 456-7890 x123" would have the format string 
-        "(###) ###-#### x###". The extension must come last. It is 
-        optional for x to include it.
+    x : None | str | float | int
+        The value to pack. If it is a float, decimal is truncated
 
     Returns
     -------
     dict | None : the packed value
 
     Examples
     --------
     >>> import qbandas
     >>> qbandas.pack._pack_phonenum('9205551234')
     {'value': '(920) 555-1234'}
-    >>> qbandas.pack._pack_phonenum('<920>888.1234x553', format = '<###>###.####x###')
+    >>> qbandas.pack._pack_phonenum('<920>888.1234x553')
     {'value': '(920) 888-1234 x553'}
     >>> qbandas.pack._pack_phonenum(None) == None
     True
 
-    """
+    '''
+    if pd.isna(x) or not x: return None
     
-    if pd.isna(x) or not x:
-        return None
+    if isinstance(x, (int, float)):
+        x = f'{x:.0f}'
     
     if not isinstance(x, str):
-        raise Exception(f"type {type(x)} is invalid for value {x}, expected type str")
+        raise Exception(f"type {type(x)} is invalid for value {x}, "
+                        "expected type str")
 
-    # a str containing only the digits in order
-    try:
-        y = [x[i] for i in range(len(x)) if format[i] == '#']
-        y = ''.join(y)
-    except IndexError:
-        raise Exception(f"could not parse '{x}' with format '{format}'") 
-
-    if not y.isnumeric() or len(y) < 10:
-        raise Exception(f"could not parse '{x}' with format '{format}'") 
-
-    t = f'({y[0:3]}) {y[3:6]}-{y[6:10]}'
-    if len(y) > 10:
-        t = t + f' x{y[10:]}'
-
-    #return "(123) 456-7890 x123"
-    return {'value':t}
-
-# a string to func mapping allowing the packing funcs to be assigned in data/field_types.json
-PACKING_FUNCS: dict[str, Callable[..., dict|None]] = {
-    'default': _pack_default,
-    'duration': _pack_duration,
-    'date': _pack_date,
-    'datetime': _pack_datetime,
-    'phonenum': _pack_phonenum,
-    }
+    x = re.sub(r'\D', '', x) 
+    if not 10 <= len(x):
+        raise Exception(f"phone number {x} is not parsable")
+    
+    # return "(123) 456-7890 x123"
+    retval = f'({x[:3]}) {x[3:6]}-{x[6:10]}' # base number
+    if 10 < len(x): retval += f' x{x[10:]}'  # extension
+    
+    return {'value':retval}
```

### Comparing `qbandas-1.1.1/qbandas/records.py` & `qbandas-1.2.0/qbandas/records/records.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-"""
-Functions that deal with sending records or information to a Quickbase 
-application.
-"""
-
 import asyncio
+import datetime as dt
 import json
-import os
+import os.path as op
 from functools import partial
-from os.path import join
-from pathlib import Path
 
 import pandas as pd
 import requests
 
-from . import FIELD_TYPES, headers
+from .. import MAX_BATCH_RECORDS, QB_PATH, TIMEZONE_OFFSET
+from ..profiles import _get_headers, is_valid_profile
+from ..schemas import _read_schema
+from . import _pack
+
+with open(op.join(QB_PATH, 'data', 'field_types.json')) as f:
+    FIELD_TYPES = json.load(f)
+    
+# resolve the packing functions
+for _, cnfg in FIELD_TYPES.items():
+    if cnfg["packing-function"]:
+        cnfg["packing-function"] = getattr(_pack, cnfg["packing-function"])
 
 
-def upload(df: pd.DataFrame, table_name: str, directory: Path|str = None,
-            **kwargs): 
-    """
+def upload_records(df: pd.DataFrame, table_name: str, profile: str,
+                   drop: bool = False): 
+    '''
     Send a table of records (rows) to a table on QuickBase.
 
     If no errors are thrown, the data was successfully uploaded to 
     QuickBase. If an error occurs when sending the data, it is possible 
     that only _some_ of your records will have been uploaded to 
     QuickBase. If that is an issue, please fix the data, and send it 
     all again.
@@ -30,125 +35,128 @@
     Parameters
     ----------
     df : pd.DataFrame
         The table of records
     table_name : str
         Identifies which table to send the data to. You should use 
         `pull_schema()` to create a valid `table_name`.
-    directory : None | Path | str
-        The directory to use for this operation. Default is current
-    """
-
-    # enable debugging print statements
-    debug = kwargs.get('debug')
-    if debug:
-        from .util import str_dict, str_resp
+    profile : str
+        The profile to authorize this request
+    drop : bool, optional
+        Toggle dropping extra columns. If False, all columns must match, by deafult False
+    '''
+
+    if __debug__: 
+        from pprint import pp
         print(df.head())
     
-    directory = directory if directory else os.getcwd()  
-    if not os.path.isdir(directory):
-        raise FileNotFoundError(f'{directory = } is not a valid directory')
-    
-    headers_ = headers.read(directory = directory)
-    with open(join(directory, 'schemas', f'{table_name}.json'), 'r') as f:
-        schema = json.load(f)
-
-    if debug:
-        print(str_dict(headers_))
-        print(str_dict(schema))
+    # headers
+    if not is_valid_profile(profile, talk =  True):
+        raise ValueError(f'profile {profile} cannot be used')
+    headers_ = _get_headers(profile)
+
+    # schema
+    dbid, schema = _read_schema(table_name)
+    if not dbid:
+        raise ValueError(f'schema for {table_name} cannot be found')
+
+    if __debug__:
+        pp(headers_)
+        print(dbid)
+        pp(schema)
 
     # Check that the columns in the df match the schema
-    if not kwargs.get('drop'):
-        unknown_columns = [] # columns in df that aren't in schema
-        for column in df.columns:
-            if column not in schema.keys():
-                unknown_columns.append(column)
+    if not drop:
+        unknown_columns = set(df.columns) - set(schema)
+        unused_columns = set(schema) - set(df.columns)
         if unknown_columns:
-            raise Exception(f"The following columns from your dataframe have \
-                            no matching column in the specified QuickBase \
-                            table. If you want to drop these columns (not \
-                            send their data), add `drop=True` to this function \
-                            call. Columns: " + ', '.join(unknown_columns))
+            raise ValueError(f'the columns {unknown_columns} are not in'
+                             f'the schema {table_name}. To drop these'
+                             'columns, add drop=True. Unused columns: '
+                             f'{unused_columns}.')
     
     # pack all the values into qb's crazy formats
     packed_df = pd.DataFrame()
     for col in df.columns:
 
-        if col not in schema: # dropped columns
-            continue
-
-        col_info = schema[col]
-        col_type = col_info['type']
-        col_kwargs = col_info['args'] if 'args' in col_info else {}
+        if col not in schema: continue
+    
+        col_type = schema[col]['type']
+        col_kwargs = schema[col].get('args', {})
 
         try:
             # get the packing function and apply it
             packing_func = partial(FIELD_TYPES[col_type]['pack'], **col_kwargs)
             packed_df[col] = df[col].copy().apply(packing_func)
         except Exception as e:
-            e.args = (f"Failed parsing column '{col}' with column type \
-                      '{col_type}' and arguments '{col_kwargs}'", *e.args)
+            e.args = (f'Failed parsing column {col} with column type'
+                      f'{col_type} and arguments {col_kwargs}', *e.args)
             raise
 
-    if debug:
+    if __debug__:
         print(packed_df.head())
 
     # grab the feild ids from schema, rename columns 
-    fids = {k: v['id'] for k, v in schema.items() if \
-            k != '_DBID_' and k in packed_df.columns}
+    fids = {k: v['id'] for k, v in schema.items()}
     renamed_df = packed_df.copy().rename(columns=fids) 
 
     def _row_to_dict(row):
         '''Convert a row into a dictonary and drop nulls'''
         row = dict(row)                                         
         return {k: v for k, v in row.items() if not pd.isna(v)} 
     records = list(renamed_df.apply(_row_to_dict, axis=1)) 
 
-    if debug:
-        print(str_dict(records[:5]))
+    if __debug__:
+        pp(records[:5])
 
     # setup destination information
-    body = {"to": schema['_DBID_']}
-
-    # look for optinal arguments to include from kwargs
-    for option in ["fieldsToReturn", 'mergeFieldId']:
-        if option in kwargs:
-            body[option] = kwargs[option]
-
-    # send the data all at once
-
-    async def main():
-        batch_size = 5
-        jobs = list()
-        for i in range(0, len(records), batch_size):
-            async def job():
-                body["data"] = records[i : i + batch_size]
-                r = requests.post('https://api.quickbase.com/v1/records', 
-                    headers = headers_, json = body)
-                if debug: print(str_resp(r))
-                r.raise_for_status()
-                print('RAN THAT YE YEE')
-            jobs.append(job())
-        await asyncio.gather(*jobs)
-    asyncio.run(main())
-    
+    body = {"to": dbid}
     
+    async def _upload_batch(i: int):
+        '''
+        Upload a section of the records asynchronously 
+        
+        Parameters
+        ----------
+        i : int
+            The index of the first record to upload
+        '''
+        body["data"] = records[i : i + MAX_BATCH_RECORDS]
+        r = requests.post('https://api.quickbase.com/v1/records', 
+            headers = headers_, json = body)
+        if __debug__: 
+            pp(r.json())
+        r.raise_for_status()
+
+    async def _upload_all():
+        '''Uploads all the records in a series of batches'''
+        jobs = []
+        for i in range(0, len(records), MAX_BATCH_RECORDS):
+            jobs.append(_upload_batch(i))
+        await asyncio.gather(*jobs)
+        
+    asyncio.run(_upload_all())
 
-def fetch(table_name: str, *columns, where: str = None, order: list = None, 
-            group_by: list = None, skip: int = 0, limit: int = None, 
-            directory: Path|str = None, **kwargs) -> pd.DataFrame:
+def fetch_records(table_name: str, profile: str, *, columns: list[str] = None, 
+                  where: str = None, order: list = None, 
+                  group_by: list = None, skip: int = 0, 
+                  limit: int = None) -> pd.DataFrame:
     '''
     Fetch a table of records from a QuickBase app
 
-    Retrieves records from QuickBase. Authorized by `headers.json`.
+    Retrieves records from QuickBase
 
     Parameters
     ----------
     table_name : str
         The table to pull from
+    profile : str
+        The name of the profile to authorize this request
+    columns : list[str], optional
+        The columns to select, by default None
     where : str, optional
         Should be written like an SQL statement, by default None
     order : list, optional
         The order in which to sort the returned records. Each entry 
         in this list is a tuple with the first element being the 
         column name, and the second is the word 'asc' or 'desc'. 
         by default None
@@ -156,39 +164,44 @@
         How to group records, by default None
     skip : int, optional
         Number of records to skip off the top off the returned 
         dataframe, by default 0
     limit : int, optional
         Maximum number of records that can be returned. None is no
         limit, by default None
-    directory : Path | str, optional
-        The directory for this operation, by default current
-    *columns
-        The columns to select
-    **kwargs
-        Unused
-
+        
     Returns
     -------
     pd.DataFrame
         The records from QuickBase. 
     
     '''
     
-    directory = directory if directory else os.getcwd()  
-    if not os.path.isdir(directory):
-        raise FileNotFoundError(f'{directory = } is not a valid directory')
-    
-    # read in headers and schema
-    headers_ = headers.read(directory = directory)
-    with open(join(directory, 'schemas', f'{table_name}.json'), 'r') as f:
-        schema = json.load(f) # for resolving column names
+    # headers
+    if not is_valid_profile(profile, talk =  True):
+        raise ValueError(f'profile {profile} cannot be used')
+    headers_ = _get_headers(profile)
+    
+    if __debug__:
+        from pprint import pp
+        pp(headers_)
+
+    # schema
+    dbid, schema = _read_schema(table_name)
+    if not dbid:
+        raise ValueError(f'schema for {table_name} cannot be found')
+    
+    if __debug__:
+        print(dbid)
+        pp(schema)
+        
+    columns = columns if columns else set(schema)
         
     body = {
-        'from': table_name,
+        'from': dbid,
         'select': [schema[c]['id'] for c in columns],
         "options": {
             "skip": skip if skip else 0,
             "top": limit if limit else -1,
             "compareWithAppLocalTime": True
         }
     }
@@ -207,32 +220,35 @@
         raise NotImplementedError('No grouping just yet!')
     
     # are we filtering?
     if where:
         body['where'] = '{fid.op.\'value\'}'
         raise NotImplementedError('No filtering just yet!')
     
+    if __debug__:
+        pp(body)
+    
     # send request
     r = requests.post('https://api.quickbase.com/v1/records/query', 
         headers = headers_, json = body)
+    if __debug__:
+        pp(r.json())
     r.raise_for_status()
     
     # unravel response
     data = r.json()['data']
     fields = r.json()['fields']
     name_map = {str(x['id']): x['label'] for x in fields}
     type_map = {str(x['id']): x['type'] for x in fields}
     
     # assemble dataframe
     for i, record in enumerate(data.copy()):
         data[i] = {k: v['value'] for k, v in record.items()}
+        
     df = pd.DataFrame(data)
-    # data typing... builtins didn't work for me
     for id, type_ in type_map.items():
         if type_ in ['timestamp', 'date']:
-            import datetime as dt
-
-            # WARNNG:: OFFSET FOR US CENTRAL TIME
-            df[id] = pd.to_datetime(df[id]) - dt.timedelta(hours=5)
+            df[id] = pd.to_datetime(df[id]) - dt.timedelta(
+                hours = TIMEZONE_OFFSET)
+            
     df.rename(columns = name_map, inplace = True)
-    
     return df
```

### Comparing `qbandas-1.1.1/qbandas/schema.py` & `qbandas-1.2.0/qbandas/schemas/schemas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,201 @@
-"""
-Methods that deal with resolving the structure of local and remote (QuickBase) tables.
-"""
 import json
 import os
-from os.path import exists, join
-from pathlib import Path
-from typing import NoReturn
+import os.path as op
+import re
 
 import requests
 
-from . import headers
+from .. import QB_PATH, USER_PATH
+from ..profiles import _get_headers, is_valid_profile
 
 
-def pull(DBID: str, directory: Path|str = None, **kwargs) -> NoReturn:
+def fetch_schema(dbid: str, profile: str, table_name: str = None):
     """
     Download a local copy of a table's structure from a QuickBase 
     application.
 
-    This operation is authorized by `./headers.json`. The schema will be
-    placed into `./schemas/` where other qBandas operations can use it. 
-
     Parameters
     ----------
-    DBID : str
+    dbid : str
         The unique identifier of the table in QuickBase.
-    directory : None | Path | str
-        The directory to use for this operation. Default is current
+    profile : str
+        The profile to authorize this request
+    table_name : str, optional
+        The name of the table. None uses the dbid, by default None
 
     Examples
     --------
     >>> import qbandas
     >>> # qbandas.schema.pull('bb7f543') # unauthorized
 
     """
-    directory = directory if directory else os.getcwd()  
-    if not os.path.isdir(directory):
-        raise FileNotFoundError(f'{directory = } is not a valid directory')
 
-    headers_ = headers.read(directory = directory)
+    headers = _get_headers(profile)
+    if not is_valid_profile(profile, talk = True):
+        raise ValueError(f'unusable profile {profile}')
 
     # send the request to quickbase
-    params = {'tableId': DBID, 'includeFieldPerms': "false"}
-    r = requests.get('https://api.quickbase.com/v1/fields', params = params, headers = headers_)
+    r = requests.get('https://api.quickbase.com/v1/fields', 
+                    params = {
+                        'tableId': dbid, 
+                        'includeFieldPerms': "false"
+                    }, 
+                    headers = headers)
     r.raise_for_status()
 
-    # convert the language in the api to user language
-    type_conversion = {
-        "timestamp": "datetime",
-        "recordid": "numeric",
-        "email": "email-address",
-        "phone": "phone-number",
-        }
-
-    address_subfields = {
-        ": Street 1": 1,
-        ": Street 2": 2,
-        ": City": 3,
-        ": State": 4,
-        ": Zip": 5,
-        ": Country": 6,
-        }
+    # get the address subfields
+    with open(op.join(QB_PATH, 'data', 'address-fields.json')) as f:        
+        address_fields = json.load(f)
 
     # parse the schema from the response
-    schema = dict()
-    schema['_DBID_'] = DBID
-    for field in r.json():
-
-        # address fields send extra unlabeled info that we cannot use. remove it
-        if field['label'] in ['Street 1', 'Street 2', 'City', 'State/Region', 'Postal Code', 'Country']:
+    fields = dict()
+    for item in r.json():
+        
+        type_ = item['fieldType']
+        id_ = item['id']
+        label_ = item['label']
+        
+        # address fields send extra unlabeled info that we cannot use. 
+        # remove it.
+        if label_ in address_fields['junk-names']:
             continue
-
-        type_ = field['fieldType']
-        if type_ in type_conversion:
-            type_ = type_conversion[type_]
         
-        schema[field['label']] = {'id': field['id'], 'type': type_}
+        fields[label_] = {'id': id_, 'type': type_}
 
         # recreate subfields for adresses with propper names
         if type_ == 'address':
-            for sufix, fid_offset in address_subfields.items():
-                schema[field['label'] + sufix] = {
-                    'id': field['id'] + fid_offset,
+            for sufix, fid_offset in address_fields["suffixes"].items():
+                fields[label_ + sufix] = {
+                    'id': id_ + fid_offset,
                     'type': "text"
                 }
 
-    # dump the schema to disk
-    schemas_dir = join(directory, 'schemas')
-    if not exists(schemas_dir):
-        os.makedirs(schemas_dir)
-    with open(join(schemas_dir, DBID + '.json'), 'w') as f:
-        json.dump(schema, f, indent=4)
+    _write_schema(table_name, dbid, fields)
     
-        
-def add_args(schema_name: str, directory: Path|str = None, *args, **kwargs):
-    """
-    Append new config options (args) for fields in a schema.
+def list_schemas() -> list[str]:
+    '''
+    List the names of all the usable schemas.
+
+    The names are 'table names'
+
+    Returns
+    -------
+    list[str]
+        The names of all the usable schemas
+    '''
+    schema_path = op.join(USER_PATH, 'schemas')
+    names = [re.sub(r'\.json', '', x) for x in os.listdir(schema_path)]
+    return names
+
+def _read_schema(table_name: str) -> tuple[str, dict]:
+    '''
+    Read in a schema
 
+    Returns the information if the schema exist
+    
     Parameters
     ----------
-    schema_name : str
-        The schema to modify.
-    directory : None | Path | str
-        The directory to use for this operation. Default is current
-    *args
-        These fields will be configured.
-    **kwargs
-        The arguments to add.
+    table_name : str
+        The name of the table to get the schema for
+
+    Returns
+    -------
+    tuple[str, dict]
+        The dbid of the table followed by the field information if the 
+        schem exists. If it doesn't exist, you get (None, dict())
+    '''
+    
+    schema_path = op.join(USER_PATH, 'schemas', table_name + '.json')
+    if not op.exists(schema_path):
+        return None, {}
+    with open(schema_path) as f:
+        data = json.load(f)
+        return data['dbid'], data['fields']
         
-    """
+def _write_schema(table_name: str, dbid: str, fields: dict):
+    '''
+    Write a schema to disk
 
-    directory = directory if directory else os.getcwd()  
-    if not os.path.isdir(directory):
-        raise FileNotFoundError(f'{directory = } is not a valid directory')
+    For internal use
+
+    Parameters
+    ----------
+    table_name : str
+        The name of the schema to write
+    dbid : str
+        The database ID of the QuickBase table
+    fields : dict
+        A dictonary of fields and their metadata
+    '''
+    schema_path = op.join(USER_PATH, 'schemas', table_name + '.json')
+    with open(schema_path, 'w') as f:
+        data = {'dbid': dbid, 'fields': fields}
+        json.dump(data, f)
+    
+def add_schema_args(table_name: str, fields: list = None, 
+                    arguments: dict = None, *fields_, **arguments_):
+    '''
+    Add arguments to a table's schema
+
+    Will append to the schema and override any existing arguments with 
+    the same name
+
+    Parameters
+    ----------
+    table_name : str
+        The table to update
+    fields : list
+        The field names to update, by default None
+    arguments : dict
+        The arguments to add, by default None
+    '''
 
     # read in the schema
-    file_name = schema_name + '.json'
-    with open(os.path.join(directory, 'schemas', file_name), 'r') as f:
-        schema = json.load(f)
+    dbid, schema = _read_schema(table_name)
+    if not dbid: raise ValueError(f'table {table_name} does not exist')
 
+    fields = (fields if fields else []) + fields_
+    arguments = (arguments if arguments else {}) | arguments_
+    
     # append the new arguments
-    for field in args:
+    for field in fields:
         if field not in schema:
-            raise Exception(f"The field {field} is not in the schema {schema_name}")
-        if 'args' not in schema[field]:
-            schema[field]['args'] = kwargs
-        else:
-            schema[field]['args'] = schema[field]['args'] | kwargs
+            raise ValueError(f"The field {field} is not in the schema"
+                             f"{table_name}.")
+        current = schema[field].get('args', {})
+        schema[field]['args'] = current | arguments
 
     # put the schema pack into the file
-    with open(join(directory, 'schemas', file_name), 'w') as f:
-        json.dump(schema, f, indent=4)
+    _write_schema(table_name, dbid, fields)
 
-def set_args(schema_name: str, directory: Path|str = None, *args, **kwargs):
-    """
-    Set the config options (args) for fields in a schema.
+def set_schema_args(table_name: str, fields: list = None, 
+                    arguments: dict = None, *fields_, **arguments_):
+    '''
+    Set the arguments for some fields in a given schema
 
     Parameters
     ----------
-    schema_name : str
-        The schema to modify.
-    directory : None | Path | str
-        The directory to use for this operation. Default is current
-    *args
-        These fields will be configured.
-    **kwargs
-        The arguments to add.
-    """
+    table_name : str
+        The nameof the table to configure
+    fields : list, optional
+        The fields to configure, by default None
+    arguments : dict, optional
+        The arguments to add, by default None
+    '''
 
-    directory = directory if directory else os.getcwd()  
-    if not os.path.isdir(directory):
-        raise FileNotFoundError(f'{directory = } is not a valid directory')
-    
     # read in the schema
-    file_name = schema_name + '.json'
-    with open(os.path.join(directory, 'schemas', file_name), 'r') as f:
-        schema = json.load(f)
+    dbid, schema = _read_schema(table_name)
+    if not dbid: raise ValueError(f'table {table_name} does not exist')
 
-    # set the arguments
-    for field in args:
+    fields = (fields if fields else []) + fields_
+    arguments = (arguments if arguments else {}) | arguments_
+    
+    # append the new arguments
+    for field in fields:
         if field not in schema:
-            raise Exception(f"The field {field} is not in the schema {schema_name}")
-        schema[field]['args'] = kwargs
+            raise ValueError(f"The field {field} is not in the schema"
+                             f"{table_name}.")
+        schema[field]['args'] = arguments
 
     # put the schema pack into the file
-    with open(os.path.join(directory, 'schemas', file_name), 'w') as f:
-        json.dump(schema, f, indent=4)
+    _write_schema(table_name, dbid, fields)
```

### Comparing `qbandas-1.1.1/LICENSE` & `qbandas-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qbandas-1.1.1/pyproject.toml` & `qbandas-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "qbandas"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
   { name = "Joshua Hopwood" },
 ]
 description = "Integrates the popular data handling library Pandas and the QuickBase API"
 dependencies = [
   "pandas==1.4.3",
   "requests==2.28.1"
@@ -20,8 +20,8 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 homepage = "https://pypi.org/project/qbandas/"
 repository = "https://github.com/jhopwood-jjk/qBandas"
-documentation = "https://jhopwood-jjk.github.io/qbandas/"
+documentation = "https://jhopwood-jjk.github.io/qbandas/index.html"
```

