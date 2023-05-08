# Comparing `tmp/ospyata-3.1.1.tar.gz` & `tmp/ospyata-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospyata-3.1.1.tar", last modified: Sun Apr 23 13:28:16 2023, max compression
+gzip compressed data, was "ospyata-3.1.3.tar", last modified: Mon May  8 04:44:12 2023, max compression
```

## Comparing `ospyata-3.1.1.tar` & `ospyata-3.1.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:28:16.665884 ospyata-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-23 13:28:05.000000 ospyata-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-23 13:28:16.665884 ospyata-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-23 13:28:05.000000 ospyata-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 13:28:16.665884 ospyata-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-23 13:28:05.000000 ospyata-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:28:16.661884 ospyata-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:28:16.661884 ospyata-3.1.1/src/ospyata/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-23 13:28:05.000000 ospyata-3.1.1/src/ospyata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-23 13:28:05.000000 ospyata-3.1.1/src/ospyata/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-04-23 13:28:05.000000 ospyata-3.1.1/src/ospyata/osmata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:28:16.665884 ospyata-3.1.1/src/ospyata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:44:12.349504 ospyata-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 04:43:57.000000 ospyata-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 04:44:12.349504 ospyata-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-08 04:43:57.000000 ospyata-3.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 04:44:12.349504 ospyata-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-08 04:43:57.000000 ospyata-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:44:12.349504 ospyata-3.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:44:12.349504 ospyata-3.1.3/src/ospyata/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-08 04:43:57.000000 ospyata-3.1.3/src/ospyata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 04:43:57.000000 ospyata-3.1.3/src/ospyata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-08 04:43:57.000000 ospyata-3.1.3/src/ospyata/osmata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:44:12.349504 ospyata-3.1.3/src/ospyata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 04:44:12.000000 ospyata-3.1.3/src/ospyata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-08 04:44:12.000000 ospyata-3.1.3/src/ospyata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 04:44:12.000000 ospyata-3.1.3/src/ospyata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 04:44:12.000000 ospyata-3.1.3/src/ospyata.egg-info/top_level.txt
```

### Comparing `ospyata-3.1.1/LICENSE` & `ospyata-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ospyata-3.1.1/PKG-INFO` & `ospyata-3.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ospyata
-Version: 3.1.1
+Version: 3.1.3
 Summary: Python library for the open source bookmark app Osmata.
 Home-page: https://github.com/aerocyber/ospyata
 Author: aerocyber
 License: MIT License
 Project-URL: Bug Reports, https://github.com/aerocyber/ospyata/issues
 Project-URL: Source, https://github.com/aerocyber/ospyata/
 Keywords: osmata,development,osmata-bindings,osmata-python-bindings,bookmarks,ospyata
