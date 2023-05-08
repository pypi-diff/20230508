# Comparing `tmp/pynldas2-0.14.0.tar.gz` & `tmp/pynldas2-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynldas2-0.14.0.tar", last modified: Sun Mar  5 16:51:42 2023, max compression
+gzip compressed data, was "pynldas2-0.15.0.tar", last modified: Mon May  8 15:16:26 2023, max compression
```

## Comparing `pynldas2-0.14.0.tar` & `pynldas2-0.15.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:42.616249 pynldas2-0.14.0/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:42.612249 pynldas2-0.14.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:42.612249 pynldas2-0.14.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:42.612249 pynldas2-0.14.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-05 16:51:26.000000 pynldas2-0.14.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-05 16:51:26.000000 pynldas2-0.14.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-05 16:51:26.000000 pynldas2-0.14.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-05 16:51:26.000000 pynldas2-0.14.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-03-05 16:51:26.000000 pynldas2-0.14.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-05 16:51:26.000000 pynldas2-0.14.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-05 16:51:26.000000 pynldas2-0.14.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-05 16:51:26.000000 pynldas2-0.14.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-03-05 16:51:42.616249 pynldas2-0.14.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-03-05 16:51:26.000000 pynldas2-0.14.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:42.608249 pynldas2-0.14.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:42.612249 pynldas2-0.14.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-05 16:51:26.000000 pynldas2-0.14.0/ci/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-05 16:51:26.000000 pynldas2-0.14.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-05 16:51:26.000000 pynldas2-0.14.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-03-05 16:51:26.000000 pynldas2-0.14.0/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:42.616249 pynldas2-0.14.0/pynldas2/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-05 16:51:26.000000 pynldas2-0.14.0/pynldas2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-05 16:51:26.000000 pynldas2-0.14.0/pynldas2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-03-05 16:51:26.000000 pynldas2-0.14.0/pynldas2/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:26.000000 pynldas2-0.14.0/pynldas2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-03-05 16:51:26.000000 pynldas2-0.14.0/pynldas2/pynldas2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:42.616249 pynldas2-0.14.0/pynldas2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-03-05 16:51:42.000000 pynldas2-0.14.0/pynldas2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-05 16:51:42.000000 pynldas2-0.14.0/pynldas2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:51:42.000000 pynldas2-0.14.0/pynldas2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:51:42.000000 pynldas2-0.14.0/pynldas2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-05 16:51:42.000000 pynldas2-0.14.0/pynldas2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-05 16:51:42.000000 pynldas2-0.14.0/pynldas2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-03-05 16:51:26.000000 pynldas2-0.14.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 16:51:42.616249 pynldas2-0.14.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:51:42.616249 pynldas2-0.14.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-05 16:51:26.000000 pynldas2-0.14.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-05 16:51:26.000000 pynldas2-0.14.0/tests/test_pynldas2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 15:16:09.000000 pynldas2-0.15.0/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-08 15:16:09.000000 pynldas2-0.15.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 15:16:09.000000 pynldas2-0.15.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-08 15:16:09.000000 pynldas2-0.15.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-08 15:16:09.000000 pynldas2-0.15.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-08 15:16:09.000000 pynldas2-0.15.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-08 15:16:09.000000 pynldas2-0.15.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 15:16:09.000000 pynldas2-0.15.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-05-08 15:16:26.813196 pynldas2-0.15.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-08 15:16:09.000000 pynldas2-0.15.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.809196 pynldas2-0.15.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-08 15:16:09.000000 pynldas2-0.15.0/ci/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 15:16:09.000000 pynldas2-0.15.0/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-08 15:16:09.000000 pynldas2-0.15.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-08 15:16:09.000000 pynldas2-0.15.0/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/pynldas2/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pynldas2/pynldas2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/pynldas2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 15:16:26.000000 pynldas2-0.15.0/pynldas2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-08 15:16:09.000000 pynldas2-0.15.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:16:26.813196 pynldas2-0.15.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:16:26.813196 pynldas2-0.15.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-08 15:16:09.000000 pynldas2-0.15.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 15:16:09.000000 pynldas2-0.15.0/tests/test_pynldas2.py
```

### Comparing `pynldas2-0.14.0/.github/ISSUE_TEMPLATE/bugreport.yml` & `pynldas2-0.15.0/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/.github/ISSUE_TEMPLATE/newfeature.yml` & `pynldas2-0.15.0/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/.github/workflows/codeql-analysis.yml` & `pynldas2-0.15.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/.github/workflows/release.yml` & `pynldas2-0.15.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/.github/workflows/test.yml` & `pynldas2-0.15.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/.gitignore` & `pynldas2-0.15.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/.pre-commit-config.yaml` & `pynldas2-0.15.0/.pre-commit-config.yaml`

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
+  rev: v3.3.2
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

### Comparing `pynldas2-0.14.0/CITATION.cff` & `pynldas2-0.15.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/CODE_OF_CONDUCT.rst` & `pynldas2-0.15.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/CONTRIBUTING.rst` & `pynldas2-0.15.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/HISTORY.rst` & `pynldas2-0.15.0/HISTORY.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,36 @@
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
+New Features
+~~~~~~~~~~~~
+- Add ``source`` argument to both ``get_bygeom`` and ``get_bycoords`` functions.
+  Valid values for source are ``grib`` (default) and ``netcdf``.
+  Both return the same values, the latter also offers additional variable ``psurf``
+  for surface pressure.
+  Valid variable names for ``netcdf`` are:
+  ``prcp``, ``pet``, ``wind_u``, ``wind_v``, ``humidity``,
+  ``temp``, ``rsds``, ``rlds``, ``psurf``
+  Valid variable names for ``grib`` source are unchanged as to not
+  introduce breaking changes.
+
+By `Luc Rébillout <https://github.com/LucRSquared>`__.
+- For now, retain compatibility with ``shapely<2`` while supporting
+  ``shapley>=2``.
+
 0.14.0 (2023-03-05)
 -------------------
 
 New Features
 ~~~~~~~~~~~~
 - Add ``snow`` and ``snow_params`` arguments to both ``get_bygeom``
   and ``get_bycoords`` functions for computing snow from ``prcp``
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pynldas2-0.14.0/LICENSE` & `pynldas2-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/PKG-INFO` & `pynldas2-0.15.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pynldas2
-Version: 0.14.0
+Version: 0.15.0
 Summary: Get NLDAS2 forcing data.
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/pynldas2/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pynldas2.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/pynldas2.html
 Project-URL: Issues, https://github.com/hyriver/pynldas2/issues
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
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
```

### Comparing `pynldas2-0.14.0/README.rst` & `pynldas2-0.15.0/README.rst`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/ci/requirements/environment-dev.yml` & `pynldas2-0.15.0/ci/requirements/environment-dev.yml`

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

