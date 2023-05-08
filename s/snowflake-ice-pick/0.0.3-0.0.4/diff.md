# Comparing `tmp/snowflake_ice_pick-0.0.3.tar.gz` & `tmp/snowflake_ice_pick-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake_ice_pick-0.0.3.tar", last modified: Thu Apr 20 02:03:35 2023, max compression
+gzip compressed data, was "C:\Snowflake\snowflake_ice_pick\dist\.tmp-g4bfg6q3\snowflake_ice_pick-0.0.4.tar", last modified: Mon May  8 15:14:18 2023, max compression
```

## Comparing `snowflake_ice_pick-0.0.3.tar` & `snowflake_ice_pick-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 02:03:35.982477 snowflake_ice_pick-0.0.3/
--rw-rw-rw-   0        0        0     1103 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-19 15:06:48.000000 snowflake_ice_pick-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5550 2023-04-20 02:03:35.982977 snowflake_ice_pick-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3601 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/README.md
--rw-rw-rw-   0        0        0     1167 2023-04-20 02:02:50.000000 snowflake_ice_pick-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      842 2023-04-20 02:03:35.984974 snowflake_ice_pick-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-19 16:32:29.000000 snowflake_ice_pick-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 02:03:35.944975 snowflake_ice_pick-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 02:03:35.963984 snowflake_ice_pick-0.0.3/src/ice_pick/
--rw-rw-rw-   0        0        0      781 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/__init__.py
--rw-rw-rw-   0        0        0    19806 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/account_object.py
--rw-rw-rw-   0        0        0     2746 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/extension.py
--rw-rw-rw-   0        0        0    10718 2023-04-20 02:00:08.000000 snowflake_ice_pick-0.0.3/src/ice_pick/filter.py
--rw-rw-rw-   0        0        0     6473 2023-04-20 01:50:52.000000 snowflake_ice_pick-0.0.3/src/ice_pick/schema_object.py
--rw-rw-rw-   0        0        0     8914 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/utils.py
--rw-rw-rw-   0        0        0      158 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/version.py
-drwxrwxrwx   0        0        0        0 2023-04-20 02:03:35.980976 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/
--rw-rw-rw-   0        0        0     5550 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 15:14:18.302052 snowflake_ice_pick-0.0.4/
+-rw-rw-rw-   0        0        0     1103 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-19 15:06:48.000000 snowflake_ice_pick-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5550 2023-05-08 15:14:18.302554 snowflake_ice_pick-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3601 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1167 2023-05-03 14:15:27.000000 snowflake_ice_pick-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      842 2023-05-08 15:14:18.304555 snowflake_ice_pick-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-19 16:32:29.000000 snowflake_ice_pick-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:14:18.244052 snowflake_ice_pick-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 15:14:18.280053 snowflake_ice_pick-0.0.4/src/ice_pick/
+-rw-rw-rw-   0        0        0     1161 2023-05-08 13:24:44.000000 snowflake_ice_pick-0.0.4/src/ice_pick/__init__.py
+-rw-rw-rw-   0        0        0    21457 2023-05-08 14:05:53.000000 snowflake_ice_pick-0.0.4/src/ice_pick/account_object.py
+-rw-rw-rw-   0        0        0     5072 2023-05-08 13:37:38.000000 snowflake_ice_pick-0.0.4/src/ice_pick/extension.py
+-rw-rw-rw-   0        0        0    21141 2023-05-08 02:54:18.000000 snowflake_ice_pick-0.0.4/src/ice_pick/filters.py
+-rw-rw-rw-   0        0        0     7809 2023-05-08 13:24:39.000000 snowflake_ice_pick-0.0.4/src/ice_pick/privileges.py
+-rw-rw-rw-   0        0        0     8145 2023-05-08 14:02:34.000000 snowflake_ice_pick-0.0.4/src/ice_pick/schema_object.py
+-rw-rw-rw-   0        0        0     9688 2023-05-08 02:22:47.000000 snowflake_ice_pick-0.0.4/src/ice_pick/utils.py
+-rw-rw-rw-   0        0        0      158 2023-05-03 14:15:10.000000 snowflake_ice_pick-0.0.4/src/ice_pick/version.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:14:18.300553 snowflake_ice_pick-0.0.4/src/snowflake_ice_pick.egg-info/
+-rw-rw-rw-   0        0        0     5550 2023-05-08 15:14:18.000000 snowflake_ice_pick-0.0.4/src/snowflake_ice_pick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-05-08 15:14:18.000000 snowflake_ice_pick-0.0.4/src/snowflake_ice_pick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 15:14:18.000000 snowflake_ice_pick-0.0.4/src/snowflake_ice_pick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2023-05-08 15:14:18.000000 snowflake_ice_pick-0.0.4/src/snowflake_ice_pick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 15:14:18.000000 snowflake_ice_pick-0.0.4/src/snowflake_ice_pick.egg-info/top_level.txt
```

### Comparing `snowflake_ice_pick-0.0.3/LICENSE` & `snowflake_ice_pick-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_ice_pick-0.0.3/PKG-INFO` & `snowflake_ice_pick-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake_ice_pick
-Version: 0.0.3
+Version: 0.0.4
 Summary: Snowpark extension to cover additional objects and higher level functions
 Author: Preston Blackburn
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Preston Blackburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `snowflake_ice_pick-0.0.3/README.md` & `snowflake_ice_pick-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_ice_pick-0.0.3/pyproject.toml` & `snowflake_ice_pick-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools>=65.5.1", "wheel"]  # PEP 518 specifications.
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "snowflake_ice_pick"
 description = "Snowpark extension to cover additional objects and higher level functions"
-version = "0.0.3"
+version = "0.0.4"
 readme = "README.md"
 authors = [{name = "Preston Blackburn"}]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `snowflake_ice_pick-0.0.3/setup.cfg` & `snowflake_ice_pick-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowflake_ice_pick-0.0.3/src/ice_pick/account_object.py` & `snowflake_ice_pick-0.0.4/src/ice_pick/account_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from snowflake.snowpark import Session
 import snowflake.snowpark as snowpark
 from ice_pick.utils import snowpark_query
 from ice_pick.schema_object import SchemaObject
 
 import pandas as pd
 