@@ -44,9 +44,11 @@
 > MIT License
 
 See [LICENSE file](https://github.com/aerocyber/ospyata/blob/main/LICENSE)
 
 ### Support
 
 Financially: [Buy me a coffee](https://www.buymeacoffee.com/aerocyber)
+
 Code/Documentation: [Open a PR](https://github.com/aerocyber/ospyata/pulls)
+
 Error reporting: [Open an issue](https://github.com/aerocyber/ospyata/issues)
```

### Comparing `ospyata-3.1.1/README.md` & `ospyata-3.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,11 @@
 > MIT License
 
 See [LICENSE file](https://github.com/aerocyber/ospyata/blob/main/LICENSE)
 
 ### Support
 
 Financially: [Buy me a coffee](https://www.buymeacoffee.com/aerocyber)
+
 Code/Documentation: [Open a PR](https://github.com/aerocyber/ospyata/pulls)
+
 Error reporting: [Open an issue](https://github.com/aerocyber/ospyata/issues)
```

### Comparing `ospyata-3.1.1/setup.py` & `ospyata-3.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
-long_description = (here / 'README.md').read_text(encoding='utf-8')
+long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
-    name='ospyata',
+    name="ospyata",
     license="MIT License",
-    version='3.1.1',
-    description='Python library for the open source bookmark app Osmata.',
+    version="3.1.3",
+    description="Python library for the open source bookmark app Osmata.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/aerocyber/ospyata',
-    author='aerocyber',
+    long_description_content_type="text/markdown",
+    url="https://github.com/aerocyber/ospyata",
+    author="aerocyber",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3 :: Only',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
     ],
-    keywords='osmata, development, osmata-bindings, osmata-python-bindings, bookmarks, ospyata',
-    package_dir={'': 'src'},
-    packages=find_packages(where='src'),
-    python_requires='>=3.11, <4',
-    install_requires=['validators'],
+    keywords="osmata, development, osmata-bindings, osmata-python-bindings, bookmarks, ospyata",
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
+    python_requires=">=3.11, <4",
+    install_requires=[],  # Thanks to django's regex, validators is no longer required.
     project_urls={
-        'Bug Reports': 'https://github.com/aerocyber/ospyata/issues',
-        'Source': 'https://github.com/aerocyber/ospyata/',
+        "Bug Reports": "https://github.com/aerocyber/ospyata/issues",
+        "Source": "https://github.com/aerocyber/ospyata/",
     },
 )
```

### Comparing `ospyata-3.1.1/src/ospyata/osmata.py` & `ospyata-3.1.3/src/ospyata/osmata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Copyright (c) 2021-present aerocyber
 #
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 import json
-import validators
+import re
 from typing import List
 import pathlib
 
 
 class OspyataException(Exception):
     pass
 
 
 class Osmata:
-
     def __init__(self):
         self.db = {}  # Initialize the datastructure.
 
     def push(self, name: str, url: str, categories: List[str] = []):
         """Push a record to the datastructure.
 
         Args:
@@ -38,18 +37,15 @@
             if self.check_existance(name=name):
                 _msg = name + " exists in db."
                 raise OspyataException(_msg)
             elif self.check_existance(url=url):
                 _msg = url + " exists in db."
                 raise OspyataException(_msg)
             else:
-                self.db[name] = {
-                    "URL": url,
-                    "Categories": categories
-                }
+                self.db[name] = {"URL": url, "Categories": categories}
 
     def pop(self, name: str):
         """Delete a record from db matching name.
 
         Args:
             name (str): The name (key) associated with the record to be deleted.
         """
@@ -63,45 +59,15 @@
 
     def validate_omio(self, dat: str):
         """Validate an omio file
 
         Args:
             dat (str): The omio string.
         """
-        # schema = {
-        #     "$schema": "https://json-schema.org/draft/2020-12/schema",
-        #     "$id": "https://example.com/product.schema.json",
-        #     "title": "Osmations",
-        #     "description": "A record of all bookmarks.",
-        #     "type": "object",
-        #     "properties": {
-        #         "Name": {
-        #             "description": "The unique identifier for a record.",
-        #             "type": "string"
-        #         },
-        #         "URL": {
-        #             "description": "URL associated with the Name.",
-        #             "type": "string"
-        #         },
-        #         "Categories": {
-        #             "description": "Tags for the Record",
-        #             "type": "array",
-        #             "items": {
-        #                 "type": "string"
-        #             }
-        #         }
-        #     },
-        #     "required": ["Name", "URL"]
-        # }
-        # try:
-        #     validate(instance=dat, schema=schema)
-        # except Exception as e:
-        #     return False
-        # else:
-        #     return True
+
         data = json.loads(dat)
         _keys = data.keys()
         _urls = []
         _is_cat_list = True
         for record in data:
             if isinstance(record, str):
                 if isinstance(data[record], dict):
@@ -120,22 +86,20 @@
                         return False
                 else:
                     return False
             else:
                 return False
         return True
 
-
-
     def dumpOmio(self):
         return json.dumps(self.db)
 
     def loadOmio(self, omio_path):
         if pathlib.Path(omio_path).exists():
-            f = open(omio_path, 'r')
+            f = open(omio_path, "r")
             data = f.read()
             f.close()
             if self.validate_omio(dat=data):
                 _json = json.loads(data)
                 return _json
             else:
                 raise OspyataException("Invalid omio file.")
@@ -148,15 +112,16 @@
         Args:
             name (str | False): Name associated. Defaults to False.
             url (str | False): Url associated. Defaults to False.
         """
         if name == False:
             if url == False:
                 raise OspyataException(
-                    "Neither name nor url is present for existance checking.")
+                    "Neither name nor url is present for existance checking."
+                )
             else:
                 _names = self.db.keys()
                 for _name in _names:
                     if url == self.db[_name]["URL"]:
                         return True
                     else:
                         return False
@@ -172,12 +137,39 @@
 
     def validate_url(self, url):
         """Check if url is valid.
 
         Args:
             url (str): Url
         """
-        try:
-            if validators.url(url.strip()):
-                return True
-        except Exception as e:
-            raise e
+        # Regex source: https://github.com/django/django/blob/main/django/core/validators.py#L69
+        regex = re.compile(
+            r"^(?:[a-z0-9.+-]*)://"  # scheme is validated separately
+            r"(?:[^\s:@/]+(?::[^\s:@/]*)?@)?"  # user:pass authentication
+            r"(?:" + r"(?:0|25[0-5]|2[0-4][0-9]|1[0-9]?[0-9]?|[1-9][0-9]?)"
+            r"(?:\.(?:0|25[0-5]|2[0-4][0-9]|1[0-9]?[0-9]?|[1-9][0-9]?)){3}"
+            + "|"
+            + r"\[[0-9a-f:.]+\]"
+            + "|"
+            + "("
+            + r"[a-z"
+            + "\u00a1-\uffff"
+            + r"0-9](?:[a-z"
+            + "\u00a1-\uffff"
+            + r"0-9-]{0,61}[a-z"
+            + "\u00a1-\uffff"
+            + r"0-9])?"
+            + r"(?:\.(?!-)[a-z"
+            + "\u00a1-\uffff"
+            + r"0-9-]{1,63}(?<!-))*"
+            + r"\."  # dot
+            r"(?!-)"  # can't start with a dash
+            r"(?:[a-z" + "\u00a1-\uffff" + "-]{2,63}"  # domain label
+            r"|xn--[a-z0-9]{1,59})"  # or punycode label
+            r"(?<!-)"  # can't end with a dash
+            r"\.?" + "|localhost)" + ")"  # may have a trailing dot
+            r"(?::[0-9]{1,5})?"  # port
+            r"(?:[/?#][^\s]*)?"  # resource path
+            r"\Z",
+            re.IGNORECASE,
+        )
+        return re.match(regex, url) is not None
```

### Comparing `ospyata-3.1.1/src/ospyata.egg-info/PKG-INFO` & `ospyata-3.1.3/src/ospyata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ospyata
-Version: 3.1.1
+Version: 3.1.3
 Summary: Python library for the open source bookmark app Osmata.
 Home-page: https://github.com/aerocyber/ospyata
 Author: aerocyber
 License: MIT License
 Project-URL: Bug Reports, https://github.com/aerocyber/ospyata/issues
 Project-URL: Source, https://github.com/aerocyber/ospyata/
 Keywords: osmata,development,osmata-bindings,osmata-python-bindings,bookmarks,ospyata
@@ -44,9 +44,11 @@
 > MIT License
 
 See [LICENSE file](https://github.com/aerocyber/ospyata/blob/main/LICENSE)
 
 ### Support
 
 Financially: [Buy me a coffee](https://www.buymeacoffee.com/aerocyber)
+
 Code/Documentation: [Open a PR](https://github.com/aerocyber/ospyata/pulls)
+
 Error reporting: [Open an issue](https://github.com/aerocyber/ospyata/issues)
```