### Comparing `pynldas2-0.14.0/ci/requirements/environment.yml` & `pynldas2-0.15.0/ci/requirements/environment.yml`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/noxfile.py` & `pynldas2-0.15.0/noxfile.py`

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

### Comparing `pynldas2-0.14.0/pynldas2/__init__.py` & `pynldas2-0.15.0/pynldas2/__init__.py`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/pynldas2/exceptions.py` & `pynldas2-0.15.0/pynldas2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/pynldas2/print_versions.py` & `pynldas2-0.15.0/pynldas2/print_versions.py`

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

### Comparing `pynldas2-0.14.0/pynldas2/pynldas2.py` & `pynldas2-0.15.0/pynldas2/pynldas2.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,24 +41,25 @@
 
             return wrapper_decorator
 
         return decorator_njit
 
 
 if TYPE_CHECKING:
-    from shapely import MultiPolygon, Polygon
+    from shapely.geometry import MultiPolygon, Polygon
 
     DF = TypeVar("DF", pd.DataFrame, xr.Dataset)
 
 # Default snow params from https://doi.org/10.5194/gmd-11-1077-2018
 T_RAIN = 2.5  # degC
 T_SNOW = 0.6  # degC
 CRSTYPE = Union[int, str, pyproj.CRS]
 URL = "https://hydro1.gesdisc.eosdis.nasa.gov/daac-bin/access/timeseries.cgi"
