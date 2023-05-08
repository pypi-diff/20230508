# Comparing `tmp/dbt-doc-py-0.1.5.tar.gz` & `tmp/dbt-doc-py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-doc-py-0.1.5.tar", last modified: Mon May  8 14:20:12 2023, max compression
+gzip compressed data, was "dbt-doc-py-0.1.6.tar", last modified: Mon May  8 14:23:13 2023, max compression
```

## Comparing `dbt-doc-py-0.1.5.tar` & `dbt-doc-py-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 14:20:12.234294 dbt-doc-py-0.1.5/
--rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.5/LICENCE
--rw-rw-rw-   0        0        0     1212 2023-05-08 14:20:12.233287 dbt-doc-py-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 14:20:12.208721 dbt-doc-py-0.1.5/dbt_doc_py/
--rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.5/dbt_doc_py/__init__.py
--rw-rw-rw-   0        0        0    21000 2023-05-08 14:19:56.000000 dbt-doc-py-0.1.5/dbt_doc_py/dbt_doc_py.py
-drwxrwxrwx   0        0        0        0 2023-05-08 14:20:12.231281 dbt-doc-py-0.1.5/dbt_doc_py.egg-info/
--rw-rw-rw-   0        0        0     1212 2023-05-08 14:20:12.000000 dbt-doc-py-0.1.5/dbt_doc_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-05-08 14:20:12.000000 dbt-doc-py-0.1.5/dbt_doc_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 14:20:12.000000 dbt-doc-py-0.1.5/dbt_doc_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-08 14:20:12.000000 dbt-doc-py-0.1.5/dbt_doc_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-05-08 14:20:12.000000 dbt-doc-py-0.1.5/dbt_doc_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 14:20:12.000000 dbt-doc-py-0.1.5/dbt_doc_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 14:20:12.234294 dbt-doc-py-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-05-08 14:20:05.000000 dbt-doc-py-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:23:13.400663 dbt-doc-py-0.1.6/
+-rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.6/LICENCE
+-rw-rw-rw-   0        0        0     1212 2023-05-08 14:23:13.398671 dbt-doc-py-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 14:23:13.375504 dbt-doc-py-0.1.6/dbt_doc_py/
+-rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.6/dbt_doc_py/__init__.py
+-rw-rw-rw-   0        0        0    21012 2023-05-08 14:23:00.000000 dbt-doc-py-0.1.6/dbt_doc_py/dbt_doc_py.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:23:13.397655 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/
+-rw-rw-rw-   0        0        0     1212 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 14:23:13.000000 dbt-doc-py-0.1.6/dbt_doc_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 14:23:13.401665 dbt-doc-py-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-05-08 14:23:06.000000 dbt-doc-py-0.1.6/setup.py
```

### Comparing `dbt-doc-py-0.1.5/LICENCE` & `dbt-doc-py-0.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.5/PKG-INFO` & `dbt-doc-py-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.5/README.md` & `dbt-doc-py-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.5/dbt_doc_py/dbt_doc_py.py` & `dbt-doc-py-0.1.6/dbt_doc_py/dbt_doc_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,11 +599,11 @@
     print("Success! Make sure to run `dbt docs generate`.")
     return 0
 
 def run_async_main():
     if sys.platform == "win32" and sys.version_info >= (3, 8):        
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
-    asyncio.run(main())
+    asyncio.run(main(sys.argv[1:]))
 
 if __name__ == "__main__":
     run_async_main()
```

### Comparing `dbt-doc-py-0.1.5/dbt_doc_py.egg-info/PKG-INFO` & `dbt-doc-py-0.1.6/dbt_doc_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.5/setup.py` & `dbt-doc-py-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt-doc-py",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
     "PyYAML", "dataclasses", "transformers", "asyncio", "argparse", "httpx",
     ],
     entry_points={
         'console_scripts': [
             'dbt-doc-py=dbt_doc_py.dbt_doc_py:main',
```

