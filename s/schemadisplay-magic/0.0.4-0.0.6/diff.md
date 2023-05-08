# Comparing `tmp/schemadisplay-magic-0.0.4.tar.gz` & `tmp/schemadisplay-magic-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemadisplay-magic-0.0.4.tar", last modified: Mon Aug 16 17:17:13 2021, max compression
+gzip compressed data, was "schemadisplay-magic-0.0.6.tar", last modified: Mon May  8 13:59:25 2023, max compression
```

## Comparing `schemadisplay-magic-0.0.4.tar` & `schemadisplay-magic-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-16 17:17:13.873874 schemadisplay-magic-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)     1057 2021-08-16 17:17:08.000000 schemadisplay-magic-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       25 2021-08-16 17:17:08.000000 schemadisplay-magic-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3644 2021-08-16 17:17:13.873874 schemadisplay-magic-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3263 2021-08-16 17:17:08.000000 schemadisplay-magic-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      138 2021-08-16 17:17:08.000000 schemadisplay-magic-0.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-16 17:17:13.873874 schemadisplay-magic-0.0.4/schemadisplay_magic/
--rw-r--r--   0 runner    (1001) docker     (116)      181 2021-08-16 17:17:08.000000 schemadisplay-magic-0.0.4/schemadisplay_magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1911 2021-08-16 17:17:08.000000 schemadisplay-magic-0.0.4/schemadisplay_magic/schemadisplay.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-16 17:17:13.873874 schemadisplay-magic-0.0.4/schemadisplay_magic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3644 2021-08-16 17:17:13.000000 schemadisplay-magic-0.0.4/schemadisplay_magic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      375 2021-08-16 17:17:13.000000 schemadisplay-magic-0.0.4/schemadisplay_magic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-16 17:17:13.000000 schemadisplay-magic-0.0.4/schemadisplay_magic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       45 2021-08-16 17:17:13.000000 schemadisplay-magic-0.0.4/schemadisplay_magic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       45 2021-08-16 17:17:13.000000 schemadisplay-magic-0.0.4/schemadisplay_magic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-08-16 17:17:13.873874 schemadisplay-magic-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1209 2021-08-16 17:17:08.000000 schemadisplay-magic-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-16 17:17:13.873874 schemadisplay-magic-0.0.4/sqlalchemy_schemadisplay/
--rw-r--r--   0 runner    (1001) docker     (116)    10698 2021-08-16 17:17:08.000000 schemadisplay-magic-0.0.4/sqlalchemy_schemadisplay/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:59:25.424592 schemadisplay-magic-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-08 13:59:22.000000 schemadisplay-magic-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 13:59:22.000000 schemadisplay-magic-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-08 13:59:25.424592 schemadisplay-magic-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-08 13:59:22.000000 schemadisplay-magic-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 13:59:22.000000 schemadisplay-magic-0.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:59:25.424592 schemadisplay-magic-0.0.6/schemadisplay_magic/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-08 13:59:22.000000 schemadisplay-magic-0.0.6/schemadisplay_magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-08 13:59:22.000000 schemadisplay-magic-0.0.6/schemadisplay_magic/schemadisplay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:59:25.424592 schemadisplay-magic-0.0.6/schemadisplay_magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-08 13:59:25.000000 schemadisplay-magic-0.0.6/schemadisplay_magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-08 13:59:25.000000 schemadisplay-magic-0.0.6/schemadisplay_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:59:25.000000 schemadisplay-magic-0.0.6/schemadisplay_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 13:59:25.000000 schemadisplay-magic-0.0.6/schemadisplay_magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 13:59:25.000000 schemadisplay-magic-0.0.6/schemadisplay_magic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:59:25.424592 schemadisplay-magic-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-08 13:59:22.000000 schemadisplay-magic-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:59:25.424592 schemadisplay-magic-0.0.6/sqlalchemy_schemadisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-05-08 13:59:22.000000 schemadisplay-magic-0.0.6/sqlalchemy_schemadisplay/__init__.py
```

### Comparing `schemadisplay-magic-0.0.4/LICENSE` & `schemadisplay-magic-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `schemadisplay-magic-0.0.4/PKG-INFO` & `schemadisplay-magic-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: schemadisplay-magic
-Version: 0.0.4
+Version: 0.0.6
 Summary: Python package installation for ipython_magic_sqlalchemy_schemadisplay
 Home-page: https://github.com/innovationOUtside/ipython_magic_sqlalchemy_schemadisplay
 Author: Tony Hirst
 Author-email: tony.hirst@open.ac.uk
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipython_magic_sqlalchemy_schemadisplay
 Magic for [sqlalchemy_schemadisplay](https://github.com/fschulze/sqlalchemy_schemadisplay)
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/innovationOUtside/ipython_magic_sqlalchemy_schemadisplay/master?filepath=notebooks/SchemaDemo.ipynb)
@@ -91,9 +90,7 @@
 
 
 ## Using the Magic in a Teaching and Learning Context
 
 The magic was developed to support teaching and learning around the topic of *relational databases*. Students were working with a PostgreSQL database, creating, editing and deleting tables, and creating foreign key relationships between tables. The magic provided an easy way to visualise the current state of the tables available in the database, and any foreign key relationships between them.
 
 In this way, students could run database and table modifying statements in a notebook. A single line magic invocation could then be used to generate a visual representation of the current state of the database to check that their intended changes had worked correctly.
-
-
```