-NLDAS_VARS = {
+
+NLDAS_VARS_GRIB = {
     "prcp": {"nldas_name": "APCPsfc", "long_name": "Precipitation hourly total", "units": "mm"},
     "pet": {"nldas_name": "PEVAPsfc", "long_name": "Potential evaporation", "units": "mm"},
     "temp": {"nldas_name": "TMP2m", "long_name": "2-m above ground temperature", "units": "K"},
     "wind_u": {
         "nldas_name": "UGRD10m",
         "long_name": "10-m above ground zonal wind",
         "units": "m/s",
@@ -80,14 +81,51 @@
     },
     "humidity": {
         "nldas_name": "SPFH2m",
         "long_name": "2-m above ground specific humidity",
         "units": "kg/kg",
     },
 }
+
+NLDAS_VARS_NETCDF = {
+    "prcp": {"nldas_name": "Rainf", "long_name": "Total precipitation", "units": "kg/m^2"},
+    "rlds": {
+        "nldas_name": "LWdown",
+        "long_name": "Surface downward longwave radiation",
+        "units": "W/m^2",
+    },
+    "rsds": {
+        "nldas_name": "SWdown",
+        "long_name": "Surface downward shortwave radiation",
+        "units": "W/m^2",
+    },
+    "pet": {"nldas_name": "PotEvap", "long_name": "Potential evaporation", "units": "kg/m^2"},
+    "psurf": {"nldas_name": "PSurf", "long_name": "Surface pressure", "units": "Pa"},
+    "humidity": {
+        "nldas_name": "Qair",
+        "long_name": "2-m above ground specific humidity",
+        "units": "kg/kg",
+    },
+    "temp": {
+        "nldas_name": "Tair",
+        "long_name": "2-m above ground temperature",
+        "units": "K",
+    },
+    "wind_u": {
+        "nldas_name": "Wind_E",
+        "long_name": "U wind component at 10-m above the surface",
+        "units": "m/s",
+    },
+    "wind_v": {
+        "nldas_name": "Wind_N",
+        "long_name": "V wind component at 10-m above the surface",
+        "units": "m/s",
+    },
+}
+
 DATE_COL = "Date&Time"
 DATE_FMT = "%Y-%m-%dT%H"
 __all__ = ["get_bycoords", "get_grid_mask", "get_bygeom"]
 
 
 @ngjit("f8[::1](f8[::1], f8[::1], f8, f8)")
 def _separate_snow(
@@ -188,19 +226,28 @@
         raise InputTypeError("clm", "pandas.DataFrame or xarray.Dataset")
 
     if isinstance(clm, xr.Dataset):
         return _snow_gridded(clm, t_rain + 273.15, t_snow)  # type: ignore
     return _snow_point(clm, t_rain + 273.15, t_snow)
 
 
-def _txt2df(txt: str, resp_id: int, kwds: list[dict[str, dict[str, str]]]) -> pd.Series:
+def _txt2df(
+    txt: str,
+    resp_id: int,
+    kwds: list[dict[str, dict[str, str]]],
+    source: str = "grib",
+) -> pd.Series:
     """Convert text to dataframe."""
     try:
-        data = pd.read_csv(StringIO(txt), skiprows=39, delim_whitespace=True).dropna()
-        data.index = pd.to_datetime(data.index + " " + data[DATE_COL], utc=True)
+        if source == "grib":
+            data = pd.read_csv(StringIO(txt), skiprows=39, delim_whitespace=True).dropna()
+            data.index = pd.to_datetime(data.index + " " + data[DATE_COL], utc=True)
+        else:
+            data = pd.read_csv(StringIO(txt), skiprows=12, delim_whitespace=True).dropna()
+            data.index = pd.to_datetime(data[DATE_COL], utc=True)
     except EmptyDataError:
         return pd.Series(name=kwds[resp_id]["params"]["variable"].split(":")[-1])
     except UFuncTypeError as ex:
         msg = "".join(re.findall("<strong>(.*?)</strong>", txt, re.DOTALL)).strip()
         raise NLDASServiceError(msg) from ex
 
     data = data.drop(columns=DATE_COL)["Data"]
@@ -209,52 +256,63 @@
 
 
 def _check_inputs(
     start_date: str,
     end_date: str,
     variables: str | list[str] | None = None,
     snow: bool = False,
-) -> tuple[list[pd.Timestamp], list[str]]:
+    source: str = "grib",
+) -> tuple[list[pd.Timestamp], list[str], dict[str, dict[str, str]]]:
     """Check inputs."""
     start = pd.to_datetime(start_date)
     end = pd.to_datetime(end_date) + pd.Timedelta("1D")
     if start < pd.to_datetime("1979-01-01T13"):
         raise InputRangeError("start_date", "1979-01-01 to yesterday")
     if end > pd.Timestamp.now() - pd.Timedelta("1D"):
         raise InputRangeError("end_date", "1979-01-01 to yesterday")
     if end <= start:
         raise InputRangeError("end_date", "after start_date")
 
     dates = pd.date_range(start, end, freq="10000D").tolist()
     dates = dates + [end] if dates[-1] < end else dates
 
+    if source == "grib":
+        source_tag = "NLDAS:NLDAS_FORA0125_H.002"
+        nldas_vars = NLDAS_VARS_GRIB
+    elif source == "netcdf":
+        source_tag = "NLDAS2:NLDAS_FORA0125_H_v2.0"
+        nldas_vars = NLDAS_VARS_NETCDF
+    else:
+        raise InputValueError("source", ["grib", "netcdf"])
+
     if variables is None:
-        clm_vars = [f"NLDAS:NLDAS_FORA0125_H.002:{d['nldas_name']}" for d in NLDAS_VARS.values()]
+        clm_vars = [f"{source_tag}:{d['nldas_name']}" for d in nldas_vars.values()]
     else:
         clm_vars = [variables] if isinstance(variables, str) else list(variables)
         clm_vars = clm_vars + ["temp"] if snow and "temp" not in clm_vars else clm_vars
-        if any(v not in NLDAS_VARS for v in clm_vars):
-            raise InputValueError("variables", list(NLDAS_VARS))
-        clm_vars = [f"NLDAS:NLDAS_FORA0125_H.002:{NLDAS_VARS[v]['nldas_name']}" for v in clm_vars]
+        if any(v not in nldas_vars for v in clm_vars):
+            raise InputValueError("variables", list(nldas_vars))
+        clm_vars = [f"{source_tag}:{nldas_vars[v]['nldas_name']}" for v in clm_vars]
 
-    return dates, clm_vars
+    return dates, clm_vars, nldas_vars
 
 
 def _byloc(
     lon: float,
     lat: float,
     start_date: str,
     end_date: str,
     variables: str | list[str] | None = None,
     n_conn: int = 4,
     snow: bool = False,
     snow_params: dict[str, float] | None = None,
+    source: str = "grib",
 ) -> pd.DataFrame:
     """Get NLDAS climate forcing data for a single location."""
-    dates, clm_vars = _check_inputs(start_date, end_date, variables, snow)
+    dates, clm_vars, nldas_vars = _check_inputs(start_date, end_date, variables, snow, source)
     kwds = [
         {
             "params": {
                 "type": "asc2",
                 "location": f"GEOM:POINT({lon}, {lat})",
                 "variable": v,
                 "startDate": s.strftime(DATE_FMT),
@@ -263,21 +321,22 @@
         }
         for (s, e), v in itertools.product(zip(dates[:-1], dates[1:]), clm_vars)
     ]
 
     n_conn = min(n_conn, 4)
     resp = ar.retrieve_text([URL] * len(kwds), kwds, max_workers=n_conn)
 
-    clm_list = (_txt2df(txt, i, kwds) for i, txt in enumerate(resp))
+    clm_list = (_txt2df(txt, i, kwds, source=source) for i, txt in enumerate(resp))
+
     clm_merged = (
         pd.concat(df)
         for _, df in itertools.groupby(sorted(clm_list, key=lambda x: x.name), lambda x: x.name)
     )
     clm = pd.concat(clm_merged, axis=1)
-    clm = clm.rename(columns={d["nldas_name"]: n for n, d in NLDAS_VARS.items()})
+    clm = clm.rename(columns={d["nldas_name"]: n for n, d in nldas_vars.items()})
 
     if snow:
         params = {"t_rain": T_RAIN, "t_snow": T_SNOW} if snow_params is None else snow_params
         clm = separate_snow(clm, **params)
     clm.index.name = "time"
     clm.index = pd.to_datetime(clm.index).tz_localize(None)
     return clm.loc[start_date:end_date]
@@ -309,14 +368,15 @@
     coords_id: Sequence[str | int] | None = None,
     crs: CRSTYPE = 4326,
     variables: str | list[str] | None = None,
     to_xarray: bool = False,
     n_conn: int = 4,
     snow: bool = False,
     snow_params: dict[str, float] | None = None,
+    source: str = "grib",
 ) -> pd.DataFrame | xr.Dataset:
     """Get NLDAS climate forcing data for a list of coordinates.
 
     Parameters
     ----------
     coords : list of tuples
         List of (lon, lat) coordinates.
@@ -325,15 +385,15 @@
     end_date : str
         End date of the data.
     crs : str, int, or pyproj.CRS, optional
         The CRS of the input coordinates, defaults to ``EPSG:4326``.
     variables : str or list of str, optional
         Variables to download. If None, all variables are downloaded.
         Valid variables are: ``prcp``, ``pet``, ``temp``, ``wind_u``, ``wind_v``,
-        ``rlds``, ``rsds``, and ``humidity``.
+        ``rlds``, ``rsds``, and ``humidity`` (and ``psurf`` if ``source=netcdf``)
     to_xarray : bool, optional
         If True, the data is returned as an xarray dataset.
     n_conn : int, optional
         Number of parallel connections to use for retrieving data, defaults to 4.
         The maximum number of connections is 4, if more than 4 are requested, 4
         connections will be used.
     snow : bool, optional
@@ -341,14 +401,16 @@
     snow_params : dict, optional
         Model-specific parameters as a dictionary that is passed to the snowfall function.
         These parameters are only used if ``snow`` is ``True``. Two parameters are required:
         ``t_rain`` (deg C) which is the threshold for temperature for considering rain and
         ``t_snow`` (deg C) which is the threshold for temperature for considering snow.
         The default values are ``{'t_rain': 2.5, 't_snow': 0.6}`` that are adopted from
         https://doi.org/10.5194/gmd-11-1077-2018.
+    source: str, optional
+        Source to pull data rods from. Valid sources are: ``grib`` and ``netcdf``
 
     Returns
     -------
     pandas.DataFrame
         The requested data as a dataframe.
     """
     lons, lats = _get_lon_lat(coords, crs)
@@ -364,23 +426,27 @@
         _byloc,
         variables=variables,
         start_date=start_date,
         end_date=end_date,
         n_conn=n_conn,
         snow=snow,
         snow_params=snow_params,
+        source=source,
     )
