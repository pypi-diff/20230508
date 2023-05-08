# Comparing `tmp/gbd_tools-4.5.3.tar.gz` & `tmp/gbd_tools-4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.5.3.tar", last modified: Fri May  5 18:49:57 2023, max compression
+gzip compressed data, was "gbd_tools-4.5.4.tar", last modified: Mon May  8 06:55:27 2023, max compression
```

## Comparing `gbd_tools-4.5.3.tar` & `gbd_tools-4.5.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:49:57.078440 gbd_tools-4.5.3/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.3/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-05 18:49:57.078440 gbd_tools-4.5.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.3/README.md
--rwxrwxr-x   0 root         (0) root         (0)    12047 2023-05-05 08:47:08.000000 gbd_tools-4.5.3/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:49:57.074440 gbd_tools-4.5.3/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.3/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9330 2023-05-05 18:47:02.000000 gbd_tools-4.5.3/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.3/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10527 2023-05-01 08:28:39.000000 gbd_tools-4.5.3/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     5065 2023-04-28 06:51:42.000000 gbd_tools-4.5.3/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5790 2023-04-25 15:20:20.000000 gbd_tools-4.5.3/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.3/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.3/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-05 18:48:49.000000 gbd_tools-4.5.3/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:49:57.074440 gbd_tools-4.5.3/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.3/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.5.3/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.3/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.3/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.3/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:49:57.074440 gbd_tools-4.5.3/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.3/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:49:57.074440 gbd_tools-4.5.3/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:49:57.078440 gbd_tools-4.5.3/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.3/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.3/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.3/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.3/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.3/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:49:57.078440 gbd_tools-4.5.3/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.3/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:49:57.078440 gbd_tools-4.5.3/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-05 18:49:56.000000 gbd_tools-4.5.3/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-05-05 18:49:56.000000 gbd_tools-4.5.3/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 18:49:56.000000 gbd_tools-4.5.3/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-05 18:49:56.000000 gbd_tools-4.5.3/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-05 18:49:56.000000 gbd_tools-4.5.3/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-05 18:49:56.000000 gbd_tools-4.5.3/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.5.3/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 18:49:57.078440 gbd_tools-4.5.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-05-05 18:47:41.000000 gbd_tools-4.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.4/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.4/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    12120 2023-05-08 06:53:24.000000 gbd_tools-4.5.4/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.188179 gbd_tools-4.5.4/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.4/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9444 2023-05-08 06:50:54.000000 gbd_tools-4.5.4/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    10587 2023-05-08 06:51:06.000000 gbd_tools-4.5.4/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     5065 2023-04-28 06:51:42.000000 gbd_tools-4.5.4/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5790 2023-04-25 15:20:20.000000 gbd_tools-4.5.4/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.4/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-05 18:48:49.000000 gbd_tools-4.5.4/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.192179 gbd_tools-4.5.4/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.4/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_init/cnf_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_init/cnf_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.192179 gbd_tools-4.5.4/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.4/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.192179 gbd_tools-4.5.4/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.4/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.4/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.4/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.4/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.4/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.4/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.5.4/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-05-08 06:54:19.000000 gbd_tools-4.5.4/setup.py
```

### Comparing `gbd_tools-4.5.3/LICENSE` & `gbd_tools-4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/PKG-INFO` & `gbd_tools-4.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.5.3
+Version: 4.5.4
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.3/README.md` & `gbd_tools-4.5.4/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd.py` & `gbd_tools-4.5.4/gbd.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     elif args.force or util.confirm("Delete feature '{}' and all associated attributes?".format(args.name)):
         api.delete_feature(args.name)
 
 def cli_rename(api: GBD, args):
     api.rename_feature(args.old_name, args.new_name)
 
 def cli_copy(api: GBD, args):
-    api.copy_feature(args.old_name, args.new_name, args.target_db)
+    api.copy_feature(args.old_name, args.new_name, args.target_db, args.query, args.hashes)
 
 
 def cli_get(api: GBD, args):
     df = api.query(args.query, args.hashes, args.resolve, args.collapse, args.group_by, args.join_type, args.subselect)
     for index, row in df.iterrows():
         print(" ".join([ item or "[None]" for item in row.to_list() ]))
 
@@ -189,14 +189,15 @@
 
     parser_rename = subparsers.add_parser('rename', help='Rename feature')
     parser_rename.add_argument('old_name', type=column_type, help='Old name of feature')
     parser_rename.add_argument('new_name', type=column_type, help='New name of feature')
     parser_rename.set_defaults(func=cli_rename)
 
     parser_copy = subparsers.add_parser('copy', help='Copy feature')
