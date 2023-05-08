# Comparing `tmp/audmetric-1.1.6.tar.gz` & `tmp/audmetric-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audmetric-1.1.6.tar", last modified: Tue Jan  3 13:16:22 2023, max compression
+gzip compressed data, was "audmetric-1.2.0.tar", last modified: Mon May  8 12:55:33 2023, max compression
```

## Comparing `audmetric-1.1.6.tar` & `audmetric-1.2.0.tar`

### file list

```diff
@@ -1,50 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.837037 audmetric-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.829037 audmetric-1.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.833037 audmetric-1.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-01-03 13:16:05.000000 audmetric-1.1.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-01-03 13:16:05.000000 audmetric-1.1.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-03 13:16:05.000000 audmetric-1.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-03 13:16:05.000000 audmetric-1.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-01-03 13:16:05.000000 audmetric-1.1.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-01-03 13:16:05.000000 audmetric-1.1.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-01-03 13:16:05.000000 audmetric-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-01-03 13:16:22.837037 audmetric-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-01-03 13:16:05.000000 audmetric-1.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.833037 audmetric-1.1.6/audmetric/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-03 13:16:05.000000 audmetric-1.1.6/audmetric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.837037 audmetric-1.1.6/audmetric/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:05.000000 audmetric-1.1.6/audmetric/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-01-03 13:16:05.000000 audmetric-1.1.6/audmetric/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-01-03 13:16:05.000000 audmetric-1.1.6/audmetric/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.837037 audmetric-1.1.6/audmetric/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-03 13:16:05.000000 audmetric-1.1.6/audmetric/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.833037 audmetric-1.1.6/audmetric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-01-03 13:16:22.000000 audmetric-1.1.6/audmetric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-01-03 13:16:22.000000 audmetric-1.1.6/audmetric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 13:16:22.000000 audmetric-1.1.6/audmetric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-03 13:16:22.000000 audmetric-1.1.6/audmetric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-03 13:16:22.000000 audmetric-1.1.6/audmetric.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.837037 audmetric-1.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.829037 audmetric-1.1.6/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.837037 audmetric-1.1.6/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.837037 audmetric-1.1.6/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/api-src/audmetric.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/api-src/audmetric.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-03 13:16:05.000000 audmetric-1.1.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-03 13:16:05.000000 audmetric-1.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-01-03 13:16:22.837037 audmetric-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-03 13:16:05.000000 audmetric-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:16:22.837037 audmetric-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-03 13:16:05.000000 audmetric-1.1.6/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-01-03 13:16:05.000000 audmetric-1.1.6/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-01-03 13:16:05.000000 audmetric-1.1.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.482677 audmetric-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-08 12:55:15.000000 audmetric-1.2.0/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-08 12:55:15.000000 audmetric-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-08 12:55:15.000000 audmetric-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-08 12:55:15.000000 audmetric-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 12:55:15.000000 audmetric-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-08 12:55:15.000000 audmetric-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-08 12:55:15.000000 audmetric-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-08 12:55:15.000000 audmetric-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-08 12:55:33.482677 audmetric-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-08 12:55:15.000000 audmetric-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/audmetric/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-08 12:55:15.000000 audmetric-1.2.0/audmetric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/audmetric/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:15.000000 audmetric-1.2.0/audmetric/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-05-08 12:55:15.000000 audmetric-1.2.0/audmetric/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-08 12:55:15.000000 audmetric-1.2.0/audmetric/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/audmetric/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 12:55:15.000000 audmetric-1.2.0/audmetric/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/audmetric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-08 12:55:33.000000 audmetric-1.2.0/audmetric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 12:55:33.000000 audmetric-1.2.0/audmetric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:55:33.000000 audmetric-1.2.0/audmetric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 12:55:33.000000 audmetric-1.2.0/audmetric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 12:55:33.000000 audmetric-1.2.0/audmetric.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.482677 audmetric-1.2.0/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/api-src/audmetric.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/api-src/audmetric.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-08 12:55:15.000000 audmetric-1.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 12:55:15.000000 audmetric-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-08 12:55:33.482677 audmetric-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 12:55:15.000000 audmetric-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.482677 audmetric-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.478677 audmetric-1.2.0/tests/assests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:55:33.482677 audmetric-1.2.0/tests/assests/linkability/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 12:55:15.000000 audmetric-1.2.0/tests/assests/linkability/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-08 12:55:15.000000 audmetric-1.2.0/tests/assests/linkability/linkability_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-08 12:55:15.000000 audmetric-1.2.0/tests/assests/linkability/results.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 12:55:15.000000 audmetric-1.2.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-05-08 12:55:15.000000 audmetric-1.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-08 12:55:15.000000 audmetric-1.2.0/tests/test_linkability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-08 12:55:15.000000 audmetric-1.2.0/tests/test_utils.py
```

### Comparing `audmetric-1.1.6/.github/workflows/publish.yml` & `audmetric-1.2.0/.github/workflows/publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       uses: actions/setup-python@v4
       with:
         python-version: '3.8'
 
     - name: Set up Node.js
       uses: actions/setup-node@v3
       with:
-        node-version: 10.7
+        node-version: '16.0'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
 
     - name: Prepare KaTeX server
@@ -74,9 +74,9 @@
     - name: Create release on Github
       id: create_release
       uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ github.ref }}
-        release_name: Release ${{ github.ref_name }}
+        name: Release ${{ github.ref_name }}
         body: ${{ steps.changelog.outputs.body }}
```

### Comparing `audmetric-1.1.6/.github/workflows/test.yml` & `audmetric-1.2.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -36,22 +36,14 @@
       run: |
         python -V
         python -m pip install --upgrade pip
         pip install -r requirements.txt
         pip install -r docs/requirements.txt
         pip install -r tests/requirements.txt
 
-    - name: Install pre-commit hooks
-      run: |
-        pre-commit install --install-hooks
-
-    - name: Code style check via pre-commit
-      run: |
-        pre-commit run --all-files
-
     - name: Test with pytest
       run: |
         python -m pytest
 
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
```

### Comparing `audmetric-1.1.6/CHANGELOG.rst` & `audmetric-1.2.0/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.2.0 (2023/05/08)
+--------------------------
+
+* Added: ``audmetric.linkability()``
+* Changed: speedup ``audmetric.concordance_cc()``
+  and ``audmetric.pearson_cc()``
+  when providing ``truth``
+  and/or ``prediction``
+  as numpy arrays
+
+
 Version 1.1.6 (2023/01/03)
 --------------------------
 
 * Fixed: require ``sphinx-audeering-theme>=1.2.1``
   to enforce correct theme
   in published docs
```

### Comparing `audmetric-1.1.6/CONTRIBUTING.rst` & `audmetric-1.2.0/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 and check for correct syntax with flake8_.
 Exceptions are defined under the ``[flake8]`` section
 in :file:`setup.cfg`.
 
 The checks are executed in the CI using `pre-commit`_.
 You can enable those checks locally by executing::
 
-    pip install -r tests/requirements.txt
+    pip install pre-commit  # consider system wide installation
     pre-commit install
     pre-commit run --all-files
 
 Afterwards flake8_ is executed
 every time you create a commit.
 
 You can also install flake8_
 and call it directly::
 
-    pip install flake8  # you might consider system wide installation
+    pip install flake8  # consider system wide installation
     flake8
 
 It can be restricted to specific folders::
 
     flake8 audfoo/ tests/
 
 .. _PEP8: http://www.python.org/dev/peps/pep-0008/
```

### Comparing `audmetric-1.1.6/LICENSE` & `audmetric-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audmetric-1.1.6/PKG-INFO` & `audmetric-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audmetric
-Version: 1.1.6
+Version: 1.2.0
 Summary: Evaluate machine-learning models
 Home-page: https://audeering.github.io/audmetric/
 Author: Johannes Wagner, Hagen Wierstorf, Stephan Huber, Andreas Triantafyllopoulos, Uwe Reichel
 Author-email: jwagner@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audmetric/
 Description: =========
@@ -49,14 +49,25 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.2.0 (2023/05/08)
+        --------------------------
+        
+        * Added: ``audmetric.linkability()``
+        * Changed: speedup ``audmetric.concordance_cc()``
+          and ``audmetric.pearson_cc()``
+          when providing ``truth``
+          and/or ``prediction``
+          as numpy arrays
+        
+        
         Version 1.1.6 (2023/01/03)
         --------------------------
         
         * Fixed: require ``sphinx-audeering-theme>=1.2.1``
           to enforce correct theme
           in published docs