+import ice_pick
+
 
 # Account Objects
 # DATABASE
 # INTEGRATION
 # NETWORK POLICY
 # SHARE
 # USER
@@ -22,14 +24,25 @@
 # SCHEMA
 # ROLE
 # SHARES
 # GRANTS
 # RESOURCE MONITOR
 
 
+class Account:
+    """
+        (TODO - see how this is handled in snowflake)   
+        For now here just as a reminder and to help with global privileges
+        Some things can only be accessed at the account level
+    """
+    def __init__(self, session):
+        self.session = session
+
+
+
 # might remove this class, it seems like a lot of account objects have their own rules
 class AccountObject:
     def __init__(self, session, name: str, object_type: str):
         self.session = session
         self.name = name
         self.object_type = object_type
 
@@ -109,14 +122,50 @@
 
         """
         grants_sql = f""" show grants on {self.object_type} "{self.name}" """
 
         grants_df = snowpark_query(self.session, grants_sql, non_select=True)
 
         return grants_df
+    
+
+    def get_grant_objects(self) -> list:
+
+        if self.object_type == "schema":
+            # need to qualify schema with database name
+            # handle later
+        
+            return []
+        
+        grants_sql = f""" show grants on {self.object_type} "{self.name}" """
+
+        grants_df = snowpark_query(self.session, grants_sql, non_select=True)
+
+        
+        if "privilege" not in grants_df.columns.tolist():
+            # need to look into this case
+            # I think it is for the information schema maybe?
+            return []
+        
+        
+        # create privilege
+        grants_df['Privilege_Obj'] = grants_df.apply(lambda x: ice_pick.privileges.Privilege(self, x['privilege']), axis = 1)
+        
+        grants_df['Role_Obj'] = grants_df['granted_to'].apply(lambda x: Role(self.session, x))
+       
+        grants_df['Grant_Obj'] = grants_df.apply(
+            lambda x: ice_pick.privileges.Grant(
+            self.session, x['Privilege_Obj'], x['Role_Obj'], x['privilege']), axis=1 )
+        
+        grant_objects = grants_df['Grant_Obj'].tolist()
+
+        return grant_objects
+    
+
+
 
     def drop(self):
         """
         drops object
 
         Supports:
         most objects
