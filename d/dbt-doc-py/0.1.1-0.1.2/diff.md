# Comparing `tmp/dbt-doc-py-0.1.1.tar.gz` & `tmp/dbt-doc-py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-doc-py-0.1.1.tar", last modified: Mon May  8 13:55:53 2023, max compression
+gzip compressed data, was "dbt-doc-py-0.1.2.tar", last modified: Mon May  8 13:59:11 2023, max compression
```

## Comparing `dbt-doc-py-0.1.1.tar` & `dbt-doc-py-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 13:55:53.480294 dbt-doc-py-0.1.1/
--rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     1212 2023-05-08 13:55:53.478301 dbt-doc-py-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 13:55:53.462016 dbt-doc-py-0.1.1/dbt-doc-py/
--rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.1/dbt-doc-py/__init__.py
--rw-rw-rw-   0        0        0    20824 2023-05-08 02:15:27.000000 dbt-doc-py-0.1.1/dbt-doc-py/dbt-doc-py.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:55:53.470228 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/
--rw-rw-rw-   0        0        0     1212 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 13:55:53.000000 dbt-doc-py-0.1.1/dbt_doc_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 13:55:53.480294 dbt-doc-py-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      724 2023-05-08 13:54:11.000000 dbt-doc-py-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:11.941377 dbt-doc-py-0.1.2/
+-rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0     1212 2023-05-08 13:59:11.940389 dbt-doc-py-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:11.910768 dbt-doc-py-0.1.2/dbt-doc-py/
+-rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.2/dbt-doc-py/__init__.py
+-rw-rw-rw-   0        0        0    20824 2023-05-08 02:15:27.000000 dbt-doc-py-0.1.2/dbt-doc-py/dbt-doc-py.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:11.932439 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/
+-rw-rw-rw-   0        0        0     1212 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:59:11.941377 dbt-doc-py-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-05-08 13:58:29.000000 dbt-doc-py-0.1.2/setup.py
```

### Comparing `dbt-doc-py-0.1.1/LICENCE` & `dbt-doc-py-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.1/PKG-INFO` & `dbt-doc-py-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.1/README.md` & `dbt-doc-py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.1/dbt-doc-py/dbt-doc-py.py` & `dbt-doc-py-0.1.2/dbt-doc-py/dbt-doc-py.py`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.1/dbt_doc_py.egg-info/PKG-INFO` & `dbt-doc-py-0.1.2/dbt_doc_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.1/setup.py` & `dbt-doc-py-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt-doc-py",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
-        "yaml", "dataclasses", "transformers", "asyncio", "argparse", "httpx",
+    "PyYAML", "dataclasses", "transformers", "asyncio", "argparse", "httpx",
     ],
     author="TextQLLabs",
     author_email="lenin@textql.com",
     description="Automatically generate docs for undocumented DBT models.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/TextQLLabs/dbt-doc-py.git",
```

