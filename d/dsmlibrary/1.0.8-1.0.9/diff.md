# Comparing `tmp/dsmlibrary-1.0.8.tar.gz` & `tmp/dsmlibrary-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmlibrary-1.0.8.tar", last modified: Wed Aug  3 09:50:09 2022, max compression
+gzip compressed data, was "dist/dsmlibrary-1.0.9.tar", last modified: Wed Aug 10 09:28:48 2022, max compression
```

## Comparing `dsmlibrary-1.0.8.tar` & `dsmlibrary-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-08-03 09:50:09.179540 dsmlibrary-1.0.8/
--rw-r--r--   0 naii       (501) staff       (20)     2124 2022-08-03 09:50:09.179200 dsmlibrary-1.0.8/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)     1530 2022-07-04 14:36:01.000000 dsmlibrary-1.0.8/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-08-03 09:50:09.172763 dsmlibrary-1.0.8/dsmlibrary/
--rw-r--r--   0 naii       (501) staff       (20)      141 2022-05-03 07:53:11.000000 dsmlibrary-1.0.8/dsmlibrary/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     3616 2022-08-01 09:03:50.000000 dsmlibrary-1.0.8/dsmlibrary/base.py
--rw-r--r--   0 naii       (501) staff       (20)     2896 2022-07-06 14:10:10.000000 dsmlibrary-1.0.8/dsmlibrary/clickhouse.py
--rw-r--r--   0 naii       (501) staff       (20)     7703 2022-08-02 08:14:28.000000 dsmlibrary-1.0.8/dsmlibrary/datanode.py
--rw-r--r--   0 naii       (501) staff       (20)     4148 2022-07-04 13:52:00.000000 dsmlibrary-1.0.8/dsmlibrary/dataset.py
--rw-r--r--   0 naii       (501) staff       (20)      225 2022-05-25 04:01:48.000000 dsmlibrary-1.0.8/dsmlibrary/task.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-08-03 09:50:09.178477 dsmlibrary-1.0.8/dsmlibrary/utils/
--rw-r--r--   0 naii       (501) staff       (20)        0 2022-06-15 06:54:09.000000 dsmlibrary-1.0.8/dsmlibrary/utils/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     1946 2022-06-12 10:41:02.000000 dsmlibrary-1.0.8/dsmlibrary/utils/clickhouse.py
--rw-r--r--   0 naii       (501) staff       (20)        0 2022-08-01 08:29:06.000000 dsmlibrary-1.0.8/dsmlibrary/utils/sqlQuery.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-08-03 09:50:09.176553 dsmlibrary-1.0.8/dsmlibrary.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)     2124 2022-08-03 09:50:08.000000 dsmlibrary-1.0.8/dsmlibrary.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      407 2022-08-03 09:50:09.000000 dsmlibrary-1.0.8/dsmlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2022-08-03 09:50:08.000000 dsmlibrary-1.0.8/dsmlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       75 2022-08-03 09:50:08.000000 dsmlibrary-1.0.8/dsmlibrary.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       11 2022-08-03 09:50:09.000000 dsmlibrary-1.0.8/dsmlibrary.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2022-08-03 09:50:09.179670 dsmlibrary-1.0.8/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1384 2022-08-03 09:50:05.000000 dsmlibrary-1.0.8/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/
+-rw-r--r--   0 naii       (501) staff       (20)     2743 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/PKG-INFO
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/dsmlibrary.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     2743 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/dsmlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      430 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/dsmlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)       75 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/dsmlibrary.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       11 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/dsmlibrary.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/dsmlibrary.egg-info/dependency_links.txt
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/dsmlibrary/
+-rw-r--r--   0 naii       (501) staff       (20)      225 2022-05-25 04:01:48.000000 dsmlibrary-1.0.9/dsmlibrary/task.py
+-rw-r--r--   0 naii       (501) staff       (20)     2896 2022-07-06 14:10:10.000000 dsmlibrary-1.0.9/dsmlibrary/clickhouse.py
+-rw-r--r--   0 naii       (501) staff       (20)      141 2022-05-03 07:53:11.000000 dsmlibrary-1.0.9/dsmlibrary/__init__.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/dsmlibrary/utils/
+-rw-r--r--   0 naii       (501) staff       (20)     1946 2022-06-12 10:41:02.000000 dsmlibrary-1.0.9/dsmlibrary/utils/clickhouse.py
+-rw-r--r--   0 naii       (501) staff       (20)        0 2022-06-15 06:54:09.000000 dsmlibrary-1.0.9/dsmlibrary/utils/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      217 2022-08-10 09:12:05.000000 dsmlibrary-1.0.9/dsmlibrary/utils/requests.py
+-rw-r--r--   0 naii       (501) staff       (20)    10604 2022-08-09 03:21:44.000000 dsmlibrary-1.0.9/dsmlibrary/datanode.py
+-rw-r--r--   0 naii       (501) staff       (20)     1177 2022-08-10 09:03:42.000000 dsmlibrary-1.0.9/dsmlibrary/datadict.py
+-rw-r--r--   0 naii       (501) staff       (20)     4148 2022-07-04 13:52:00.000000 dsmlibrary-1.0.9/dsmlibrary/dataset.py
+-rw-r--r--   0 naii       (501) staff       (20)     3616 2022-08-01 09:03:50.000000 dsmlibrary-1.0.9/dsmlibrary/base.py
+-rw-r--r--   0 naii       (501) staff       (20)     1530 2022-07-04 14:36:01.000000 dsmlibrary-1.0.9/README.md
+-rw-r--r--   0 naii       (501) staff       (20)     1384 2022-08-10 09:28:38.000000 dsmlibrary-1.0.9/setup.py
+-rw-r--r--   0 naii       (501) staff       (20)       38 2022-08-10 09:28:48.000000 dsmlibrary-1.0.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dsmlibrary-1.0.8/PKG-INFO` & `dsmlibrary-1.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 Metadata-Version: 2.1
 Name: dsmlibrary
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://gitlab.com/public-project2/dsm-library
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
+Description: # DSM Library
+        
+        ## DataNode
+        0. init DataNode
+        ```python
+        from dsmlibrary.datanode import DataNode 
+        
+        data = DataNode(token)
+        ```
+        1. upload file
+        ```python
+        data.upload_file(directory_id=<directory_id>, file_path='<file_path>', description="<description(optional)>")
+        ```
+        
+        2. download file
+        ```python
+        data.download_file(file_id=<file_id>, download_path="<place download file save> (default ./dsm.tmp)")
+        ```
+        3. get file
+        ```python
+        meta, file = get_file(file_id="<file_id>")
+        # meta -> dict
+        # file -> io bytes
+        ```
+        ```python
+        # example read csv pandas
+         
+        meta, file = get_file(file_id="<file_id>")
+        df = pd.read_csv(file)
+        ...
+        ``` 
+        
+        4. write parquet file
+        ```python
+        df = ... # pandas dataframe or dask dataframe
+        
+        data.write(df=df, directory=<directory_id>, name=<save_file_name>, profiling=<True or False default False>)
+        ```
+        
+        ## Clickhouse
+        1. imoprt data to clickhouse
+        
+        ```python
+        from dsmlibrary.clickhouse import ClickHouse
+        
+        ddf = ... # pandas dataframe or dask dataframe
+        
+        ## to warehouse
+        table_name = <your_table_name>
+        table_key = <your_table_key>
+        
+        connection = { 
+          'host': '', 
+          'port': , 
+          'database': '', 
+          'user': '', 
+          'password': '', 
+          'settings':{ 
+             'use_numpy': True 
+          }, 
+          'secure': False 
+        }
+        
+        warehouse = ClickHouse(connection=connection)
+        
+        tableName = warehouse.get_or_createTable(ddf=ddf, tableName=table_name, key=table_key)
+        warehouse.write(ddf=ddf, tableName=tableName, key=table_key)
+        ```
+        
+        2. query data from clickhouse
+        ```python
+        query = f""" 
+            SELECT * FROM {tableName} LIMIT 10 
+        """ 
+        warehouse.read(sqlQuery=query)
+        
+        ```
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-
-# DSM Library
-
-## DataNode
-0. init DataNode
-```python
-from dsmlibrary.datanode import DataNode 
-
-data = DataNode(token)
-```
-1. upload file
-```python
-data.upload_file(directory_id=<directory_id>, file_path='<file_path>', description="<description(optional)>")
-```
-
-2. download file
-```python
-data.download_file(file_id=<file_id>, download_path="<place download file save> (default ./dsm.tmp)")
-```
-3. get file
-```python
-meta, file = get_file(file_id="<file_id>")
-# meta -> dict
-# file -> io bytes
-```
-```python
-# example read csv pandas
- 
-meta, file = get_file(file_id="<file_id>")
-df = pd.read_csv(file)
-...
-``` 
-
-4. write parquet file
-```python
-df = ... # pandas dataframe or dask dataframe
-
-data.write(df=df, directory=<directory_id>, name=<save_file_name>, profiling=<True or False default False>)
-```
-
-## Clickhouse
-1. imoprt data to clickhouse
-
-```python
-from dsmlibrary.clickhouse import ClickHouse
-
-ddf = ... # pandas dataframe or dask dataframe
-
-## to warehouse
-table_name = <your_table_name>
-table_key = <your_table_key>
-
-connection = { 
-  'host': '', 
-  'port': , 
-  'database': '', 
-  'user': '', 
-  'password': '', 
-  'settings':{ 
-     'use_numpy': True 
-  }, 
-  'secure': False 
-}
-
-warehouse = ClickHouse(connection=connection)
-
-tableName = warehouse.get_or_createTable(ddf=ddf, tableName=table_name, key=table_key)
-warehouse.write(ddf=ddf, tableName=tableName, key=table_key)
-```
-
-2. query data from clickhouse
-```python
-query = f""" 
-    SELECT * FROM {tableName} LIMIT 10 
-""" 
-warehouse.read(sqlQuery=query)
-
-```
-
```

### Comparing `dsmlibrary-1.0.8/README.md` & `dsmlibrary-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dsmlibrary-1.0.8/dsmlibrary/base.py` & `dsmlibrary-1.0.9/dsmlibrary/base.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary-1.0.8/dsmlibrary/clickhouse.py` & `dsmlibrary-1.0.9/dsmlibrary/clickhouse.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary-1.0.8/dsmlibrary/datanode.py` & `dsmlibrary-1.0.9/dsmlibrary/datanode.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import io
+import time
+import inspect
 import requests
 import pandas as pd
 import dask.dataframe as dd
