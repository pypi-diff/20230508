# Comparing `tmp/ipython-ngql-0.4.tar.gz` & `tmp/ipython-ngql-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython-ngql-0.4.tar", last modified: Thu May 27 12:29:33 2021, max compression
+gzip compressed data, was "ipython-ngql-0.5.tar", last modified: Mon May  8 10:25:57 2023, max compression
```

## Comparing `ipython-ngql-0.4.tar` & `ipython-ngql-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 weyl       (501) staff       (20)        0 2021-05-27 12:29:33.353870 ipython-ngql-0.4/
--rw-r--r--   0 weyl       (501) staff       (20)      545 2021-05-27 11:59:31.000000 ipython-ngql-0.4/LICENSE
--rw-r--r--   0 weyl       (501) staff       (20)    10366 2021-05-27 12:29:33.353744 ipython-ngql-0.4/PKG-INFO
--rw-r--r--   0 weyl       (501) staff       (20)     9809 2021-05-27 12:28:00.000000 ipython-ngql-0.4/README.md
-drwxr-xr-x   0 weyl       (501) staff       (20)        0 2021-05-27 12:29:33.353199 ipython-ngql-0.4/ipython_ngql.egg-info/
--rw-r--r--   0 weyl       (501) staff       (20)    10366 2021-05-27 12:29:33.000000 ipython-ngql-0.4/ipython_ngql.egg-info/PKG-INFO
--rw-r--r--   0 weyl       (501) staff       (20)      236 2021-05-27 12:29:33.000000 ipython-ngql-0.4/ipython_ngql.egg-info/SOURCES.txt
--rw-r--r--   0 weyl       (501) staff       (20)        1 2021-05-27 12:29:33.000000 ipython-ngql-0.4/ipython_ngql.egg-info/dependency_links.txt
--rw-r--r--   0 weyl       (501) staff       (20)       36 2021-05-27 12:29:33.000000 ipython-ngql-0.4/ipython_ngql.egg-info/requires.txt
--rw-r--r--   0 weyl       (501) staff       (20)        5 2021-05-27 12:29:33.000000 ipython-ngql-0.4/ipython_ngql.egg-info/top_level.txt
-drwxr-xr-x   0 weyl       (501) staff       (20)        0 2021-05-27 12:29:33.353481 ipython-ngql-0.4/ngql/
--rw-r--r--   0 weyl       (501) staff       (20)      111 2021-05-27 11:59:31.000000 ipython-ngql-0.4/ngql/__init__.py
--rw-r--r--   0 weyl       (501) staff       (20)     9258 2021-05-27 11:59:31.000000 ipython-ngql-0.4/ngql/magic.py
--rw-r--r--   0 weyl       (501) staff       (20)       38 2021-05-27 12:29:33.353902 ipython-ngql-0.4/setup.cfg
--rw-r--r--   0 weyl       (501) staff       (20)      879 2021-05-27 12:29:04.000000 ipython-ngql-0.4/setup.py
+drwxr-xr-x   0 weyl       (501) staff       (20)        0 2023-05-08 10:25:57.957041 ipython-ngql-0.5/
+-rw-r--r--   0 weyl       (501) staff       (20)      545 2023-05-08 06:34:44.000000 ipython-ngql-0.5/LICENSE
+-rw-r--r--   0 weyl       (501) staff       (20)     7561 2023-05-08 10:25:57.956854 ipython-ngql-0.5/PKG-INFO
+-rw-r--r--   0 weyl       (501) staff       (20)     7042 2023-05-08 10:25:50.000000 ipython-ngql-0.5/README.md
+drwxr-xr-x   0 weyl       (501) staff       (20)        0 2023-05-08 10:25:57.956053 ipython-ngql-0.5/ipython_ngql.egg-info/
+-rw-r--r--   0 weyl       (501) staff       (20)     7561 2023-05-08 10:25:57.000000 ipython-ngql-0.5/ipython_ngql.egg-info/PKG-INFO
+-rw-r--r--   0 weyl       (501) staff       (20)      236 2023-05-08 10:25:57.000000 ipython-ngql-0.5/ipython_ngql.egg-info/SOURCES.txt
+-rw-r--r--   0 weyl       (501) staff       (20)        1 2023-05-08 10:25:57.000000 ipython-ngql-0.5/ipython_ngql.egg-info/dependency_links.txt
+-rw-r--r--   0 weyl       (501) staff       (20)       29 2023-05-08 10:25:57.000000 ipython-ngql-0.5/ipython_ngql.egg-info/requires.txt
+-rw-r--r--   0 weyl       (501) staff       (20)        5 2023-05-08 10:25:57.000000 ipython-ngql-0.5/ipython_ngql.egg-info/top_level.txt
+drwxr-xr-x   0 weyl       (501) staff       (20)        0 2023-05-08 10:25:57.956610 ipython-ngql-0.5/ngql/
+-rw-r--r--   0 weyl       (501) staff       (20)      111 2023-05-08 06:34:44.000000 ipython-ngql-0.5/ngql/__init__.py
+-rw-r--r--   0 weyl       (501) staff       (20)    11965 2023-05-08 10:25:50.000000 ipython-ngql-0.5/ngql/magic.py
+-rw-r--r--   0 weyl       (501) staff       (20)       38 2023-05-08 10:25:57.957091 ipython-ngql-0.5/setup.cfg
+-rw-r--r--   0 weyl       (501) staff       (20)      871 2023-05-08 10:25:50.000000 ipython-ngql-0.5/setup.py
```

### Comparing `ipython-ngql-0.4/LICENSE` & `ipython-ngql-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipython-ngql-0.4/PKG-INFO` & `ipython-ngql-0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: ipython-ngql
-Version: 0.4
-Summary: iPython and Jupyter Plugin for Nebula Graph
+Version: 0.5
+Summary: iPython and Jupyter Plugin for NebulaGraph
 Home-page: https://github.com/wey-gu/ipython-ngql
 Author: Wey Gu
 Author-email: weyl.gu@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/wey-gu/ipython-ngql/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-> Note, this is an pre-release version. Becuase the tabular return resut is not yet fully supported in some queries.
