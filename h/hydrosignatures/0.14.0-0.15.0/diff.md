# Comparing `tmp/hydrosignatures-0.14.0.tar.gz` & `tmp/hydrosignatures-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrosignatures-0.14.0.tar", last modified: Sun Mar  5 16:51:21 2023, max compression
+gzip compressed data, was "hydrosignatures-0.15.0.tar", last modified: Sun May  7 22:51:13 2023, max compression
```

## Comparing `hydrosignatures-0.14.0.tar` & `hydrosignatures-0.15.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:21.197584 hydrosignatures-0.14.0/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:21.193584 hydrosignatures-0.14.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:21.193584 hydrosignatures-0.14.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:21.193584 hydrosignatures-0.14.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-03-05 16:51:21.197584 hydrosignatures-0.14.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:21.189583 hydrosignatures-0.14.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:21.193584 hydrosignatures-0.14.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/ci/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:21.197584 hydrosignatures-0.14.0/hydrosignatures/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/hydrosignatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/hydrosignatures/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24879 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/hydrosignatures/hydrosignatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/hydrosignatures/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/hydrosignatures/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:21.197584 hydrosignatures-0.14.0/hydrosignatures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-03-05 16:51:21.000000 hydrosignatures-0.14.0/hydrosignatures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-05 16:51:21.000000 hydrosignatures-0.14.0/hydrosignatures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:51:21.000000 hydrosignatures-0.14.0/hydrosignatures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:51:20.000000 hydrosignatures-0.14.0/hydrosignatures.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-05 16:51:21.000000 hydrosignatures-0.14.0/hydrosignatures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-05 16:51:21.000000 hydrosignatures-0.14.0/hydrosignatures.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 16:51:21.197584 hydrosignatures-0.14.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:21.197584 hydrosignatures-0.14.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   144810 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/tests/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/tests/test_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-05 16:51:04.000000 hydrosignatures-0.14.0/tests/test_hydrosignatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:13.253622 hydrosignatures-0.15.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:13.249622 hydrosignatures-0.15.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:13.249622 hydrosignatures-0.15.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:13.249622 hydrosignatures-0.15.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-05-07 22:51:13.249622 hydrosignatures-0.15.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:13.245622 hydrosignatures-0.15.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:13.249622 hydrosignatures-0.15.0/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/ci/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:13.249622 hydrosignatures-0.15.0/hydrosignatures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/hydrosignatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/hydrosignatures/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24943 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/hydrosignatures/hydrosignatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/hydrosignatures/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/hydrosignatures/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:13.249622 hydrosignatures-0.15.0/hydrosignatures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-05-07 22:51:13.000000 hydrosignatures-0.15.0/hydrosignatures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-07 22:51:13.000000 hydrosignatures-0.15.0/hydrosignatures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 22:51:13.000000 hydrosignatures-0.15.0/hydrosignatures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 22:51:12.000000 hydrosignatures-0.15.0/hydrosignatures.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 22:51:13.000000 hydrosignatures-0.15.0/hydrosignatures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 22:51:13.000000 hydrosignatures-0.15.0/hydrosignatures.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 22:51:13.253622 hydrosignatures-0.15.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:13.249622 hydrosignatures-0.15.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   144810 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/tests/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/tests/test_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-07 22:50:56.000000 hydrosignatures-0.15.0/tests/test_hydrosignatures.py
```

### Comparing `hydrosignatures-0.14.0/.github/ISSUE_TEMPLATE/bugreport.yml` & `hydrosignatures-0.15.0/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/.github/ISSUE_TEMPLATE/newfeature.yml` & `hydrosignatures-0.15.0/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/.github/workflows/codeql-analysis.yml` & `hydrosignatures-0.15.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/.github/workflows/release.yml` & `hydrosignatures-0.15.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/.github/workflows/test.yml` & `hydrosignatures-0.15.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/.gitignore` & `hydrosignatures-0.15.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/.pre-commit-config.yaml` & `hydrosignatures-0.15.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
   - id: check-toml
   - id: check-yaml
   - id: debug-statements
   - id: mixed-line-ending
     args: [--fix=lf]
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: 0.9.2
+  rev: 0.11.1
   hooks:
   - id: pyproject-fmt
     name: Apply a consistent format to pyproject.toml
 
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.7.0
+  rev: v2.8.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
 
 - repo: https://github.com/hadialqattan/pycln
   rev: v2.1.3
   hooks:
@@ -48,29 +48,29 @@
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
   - id: isort
     name: Sort imports with isort
 
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
     name: Autoformat with black
 
 - repo: https://github.com/asottile/blacken-docs
   rev: 1.13.0
   hooks:
   - id: blacken-docs
     name: Autoformat codes in docstrings with blacken-docs
     additional_dependencies: [black]
     args: [-t, py38, -l, '100']
 
 - repo: https://github.com/guilatrova/tryceratops
-  rev: v1.1.0
+  rev: v2.0.0
   hooks:
   - id: tryceratops
     name: Check try-exceptions blocks with tryceratops
 
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: v1.10.0
   hooks:
@@ -83,23 +83,23 @@
   rev: v1.1.1
   hooks:
   - id: doc8
     name: Check documentation formats with doc8
     args: [--max-line-length, '100']
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.2
+  rev: v2.2.4
   hooks:
   - id: codespell
     name: Check common misspellings in text files with codespell.
     additional_dependencies:
     - tomli
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.4.0
   hooks:
   - id: pyupgrade
     name: Upgrade sytnax to python 3.8+ with pyupgrade
     args: [--py38-plus]
 
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
@@ -111,24 +111,25 @@
     - flake8-builtins
     - flake8-blind-except
     - flake8-bugbear
     - flake8-use-fstring
     - flake8-docstrings
     - flake8-type-checking
     - flake8-simplify
+    - flake8-print
     - pep8-naming
 
 - repo: https://github.com/dosisod/refurb
-  rev: v1.13.0
+  rev: v1.16.0
   hooks:
   - id: refurb
     name: Modernizing Python codebases using Refurb
     additional_dependencies:
     - numpy
 
 - repo: https://github.com/PyCQA/bandit
-  rev: 1.7.4
+  rev: 1.7.5
   hooks:
   - id: bandit
     name: Check for security issues with bandit
     args: [-lll]
     files: .py$
```

### Comparing `hydrosignatures-0.14.0/CITATION.cff` & `hydrosignatures-0.15.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/CODE_OF_CONDUCT.rst` & `hydrosignatures-0.15.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/CONTRIBUTING.rst` & `hydrosignatures-0.15.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/HISTORY.rst` & `hydrosignatures-0.15.0/HISTORY.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 =======
 History
 =======
 
+0.15.0 (2023-05-07)
+-------------------
+From release 0.15 onward, all minor versions of HyRiver packages
+will be pinned. This ensures that previous minor versions of HyRiver
+packages cannot be installed with later minor releases. For example,
+if you have ``py3dep==0.14.x`` installed, you cannot install
+``pydaymet==0.15.x``. This is to ensure that the API is
+consistent across all minor versions.
+
+Internal Changes
+~~~~~~~~~~~~~~~~
+- Explicitly use ``nopython`` mode in ``numba``-decorated functions
+  to avoid deprecation warnings.
+
 0.14.0 (2023-03-05)
 -------------------
 
 Bug Fixes
 ~~~~~~~~~
 - Address an issue in ``compute_fdc_slope`` where if the input
   includes NANs, it returns NAN. Now, the function correctly
```

### Comparing `hydrosignatures-0.14.0/LICENSE` & `hydrosignatures-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/PKG-INFO` & `hydrosignatures-0.15.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: hydrosignatures
-Version: 0.14.0
+Version: 0.15.0
 Summary: A collection of tools for computing hydrological signatures
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/hydrosignatures/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/hydrosignatures.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/hydrosignatures.html
 Project-URL: Issues, https://github.com/hyriver/hydrosignatures/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