+
 from .base import bucket_name, Base
 from .dataset import DatasetManager
-import io
-import time
+from .utils.requests import check_http_status_code
 
 def append_slash(txt):
     if txt[-1] != '/':
         txt += '/'
     return txt
 
 class DataNode(DatasetManager):
@@ -76,26 +79,38 @@
             })
             meta = {key: value for key,value in meta.items() if key in ['owner', 'name', 'description', 'path', 'directory', 'human_size']}
             return meta, io.BytesIO(response.data)
         
     
     def read_ddf(self, file_id=None):
         _res = requests.get(f"{self._discovery_api}/file/{file_id}/", headers=self._jwt_header)
-        if _res.status_code != 200:
-            txt = _res.json() if _res.status_code < 500 else " "
-            raise Exception(f"Some thing wrong, {txt}")
+        check_http_status_code(_res)
         meta = _res.json()
         meta.update({
             'key': append_slash(meta['s3_key'])
         })
         _f_type = meta['type']['name']
         if _f_type == "parquet":
             return dd.read_parquet(f"s3://{bucket_name}/{meta['key']}", storage_options=self._storage_options)
         elif _f_type == "csv":
             return dd.read_csv(f"s3://{bucket_name}/{meta['key']}", storage_options=self._storage_options)
+        elif _f_type == "sql-query":
+            r = requests.get(f"{self._base_discovery_api}/api/v2/file/{meta['id']}/getSqlQuery/", headers=self._jwt_header)
+            check_http_status_code(r)
+            r = requests.get(f"{self._base_discovery_api}/api/sql/query/{r.json()['id']}/", headers=self._jwt_header)
+            check_http_status_code(r)
+            data = r.json()
+            _database = DatabaseManagement(token=self.token)
+            meta, schema = _database.get_table_schema(table_id=data['table'])
+            exec(f"""
+{schema}
+from sqlalchemy import sql
+{data['query']}
+            """, globals())
+            return _database.read_sql_query(table_id=data['table'], query_function=query, pk_column=data['pk_column'])
         return Exception(f"Can not read file extension {_f_type}, support [parquet, csv]")
         
     def read_df(self, file_id=None):
         _res = requests.get(f"{self._discovery_api}/file/{file_id}/", headers=self._jwt_header)
         if _res.status_code != 200:
             txt = _res.json() if _res.status_code < 500 else " "
             raise Exception(f"Some thing wrong, {txt}")