@@ -161,14 +210,16 @@
 
 
 class Role(AccountObject):
     def __init__(self, session, name: str):
         super().__init__(session, name, "role")
 
     def show_grants_of(self):
+
+
         return
 
     def show_grants_to(self):
         show_grants_sql = f""" show grants to role {self.name}"""
 
         grants_to_df = snowpark_query(self.session, show_grants_sql, non_select=True)
 
@@ -605,8 +656,12 @@
 class Integration(AccountObject):
     def __init__(self, session, name: str):
         super().__init__(session, name, "integration")
 
 
 class NetworkPolicy(AccountObject):
     def __init__(self, session, name: str):
-        super().__init__(session, name, "schema")
+        super().__init__(session, name, "network policy")
+
+class ResourceMonitor(AccountObject):
+    def __init__(self, session, name: str):
+        super().__init__(session, name, "resource monitor")
```

### Comparing `snowflake_ice_pick-0.0.3/src/ice_pick/extension.py` & `snowflake_ice_pick-0.0.4/src/ice_pick/extension.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,134 @@
 """
 The extensions module monkey patches the Snowpark Session to add additional functionality.
 For now this is to give ice_pick a more native feel, where added ice_pick functions can be called from the Snowpark Session class.
 """
 
 from snowflake.snowpark import Session
+from typing import List, Union, Literal
 
 from ice_pick.schema_object import SchemaObject
-from ice_pick.filter import SchemaObjectFilter
+from ice_pick.account_object import (
+    AccountObject,
+    Account,
+    Warehouse, 
+    Role, 
+    User,
+    Database,
+    Schema,
+    Integration,
+    NetworkPolicy,
+    ResourceMonitor,
+)
+
+from ice_pick.filters import SchemaObjectFilter, AccountObjectFilter
 from ice_pick.utils import concat_standalone
 from ice_pick.utils import melt_standalone
 
 from ice_pick.account_object import AccountObject, Warehouse, Role, User
 
+from ice_pick.privileges import Privilege, Grant
+
+
+# todo - create a wrapper/decorator to help with monkey patching
+# (can probably do most of this at the function level instead of importing everyting)
 
-# todo - create a wrapper to help with monkey patching
 
 
+# -----------------------  Schema Level Extensions ----------------------------
+
 def create_schema_object(self, database, schema, object_name, object_type):
     return SchemaObject(self, database, schema, object_name, object_type)
 
-
 def create_schema_object_filter(
     self,
     databases,
     schemas,
     object_names,
     object_types,
     ignore_dbs=["SNOWFLAKE_SAMPLE_DATA", "SNOWFLAKE"],
     ignore_schemas=["INFORMATION_SCHEMA"],
 ):
     return SchemaObjectFilter(
         self, databases, schemas, object_names, object_types, ignore_dbs, ignore_schemas
     )
 
 
+
+
+
+# -----------------------  Account Level Extensions ----------------------------
+
 def create_account_object(self, name, object_type):
     return AccountObject(self, name, object_type)
 
-
 def create_warehouse(self, name):
     return Warehouse(self, name)
 
-
 def create_role(self, name):
     return Role(self, name)
 
-
 def create_user(self, name):
     return User(self, name)
 