+
+    _, _, nldas_vars = _check_inputs(start_date, end_date, variables, snow, source)
+
     clm_list = itertools.starmap(nldas, zip(points.x, points.y))
     if to_xarray:
         clm_ds = xr.concat(
             (xr.Dataset.from_dataframe(clm) for clm in clm_list), dim=pd.Index(idx, name="id")
         )
         clm_ds.attrs["tz"] = "UTC"
         for v in clm_ds.data_vars:
-            clm_ds[v].attrs = NLDAS_VARS[str(v)]
+            clm_ds[v].attrs = nldas_vars[str(v)]
         return clm_ds
 
     if n_pts == 1:
         clm = next(iter(clm_list), pd.DataFrame())
     else:
         clm = cast("pd.DataFrame", pd.concat(clm_list, keys=idx, axis=1))
         clm.columns = clm.columns.set_names(["id", "variable"])
@@ -401,25 +467,32 @@
         (
             "https://ldas.gsfc.nasa.gov/sites/default",
             "files/ldas/nldas/NLDAS_masks-veg-soil.nc4",
         )
     )
     resp = ar.retrieve_binary([url])
     grid = xr.open_dataset(BytesIO(resp[0]), engine="h5netcdf")
-    grid = grid.rio.write_transform()
-    grid = grid.rio.write_crs(4326)
-    grid = grid.rio.write_coordinate_system()
+    grid = hgu.xd_write_crs(grid, 4326)
     return grid
 
 