@@ -106,35 +121,17 @@
         _f_type = meta['type']['name']
         if _f_type == "parquet":
             return pd.read_parquet(f"s3://{bucket_name}/{meta['key']}", storage_options=self._storage_options)
         elif _f_type == "csv":
             return pd.read_csv(f"s3://{bucket_name}/{meta['key']}", storage_options=self._storage_options)
         return Exception(f"Can not read file extension {_f_type}, support [parquet, csv]")
     
-    def write_sql_query(self, query, directory_id, con_id, pk_column):
-        '''Write sql_connection in pickle with checking permission
-        
-        Args:
-        ...
-        '''
-        db = DatabaseManagement(token=self.token)
-        db.check_permission(con_id=con_id, table=table_name) # check permission before write sql connection
-        
-        sql_node_data = {
-            'query': query,
-            'con_id': con_id,
-            'pk_column': pk_column,
-        }
-        
-        # write pickle file to Discovery with special file extension (for changing icon in Discovery)
-        pass    
     
 class DatabaseManagement(Base):
-    
-    def get_connection_str(self, con_id=None):
+    def _get_connection_str(self, con_id=None):
         '''Get sqlalchemy connection string
         
         Args:
         ...
         '''
         if type(con_id) != int:
             raise Exception(f"Expect `con_id`=<int> but got {type(con_id)}, please input `con_id` eg con_id=0")