->
-> Still you can use it with `%config IPythonNGQL.ngql_result_style="raw"`, after which line being executed, the result will be raw ResultSet.
->
-> If you like to use it, please let me know, I may put more time into this project to make the tabular work.
+`ipython-ngql` is a Python package to extend the ability to connect NebulaGraph from your Jupyter Notebook or iPython. It's easier for data scientists to create, debug and share reusable and all-in-one Jupyter Notebooks with Nebula Graph interaction embedded.
 
+`ipython-ngql`  is inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) created by [Catherine Devlin](https://catherinedevlin.blogspot.com/)
 
 
-`ipython-ngql` is a python package to extend the ability to connect Nebula Graph from your Jupyter Notebook or iPython. It's easier for data scientists to create, debug and share reusable and all-in-one Jupyter Notebooks with Nebula Graph interaction embedded.
 
-`ipython-ngql`  is inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) created by [Catherine Devlin](https://catherinedevlin.blogspot.com/)
+![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
+
+![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
+
 
-![get_started](https://github.com/wey-gu/ipython-ngql/blob/main/examples/get_started.png?raw=true)
 
 ## Get Started
 
 ### Installation
 
 `ipython-ngql` could be installed either via pip or from this git repo itself.
 
@@ -75,60 +71,75 @@
 ### Make Queries
 
 Now two kind of iPtython Magics are supported:
 
 Option 1: The one line stype with `%ngql`:
 
 ```python
-%ngql GO FROM "Tom" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id;
+%ngql USE basketballplayer;
+%ngql MATCH (v:player{name:"Tim Duncan"})-->(v2:player) RETURN v2.player.name AS Name;
 ```
 
 Option 2: The multiple lines stype with `%%ngql `
 
 ```python
 %%ngql
-USE pokemon_club;
 SHOW TAGS;
 SHOW HOSTS;
 ```
 
 > There will be other options in future, i.e. from a `.ngql` file.
 
 ### Query String with Variables
 
 `ipython-ngql` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
-In [8]: trainer = "Sue"
+In [8]: vid = "player100"
 
 In [9]: %%ngql
-   ...: GO FROM "{{ trainer }}" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
-   ...:
+   ...: MATCH (v)<-[e:follow]- (v2)-[e2:serve]->(v3)
+   ...:   WHERE id(v) == "{{ vid }}"
+   ...: RETURN v2.player.name AS FriendOf, v3.team.name AS Team LIMIT 3;
+Out[9]:   RETURN v2.player.name AS FriendOf, v3.team.name AS Team LIMIT 3;
+FriendOf	Team
+0	LaMarcus Aldridge	Trail Blazers
+1	LaMarcus Aldridge	Spurs
+2	Marco Belinelli	Warriors
+```
+
+### Draw query results
 
-Out[9]:
-  Trainer_Name
-0        Jerry
-1          Sue
-2          Tom
-3          Wey
+Just call `%ng_draw` after queries with graph data.
+
+```python
+# one query
+%ngql GET SUBGRAPH 2 STEPS FROM "player101" YIELD VERTICES AS nodes, EDGES AS relationships;
+%ng_draw
+
+# another query
+%ngql match p=(:player)-[]->() return p LIMIT 5
+%ng_draw
 ```
 
+![](https://user-images.githubusercontent.com/1651790/236797874-c142cfd8-b0de-4689-95ef-1da386e137d3.png)
+
 ### Configure `ngql_result_style`
 
-By default, `ipython-ngql` will use pandas dataframe as output style to enable more human readable output, while it's supported to use the raw thrift data format comes from the `nebula2-python` itself.
+By default, `ipython-ngql` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
 
 This can be done ad-hoc with below one line:
 
 ```python
 %config IPythonNGQL.ngql_result_style="raw"
 ```
 
-After above line being executed, the output will be like:
+After the above line is executed, the output will be like this:
 
 ```python
 ResultSet(ExecutionResponse(
     error_code=0,
     latency_in_us=2844,
     data=DataSet(
         column_names=[b'Trainer_Name'],
@@ -242,141 +253,26 @@
 #### Jupyter Notebook
 
 Please refer here:https://github.com/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb
 
 #### iPython
 
 ```python
-venv ❯ ipython
-
 In [1]: %load_ext ngql
 
-In [2]: %ngql --address 127.0.0.1 --port 9669 --user user --password password
+In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
 Connection Pool Created
-Out[2]:
-           Name
-0  pokemon_club
-
-In [3]: %ngql GO FROM "Tom" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name
-Out[3]:
-  Trainer_Name
-0          Tom
-1        Jerry
-2          Sue
-3          Tom
-4          Wey
-
-In [4]: %%ngql
-   ...: SHOW TAGS;
-   ...: SHOW HOSTS;
-   ...:
-   ...:
-Out[4]:
-        Host    Port  Status  Leader count Leader distribution Partition distribution
-0  storaged0  9779.0  ONLINE             0  No valid partition     No valid partition
-1  storaged1  9779.0  ONLINE             1      pokemon_club:1         pokemon_club:1
-2  storaged2  9779.0  ONLINE             0  No valid partition     No valid partition
-3      Total     NaN    None             1      pokemon_club:1         pokemon_club:1
-
-In [5]: trainer = "Sue"
-
-In [6]: %%ngql
-   ...: GO FROM "{{ trainer }}" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
-   ...:
-Out[6]:
-  Trainer_Name
-0        Jerry
-1          Sue
-2          Tom
-3          Wey
-
-In [7]: %ngql help
-
-
-        Supported Configurations:
-        ------------------------
-
-        > How to config ngql_result_style in "raw", "pandas"
-        %config IPythonNGQL.ngql_result_style="raw"
-        %config IPythonNGQL.ngql_result_style="pandas"
-
-        > How to config ngql_verbose in True, False
-        %config IPythonNGQL.ngql_verbose=True
-
-        > How to config max_connection_pool_size
-        %config IPythonNGQL.max_connection_pool_size=10
-
-        Quick Start:
-        -----------
-
-        > Connect to Neubla Graph
-        %ngql --address 127.0.0.1 --port 9669 --user user --password password
-
-        > Use Space
-        %ngql USE nba
-
-        > Query
-        %ngql SHOW TAGS;
-
-        > Multile Queries
-        %%ngql
-        SHOW TAGS;
-        SHOW HOSTS;
-
-        Reload ngql Magic
-        %reload_ext ngql
-
-        > Variables in query, we are using Jinja2 here
-        name = "nba"
-        %ngql USE "{{ name }}"
-
-In [8]: trainer = "Sue"
-
-In [9]: %%ngql
-   ...: GO FROM "{{ trainer }}" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
-   ...:
-   ...:
-Out[9]:
-  Trainer_Name
-0        Jerry
-1          Sue
-2          Tom
-3          Wey
-
-In [10]: %config IPythonNGQL.ngql_result_style="raw"
-
-In [11]: %%ngql USE pokemon_club;
-    ...: GO FROM "Tom" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id
-    ...: | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
-    ...:
-    ...:
-Out[11]:
-ResultSet(ExecutionResponse(
-    error_code=0,
-    latency_in_us=3270,
-    data=DataSet(
-        column_names=[b'Trainer_Name'],
-        rows=[Row(
-            values=[Value(
-                sVal=b'Tom')]),
-        Row(
-            values=[Value(
-                sVal=b'Jerry')]),
-        Row(
-            values=[Value(
-                sVal=b'Sue')]),
-        Row(
-            values=[Value(
-                sVal=b'Tom')]),
-        Row(
-            values=[Value(
-                sVal=b'Wey')])]),
-    space_name=b'pokemon_club'))
-
-In [12]: r = _
-
-In [13]: r.column_values(key='Trainer_Name')[0]._value.value
-Out[13]: b'Tom'
+Out[2]: 
+                        Name
+0           basketballplayer
+1  demo_movie_recommendation
+2                        k8s
+3                       test
+
+In [3]: %ngql USE basketballplayer;
+   ...: %ngql MATCH (v:player{name:"Tim Duncan"})-->(v2:player) RETURN v2.player.name AS Name;
+Out[3]: 
+            Name
+0    Tony Parker
+1  Manu Ginobili
 ```
 
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ipython-ngql-0.4/README.md` & `ipython-ngql-0.5/ipython_ngql.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,33 @@
-> Note, this is an pre-release version. Becuase the tabular return resut is not yet fully supported in some queries.
->
-> Still you can use it with `%config IPythonNGQL.ngql_result_style="raw"`, after which line being executed, the result will be raw ResultSet.
->
-> If you like to use it, please let me know, I may put more time into this project to make the tabular work.
+Metadata-Version: 2.1
+Name: ipython-ngql
+Version: 0.5
+Summary: iPython and Jupyter Plugin for NebulaGraph
+Home-page: https://github.com/wey-gu/ipython-ngql
+Author: Wey Gu
+Author-email: weyl.gu@gmail.com
+Project-URL: Bug Tracker, https://github.com/wey-gu/ipython-ngql/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
+`ipython-ngql` is a Python package to extend the ability to connect NebulaGraph from your Jupyter Notebook or iPython. It's easier for data scientists to create, debug and share reusable and all-in-one Jupyter Notebooks with Nebula Graph interaction embedded.
 
+`ipython-ngql`  is inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) created by [Catherine Devlin](https://catherinedevlin.blogspot.com/)
 
-`ipython-ngql` is a python package to extend the ability to connect Nebula Graph from your Jupyter Notebook or iPython. It's easier for data scientists to create, debug and share reusable and all-in-one Jupyter Notebooks with Nebula Graph interaction embedded.
 
-`ipython-ngql`  is inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) created by [Catherine Devlin](https://catherinedevlin.blogspot.com/)
 
-![get_started](https://github.com/wey-gu/ipython-ngql/blob/main/examples/get_started.png?raw=true)
+![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
+
+![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
+
+
 
 ## Get Started
 
 ### Installation
 
 `ipython-ngql` could be installed either via pip or from this git repo itself.
 
@@ -58,60 +71,75 @@
 ### Make Queries
 
 Now two kind of iPtython Magics are supported:
 
 Option 1: The one line stype with `%ngql`:
 
 ```python
-%ngql GO FROM "Tom" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id;
+%ngql USE basketballplayer;
+%ngql MATCH (v:player{name:"Tim Duncan"})-->(v2:player) RETURN v2.player.name AS Name;
 ```
 
 Option 2: The multiple lines stype with `%%ngql `
 
 ```python
 %%ngql
-USE pokemon_club;
 SHOW TAGS;
 SHOW HOSTS;
 ```
 
 > There will be other options in future, i.e. from a `.ngql` file.
 
 ### Query String with Variables
 
 `ipython-ngql` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
-In [8]: trainer = "Sue"
+In [8]: vid = "player100"
 
 In [9]: %%ngql
-   ...: GO FROM "{{ trainer }}" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
-   ...:
+   ...: MATCH (v)<-[e:follow]- (v2)-[e2:serve]->(v3)
+   ...:   WHERE id(v) == "{{ vid }}"
+   ...: RETURN v2.player.name AS FriendOf, v3.team.name AS Team LIMIT 3;
+Out[9]:   RETURN v2.player.name AS FriendOf, v3.team.name AS Team LIMIT 3;
+FriendOf	Team
+0	LaMarcus Aldridge	Trail Blazers
+1	LaMarcus Aldridge	Spurs
+2	Marco Belinelli	Warriors
+```
 
-Out[9]:
-  Trainer_Name
-0        Jerry
-1          Sue
-2          Tom
-3          Wey
+### Draw query results
+
+Just call `%ng_draw` after queries with graph data.
+
+```python
+# one query
+%ngql GET SUBGRAPH 2 STEPS FROM "player101" YIELD VERTICES AS nodes, EDGES AS relationships;
+%ng_draw
+
+# another query
+%ngql match p=(:player)-[]->() return p LIMIT 5
+%ng_draw
 ```
 
+![](https://user-images.githubusercontent.com/1651790/236797874-c142cfd8-b0de-4689-95ef-1da386e137d3.png)
+
 ### Configure `ngql_result_style`
 
-By default, `ipython-ngql` will use pandas dataframe as output style to enable more human readable output, while it's supported to use the raw thrift data format comes from the `nebula2-python` itself.
+By default, `ipython-ngql` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
 
 This can be done ad-hoc with below one line:
 
 ```python
 %config IPythonNGQL.ngql_result_style="raw"
 ```
 
-After above line being executed, the output will be like:
+After the above line is executed, the output will be like this:
 
 ```python
 ResultSet(ExecutionResponse(
     error_code=0,
     latency_in_us=2844,
     data=DataSet(
         column_names=[b'Trainer_Name'],
@@ -225,139 +253,26 @@
 #### Jupyter Notebook
 
 Please refer here:https://github.com/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb
 
 #### iPython
 
 ```python
-venv ❯ ipython
-
 In [1]: %load_ext ngql
 
-In [2]: %ngql --address 127.0.0.1 --port 9669 --user user --password password
+In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
 Connection Pool Created
-Out[2]:
-           Name
-0  pokemon_club
-
-In [3]: %ngql GO FROM "Tom" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name
-Out[3]:
-  Trainer_Name
-0          Tom
-1        Jerry
-2          Sue
-3          Tom
-4          Wey
-
-In [4]: %%ngql
-   ...: SHOW TAGS;
-   ...: SHOW HOSTS;
-   ...:
-   ...:
-Out[4]:
-        Host    Port  Status  Leader count Leader distribution Partition distribution
-0  storaged0  9779.0  ONLINE             0  No valid partition     No valid partition
-1  storaged1  9779.0  ONLINE             1      pokemon_club:1         pokemon_club:1
-2  storaged2  9779.0  ONLINE             0  No valid partition     No valid partition
-3      Total     NaN    None             1      pokemon_club:1         pokemon_club:1
-
-In [5]: trainer = "Sue"
-
-In [6]: %%ngql
-   ...: GO FROM "{{ trainer }}" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
-   ...:
-Out[6]:
-  Trainer_Name
-0        Jerry
-1          Sue
-2          Tom
-3          Wey
-
-In [7]: %ngql help
-
-
-        Supported Configurations:
-        ------------------------
-
-        > How to config ngql_result_style in "raw", "pandas"
-        %config IPythonNGQL.ngql_result_style="raw"
-        %config IPythonNGQL.ngql_result_style="pandas"
-
-        > How to config ngql_verbose in True, False
-        %config IPythonNGQL.ngql_verbose=True
-
-        > How to config max_connection_pool_size
-        %config IPythonNGQL.max_connection_pool_size=10
-
-        Quick Start:
-        -----------
-
-        > Connect to Neubla Graph
-        %ngql --address 127.0.0.1 --port 9669 --user user --password password
-
-        > Use Space
-        %ngql USE nba
-
-        > Query
-        %ngql SHOW TAGS;
-
-        > Multile Queries
-        %%ngql
-        SHOW TAGS;
-        SHOW HOSTS;
-
-        Reload ngql Magic
-        %reload_ext ngql
-
-        > Variables in query, we are using Jinja2 here
-        name = "nba"
-        %ngql USE "{{ name }}"
-
-In [8]: trainer = "Sue"
-
-In [9]: %%ngql
-   ...: GO FROM "{{ trainer }}" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
-   ...:
-   ...:
-Out[9]:
-  Trainer_Name
-0        Jerry
-1          Sue
-2          Tom
-3          Wey
-
-In [10]: %config IPythonNGQL.ngql_result_style="raw"
-
-In [11]: %%ngql USE pokemon_club;
-    ...: GO FROM "Tom" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id
-    ...: | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
-    ...:
-    ...:
-Out[11]:
-ResultSet(ExecutionResponse(
-    error_code=0,
-    latency_in_us=3270,
-    data=DataSet(
-        column_names=[b'Trainer_Name'],
-        rows=[Row(
-            values=[Value(
-                sVal=b'Tom')]),
-        Row(
-            values=[Value(
-                sVal=b'Jerry')]),
-        Row(
-            values=[Value(
-                sVal=b'Sue')]),
-        Row(
-            values=[Value(
-                sVal=b'Tom')]),
-        Row(
-            values=[Value(
-                sVal=b'Wey')])]),
-    space_name=b'pokemon_club'))
-
-In [12]: r = _
-
-In [13]: r.column_values(key='Trainer_Name')[0]._value.value
-Out[13]: b'Tom'
+Out[2]: 
+                        Name
+0           basketballplayer
+1  demo_movie_recommendation
+2                        k8s
+3                       test
+
+In [3]: %ngql USE basketballplayer;
+   ...: %ngql MATCH (v:player{name:"Tim Duncan"})-->(v2:player) RETURN v2.player.name AS Name;
+Out[3]: 
+            Name
+0    Tony Parker
+1  Manu Ginobili
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ipython-ngql-0.4/setup.py` & `ipython-ngql-0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipython-ngql",
-    version="0.4",
+    version="0.5",
     author="Wey Gu",
     author_email="weyl.gu@gmail.com",
-    description="iPython and Jupyter Plugin for Nebula Graph",
+    description="iPython and Jupyter Plugin for NebulaGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wey-gu/ipython-ngql",
     project_urls={
         "Bug Tracker": "https://github.com/wey-gu/ipython-ngql/issues",
     },
     classifiers=[
@@ -20,11 +20,11 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
     install_requires=[
         'Jinja2',
-        'nebula2-python==2.0.0',
+        'nebula3-python',
         'pandas',
     ],
 )
```

