# Comparing `tmp/pygeohydro-0.14.0.tar.gz` & `tmp/pygeohydro-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeohydro-0.14.0.tar", last modified: Sun Mar  5 16:52:36 2023, max compression
+gzip compressed data, was "pygeohydro-0.15.0.tar", last modified: Sun May  7 22:56:54 2023, max compression
```

## Comparing `pygeohydro-0.14.0.tar` & `pygeohydro-0.15.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:36.369676 pygeohydro-0.14.0/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:36.365676 pygeohydro-0.14.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:36.365676 pygeohydro-0.14.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:36.365676 pygeohydro-0.14.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    30709 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-03-05 16:52:36.369676 pygeohydro-0.14.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:36.361676 pygeohydro-0.14.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:36.365676 pygeohydro-0.14.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/ci/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:36.369676 pygeohydro-0.14.0/pygeohydro/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25292 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/nwis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44527 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/pygeohydro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/us_abbrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/waterdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pygeohydro/watershed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:36.369676 pygeohydro-0.14.0/pygeohydro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-03-05 16:52:36.000000 pygeohydro-0.14.0/pygeohydro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-05 16:52:36.000000 pygeohydro-0.14.0/pygeohydro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:52:36.000000 pygeohydro-0.14.0/pygeohydro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:52:35.000000 pygeohydro-0.14.0/pygeohydro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-05 16:52:36.000000 pygeohydro-0.14.0/pygeohydro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-05 16:52:36.000000 pygeohydro-0.14.0/pygeohydro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 16:52:36.369676 pygeohydro-0.14.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:52:36.369676 pygeohydro-0.14.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-03-05 16:52:19.000000 pygeohydro-0.14.0/tests/test_pygeohydro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:54.825149 pygeohydro-0.15.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:54.821149 pygeohydro-0.15.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:54.821149 pygeohydro-0.15.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:54.821149 pygeohydro-0.15.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    31988 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-05-07 22:56:54.825149 pygeohydro-0.15.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:54.817149 pygeohydro-0.15.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:54.821149 pygeohydro-0.15.0/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/ci/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:54.825149 pygeohydro-0.15.0/pygeohydro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/nwis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44591 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/pygeohydro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/us_abbrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/waterdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pygeohydro/watershed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:54.825149 pygeohydro-0.15.0/pygeohydro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-05-07 22:56:54.000000 pygeohydro-0.15.0/pygeohydro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-07 22:56:54.000000 pygeohydro-0.15.0/pygeohydro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 22:56:54.000000 pygeohydro-0.15.0/pygeohydro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 22:56:54.000000 pygeohydro-0.15.0/pygeohydro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-07 22:56:54.000000 pygeohydro-0.15.0/pygeohydro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 22:56:54.000000 pygeohydro-0.15.0/pygeohydro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 22:56:54.825149 pygeohydro-0.15.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:56:54.825149 pygeohydro-0.15.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-07 22:56:37.000000 pygeohydro-0.15.0/tests/test_pygeohydro.py
```

### Comparing `pygeohydro-0.14.0/.github/ISSUE_TEMPLATE/bugreport.yml` & `pygeohydro-0.15.0/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/.github/ISSUE_TEMPLATE/newfeature.yml` & `pygeohydro-0.15.0/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/.github/workflows/codeql-analysis.yml` & `pygeohydro-0.15.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/.github/workflows/release.yml` & `pygeohydro-0.15.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/.github/workflows/test.yml` & `pygeohydro-0.15.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/.gitignore` & `pygeohydro-0.15.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/.pre-commit-config.yaml` & `pygeohydro-0.15.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,8 @@
 repos:
-- repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
-  hooks:
-  - id: trailing-whitespace
-  - id: requirements-txt-fixer
-  - id: check-added-large-files
-    args: [--maxkb=50000]
-  - id: end-of-file-fixer
-  - id: check-merge-conflict
-  - id: check-toml
-  - id: check-yaml
-  - id: debug-statements
-  - id: mixed-line-ending
-    args: [--fix=lf]
-
-- repo: https://github.com/tox-dev/pyproject-fmt
-  rev: 0.9.2
-  hooks:
-  - id: pyproject-fmt
-    name: Apply a consistent format to pyproject.toml
-
-- repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.7.0
-  hooks:
-  - id: pretty-format-yaml
-    args: [--autofix, --indent, '2']
-
 - repo: https://github.com/hadialqattan/pycln
   rev: v2.1.3
   hooks:
   - id: pycln
     name: Find and remove unused import statements with pycln
     args: [--config=pyproject.toml]
 
@@ -41,94 +14,90 @@
 
 - repo: https://github.com/MarcoGorelli/absolufy-imports
   rev: v0.3.1
   hooks:
   - id: absolufy-imports
     name: Convert relative imports to absolute with absolufy-imports
 
-- repo: https://github.com/PyCQA/isort
-  rev: 5.12.0
-  hooks:
-  - id: isort
-    name: Sort imports with isort
-
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
 
-- repo: https://github.com/guilatrova/tryceratops
-  rev: v1.1.0
-  hooks:
-  - id: tryceratops
-    name: Check try-exceptions blocks with tryceratops
-
-- repo: https://github.com/pre-commit/pygrep-hooks
-  rev: v1.10.0
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  rev: v0.0.265
   hooks:
-  - id: rst-backticks
-    name: Check backsticks in rst files
-  - id: rst-directive-colons
-    name: Check directives in rst files
+  - id: ruff
+    name: Linting with Ruff
+    args: [--fix, --exit-non-zero-on-fix]
 
 - repo: https://github.com/PyCQA/doc8
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
 
-- repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
-  hooks:
-  - id: pyupgrade
-    name: Upgrade sytnax to python 3.8+ with pyupgrade
-    args: [--py38-plus]
-
-- repo: https://github.com/PyCQA/flake8
-  rev: 6.0.0
-  hooks:
-  - id: flake8
-    name: Linting with flake8
-    additional_dependencies:
-    - flake8-comprehensions
-    - flake8-builtins
-    - flake8-blind-except
-    - flake8-bugbear
-    - flake8-use-fstring
-    - flake8-docstrings
-    - flake8-type-checking
-    - flake8-simplify
-    - pep8-naming
-
 - repo: https://github.com/dosisod/refurb
-  rev: v1.13.0
+  rev: v1.16.0
   hooks:
   - id: refurb
     name: Modernizing Python codebases using Refurb
     additional_dependencies:
     - numpy
 
-- repo: https://github.com/PyCQA/bandit
-  rev: 1.7.4
+- repo: https://github.com/tox-dev/pyproject-fmt
+  rev: 0.11.1
+  hooks:
+  - id: pyproject-fmt
+    name: Apply a consistent format to pyproject.toml
+
+- repo: https://github.com/pre-commit/pre-commit-hooks
+  rev: v4.4.0
   hooks:
