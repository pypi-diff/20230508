# Comparing `tmp/dbt-doc-py-0.1.2.tar.gz` & `tmp/dbt-doc-py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-doc-py-0.1.2.tar", last modified: Mon May  8 13:59:11 2023, max compression
+gzip compressed data, was "dbt-doc-py-0.1.3.tar", last modified: Mon May  8 14:09:28 2023, max compression
```

## Comparing `dbt-doc-py-0.1.2.tar` & `dbt-doc-py-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 13:59:11.941377 dbt-doc-py-0.1.2/
--rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.2/LICENCE
--rw-rw-rw-   0        0        0     1212 2023-05-08 13:59:11.940389 dbt-doc-py-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 13:59:11.910768 dbt-doc-py-0.1.2/dbt-doc-py/
--rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.2/dbt-doc-py/__init__.py
--rw-rw-rw-   0        0        0    20824 2023-05-08 02:15:27.000000 dbt-doc-py-0.1.2/dbt-doc-py/dbt-doc-py.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:59:11.932439 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/
--rw-rw-rw-   0        0        0     1212 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 13:59:11.000000 dbt-doc-py-0.1.2/dbt_doc_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 13:59:11.941377 dbt-doc-py-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-05-08 13:58:29.000000 dbt-doc-py-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:09:28.938464 dbt-doc-py-0.1.3/
+-rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.3/LICENCE
+-rw-rw-rw-   0        0        0     1212 2023-05-08 14:09:28.937466 dbt-doc-py-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 14:09:28.912204 dbt-doc-py-0.1.3/dbt_doc_py/
+-rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.3/dbt_doc_py/__init__.py
+-rw-rw-rw-   0        0        0    20824 2023-05-08 02:15:27.000000 dbt-doc-py-0.1.3/dbt_doc_py/dbt_doc_py.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:09:28.936458 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/
+-rw-rw-rw-   0        0        0     1212 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 14:09:28.938464 dbt-doc-py-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-05-08 14:09:24.000000 dbt-doc-py-0.1.3/setup.py
```

### Comparing `dbt-doc-py-0.1.2/LICENCE` & `dbt-doc-py-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.2/PKG-INFO` & `dbt-doc-py-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.2/README.md` & `dbt-doc-py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.2/dbt-doc-py/dbt-doc-py.py` & `dbt-doc-py-0.1.3/dbt_doc_py/dbt_doc_py.py`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.2/dbt_doc_py.egg-info/PKG-INFO` & `dbt-doc-py-0.1.3/dbt_doc_py.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.2/setup.py` & `dbt-doc-py-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt-doc-py",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
     "PyYAML", "dataclasses", "transformers", "asyncio", "argparse", "httpx",
     ],
+    entry_points={
+        'console_scripts': [
+            'dbt-doc-py=dbt_doc_py.dbt_doc_py:main',
+        ],
+    },
     author="TextQLLabs",
     author_email="lenin@textql.com",
     description="Automatically generate docs for undocumented DBT models.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/TextQLLabs/dbt-doc-py.git",
     classifiers=[
```

