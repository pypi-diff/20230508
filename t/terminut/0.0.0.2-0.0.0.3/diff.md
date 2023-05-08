# Comparing `tmp/terminut-0.0.0.2.tar.gz` & `tmp/terminut-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminut-0.0.0.2.tar", last modified: Mon May  8 01:45:28 2023, max compression
+gzip compressed data, was "terminut-0.0.0.3.tar", last modified: Mon May  8 02:02:01 2023, max compression
```

## Comparing `terminut-0.0.0.2.tar` & `terminut-0.0.0.3.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 01:45:28.886674 terminut-0.0.0.2/
--rw-rw-rw-   0        0        0      984 2023-05-08 01:45:28.886674 terminut-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-08 01:45:28.886674 terminut-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1298 2023-05-08 01:45:05.000000 terminut-0.0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:45:28.879946 terminut-0.0.0.2/terminut/
--rw-rw-rw-   0        0        0      240 2023-05-08 01:43:34.000000 terminut-0.0.0.2/terminut/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-08 01:40:13.000000 terminut-0.0.0.2/terminut/console.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:45:28.886211 terminut-0.0.0.2/terminut.egg-info/
--rw-rw-rw-   0        0        0      984 2023-05-08 01:45:28.000000 terminut-0.0.0.2/terminut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-08 01:45:28.000000 terminut-0.0.0.2/terminut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 01:45:28.000000 terminut-0.0.0.2/terminut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 01:45:28.000000 terminut-0.0.0.2/terminut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 02:02:01.762266 terminut-0.0.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1994 2023-05-08 02:02:01.762266 terminut-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2023-05-08 01:53:38.000000 terminut-0.0.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 02:02:01.762266 terminut-0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1598 2023-05-08 02:01:50.000000 terminut-0.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 02:02:01.747306 terminut-0.0.0.3/terminut/
+-rw-rw-rw-   0        0        0      240 2023-05-08 01:43:34.000000 terminut-0.0.0.3/terminut/__init__.py
+-rw-rw-rw-   0        0        0     1600 2023-05-08 01:53:07.000000 terminut-0.0.0.3/terminut/console.py
+drwxrwxrwx   0        0        0        0 2023-05-08 02:02:01.761268 terminut-0.0.0.3/terminut.egg-info/
+-rw-rw-rw-   0        0        0     1994 2023-05-08 02:02:01.000000 terminut-0.0.0.3/terminut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-08 02:02:01.000000 terminut-0.0.0.3/terminut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 02:02:01.000000 terminut-0.0.0.3/terminut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-08 02:02:01.000000 terminut-0.0.0.3/terminut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 02:02:01.000000 terminut-0.0.0.3/terminut.egg-info/top_level.txt
```

### Comparing `terminut-0.0.0.2/PKG-INFO` & `terminut-0.0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Terminut // vast#1337
-Home-page: http://pypi.python.org/pypi/(terminut)
+Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
+Project-URL: Homepage, https://github.com/imvast/terminut
+Project-URL: Suggestions, https://github.com/imvast/terminut/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -18,7 +20,42 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Terminut.
+<img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
+<img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
+
+```less
+            > Custom Console Going To Be Used For My Projects
+                And Available To Anyone Else Who Wants To Use <
+```
+
+---
+
+### Installation
+```yaml
+! package not available yet for non-personal use !
+```
+
+### Usage
+```py
+from terminut.console import printf as print, inputf as input, init
+
+init(
+    gradient=True,
+    showTimestamp=True,
+    madeBy="vast#1337"
+)
+
+print("Cool Stuff")
+```
+
+---
+
+## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

### Comparing `terminut-0.0.0.2/setup.py` & `terminut-0.0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-projname = "terminut"
-
-setup(name=f"{projname}",
-      version="0.0.0.2",
+vers = "0.0.0.3"
+    
+setup(name="terminut",
+      version=vers,
       description="Terminut // vast#1337",
+      long_description_content_type="text/markdown",
+      long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
       author="vast#1337",
-      url=f"http://pypi.python.org/pypi/({projname})",
+      url=f"http://pypi.python.org/pypi/terminut",
       author_email="vastcord@proton.me",
       license="MIT",
       classifiers=[
           "Development Status :: 3 - Alpha",
           "Intended Audience :: Developers",
           "License :: OSI Approved :: MIT License",
           "Natural Language :: English",
@@ -25,14 +27,19 @@
           "Topic :: Scientific/Engineering",
           "Topic :: Scientific/Engineering :: Information Analysis",
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Scientific/Engineering :: Visualization",
           "Topic :: Software Development :: Libraries",
           "Topic :: Utilities",
       ],
-
+      project_urls={
+        'Homepage': 'https://github.com/imvast/terminut',
+        'Suggestions': 'https://github.com/imvast/terminut/issues',
+      },
+    
       python_requires="~=3.7",
 
-      #install_requires=[
-      #    "config4py>=0.1.0"
-      #]
+      install_requires=[
+          "colorama>=0.4.6",
+          "requests>=2.30.0"
+      ]
 )
```

### Comparing `terminut-0.0.0.2/terminut.egg-info/PKG-INFO` & `terminut-0.0.0.3/terminut.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Terminut // vast#1337
-Home-page: http://pypi.python.org/pypi/(terminut)
+Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
+Project-URL: Homepage, https://github.com/imvast/terminut
+Project-URL: Suggestions, https://github.com/imvast/terminut/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -18,7 +20,42 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Terminut.
+<img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
+<img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
+
+```less
+            > Custom Console Going To Be Used For My Projects
+                And Available To Anyone Else Who Wants To Use <
+```
+
+---
+
+### Installation
+```yaml
+! package not available yet for non-personal use !
+```
+
+### Usage
+```py
+from terminut.console import printf as print, inputf as input, init
+
+init(
+    gradient=True,
+    showTimestamp=True,
+    madeBy="vast#1337"
+)
+
+print("Cool Stuff")
+```
+
+---
+
+## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

