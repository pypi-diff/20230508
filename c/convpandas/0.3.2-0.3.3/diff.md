# Comparing `tmp/convpandas-0.3.2.tar.gz` & `tmp/convpandas-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convpandas-0.3.2.tar", max compression
+gzip compressed data, was "convpandas-0.3.3.tar", max compression
```

## Comparing `convpandas-0.3.2.tar` & `convpandas-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1067 2021-01-18 12:28:00.704854 convpandas-0.3.2/LICENSE
--rw-r--r--   0        0        0     3251 2021-09-08 06:11:23.953856 convpandas-0.3.2/README.md
--rw-r--r--   0        0        0       64 2021-01-18 12:28:00.704854 convpandas-0.3.2/convpandas/__init__.py
--rw-r--r--   0        0        0     1299 2021-09-08 06:11:23.953856 convpandas-0.3.2/convpandas/__main__.py
--rw-r--r--   0        0        0       22 2021-10-01 15:47:13.514832 convpandas-0.3.2/convpandas/__version__.py
--rw-r--r--   0        0        0        0 2021-01-18 12:28:00.704854 convpandas-0.3.2/convpandas/command/__init__.py
--rw-r--r--   0        0        0     4918 2021-10-01 15:46:28.062832 convpandas-0.3.2/convpandas/command/csv2xlsx.py
--rw-r--r--   0        0        0     2644 2021-09-08 06:11:23.953856 convpandas-0.3.2/convpandas/command/xlsx2csv.py
--rw-r--r--   0        0        0       74 2021-09-08 06:11:23.953856 convpandas-0.3.2/convpandas/common/__init__.py
--rw-r--r--   0        0        0      237 2021-09-08 06:11:23.953856 convpandas-0.3.2/convpandas/common/cli.py
--rw-r--r--   0        0        0     1193 2021-10-01 15:47:19.094832 convpandas-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4217 2021-10-01 15:50:13.545668 convpandas-0.3.2/setup.py
--rw-r--r--   0        0        0     4280 2021-10-01 15:50:13.546051 convpandas-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-01-18 12:28:00.704854 convpandas-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3251 2021-09-08 06:11:23.953856 convpandas-0.3.3/README.md
+-rw-r--r--   0        0        0       64 2021-01-18 12:28:00.704854 convpandas-0.3.3/convpandas/__init__.py
+-rw-r--r--   0        0        0     1299 2021-09-08 06:11:23.953856 convpandas-0.3.3/convpandas/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-08 06:00:18.816410 convpandas-0.3.3/convpandas/__version__.py
+-rw-r--r--   0        0        0        0 2021-01-18 12:28:00.704854 convpandas-0.3.3/convpandas/command/__init__.py
+-rw-r--r--   0        0        0     4918 2022-01-05 13:44:35.624680 convpandas-0.3.3/convpandas/command/csv2xlsx.py
+-rw-r--r--   0        0        0     2644 2021-09-08 06:11:23.953856 convpandas-0.3.3/convpandas/command/xlsx2csv.py
+-rw-r--r--   0        0        0       74 2021-09-08 06:11:23.953856 convpandas-0.3.3/convpandas/common/__init__.py
+-rw-r--r--   0        0        0      237 2021-09-08 06:11:23.953856 convpandas-0.3.3/convpandas/common/cli.py
+-rw-r--r--   0        0        0     1223 2023-05-08 06:00:11.352388 convpandas-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 convpandas-0.3.3/PKG-INFO
```

### Comparing `convpandas-0.3.2/LICENSE` & `convpandas-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `convpandas-0.3.2/README.md` & `convpandas-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `convpandas-0.3.2/convpandas/__main__.py` & `convpandas-0.3.3/convpandas/__main__.py`

 * *Files identical despite different names*

### Comparing `convpandas-0.3.2/convpandas/command/csv2xlsx.py` & `convpandas-0.3.3/convpandas/command/csv2xlsx.py`

 * *Files identical despite different names*

### Comparing `convpandas-0.3.2/convpandas/command/xlsx2csv.py` & `convpandas-0.3.3/convpandas/command/xlsx2csv.py`

 * *Files identical despite different names*

### Comparing `convpandas-0.3.2/pyproject.toml` & `convpandas-0.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convpandas"
-version = "0.3.2"
+version = "0.3.3"
 description = "Convert file format with pandas"
 authors = ["yuji38kwmt"]
 maintainers = ["yuji38kwmt"]
 license = "MIT"
 keywords=["pandas", "csv","xlsx", "excel"]
 readme="README.md"
 repository="https://github.com/yuji38kwmt/convert-fileformat-with-pandas.git"
@@ -21,30 +21,32 @@
     "Topic :: Utilities",
     "Operating System :: OS Independent",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
-pandas = "^1.2"
+pandas = ">=1"
 openpyxl = "*"
 
 [tool.poetry.dev-dependencies]
 mypy = "*"
 flake8 = "*"
 autoflake = "*"
 isort = "*"
 black = {version = "^21.8b0", allow-prereleases = true}
 pytest = "*"
-
+pytest-cov = "*"
+codecov = "*"
 
 [tool.poetry.scripts]
 convpandas = "convpandas.__main__:cli"
 
 
 [tool.mypy]
 ignore_missing_imports = true
 
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
+
```

### Comparing `convpandas-0.3.2/PKG-INFO` & `convpandas-0.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: convpandas
-Version: 0.3.2
+Version: 0.3.3
 Summary: Convert file format with pandas
 Home-page: https://github.com/yuji38kwmt/convert-fileformat-with-pandas.git
 License: MIT
 Keywords: pandas,csv,xlsx,excel
 Author: yuji38kwmt
 Maintainer: yuji38kwmt
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: openpyxl
-Requires-Dist: pandas (>=1.2,<2.0)
+Requires-Dist: pandas (>=1)
 Project-URL: Repository, https://github.com/yuji38kwmt/convert-fileformat-with-pandas.git
 Description-Content-Type: text/markdown
 
 # convert-fileformat-with-pandas
 Convert file format with [pandas](https://pandas.pydata.org/).
 
 [![Build Status](https://travis-ci.org/yuji38kwmt/convpandas.svg?branch=master)](https://travis-ci.org/yuji38kwmt/convpandas)
```