-def _txt2da(txt: str, resp_id: int, kwds: list[dict[str, dict[str, str]]]) -> xr.DataArray:
+def _txt2da(
+    txt: str,
+    resp_id: int,
+    kwds: list[dict[str, dict[str, str]]],
+    source: str = "grib",
+) -> xr.DataArray:
     """Convert text to dataarray."""
     try:
-        data = pd.read_csv(StringIO(txt), skiprows=39, delim_whitespace=True).dropna()
-        data.index = pd.to_datetime(data.index + " " + data[DATE_COL])
+        if source == "grib":
+            data = pd.read_csv(StringIO(txt), skiprows=39, delim_whitespace=True).dropna()
+            data.index = pd.to_datetime(data.index + " " + data[DATE_COL], utc=True)
+        else:
+            data = pd.read_csv(StringIO(txt), skiprows=12, delim_whitespace=True).dropna()
+            data.index = pd.to_datetime(data[DATE_COL], utc=True)
     except EmptyDataError:
         return xr.DataArray(name=kwds[resp_id]["params"]["variable"].split(":")[-1])
     except UFuncTypeError as ex:
         msg = "".join(re.findall("<strong>(.*?)</strong>", txt, re.DOTALL)).strip()
         raise NLDASServiceError(msg) from ex
 
     data = data["Data"]