```

### Comparing `audmetric-1.1.6/README.rst` & `audmetric-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `audmetric-1.1.6/audmetric/__init__.py` & `audmetric-1.2.0/audmetric/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     concordance_cc,
     confusion_matrix,
     detection_error_tradeoff,
     edit_distance,
     equal_error_rate,
     event_error_rate,
     fscore_per_class,
+    linkability,
     mean_absolute_error,
     mean_squared_error,
     pearson_cc,
     precision_per_class,
     recall_per_class,
     unweighted_average_bias,
     unweighted_average_fscore,
```

### Comparing `audmetric-1.1.6/audmetric/core/api.py` & `audmetric-1.2.0/audmetric/core/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import namedtuple
+import collections
 import operator
 import typing
 import warnings
 
 import numpy as np
 
 import audeer
@@ -102,16 +102,18 @@
     Examples:
         >>> concordance_cc([0, 1, 2], [0, 1, 1])
         0.6666666666666666
 
     """
     assert_equal_length(truth, prediction)
 
-    prediction = np.array(list(prediction))
-    truth = np.array(list(truth))
+    if not isinstance(truth, np.ndarray):
+        truth = np.array(list(truth))
+    if not isinstance(prediction, np.ndarray):
+        prediction = np.array(list(prediction))
 
     if len(prediction) < 2:
         return np.NaN
 
     r = pearson_cc(prediction, truth)
     x_mean = prediction.mean()
     y_mean = truth.mean()
@@ -240,32 +242,19 @@
     Examples:
         >>> truth = [1, 0]
         >>> prediction = [0.9, 0.1]
         >>> detection_error_tradeoff(truth, prediction)
         (array([1., 0.]), array([0., 0.]), array([0.1, 0.9]))
 
     """  # noqa: E501
-    truth = np.array(truth)
-
-    allowed_truth_values = set([1, 0, True, False])
-    if not set(truth).issubset(allowed_truth_values):
-        raise ValueError(
-            "'truth' is only allowed to contain "
-            "[1, 0, True, False], "
-            'yours contains:\n'
-            f"[{', '.join([str(t) for t in set(truth)])}]"
-        )
-
-    truth = truth.astype(bool)
-    prediction = np.array(prediction).astype(np.float64)
-
-    # Genuine matching scores
-    gscores = prediction[truth]
-    # Impostor matching scores
-    iscores = prediction[~truth]
+    # Get mated scores
+    # (genuine matching scores)
+    # and non-mated scores
+    # (impostor matching scores)
+    gscores, iscores = _matching_scores(truth, prediction)
 
     gscores_number = len(gscores)
     iscores_number = len(iscores)
 
     # Labeling genuine scores as 1 and impostor scores as 0
     gscores = list(zip(gscores, [1] * gscores_number))
     iscores = list(zip(iscores, [0] * iscores_number))
@@ -351,15 +340,15 @@
         typing.Union[bool, int],
         typing.Sequence[typing.Union[bool, int]]
     ],
     prediction: typing.Union[
         typing.Union[bool, int, float],
         typing.Sequence[typing.Union[bool, int, float]]
     ],
-) -> typing.Tuple[float, namedtuple]:
+) -> typing.Tuple[float, collections.namedtuple]:
     r"""Equal error rate for verification tasks.
 
     The equal error rate (EER) is the point
     where false non-match rate (FNMR)
     and the impostors or false match rate (FMR)
     are identical.
     The FNMR indicates
@@ -416,15 +405,15 @@
         >>> eer, stats = equal_error_rate(truth, prediction)
         >>> eer
         0.16666666666666666
         >>> stats.threshold
         0.5
 
     """