```

### Comparing `hydrosignatures-0.14.0/README.rst` & `hydrosignatures-0.15.0/README.rst`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/ci/requirements/environment-dev.yml` & `hydrosignatures-0.15.0/ci/requirements/environment-dev.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 name: hyriver-dev
 channels:
-- numba
 - conda-forge
 - nodefaults
 dependencies:
 - python>=3.10
 
 # async-retriever deps
 - aiodns
@@ -18,15 +17,14 @@
 
 # pygeoogc deps
 # - async-retriever >=0.3.5
 - cytoolz
 - defusedxml
 - owslib >=0.27.2
 - pyproj >=2.2
-- pyyaml
 - requests
 - requests-cache >=0.9.6
 - shapely >=2.0
 - urllib3
 
 # pygeoutils deps
 - cytoolz
@@ -142,14 +140,15 @@
 - pytables
 - ffmpeg
 - xarray-spatial
 - datashader
 
 # dev deps
 - ipywidgets
+- ipykernel
 - codespell
 - tomli
 - nox
 - pre-commit
 - psutil
 - pytest-cov
 - pytest-xdist
```

### Comparing `hydrosignatures-0.14.0/ci/requirements/environment.yml` & `hydrosignatures-0.15.0/ci/requirements/environment.yml`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
   # pygeoogc deps
   # - async-retriever >=0.3.5
 - cytoolz
 - defusedxml
 - owslib >=0.27.2
 - pyproj >=2.2
-- pyyaml
 - requests
 - requests-cache >=0.9.6
 - shapely >=2.0
 - urllib3
 
   # pygeoutils deps
 - cytoolz
```

### Comparing `hydrosignatures-0.14.0/hydrosignatures/__init__.py` & `hydrosignatures-0.15.0/hydrosignatures/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/hydrosignatures/exceptions.py` & `hydrosignatures-0.15.0/hydrosignatures/exceptions.py`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/hydrosignatures/hydrosignatures.py` & `hydrosignatures-0.15.0/hydrosignatures/hydrosignatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 import xarray as xr
 from scipy import signal
 
 from hydrosignatures.exceptions import InputRangeError, InputTypeError, InputValueError
 
 try:
     from numba import config as numba_config
-    from numba import njit, prange
+    from numba import jit, prange
 
-    ngjit = functools.partial(njit, cache=True, nogil=True)
+    ngjit = functools.partial(jit, nopython=True, cache=True, nogil=True)
     numba_config.THREADING_LAYER = "workqueue"
     has_numba = True
 except ImportError:
     has_numba = False
     prange = range
     numba_config = None
-    njit = None
+    jit = None
 
     R = TypeVar("R")
 
     def ngjit(ntypes: str, parallel: bool | None = None) -> Callable[..., Any]:
         def decorator_njit(func: Callable[..., R]) -> Callable[..., R]:
             @functools.wraps(func)
             def wrapper_decorator(*args: Any, **kwargs: Any):
@@ -203,19 +203,21 @@
     dayofyear = daily.index.dayofyear
     return daily.rolling(30).mean().groupby(dayofyear).mean()
 
 
 @ngjit("f8[::1](f8[::1], f8)")
 def __forward_pass(q: npt.NDArray[np.float64], alpha: float) -> npt.NDArray[np.float64]:
     """Perform forward pass of the Lyne and Hollick filter."""
-    qf = np.zeros_like(q)
-    qf[0] = q[0]
+    qb = np.zeros_like(q)
+    qb[0] = q[0]
     for i in range(1, q.size):
-        qf[i] = alpha * qf[i - 1] + 0.5 * (1 + alpha) * (q[i] - q[i - 1])
-    qb = np.where(qf > 0, q - qf, q)
+        qb[i] = alpha * qb[i - 1] + 0.5 * (1 + alpha) * (q[i] - q[i - 1])
+
+    for i in range(q.size):
+        qb[i] = q[i] - qb[i] if qb[i] > 0 else q[i]
     return qb
 
 
 @ngjit("f8[:,::1](f8[:,::1], f8)", parallel=True)
 def __batch_forward(q: npt.NDArray[np.float64], alpha: float) -> npt.NDArray[np.float64]:
     """Perform forward pass of the Lyne and Hollick filter."""
     qb = np.zeros_like(q)
@@ -591,15 +593,15 @@
                 "precipitation": compute_mean_monthly(self.p_mmpt, index_abbr=True),
             }
         )
 
     def seasonality_index(self) -> np.float64:
         """Compute seasonality index."""
         if self.si_method == "walsh":
-            return np.float64(compute_si_walsh(self.q_mmpt))
+            return np.float64(compute_si_walsh(self.q_mmpt).iloc[0])
         if self.si_method == "markham":
             return np.float64(compute_si_markham(self.q_mmpt).seasonality_index.iloc[0])
         raise InputValueError("method", ["walsh", "markham"])
 
     def mean_annual_flood(self) -> np.float64:
         """Compute mean annual flood."""
         return np.float64(self.q_mmpt.resample("Y").max().mean())
```

