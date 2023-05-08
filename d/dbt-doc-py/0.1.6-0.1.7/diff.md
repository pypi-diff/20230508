# Comparing `tmp/dbt-doc-py-0.1.6.tar.gz` & `tmp/dbt-doc-py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-doc-py-0.1.6.tar", last modified: Mon May  8 14:23:13 2023, max compression
+gzip compressed data, was "dbt-doc-py-0.1.7.tar", last modified: Mon May  8 14:25:22 2023, max compression
```

## Comparing `dbt-doc-py-0.1.6.tar` & `dbt-doc-py-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 14:23:13.400663 dbt-doc-py-0.1.6/
--rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.6/LICENCE
--rw-rw-rw-   0        0        0     1212 2023-05-08 14:23:13.398671 dbt-doc-py-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 14:23:13.375504 dbt-doc-py-0.1.6/dbt_doc_py/
--rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.6/dbt_doc_py/__init__.py
--rw-rw-rw-   0        0        0    21012 2023-05-08 14:23:00.000000 dbt-doc-py-0.1.6/dbt_doc_py/dbt_doc_py.py
-drwxrwxrwx   0        0        0        0 2023-05-08 14:23:13.397655 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/
--rw-rw-rw-   0        0        0     1212 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 14:23:13.401665 dbt-doc-py-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-05-08 14:23:06.000000 dbt-doc-py-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:25:22.293283 dbt-doc-py-0.1.7/
+-rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.7/LICENCE
+-rw-rw-rw-   0        0        0     1212 2023-05-08 14:25:22.292276 dbt-doc-py-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 14:25:22.267218 dbt-doc-py-0.1.7/dbt_doc_py/
+-rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.7/dbt_doc_py/__init__.py
+-rw-rw-rw-   0        0        0    21179 2023-05-08 14:25:08.000000 dbt-doc-py-0.1.7/dbt_doc_py/dbt_doc_py.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:25:22.290269 dbt-doc-py-0.1.7/dbt_doc_py.egg-info/
+-rw-rw-rw-   0        0        0     1212 2023-05-08 14:25:22.000000 dbt-doc-py-0.1.7/dbt_doc_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-05-08 14:25:22.000000 dbt-doc-py-0.1.7/dbt_doc_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 14:25:22.000000 dbt-doc-py-0.1.7/dbt_doc_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-08 14:25:22.000000 dbt-doc-py-0.1.7/dbt_doc_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-05-08 14:25:22.000000 dbt-doc-py-0.1.7/dbt_doc_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 14:25:22.000000 dbt-doc-py-0.1.7/dbt_doc_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 14:25:22.293283 dbt-doc-py-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-05-08 14:25:17.000000 dbt-doc-py-0.1.7/setup.py
```

### Comparing `dbt-doc-py-0.1.6/LICENCE` & `dbt-doc-py-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.6/PKG-INFO` & `dbt-doc-py-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.6/README.md` & `dbt-doc-py-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.6/dbt_doc_py/dbt_doc_py.py` & `dbt-doc-py-0.1.7/dbt_doc_py/dbt_doc_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -602,8 +602,10 @@
 def run_async_main():
     if sys.platform == "win32" and sys.version_info >= (3, 8):        
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
     asyncio.run(main(sys.argv[1:]))
 
 if __name__ == "__main__":
-    run_async_main()
+    if sys.version_info >= (3, 8) and sys.platform.startswith("win"):
+        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+    asyncio.run(main(sys.argv[1:]))
```

### Comparing `dbt-doc-py-0.1.6/dbt_doc_py.egg-info/PKG-INFO` & `dbt-doc-py-0.1.7/dbt_doc_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.6/setup.py` & `dbt-doc-py-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt-doc-py",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=[
     "PyYAML", "dataclasses", "transformers", "asyncio", "argparse", "httpx",
     ],
     entry_points={
         'console_scripts': [
             'dbt-doc-py=dbt_doc_py.dbt_doc_py:main',
```

