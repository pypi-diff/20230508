# Comparing `tmp/async_retriever-0.3.7.tar.gz` & `tmp/async_retriever-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_retriever-0.3.7.tar", last modified: Fri Dec  9 22:46:51 2022, max compression
+gzip compressed data, was "async_retriever-0.3.8.tar", last modified: Sun Dec 11 02:48:42 2022, max compression
```

## Comparing `async_retriever-0.3.7.tar` & `async_retriever-0.3.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:50.994895 async_retriever-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      194 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:50.990895 async_retriever-0.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:50.990895 async_retriever-0.3.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:50.990895 async_retriever-0.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-09 22:46:34.000000 async_retriever-0.3.7/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-09 22:46:34.000000 async_retriever-0.3.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2022-12-09 22:46:34.000000 async_retriever-0.3.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2022-12-09 22:46:34.000000 async_retriever-0.3.7/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2022-12-09 22:46:34.000000 async_retriever-0.3.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2022-12-09 22:46:34.000000 async_retriever-0.3.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-09 22:46:34.000000 async_retriever-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-09 22:46:34.000000 async_retriever-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15844 2022-12-09 22:46:50.994895 async_retriever-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2022-12-09 22:46:34.000000 async_retriever-0.3.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:50.994895 async_retriever-0.3.7/async_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-09 22:46:34.000000 async_retriever-0.3.7/async_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17312 2022-12-09 22:46:34.000000 async_retriever-0.3.7/async_retriever/async_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2022-12-09 22:46:34.000000 async_retriever-0.3.7/async_retriever/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2022-12-09 22:46:34.000000 async_retriever-0.3.7/async_retriever/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:34.000000 async_retriever-0.3.7/async_retriever/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2022-12-09 22:46:34.000000 async_retriever-0.3.7/async_retriever/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:50.994895 async_retriever-0.3.7/async_retriever.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15844 2022-12-09 22:46:50.000000 async_retriever-0.3.7/async_retriever.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-09 22:46:50.000000 async_retriever-0.3.7/async_retriever.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 22:46:50.000000 async_retriever-0.3.7/async_retriever.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 22:46:50.000000 async_retriever-0.3.7/async_retriever.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2022-12-09 22:46:50.000000 async_retriever-0.3.7/async_retriever.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-09 22:46:50.000000 async_retriever-0.3.7/async_retriever.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:50.986895 async_retriever-0.3.7/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:50.994895 async_retriever-0.3.7/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2022-12-09 22:46:34.000000 async_retriever-0.3.7/ci/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-09 22:46:34.000000 async_retriever-0.3.7/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-09 22:46:34.000000 async_retriever-0.3.7/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2022-12-09 22:46:34.000000 async_retriever-0.3.7/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2022-12-09 22:46:34.000000 async_retriever-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2022-12-09 22:46:50.994895 async_retriever-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-09 22:46:34.000000 async_retriever-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:46:50.994895 async_retriever-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2022-12-09 22:46:34.000000 async_retriever-0.3.7/tests/test_async_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2022-12-09 22:46:34.000000 async_retriever-0.3.7/tests/test_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:42.353026 async_retriever-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:42.353026 async_retriever-0.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:42.353026 async_retriever-0.3.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:42.353026 async_retriever-0.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-11 02:48:26.000000 async_retriever-0.3.8/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-11 02:48:26.000000 async_retriever-0.3.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2022-12-11 02:48:26.000000 async_retriever-0.3.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2022-12-11 02:48:26.000000 async_retriever-0.3.8/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2022-12-11 02:48:26.000000 async_retriever-0.3.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2022-12-11 02:48:26.000000 async_retriever-0.3.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-11 02:48:26.000000 async_retriever-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-11 02:48:26.000000 async_retriever-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15844 2022-12-11 02:48:42.353026 async_retriever-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2022-12-11 02:48:26.000000 async_retriever-0.3.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:42.353026 async_retriever-0.3.8/async_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-11 02:48:26.000000 async_retriever-0.3.8/async_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17312 2022-12-11 02:48:26.000000 async_retriever-0.3.8/async_retriever/async_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2022-12-11 02:48:26.000000 async_retriever-0.3.8/async_retriever/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2022-12-11 02:48:26.000000 async_retriever-0.3.8/async_retriever/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:26.000000 async_retriever-0.3.8/async_retriever/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2022-12-11 02:48:26.000000 async_retriever-0.3.8/async_retriever/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:42.353026 async_retriever-0.3.8/async_retriever.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15844 2022-12-11 02:48:42.000000 async_retriever-0.3.8/async_retriever.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-11 02:48:42.000000 async_retriever-0.3.8/async_retriever.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 02:48:42.000000 async_retriever-0.3.8/async_retriever.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 02:48:41.000000 async_retriever-0.3.8/async_retriever.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-11 02:48:42.000000 async_retriever-0.3.8/async_retriever.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-11 02:48:42.000000 async_retriever-0.3.8/async_retriever.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:42.349025 async_retriever-0.3.8/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:42.353026 async_retriever-0.3.8/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2022-12-11 02:48:26.000000 async_retriever-0.3.8/ci/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-11 02:48:26.000000 async_retriever-0.3.8/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-11 02:48:26.000000 async_retriever-0.3.8/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2022-12-11 02:48:26.000000 async_retriever-0.3.8/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2022-12-11 02:48:26.000000 async_retriever-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2022-12-11 02:48:42.357025 async_retriever-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-11 02:48:26.000000 async_retriever-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:48:42.353026 async_retriever-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2022-12-11 02:48:26.000000 async_retriever-0.3.8/tests/test_async_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2022-12-11 02:48:26.000000 async_retriever-0.3.8/tests/test_exceptions.py
```

### Comparing `async_retriever-0.3.7/.github/ISSUE_TEMPLATE/bugreport.yml` & `async_retriever-0.3.8/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/.github/ISSUE_TEMPLATE/newfeature.yml` & `async_retriever-0.3.8/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/.github/workflows/codeql-analysis.yml` & `async_retriever-0.3.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/.github/workflows/release.yml` & `async_retriever-0.3.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/.github/workflows/test.yml` & `async_retriever-0.3.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/.gitignore` & `async_retriever-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/.pre-commit-config.yaml` & `async_retriever-0.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/CITATION.cff` & `async_retriever-0.3.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/CODE_OF_CONDUCT.rst` & `async_retriever-0.3.8/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/CONTRIBUTING.rst` & `async_retriever-0.3.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/HISTORY.rst` & `async_retriever-0.3.8/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/LICENSE` & `async_retriever-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/PKG-INFO` & `async_retriever-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_retriever
-Version: 0.3.7
+Version: 0.3.8
 Summary: High-level API for asynchronous requests with persistent caching.
 Home-page: https://github.com/hyriver/async-retriever
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT
 Project-URL: Homepage, https://docs.hyriver.io/readme/async-retriever.html
 Project-URL: Issues, https://github.com/hyriver/async-retriever/issues