+    add_query_and_hashes_arguments(parser_copy)
     parser_copy.add_argument('--target_db', help='Target database (default: first in list)', default=None)
     parser_copy.add_argument('old_name', type=column_type, help='Old name of feature')
     parser_copy.add_argument('new_name', type=column_type, help='New name of feature')
     parser_copy.set_defaults(func=cli_copy)
 
     # GET META INFO
     parser_info = subparsers.add_parser('info', help='Print info about available features')
```

### Comparing `gbd_tools-4.5.3/gbd_core/api.py` & `gbd_tools-4.5.4/gbd_core/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
             raise GBDException("Feature '{}' does not exist".format(old_name))
         elif self.feature_exists(new_name, target_db):
             raise GBDException("Feature '{}' does already exist".format(new_name))
         else:
             self.database.rename_feature(old_name, new_name, target_db)
 
 
-    def copy_feature(self, old_name, new_name, target_db=None):
+    def copy_feature(self, old_name, new_name, target_db=None, gbd_query=None, hashes=[]):
         """ Copies feature with given name
 
             Args:
                 old_name (str): old feature name
                 new_name (str): new feature name
                 target_db (str): name of database to copy feature to
                     if None, default database (fist in list) is used
@@ -254,9 +254,11 @@
         """
         if not self.feature_exists(old_name):
             raise GBDException("Feature '{}' does not exist".format(old_name))
         
         if not self.feature_exists(new_name, target_db):
             self.create_feature(new_name, target_db=target_db)
 
-        self.database.copy_feature(old_name, new_name, target_db)
+        hashes = list(self.query(gbd_query=gbd_query, hashes=hashes)["hash"])
+
+        self.database.copy_feature(old_name, new_name, target_db, hashes)
```

### Comparing `gbd_tools-4.5.3/gbd_core/contexts.py` & `gbd_tools-4.5.4/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_core/database.py` & `gbd_tools-4.5.4/gbd_core/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,13 +252,13 @@
             remaining = [ r[0] for r in self.query("SELECT DISTINCT(hash) FROM {d}.{tab} WHERE hash in ('{h}')".format(d=db, tab=fname, h="', '".join(hashlist))) ]
             setnone = [ h for h in hashlist if not h in remaining ]
             self.execute("UPDATE {d}.features SET {col} = 'None' WHERE hash IN ('{h}')".format(d=db, col=fname, h="', '".join(setnone)))
         else:
             self.execute("UPDATE {d}.features SET {col} = '{default}' WHERE {w}".format(d=db, col=fname, default=finfo.default, w=where))
 
 
-    def copy_feature(self, old_name, new_name, target_db):
+    def copy_feature(self, old_name, new_name, target_db, hashlist=[]):
         old_finfo = self.finfo(old_name)
-        data = self.query("SELECT hash, {col} FROM {d}.{tab}".format(d=old_finfo.database, col=old_finfo.column, tab=old_finfo.table))
+        data = self.query("SELECT hash, {col} FROM {d}.{tab} WHERE hash IN ('{h}')".format(d=old_finfo.database, col=old_finfo.column, tab=old_finfo.table, h="', '".join(hashlist)))
         for (hash, value) in data:
             self.set_values(new_name, value, [hash], target_db)
```

### Comparing `gbd_tools-4.5.3/gbd_core/grammar.py` & `gbd_tools-4.5.4/gbd_core/grammar.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_core/query.py` & `gbd_tools-4.5.4/gbd_core/query.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_core/schema.py` & `gbd_tools-4.5.4/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_core/util.py` & `gbd_tools-4.5.4/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_core/util_argparse.py` & `gbd_tools-4.5.4/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_init/cnf_extractors.py` & `gbd_tools-4.5.4/gbd_init/cnf_extractors.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_init/cnf_transformers.py` & `gbd_tools-4.5.4/gbd_init/cnf_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_init/gbdhash.py` & `gbd_tools-4.5.4/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_init/initializer.py` & `gbd_tools-4.5.4/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.5.4/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.5.4/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.5.4/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_server/static/main.css` & `gbd_tools-4.5.4/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_server/static/w3.js` & `gbd_tools-4.5.4/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_server/templates/index.html` & `gbd_tools-4.5.4/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.5.4/gbd_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.5.3
+Version: 4.5.4
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.3/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.5.4/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/server.py` & `gbd_tools-4.5.4/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.3/setup.py` & `gbd_tools-4.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.5.3',
+  version='4.5.4',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

