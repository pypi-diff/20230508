# Comparing `tmp/dbt-doc-py-0.1.0.tar.gz` & `tmp/dbt-doc-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-doc-py-0.1.0.tar", last modified: Mon May  8 02:31:43 2023, max compression
+gzip compressed data, was "dbt-doc-py-0.1.1.tar", last modified: Mon May  8 13:55:53 2023, max compression
```

## Comparing `dbt-doc-py-0.1.0.tar` & `dbt-doc-py-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 02:31:43.260167 dbt-doc-py-0.1.0/
--rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     1212 2023-05-08 02:31:43.259162 dbt-doc-py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      764 2023-05-08 02:30:30.000000 dbt-doc-py-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 02:31:43.242013 dbt-doc-py-0.1.0/dbt-doc-py/
--rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.0/dbt-doc-py/__init__.py
--rw-rw-rw-   0        0        0    20824 2023-05-08 02:15:27.000000 dbt-doc-py-0.1.0/dbt-doc-py/dbt-doc-py.py
-drwxrwxrwx   0        0        0        0 2023-05-08 02:31:43.258171 dbt-doc-py-0.1.0/dbt_doc_py.egg-info/
--rw-rw-rw-   0        0        0     1212 2023-05-08 02:31:43.000000 dbt-doc-py-0.1.0/dbt_doc_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-08 02:31:43.000000 dbt-doc-py-0.1.0/dbt_doc_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 02:31:43.000000 dbt-doc-py-0.1.0/dbt_doc_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-08 02:31:43.000000 dbt-doc-py-0.1.0/dbt_doc_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 02:31:43.000000 dbt-doc-py-0.1.0/dbt_doc_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 02:31:43.261161 dbt-doc-py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-05-08 02:08:17.000000 dbt-doc-py-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:55:53.480294 dbt-doc-py-0.1.1/
+-rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     1212 2023-05-08 13:55:53.478301 dbt-doc-py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 13:55:53.462016 dbt-doc-py-0.1.1/dbt-doc-py/
+-rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.1/dbt-doc-py/__init__.py
+-rw-rw-rw-   0        0        0    20824 2023-05-08 02:15:27.000000 dbt-doc-py-0.1.1/dbt-doc-py/dbt-doc-py.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:55:53.470228 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/
+-rw-rw-rw-   0        0        0     1212 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:55:53.480294 dbt-doc-py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      724 2023-05-08 13:54:11.000000 dbt-doc-py-0.1.1/setup.py
```

### Comparing `dbt-doc-py-0.1.0/LICENCE` & `dbt-doc-py-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.0/PKG-INFO` & `dbt-doc-py-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -37,15 +37,15 @@
 ```
 dbt-doc-py
 ```
 
 You can execute it from other directories, this way:
 
 ```
-dbt-doc-py --working_directory /folder/DBTproject
+dbt-doc-py --working-directory /folder/DBTproject
 ```
 
 TO-DO: Finish README file:
 
 ## Documentation
```

### Comparing `dbt-doc-py-0.1.0/README.md` & `dbt-doc-py-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ```
 dbt-doc-py
 ```
 
 You can execute it from other directories, this way:
 
 ```
-dbt-doc-py --working_directory /folder/DBTproject
+dbt-doc-py --working-directory /folder/DBTproject
 ```
 
 TO-DO: Finish README file:
 
 ## Documentation
```

### Comparing `dbt-doc-py-0.1.0/dbt-doc-py/dbt-doc-py.py` & `dbt-doc-py-0.1.1/dbt-doc-py/dbt-doc-py.py`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.0/dbt_doc_py.egg-info/PKG-INFO` & `dbt-doc-py-0.1.1/dbt_doc_py.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -37,15 +37,15 @@
 ```
 dbt-doc-py
 ```
 
 You can execute it from other directories, this way:
 
 ```
-dbt-doc-py --working_directory /folder/DBTproject
+dbt-doc-py --working-directory /folder/DBTproject
 ```
 
 TO-DO: Finish README file:
 
 ## Documentation
```