@@ -183,8 +180,61 @@
         ...
         '''
         for column in query.column_descriptions:
             table_name = column['expr'].table.name
             
             # check permission by using column['name'] and table_name
             if not self.check_permission(con_id=con_id, table=table_name, column=column['name']):
-                raise Exception(f"You don't have permission in table={table_name}, column={column['name']}")  
+                raise Exception(f"You don't have permission in table={table_name}, column={column['name']}")  
+            
+    def write_sql_query(self, query_function=None, directory_id=None, table_id=None, pk_column=None, name=None, desciption=None, *args, **kwargs):
+        '''Write sql_connection in pickle with checking permission
+        
+        Args:
+        ...
+        '''
+        
+        if query_function is None or inspect.isfunction(query_function)==False:
+            raise Exception(f"Expect `query`=<function> but got {type(query_function)}, please input `query`")
+        
+        if directory_id == None or type(directory_id) != int:
+            raise Exception(f"Please input data `directory`=<int>, but got {type(directory_id)} eg directory_id=0")
+        
+        if table_id == None or type(table_id) != int:
+            raise Exception(f"Please input data `table_id`=<int>, but got {type(table_id)} eg table_id=0")
+        
+        if pk_column == None or type(pk_column) != str:
+            raise Exception(f"Please input data `con_id`=<str>, but got {type(pk_column)} eg pk_column='id' ")
+        
+        if name == None or type(name) != str:
+            raise Exception(f"Please input data `name`=<str>, but got {type(name)} eg name='myData' ")
+        
+        if desciption == None:
+            desciption = f"query of {name}"
+        
+        _replace = self._check_fileExists(directory=directory_id, name=name)
+        
+        r = requests.post(f"{self._base_discovery_api}/api/sql/query/", headers=self._jwt_header,
+                          json={
+                                "directory": directory_id,
+                                "table": table_id,
+                                "name": name,
+                                "description": desciption,
+                                "pk_column": pk_column,
+                                "query": inspect.getsource(query_function),
+                                "replace": _replace
+                          }
+        )
+        return r.json() if r.status_code < 500 else r.content
+        
+    def read_sql_query(self, table_id=None, query_function=None, pk_column=None):
+        if table_id == None or type(table_id) != int:
+            raise Exception(f"Please input data `table_id`=<int>, but got {type(table_id)} eg table_id=0")
+        
+        if query_function is None or inspect.isfunction(query_function) == False:
+            raise Exception(f"Expect `query`=<function> but got {type(query_function)}, please input `query`")
+        
+        if pk_column == None or type(pk_column) != str:
+            raise Exception(f"Please input data `con_id`=<str>, but got {type(pk_column)} eg pk_column='id' ")
+        meta, schema = self.get_table_schema(table_id=table_id)
+        con_str = self._get_connection_str(con_id=meta['database'])
+        return dd.read_sql_query(sql=query_function(), con=con_str, index_col=pk_column)
```

### Comparing `dsmlibrary-1.0.8/dsmlibrary/dataset.py` & `dsmlibrary-1.0.9/dsmlibrary/dataset.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary-1.0.8/dsmlibrary/utils/clickhouse.py` & `dsmlibrary-1.0.9/dsmlibrary/utils/clickhouse.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary-1.0.8/dsmlibrary.egg-info/PKG-INFO` & `dsmlibrary-1.0.9/dsmlibrary.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 Metadata-Version: 2.1
 Name: dsmlibrary
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://gitlab.com/public-project2/dsm-library
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
+Description: # DSM Library
+        
+        ## DataNode
+        0. init DataNode
+        ```python
+        from dsmlibrary.datanode import DataNode 
+        
+        data = DataNode(token)
+        ```
+        1. upload file
+        ```python
+        data.upload_file(directory_id=<directory_id>, file_path='<file_path>', description="<description(optional)>")
+        ```
+        
+        2. download file
+        ```python
+        data.download_file(file_id=<file_id>, download_path="<place download file save> (default ./dsm.tmp)")
+        ```
+        3. get file
+        ```python
+        meta, file = get_file(file_id="<file_id>")
+        # meta -> dict
+        # file -> io bytes
+        ```
+        ```python
+        # example read csv pandas
+         
+        meta, file = get_file(file_id="<file_id>")
+        df = pd.read_csv(file)
+        ...
+        ``` 
+        
+        4. write parquet file
+        ```python
+        df = ... # pandas dataframe or dask dataframe
+        
+        data.write(df=df, directory=<directory_id>, name=<save_file_name>, profiling=<True or False default False>)
+        ```
+        
+        ## Clickhouse
+        1. imoprt data to clickhouse
+        
+        ```python
+        from dsmlibrary.clickhouse import ClickHouse
+        
+        ddf = ... # pandas dataframe or dask dataframe
+        
+        ## to warehouse
+        table_name = <your_table_name>
+        table_key = <your_table_key>
+        
+        connection = { 
+          'host': '', 
+          'port': , 
+          'database': '', 
+          'user': '', 
+          'password': '', 
+          'settings':{ 
+             'use_numpy': True 
+          }, 
+          'secure': False 
+        }
+        
+        warehouse = ClickHouse(connection=connection)
+        
+        tableName = warehouse.get_or_createTable(ddf=ddf, tableName=table_name, key=table_key)
+        warehouse.write(ddf=ddf, tableName=tableName, key=table_key)
+        ```
+        
+        2. query data from clickhouse
+        ```python
+        query = f""" 
+            SELECT * FROM {tableName} LIMIT 10 
+        """ 
+        warehouse.read(sqlQuery=query)
+        
+        ```
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-
-# DSM Library
-
-## DataNode
-0. init DataNode
-```python
-from dsmlibrary.datanode import DataNode 
-
-data = DataNode(token)
-```
-1. upload file
-```python
-data.upload_file(directory_id=<directory_id>, file_path='<file_path>', description="<description(optional)>")
-```
-
-2. download file
-```python
-data.download_file(file_id=<file_id>, download_path="<place download file save> (default ./dsm.tmp)")
-```
-3. get file
-```python
-meta, file = get_file(file_id="<file_id>")
-# meta -> dict
-# file -> io bytes
-```
-```python
-# example read csv pandas
- 
-meta, file = get_file(file_id="<file_id>")
-df = pd.read_csv(file)
-...
-``` 
-
-4. write parquet file
-```python
-df = ... # pandas dataframe or dask dataframe
-
-data.write(df=df, directory=<directory_id>, name=<save_file_name>, profiling=<True or False default False>)
-```
-
-## Clickhouse
-1. imoprt data to clickhouse
-
-```python
-from dsmlibrary.clickhouse import ClickHouse
-
-ddf = ... # pandas dataframe or dask dataframe
-
-## to warehouse
-table_name = <your_table_name>
-table_key = <your_table_key>
-
-connection = { 
-  'host': '', 
-  'port': , 
-  'database': '', 
-  'user': '', 
-  'password': '', 
-  'settings':{ 
-     'use_numpy': True 
-  }, 
-  'secure': False 
-}
-
-warehouse = ClickHouse(connection=connection)
-
-tableName = warehouse.get_or_createTable(ddf=ddf, tableName=table_name, key=table_key)
-warehouse.write(ddf=ddf, tableName=tableName, key=table_key)
-```
-
-2. query data from clickhouse
-```python
-query = f""" 
-    SELECT * FROM {tableName} LIMIT 10 
-""" 
-warehouse.read(sqlQuery=query)
-
-```
-
```

### Comparing `dsmlibrary-1.0.8/setup.py` & `dsmlibrary-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='dsmlibrary',
-    version='1.0.8',
+    version='1.0.9',
     url='https://gitlab.com/public-project2/dsm-library',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple way to use Dataset. for dsm',
     long_description=README,
     long_description_content_type='text/markdown',
```