-  - id: bandit
-    name: Check for security issues with bandit
-    args: [-lll]
-    files: .py$
+  - id: check-added-large-files
+    args: [--maxkb=50000]
+  - id: mixed-line-ending
+    args: [--fix=lf]
+  - id: check-ast
+  - id: check-builtin-literals
+  - id: check-case-conflict
+  - id: check-docstring-first
+  - id: check-shebang-scripts-are-executable
+  - id: check-merge-conflict
+  - id: check-json
+  - id: check-toml
+  - id: check-xml
+  - id: check-yaml
+  - id: debug-statements
+  - id: destroyed-symlinks
+  - id: detect-private-key
+  - id: end-of-file-fixer
+    exclude: ^LICENSE|\.(html|csv|txt|svg|py)$
+  - id: pretty-format-json
+    args: [--autofix, --no-ensure-ascii, --no-sort-keys]
+  - id: trailing-whitespace
+    args: [--markdown-linebreak-ext=md]
+    exclude: \.(html|svg)$
+
+- repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
+  rev: v2.8.0
+  hooks:
+  - id: pretty-format-yaml
+    args: [--autofix, --indent, '2']
```

### Comparing `pygeohydro-0.14.0/CITATION.cff` & `pygeohydro-0.15.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/CODE_OF_CONDUCT.rst` & `pygeohydro-0.15.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/CONTRIBUTING.rst` & `pygeohydro-0.15.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/HISTORY.rst` & `pygeohydro-0.15.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,39 @@
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
+- Add a new option to ``NWIS.get_info``, called ``nhd_info``, for
+  retrieving NHDPlus related info on the sites. This will two new
+  service calls that might slow down the function, so it's disabled
+  by default.
+- Update links in ``NID`` to the latest CSV and GPKG versions of
+  the NID dataset.
+- Add two new properties to ``NID`` to access the entire NID dataset.
+  You can use ``NID.df`` to access the CSV version as a
+  ``pandas.DataFrame`` and ``NID.gdf`` to access the GPKG version
+  as a ``geopandas.GeoDataFrame``. Installing ``pyogrio`` is highly
+  recommended for much faster reading of the GPKG version.
+- Refactor ``NID.bygeom`` to use the new ``NID.gdf`` property for
+  spatial querying of the dataset. This change should make the query
+  much faster.
+- For now, retain compatibility with ``shapely<2`` while supporting
+  ``shapley>=2``.
+
 0.14.0 (2023-03-05)
 -------------------
 
 New Features
 ~~~~~~~~~~~~
 - Add a new function, called ``nlcd_area_percent``, for computing the
   percentages or natural, developed, and impervious areas within geometries
```

### Comparing `pygeohydro-0.14.0/LICENSE` & `pygeohydro-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/PKG-INFO` & `pygeohydro-0.15.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pygeohydro
-Version: 0.14.0
+Version: 0.15.0
 Summary: Access geospatial web services that offer hydrological data
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/pygeohydro/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pygeohydro.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/pygeohydro.html
 Project-URL: Issues, https://github.com/hyriver/pygeohydro/issues
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

### Comparing `pygeohydro-0.14.0/README.rst` & `pygeohydro-0.15.0/README.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/ci/requirements/environment-dev.yml` & `pygeohydro-0.15.0/ci/requirements/environment-dev.yml`

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

### Comparing `pygeohydro-0.14.0/ci/requirements/environment.yml` & `pygeohydro-0.15.0/ci/requirements/environment.yml`

 * *Files 1% similar despite different names*

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

### Comparing `pygeohydro-0.14.0/noxfile.py` & `pygeohydro-0.15.0/noxfile.py`

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
+        deps += list(version_limit)
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

### Comparing `pygeohydro-0.14.0/pygeohydro/__init__.py` & `pygeohydro-0.15.0/pygeohydro/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/pygeohydro/exceptions.py` & `pygeohydro-0.15.0/pygeohydro/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Parameters
     ----------
     missing : list
         List of missing columns.
     """
 
     def __init__(self, missing: list[str]) -> None:
-        self.message = "The following columns are missing:\n" + f"{', '.join(missing)}"
+        self.message = f"The following columns are missing:\n{', '.join(missing)}"
         super().__init__(self.message)
 
     def __str__(self) -> str:
         return self.message
 
 
 class MissingCRSError(Exception):
```

### Comparing `pygeohydro-0.14.0/pygeohydro/helpers.py` & `pygeohydro-0.15.0/pygeohydro/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Some helper function for PyGeoHydro."""
 from __future__ import annotations
 
 import io
 from typing import Any, NamedTuple
 
-import async_retriever as ar
 import cytoolz.curried as tlz
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import ujson as json
 from defusedxml import ElementTree
-from pygeoogc import ServiceURL
 
+import async_retriever as ar
 from pygeohydro import us_abbrs
 from pygeohydro.exceptions import InputRangeError, InputTypeError, InputValueError
+from pygeoogc import ServiceURL
 
 __all__ = ["nlcd_helper", "nwis_errors", "states_lookup_table", "get_us_states"]
 
 
 def nlcd_helper() -> dict[str, Any]:
     """Get legends and properties of the NLCD cover dataset.
 
@@ -207,14 +207,16 @@
     if subset_key is not None:
         state_cd = _get_state_codes(subset_key)
         return us_states[us_states.STUSPS.isin(state_cd)].copy()
     return us_states
 
 
 class StateCounties(NamedTuple):
+    """State and county codes and names."""
+
     name: str
     code: str | None
     counties: pd.Series
 
 
 def states_lookup_table() -> dict[str, StateCounties]:
     """Get codes and names of US states and their counties.
```

### Comparing `pygeohydro-0.14.0/pygeohydro/nwis.py` & `pygeohydro-0.15.0/pygeohydro/nwis.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 """Accessing NWIS."""
 from __future__ import annotations
 
 import contextlib
-import io
 import itertools
 import re
 import warnings
-from typing import TYPE_CHECKING, Any, Iterable, Literal, Sequence, TypeVar, cast, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Iterable,
+    Literal,
+    Sequence,
+    TypeVar,
+    cast,
+    overload,
+)
 
-import async_retriever as ar
 import cytoolz.curried as tlz
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import xarray as xr
-from pygeoogc import ServiceURL
-from pygeoogc import utils as ogc_utils
 
+import async_retriever as ar
+import pynhd
 from pygeohydro.exceptions import (
     DataNotAvailableError,
     InputTypeError,
     InputValueError,
     ZeroMatchedError,
 )
+from pygeoogc import ServiceURL
+from pygeoogc import utils as ogc_utils
+from pynhd import NLDI
 
 try:
     from pandas.errors import IntCastingNaNError
 except ImportError:
-    IntCastingNaNError = TypeError
+    IntCastingNaNError = ValueError
 
 T_FMT = "%Y-%m-%d"
 __all__ = ["NWIS", "streamflow_fillna"]
 
 if TYPE_CHECKING:
     ArrayLike = TypeVar("ArrayLike", pd.Series, pd.DataFrame, xr.DataArray)
 
@@ -42,15 +52,15 @@
     It drops stations with more than ``missing_max`` days missing data
     per year. Missing data in the remaining stations, are filled with
     day-of-year average over the entire dataset.
 
     Parameters
     ----------
     discharge : xarray.DataArray or pandas.DataFrame or pandas.Series
-        Streamflow observations with at least 10 years of daily data.
+        Daily streamflow observations with at least 10 years of daily data.
     missing_max : int
         Maximum allowed number of missing daily data per year for filling,
         defaults to 5.
 
     Returns
     -------
     xarray.DataArray or pandas.DataFrame or pandas.Series
@@ -66,16 +76,16 @@
 
     if isinstance(df, pd.Series):
         df = df.to_frame(df.name or "0" * 8)
 
     df = cast("pd.DataFrame", df)
     df.columns = df.columns.astype(str)
     df.index = pd.DatetimeIndex(pd.to_datetime(df.index).date)
-    if pd.infer_freq(df.index) != "D" and df.index.year.unique().size >= 10:
-        raise InputTypeError("streamflow", "array with at least 10 years of data")
+    if df.index.year.unique().size < 10:
+        raise InputTypeError("streamflow", "array with at least 10 years of daily data")
 
     df[df < 0] = np.nan
     s_nan = pd.DataFrame.from_dict(
         {yr: q.isna().sum() for yr, q in df.resample("Y")}, orient="index"
     )
     if np.all(s_nan == 0):
         return streamflow
