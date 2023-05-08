# Comparing `tmp/cpggen-1.0.3.tar.gz` & `tmp/cpggen-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.0.3.tar", max compression
+gzip compressed data, was "cpggen-1.0.4.tar", max compression
```

## Comparing `cpggen-1.0.3.tar` & `cpggen-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-03 23:53:48.127528 cpggen-1.0.3/LICENSE
--rw-r--r--   0        0        0     8804 2023-05-03 23:53:48.127528 cpggen-1.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/__init__.py
--rw-r--r--   0        0        0    15322 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/cli.py
--rw-r--r--   0        0        0    35417 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/logger.py
--rw-r--r--   0        0        0    11547 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/utils.py
--rw-r--r--   0        0        0     1269 2023-05-03 23:53:48.131528 cpggen-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    10132 1970-01-01 00:00:00.000000 cpggen-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 18:36:40.291380 cpggen-1.0.4/LICENSE
+-rw-r--r--   0        0        0     8804 2023-05-08 18:36:40.291380 cpggen-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 18:36:40.291380 cpggen-1.0.4/cpggen/__init__.py
+-rw-r--r--   0        0        0    15322 2023-05-08 18:36:40.291380 cpggen-1.0.4/cpggen/cli.py
+-rw-r--r--   0        0        0    35417 2023-05-08 18:36:40.291380 cpggen-1.0.4/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-05-08 18:36:40.291380 cpggen-1.0.4/cpggen/logger.py
+-rw-r--r--   0        0        0    11547 2023-05-08 18:36:40.295380 cpggen-1.0.4/cpggen/utils.py
+-rw-r--r--   0        0        0     1278 2023-05-08 18:36:40.295380 cpggen-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    10084 1970-01-01 00:00:00.000000 cpggen-1.0.4/PKG-INFO
```

### Comparing `cpggen-1.0.3/LICENSE` & `cpggen-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.3/README.md` & `cpggen-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.3/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.4/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.3/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.4/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

### Comparing `cpggen-1.0.3/cpggen/cli.py` & `cpggen-1.0.4/cpggen/cli.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.3/cpggen/executor.py` & `cpggen-1.0.4/cpggen/executor.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.3/cpggen/logger.py` & `cpggen-1.0.4/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.3/cpggen/utils.py` & `cpggen-1.0.4/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.3/pyproject.toml` & `cpggen-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.0.3"
+version = "1.0.4"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
@@ -23,23 +23,23 @@
 exclude = ["contrib", "tests"]
 
 [tool.poetry.scripts]
 cpggen = 'cpggen.cli:main'
 cpg = 'cpggen.cli:main'
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8.1,<3.12"
 rich = "^13.3.5"
 gitpython = "^3.1.31"
 quart = "^0.18.4"
 psutil = "^5.9.5"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-black = "^22.3.0"
-flake8 = "^4.0.1"
-pytest-cov = "^3.0.0"
-pyinstaller = "^5.0.1"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+black = "^23.3.0"
+flake8 = "^6.0.0"
+pytest-cov = "^4.0.0"
+pyinstaller = "^5.10.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cpggen-1.0.3/PKG-INFO` & `cpggen-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
@@ -59,23 +58,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.3/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.4/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.3/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.4/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

