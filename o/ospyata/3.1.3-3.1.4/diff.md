# Comparing `tmp/ospyata-3.1.3.tar.gz` & `tmp/ospyata-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospyata-3.1.3.tar", last modified: Mon May  8 04:44:12 2023, max compression
+gzip compressed data, was "ospyata-3.1.4.tar", last modified: Mon May  8 06:15:46 2023, max compression
```

## Comparing `ospyata-3.1.3.tar` & `ospyata-3.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:44:12.349504 ospyata-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 04:43:57.000000 ospyata-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 04:44:12.349504 ospyata-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-08 04:43:57.000000 ospyata-3.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 04:44:12.349504 ospyata-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-08 04:43:57.000000 ospyata-3.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:44:12.349504 ospyata-3.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:44:12.349504 ospyata-3.1.3/src/ospyata/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-08 04:43:57.000000 ospyata-3.1.3/src/ospyata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 04:43:57.000000 ospyata-3.1.3/src/ospyata/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-08 04:43:57.000000 ospyata-3.1.3/src/ospyata/osmata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:44:12.349504 ospyata-3.1.3/src/ospyata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 04:44:12.000000 ospyata-3.1.3/src/ospyata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-08 04:44:12.000000 ospyata-3.1.3/src/ospyata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 04:44:12.000000 ospyata-3.1.3/src/ospyata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 04:44:12.000000 ospyata-3.1.3/src/ospyata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:46.689956 ospyata-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 06:15:33.000000 ospyata-3.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 06:15:46.689956 ospyata-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-08 06:15:33.000000 ospyata-3.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 06:15:46.689956 ospyata-3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-08 06:15:33.000000 ospyata-3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:46.685956 ospyata-3.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:46.689956 ospyata-3.1.4/src/ospyata/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-08 06:15:33.000000 ospyata-3.1.4/src/ospyata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 06:15:33.000000 ospyata-3.1.4/src/ospyata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-08 06:15:33.000000 ospyata-3.1.4/src/ospyata/osmata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:15:46.689956 ospyata-3.1.4/src/ospyata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 06:15:46.000000 ospyata-3.1.4/src/ospyata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-08 06:15:46.000000 ospyata-3.1.4/src/ospyata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:15:46.000000 ospyata-3.1.4/src/ospyata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 06:15:46.000000 ospyata-3.1.4/src/ospyata.egg-info/top_level.txt
```

### Comparing `ospyata-3.1.3/LICENSE` & `ospyata-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ospyata-3.1.3/PKG-INFO` & `ospyata-3.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ospyata
-Version: 3.1.3
+Version: 3.1.4
 Summary: Python library for the open source bookmark app Osmata.
 Home-page: https://github.com/aerocyber/ospyata
 Author: aerocyber
 License: MIT License
 Project-URL: Bug Reports, https://github.com/aerocyber/ospyata/issues
 Project-URL: Source, https://github.com/aerocyber/ospyata/
 Keywords: osmata,development,osmata-bindings,osmata-python-bindings,bookmarks,ospyata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.11, <4
+Requires-Python: >=3.09, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ospyata
 
 ![Python](https://ForTheBadge.com/images/badges/made-with-python.svg)
 ![Built with :heart:](https://ForTheBadge.com/images/badges/built-with-love.svg)
```

### Comparing `ospyata-3.1.3/README.md` & `ospyata-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ospyata-3.1.3/setup.py` & `ospyata-3.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="ospyata",
     license="MIT License",
-    version="3.1.3",
+    version="3.1.4",
     description="Python library for the open source bookmark app Osmata.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aerocyber/ospyata",
     author="aerocyber",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -32,14 +32,14 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="osmata, development, osmata-bindings, osmata-python-bindings, bookmarks, ospyata",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
-    python_requires=">=3.11, <4",
+    python_requires=">=3.09, <4",
     install_requires=[],  # Thanks to django's regex, validators is no longer required.
     project_urls={
         "Bug Reports": "https://github.com/aerocyber/ospyata/issues",
         "Source": "https://github.com/aerocyber/ospyata/",
     },
 )
```

### Comparing `ospyata-3.1.3/src/ospyata/osmata.py` & `ospyata-3.1.4/src/ospyata/osmata.py`

 * *Files identical despite different names*

### Comparing `ospyata-3.1.3/src/ospyata.egg-info/PKG-INFO` & `ospyata-3.1.4/src/ospyata.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ospyata
-Version: 3.1.3
+Version: 3.1.4
 Summary: Python library for the open source bookmark app Osmata.
 Home-page: https://github.com/aerocyber/ospyata
 Author: aerocyber
 License: MIT License
 Project-URL: Bug Reports, https://github.com/aerocyber/ospyata/issues
 Project-URL: Source, https://github.com/aerocyber/ospyata/
 Keywords: osmata,development,osmata-bindings,osmata-python-bindings,bookmarks,ospyata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.11, <4
+Requires-Python: >=3.09, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ospyata
 
 ![Python](https://ForTheBadge.com/images/badges/made-with-python.svg)
 ![Built with :heart:](https://ForTheBadge.com/images/badges/built-with-love.svg)
```

