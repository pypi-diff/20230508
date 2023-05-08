# Comparing `tmp/uintel-0.4.1.tar.gz` & `tmp/uintel-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uintel-0.4.1.tar", last modified: Mon May  8 03:47:47 2023, max compression
+gzip compressed data, was "uintel-0.4.2.tar", last modified: Mon May  8 03:59:51 2023, max compression
```

## Comparing `uintel-0.4.1.tar` & `uintel-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:47:47.657773 uintel-0.4.1/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1075 2023-04-03 04:47:18.000000 uintel-0.4.1/LICENSE
--rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-05-08 03:47:47.657773 uintel-0.4.1/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)     3274 2023-04-03 04:47:18.000000 uintel-0.4.1/README.md
--rw-rw-r--   0 sam       (1000) sam       (1000)       95 2023-04-03 04:47:18.000000 uintel-0.4.1/pyproject.toml
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-05-08 03:47:47.657773 uintel-0.4.1/setup.cfg
--rw-rw-r--   0 sam       (1000) sam       (1000)     1560 2023-05-08 03:47:15.000000 uintel-0.4.1/setup.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:47:47.653773 uintel-0.4.1/src/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:47:47.653773 uintel-0.4.1/src/uintel/
--rw-rw-r--   0 sam       (1000) sam       (1000)     3030 2023-04-03 04:47:18.000000 uintel-0.4.1/src/uintel/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7978 2023-05-05 02:33:43.000000 uintel-0.4.1/src/uintel/aws.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     4657 2023-04-03 04:47:18.000000 uintel-0.4.1/src/uintel/colours.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    10626 2023-05-05 02:33:43.000000 uintel-0.4.1/src/uintel/esri.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:47:47.657773 uintel-0.4.1/src/uintel/fonts/
--rw-rw-r--   0 sam       (1000) sam       (1000)    94884 2023-04-03 04:47:18.000000 uintel-0.4.1/src/uintel/fonts/Myriad Pro (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)   208636 2023-04-03 04:47:18.000000 uintel-0.4.1/src/uintel/fonts/Rubik (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)   202424 2023-04-03 04:47:18.000000 uintel-0.4.1/src/uintel/fonts/Rubik Italic (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)    20290 2023-05-05 02:33:43.000000 uintel-0.4.1/src/uintel/geometry.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    23184 2023-04-03 04:47:18.000000 uintel-0.4.1/src/uintel/install.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2308 2023-04-03 04:47:18.000000 uintel-0.4.1/src/uintel/ogc.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3808 2023-04-03 04:47:18.000000 uintel-0.4.1/src/uintel/query.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7934 2023-05-05 02:33:43.000000 uintel-0.4.1/src/uintel/server.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    13281 2023-05-05 02:33:43.000000 uintel-0.4.1/src/uintel/slack.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6413 2023-05-08 03:47:08.000000 uintel-0.4.1/src/uintel/sql.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:47:47.657773 uintel-0.4.1/src/uintel/styles/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1046 2023-04-03 04:47:18.000000 uintel-0.4.1/src/uintel/styles/ui.mplstyle
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:47:47.657773 uintel-0.4.1/src/uintel.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-05-08 03:47:47.000000 uintel-0.4.1/src/uintel.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      590 2023-05-08 03:47:47.000000 uintel-0.4.1/src/uintel.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-05-08 03:47:47.000000 uintel-0.4.1/src/uintel.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)      158 2023-05-08 03:47:47.000000 uintel-0.4.1/src/uintel.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        7 2023-05-08 03:47:47.000000 uintel-0.4.1/src/uintel.egg-info/top_level.txt
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.147077 uintel-0.4.2/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1075 2023-04-03 04:47:18.000000 uintel-0.4.2/LICENSE
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-05-08 03:59:51.147077 uintel-0.4.2/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3274 2023-04-03 04:47:18.000000 uintel-0.4.2/README.md
+-rw-rw-r--   0 sam       (1000) sam       (1000)       95 2023-04-03 04:47:18.000000 uintel-0.4.2/pyproject.toml
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-05-08 03:59:51.147077 uintel-0.4.2/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1560 2023-05-08 03:59:33.000000 uintel-0.4.2/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.139077 uintel-0.4.2/src/
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.143077 uintel-0.4.2/src/uintel/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3030 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7978 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/aws.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4657 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/colours.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    10626 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/esri.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.143077 uintel-0.4.2/src/uintel/fonts/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    94884 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/fonts/Myriad Pro (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   208636 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/fonts/Rubik (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   202424 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/fonts/Rubik Italic (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)    20290 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/geometry.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    23184 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/install.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2308 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/ogc.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3808 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/query.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7934 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/server.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    13281 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/slack.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6374 2023-05-08 03:59:28.000000 uintel-0.4.2/src/uintel/sql.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.147077 uintel-0.4.2/src/uintel/styles/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1046 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/styles/ui.mplstyle
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.143077 uintel-0.4.2/src/uintel.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      590 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)      158 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        7 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/top_level.txt
```

### Comparing `uintel-0.4.1/LICENSE` & `uintel-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/PKG-INFO` & `uintel-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.4.1
+Version: 0.4.2
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.4.1/README.md` & `uintel-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/setup.py` & `uintel-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 setuptools.setup(
     # State the generic information about the package
     name='uintel',
-    version='0.4.1',
+    version='0.4.2',
     author="Sam Archie",
     author_email="sam.archie@urbanintelligence.co.nz",
     description="Urban Intelligence's unified Python data analysis toolkit",
     long_description=open('README.md').read().replace("docs/images/blue_logo.svg", "https://urbanintelligence.co.nz/wp-content/uploads/2022/05/Artboard-1-copy-23.svg"),
     long_description_content_type='text/markdown',
     license="MIT",
     url="https://uintel.github.io/pyui/",
```

### Comparing `uintel-0.4.1/src/uintel/__init__.py` & `uintel-0.4.2/src/uintel/__init__.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/aws.py` & `uintel-0.4.2/src/uintel/aws.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/colours.py` & `uintel-0.4.2/src/uintel/colours.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/esri.py` & `uintel-0.4.2/src/uintel/esri.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/fonts/Myriad Pro (TrueType).ttf` & `uintel-0.4.2/src/uintel/fonts/Myriad Pro (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/fonts/Rubik (TrueType).ttf` & `uintel-0.4.2/src/uintel/fonts/Rubik (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/fonts/Rubik Italic (TrueType).ttf` & `uintel-0.4.2/src/uintel/fonts/Rubik Italic (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/geometry.py` & `uintel-0.4.2/src/uintel/geometry.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/install.py` & `uintel-0.4.2/src/uintel/install.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/ogc.py` & `uintel-0.4.2/src/uintel/ogc.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/query.py` & `uintel-0.4.2/src/uintel/query.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/server.py` & `uintel-0.4.2/src/uintel/server.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/slack.py` & `uintel-0.4.2/src/uintel/slack.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel/sql.py` & `uintel-0.4.2/src/uintel/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     # Make a connection to the database
     connection = psycopg2.connect(f"host={host} dbname={database_name} user={credentials['username']} password='{credentials['password']}' port={str(credentials['port'])}", **connect_args)
 
     return {"engine": engine, "con": connection}
     
 
-def _database_exists(database_name: str, engine: sqlalchemy.Engine, connect_args: dict):
+def _database_exists(database_name: str, engine, connect_args: dict):
     """Check if a postgis database exists.
 
     Checks if a databse already exists in postgreSQL. 
 
     Args:
         database_name: The name of the database.
         engine: A SQLAlchemy engine.
@@ -75,22 +75,22 @@
     url = sqlalchemy_utils.functions.database._set_url_database(engine.url, "postgres")
     engine = sqlalchemy.create_engine(url, connect_args=connect_args)
     existing_tables = pandas.read_sql(f"SELECT datname FROM pg_database WHERE datname = '{database_name}' AND datistemplate = 'false' AND datallowconn = 'true'", engine)
     engine.dispose()
     return len(existing_tables) > 0
         
 
-def _create_database(database_name: str, engine: sqlalchemy.Engine, connect_args: dict):
+def _create_database(database_name: str, engine, connect_args: dict):
     """Create a new postgis database.
 
     Create a new database in postgres and enable the postgis extension.
 
     Args:
         database_name: The name of the database to connect to, or create if it does not exist.
-        url: A SQLAlchemy engine URL.
+        engine: A SQLAlchemy engine.
         connect_args: A dictionary of connection arguments passed to sqlalchemy.create_engine function. These usually pertain to SSL connections.
 
     Returns:
         None.
     """
 
     # Connect to the postgres table (poentially using SSL) and create the new table
```

### Comparing `uintel-0.4.1/src/uintel/styles/ui.mplstyle` & `uintel-0.4.2/src/uintel/styles/ui.mplstyle`

 * *Files identical despite different names*

### Comparing `uintel-0.4.1/src/uintel.egg-info/PKG-INFO` & `uintel-0.4.2/src/uintel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.4.1
+Version: 0.4.2
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.4.1/src/uintel.egg-info/SOURCES.txt` & `uintel-0.4.2/src/uintel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