+def create_database(self, name):
+    return Database(self, name)
+
+def create_schema(self, name):
+    return Schema(self, name)
+
+def create_integration(self, name):
+    return Integration(self, name)
+
+def create_network_policy(self, name):
+    return NetworkPolicy(self, name)
+
+def create_resource_monitor(self, name):
+    return ResourceMonitor(self, name)
+
+
+def create_account_object_filter(
+       self,
+       object_names,
+       object_types,
+       ignore_names = None,
+):
+    return AccountObjectFilter(
+        self, object_names, object_types, ignore_names
+    )
+
+
+
+# ----------------------- Privileges/Grants -----------------------------
+
+
+def create_privilege(
+        object: Union[SchemaObject, AccountObject, Account],
+        privilege:str,
+     ):
+    
+    return Privilege(object, privilege)
+
+
+def create_grant(
+        self,
+        session: Session, 
+        privilege: Privilege,
+        role: Role,
+        grant_option: str = None,
+        future_str: str = None
+):
+    return Grant(
+        self, privilege, role, grant_option, future_str
+    )
+
+
+
+
+# ---------------------  Pandas like utils --------------------------
 
 def concat(self, union_dfs: list):
     unioned_dfs = concat_standalone(self, union_dfs)
 
     return unioned_dfs
 
 
@@ -67,14 +143,20 @@
     melt_df = melt_standalone(
         self, df, id_vars, value_vars, var_name=var_name, value_name=value_name
     )
 
     return melt_df
 
 
+
+
+
+
+# -----------------------  Extend the session with the new functionality  ---------------------------
+
 def extend_session(Session: Session) -> Session:
     """
     Returns the extended Session class
 
     Parameters
     ----------
     session : Session
@@ -91,17 +173,30 @@
     """
 
     # adding the methods to create the schema objects
     Session.create_schema_object = create_schema_object
     Session.create_schema_object_filter = create_schema_object_filter
 
     # adding the methods to create the account objects
-    Session.AccountObject = create_account_object
-    Session.Role = create_role
-    Session.Warehouse = create_warehouse
-    Session.User = create_user
+    Session.create_account_object = create_account_object
+    Session.role = create_role
+    Session.warehouse = create_warehouse
+    Session.user = create_user
+    Session.database = create_database
+    Session.schema = create_schema
+    Session.integration = create_integration
+    Session.network_policy = create_network_policy
+    Session.resource_monitor = create_resource_monitor
+
+    Session.create_account_object_filter = create_account_object_filter
+    
+
+    # permission handling
+    Session.privilege = create_privilege
+    Session.grant = create_grant
+    
 
     # adding the methods to create misc functions
     Session.concat = concat
     Session.melt = melt
 
     return Session
```

### Comparing `snowflake_ice_pick-0.0.3/src/ice_pick/schema_object.py` & `snowflake_ice_pick-0.0.4/src/ice_pick/schema_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from snowflake.snowpark.row import Row
 
 import pandas as pd
 import numpy as np
 
 from ice_pick.utils import snowpark_query
 
+import ice_pick
+
 
 @dataclass
 class SchemaObject:
     """Represents a Snowflake Schema object.
 
     Schema Objects Include: ALERTS, EXTERNAL FUNCTIONS, EXTERNAL TABLES, FILE FORMATS,
     MATERIALIZED VIEWS, MASKING POLICIES, PASSWORD POLICIES, PIPES, PROCEDURES,
@@ -110,14 +112,50 @@
         Return a list of grants on the schema object as a list
         """
         grants_sql = f"""show grants on {self.object_type} 
                     "{self.database}"."{self.schema}"."{self.object_name}";"""
         grants_df = snowpark_query(self.session, grants_sql, non_select=True)
 
         return grants_df