### Comparing `hydrosignatures-0.14.0/hydrosignatures/print_versions.py` & `hydrosignatures-0.15.0/hydrosignatures/print_versions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utility functions for printing version information.
 
 The original script is from
 `xarray <https://github.com/pydata/xarray/blob/master/xarray/util/print_versions.py>`__
 """
+# pyright: reportMissingImports=false
 from __future__ import annotations
 
 import importlib
 import importlib.util
 import locale
 import os
 import platform
@@ -21,20 +22,20 @@
 
 
 def netcdf_and_hdf5_versions() -> list[tuple[str, str | None]]:
     libhdf5_version = None
     libnetcdf_version = None
 
     if importlib.util.find_spec("netCDF4"):
-        import netCDF4  # type: ignore
+        import netCDF4
 
         libhdf5_version = netCDF4.__hdf5libversion__
         libnetcdf_version = netCDF4.__netcdf4libversion__
     elif importlib.util.find_spec("h5py"):
-        import h5py  # type: ignore
+        import h5py
 
         libhdf5_version = h5py.version.hdf5_version
 
     return [("libhdf5", libhdf5_version), ("libnetcdf", libnetcdf_version)]
 
 
 def get_sys_info() -> list[tuple[str, str | None]]:
@@ -56,15 +57,15 @@
             v = os.environ.get(k)
             if v is not None:
                 env[k] = v
         # LANGUAGE is used on win32
         env["LANGUAGE"] = "C"
         env["LANG"] = "C"
         env["LC_ALL"] = "C"
-        out = subprocess.check_output(cmd, stderr=subprocess.STDOUT, env=env)
+        out = subprocess.check_output(cmd, stderr=subprocess.STDOUT, env=env)  # noqa: S603
         return out
 
     commit = None
     try:
         out = _minimal_ext_cmd(["git", "rev-parse", "HEAD"])
         commit = out.strip().decode("ascii")
     except (subprocess.SubprocessError, OSError):
```

### Comparing `hydrosignatures-0.14.0/hydrosignatures.egg-info/PKG-INFO` & `hydrosignatures-0.15.0/hydrosignatures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: hydrosignatures
-Version: 0.14.0
+Version: 0.15.0
 Summary: A collection of tools for computing hydrological signatures
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/hydrosignatures/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/hydrosignatures.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/hydrosignatures.html
 Project-URL: Issues, https://github.com/hyriver/hydrosignatures/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
```

### Comparing `hydrosignatures-0.14.0/hydrosignatures.egg-info/SOURCES.txt` & `hydrosignatures-0.15.0/hydrosignatures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/noxfile.py` & `hydrosignatures-0.15.0/noxfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,40 @@
+from __future__ import annotations
+
 import shutil
 import textwrap
 from pathlib import Path
 
 import nox
 
 try:
     import tomllib as tomli
 except ImportError:
     import tomli
 
 
 def get_package_name() -> str:
     """Get the name of the package."""
-    with open("pyproject.toml", "rb") as f:
+    with Path("pyproject.toml").open("rb") as f:
         return tomli.load(f)["project"]["name"]
 
 
 def get_extras() -> list[str]:
     """Get the name of the package."""
-    with open("pyproject.toml", "rb") as f:
+    with Path("pyproject.toml").open("rb") as f:
         extras = tomli.load(f)["project"]["optional-dependencies"]
     return [e for e in extras if e not in ("test", "typeguard")]
 
 
+def get_deps() -> list[str]:
+    """Get the name of the package."""
+    with Path("pyproject.toml").open("rb") as f:
+        return tomli.load(f)["project"]["dependencies"]
+
+
 python_versions = ["3.8"]
 lint_versions = ["3.11"]
 package = get_package_name()
 gh_deps = {
     "async-retriever": [],
     "hydrosignatures": [],
     "pygeoogc": ["async-retriever"],
@@ -37,21 +45,26 @@
     "pydaymet": ["async-retriever", "pygeoogc", "pygeoutils", "py3dep"],
     "pynldas2": ["async-retriever", "pygeoutils"],
 }
 nox.options.sessions = (
     "pre-commit",
     "type-check",
     "tests",
+    "test-shapely",
 )
 
 
-def install_deps(session: nox.Session, extra=None) -> None:
+def install_deps(
+    session: nox.Session, extra: str | None = None, version_limit: list[str] | None = None
+) -> None:
     """Install package dependencies."""
     deps = [f".[{extra}]"] if extra else ["."]
     deps += [f"git+https://github.com/hyriver/{p}.git" for p in gh_deps[package]]
+    if version_limit:
+        deps += [p for p in version_limit]
     session.install(*deps)
     dirs = [".pytest_cache", "build", "dist", ".eggs"]
     for d in dirs:
         shutil.rmtree(d, ignore_errors=True)
 
     patterns = ["*.egg-info", "*.egg", "*.pyc", "*~", "**/__pycache__"]
     for p in patterns:
@@ -143,7 +156,19 @@
         install_deps(session, "speedup")
         session.run("pytest", "--doctest-modules", "-m", "speedup", *session.posargs)
     else:
         install_deps(session, ",".join(["test"] + extras))
         session.run("pytest", "--doctest-modules", *session.posargs)
         session.run("coverage", "report")
         session.run("coverage", "html")
+
+
+@nox.session(name="test-shapely", python=python_versions)
+def test_shapely(session: nox.Session) -> None:
+    """Run the test suite with shapely<2."""
+    extras = get_extras()
+    deps = get_deps()
+    if any("shapely" in d for d in deps):
+        install_deps(session, ",".join(["test"] + extras), ["pygeos", "shapely<2"])
+        session.run("pytest", "--doctest-modules", *session.posargs)
+    else:
+        session.skip("No shapely dependency found.")
```

### Comparing `hydrosignatures-0.14.0/pyproject.toml` & `hydrosignatures-0.15.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: GIS",
   "Topic :: Scientific/Engineering :: Hydrology",
-  "Typing :: Typed"
+  "Typing :: Typed",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "numpy>=1.21",
   "pandas>=1",
```

### Comparing `hydrosignatures-0.14.0/tests/test_data.csv` & `hydrosignatures-0.15.0/tests/test_data.csv`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/tests/test_data.json` & `hydrosignatures-0.15.0/tests/test_data.json`

 * *Files identical despite different names*

### Comparing `hydrosignatures-0.14.0/tests/test_hydrosignatures.py` & `hydrosignatures-0.15.0/tests/test_hydrosignatures.py`

 * *Files identical despite different names*