### Comparing `schemadisplay-magic-0.0.4/README.md` & `schemadisplay-magic-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `schemadisplay-magic-0.0.4/schemadisplay_magic/schemadisplay.py` & `schemadisplay-magic-0.0.6/schemadisplay_magic/schemadisplay.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         
         args = parser.parse_args(shlex.split(line))
         
         if args.connection_string is None: return
         
         include_tables = [i for i in reader([args.include_tables])][0] if args.include_tables is not None else None
         
-        graph = create_schema_graph(metadata=MetaData(args.connection_string),
+        graph = create_schema_graph(connection_string=args.connection_string,
             show_datatypes=args.show_datatypes, # The image would get nasty big if we'd show the datatypes
             show_indexes=False, # ditto for indexes
             rankdir='LR', # From left to right (instead of top to bottom),
             restrict_tables=include_tables,
             concentrate=False, # Don't try to join the relation lines together
             show_column_keys=args.show_column_keys)
```

### Comparing `schemadisplay-magic-0.0.4/schemadisplay_magic.egg-info/PKG-INFO` & `schemadisplay-magic-0.0.6/schemadisplay_magic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: schemadisplay-magic
-Version: 0.0.4
+Version: 0.0.6
 Summary: Python package installation for ipython_magic_sqlalchemy_schemadisplay
 Home-page: https://github.com/innovationOUtside/ipython_magic_sqlalchemy_schemadisplay
 Author: Tony Hirst
 Author-email: tony.hirst@open.ac.uk
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipython_magic_sqlalchemy_schemadisplay
 Magic for [sqlalchemy_schemadisplay](https://github.com/fschulze/sqlalchemy_schemadisplay)
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/innovationOUtside/ipython_magic_sqlalchemy_schemadisplay/master?filepath=notebooks/SchemaDemo.ipynb)
@@ -91,9 +90,7 @@
 
 
 ## Using the Magic in a Teaching and Learning Context
 
 The magic was developed to support teaching and learning around the topic of *relational databases*. Students were working with a PostgreSQL database, creating, editing and deleting tables, and creating foreign key relationships between tables. The magic provided an easy way to visualise the current state of the tables available in the database, and any foreign key relationships between them.
 
 In this way, students could run database and table modifying statements in a notebook. A single line magic invocation could then be used to generate a visual representation of the current state of the database to check that their intended changes had worked correctly.
-
-
```

### Comparing `schemadisplay-magic-0.0.4/setup.py` & `schemadisplay-magic-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 setup(author='Tony Hirst',
     author_email='tony.hirst@open.ac.uk',
     description='Python package installation for ipython_magic_sqlalchemy_schemadisplay',
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     license='MIT',
     url='https://github.com/innovationOUtside/ipython_magic_sqlalchemy_schemadisplay',
-    version='0.0.4',
+    version='0.0.6',
     name='schemadisplay-magic',
     packages=['schemadisplay_magic', 'sqlalchemy_schemadisplay'],
     install_requires=requirements
 )
```