@@ -94,15 +104,15 @@
 
     if isinstance(streamflow, pd.Series):
         return df.squeeze()
 
     if isinstance(streamflow, pd.DataFrame):
         return df
 
-    return xr.DataArray(  # type: ignore
+    return xr.DataArray(  # pyright: ignore[reportGeneralTypeIssues]
         df,
         coords={
             "time": df.index.to_numpy("datetime64[ns]"),
             "station_id": s_fill,
         },
         name=streamflow.name or "discharge",
     )
@@ -147,24 +157,25 @@
         except ar.ServiceError as ex:
             raise ZeroMatchedError(ogc_utils.check_response(str(ex))) from ex
 
         with contextlib.suppress(StopIteration):
             not_found = next(filter(lambda x: x[0] != "#", resp), None)
             if not_found is not None:
                 msg = re.findall("<p>(.*?)</p>", not_found)[1].rsplit(">", 1)[1]
-                raise ZeroMatchedError(f"Server error message:\n{msg}")
+                msg = f"Server error message:\n{msg}"
+                raise ZeroMatchedError(msg)
 
         data = [r.strip().split("\n") for r in resp if r[0] == "#"]
         data = [t.split("\t") for d in data for t in d if "#" not in t]
         if not data:
             raise ZeroMatchedError
 
         rdb_df = pd.DataFrame.from_dict(dict(zip(data[0], d)) for d in data[2:])
         if "agency_cd" in rdb_df:
-            rdb_df = rdb_df[~rdb_df.agency_cd.str.contains("agency_cd|5s")].copy()
+            rdb_df = rdb_df[~rdb_df["agency_cd"].str.contains("agency_cd|5s")].copy()
         return rdb_df
 
     @staticmethod
     def _validate_usgs_queries(
         queries: list[dict[str, str]], expanded: bool = False
     ) -> list[dict[str, str]]:
         """Validate queries to be used with USGS Site Web Service.
@@ -251,45 +262,78 @@
             "holdDepthMinVa",
             "holeDepthMax",
             "holeDepthMaxVa",
         ]
 
         not_valid = list(tlz.concat(set(q).difference(set(valid_query_keys)) for q in queries))
         if not_valid:
-            raise InputValueError(f"query keys ({', '.join(not_valid)})", valid_query_keys)
+            invalid_keys = f"query keys ({', '.join(not_valid)})"
+            raise InputValueError(invalid_keys, valid_query_keys)
 
         _queries = queries.copy()
         if expanded:
             _ = [
                 q.pop(k) for k in ("outputDataTypeCd", "outputDataType") for q in _queries if k in q
             ]
             output_type = {"siteOutput": "expanded"}
         else:
             output_type = {"siteOutput": "basic"}
 
         return [{**query, **output_type, "format": "rdb"} for query in _queries]
 
+    @staticmethod
+    def _nhd_info(site_ids: list[str]) -> pd.DataFrame:
+        """Get drainage area of the stations from NHDPlus."""
+        site_list = [f"USGS-{s}" for s in site_ids]
+        area = NLDI().getfeature_byid("nwissite", site_list)
+        try:
+            area["comid"] = area["comid"].astype("int32")
+        except (TypeError, IntCastingNaNError):
+            area["comid"] = area["comid"].astype("Int32")
+        nhd_area = pynhd.streamcat("fert", comids=area["comid"].to_list())
+        area = area.merge(nhd_area[["COMID", "WSAREASQKM"]], left_on="comid", right_on="COMID")
+        area["identifier"] = area["identifier"].str.replace("USGS-", "")
+        area = area[["identifier", "comid", "reachcode", "measure", "WSAREASQKM"]].copy()
+        area = area.rename(
+            columns={
+                "identifier": "site_no",
+                "comid": "nhd_id",
+                "reachcode": "nhd_reachcode",
+                "measure": "nhd_measure",
+                "WSAREASQKM": "nhd_areasqkm",
+            }
+        )
+        return area
+
     def get_info(
         self,
         queries: dict[str, str] | list[dict[str, str]],
         expanded: bool = False,
         fix_names: bool = True,
+        nhd_info: bool = False,
     ) -> gpd.GeoDataFrame:
         """Send multiple queries to USGS Site Web Service.
 
         Parameters
         ----------
         queries : dict or list of dict
             A single or a list of valid queries.
         expanded : bool, optional
             Whether to get expanded site information for example drainage area,
             default to False.
         fix_names : bool, optional
             If ``True``, reformat station names and some small annoyances,
             defaults to ``True``.
+        nhd_info : bool, optional
+            If ``True``, get NHD information for each site, defaults to ``False``.
+            This will add four new columns: ``nhd_comid``, ``nhd_areasqkm``,
+            ``nhd_reachcode``, and ``nhd_measure``. Where ``nhd_id`` is the NHD
+            COMID of the flowline that the site is located in, ``nhd_reachcode``
+            is the NHD Reach Code that the site is located in, and ``nhd_measure``
+            is the measure along the flowline that the site is located at.
 
         Returns
         -------
         geopandas.GeoDataFrame
             A correctly typed ``GeoDataFrame`` containing site(s) information.
         """
         queries = [queries] if isinstance(queries, dict) else queries
@@ -325,45 +369,28 @@
             sites = sites.filter(regex="^(?!.*_overlap)")
             numeric_cols += ["drain_area_va", "contrib_drain_area_va"]
 
         with contextlib.suppress(KeyError):
             sites["begin_date"] = pd.to_datetime(sites["begin_date"])
             sites["end_date"] = pd.to_datetime(sites["end_date"])
 
+        if nhd_info:
+            nhd = self._nhd_info(sites["site_no"].to_list())
+            sites = pd.merge(sites, nhd, left_on="site_no", right_on="site_no", how="left")
+
         urls = [
             "/".join(
                 (
                     "https://gist.githubusercontent.com/cheginit",
                     "2dbc4b9c096f19089dbadb522821e8f3/raw/hcdn_2009_station_ids.txt",
                 )
-            ),
-            "/".join(
-                (
-                    "https://gist.githubusercontent.com/cheginit",
-                    "03129c5a0fb57272792aa4165b06fc19/raw/conus_station_ids.csv",
-                )
-            ),
+            )
         ]
         resp = ar.retrieve_text(urls)
-        nhd = pd.read_csv(
-            io.StringIO(resp[1]), dtype={"site_no": str, "nhd_id": int, "nhd_areasqkm": float}
-        )
-
-        sites = pd.merge(
-            sites,
-            nhd,
-            left_on="site_no",
-            right_on="site_no",
-            how="left",
-        )
         sites["hcdn_2009"] = sites["site_no"].isin(resp[0].split(","))
-        try:
-            sites["nhd_id"] = sites["nhd_id"].astype("int32")
-        except (ValueError, TypeError, IntCastingNaNError):
-            sites["nhd_id"] = sites["nhd_id"].astype("Int32")
 
         if "count_nu" in sites:
             numeric_cols.append("count_nu")
         sites[numeric_cols] = sites[numeric_cols].apply(pd.to_numeric, errors="coerce")
 
         return gpd.GeoDataFrame(
             sites,
@@ -449,16 +476,16 @@
                 {
                     "begin_date": "availability begin date",
                     "end_date": "availability end date",
                 }
             )
         attr_df = siteinfo[cols.keys()].groupby("site_no").first()
         if "begin_date" in attr_df and "end_date" in attr_df:
-            attr_df["begin_date"] = attr_df.begin_date.dt.strftime(T_FMT)
-            attr_df["end_date"] = attr_df.end_date.dt.strftime(T_FMT)
+            attr_df["begin_date"] = attr_df["begin_date"].dt.strftime(T_FMT)
+            attr_df["end_date"] = attr_df["end_date"].dt.strftime(T_FMT)
         attr_df.index = "USGS-" + attr_df.index
         attr_df["units"] = "mm/day" if mmd else "cms"
         attr_df["tz"] = "UTC"
         _ = cols.pop("site_no")
         return attr_df.to_dict(orient="index"), cols
 
     @staticmethod
@@ -482,15 +509,19 @@
 
         start = pd.to_datetime(dates[0], utc=utc)
         end = pd.to_datetime(dates[1], utc=utc)
         return sids_df.to_list(), start, end
 
     def _drainage_area_sqm(self, siteinfo: pd.DataFrame, freq: str) -> pd.Series:
         """Get drainage area of the stations."""
-        area = siteinfo[["site_no", "nhd_areasqkm"]].copy()
+        if "nhd_areasqkm" not in siteinfo:
+            area = self._nhd_info(siteinfo["site_no"].to_list())
+            area = area[["site_no", "nhd_areasqkm"]].copy()
+        else:
+            area = siteinfo[["site_no", "nhd_areasqkm"]].copy()
         if area["nhd_areasqkm"].isna().any():
             sids = area[area["nhd_areasqkm"].isna()].site_no
             queries = [
                 {
                     "parameterCd": "00060",
                     "siteStatus": "all",
                     "outputDataTypeCd": freq,
@@ -690,16 +721,18 @@
         end_dt = end.strftime(time_fmt)
         qobs = self._get_streamflow(sids, start_dt, end_dt, freq, params)
 
         n_orig = len(sids)
         sids = [s.split("-")[1] for s in qobs]
         if len(sids) != n_orig:
             warnings.warn(
-                f"Dropped {n_orig - len(sids)} stations since they don't have discharge data"
-                + f" from {start_dt} to {end_dt}.",
+                (
+                    f"Dropped {n_orig - len(sids)} stations since they don't have discharge data"
+                    f" from {start_dt} to {end_dt}."
+                ),
                 UserWarning,
                 stacklevel=2,
             )
         siteinfo = siteinfo[siteinfo.site_no.isin(sids)]
         if mmd:
             area_sqm = self._drainage_area_sqm(siteinfo, freq)
             ms2mmd = 1000.0 * 24.0 * 3600.0
```

### Comparing `pygeohydro-0.14.0/pygeohydro/plot.py` & `pygeohydro-0.15.0/pygeohydro/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from __future__ import annotations
 
 import contextlib
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, NamedTuple, TypeVar, Union
 
 import folium
-import hydrosignatures as hs
 import matplotlib.pyplot as plt
 import pandas as pd
 import pyproj
 from matplotlib.colors import BoundaryNorm, ListedColormap
-from pygeoogc import utils as ogc_utils
 
+import hydrosignatures as hs
 from pygeohydro import helpers
 from pygeohydro.exceptions import InputTypeError
 from pygeohydro.nwis import NWIS
+from pygeoogc import utils as ogc_utils
 
 if TYPE_CHECKING:
     DF = TypeVar("DF", pd.DataFrame, pd.Series)
     CRSTYPE = Union[int, str, pyproj.CRS]
 
 __all__ = ["signatures", "prepare_plot_data"]
 
@@ -269,15 +269,15 @@
     """
     nwis = NWIS()
     bbox = ogc_utils.match_crs(bbox, crs, 4326)
     query = {"bBox": ",".join(f"{b:.06f}" for b in bbox)}
     if isinstance(nwis_kwds, dict):
         query.update(nwis_kwds)
 
-    sites = nwis.get_info(query, expanded=True)
+    sites = nwis.get_info(query, expanded=True, nhd_info=True)
 
     sites["coords"] = list(sites[["dec_long_va", "dec_lat_va"]].itertuples(name=None, index=False))
     sites["altitude"] = (
         sites["alt_va"].astype("str") + " ft above " + sites["alt_datum_cd"].astype("str")
     )
 
     sites["drain_area_va"] = sites["drain_area_va"].astype("str") + " sqmi"
```

### Comparing `pygeohydro-0.14.0/pygeohydro/print_versions.py` & `pygeohydro-0.15.0/pygeohydro/print_versions.py`

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

### Comparing `pygeohydro-0.14.0/pygeohydro/pygeohydro.py` & `pygeohydro-0.15.0/pygeohydro/pygeohydro.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 """Accessing data from the supported databases through their APIs."""
 from __future__ import annotations
 
+import importlib.util
 import io
 import itertools
 import warnings
 import zipfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Mapping, Sequence, Tuple, Union, cast
 from unittest.mock import patch
 
-import async_retriever as ar
 import cytoolz.curried as tlz
 import dask.config
 import geopandas as gpd
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
-import pygeoogc as ogc
-import pygeoutils as geoutils
 import pyproj
 import rasterio as rio
 import xarray as xr
-from pygeoogc import WMS, ArcGISRESTful, RetrySession, ServiceURL
-from pygeoogc import utils as ogc_utils
-from pynhd.core import ScienceBase
 from rioxarray import _io as rxr
 
+import async_retriever as ar
+import pygeoogc as ogc
+import pygeoutils as geoutils
 from pygeohydro import helpers
 from pygeohydro.exceptions import (
     DependencyError,
     InputTypeError,
     InputValueError,
     MissingColumnError,
     MissingCRSError,
     ServiceUnavailableError,
     ZeroMatchedError,
 )
 from pygeohydro.helpers import Stats
+from pygeoogc import WMS, RetrySession, ServiceURL
+from pygeoogc import utils as ogc_utils
+from pynhd.core import ScienceBase
 
 if TYPE_CHECKING:
     from numbers import Number
     from ssl import SSLContext
 
-    from shapely import MultiPolygon, Polygon
+    from shapely.geometry import MultiPolygon, Polygon
 
     GTYPE = Union[Polygon, MultiPolygon, Tuple[float, float, float, float]]
     CRSTYPE = Union[int, str, pyproj.CRS]
 
 __all__ = [
     "get_camels",
     "ssebopeta_bycoords",
@@ -145,15 +147,15 @@
     co_list = list(zip(_coords.x, _coords.y))
 
     f_list = helpers.get_ssebopeta_urls(dates)
     session = RetrySession()
 
     with patch("socket.has_ipv6", False):
 
-        def _ssebop(url: str) -> list[np.ndarray]:  # type: ignore
+        def _ssebop(url: str) -> list[npt.NDArray[np.float64]]:
             r = session.get(url)
             z = zipfile.ZipFile(io.BytesIO(r.content))
 
             with rio.MemoryFile() as memfile:
                 memfile.write(z.read(z.filelist[0].filename))
                 with memfile.open() as src:
                     return list(src.sample(co_list))
@@ -466,15 +468,15 @@
     points_proj = points.to_crs(nlcd_wms.crs)
     geoms = points_proj.buffer(50, cap_style=3)
     ds_list = [nlcd_wms.get_map(g, 30) for g in geoms]
 
     def get_value(da: xr.DataArray, x: float, y: float) -> Number:
         nodata = da.attrs["nodatavals"][0]
         value = da.fillna(nodata).interp(x=[x], y=[y], method="nearest")
-        return da.dtype.type(value)[0, 0]  # type: ignore
+        return da.dtype.type(value)[0, 0]
 
     values = {
         v: [get_value(ds[v], p.x, p.y) for ds, p in zip(ds_list, points_proj)] for v in ds_list[0]
     }
     return points.to_frame("geometry").merge(
         pd.DataFrame(values), left_index=True, right_index=True
     )
@@ -528,15 +530,15 @@
     zero_idx = np.argwhere(val == 127)
     val = np.delete(val, zero_idx).astype(str)
     freq = np.delete(freq, zero_idx)
     freq_dict = dict(zip(val, freq))
     total_count = freq.sum()
 
     if any(c not in nlcd_meta["classes"] for c in freq_dict):
-        raise InputValueError("ds values", list(nlcd_meta["classes"]))  # noqa: TC003
+        raise InputValueError("ds", list(nlcd_meta["classes"]))
 
     class_percentage = {
         nlcd_meta["classes"][k].split(" -")[0].strip(): v / total_count * 100.0
         for k, v in freq_dict.items()
     }
     category_percentage = {
         k: sum(freq_dict[c] for c in v if c in freq_dict) / total_count * 100.0
@@ -638,15 +640,15 @@
 
     def __init__(self) -> None:
         self.base_url = ServiceURL().restful.nid
         self.suggest_url = f"{self.base_url}/suggestions"
         resp = ar.retrieve_json([f"{self.base_url}/advanced-fields"])
         resp = cast("list[dict[str, Any]]", resp)
         self.fields_meta = pd.DataFrame(resp[0])
-        self.valid_fields = self.fields_meta.name
+        self.valid_fields = self.fields_meta["name"]
         self.dam_type = {
             pd.NA: "N/A",
             None: "N/A",
             1: "Arch",
             2: "Multi-Arch",
             3: "Stone",
             4: "Roller-Compacted Concrete",
@@ -691,15 +693,25 @@
             "maxStorage": "acre-ft",
             "normalStorage": "acre-ft",
             "surfaceArea": "acre",
             "drainageArea": "square miles",
             "maxDischarge": "cfs",
             "spillwayWidth": "ft",
         }
-        self.nid_inventory_path = Path("cache", "nid_inventory.feather")
+        self._nid_inventory_path = Path("cache", "nid_inventory.feather")
+
+    @property
+    def nid_inventory_path(self) -> Path:
+        """Path to the NID inventory feather file."""
+        return self._nid_inventory_path
+
+    @nid_inventory_path.setter
+    def nid_inventory_path(self, value: Path | str) -> None:
+        self._nid_inventory_path = Path(value)
+        self._nid_inventory_path.parent.mkdir(parents=True, exist_ok=True)
 
     def stage_nid_inventory(self, fname: str | Path | None = None) -> None:
         """Download the entire NID inventory data and save to a feather file.
 
         Parameters
         ----------
         fname : str, pathlib.Path, optional
@@ -708,43 +720,43 @@
         """
         fname = self.nid_inventory_path if fname is None else Path(fname)
         if fname.suffix != ".feather":
             fname = fname.with_suffix(".feather")
 
         self.nid_inventory_path = fname
         if not self.nid_inventory_path.exists():
-            url = "/".join(
-                [
-                    "https://usace-cwbi-prod-il2-nld2-docs.s3-us-gov-west-1.amazonaws.com",
-                    "national-export/dams/nation/7783878c-6db4-46aa-99ef-8c283109ea78/nation.gpkg",
-                ]
-            )
+            url = "https://nid.sec.usace.army.mil/api/nation/gpkg"
             _ = ogc.streaming_download(url, fnames=fname.with_suffix(".gpkg"))
-            dams = gpd.read_file(fname.with_suffix(".gpkg"))
+            dams = (
+                gpd.read_file(fname.with_suffix(".gpkg"), engine="pyogrio", use_arrow=True)
+                if importlib.util.find_spec("pyogrio")
+                else gpd.read_file(fname.with_suffix(".gpkg"))
+            )
+
             dams = dams.astype(
                 {
                     "name": str,
                     "otherNames": str,
                     "formerNames": str,
                     "nidId": str,
                     "otherStructureId": str,
                     "federalId": str,
                     "ownerNames": str,
                     "ownerTypeIds": str,
-                    "primaryOwnerTypeId": "Int8",
+                    "primaryOwnerTypeId": str,
                     "stateFedId": str,
-                    "separateStructuresCount": "Int8",
+                    "separateStructuresCount": str,
                     "designerNames": str,
-                    "nonFederalDamOnFederalId": "Int8",
-                    "stateRegulatedId": "int8",
-                    "jurisdictionAuthorityId": "Int8",
+                    "nonFederalDamOnFederalId": str,
+                    "stateRegulatedId": str,
+                    "jurisdictionAuthorityId": str,
                     "stateRegulatoryAgency": str,
-                    "permittingAuthorityId": "Int8",
-                    "inspectionAuthorityId": "Int8",
-                    "enforcementAuthorityId": "Int8",
+                    "permittingAuthorityId": str,
+                    "inspectionAuthorityId": str,
+                    "enforcementAuthorityId": str,
                     "sourceAgency": str,
                     "latitude": "f8",
                     "longitude": "f8",
                     "county": str,
                     "state": str,
                     "city": str,
                     "distance": "f8",
@@ -756,70 +768,92 @@
                     "fedFundingIds": str,
                     "fedDesignIds": str,
                     "fedConstructionIds": str,
                     "fedRegulatoryIds": str,
                     "fedInspectionIds": str,
                     "fedOperationIds": str,
                     "fedOtherIds": str,
-                    "primaryPurposeId": "Int8",
+                    "primaryPurposeId": str,
                     "purposeIds": str,
-                    "primaryDamTypeId": "Int8",
+                    "primaryDamTypeId": str,
                     "damTypeIds": str,
                     "coreTypeIds": str,
                     "foundationTypeIds": str,
                     "damHeight": "f8",
                     "hydraulicHeight": "f8",
                     "structuralHeight": "f8",
                     "nidHeight": "f8",
-                    "nidHeightId": "f8",
+                    "nidHeightId": str,
                     "damLength": "f8",
                     "volume": "f8",
                     "yearCompleted": "Int32",
-                    "yearCompletedId": "Int8",
+                    "yearCompletedId": str,
                     "nidStorage": "f8",
                     "maxStorage": "f8",
                     "normalStorage": "f8",
                     "surfaceArea": "f8",
                     "drainageArea": "f8",
                     "maxDischarge": "f8",
-                    "spillwayTypeId": "Int8",
+                    "spillwayTypeId": str,
                     "spillwayWidth": "f8",
                     "numberOfLocks": "Int32",
                     "lengthOfLocks": "f8",
                     "widthOfLocks": "f8",
                     "yearsModified": str,
                     "outletGateTypes": str,
-                    "dataUpdated": "int64",
+                    "dataUpdated": "datetime64[ns]",
                     "inspectionDate": str,
                     "inspectionFrequency": "f4",
-                    "hazardId": "Int8",
-                    "conditionAssessId": "Int8",
-                    "conditionAssessDate": "int64",
-                    "eapId": "Int8",
-                    "eapLastRevDate": "int64",
+                    "hazardId": str,
+                    "conditionAssessId": str,
+                    "conditionAssessDate": "datetime64[ns]",
+                    "eapId": str,
+                    "eapLastRevDate": "datetime64[ns]",
                     "websiteUrl": str,
-                    "privateDamId": "Int8",
-                    "politicalPartyId": "Int8",
+                    "privateDamId": str,
+                    "politicalPartyId": str,
                     "id": "int32",
                     "systemId": "int32",
                     "huc2": str,
                     "huc4": str,
                     "huc6": str,
                     "huc8": str,
                     "zipcode": str,
                     "nation": str,
                     "stateKey": str,
                     "femaRegion": str,
                     "femaCommunity": str,
                 }
             )
-            dams.loc[dams.yearCompleted < 1000, "yearCompleted"] = pd.NA
+            for c in dams:
+                if (dams[c] == "Yes").any():
+                    dams[c] = dams[c] == "Yes"
+            dams.loc[dams["yearCompleted"] < 1000, "yearCompleted"] = pd.NA
             dams.to_feather(fname)
             fname.with_suffix(".gpkg").unlink()
 
+    @property
+    def df(self):
+        """Entire NID inventory (``csv`` version) as a ``pandas.DataFrame``."""
+        fname = self.nid_inventory_path
+        par_name = fname.with_suffix(".parquert")
+        if par_name.exists():
+            return pd.read_parquet(par_name)
+        url = "https://nid.sec.usace.army.mil/api/nation/csv"
+        _ = ogc.streaming_download(url, fnames=fname.with_suffix(".csv"))
+        dams = pd.read_csv(fname.with_suffix(".csv"), header=1, engine="pyarrow")
+        dams.to_parquet(par_name)
+        return dams
+
+    @property
+    def gdf(self):
+        """Entire NID inventory (``gpkg`` version) as a ``geopandas.GeoDataFrame``."""
+        self.stage_nid_inventory()
+        return gpd.read_feather(self.nid_inventory_path)
+
     @staticmethod
     def _get_json(
         urls: Sequence[str], params: list[dict[str, str]] | None = None
     ) -> list[dict[str, Any]]:
         """Get JSON response from NID web service.
 
         Parameters
@@ -833,18 +867,15 @@
         -------
         list of dict
             List of JSON responses from the web service.
         """
         if not isinstance(urls, list):
             raise InputTypeError("urls", "list or str")
 
-        if params is None:
-            kwds = None
-        else:
-            kwds = [{"params": {**p, "out": "json"}} for p in params]
+        kwds = None if params is None else [{"params": {**p, "out": "json"}} for p in params]
         resp = ar.retrieve_json(urls, kwds)
         resp = cast("list[dict[str, Any]]", resp)
         if not resp:
             raise ZeroMatchedError
 
         failed = [(i, f"Req_{i}: {r['message']}") for i, r in enumerate(resp) if "error" in r]
         if failed:
@@ -872,15 +903,15 @@
         Returns
         -------
         geopandas.GeoDataFrame
             GeoDataFrame of NID data
         """
         return gpd.GeoDataFrame(
             nid_df,
-            geometry=gpd.points_from_xy(nid_df.longitude, nid_df.latitude),
+            geometry=gpd.points_from_xy(nid_df["longitude"], nid_df["latitude"]),
             crs=4326,
         )
 
     def get_byfilter(self, query_list: list[dict[str, list[str]]]) -> list[gpd.GeoDataFrame]:
         """Query dams by filters from the National Inventory of Dams web service.
 
         Parameters
@@ -890,28 +921,26 @@
             use the advanced fields dataframe that can be accessed via ``NID().fields_meta``.
             Some filter require min/max values such as ``damHeight`` and ``drainageArea``.
             For such filters, the min/max values should be passed like so:
             ``{filter_key: ["[min1 max1]", "[min2 max2]"]}``.
 
         Returns
         -------
-        geopandas.GeoDataFrame
-            Query results.
+        list of geopandas.GeoDataFrame
+            Query results in the same order as the input query list.
 
         Examples
         --------
         >>> from pygeohydro import NID
         >>> nid = NID()
         >>> query_list = [
         ...    {"drainageArea": ["[200 500]"]},
         ...    {"nidId": ["CA01222"]},
         ... ]
         >>> dam_dfs = nid.get_byfilter(query_list)
-        >>> print(dam_dfs[0].loc[dam_dfs[0].name == "Prairie Portage"].id.item())
-        496613
         """
         fields = self.valid_fields.to_list()
         invalid = [k for key in query_list for k in key if k not in fields]
         if invalid:
             raise InputValueError("query_dict", fields)
         params = [
             {"sy": " ".join(f"@{s}:{fid}" for s, fids in key.items() for fid in fids)}
@@ -926,85 +955,64 @@
         """Retrieve NID data within a geometry.
 
         Parameters
         ----------
         geometry : Polygon, MultiPolygon, or tuple of length 4
             Geometry or bounding box (west, south, east, north) for extracting the data.
         geo_crs : list of str
-            The CRS of the input geometry, defaults to ``epsg:4326``.
+            The CRS of the input geometry.
 
         Returns
         -------
         geopandas.GeoDataFrame
             GeoDataFrame of NID data
 
         Examples
         --------
         >>> from pygeohydro import NID
         >>> nid = NID()
         >>> dams = nid.get_bygeom((-69.77, 45.07, -69.31, 45.45), 4326)
-        >>> print(dams.name.iloc[0])
-        Little Moose
         """
-        _geometry = geoutils.geo2polygon(geometry, geo_crs, 4326)
-        wbd = ArcGISRESTful(ServiceURL().restful.wbd, 4, outformat="json", outfields="huc8")
-        resp = wbd.get_features(wbd.oids_bygeom(_geometry), return_geom=False)
-        huc_ids = [
-            tlz.get_in(["attributes", "huc8"], i) for r in resp for i in tlz.get_in(["features"], r)
-        ]
-
-        dams = self.get_byfilter([{"huc8": huc_ids}])[0]
-        return dams[dams.within(_geometry)].copy()
+        _geometry = geoutils.geo2polygon(geometry, geo_crs, self.gdf.crs)
+        idx = self.gdf.sindex.query(_geometry, "contains")
+        return self.gdf.iloc[idx].copy()
 
-    def inventory_byid(self, federal_ids: list[int], stage_nid: bool = False) -> gpd.GeoDataFrame:
+    def inventory_byid(self, federal_ids: list[int]) -> gpd.GeoDataFrame:
         """Get extra attributes for dams based on their dam ID.
 
         Notes
         -----
         This function is meant to be used for getting extra attributes for dams.
         For example, first you need to use either ``get_bygeom`` or ``get_byfilter``
         to get basic attributes of the target dams. Then you can use this function
         to get extra attributes using the ``id`` column of the ``GeoDataFrame``
         that ``get_bygeom`` or ``get_byfilter`` returns.
 
         Parameters
         ----------
         federal_ids : list of str
             List of the target dam Federal IDs.
-        stage_nid : bool, optional
-            Whether to get the entire NID and then query locally or query from the
-            NID web service which tends to be very slow for large number of requests.
-            Defaults to ``False``. The staged NID database is saved as a `feather` file
-            in `./cache/nid_inventory.feather`.
 
         Returns
         -------
         pandas.DataFrame
             Dams with extra attributes in addition to the standard NID fields
             that other ``NID`` methods return.
 
         Examples
         --------
         >>> from pygeohydro import NID
         >>> nid = NID()
         >>> dams = nid.inventory_byid(['KY01232', 'GA02400', 'NE04081', 'IL55070', 'TN05345'])
-        >>> print(dams.damHeight.max())
-        39.0
         """
         ids = set(federal_ids) if isinstance(federal_ids, (list, tuple)) else {federal_ids}
         ids = {str(i).upper() for i in ids}
         urls = [f"{self.base_url}/dams/{i}/inventory" for i in ids]
         if len(urls) != len(ids):
             raise InputTypeError("dam_ids", "list of Federal IDs")
-
-        if stage_nid:
-            self.stage_nid_inventory()
-            dams = gpd.read_feather(self.nid_inventory_path)
-            return dams[dams.federalId.isin(list(ids))].copy()
-
         return self._to_geodf(pd.DataFrame(self._get_json(urls)).set_index("id"))
 
     def get_suggestions(
         self, text: str, context_key: str | None = None
     ) -> tuple[pd.DataFrame, pd.DataFrame]:
         """Get suggestions from the National Inventory of Dams web service.
 
@@ -1029,16 +1037,14 @@
             second, those found in the query fields such as states, huc6, etc.
 
         Examples
         --------
         >>> from pygeohydro import NID
         >>> nid = NID()
         >>> dams, contexts = nid.get_suggestions("houston", "city")
-        >>> print(contexts["suggestion"].to_list())
-        ['Houston', 'Houston Lake']
         """
         fields = self.valid_fields.to_list()
         params = {"text": text}
         if context_key:
             if context_key not in fields:
                 raise InputValueError("context", fields)
             params["contextKey"] = context_key
@@ -1107,16 +1113,16 @@
     _ = ogc.streaming_download(urls, fnames=files)
 
     def get_tif(file: Path) -> xr.DataArray:
         """Get the .tif file from a zip file."""
         with zipfile.ZipFile(file) as z:
             try:
                 fname = next(f.filename for f in z.filelist if f.filename.endswith(".tif"))
-            except StopIteration:
-                raise ZeroMatchedError
+            except StopIteration as ex:
+                raise ZeroMatchedError from ex
             ds = rxr.open_rasterio(io.BytesIO(z.read(fname)))
             ds = cast("xr.DataArray", ds)
             if "band" in ds.dims:
                 ds = ds.squeeze("band", drop=True)
             ds.name = valid_props[file.stem.split("_")[0]]["name"]
             ds.attrs["units"] = valid_props[file.stem.split("_")[0]]["units"]
             ds.attrs["long_name"] = valid_props[file.stem.split("_")[0]]["long_name"]
```

### Comparing `pygeohydro-0.14.0/pygeohydro/us_abbrs.py` & `pygeohydro-0.15.0/pygeohydro/us_abbrs.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.14.0/pygeohydro/waterdata.py` & `pygeohydro-0.15.0/pygeohydro/waterdata.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Accessing WaterData related APIs."""
 from __future__ import annotations
 
 import io
 from typing import Any, Literal, cast, overload
 
-import async_retriever as ar
 import cytoolz.curried as tlz
 import geopandas as gpd
 import pandas as pd
-import pygeoutils as geoutils
 
+import async_retriever as ar
+import pygeoutils as geoutils
 from pygeohydro.exceptions import InputTypeError, InputValueError, ServiceError
 
 __all__ = ["WaterQuality", "SensorThings"]
 
 
 class WaterQuality:
     """Water Quality Web Service https://www.waterqualitydata.us.
```

### Comparing `pygeohydro-0.14.0/pygeohydro/watershed.py` & `pygeohydro-0.15.0/pygeohydro/watershed.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from __future__ import annotations
 
 import importlib.util
 import io
 from pathlib import Path
 from typing import TYPE_CHECKING, Union
 
-import async_retriever as ar
 import geopandas as gpd
 import pandas as pd
-import pygeoogc as ogc
 import pyproj
 import xarray as xr
+
+import async_retriever as ar
+import pygeoogc as ogc
+from pygeohydro.exceptions import InputValueError
 from pygeoogc import ServiceURL
 from pynhd import AGRBase
 from pynhd.core import ScienceBase
 
-from pygeohydro.exceptions import InputValueError
-
 if TYPE_CHECKING:
     CRSTYPE = Union[int, str, pyproj.CRS]
 
 __all__ = [
     "WBD",
     "huc_wb_full",
     "irrigation_withdrawals",
@@ -100,15 +100,15 @@
     if huc_lvl not in valid_hucs:
         raise InputValueError("huc_lvl", list(map(str, valid_hucs)))
 
     base_url = "https://prd-tnm.s3.amazonaws.com/StagedProducts/Hydrography/WBD/HU2/Shape"
 
     urls = [f"{base_url}/WBD_{h2:02}_HU2_Shape.zip" for h2 in range(1, 23)]
     fnames = [Path("cache", Path(url).name) for url in urls]
-    _ = ogc.streaming_download(urls, fnames=fnames)  # type: ignore
+    _ = ogc.streaming_download(urls, fnames=fnames)
     keys = (p.stem.split("_")[1] for p in fnames)
     engine = "pyogrio" if importlib.util.find_spec("pyogrios") else "fiona"
     huc = gpd.GeoDataFrame(
         pd.concat(
             (gpd.read_file(f"{p}!Shape/WBDHU{huc_lvl}.shp", engine=engine) for p in fnames),
             keys=keys,
         )
```

### Comparing `pygeohydro-0.14.0/pygeohydro.egg-info/PKG-INFO` & `pygeohydro-0.15.0/pygeohydro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pygeohydro
-Version: 0.14.0
+Version: 0.15.0
 Summary: Access geospatial web services that offer hydrological data
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/pygeohydro/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pygeohydro.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/pygeohydro.html
 Project-URL: Issues, https://github.com/hyriver/pygeohydro/issues
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

### Comparing `pygeohydro-0.14.0/pygeohydro.egg-info/SOURCES.txt` & `pygeohydro-0.15.0/pygeohydro.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .codecov.yml
 .deepsource.toml
-.flake8
 .git_archival.txt
 .gitattributes
 .gitignore
 .pep8speaks.yml
 .pre-commit-config.yaml
 .sonarcloud.properties
 AUTHORS.rst
```

### Comparing `pygeohydro-0.14.0/tests/test_exceptions.py` & `pygeohydro-0.15.0/tests/test_exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import sys
 
 import geopandas as gpd
 import pandas as pd
 import pytest
-from shapely import Polygon
+from shapely.geometry import Polygon
 
 import pygeohydro as gh
-from pygeohydro import DataNotAvailableError, InputRangeError, InputTypeError, InputValueError
+from pygeohydro import (
+    DataNotAvailableError,
+    InputRangeError,
+    InputTypeError,
+    InputValueError,
+)
 
-has_typeguard = True if sys.modules.get("typeguard") else False
+has_typeguard = bool(sys.modules.get("typeguard"))
 
 SID_NATURAL = "01031500"
 GEOM = Polygon(
     [
         [-69.77, 45.07],
         [-69.31, 45.07],
         [-69.31, 45.45],
         [-69.77, 45.45],
         [-69.77, 45.07],
     ]
 )
 
 
 class TestETAExceptions:
-    "Test ssebopeta Exceptions"
     dates = ("2000-01-01", "2000-01-05")
 
     @pytest.mark.skipif(has_typeguard, reason="Broken if Typeguard is enabled")
     def test_invalid_dates(self):
         with pytest.raises(InputTypeError) as ex:
             _ = gh.ssebopeta_bycoords((GEOM.centroid.x, GEOM.centroid.y), dates="2000-01-01")
         assert "pandas.DataFrame" in str(ex.value)
@@ -44,15 +48,16 @@
         )
         with pytest.raises(InputRangeError) as ex:
             _ = gh.ssebopeta_bycoords(coords, dates=[2010, 2014, 2021])
         assert "2020" in str(ex.value)
 
 
 class TestNLCDExceptions:
-    "Test NLCD Exceptions"
+    """Test NLCD Exceptions."""
+
     years = {"cover": [2016, 2019]}
     res = 1e3
     geom = gpd.GeoSeries([GEOM], crs=4326)
 
     @pytest.mark.skipif(has_typeguard, reason="Broken if Typeguard is enabled")
     def test_invalid_years_type(self):
         with pytest.raises(InputTypeError) as ex:
@@ -94,14 +99,13 @@
                 ssl=False,
             )
             _ = gh.cover_statistics(lulc[0].cover_2016 * 2)
         assert "11" in str(ex.value)
 
 
 class TestNWISExceptions:
-    "Test NWIS"
     nwis = gh.NWIS()
 
     def test_invaild_station(self):
         with pytest.raises(DataNotAvailableError) as ex:
             _ = self.nwis.get_streamflow(SID_NATURAL, ("1900-01-01", "1900-01-31"))
         assert "Discharge" in str(ex.value)
```

### Comparing `pygeohydro-0.14.0/tests/test_pygeohydro.py` & `pygeohydro-0.15.0/tests/test_pygeohydro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """Tests for PyGeoHydro package."""
 import io
 import shutil
-import sys
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pytest
 import xarray as xr
-from pygeoogc import utils as ogc_utils
-from shapely import Polygon
+from shapely.geometry import Polygon
 
 import pygeohydro as gh
 from pygeohydro import NID, NWIS, WBD
-
-has_typeguard = True if sys.modules.get("typeguard") else False
+from pygeoogc import utils as ogc_utils
 
 DEF_CRS = 4326
-ALT_CRS = "epsg:3542"
+ALT_CRS = 3542
 SID_NATURAL = "01031500"
 SID_URBAN = "11092450"
 DATES = ("2005-01-01", "2005-01-31")
 DATES_LONG = ("2000-01-01", "2009-12-31")
 GEOM = Polygon(
     [
         [-69.77, 45.07],
@@ -34,41 +31,40 @@
 
 
 def assert_close(a: float, b: float) -> None:
     assert np.isclose(a, b, rtol=1e-3).all()
 
 
 class TestNWIS:
-    "Test NWIS"
     nwis: NWIS = NWIS()
 
     def test_qobs_dv(self):
         df = self.nwis.get_streamflow(SID_NATURAL, DATES)
         ds = self.nwis.get_streamflow(SID_NATURAL, DATES, to_xarray=True)
         col = f"USGS-{SID_NATURAL}"
         assert_close(df[col].sum().item(), ds.sel(station_id=col).discharge.sum().item())
         assert df.attrs[col]["huc_cd"] == ds.sel(station_id=col).huc_cd.item()
 
     def test_qobs_mmd(self):
         df = self.nwis.get_streamflow(SID_NATURAL, DATES, mmd=True)
-        assert_close(df[f"USGS-{SID_NATURAL}"].sum().item(), 27.7142)
+        assert_close(df[f"USGS-{SID_NATURAL}"].sum().item(), 27.6375)
 
     def test_cst_tz(self):
         q = self.nwis.get_streamflow(["08075000", "11092450"], DATES)
-        assert q.index.tz.tzname("") == "UTC"
+        assert q.index.tz.tzname(None) == "UTC"
 
     def test_qobs_iv(self):
         iv = self.nwis.get_streamflow(SID_NATURAL, ("2020-01-01", "2020-01-31"), freq="iv")
         dv = self.nwis.get_streamflow(SID_NATURAL, ("2020-01-01", "2020-01-31"), freq="dv")
         assert_close(abs(iv.mean().item() - dv.mean().item()), 0.0539)
 
     def test_info(self):
         query = {"sites": ",".join([SID_NATURAL])}
-        info = self.nwis.get_info(query, expanded=True)
-        assert_close(info.nhd_areasqkm.item(), 771.82)
+        info = self.nwis.get_info(query, expanded=True, nhd_info=True)
+        assert_close(info["nhd_areasqkm"].item(), 773.964)
         assert info.hcdn_2009.item()
 
     def test_info_box(self):
         query = {"bBox": ",".join(f"{b:.06f}" for b in GEOM.bounds)}
         info_box = self.nwis.get_info(query)
         assert info_box.shape[0] == 35
 
@@ -88,21 +84,16 @@
         qf = gh.streamflow_fillna(q)
         assert np.all(qf == 1)
         qf = gh.streamflow_fillna(q.to_frame("12345678"))
         assert np.all(qf == 1)
         qf = gh.streamflow_fillna(xr.DataArray(q))
         assert np.all(qf == 1)
 
-    def test_ice_negative(self):
-        ice = self.nwis.get_streamflow("04010500", ("2023-01-01", "2023-1-08"))
-        assert ice.isna().sum().item() == 8
-
 
 class TestETA:
-    "Test ssebopeta"
     dates = ("2000-01-01", "2000-01-05")
     years = [2010, 2014, 2015]
 
     def test_coords(self):
         coords = pd.DataFrame(
             [
                 ["s1", -72.77, 40.07],
@@ -171,37 +162,36 @@
     nid = NID()
     ids = ("KY01232", "GA02400", "NE04081", "IL55070", "TN05345")
 
     def test_suggestion(self):
         dams, contexts = self.nid.get_suggestions("houston", "city")
         assert dams.empty and contexts["suggestion"].to_list() == ["Houston", "Houston Lake"]
 
-    @pytest.mark.skipif(has_typeguard, reason="Broken if Typeguard is enabled")
     def test_filter(self):
         query_list = [
             {"drainageArea": ["[200 500]"]},
             {"nidId": ["CA01222"]},
         ]
         dam_dfs = self.nid.get_byfilter(query_list)
         assert dam_dfs[0].loc[dam_dfs[0].name == "Prairie Portage"].id.item() == "496613"
 
     def test_id(self):
         dams = self.nid.inventory_byid(self.ids)
         assert_close(dams.damHeight.max(), 39)
 
-    def test_stage_id(self):
-        dams = self.nid.inventory_byid(self.ids, stage_nid=True)
-        assert_close(dams.damHeight.max(), 39)
-
-    @pytest.mark.skipif(has_typeguard, reason="Broken if Typeguard is enabled")
     def test_geom(self):
         dams_geo = self.nid.get_bygeom(GEOM, DEF_CRS)
         bbox = ogc_utils.match_crs(GEOM.bounds, DEF_CRS, ALT_CRS)
         dams_box = self.nid.get_bygeom(bbox, ALT_CRS)
-        assert dams_geo.name.iloc[0] == dams_box.name.iloc[0] == "Little Moose"
+        name = "Pingree Pond"
+        assert (dams_geo.name == name).any() and (dams_box.name == "Pingree Pond").any()
+
+    def test_nation(self):
+        assert self.nid.df.shape == (91752, 77)
+        assert self.nid.gdf.shape == (91604, 92)
 
 
 class TestWaterQuality:
     wq: gh.WaterQuality = gh.WaterQuality()
 
     def test_bbox(self):
         stations = self.wq.station_bybbox(
@@ -323,14 +313,14 @@
     df = sensor.query_byodata(odata)
     assert df.shape[0] == 192
 
     df = sensor.sensor_info("USGS-09380000")
     assert df["description"].iloc[0] == "Stream"
 
     df = sensor.sensor_property("Datastreams", "USGS-09380000")
-    assert df["@iot.id"].iloc[0] == "a62122d8ff094125b63bb2f73410b2b4"
+    assert df["observationType"].unique()[0] == "Instantaneous"
 
 
 def test_show_versions():
     f = io.StringIO()
     gh.show_versions(file=f)
     assert "SYS INFO" in f.getvalue()
```