```

### Comparing `async_retriever-0.3.7/README.rst` & `async_retriever-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/async_retriever/__init__.py` & `async_retriever-0.3.8/async_retriever/__init__.py`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/async_retriever/async_retriever.py` & `async_retriever-0.3.8/async_retriever/async_retriever.py`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/async_retriever/exceptions.py` & `async_retriever-0.3.8/async_retriever/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/async_retriever/print_versions.py` & `async_retriever-0.3.8/async_retriever/print_versions.py`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/async_retriever/utils.py` & `async_retriever-0.3.8/async_retriever/utils.py`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/async_retriever.egg-info/PKG-INFO` & `async_retriever-0.3.8/async_retriever.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-retriever
-Version: 0.3.7
+Version: 0.3.8
 Summary: High-level API for asynchronous requests with persistent caching.
 Home-page: https://github.com/hyriver/async-retriever
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT
 Project-URL: Homepage, https://docs.hyriver.io/readme/async-retriever.html
 Project-URL: Issues, https://github.com/hyriver/async-retriever/issues
```

### Comparing `async_retriever-0.3.7/async_retriever.egg-info/SOURCES.txt` & `async_retriever-0.3.8/async_retriever.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/ci/requirements/environment-dev.yml` & `async_retriever-0.3.8/ci/requirements/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/noxfile.py` & `async_retriever-0.3.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/pyproject.toml` & `async_retriever-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/setup.cfg` & `async_retriever-0.3.8/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -30,19 +30,17 @@
 	Issues = https://github.com/hyriver/async-retriever/issues
 	CI = https://github.com/hyriver/async-retriever/actions
 	Changelog = https://docs.hyriver.io/changelogs/async-retriever.html
 
 [options]
 packages = find:
 install_requires = 
-	aiodns
-	aiohttp>=3.8.1
+	aiohttp[speedups]>=3.8.1
 	aiohttp-client-cache>=0.7.3
 	aiosqlite
-	brotli
 	cytoolz
 	ujson
 python_requires = >=3.8
 include_package_data = True
 zip_safe = False
 
 [options.extras_require]
```

### Comparing `async_retriever-0.3.7/tests/test_async_retriever.py` & `async_retriever-0.3.8/tests/test_async_retriever.py`

 * *Files identical despite different names*

### Comparing `async_retriever-0.3.7/tests/test_exceptions.py` & `async_retriever-0.3.8/tests/test_exceptions.py`

 * *Files identical despite different names*

