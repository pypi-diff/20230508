# Comparing `tmp/finance_ml-0.0.2.tar.gz` & `tmp/finance_ml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\finance_ml-0.0.2.tar", last modified: Sat May  6 19:29:08 2023, max compression
+gzip compressed data, was "dist\finance_ml-0.0.3.tar", last modified: Mon May  8 01:13:20 2023, max compression
```

## Comparing `finance_ml-0.0.2.tar` & `finance_ml-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 19:29:08.000000 finance_ml-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-05-06 16:37:21.000000 finance_ml-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      603 2023-05-06 19:29:08.000000 finance_ml-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-06 16:43:18.000000 finance_ml-0.0.2/README.md
--rw-rw-rw-   0        0        0      201 2023-05-06 16:37:21.000000 finance_ml-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 19:29:08.000000 finance_ml-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1128 2023-05-06 19:28:54.000000 finance_ml-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml/
--rw-rw-rw-   0        0        0       39 2023-05-06 19:18:52.000000 finance_ml-0.0.2/src/finance_ml/__init__.py
--rw-rw-rw-   0        0        0       75 2023-05-06 18:23:10.000000 finance_ml-0.0.2/src/finance_ml/dataprep_ml.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/
--rw-rw-rw-   0        0        0      603 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/
+-rw-rw-rw-   0        0        0     3259 2023-05-07 18:26:13.000000 finance_ml-0.0.3/.gitignore
+-rw-rw-rw-   0        0        0        0 2023-05-06 16:37:21.000000 finance_ml-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      603 2023-05-08 01:13:20.000000 finance_ml-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-06 16:43:18.000000 finance_ml-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/dist/
+-rw-rw-rw-   0        0        0     2589 2023-05-08 01:12:45.000000 finance_ml-0.0.3/dist/finance_ml-0.0.2-py3-none-any.whl
+-rw-rw-rw-   0        0        0    10041 2023-05-08 01:12:44.000000 finance_ml-0.0.3/dist/finance_ml-0.0.2.tar.gz
+drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/finance_ml.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/notebooks/
+-rw-rw-rw-   0        0        0    16037 2023-05-08 01:10:05.000000 finance_ml-0.0.3/notebooks/module_testing.ipynb
+-rw-rw-rw-   0        0        0      201 2023-05-06 16:37:21.000000 finance_ml-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 01:13:20.000000 finance_ml-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2023-05-08 01:13:14.000000 finance_ml-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/src/finance_ml/
+-rw-rw-rw-   0        0        0       39 2023-05-06 19:18:52.000000 finance_ml-0.0.3/src/finance_ml/__init__.py
+-rw-rw-rw-   0        0        0     2383 2023-05-08 01:10:08.000000 finance_ml-0.0.3/src/finance_ml/dataprep_ml.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/src/finance_ml.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-05-08 01:13:19.000000 finance_ml-0.0.3/src/finance_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-05-08 01:13:20.000000 finance_ml-0.0.3/src/finance_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 01:13:19.000000 finance_ml-0.0.3/src/finance_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-08 01:13:19.000000 finance_ml-0.0.3/src/finance_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 01:13:19.000000 finance_ml-0.0.3/src/finance_ml.egg-info/top_level.txt
```

### Comparing `finance_ml-0.0.2/PKG-INFO` & `finance_ml-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finance_ml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Application of Machine Learning in Finances
 Author: Fabio Maia
 Author-email: <fabio.masaracchia@gmail.com>
 Keywords: python,finance,mlops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `finance_ml-0.0.2/setup.py` & `finance_ml-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Application of Machine Learning in Finances'
 LONG_DESCRIPTION = 'A package that allows you to build pipelines and evaluate trading strategies, resulting in instructions to operate in the market.'
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
@@ -18,15 +18,15 @@
     author="Fabio Maia",
     author_email="<fabio.masaracchia@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pandas', 'numpy', 'matplotlib'],
+    install_requires=['pandas', 'numpy', 'matplotlib','pyarrow'],
     keywords=['python', 'finance', 'mlops'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `finance_ml-0.0.2/src/finance_ml.egg-info/PKG-INFO` & `finance_ml-0.0.3/src/finance_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finance-ml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Application of Machine Learning in Finances
 Author: Fabio Maia
 Author-email: <fabio.masaracchia@gmail.com>
 Keywords: python,finance,mlops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