@@ -438,14 +511,15 @@
     start_date: str,
     end_date: str,
     geo_crs: CRSTYPE,
     variables: str | list[str] | None = None,
     n_conn: int = 4,
     snow: bool = False,
     snow_params: dict[str, float] | None = None,
+    source: str = "grib",
 ) -> xr.Dataset:
     """Get hourly NLDAS climate forcing within a geometry at 0.125 resolution.
 
     Parameters
     ----------
     geometry : shapely.Polygon, shapely.MultiPolygon, or tuple of length 4
         Input polygon or a bounding box like so (xmin, ymin, xmax, ymax).
@@ -454,34 +528,36 @@
     end_date : str
         End date of the data.
     geo_crs : int, str, or pyproj.CRS
         CRS of the input geometry
     variables : str or list of str, optional
         Variables to download. If None, all variables are downloaded.
         Valid variables are: ``prcp``, ``pet``, ``temp``, ``wind_u``, ``wind_v``,
-        ``rlds``, ``rsds``, and ``humidity``.
+        ``rlds``, ``rsds``, and ``humidity`` (and ``psurf`` if ``source=netcdf``)
     n_conn : int, optional
         Number of parallel connections to use for retrieving data, defaults to 4.
         It should be less than 4.
     snow : bool, optional
         Compute snowfall from precipitation and temperature. Defaults to ``False``.
     snow_params : dict, optional
         Model-specific parameters as a dictionary that is passed to the snowfall function.
         These parameters are only used if ``snow`` is ``True``. Two parameters are required:
         ``t_rain`` (deg C) which is the threshold for temperature for considering rain and
         ``t_snow`` (deg C) which is the threshold for temperature for considering snow.
         The default values are ``{'t_rain': 2.5, 't_snow': 0.6}`` that are adopted from
         https://doi.org/10.5194/gmd-11-1077-2018.
+    source: str, optional
+        Source to pull data rods from. Valid sources are: ``grib`` and ``netcdf``.
 
     Returns
     -------
     xarray.Dataset
         The requested forcing data.
     """
-    dates, clm_vars = _check_inputs(start_date, end_date, variables, snow)
+    dates, clm_vars, nldas_vars = _check_inputs(start_date, end_date, variables, snow, source)
 
     nldas_grid = get_grid_mask()
     geom = hgu.geo2polygon(geometry, geo_crs, nldas_grid.rio.crs)
     msk = nldas_grid.CONUS_mask.rio.clip([geom], all_touched=True)
     coords = itertools.product(msk.get_index("lon"), msk.get_index("lat"))
     kwds = [
         {
@@ -495,21 +571,21 @@
         }
         for (lon, lat), (s, e), v in itertools.product(coords, zip(dates[:-1], dates[1:]), clm_vars)
     ]
 
     n_conn = min(n_conn, 4)
     resp = ar.retrieve_text([URL] * len(kwds), kwds, max_workers=n_conn)
 
-    clm = xr.merge(_txt2da(txt, i, kwds) for i, txt in enumerate(resp))
-    clm = clm.rename({d["nldas_name"]: n for n, d in NLDAS_VARS.items() if d["nldas_name"] in clm})
+    clm = xr.merge(_txt2da(txt, i, kwds, source=source) for i, txt in enumerate(resp))
+    clm = clm.rename({d["nldas_name"]: n for n, d in nldas_vars.items() if d["nldas_name"] in clm})
     clm = clm.sel(time=slice(start_date, end_date))
     clm.attrs["tz"] = "UTC"
     clm = clm.transpose("time", "y", "x")
     for v in clm:
-        clm[v].attrs = NLDAS_VARS[str(v)]
+        clm[v].attrs = nldas_vars[str(v)]
     clm = hgu.xd_write_crs(clm, 4326)
     if snow:
         params = {"t_rain": T_RAIN, "t_snow": T_SNOW} if snow_params is None else snow_params
         clm = separate_snow(clm, **params)
     if isinstance(geometry, (list, tuple)):
         return clm
     clm = hgu.xarray_geomask(clm, geometry, geo_crs, all_touched=True)