+    
+    def get_grant_objects(self) -> list:
+        
+        object_exceptions = ['USER FUNCTION', 'PROCEDURE']
+
+        if self.object_type not in object_exceptions:
+            grants_sql = f""" show grants on {self.object_type} "{self.database}"."{self.schema}"."{self.object_name}" """
+        elif self.object_type == "USER FUNCTION":
+            func_name = self.object_name.split("(")[0]
+            func_args = "(" + self.object_name.split("(")[-1]
+            grants_sql = f""" show grants on FUNCTION "{self.database}"."{self.schema}"."{func_name}"{func_args} """
+        else:
+            func_name = self.object_name.split("(")[0]
+            func_args = "(" + self.object_name.split("(")[-1]
+            grants_sql = f""" show grants on {self.object_type} "{self.database}"."{self.schema}"."{func_name}"{func_args} """
+
+
+        grants_df = snowpark_query(self.session, grants_sql, non_select=True)
+        
+        # create privilege
+        if "privilege" not in grants_df.columns.tolist():
+            # need to look into this case
+            return []
+        
+        grants_df['Privilege_Obj'] = grants_df['privilege'].apply(lambda x: ice_pick.privileges.Privilege(self, x))
+        
+        grants_df['Role_Obj'] = grants_df['grantee_name'].apply(lambda x: ice_pick.account_object.Role(self.session, x))
+       
+        grants_df['Grant_Obj'] = grants_df.apply(
+            lambda x: ice_pick.privileges.Grant(
+            self.session, x['Privilege_Obj'], x['Role_Obj'], x['privilege']), axis=1 )
+        
+        grant_objects = grants_df['Grant_Obj'].tolist()
+
+        return grant_objects
+
 
     def grant(self, privilege: list, grantee: str) -> str:
         """grant access on object, return status
 
         | -- For TABLE
         |   { SELECT | INSERT | UPDATE | DELETE | TRUNCATE | REFERENCES } [ , ... ]
         | -- For VIEW
```

### Comparing `snowflake_ice_pick-0.0.3/src/ice_pick/utils.py` & `snowflake_ice_pick-0.0.4/src/ice_pick/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass, field
 from typing import List
 import copy
 import re
 import configparser
+import functools
 
 from snowflake.snowpark import Session
 import snowflake.snowpark as snowpark
 from snowflake.snowpark.row import Row
 from snowflake.snowpark.types import (
     IntegerType,
     StringType,
@@ -17,23 +18,37 @@
 )
 from snowflake.snowpark.functions import lit
 
 import pandas as pd
 import numpy as np
 
 
+# decorator for dry run sql
+class SQLTracker:
+    def __init__(self, func):
+        functools.update_wrapper(self, func)
+        self.func = func
+        self.sql = []
+
+    def __call__(self, *args, **kwargs):
+        self.sql.append(args[1])
+        return self.func(*args, **kwargs)
+    
+
 # maybe add an option to log all sql executions
+# and collect all of the sql before execution?
+# --- That could make it more confusing if sql isn't executed right away
 # could be nice to have more transparency
 # (at least add logging for debugging)
-def snowpark_query(session, sql, non_select=False):
+@SQLTracker
+def snowpark_query(session, sql, non_select=False, dry=False, collect=False):
     """
     non-select queries include things like:
      "show databases;"
 
-
     """
 
     if non_select:
         # apply the Row function "as_dict" to all rows then conver to pandas
         row_objs = session.sql(sql).collect()
 
         dict_array = np.array(list(map(Row.as_dict, row_objs)))
@@ -44,14 +59,32 @@
 
     else:
         df = session.sql(sql).to_pandas()
 
         return df
 
 
+
+# ----------------------   Account State Management --------------------------
+# Is this out of scope?
+# Should this just be filter?
+
+
+
+
+
+
+
+
+
+
+
+
+# ---------------------   Pandas-like Functionality  --------------------
+# (mostly just to cover edge cases, or features I want)
 ### Auto union
 def _get_schemas(union_dfs: list) -> list:
     # get a flat list of all structs in all dataframes
     struct_field_list = []
     for df in union_dfs:
         structs = df.schema.fields
         for struct in structs:
```

### Comparing `snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/PKG-INFO` & `snowflake_ice_pick-0.0.4/src/snowflake_ice_pick.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-ice-pick
-Version: 0.0.3
+Version: 0.0.4
 Summary: Snowpark extension to cover additional objects and higher level functions
 Author: Preston Blackburn
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Preston Blackburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