-    Stats = namedtuple(
+    Stats = collections.namedtuple(
         'stats',
         [
             'fmr',  # False match rates (FMR)
             'fnmr',  # False non-match rates (FNMR)
             'thresholds',  # Thresholds
             'threshold',  # verification threshold for EER
         ],
@@ -569,14 +558,124 @@
         elif (p == 0.0 and np.isnan(r)) or (r == 0.0 and np.isnan(p)):
             fscore[label] = 0.0
         else:
             fscore[label] = (2 * p * r) / (p + r)
     return fscore
 
 
+def linkability(
+        truth: typing.Union[
+            typing.Union[bool, int],
+            typing.Sequence[typing.Union[bool, int]]
+        ],
+        prediction: typing.Union[
+            typing.Union[bool, int, float],
+            typing.Sequence[typing.Union[bool, int, float]]
+        ],
+        omega: float = 1.0,
+        nbins: int = None,
+) -> float:
+    r"""Linkability for verification tasks.
+
+    Let :math:`s` be the provided prediction score
+    for the similarity of the tested sample.
+    The clipped local linkability metric is then defined as:
+
+    .. math::
+
+        \text{max}(0, p(\text{mated} | s) - p(\text{non-mated} | s))
+
+    The higher the value,
+    the more likely
+    that an attacker can link two mated samples.
+    The global linkability metric :math:`D_\text{sys}`
+    is the mean value
+    over all local scores,\ :footcite:`GomezBarrero2017`
+    and in the range :math:`0` and :math:`1`.
+
+    Implementation is based on
+    `code from M. Maouche`_,
+    which is licensed under LGPL.
+
+    .. footbibliography::
+
+    .. _code from M. Maouche: https://gitlab.inria.fr/magnet/anonymization_metrics
+
+    Args:
+        truth: ground truth classes
+        prediction: predicted classes or similarity scores
+        omega: prior ratio
+            :math:`\frac{p(\text{mated})}{p(\text{non-mated})}`
+        nbins: number of bins
+            of the histograms
+            that estimate the distributions
+            of mated and non-mated scores.
+            If ``None`` it is set to
+            :math:`\min(\frac{\text{len}(\text{mated})}{10}, 100)`
+
+    Returns:
+        global linkability :math:`D_\text{sys}`
+
+    Raises:
+        ValueError: if ``truth`` contains values
+            different from ``1``, ``0``, ``True``, ``False``
+
+    Examples:
+        >>> np.random.seed(1)
+        >>> samples = 10000
+        >>> truth = [1, 0] * int(samples / 2)
+        >>> prediction = []
+        >>> for _ in range(int(samples / 2)):
+        ...     prediction.extend(
+        ...         [np.random.uniform(0, 0.2), np.random.uniform(0.8, 1.0)]
+        ...     )
+        >>> linkability(truth, prediction)
+        0.9747999999999999
+        >>> truth = [1, 0, 0, 0] * int(samples / 4)
+        >>> prediction = [np.random.uniform(0, 1) for _ in range(samples)]
+        >>> linkability(truth, prediction, omega=1/3)
+        0.0
+
+    """  # noqa: E501
+    mated_scores, non_mated_scores = _matching_scores(truth, prediction)
+
+    # Limiting the number of bins
+    # (100 maximum or lower if few scores available)
+    if nbins is None:
+        nbins = min(int(len(mated_scores) / 10), 100)
+
+    # Define range of scores to compute D
+    bin_edges = np.linspace(
+        min([min(mated_scores), min(non_mated_scores)]),
+        max([max(mated_scores), max(non_mated_scores)]),
+        num=nbins + 1,
+        endpoint=True,
+    )
+    bin_centers = (bin_edges[1:] + bin_edges[:-1]) / 2
+
+    # Compute score distributions using normalized histograms
+    y1 = np.histogram(mated_scores, bins=bin_edges, density=True)[0]
+    y2 = np.histogram(non_mated_scores, bins=bin_edges, density=True)[0]
+    # LR = P[s|mated ]/P[s|non-mated]
+    LR = np.divide(y1, y2, out=np.ones_like(y1), where=y2 != 0)
+    D = 2 * (omega * LR / (1 + omega*LR)) - 1
+    # Def of D
+    D[omega * LR <= 1] = 0
+    # Taking care of inf/NaN
+    mask = [
+        True if y2[i] == 0 and y1[i] != 0 else False
+        for i in range(len(y1))
+    ]
+    D[mask] = 1
+    # Global measure using trapz numerical integration
+    Dsys = np.trapz(x=bin_centers, y=D * y1)
+
+    return Dsys
+
+
 def mean_absolute_error(
         truth: typing.Sequence[float],
         prediction: typing.Sequence[float],
 ) -> float:
     r"""Mean absolute error.
 
     .. math::
@@ -668,16 +767,18 @@
     Examples:
         >>> pearson_cc([0, 1, 2], [0, 1, 1])
         0.8660254037844385
 
     """
     assert_equal_length(truth, prediction)
 
-    prediction = np.array(list(prediction))
-    truth = np.array(list(truth))
+    if not isinstance(truth, np.ndarray):
+        truth = np.array(list(truth))
+    if not isinstance(prediction, np.ndarray):
+        prediction = np.array(list(prediction))
 
     if len(prediction) < 2 or prediction.std() == 0:
         return np.NaN
     else:
         return float(np.corrcoef(prediction, truth)[0][1])
 
 
@@ -1134,7 +1235,83 @@
 
         n = max(len(t), len(p))
         n = n if n > 1 else 1
         wer += edit_distance(t, p) / n
 
     num_samples = len(truth) if len(truth) > 1 else 1
     return wer / num_samples
+
+
+def _matching_scores(
+    truth: typing.Union[
+        typing.Union[bool, int],
+        typing.Sequence[typing.Union[bool, int]]
+    ],
+    prediction: typing.Union[
+        typing.Union[bool, int, float],
+        typing.Sequence[typing.Union[bool, int, float]]
+    ],
+) -> typing.Tuple[np.ndarray, np.ndarray]:
+    r"""Mated and non-mated scores for verification tasks.
+
+    For verification task,
+    predictions are usually seperated
+    in all predictions belonging
+    to the matching examples,
+    and all other predictions.
+    The first are called mated scores
+    or genuine matching scores,
+    the second non-mated scores
+    or impostor matching scores.
+
+    For example,
+    in a speaker verification task
+    the mated scores are all similarity values
+    that belong to the matching speaker.
+
+    Args:
+        truth: ground truth classes
+        prediction: predicted classes or similarity scores
+
+    Returns:
+        * mated scores
+        * non-mated scores
+
+    Raises:
+        ValueError: if ``truth`` contains values
+            different from ``1, 0, True, False``
+
+    Examples:
+        >>> truth = [1, 0]
+        >>> prediction = [0.9, 0.1]
+        >>> _matching_scores(truth, prediction)
+        (array([0.9]), array([0.1]))
+
+    """
+    truth = np.array(truth)
+
+    allowed_truth_values = set([1, 0, True, False])
+    if not set(truth).issubset(allowed_truth_values):
+        raise ValueError(
+            "'truth' is only allowed to contain "
+            "[1, 0, True, False], "
+            'yours contains:\n'
+            f"[{', '.join([str(t) for t in set(truth)])}]"
+        )
+
+    truth = truth.astype(bool)
+    prediction = np.array(prediction).astype(np.float64)
+
+    # Predictions for all matching examples
+    # (truth is 1 or True)
+    # In literature these are called
+    # "genuine matching scores"
+    # or "mated scores"
+    mated_scores = prediction[truth]
+    # Predictions for all non-matching examples
+    # (truth is 0 or False)
+    # In literature these are called
+    # "impostor matching scores"
+    # or "non-mated scores"
+    non_mated_scores = prediction[~truth]
+
+    return mated_scores, non_mated_scores
```

### Comparing `audmetric-1.1.6/audmetric/core/utils.py` & `audmetric-1.2.0/audmetric/core/utils.py`

 * *Files identical despite different names*

### Comparing `audmetric-1.1.6/audmetric.egg-info/PKG-INFO` & `audmetric-1.2.0/audmetric.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audmetric
-Version: 1.1.6
+Version: 1.2.0
 Summary: Evaluate machine-learning models
 Home-page: https://audeering.github.io/audmetric/
 Author: Johannes Wagner, Hagen Wierstorf, Stephan Huber, Andreas Triantafyllopoulos, Uwe Reichel
 Author-email: jwagner@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audmetric/
 Description: =========
@@ -49,14 +49,25 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.2.0 (2023/05/08)
+        --------------------------
+        
+        * Added: ``audmetric.linkability()``
+        * Changed: speedup ``audmetric.concordance_cc()``
+          and ``audmetric.pearson_cc()``
+          when providing ``truth``
+          and/or ``prediction``
+          as numpy arrays
+        
+        
         Version 1.1.6 (2023/01/03)
         --------------------------
         
         * Fixed: require ``sphinx-audeering-theme>=1.2.1``
           to enforce correct theme
           in published docs
```

### Comparing `audmetric-1.1.6/audmetric.egg-info/SOURCES.txt` & `audmetric-1.2.0/audmetric.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 README.rst
 requirements.txt
 setup.cfg
 setup.py
+.github/workflows/flake8.yml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 audmetric/__init__.py
 audmetric.egg-info/PKG-INFO
 audmetric.egg-info/SOURCES.txt
 audmetric.egg-info/dependency_links.txt
 audmetric.egg-info/requires.txt
@@ -30,8 +31,12 @@
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/function.rst
 docs/api-src/audmetric.rst
 docs/api-src/audmetric.utils.rst
 tests/requirements.txt
 tests/test_api.py
-tests/test_utils.py
+tests/test_linkability.py
+tests/test_utils.py
+tests/assests/linkability/README.md
+tests/assests/linkability/linkability_reference.py
+tests/assests/linkability/results.txt
```

### Comparing `audmetric-1.1.6/docs/_templates/autosummary/class.rst` & `audmetric-1.2.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audmetric-1.1.6/docs/api-src/audmetric.rst` & `audmetric-1.2.0/docs/api-src/audmetric.rst`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     accuracy
     concordance_cc
     confusion_matrix
     detection_error_tradeoff
     edit_distance
     equal_error_rate
     event_error_rate
+    linkability
     mean_absolute_error
     mean_squared_error
     pearson_cc
     fscore_per_class
     precision_per_class
     recall_per_class
     unweighted_average_bias
```

### Comparing `audmetric-1.1.6/docs/conf.py` & `audmetric-1.2.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     'sphinxcontrib.katex',  # has to be before jupyter_sphinx
 ]
 
 napoleon_use_ivar = True  # List of class attributes
 autodoc_inherit_docstrings = False  # disable docstring inheritance
 bibtex_bibfiles = ['refs.bib']
 # Don't check for DOIs as they will always work
+# and tend to fail the test
 linkcheck_ignore = [
-    'https://doi.org/10.2307/2532051',
-    'https://doi.org/10.1109/34.990140',
+    'https://doi.org/',
 ]
 
 # Disable auto-generation of TOC entries in the API
 # https://github.com/sphinx-doc/sphinx/issues/6316
 toc_object_entries = False
```

### Comparing `audmetric-1.1.6/docs/index.rst` & `audmetric-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audmetric-1.1.6/docs/refs.bib` & `audmetric-1.2.0/docs/refs.bib`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+@article{GomezBarrero2017,
+    author={Gomez-Barrero, M. and Galbally, J. and Rathgeb, C. and Busch, C.},
+    title={General framework to evaluate unlinkability in biometric template protection systems},
+    journal={IEEE Transactions on Information Forensics and Security},
+    volume={13},
+    issue={6},
+    pages={1406--1420},
+    doi={10.1109/TIFS.2017.2788000},
+    year={2017}
+}
 @article{Lin1989,
     author={Lin, Lawrence I-Kuei},
     title={A concordance correlation coefficient to evaluate reproducibility},
     journal={Biometrics},
     volume={45},
     issue={1},
     pages={255--268},
```

### Comparing `audmetric-1.1.6/setup.cfg` & `audmetric-1.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 [tool:pytest]
 addopts = 
 	--doctest-plus
 	--cov=audmetric
 	--cov-fail-under=100
 	--cov-report xml
 	--cov-report term-missing
+	--ignore tests/assests/linkability/
 xfail_strict = true
 
 [flake8]
 exclude = 
 	.eggs,
 	build,
 extend-ignore =
```

### Comparing `audmetric-1.1.6/tests/test_api.py` & `audmetric-1.2.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `audmetric-1.1.6/tests/test_utils.py` & `audmetric-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

