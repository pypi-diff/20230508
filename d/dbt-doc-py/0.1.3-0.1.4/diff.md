# Comparing `tmp/dbt-doc-py-0.1.3.tar.gz` & `tmp/dbt-doc-py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-doc-py-0.1.3.tar", last modified: Mon May  8 14:09:28 2023, max compression
+gzip compressed data, was "dbt-doc-py-0.1.4.tar", last modified: Mon May  8 14:17:12 2023, max compression
```

## Comparing `dbt-doc-py-0.1.3.tar` & `dbt-doc-py-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 14:09:28.938464 dbt-doc-py-0.1.3/
--rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.3/LICENCE
--rw-rw-rw-   0        0        0     1212 2023-05-08 14:09:28.937466 dbt-doc-py-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 14:09:28.912204 dbt-doc-py-0.1.3/dbt_doc_py/
--rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.3/dbt_doc_py/__init__.py
--rw-rw-rw-   0        0        0    20824 2023-05-08 02:15:27.000000 dbt-doc-py-0.1.3/dbt_doc_py/dbt_doc_py.py
-drwxrwxrwx   0        0        0        0 2023-05-08 14:09:28.936458 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/
--rw-rw-rw-   0        0        0     1212 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 14:09:28.000000 dbt-doc-py-0.1.3/dbt_doc_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 14:09:28.938464 dbt-doc-py-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-05-08 14:09:24.000000 dbt-doc-py-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:17:12.478902 dbt-doc-py-0.1.4/
+-rw-rw-rw-   0        0        0     1082 2023-05-08 02:05:10.000000 dbt-doc-py-0.1.4/LICENCE
+-rw-rw-rw-   0        0        0     1212 2023-05-08 14:17:12.476939 dbt-doc-py-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2023-05-08 02:38:19.000000 dbt-doc-py-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 14:17:12.452111 dbt-doc-py-0.1.4/dbt_doc_py/
+-rw-rw-rw-   0        0        0        0 2023-05-08 01:48:19.000000 dbt-doc-py-0.1.4/dbt_doc_py/__init__.py
+-rw-rw-rw-   0        0        0    20808 2023-05-08 14:16:40.000000 dbt-doc-py-0.1.4/dbt_doc_py/dbt_doc_py.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:17:12.474900 dbt-doc-py-0.1.4/dbt_doc_py.egg-info/
+-rw-rw-rw-   0        0        0     1212 2023-05-08 14:17:12.000000 dbt-doc-py-0.1.4/dbt_doc_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-05-08 14:17:12.000000 dbt-doc-py-0.1.4/dbt_doc_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 14:17:12.000000 dbt-doc-py-0.1.4/dbt_doc_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-08 14:17:12.000000 dbt-doc-py-0.1.4/dbt_doc_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-05-08 14:17:12.000000 dbt-doc-py-0.1.4/dbt_doc_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 14:17:12.000000 dbt-doc-py-0.1.4/dbt_doc_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 14:17:12.478902 dbt-doc-py-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-05-08 14:16:55.000000 dbt-doc-py-0.1.4/setup.py
```

### Comparing `dbt-doc-py-0.1.3/LICENCE` & `dbt-doc-py-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.3/PKG-INFO` & `dbt-doc-py-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.3/README.md` & `dbt-doc-py-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt-doc-py-0.1.3/dbt_doc_py/dbt_doc_py.py` & `dbt-doc-py-0.1.4/dbt_doc_py/dbt_doc_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -527,17 +527,17 @@
     def __init__(self, email: str):
         self.email = email
 
 class Key:
     def __init__(self, key: str):
         self.key = key
 
-async def main(argv) -> int:
-    try:        
-        args_env = parse_args(argv)
+async def main() -> int:
+    try:
+        args_env = parse_args(sys.argv[1:])
 
         manifest_path = os.path.join(args_env.working_directory, "target", "manifest.json")
         try:
             with open(manifest_path, "r") as f:
                 contents = f.read()
         except Exception as e:
             print("Reading target/manifest.json failed. Please re-run from a dbt project with generated docs")
@@ -596,8 +596,8 @@
     for patch_path, group in itertools.groupby(sorted(summarized_nodes, key=lambda x: x.patch_path), key=lambda x: x.patch_path):
         insert_docs(env, patch_path, list(group))
 
     print("Success! Make sure to run `dbt docs generate`.")
     return 0
 
 if __name__ == "__main__":
-    sys.exit(asyncio.run(main(sys.argv[1:])))
+    sys.exit(asyncio.run(main()))
```

### Comparing `dbt-doc-py-0.1.3/dbt_doc_py.egg-info/PKG-INFO` & `dbt-doc-py-0.1.4/dbt_doc_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-doc-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automatically generate docs for undocumented DBT models.
 Home-page: https://github.com/TextQLLabs/dbt-doc-py.git
 Author: TextQLLabs
 Author-email: lenin@textql.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dbt-doc-py-0.1.3/setup.py` & `dbt-doc-py-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt-doc-py",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
     "PyYAML", "dataclasses", "transformers", "asyncio", "argparse", "httpx",
     ],
     entry_points={
         'console_scripts': [
             'dbt-doc-py=dbt_doc_py.dbt_doc_py:main',
```