```

### Comparing `pynldas2-0.14.0/pynldas2.egg-info/PKG-INFO` & `pynldas2-0.15.0/pynldas2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pynldas2
-Version: 0.14.0
+Version: 0.15.0
 Summary: Get NLDAS2 forcing data.
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/pynldas2/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pynldas2.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/pynldas2.html
 Project-URL: Issues, https://github.com/hyriver/pynldas2/issues
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
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
```

### Comparing `pynldas2-0.14.0/pynldas2.egg-info/SOURCES.txt` & `pynldas2-0.15.0/pynldas2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynldas2-0.14.0/pyproject.toml` & `pynldas2-0.15.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,36 +14,35 @@
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
   "Topic :: Scientific/Engineering :: Atmospheric Science",
   "Topic :: Scientific/Engineering :: GIS",
   "Topic :: Scientific/Engineering :: Hydrology",
-  "Typing :: Typed"
+  "Typing :: Typed",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "async-retriever>=0.14",
+  "async-retriever==0.15",
   "h5netcdf",
   "numpy>=1.21",
   "pandas>=1",
-  "pygeoutils>=0.14",
-  "pyproj>=2.2",
+  "pygeoutils==0.15",
+  "pyproj>=3.0.1",
   "rioxarray>=0.11",
   "xarray>=2022.03",
 ]
 [project.optional-dependencies]
 speedup = [
   "numba",
 ]
```

### Comparing `pynldas2-0.14.0/tests/test_exceptions.py` & `pynldas2-0.15.0/tests/test_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for exceptions and requests"""
 import pytest
-from shapely import Polygon
+from shapely.geometry import Polygon
 
 import pynldas2 as nldas
 from pynldas2 import InputRangeError, InputTypeError, InputValueError
 
 GEOM = Polygon(
     [[-69.77, 45.07], [-69.31, 45.07], [-69.31, 45.45], [-69.77, 45.45], [-69.77, 45.07]]
 )
```

### Comparing `pynldas2-0.14.0/tests/test_pynldas2.py` & `pynldas2-0.15.0/tests/test_pynldas2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,57 @@
 """Tests for the package PyNLDAS2."""
 import io
 import os
 
 import numpy as np
 import pytest
-from shapely import Point, Polygon
+from shapely.geometry import Point, Polygon
 
 import pynldas2 as nldas
 
 GEOM = Polygon(
     [[-69.77, 45.07], [-69.31, 45.07], [-69.31, 45.45], [-69.77, 45.45], [-69.77, 45.07]]
 )
 VAR = ["prcp", "pet"]
 DEF_CRS = 4326
 ALT_CRS = 3542
 COORDS = (-1431147.7928, 318483.4618)
 START = "2000-01-01"
 END = "2000-01-12"
+START_ALT = "2022-01-01"  # at the time of testing, the rods for source="netcdf" were
+END_ALT = "2022-01-31"  # unavailable except for the year 2022
 CONN = 1 if int(os.environ.get("GH_CI", 0)) else 4
+SOURCE_GRIB = "grib"
+SOURCE_NETCDF = "netcdf"
 
 
 def assert_close(a: float, b: float, rtol: float = 1e-2) -> bool:
     assert np.isclose(a, b, rtol=rtol).all()
 
 
 def test_coords():
     clm = nldas.get_bycoords(COORDS, START, END, crs=ALT_CRS, variables=VAR, n_conn=CONN)
     assert_close(clm.prcp.mean(), 0.0051)
     assert_close(clm.pet.mean(), 0.1346)
 
 
+def test_coords_explicit_source():
+    clm = nldas.get_bycoords(
+        COORDS, START, END, crs=ALT_CRS, source=SOURCE_GRIB, variables=VAR, n_conn=CONN
+    )
+    assert_close(clm.prcp.mean(), 0.0051)
+    assert_close(clm.pet.mean(), 0.1346)
+
+    clm = nldas.get_bycoords(
+        COORDS, START_ALT, END_ALT, crs=ALT_CRS, source=SOURCE_NETCDF, variables=VAR, n_conn=CONN
+    )
+    assert_close(clm.prcp.mean(), 0.0058)
+    assert_close(clm.pet.mean(), 0.1242)
+
+
 def test_coords_xr():
     clm = nldas.get_bycoords(
         COORDS, START, END, crs=ALT_CRS, variables="prcp", to_xarray=True, n_conn=CONN
     )
     assert_close(clm.prcp.mean(), 0.0051)
```

