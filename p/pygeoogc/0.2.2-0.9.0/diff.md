# Comparing `tmp/pygeoogc-0.2.2.tar.gz` & `tmp/pygeoogc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygeoogc-0.2.2.tar", last modified: Mon Dec  7 22:34:18 2020, max compression
+gzip compressed data, was "pygeoogc-0.9.0.tar", last modified: Wed Feb 17 18:19:38 2021, max compression
```

## Comparing `pygeoogc-0.2.2.tar` & `pygeoogc-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.867963 pygeoogc-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (116)      146 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (116)       97 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)      242 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.863963 pygeoogc-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.863963 pygeoogc-0.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      923 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (116)      684 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (116)      125 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.863963 pygeoogc-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2584 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (116)      288 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1163 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1202 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      163 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1579 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      157 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3444 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4193 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2741 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      183 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2186 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)    14664 2020-12-07 22:34:18.871963 pygeoogc-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    11671 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.859963 pygeoogc-0.2.2/ci/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.867963 pygeoogc-0.2.2/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)      302 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (116)      239 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/ci/requirements/py3.6.yml
--rw-r--r--   0 runner    (1001) docker     (116)      223 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/ci/requirements/py3.7.yml
--rw-r--r--   0 runner    (1001) docker     (116)      223 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/ci/requirements/py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (116)      239 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/ci/requirements/py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.867963 pygeoogc-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     8187 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.867963 pygeoogc-0.2.2/docs/_template/
--rw-r--r--   0 runner    (1001) docker     (116)       85 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/docs/_template/layout.html
--rw-r--r--   0 runner    (1001) docker     (116)    11895 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      771 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       71 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (116)      875 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/docs/pygeoogc.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.867963 pygeoogc-0.2.2/pygeoogc/
--rw-r--r--   0 runner    (1001) docker     (116)      540 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/pygeoogc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14704 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/pygeoogc/core.py
--rw-r--r--   0 runner    (1001) docker     (116)     2448 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/pygeoogc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     5079 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/pygeoogc/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (116)    20853 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/pygeoogc/pygeoogc.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.867963 pygeoogc-0.2.2/pygeoogc/static/
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/pygeoogc/static/urls.yml
--rw-r--r--   0 runner    (1001) docker     (116)    19475 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/pygeoogc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.867963 pygeoogc-0.2.2/pygeoogc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    14664 2020-12-07 22:34:18.000000 pygeoogc-0.2.2/pygeoogc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1170 2020-12-07 22:34:18.000000 pygeoogc-0.2.2/pygeoogc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 22:34:18.000000 pygeoogc-0.2.2/pygeoogc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 22:34:18.000000 pygeoogc-0.2.2/pygeoogc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      117 2020-12-07 22:34:18.000000 pygeoogc-0.2.2/pygeoogc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-07 22:34:18.000000 pygeoogc-0.2.2/pygeoogc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      249 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.867963 pygeoogc-0.2.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)     4671 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/scripts/generate_pip_deps_from_conda.py
--rw-r--r--   0 runner    (1001) docker     (116)     1867 2020-12-07 22:34:18.871963 pygeoogc-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 22:34:18.867963 pygeoogc-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1777 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     8413 2020-12-07 22:34:14.000000 pygeoogc-0.2.2/tests/test_pygeoogc.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       97 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (116)      242 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.498020 pygeoogc-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.498020 pygeoogc-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (116)      684 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (116)      321 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.498020 pygeoogc-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2719 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1306 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1345 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1226 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      163 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1867 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      157 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3444 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4192 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3625 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1096 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      183 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2186 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)    16531 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    13282 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.490020 pygeoogc-0.9.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (116)      328 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      266 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/ci/requirements/py3.6.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/ci/requirements/py3.7.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/ci/requirements/py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/ci/requirements/py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     8187 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/docs/_template/
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/docs/_template/layout.html
+-rw-r--r--   0 runner    (1001) docker     (116)    11895 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      771 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (116)       71 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      875 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/docs/pygeoogc.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/pygeoogc/
+-rw-r--r--   0 runner    (1001) docker     (116)      679 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/pygeoogc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15061 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/pygeoogc/core.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2440 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/pygeoogc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5251 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/pygeoogc/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22472 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/pygeoogc/pygeoogc.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/pygeoogc/static/
+-rw-r--r--   0 runner    (1001) docker     (116)     1629 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/pygeoogc/static/urls.yml
+-rw-r--r--   0 runner    (1001) docker     (116)    20651 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/pygeoogc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/pygeoogc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    16531 2021-02-17 18:19:38.000000 pygeoogc-0.9.0/pygeoogc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1170 2021-02-17 18:19:38.000000 pygeoogc-0.9.0/pygeoogc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:19:38.000000 pygeoogc-0.9.0/pygeoogc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:19:38.000000 pygeoogc-0.9.0/pygeoogc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      136 2021-02-17 18:19:38.000000 pygeoogc-0.9.0/pygeoogc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2021-02-17 18:19:38.000000 pygeoogc-0.9.0/pygeoogc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      268 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4753 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/scripts/generate_pip_deps_from_conda.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2033 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      587 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:19:38.502020 pygeoogc-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     1777 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7727 2021-02-17 18:19:33.000000 pygeoogc-0.9.0/tests/test_pygeoogc.py
```

### Comparing `pygeoogc-0.2.2/.github/ISSUE_TEMPLATE/bug-report.md` & `pygeoogc-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/.github/ISSUE_TEMPLATE/feature-request.md` & `pygeoogc-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/.github/workflows/codeql-analysis.yml` & `pygeoogc-0.9.0/.github/workflows/codeql-analysis.yml`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         # Override automatic language detection by changing the below list
         # Supported options are ['csharp', 'cpp', 'go', 'java', 'javascript', 'python']
         language: ['python']
         # Learn more...
         # https://docs.github.com/en/github/finding-security-vulnerabilities-and-errors-in-your-code/configuring-code-scanning#overriding-automatic-language-detection
 
     steps:
+    - name: Cancel Previous Runs
+      uses: styfle/cancel-workflow-action@0.6.0
+      with:
+        access_token: ${{ github.token }}
     - name: Checkout repository
       uses: actions/checkout@v2
       with:
         # We must fetch at least the immediate parents so that if this is
         # a pull request then we can checkout the head.
         fetch-depth: 2
```

### Comparing `pygeoogc-0.2.2/.github/workflows/release.yml` & `pygeoogc-0.9.0/.github/workflows/release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 name: Release and publish
 
 jobs:
   build:
     name: Create Release
     runs-on: ubuntu-latest
     steps:
+      - name: Cancel Previous Runs
+        uses: styfle/cancel-workflow-action@0.6.0
+        with:
+          access_token: ${{ github.token }}
       - name: Checkout code
         uses: actions/checkout@v2
 
       - name: Create Release
         id: create_release
         uses: actions/create-release@v1
         env:
```

### Comparing `pygeoogc-0.2.2/.github/workflows/test.yml` & `pygeoogc-0.9.0/.github/workflows/test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,18 @@
         python-version: [3.6, 3.7, 3.8, 3.9]
         os: [ubuntu-latest, macos-latest, windows-latest]
         exclude:
             - os: windows-latest
               python-version: 3.6
 
     steps:
+      - name: Cancel Previous Runs
+        uses: styfle/cancel-workflow-action@0.6.0
+        with:
+          access_token: ${{ github.token }}
       - uses: actions/checkout@master
       - name: Setup miniconda
         uses: conda-incubator/setup-miniconda@master
         with:
           activate-environment: pygeoogc
           python-version: ${{ matrix.python-version }}
           environment-file: ci/requirements/py${{ matrix.python-version }}.yml
```

### Comparing `pygeoogc-0.2.2/.gitignore` & `pygeoogc-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/.pre-commit-config.yaml` & `pygeoogc-0.9.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,72 @@
 repos:
-  # isort should run before black as black sometimes tweaks the isort output
   - repo: https://github.com/timothycrosley/isort
-    rev: 5.6.4
+    rev: 5.7.0
     hooks:
       - id: isort
         name: Sort imports with isort
 
   - repo: https://github.com/python/black
     rev: 20.8b1
     hooks:
       - id: black
         name: Autoformat with black
         args: [-t, py38, -l, "100"]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.3.0
+    rev: v3.4.0
     hooks:
     - id: trailing-whitespace
     - id: check-executables-have-shebangs
     - id: requirements-txt-fixer
+    - id: check-added-large-files
+      args: ['--maxkb=50000']
+    - id: end-of-file-fixer
+
+  - repo: https://github.com/pre-commit/pygrep-hooks
+    rev: v1.7.1
+    hooks:
+    - id: rst-backticks
+    - id: rst-directive-colons
+
+  - repo: https://github.com/jumanjihouse/pre-commit-hooks
+    rev: 2.1.4
+    hooks:
+    - id: shfmt
 
   - repo: https://github.com/PyCQA/doc8
     rev: 0.9.0a1
     hooks:
     - id: doc8
       name: Autoformat with doc8
       args: [--max-line-length, "100"]
 
   - repo: https://gitlab.com/pycqa/flake8
     rev: 3.8.4
     hooks:
       - id: flake8
         name: Linting with flake8
         exclude: docs/conf.py
-        additional_dependencies: [flake8-comprehensions, flake8-builtins, flake8-blind-except, flake8-bugbear, flake8-use-fstring, flake8-docstrings]
+        additional_dependencies: [flake8-comprehensions, flake8-builtins, flake8-blind-except, flake8-bugbear, flake8-use-fstring, flake8-docstrings, flake8-simplify]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.790
+    rev: v0.800
     hooks:
       - id: mypy
         name: Static type checking with mypy
-        files: pygeoogc
+        exclude: tests
+        files: pynhd
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.7.4
+    rev: v2.10.0
     hooks:
       - id: pyupgrade
         name: Upgrade synax to python 3.6+ with pyupgrade
         args: [--py36-plus]
 
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.6.3
+    rev: 1.7.0
     hooks:
       - id: bandit
         name: Check for security issues with bandit
-        args: [-lll, --recursive, pygeoogc]
+        args: [-lll, --recursive, pynhd]
         files: .py$
```

### Comparing `pygeoogc-0.2.2/CODE_OF_CONDUCT.rst` & `pygeoogc-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/CONTRIBUTING.rst` & `pygeoogc-0.9.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -145,8 +145,7 @@
 
     $ git tag -a vX.X.X -m "vX.X.X"
     $ git push --follow-tags
 
 where ``X.X.X`` is the version number following the
 `semantic versioning spec <https://semver.org>`__ i.e., MAJOR.MINOR.PATCH.
 Then release the tag from Github and Github Actions will deploy it to PyPi.
-
```

### Comparing `pygeoogc-0.2.2/HISTORY.rst` & `pygeoogc-0.9.0/HISTORY.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 =======
 History
 =======
 
+0.9.0 (2021-02-14)
+------------------
+
+- Bump version to the same version as Hydrodata.
+- Add support for query by point and multi-points to ``ArcGISRESTful.bygeom``.
+- Add support for buffer distance to ``ArcGISRESTful.bygeom``.
+- Add support for generating ESRI-based queries for points and multi-points
+  to ``ESRIGeomQuery``.
+- Add all the missing type annotations.
+- Update the Daymet url to version 4. You can check the release information
+  `here <https://daac.ornl.gov/DAYMET/guides/Daymet_Daily_V4.html>`_
+- Use ``cytoolz`` library for some of the operations for improving performance.
+- Add ``extent`` property to ``ArcGISRESTful`` class that get the spatial extent
+  of the service.
+- Add url to ``airmap`` service for getting elevation data at 30 m resolution.
+
+0.2.3 (2020-12-19)
+-------------------
+
+- Fix ``urlib3`` deprecation warning about using ``method_whitelist``.
+
 0.2.2 (2020-12-05)
 -------------------
 
 - Remove unused variables in ``async_requests`` and use ``max_workers``.
 - Fix the ``async_requests`` issue on Windows systems.
 
 
@@ -54,22 +75,22 @@
 - Add ``always_xy`` flag to ``WMS`` and ``WFS`` which is False by default. It is useful
   for cases where a web service doesn't change the axis order from the transitional
   ``xy`` to ``yx`` for versions higher than 1.3.0.
 
 0.1.3 (2020-07-21)
 ------------------
 
-- Remove unneccassary transformation of the input bbox in WFS.
+- Remove unnecessary transformation of the input bbox in WFS.
 - Use ``setuptools_scm`` for versioning.
 
 0.1.2 (2020-07-16)
 ------------------
 
 - Add the missing ``max_pixel`` argument to the ``wms_bybox`` function.
 - Change the ``onlyIPv4`` method of ``RetrySession`` class to ``onlyipv4``
   to conform to the ``snake_case`` convention.
-- Improve docsctrings.
+- Improve docstrings.
 
 0.1.1 (2020-07-15)
 ------------------
 
 - Initial release.
```

### Comparing `pygeoogc-0.2.2/LICENSE` & `pygeoogc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/Makefile` & `pygeoogc-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/PKG-INFO` & `pygeoogc-0.9.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,294 +1,304 @@
-Metadata-Version: 2.1
-Name: pygeoogc
-Version: 0.2.2
-Summary: An interface to ArcGIS RESTful-, WFS-, and WMS-based services.
-Home-page: https://github.com/cheginit/pygeoogc
-Author: Taher Chegini
-Author-email: cheginit@gmail.com
-License: MIT license
-Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pygeoogc_logo.png
-            :target: https://github.com/cheginit/pygeoogc
-            :align: center
-        
-        |
-        
-        .. |hydrodata| image:: https://github.com/cheginit/hydrodata/workflows/pytest/badge.svg
-            :target: https://github.com/cheginit/hydrodata/actions?query=workflow%3Apytest
-            :alt: Github Actions
-        
-        .. |pygeoogc| image:: https://github.com/cheginit/pygeoogc/workflows/pytest/badge.svg
-            :target: https://github.com/cheginit/pygeoogc/actions?query=workflow%3Apytest
-            :alt: Github Actions
-        
-        .. |pygeoutils| image:: https://github.com/cheginit/pygeoutils/workflows/pytest/badge.svg
-            :target: https://github.com/cheginit/pygeoutils/actions?query=workflow%3Apytest
-            :alt: Github Actions
-        
-        .. |pynhd| image:: https://github.com/cheginit/pynhd/workflows/pytest/badge.svg
-            :target: https://github.com/cheginit/pynhd/actions?query=workflow%3Apytest
-            :alt: Github Actions
-        
-        .. |py3dep| image:: https://github.com/cheginit/py3dep/workflows/pytest/badge.svg
-            :target: https://github.com/cheginit/py3dep/actions?query=workflow%3Apytest
-            :alt: Github Actions
-        
-        .. |pydaymet| image:: https://github.com/cheginit/pydaymet/workflows/pytest/badge.svg
-            :target: https://github.com/cheginit/pydaymet/actions?query=workflow%3Apytest
-            :alt: Github Actions
-        
-        =========== ==================================================================== ============
-        Package     Description                                                          Status
-        =========== ==================================================================== ============
-        Hydrodata_  Access NWIS, HCDN 2009, NLCD, and SSEBop databases                   |hydrodata|
-        PyGeoOGC_   Send queries to any ArcGIS RESTful-, WMS-, and WFS-based services    |pygeoogc|
-        PyGeoUtils_ Convert responses from PyGeoOGC's supported web services to datasets |pygeoutils|
-        PyNHD_      Navigate and subset NHDPlus (MR and HR) using web services           |pynhd|
-        Py3DEP_     Access topographic data through National Map's 3DEP web service      |py3dep|
-        PyDaymet_   Access Daymet for daily climate data both single pixel and gridded   |pydaymet|
-        =========== ==================================================================== ============
-        
-        .. _Hydrodata: https://github.com/cheginit/hydrodata
-        .. _PyGeoOGC: https://github.com/cheginit/pygeoogc
-        .. _PyGeoUtils: https://github.com/cheginit/pygeoutils
-        .. _PyNHD: https://github.com/cheginit/pynhd
-        .. _Py3DEP: https://github.com/cheginit/py3dep
-        .. _PyDaymet: https://github.com/cheginit/pydaymet
-        
-        PyGeoOGC: Query ArcGIS RESTful, WMS, and WFS
-        --------------------------------------------
-        
-        .. image:: https://img.shields.io/pypi/v/pygeoogc.svg
-            :target: https://pypi.python.org/pypi/pygeoogc
-            :alt: PyPi
-        
-        .. image:: https://img.shields.io/conda/vn/conda-forge/pygeoogc.svg
-            :target: https://anaconda.org/conda-forge/pygeoogc
-            :alt: Conda Version
-        
-        .. image:: https://codecov.io/gh/cheginit/pygeoogc/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/cheginit/pygeoogc
-            :alt: CodeCov
-        
-        .. image:: https://mybinder.org/badge_logo.svg
-            :target: https://mybinder.org/v2/gh/cheginit/hydrodata/master?filepath=docs%2Fexamples
-            :alt: Binder
-        
-        |
-        
-        .. image:: https://img.shields.io/badge/security-bandit-green.svg
-            :target: https://github.com/PyCQA/bandit
-            :alt: Security Status
-        
-        .. image:: https://www.codefactor.io/repository/github/cheginit/pygeoogc/badge
-           :target: https://www.codefactor.io/repository/github/cheginit/pygeoogc
-           :alt: CodeFactor
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/psf/black
-            :alt: black
-        
-        .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
-            :target: https://github.com/pre-commit/pre-commit
-            :alt: pre-commit
-        
-        |
-        
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
-        Features
-        --------
-        
-        PyGeoOGC is a part of Hydrodata software stack and provides interfaces to web services
-        that are based on
-        `ArcGIS RESTful <https://en.wikipedia.org/wiki/Representational_state_transfer>`__,
-        `WMS <https://en.wikipedia.org/wiki/Web_Map_Service>`__, and
-        `WFS <https://en.wikipedia.org/wiki/Web_Feature_Service>`__. It is noted that although
-        all these web service have limits on the number of objects per requests (e.g., 1000
-        objectIDs for RESTful and 8 million pixels for WMS), PyGeoOGC divides the requests into
-        smaller chunks under-the-hood and then merges the returned responses.
-        
-        There is also an inventory of URLs for some of these web services in form of a class called
-        ``ServiceURL``. These URLs are in three categories: ``ServiceURL().restful``,
-        ``ServiceURL().wms``, and ``ServiceURL().wfs``. These URLs provide you with some examples
-        of the services that PyGeoOGC supports. All the URLs are read from a YAML file located
-        `here <pygeoogc/static/urls.yml>`_. If you had success using PyGeoOGC with a web service
-        please consider adding its URL to this YAML file which is located at ``pygeoogc/static/urls.yml``.
-        
-        There are three main classes:
-        
-        * ``ArcGISRESTful``: This class can be instantiated by providing the target layer URL.
-          For example, for getting Watershed Boundary Data we can use ``ServiceURL().restful.wbd``.
-          By looking at the web service website
-          (https://hydro.nationalmap.gov/arcgis/rest/services/wbd/MapServer) we see that there are 9
-          layers; 1 for 2-digit HU (Region), 6 for 12-digit HU (Subregion), and so on. We can either
-          pass the base URL or concatenate the target layer number like so
-          ``f"{ServiceURL().restful.wbd}/6"``.
-        
-          If you want to change the layer you can simply set the ``layer`` property of the class.
-          Afterward, we can request for the data in two steps. First, get the object IDs using
-          ``oids_bygeom`` (within a geometry), ``oids_byfield`` (specific field IDs), or ``oids_bysql``
-          (any valid SQL 92 WHERE clause) class methods. Second, get the actual data using ``get_features``
-          class method. The returned response can be converted into a GeoDataFrame using ``json2geodf``
-          function from `PyGeoOGC <https://github.com/cheginit/pygeoutils>`__ package.
-        
-        * ``WMS``: Instantiation of this class requires at least 3 arguments: service URL, layer(s)
-          name(s), and output format. Additionally, target CRS and the web service version can be provided.
-          Upon instantiation, we could use ``getmap_bybox`` method class to get the raster data within a
-          bounding box. The box can be any valid CRS and if it is different from the default EPSG:4326, it
-          should be passed to the function using ``box_crs`` argumnet. The service response can be
-          converted into a ``xarray.Dataset`` using ``gtiff2xarray`` function from PyGeoOGC package.
-        
-        * ``WFS``: Instantiation of this class is similar to ``WMS`` and the only difference is that
-          only one layer name can be passed. Upon instantiation there are three ways to get the data:
-        
-          - ``getfeature_bybox``: Get all the features within a bounding box in any valid CRS.
-          - ``getfeature_byid``: Get all the features based on the IDs. Note that two arguments should be
-            provided: ``featurename``, and ``featureids``. You can get a list of valid feature names using
-            ``get_validnames`` class method.
-          - ``getfeature_byfilter``: Get the data based on a valid
-            `CQL <https://docs.geoserver.org/latest/en/user/tutorials/cql/cql_tutorial.html>`__ filter.
-        
-          You can convert the returned response to a GeoDataFrame using ``json2geodf`` function
-          from PyGeoOGC package.
-        
-        You can try using PyGeoOGC without installing it on you system by clicking on the binder badge
-        below the PyGeoOGC banner. A Jupyter notebook instance with the Hydrodata software stack
-        pre-installed will be launched in your web browser and you can start coding!
-        
-        Moreover, requests for additional functionalities can be submitted via
-        `issue tracker <https://github.com/cheginit/pygeoogc/issues>`__.
-        
-        Installation
-        ------------
-        
-        You can install PyGeoOGC using ``pip``:
-        
-        .. code-block:: console
-        
-            $ pip install pygeoogc
-        
-        Alternatively, PyGeoOGC can be installed from the ``conda-forge`` repository
-        using `Conda <https://docs.conda.io/en/latest/>`__:
-        
-        .. code-block:: console
-        
-            $ conda install -c conda-forge pygeoogc
-        
-        Quick start
-        -----------
-        
-        We can access
-        `NHDPlus HR <https://edits.nationalmap.gov/arcgis/rest/services/NHDPlus_HR/NHDPlus_HR/MapServer>`__
-        via RESTful service,
-        `National Wetlands Inventory <https://www.fws.gov/wetlands/>`__ from WMS, and
-        `FEMA National Flood Hazard <https://www.fema.gov/national-flood-hazard-layer-nfhl>`__
-        via WFS. The output for these functions are of type ``requests.Response`` that
-        can be converted to ``GeoDataFrame`` or ``xarray.Dataset`` using
-        `PyGeoOGC <https://github.com/cheginit/pygeoogc>`__.
-        
-        Let's start the National Map's NHDPlus HR web service. We can query the flowlines that are
-        within a geometry as follows:
-        
-        .. code-block:: python
-        
-            from pygeoogc import ArcGISRESTful, WFS, WMS, ServiceURL
-            import pygeoutils as geoutils
-            from pynhd import NLDI
-        
-            basin_geom = NLDI().getfeature_byid(
-                "nwissite",
-                "USGS-11092450",
-                basin=True
-            ).geometry[0]
-        
-            hr = ArcGISRESTful(ServiceURL().restful.nhdplushr, outformat="json")
-            hr.layer = 2
-        
-            hr.oids_bygeom(basin_geom, "epsg:4326")
-            resp = hr.get_features()
-            flowlines = geoutils.json2geodf(resp)
-        
-        Note ``oids_bygeom`` has an additional argument for passing any valid SQL WHERE clause
-        to further filter the data on the server side.
-        
-        We can also submit a query based on IDs of any valid field in the database. If the measure
-        property is desired you can pass ``return_m`` as ``True`` to the ``get_features`` class method:
-        
-        .. code-block:: python
-        
-            hr.oids_byfield("NHDPLUSID", [5000500013223, 5000400039708, 5000500004825])
-            resp = hr.get_features(return_m=True)
-            flowlines = geoutils.json2geodf(resp)
-        
-        Additionally, any valid SQL 92 WHERE clause can be used. For more details look
-        `here <https://developers.arcgis.com/rest/services-reference/query-feature-service-.htm#ESRI_SECTION2_07DD2C5127674F6A814CE6C07D39AD46>`__.
-        
-        .. code-block:: python
-        
-            hr.oids_bysql("NHDPLUSID IN (5000500013223, 5000400039708, 5000500004825)")
-            resp = hr.get_features()
-            flowlines = geoutils.json2geodf(resp)
-        
-        A WMS-based example is shown below:
-        
-        .. code-block:: python
-        
-            wms = WMS(
-                ServiceURL().wms.fws,
-                layers="0",
-                outformat="image/tiff",
-                crs="epsg:3857",
-            )
-            r_dict = wms.getmap_bybox(
-                basin_geom.bounds,
-                1e3,
-                box_crs="epsg:4326",
-            )
-            wetlands = geoutils.gtiff2xarray(r_dict, basin_geom, "epsg:4326")
-        
-        Query from a WFS-based web service can be done either within a bounding box or using
-        any valid `CQL filter <https://docs.geoserver.org/stable/en/user/tutorials/cql/cql_tutorial.html>`__.
-        
-        .. code-block:: python
-        
-            wfs = WFS(
-                ServiceURL().wfs.fema,
-                layer="public_NFHL:Base_Flood_Elevations",
-                outformat="esrigeojson",
-                crs="epsg:4269",
-            )
-            r = wfs.getfeature_bybox(basin_geom.bounds, box_crs="epsg:4326")
-            flood = geoutils.json2geodf(r.json(), "epsg:4269", "epsg:4326")
-        
-            layer = "wmadata:huc08"
-            wfs = WFS(
-                ServiceURL().wfs.waterdata,
-                layer=layer,
-                outformat="application/json",
-                version="2.0.0",
-                crs="epsg:4269",
-            )
-            r = wfs.getfeature_byfilter(f"huc8 LIKE '13030%'")
-            huc8 = geoutils.json2geodf(r.json(), "epsg:4269", "epsg:4326")
-        
-        
-        Contributing
-        ------------
-        
-        Contributions are appreciated and very welcomed. Please read
-        `CONTRIBUTING.rst <https://github.com/cheginit/pygeoogc/blob/master/CONTRIBUTING.rst>`__
-        for instructions.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
+.. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pygeoogc_logo.png
+    :target: https://github.com/cheginit/pygeoogc
+    :align: center
+
+|
+
+.. |hydrodata| image:: https://github.com/cheginit/hydrodata/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/hydrodata/actions?query=workflow%3Apytest
+    :alt: Github Actions
+
+.. |pygeoogc| image:: https://github.com/cheginit/pygeoogc/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/pygeoogc/actions?query=workflow%3Apytest
+    :alt: Github Actions
+
+.. |pygeoutils| image:: https://github.com/cheginit/pygeoutils/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/pygeoutils/actions?query=workflow%3Apytest
+    :alt: Github Actions
+
+.. |pynhd| image:: https://github.com/cheginit/pynhd/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/pynhd/actions?query=workflow%3Apytest
+    :alt: Github Actions
+
+.. |py3dep| image:: https://github.com/cheginit/py3dep/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/py3dep/actions?query=workflow%3Apytest
+    :alt: Github Actions
+
+.. |pydaymet| image:: https://github.com/cheginit/pydaymet/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/pydaymet/actions?query=workflow%3Apytest
+    :alt: Github Actions
+
+=========== ==================================================================== ============
+Package     Description                                                          Status
+=========== ==================================================================== ============
+Hydrodata_  Access NWIS, HCDN 2009, NLCD, and SSEBop databases                   |hydrodata|
+PyGeoOGC_   Send queries to any ArcGIS RESTful-, WMS-, and WFS-based services    |pygeoogc|
+PyGeoUtils_ Convert responses from PyGeoOGC's supported web services to datasets |pygeoutils|
+PyNHD_      Navigate and subset NHDPlus (MR and HR) using web services           |pynhd|
+Py3DEP_     Access topographic data through National Map's 3DEP web service      |py3dep|
+PyDaymet_   Access Daymet for daily climate data both single pixel and gridded   |pydaymet|
+=========== ==================================================================== ============
+
+.. _Hydrodata: https://github.com/cheginit/hydrodata
+.. _PyGeoOGC: https://github.com/cheginit/pygeoogc
+.. _PyGeoUtils: https://github.com/cheginit/pygeoutils
+.. _PyNHD: https://github.com/cheginit/pynhd
+.. _Py3DEP: https://github.com/cheginit/py3dep
+.. _PyDaymet: https://github.com/cheginit/pydaymet
+
+PyGeoOGC: Query ArcGIS RESTful, WMS, and WFS
+--------------------------------------------
+
+.. image:: https://img.shields.io/pypi/v/pygeoogc.svg
+    :target: https://pypi.python.org/pypi/pygeoogc
+    :alt: PyPi
+
+.. image:: https://img.shields.io/conda/vn/conda-forge/pygeoogc.svg
+    :target: https://anaconda.org/conda-forge/pygeoogc
+    :alt: Conda Version
+
+.. image:: https://codecov.io/gh/cheginit/pygeoogc/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/cheginit/pygeoogc
+    :alt: CodeCov
+
+.. image:: https://mybinder.org/badge_logo.svg
+    :target: https://mybinder.org/v2/gh/cheginit/hydrodata/master?filepath=docs%2Fexamples
+    :alt: Binder
+
+|
+
+.. image:: https://img.shields.io/badge/security-bandit-green.svg
+    :target: https://github.com/PyCQA/bandit
+    :alt: Security Status
+
+.. image:: https://www.codefactor.io/repository/github/cheginit/pygeoogc/badge
+   :target: https://www.codefactor.io/repository/github/cheginit/pygeoogc
+   :alt: CodeFactor
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: black
+
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+    :target: https://github.com/pre-commit/pre-commit
+    :alt: pre-commit
+
+|
+
+Features
+--------
+
+PyGeoOGC is a part of Hydrodata software stack and provides interfaces to web services
+that are based on
+`ArcGIS RESTful <https://en.wikipedia.org/wiki/Representational_state_transfer>`__,
+`WMS <https://en.wikipedia.org/wiki/Web_Map_Service>`__, and
+`WFS <https://en.wikipedia.org/wiki/Web_Feature_Service>`__. It is noted that although
+all these web service have limits on the number of features per requests (e.g., 1000
+objectIDs for a RESTful request or 8 million pixels for a WMS request), PyGeoOGC divides
+the requests into smaller chunks under-the-hood and then merges the returned responses.
+
+There is also an inventory of URLs for some of these web services in form of a class called
+``ServiceURL``. These URLs are in three categories: ``ServiceURL().restful``,
+``ServiceURL().wms``, and ``ServiceURL().wfs``. These URLs provide you with some examples
+of the services that PyGeoOGC supports. All the URLs are read from a YAML file located
+`here <pygeoogc/static/urls.yml>`_. If you have success using PyGeoOGC with a web service
+please consider adding its URL to this YAML file which is located at ``pygeoogc/static/urls.yml``.
+
+There are three main classes:
+
+* ``ArcGISRESTful``: This class can be instantiated by providing the target layer URL.
+  For example, for getting Watershed Boundary Data we can use ``ServiceURL().restful.wbd``.
+  By looking at the web service `website <https://hydro.nationalmap.gov/arcgis/rest/services/wbd/MapServer>`_
+  we see that there are 9
+  layers. For example, 1 for 2-digit HU (Region), 6 for 12-digit HU (Subregion), and so on. We can
+  pass the URL to the target layer like this
+  ``f"{ServiceURL().restful.wbd}/6"``.
+
+  Another option is to pass the base URL, ``ServiceURL().restful.wbd``, then set the ``layer``
+  property of the class.
+  Afterward, we request for the data in two steps. First, we need to get the taget object IDs using
+  ``oids_bygeom`` (within a geometry), ``oids_byfield`` (specific field IDs), or ``oids_bysql``
+  (any valid SQL 92 WHERE clause) class methods. Then, we can get the target features using
+  ``get_features`` class method. The returned response can be converted into a GeoDataFrame using
+  ``json2geodf`` function from `PyGeoUtils <https://github.com/cheginit/pygeoutils>`__ package.
+
+* ``WMS``: Instantiation of this class requires at least 3 arguments: service URL, layer
+  name(s), and output format. Additionally, target CRS and the web service version can be provided.
+  Upon instantiation, we could use ``getmap_bybox`` method class to get the target raster data
+  within a bounding box. The box can be in any valid CRS and if it is different from the default
+  CRS, EPSG:4326, it should be passed using ``box_crs`` argumnet. The service response can be
+  converted into a ``xarray.Dataset`` using ``gtiff2xarray`` function from PyGeoUtils package.
+
+* ``WFS``: Instantiation of this class is similar to ``WMS``. The only difference is that
+  only one layer name can be passed. Upon instantiation there are three ways to get the data:
+
+  - ``getfeature_bybox``: Get all the target features within a bounding box in any valid CRS.
+  - ``getfeature_byid``: Get all the target features based on the IDs. Note that two arguments
+    should be provided: ``featurename``, and ``featureids``. You can get a list of valid feature
+    names using ``get_validnames`` class method.
+  - ``getfeature_byfilter``: Get the data based on any valid
+    `CQL <https://docs.geoserver.org/latest/en/user/tutorials/cql/cql_tutorial.html>`__ filter.
+
+  You can convert the returned response of this function to a GeoDataFrame using ``json2geodf``
+  function from PyGeoUtils package.
+
+You can try using PyGeoOGC without installing it on you system by clicking on the binder badge
+below the PyGeoOGC banner. A Jupyter notebook instance with the Hydrodata software stack
+pre-installed will be launched in your web browser and you can start coding!
+
+Please note that since Hydrodata is in early development stages, while the provided
+functionaities should be stable, changes in APIs are possible in new releases. But we
+appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+
+Moreover, requests for additional functionalities can be submitted via
+`issue tracker <https://github.com/cheginit/pygeoogc/issues>`__.
+
+Installation
+------------
+
+You can install PyGeoOGC using ``pip``:
+
+.. code-block:: console
+
+    $ pip install pygeoogc
+
+Alternatively, PyGeoOGC can be installed from the ``conda-forge`` repository
+using `Conda <https://docs.conda.io/en/latest/>`__:
+
+.. code-block:: console
+
+    $ conda install -c conda-forge pygeoogc
+
+Quick start
+-----------
+
+We can access
+`NHDPlus HR <https://edits.nationalmap.gov/arcgis/rest/services/NHDPlus_HR/NHDPlus_HR/MapServer>`__
+via RESTful service,
+`National Wetlands Inventory <https://www.fws.gov/wetlands/>`__ from WMS, and
+`FEMA National Flood Hazard <https://www.fema.gov/national-flood-hazard-layer-nfhl>`__
+via WFS. The output for these functions are of type ``requests.Response`` that
+can be converted to ``GeoDataFrame`` or ``xarray.Dataset`` using
+`PyGeoUtils <https://github.com/cheginit/pygeoutils>`__.
+
+Let's start the National Map's NHDPlus HR web service. We can query the flowlines that are
+within a geometry as follows:
+
+.. code-block:: python
+
+    from pygeoogc import ArcGISRESTful, WFS, WMS, ServiceURL
+    import pygeoutils as geoutils
+    from pynhd import NLDI
+
+    basin_geom = NLDI().get_basins("01031500").geometry[0]
+
+    hr = ArcGISRESTful(ServiceURL().restful.nhdplushr, outformat="json")
+    hr.layer = 2
+
+    hr.oids_bygeom(basin_geom, "epsg:4326")
+    resp = hr.get_features()
+    flowlines = geoutils.json2geodf(resp)
+
+Note ``oids_bygeom`` has an additional argument for passing any valid SQL WHERE clause
+to further filter the data on the server side.
+
+We can also submit a query based on IDs of any valid field in the database. If the measure
+property is desired you can pass ``return_m`` as ``True`` to the ``get_features`` class method:
+
+.. code-block:: python
+
+    hr.oids_byfield("PERMANENT_IDENTIFIER", ["103455178", "103454362", "103453218"])
+    resp = hr.get_features(return_m=True)
+    flowlines = geoutils.json2geodf(resp)
+
+Additionally, any valid SQL 92 WHERE clause can be used. For more details look
+`here <https://developers.arcgis.com/rest/services-reference/query-feature-service-.htm#ESRI_SECTION2_07DD2C5127674F6A814CE6C07D39AD46>`__.
+
+.. code-block:: python
+
+    hr.oids_bysql("PERMANENT_IDENTIFIER IN ('103455178', '103454362', '103453218')")
+    resp = hr.get_features()
+    flowlines = geoutils.json2geodf(resp)
+
+A WMS-based example is shown below:
+
+.. code-block:: python
+
+    wms = WMS(
+        ServiceURL().wms.fws,
+        layers="0",
+        outformat="image/tiff",
+        crs="epsg:3857",
+    )
+    r_dict = wms.getmap_bybox(
+        basin_geom.bounds,
+        1e3,
+        box_crs="epsg:4326",
+    )
+    wetlands = geoutils.gtiff2xarray(r_dict, basin_geom, "epsg:4326")
+
+Query from a WFS-based web service can be done either within a bounding box or using
+any valid `CQL filter <https://docs.geoserver.org/stable/en/user/tutorials/cql/cql_tutorial.html>`__.
+
+.. code-block:: python
+
+    wfs = WFS(
+        ServiceURL().wfs.fema,
+        layer="public_NFHL:Base_Flood_Elevations",
+        outformat="esrigeojson",
+        crs="epsg:4269",
+    )
+    r = wfs.getfeature_bybox(basin_geom.bounds, box_crs="epsg:4326")
+    flood = geoutils.json2geodf(r.json(), "epsg:4269", "epsg:4326")
+
+    layer = "wmadata:huc08"
+    wfs = WFS(
+        ServiceURL().wfs.waterdata,
+        layer=layer,
+        outformat="application/json",
+        version="2.0.0",
+        crs="epsg:4269",
+    )
+    r = wfs.getfeature_byfilter(f"huc8 LIKE '13030%'")
+    huc8 = geoutils.json2geodf(r.json(), "epsg:4269", "epsg:4326")
+
+PyGeoOGC, has a function for asynchronous download which can help speed up sending/receiveing requests. For example, let's use this function to get `NDVI <https://daac.ornl.gov/VEGETATION/guides/US_MODIS_NDVI.html>`_ data from DACC server. The function can be directly passed to ``xarray.open_mfdataset`` to get the data as an xarray Dataset.
+
+.. code-block:: python
+
+    import xarray as xr
+    import pygeoogc as ogc
+    from datetime import datetime
+
+    west, south, east, north = basin_geom.bounds
+    base_url = "https://thredds.daac.ornl.gov/thredds/ncss/ornldaac/1299"
+    urls = []
+    dates_itr = [(datetime(y, 1, 1), datetime(y, 1, 31)) for y in range(2000, 2005)]
+    urls = (
+        (
+            f"{base_url}/MCD13.A{s.year}.unaccum.nc4",
+            {
+                "var": "NDVI",
+                "north": f"{north}",
+                "west": f"{west}",
+                "east": f"{east}",
+                "south": f"{south}",
+                "disableProjSubset": "on",
+                "horizStride": "1",
+                "time_start": s.strftime("%Y-%m-%dT%H:%M:%SZ"),
+                "time_end": e.strftime("%Y-%m-%dT%H:%M:%SZ"),
+                "timeStride": "1",
+                "addLatLon": "true",
+                "accept": "netcdf",
+            },
+        )
+        for s, e in dates_itr
+    )
+    data = xr.open_mfdataset(ogc.async_requests(urls, "binary", max_workers=8))
+
+Contributing
+------------
+
+Contributions are appreciated and very welcomed. Please read
+`CONTRIBUTING.rst <https://github.com/cheginit/pygeoogc/blob/master/CONTRIBUTING.rst>`__
+for instructions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygeoogc-0.2.2/docs/Makefile` & `pygeoogc-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/docs/conf.py` & `pygeoogc-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/docs/make.bat` & `pygeoogc-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/docs/pygeoogc.rst` & `pygeoogc-0.9.0/docs/pygeoogc.rst`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/pygeoogc/__init__.py` & `pygeoogc-0.9.0/pygeoogc/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Top-level package for PyGeoOGC."""
+import asyncio
+import sys
+
 from pkg_resources import DistributionNotFound, get_distribution
 
 from .exceptions import (
     InvalidInputType,
     InvalidInputValue,
     MissingInputs,
     ServerError,
@@ -14,7 +17,10 @@
 from .utils import RetrySession, async_requests
 
 try:
     __version__ = get_distribution(__name__).version
 except DistributionNotFound:
     # package is not installed
     pass
+
+if sys.platform.startswith("win"):
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
```

### Comparing `pygeoogc-0.2.2/pygeoogc/core.py` & `pygeoogc-0.9.0/pygeoogc/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Base classes and function for REST, WMS, and WMF services."""
 from dataclasses import dataclass
-from itertools import zip_longest
 from typing import Dict, List, Optional, Tuple, Union
 
+import cytoolz as tlz
 import pyproj
 from orjson import JSONDecodeError
 from owslib.wfs import WebFeatureService
 from owslib.wms import WebMapService
 
 from . import utils
 from .exceptions import InvalidInputType, InvalidInputValue, MissingInputs, ServerError, ZeroMatched
@@ -75,15 +75,14 @@
     def layer(self, value: int) -> None:
         try:
             existing_lyr = int(self.base_url.split("/")[-1])
             self.base_url = self.base_url.replace(f"/{existing_lyr}", "")
         except ValueError:
             pass
 
-        self.valid_layers = self.get_validlayers()
         if value not in self.valid_layers:
             valids = [f'"{i}" for {n}' for i, n in self.valid_layers.items()]
             raise InvalidInputValue("layer", valids)
 
         self._layer = f"{value}"
         try:
             existing_lyr = int(self.base_url.split("/")[-1])
@@ -132,14 +131,56 @@
     @outfields.setter
     def outfields(self, value: Union[List[str], str]) -> None:
         if not isinstance(value, (list, str)):
             raise InvalidInputType("outfields", "str or list")
 
         self._outfields = value if isinstance(value, list) else [value]
 
+    @property
+    def n_threads(self) -> int:
+        return self._n_threads
+
+    @n_threads.setter
+    def n_threads(self, value: int) -> None:
+        if not isinstance(value, int) or value < 0:
+            raise InvalidInputType("n_threads", "positive int")
+        self._n_threads = value
+
+    @property
+    def max_nrecords(self) -> int:
+        return self._max_nrecords
+
+    @max_nrecords.setter
+    def max_nrecords(self, value: int) -> None:
+        if value > self.max_nrecords:
+            raise ValueError(
+                f"The server doesn't accept more than {self.max_nrecords}" + " records per request."
+            )
+        if value < 0:
+            raise InvalidInputType("max_nrecords", "positive int")
+
+        self._max_nrecords = value
+
+    @property
+    def featureids(self) -> List[Tuple[str, ...]]:
+        return self._featureids
+
+    @featureids.setter
+    def featureids(self, value: Union[List[int], int]) -> None:
+        if not isinstance(value, (list, int)):
+            raise InvalidInputType("featureids", "int or list")
+
+        oids = [str(value)] if isinstance(value, (int, str)) else [str(v) for v in value]
+
+        self.nfeatures = len(oids)
+        if self.nfeatures == 0:
+            raise ZeroMatched(self._zeromatched)
+
+        self._featureids = list(tlz.partition_all(self.max_nrecords, oids))
+
     def get_validlayers(self) -> Dict[str, str]:
         try:
             existing_lyr = int(self.base_url.split("/")[-1])
             url = self.base_url.replace(f"/{existing_lyr}", "")
         except ValueError:
             url = self.base_url
 
@@ -162,80 +203,45 @@
         """Test the generated url and get the required parameters from the service."""
         try:
             resp = self.session.get(self.base_url, {"f": "json"}).json()
             try:
                 self.units = resp["units"].replace("esri", "").lower()
             except KeyError:
                 self.units = None
-            self.maxrec_ount = resp["maxRecordCount"]
+            self._max_nrecords = int(resp["maxRecordCount"])
             self.query_formats = resp["supportedQueryFormats"].replace(" ", "").lower().split(",")
             self.valid_fields = list(
                 set(
                     utils.traverse_json(resp, ["fields", "name"])
                     + utils.traverse_json(resp, ["fields", "alias"])
                     + ["*"]
                 )
             )
+            try:
+                extent = resp["extent"] if "extent" in resp else resp["fullExtent"]
+                bounds = (extent["xmin"], extent["ymin"], extent["xmax"], extent["ymax"])
+                crs = extent["spatialReference"]["latestWkid"]
+                self.extent = utils.MatchCRS.bounds(bounds, crs, DEF_CRS)
+            except KeyError:
+                self.extent = None
         except KeyError:
             raise ServerError(self.base_url)
 
-        self._max_nrecords = self.maxrec_ount
-
-    @property
-    def n_threads(self) -> int:
-        return self._n_threads
-
-    @n_threads.setter
-    def n_threads(self, value: int) -> None:
-        if not isinstance(value, int) or value < 0:
-            raise InvalidInputType("n_threads", "positive int")
-        self._n_threads = value
-
-    @property
-    def max_nrecords(self) -> int:
-        return self._max_nrecords
-
-    @max_nrecords.setter
-    def max_nrecords(self, value: int) -> None:
-        if value > self.maxrec_ount:
-            raise ValueError(
-                f"The server doesn't accept more than {self.maxrec_ount}" + " records per request."
-            )
-        if value > 0:
-            self._max_nrecords = value
-        else:
-            raise InvalidInputType("max_nrecords", "positive int")
-
-    @property
-    def featureids(self) -> List[Tuple[str, ...]]:
-        return self._featureids
-
-    @featureids.setter
-    def featureids(self, value: Union[List[int], int]) -> None:
-        if not isinstance(value, (list, int)):
-            raise InvalidInputType("featureids", "int or list")
-
-        oids = [str(value)] if isinstance(value, int) else [str(v) for v in value]
-
-        self.nfeatures = len(oids)
-        if self.nfeatures == 0:
-            raise ZeroMatched(self._zeromatched)
-
-        oid_list = list(zip_longest(*[iter(oids)] * self.max_nrecords))
-        oid_list[-1] = tuple(i for i in oid_list[-1] if i is not None)
-        self._featureids = oid_list
-
     def __repr__(self) -> str:
         """Print the service configuration."""
-        return (
-            "Service configurations:\n"
-            + f"URL: {self.base_url}\n"
-            + f"Max Record Count: {self.maxrec_ount}\n"
-            + f"Supported Query Formats: {self.query_formats}\n"
-            + f"Units: {self.units}"
+        extent = ", ".join(f"{c:.3f}" for c in self.extent) if self.extent else None
+        return "\n".join(
+            [
+                "Service configurations:",
+                f"URL: {self.base_url}",
+                f"Max Record Count: {self.max_nrecords}",
+                f"Supported Query Formats: {self.query_formats}",
+                f"Units: {self.units}",
+                f"Extent: ({extent})",
+            ]
         )
 
 
 @dataclass
 class WMSBase:
     """Base class for accessing a WMS service.
 
@@ -338,15 +344,15 @@
             + f"URL: {self.url}\n"
             + f"Version: {self.version}\n"
             + f"Layer: {self.layer}\n"
             + f"Output Format: {self.outformat}\n"
             + f"Output CRS: {self.crs}"
         )
 
-    def validate_wfs(self):
+    def validate_wfs(self) -> None:
         """Validate input arguments with the WFS service."""
         wfs = WebFeatureService(self.url, version=self.version)
 
         valid_layers = list(wfs.contents)
         if self.layer is None:
             raise MissingInputs(
                 "The layer argument is missing."
```

### Comparing `pygeoogc-0.2.2/pygeoogc/exceptions.py` & `pygeoogc-0.9.0/pygeoogc/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Parameters
     ----------
     url : str
         The server url
     """
 
     def __init__(self, url: str) -> None:
-        self.message = f"The requested server is no available in the URL:\n{url}"
+        self.message = f"The requested server is no available at:\n{url}"
         super().__init__(self.message)
 
     def __str__(self) -> str:
         return self.message
 
 
 class ThreadingException(Exception):
```

### Comparing `pygeoogc-0.2.2/pygeoogc/print_versions.py` & `pygeoogc-0.9.0/pygeoogc/print_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 import importlib
 import locale
 import os
 import platform
 import struct
 import subprocess
 import sys
+from typing import IO, List, Optional, Tuple
 
 
-def get_sys_info():
+def get_sys_info() -> List[Tuple[str, Optional[str]]]:
     """Return system information as a dict.
 
     From https://github.com/numpy/numpy/blob/master/setup.py#L64-L89
     """
     blob = []
 
-    def _minimal_ext_cmd(cmd):
+    def _minimal_ext_cmd(cmd: List[str]) -> bytes:
         # construct minimal environment
         env = {}
         for k in ["SYSTEMROOT", "PATH", "HOME"]:
             v = os.environ.get(k)
             if v is not None:
                 env[k] = v
         # LANGUAGE is used on win32
@@ -38,34 +39,34 @@
         out = _minimal_ext_cmd(["git", "rev-parse", "HEAD"])
         commit = out.strip().decode("ascii")
     except (subprocess.SubprocessError, OSError):
         pass
 
     blob.append(("commit", commit))
 
-    (sysname, _nodename, release, _version, machine, processor) = platform.uname()
+    (sysname, _, release, _, machine, processor) = platform.uname()
     blob.extend(
         [
             ("python", sys.version),
-            ("python-bits", struct.calcsize("P") * 8),
+            ("python-bits", f"{struct.calcsize('P') * 8}"),
             ("OS", f"{sysname}"),
             ("OS-release", f"{release}"),
             ("machine", f"{machine}"),
             ("processor", f"{processor}"),
             ("byteorder", f"{sys.byteorder}"),
             ("LC_ALL", f'{os.environ.get("LC_ALL", "None")}'),
             ("LANG", f'{os.environ.get("LANG", "None")}'),
             ("LOCALE", ".".join(str(i) for i in locale.getlocale())),
         ]
     )
 
     return blob
 
 
-def netcdf_and_hdf5_versions():
+def netcdf_and_hdf5_versions() -> List[Tuple[str, Optional[str]]]:
     """Get netcdf and hdf5 versions."""
     libhdf5_version = None
     libnetcdf_version = None
     try:
         import netCDF4
 
         libhdf5_version = netCDF4.__hdf5libversion__
@@ -76,15 +77,15 @@
 
             libhdf5_version = h5py.version.hdf5_version
         except ImportError:
             pass
     return [("libhdf5", libhdf5_version), ("libnetcdf", libnetcdf_version)]
 
 
-def show_versions(file=sys.stdout):
+def show_versions(file: IO = sys.stdout) -> None:
     """Print the versions of hydrodata stack and its dependencies.
 
     Parameters
     ----------
     file : file-like, optional
         print to the given file-like object. Defaults to sys.stdout.
     """
@@ -129,15 +130,15 @@
         ("conda", lambda mod: mod.__version__),
         ("pytest", lambda mod: mod.__version__),
         # Misc.
         ("IPython", lambda mod: mod.__version__),
         ("sphinx", lambda mod: mod.__version__),
     ]
 
-    deps_blob = []
+    deps_blob: List[Tuple[str, Optional[str]]] = []
     for (modname, ver_f) in deps:
         try:
             if modname in sys.modules:
                 mod = sys.modules[modname]
             else:
                 mod = importlib.import_module(modname)
         except ModuleNotFoundError:
```

### Comparing `pygeoogc-0.2.2/pygeoogc/pygeoogc.py` & `pygeoogc-0.9.0/pygeoogc/pygeoogc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Base classes and function for REST, WMS, and WMF services."""
-from collections import defaultdict, namedtuple
+from collections import defaultdict
 from itertools import product
 from pathlib import Path
+from types import SimpleNamespace
 from typing import Any, Dict, List, Optional, Tuple, Union
 from warnings import warn
 
 import pyproj
 import shapely.ops as ops
 import yaml
-from orjson import JSONDecodeError
 from requests import Response
-from shapely.geometry import MultiPolygon, Polygon
+from shapely.geometry import MultiPoint, MultiPolygon, Point, Polygon
+from simplejson import JSONDecodeError
 
 from . import utils
 from .core import ArcGISRESTfulBase, WFSBase, WMSBase
 from .exceptions import InvalidInputType, InvalidInputValue, ZeroMatched
 from .utils import MatchCRS, RetrySession
 
 DEF_CRS = "epsg:4326"
@@ -44,70 +45,98 @@
         that some services might face issues when several requests are sent
         simultaniously and will return the requests partially. It's recommended
         to avoid performing threading unless you are certain the web service can handle it.
     """
 
     def oids_bygeom(
         self,
-        geom: Union[Polygon, Tuple[float, float, float, float]],
+        geom: Union[
+            Polygon,
+            Point,
+            MultiPoint,
+            Tuple[float, float],
+            List[Tuple[float, float]],
+            Tuple[float, float, float, float],
+        ],
         geo_crs: str = DEF_CRS,
         sql_clause: str = "",
+        distance: Optional[int] = None,
     ) -> None:
         """Get feature IDs within a geometry that can be combined with a SQL where clause.
 
         Parameters
         ----------
-        geom : Polygon or tuple
-            A geometry (Polgon) or bounding box (tuple of length 4).
+        geom : Polygon, Point, MultiPoint, tuple, or list of tuples
+            A geometry (Polygon, Point, MultiPoint), tuple of length 2 (x, y),
+            a list of tuples of length 2 [(x, y), ...], or bounding box (tuple of length 4).
         geo_crs : str
-            The spatial reference of the input geometry, defaults to EPSG:4326
+            The spatial reference of the input geometry, defaults to EPSG:4326.
         sql_clause : str, optional
-            A valid SQL 92 WHERE clause, default to an empty string i.e., no
+            A valid SQL 92 WHERE clause, default to an empty string.
+        distance : int, optional
+            The buffer distance for the input geometries in meters, default to None.
         """
         if not isinstance(sql_clause, str):
             raise InvalidInputType("sql_clause", str)
 
-        if isinstance(geom, tuple):
+        if isinstance(geom, tuple) and len(geom) == 2:
+            geom = Point(geom)
+        elif isinstance(geom, list) and all(len(g) == 2 for g in geom):
+            geom = MultiPoint(geom)
+
+        geom_query = None
+        if isinstance(geom, tuple) and len(geom) == 4:
             geom = MatchCRS.bounds(geom, geo_crs, self.crs)  # type: ignore
             geom_query = utils.ESRIGeomQuery(geom, self.out_sr).bbox()
+        elif isinstance(geom, Point):
+            geom = MatchCRS.geometry(geom, geo_crs, self.crs)
+            geom_query = utils.ESRIGeomQuery((geom.x, geom.y), self.out_sr).point()
+        elif isinstance(geom, MultiPoint):
+            geom = MatchCRS.geometry(geom, geo_crs, self.crs)
+            geom_query = utils.ESRIGeomQuery([(g.x, g.y) for g in geom], self.out_sr).multipoint()
         elif isinstance(geom, Polygon):
             geom = MatchCRS.geometry(geom, geo_crs, self.crs)
             geom_query = utils.ESRIGeomQuery(geom, self.out_sr).polygon()
-        else:
-            raise InvalidInputType("geom", "tuple or Polgon")
+
+        if geom_query is None:
+            raise InvalidInputType("geom", "Polygon, Point, MultiPoint, tuple, or list of tuples")
 
         payload = {
             **geom_query,  # type: ignore
             "spatialRel": self.spatial_relation,
             "returnGeometry": "false",
             "returnIdsOnly": "true",
             "f": self.outformat,
         }
+        if distance:
+            payload["distance"] = f"{distance}"
+            payload["units"] = "esriSRUnit_Meter"
 
         if len(sql_clause) > 0:
             payload.update({"where": sql_clause})
 
         resp = self.session.post(f"{self.base_url}/query", payload)
 
         try:
-            self.featureids = resp.json()["objectIds"]
+            r_json = resp.json()["objectIds"]
+            if r_json is None:
+                raise ZeroMatched(self._zeromatched)
+            self.featureids = r_json
         except (KeyError, TypeError, IndexError, JSONDecodeError):
             raise ZeroMatched(self._zeromatched)
 
-    def oids_byfield(self, field: str, ids: Union[str, List[str]], return_m: bool = False) -> None:
+    def oids_byfield(self, field: str, ids: Union[str, List[str]]) -> None:
         """Get Object IDs based on a list of field IDs.
 
         Parameters
         ----------
         field : str
             Name of the target field that IDs belong to.
         ids : str or list
             A list of target ID(s).
-        return_m : bool
-            Whether to activate the Return M (measure) in the request, defaults to False.
 
         Returns
         -------
         geopandas.GeoDataFrame
             The requested features as a GeoDataFrame.
         """
         valid_fields = self.get_validfields()
@@ -143,15 +172,18 @@
             "returnGeometry": "false",
             "returnIdsOnly": "true",
             "f": self.outformat,
         }
         resp = self.session.post(f"{self.base_url}/query", payload)
 
         try:
-            self.featureids = resp.json()["objectIds"]
+            r_json = resp.json()["objectIds"]
+            if r_json is None:
+                raise ZeroMatched(self._zeromatched)
+            self.featureids = r_json
         except (KeyError, TypeError, IndexError, JSONDecodeError):
             raise ZeroMatched(self._zeromatched)
 
     def get_features(self, return_m: bool = False) -> List[Dict[str, Any]]:
         """Get features based on the feature IDs.
 
         Parameters
@@ -171,18 +203,18 @@
             "returnGeometry": "true",
             "outSR": self.out_sr,
             "outfields": ",".join(self.outfields),
             "ReturnM": return_m,
             "f": self.outformat,
         }
 
-        def getter(ids: Tuple[str, ...]) -> Union[Response, Tuple[str, ...]]:
+        def getter(ids: Tuple[str, ...]) -> Union[Dict[str, Any], Tuple[str, ...]]:
             payload.update({"objectIds": ", ".join(ids)})
             resp = self.session.post(f"{self.base_url}/query", payload)
-            r_json = resp.json()
+            r_json: Dict[str, Any] = resp.json()
             try:
                 if "error" in r_json:
                     return ids
 
                 return r_json
             except AssertionError:
                 if self.outformat == "geojson":
@@ -311,24 +343,26 @@
             payload["srs"] = self.crs
 
         else:
             payload["crs"] = self.crs
 
         geographic_crs = pyproj.CRS.from_user_input(self.crs).is_geographic
 
-        def _getmap(args):
+        def _getmap(
+            args: Tuple[str, Tuple[Tuple[float, float, float, float], str, int, int]]
+        ) -> Tuple[str, bytes]:
             lyr, bnds = args
             _bbox, counter, _width, _height = bnds
 
             if self.version != "1.1.1" and geographic_crs and not always_xy:
                 _bbox = (_bbox[1], _bbox[0], _bbox[3], _bbox[2])
 
             payload["bbox"] = f'{",".join(str(c) for c in _bbox)}'
-            payload["width"] = _width
-            payload["height"] = _height
+            payload["width"] = str(_width)
+            payload["height"] = str(_height)
             payload["layers"] = lyr
             resp = self.session.get(self.url, payload)
             return f"{lyr}_dd_{counter}", resp.content
 
         return dict(_getmap(i) for i in product(self.layers, bounds))
 
 
@@ -443,15 +477,15 @@
             order from xy to yx, following the latest WFS version specifications but some don't.
             If the returned value does not have any geometry, it indicates that most probably the
             axis order does not match. You can set this to True in that case.
         predicate : str, optional
             The geometric prediacte to use for requesting the data, defaults to
             INTERSECTS. Valid predicates are:
             EQUALS, DISJOINT, INTERSECTS, TOUCHES, CROSSES, WITHIN, CONTAINS,
-            OVERLAPS, RELATE, DWITHIN, BEYOND
+            OVERLAPS, RELATE, BEYOND
 
         Returns
         -------
         requests.Response
             WFS query response based on the given geometry.
         """
         geom = MatchCRS().geometry(geometry, geo_crs, self.crs)
@@ -471,15 +505,14 @@
             "INTERSECTS",
             "TOUCHES",
             "CROSSES",
             "WITHIN",
             "CONTAINS",
             "OVERLAPS",
             "RELATE",
-            "DWITHIN",
             "BEYOND",
         ]
         if predicate not in valid_predicates:
             raise InvalidInputValue("predicate", valid_predicates)
 
         return self.getfeature_byfilter(f"{predicate.upper()}(the_geom, {g_wkt})", method="POST")
 
@@ -538,14 +571,18 @@
         -------
         requests.Response
             WFS query response
         """
         if not isinstance(cql_filter, str):
             raise InvalidInputType("cql_filter", "str")
 
+        valid_methods = ["GET", "POST"]
+        if method not in valid_methods:
+            raise InvalidInputValue("method", valid_methods)
+
         payload = {
             "service": "wfs",
             "version": self.version,
             "outputFormat": self.outformat,
             "request": "GetFeature",
             "typeName": self.layer,
             "srsName": self.crs,
@@ -553,41 +590,39 @@
         }
 
         if method == "GET":
             resp = self.session.get(self.url, payload)
         elif method == "POST":
             headers = {"content-type": "application/x-www-form-urlencoded"}
             resp = self.session.post(self.url, payload, headers)
-        else:
-            raise InvalidInputValue("method", ["GET", "POST"])
 
         utils.check_response(resp)
 
         return resp
 
 
 class ServiceURL:
     """Base URLs of the supported services."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         fpath = Path(__file__).parent.joinpath("static/urls.yml")
         with open(fpath) as fp:
             self.urls = yaml.safe_load(fp)
 
-    def _make_nt(self, service):
-        return namedtuple(service, self.urls[service].keys())(*self.urls[service].values())
+    def _make_nt(self, service: str) -> SimpleNamespace:
+        return SimpleNamespace(**self.urls[service])
 
     @property
-    def restful(self):
+    def restful(self) -> SimpleNamespace:
         return self._make_nt("restful")
 
     @property
-    def wms(self):
+    def wms(self) -> SimpleNamespace:
         return self._make_nt("wms")
 
     @property
-    def wfs(self):
+    def wfs(self) -> SimpleNamespace:
         return self._make_nt("wfs")
 
     @property
-    def http(self):
+    def http(self) -> SimpleNamespace:
         return self._make_nt("http")
```

### Comparing `pygeoogc-0.2.2/pygeoogc/static/urls.yml` & `pygeoogc-0.9.0/pygeoogc/static/urls.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 http:
   ssebopeta: https://edcintl.cr.usgs.gov/downloads/sciweb1/shared/uswem/web/conus/eta/modis_eta/daily/downloads
 
 restful:
-  daymet_grid: https://thredds.daac.ornl.gov/thredds/ncss/ornldaac/1328
+  daymet: https://thredds.daac.ornl.gov/thredds/ncss/ornldaac
   daymet_point: https://daymet.ornl.gov/single-pixel/api/data
   fema: https://hazards.fema.gov/gis/nfhl/rest/services/public/NFHL/MapServer
   fws: https://www.fws.gov/wetlands/arcgis/rest/services
   nldi: https://labs.waterdata.usgs.gov/api/nldi
   nwis: https://waterservices.usgs.gov/nwis
   wbd: https://hydro.nationalmap.gov/arcgis/rest/services/wbd/MapServer
-  nhdhr: https://edits.nationalmap.gov/arcgis/rest/services/HEM/NHDHigh/MapServer
+  nhd: https://hydro.nationalmap.gov/arcgis/rest/services/nhd/MapServer
   nhdplushr: https://hydro.nationalmap.gov/arcgis/rest/services/NHDPlus_HR/MapServer
+  nhdhr_edits: https://edits.nationalmap.gov/arcgis/rest/services/HEM/NHDHigh/MapServer
+  nhdplushr_edits: https://edits.nationalmap.gov/arcgis/rest/services/NHDPlus_HR/NHDPlus_HR/MapServer
+  nhdplus_epa: https://watersgeo.epa.gov/arcgis/rest/services/NHDPlus/NHDPlus/MapServer
+  nhd_fabric: https://watersgeo.epa.gov/arcgis/rest/services/Support/CatchmentFabric/MapServer
+  airmap: https://api.airmap.com/elevation/v1/ele
 
 wfs:
   fema: https://hazards.fema.gov/gis/nfhl/services/public/NFHL/MapServer/WFSServer
   waterdata: https://labs.waterdata.usgs.gov/geoserver/wmadata/ows
 
 wms:
   fema: https://hazards.fema.gov/gis/nfhl/rest/services/public/NFHLWMS/MapServer/WMSServer
```

### Comparing `pygeoogc-0.2.2/pygeoogc/utils.py` & `pygeoogc-0.9.0/pygeoogc/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Some utilities for PyGeoOGC."""
 import asyncio
 import socket
 from concurrent import futures
 from dataclasses import dataclass
-from itertools import zip_longest
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Mapping,
@@ -15,24 +14,25 @@
     Optional,
     Tuple,
     Union,
 )
 from unittest.mock import _patch, patch
 
 import aiohttp
+import cytoolz as tlz
 import nest_asyncio
 import numpy as np
 import orjson as json
 import pyproj
 from defusedxml import cElementTree as etree
 from requests import Response, Session
 from requests.adapters import HTTPAdapter
 from requests.exceptions import RequestException
-from shapely.geometry import LineString, MultiPolygon, Point, Polygon, box
-from shapely.ops import transform
+from shapely import ops
+from shapely.geometry import LineString, MultiPoint, MultiPolygon, Point, Polygon, box
 from urllib3 import Retry
 
 from .exceptions import InvalidInputType, InvalidInputValue, ThreadingException, ZeroMatched
 
 nest_asyncio.apply()
 DEF_CRS = "epsg:4326"
 BOX_ORD = "(west, south, east, north)"
@@ -63,22 +63,27 @@
         backoff_factor: float = 0.3,
         status_to_retry: Tuple[int, ...] = (500, 502, 504),
         prefixes: Tuple[str, ...] = ("https://",),
     ) -> None:
         self.session = Session()
         self.retries = retries
 
-        r = Retry(
-            total=retries,
-            read=retries,
-            connect=retries,
-            backoff_factor=backoff_factor,
-            status_forcelist=status_to_retry,
-            method_whitelist=False,
-        )
+        retry_args = {
+            "total": retries,
+            "read": retries,
+            "connect": retries,
+            "backoff_factor": backoff_factor,
+            "status_forcelist": status_to_retry,
+        }
+        if hasattr(Retry.DEFAULT, "allowed_methods"):
+            retry_args.update({"allowed_methods": False})
+        else:
+            retry_args.update({"method_whitelist": False})
+
+        r = Retry(**retry_args)
         adapter = HTTPAdapter(max_retries=r)
         for prefix in prefixes:
             self.session.mount(prefix, adapter)
         self.session.hooks = {"response": [lambda r, *args, **kwargs: r.raise_for_status()]}
 
     def get(
         self,
@@ -105,15 +110,30 @@
             raise ConnectionError(f"Connection failed after {self.retries} retries.")
 
     @staticmethod
     def onlyipv4() -> _patch:
         """Disable IPv6 and only use IPv4."""
         orig_getaddrinfo = socket.getaddrinfo
 
-        def getaddrinfo_ipv4(host, port, family=socket.AF_INET, ptype=0, proto=0, flags=0):
+        def getaddrinfo_ipv4(
+            host: str,
+            port: str,
+            family: socket.AddressFamily = socket.AF_INET,
+            ptype: int = 0,
+            proto: int = 0,
+            flags: int = 0,
+        ) -> List[
+            Tuple[
+                socket.AddressFamily,
+                socket.SocketKind,
+                int,
+                str,
+                Union[Tuple[str, int], Tuple[str, int, int, int]],
+            ]
+        ]:
             return orig_getaddrinfo(
                 host=host,
                 port=port,
                 family=family,
                 type=ptype,
                 proto=proto,
                 flags=flags,
@@ -140,15 +160,15 @@
 
     Returns
     -------
     bytes
         The retrieved response as binary
     """
     async with session_req(url, **payload) as response:
-        return await response.read()
+        return await response.read()  # type: ignore
 
 
 async def _request_json(
     url: str,
     session_req: aiohttp.ClientSession,
     payload: Dict[str, Optional[MutableMapping[str, Any]]],
 ) -> MutableMapping[str, Any]:
@@ -165,15 +185,15 @@
 
     Returns
     -------
     dict
         The retrieved response as json
     """
     async with session_req(url, **payload) as response:
-        return await response.json()
+        return await response.json()  # type: ignore
 
 
 async def _request_text(
     url: str,
     session_req: aiohttp.ClientSession,
     payload: Dict[str, Optional[MutableMapping[str, Any]]],
 ) -> str:
@@ -190,15 +210,15 @@
 
     Returns
     -------
     dict
         The retrieved response as string
     """
     async with session_req(url, **payload) as response:
-        return await response.text()
+        return await response.text()  # type: ignore
 
 
 async def _async_session(
     url_payload: Tuple[Tuple[str, Optional[MutableMapping[str, Any]]], ...],
     read: str,
     request: str,
 ) -> Callable:
@@ -232,58 +252,48 @@
             read_method[read](u, request_method[request], {paylod[request]: p})
             for u, p in url_payload
         )
         return await asyncio.gather(*tasks, return_exceptions=True)  # type: ignore
 
 
 def async_requests(
-    urls: Union[List[str], Dict[str, Optional[MutableMapping[str, Any]]]],
+    url_payload: List[Tuple[str, Optional[MutableMapping[str, Any]]]],
     read: str,
     request: str = "GET",
     max_workers: int = 8,
 ) -> List[Union[str, MutableMapping[str, Any], bytes]]:
     """Send async requests.
 
     This function is based on
     `this <https://github.com/HydrologicEngineeringCenter/data-retrieval-scripts/blob/master/qpe_async_download.py>`__
     script.
 
     Parameters
     ----------
-    urls : list of str or dict of str and dict
-        A list of URLs or URLs with their payloads to be retrieved.
+    url_payload : list of tuples
+        A list of URLs and payloads as a tuple.
     read : str
         The method for returning the request; binary, json, and text.
     request : str, optional
         The request type; GET or POST, defaults to GET.
     max_workers : int, optional
         The maximum number of async processes, defaults to 8.
 
     Returns
     -------
     list
         A list of responses
     """
-    import sys
-
-    if not isinstance(urls, list) and not isinstance(urls, dict):
-        raise InvalidInputType("urls", "list of urls or dict of urls and payloads")
-
-    url_payload = urls if isinstance(urls, dict) else {u: None for u in urls}
-    chunked_urls = list(zip_longest(*[iter(url_payload.items())] * max_workers))
-    chunked_urls[-1] = tuple(i for i in chunked_urls[-1] if i is not None)
+    chunked_urls = tlz.partition_all(max_workers, url_payload)
 
     results: List[Union[str, MutableMapping[str, Any], bytes]] = []
     for chunk in chunked_urls:
-        if sys.platform.startswith("win"):
-            asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
         loop = asyncio.get_event_loop()
         results.append(loop.run_until_complete(_async_session(chunk, read, request)))  # type: ignore
-        del loop
-    return [x for y in results for x in y]  # type: ignore
+    return list(tlz.concat(results))
 
 
 def threading(
     func: Callable,
     iter_list: Iterable,
     param_list: Optional[List[Any]] = None,
     max_workers: int = 8,
@@ -314,15 +324,15 @@
     param_list = [] if param_list is None else param_list
     with futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
         future_to_itr = {executor.submit(func, itr, *param_list): itr for itr in iter_list}
         for future in futures.as_completed(future_to_itr):
             itr = future_to_itr[future]
             try:
                 data.append(future.result())
-            except Exception as exc:
+            except Exception as exc:  # noqa: B902
                 raise ThreadingException(itr, exc)
     return data
 
 
 def traverse_json(
     obj: Union[Dict[str, Any], List[Dict[str, Any]]], path: Union[str, List[str]]
 ) -> List[Any]:
@@ -339,15 +349,20 @@
 
     Returns
     -------
     list
         The items founds in the JSON
     """
 
-    def extract(obj, path, ind, arr):
+    def extract(
+        obj: Optional[Union[List[Any], Dict[str, Any]]],
+        path: Union[str, List[str]],
+        ind: int,
+        arr: List[Any],
+    ) -> List[Any]:
         key = path[ind]
         if ind + 1 < len(path):
             if isinstance(obj, dict):
                 if key in obj.keys():
                     extract(obj.get(key), path, ind + 1, arr)
                 else:
                     arr.append(None)
@@ -386,39 +401,50 @@
 @dataclass
 class ESRIGeomQuery:
     """Generate input geometry query for ArcGIS RESTful services.
 
     Parameters
     ----------
     geometry : tuple or Polygon
-        The input geometry which can be a point (x, y),
+        The input geometry which can be a point (x, y), a list of points [(x, y), ...],
         bbox (xmin, ymin, xmax, ymax), or a Shapely's Polygon.
     wkid : int
         The Well-known ID (WKID) of the geometry's spatial reference e.g., for EPSG:4326,
         4326 should be passed. Check
         `ArcGIS <https://developers.arcgis.com/rest/services-reference/geographic-coordinate-systems.htm>`__
         for reference.
     """
 
-    geometry: Union[Tuple[float, float], Tuple[float, float, float, float], Polygon]
+    geometry: Union[
+        Tuple[float, float], List[Tuple[float, float]], Tuple[float, float, float, float], Polygon
+    ]
     wkid: int
 
     def point(self) -> Dict[str, Union[str, bytes]]:
         """Query for a point."""
-        if len(self.geometry) != 2:
+        if not isinstance(self.geometry, tuple) and len(self.geometry) != 2:
             raise InvalidInputType("geometry (point)", "tuple", "(x, y)")
 
         geo_type = "esriGeometryPoint"
         geo_json = dict(zip(("x", "y"), self.geometry))
         return self.get_payload(geo_type, geo_json)
 
+    def multipoint(self) -> Dict[str, Union[str, bytes]]:
+        """Query for a multi-point."""
+        if not isinstance(self.geometry, list) and any(len(g) != 2 for g in self.geometry):  # type: ignore
+            raise InvalidInputType("geometry (multi-point)", "list of tuples", "[(x, y), ...]")
+
+        geo_type = "esriGeometryMultipoint"
+        geo_json = {"points": [[x, y] for x, y in self.geometry]}  # type: ignore
+        return self.get_payload(geo_type, geo_json)
+
     def bbox(self) -> Dict[str, Union[str, bytes]]:
         """Query for a bbox."""
-        if len(self.geometry) != 4:
-            raise InvalidInputType("geometry (bbox)", "tuple", BOX_ORD)
+        if not isinstance(self.geometry, (tuple, list)) and len(self.geometry) != 4:
+            raise InvalidInputType("geometry (bbox)", "tuple or list", BOX_ORD)
 
         geo_type = "esriGeometryEnvelope"
         geo_json = dict(zip(("xmin", "ymin", "xmax", "ymax"), self.geometry))
         return self.get_payload(geo_type, geo_json)
 
     def polygon(self) -> Dict[str, Union[str, bytes]]:
         """Query for a polygon."""
@@ -448,30 +474,33 @@
     in_crs : str
         The spatial reference of the input geometry
     out_crs : str
         The target spatial reference
     """
 
     @staticmethod
-    def geometry(geom: Union[Polygon, MultiPolygon], in_crs: str, out_crs: str) -> Polygon:
-        if not isinstance(geom, (Polygon, MultiPolygon)):
-            raise InvalidInputType("geom", "Polygon")
+    def geometry(
+        geom: Union[Polygon, MultiPolygon, Point, MultiPoint], in_crs: str, out_crs: str
+    ) -> Union[Polygon, MultiPolygon, Point, MultiPoint]:
+        if not isinstance(geom, (Polygon, MultiPolygon, Point, MultiPoint)):
+            raise InvalidInputType("geom", "Polygon, MultiPolygon, Point, or MultiPoint")
 
         project = pyproj.Transformer.from_crs(in_crs, out_crs, always_xy=True).transform
-        return transform(project, geom)
+        return ops.transform(project, geom)
 
     @staticmethod
     def bounds(
         geom: Tuple[float, float, float, float], in_crs: str, out_crs: str
     ) -> Tuple[float, float, float, float]:
         if not isinstance(geom, tuple) and len(geom) != 4:
             raise InvalidInputType("geom", "tuple of length 4", BOX_ORD)
 
         project = pyproj.Transformer.from_crs(in_crs, out_crs, always_xy=True).transform
-        return transform(project, box(*geom)).bounds
+        bbox: Tuple[float, float, float, float] = ops.transform(project, box(*geom)).bounds
+        return bbox
 
     @staticmethod
     def coords(
         geom: Tuple[Tuple[float, ...], Tuple[float, ...]], in_crs: str, out_crs: str
     ) -> Tuple[Any, ...]:
         if not isinstance(geom, tuple) and len(geom) != 2:
             raise InvalidInputType("geom", "tuple of length 2", "((xs), (ys))")
@@ -552,20 +581,22 @@
     n_px = width * height
     if n_px < max_px:
         return [(bbox, "0_0", width, height)]
 
     geod = pyproj.Geod(ellps="WGS84")
     west, south, east, north = _bbox
 
-    def directional_split(az: float, origin: float, dest: float, lvl: float, xy: bool, px: int):
+    def directional_split(
+        az: float, origin: float, dest: float, lvl: float, xy: bool, px: int
+    ) -> Tuple[List[Tuple[float, Any]], List[int]]:
         divs = [0]
         mul = 1.0
         coords = []
 
-        def get_args(dst, dx):
+        def get_args(dst: float, dx: float) -> Tuple[float, float, float, float, int]:
             return (dst, lvl, az, dx, 0) if xy else (lvl, dst, az, dx, 1)
 
         while divs[-1] < 1:
             dim = int(np.sqrt(max_px) * mul)
             step = (dim - 1) * resolution
 
             _dest = origin
```

### Comparing `pygeoogc-0.2.2/pygeoogc.egg-info/PKG-INFO` & `pygeoogc-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoogc
-Version: 0.2.2
+Version: 0.9.0
 Summary: An interface to ArcGIS RESTful-, WFS-, and WMS-based services.
 Home-page: https://github.com/cheginit/pygeoogc
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT license
 Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pygeoogc_logo.png
             :target: https://github.com/cheginit/pygeoogc
@@ -89,76 +89,79 @@
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
             :target: https://github.com/pre-commit/pre-commit
             :alt: pre-commit
         
         |
         
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
         Features
         --------
         
         PyGeoOGC is a part of Hydrodata software stack and provides interfaces to web services
         that are based on
         `ArcGIS RESTful <https://en.wikipedia.org/wiki/Representational_state_transfer>`__,
         `WMS <https://en.wikipedia.org/wiki/Web_Map_Service>`__, and
         `WFS <https://en.wikipedia.org/wiki/Web_Feature_Service>`__. It is noted that although
-        all these web service have limits on the number of objects per requests (e.g., 1000
-        objectIDs for RESTful and 8 million pixels for WMS), PyGeoOGC divides the requests into
-        smaller chunks under-the-hood and then merges the returned responses.
+        all these web service have limits on the number of features per requests (e.g., 1000
+        objectIDs for a RESTful request or 8 million pixels for a WMS request), PyGeoOGC divides
+        the requests into smaller chunks under-the-hood and then merges the returned responses.
         
         There is also an inventory of URLs for some of these web services in form of a class called
         ``ServiceURL``. These URLs are in three categories: ``ServiceURL().restful``,
         ``ServiceURL().wms``, and ``ServiceURL().wfs``. These URLs provide you with some examples
         of the services that PyGeoOGC supports. All the URLs are read from a YAML file located
-        `here <pygeoogc/static/urls.yml>`_. If you had success using PyGeoOGC with a web service
+        `here <pygeoogc/static/urls.yml>`_. If you have success using PyGeoOGC with a web service
         please consider adding its URL to this YAML file which is located at ``pygeoogc/static/urls.yml``.
         
         There are three main classes:
         
         * ``ArcGISRESTful``: This class can be instantiated by providing the target layer URL.
           For example, for getting Watershed Boundary Data we can use ``ServiceURL().restful.wbd``.
-          By looking at the web service website
-          (https://hydro.nationalmap.gov/arcgis/rest/services/wbd/MapServer) we see that there are 9
-          layers; 1 for 2-digit HU (Region), 6 for 12-digit HU (Subregion), and so on. We can either
-          pass the base URL or concatenate the target layer number like so
+          By looking at the web service `website <https://hydro.nationalmap.gov/arcgis/rest/services/wbd/MapServer>`_
+          we see that there are 9
+          layers. For example, 1 for 2-digit HU (Region), 6 for 12-digit HU (Subregion), and so on. We can
+          pass the URL to the target layer like this
           ``f"{ServiceURL().restful.wbd}/6"``.
         
-          If you want to change the layer you can simply set the ``layer`` property of the class.
-          Afterward, we can request for the data in two steps. First, get the object IDs using
+          Another option is to pass the base URL, ``ServiceURL().restful.wbd``, then set the ``layer``
+          property of the class.
+          Afterward, we request for the data in two steps. First, we need to get the taget object IDs using
           ``oids_bygeom`` (within a geometry), ``oids_byfield`` (specific field IDs), or ``oids_bysql``
-          (any valid SQL 92 WHERE clause) class methods. Second, get the actual data using ``get_features``
-          class method. The returned response can be converted into a GeoDataFrame using ``json2geodf``
-          function from `PyGeoOGC <https://github.com/cheginit/pygeoutils>`__ package.
+          (any valid SQL 92 WHERE clause) class methods. Then, we can get the target features using
+          ``get_features`` class method. The returned response can be converted into a GeoDataFrame using
+          ``json2geodf`` function from `PyGeoUtils <https://github.com/cheginit/pygeoutils>`__ package.
         
-        * ``WMS``: Instantiation of this class requires at least 3 arguments: service URL, layer(s)
+        * ``WMS``: Instantiation of this class requires at least 3 arguments: service URL, layer
           name(s), and output format. Additionally, target CRS and the web service version can be provided.
-          Upon instantiation, we could use ``getmap_bybox`` method class to get the raster data within a
-          bounding box. The box can be any valid CRS and if it is different from the default EPSG:4326, it
-          should be passed to the function using ``box_crs`` argumnet. The service response can be
-          converted into a ``xarray.Dataset`` using ``gtiff2xarray`` function from PyGeoOGC package.
+          Upon instantiation, we could use ``getmap_bybox`` method class to get the target raster data
+          within a bounding box. The box can be in any valid CRS and if it is different from the default
+          CRS, EPSG:4326, it should be passed using ``box_crs`` argumnet. The service response can be
+          converted into a ``xarray.Dataset`` using ``gtiff2xarray`` function from PyGeoUtils package.
         
-        * ``WFS``: Instantiation of this class is similar to ``WMS`` and the only difference is that
+        * ``WFS``: Instantiation of this class is similar to ``WMS``. The only difference is that
           only one layer name can be passed. Upon instantiation there are three ways to get the data:
         
-          - ``getfeature_bybox``: Get all the features within a bounding box in any valid CRS.
-          - ``getfeature_byid``: Get all the features based on the IDs. Note that two arguments should be
-            provided: ``featurename``, and ``featureids``. You can get a list of valid feature names using
-            ``get_validnames`` class method.
-          - ``getfeature_byfilter``: Get the data based on a valid
+          - ``getfeature_bybox``: Get all the target features within a bounding box in any valid CRS.
+          - ``getfeature_byid``: Get all the target features based on the IDs. Note that two arguments
+            should be provided: ``featurename``, and ``featureids``. You can get a list of valid feature
+            names using ``get_validnames`` class method.
+          - ``getfeature_byfilter``: Get the data based on any valid
             `CQL <https://docs.geoserver.org/latest/en/user/tutorials/cql/cql_tutorial.html>`__ filter.
         
-          You can convert the returned response to a GeoDataFrame using ``json2geodf`` function
-          from PyGeoOGC package.
+          You can convert the returned response of this function to a GeoDataFrame using ``json2geodf``
+          function from PyGeoUtils package.
         
         You can try using PyGeoOGC without installing it on you system by clicking on the binder badge
         below the PyGeoOGC banner. A Jupyter notebook instance with the Hydrodata software stack
         pre-installed will be launched in your web browser and you can start coding!
         
+        Please note that since Hydrodata is in early development stages, while the provided
+        functionaities should be stable, changes in APIs are possible in new releases. But we
+        appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+        
         Moreover, requests for additional functionalities can be submitted via
         `issue tracker <https://github.com/cheginit/pygeoogc/issues>`__.
         
         Installation
         ------------
         
         You can install PyGeoOGC using ``pip``:
@@ -180,30 +183,26 @@
         We can access
         `NHDPlus HR <https://edits.nationalmap.gov/arcgis/rest/services/NHDPlus_HR/NHDPlus_HR/MapServer>`__
         via RESTful service,
         `National Wetlands Inventory <https://www.fws.gov/wetlands/>`__ from WMS, and
         `FEMA National Flood Hazard <https://www.fema.gov/national-flood-hazard-layer-nfhl>`__
         via WFS. The output for these functions are of type ``requests.Response`` that
         can be converted to ``GeoDataFrame`` or ``xarray.Dataset`` using
-        `PyGeoOGC <https://github.com/cheginit/pygeoogc>`__.
+        `PyGeoUtils <https://github.com/cheginit/pygeoutils>`__.
         
         Let's start the National Map's NHDPlus HR web service. We can query the flowlines that are
         within a geometry as follows:
         
         .. code-block:: python
         
             from pygeoogc import ArcGISRESTful, WFS, WMS, ServiceURL
             import pygeoutils as geoutils
             from pynhd import NLDI
         
-            basin_geom = NLDI().getfeature_byid(
-                "nwissite",
-                "USGS-11092450",
-                basin=True
-            ).geometry[0]
+            basin_geom = NLDI().get_basins("01031500").geometry[0]
         
             hr = ArcGISRESTful(ServiceURL().restful.nhdplushr, outformat="json")
             hr.layer = 2
         
             hr.oids_bygeom(basin_geom, "epsg:4326")
             resp = hr.get_features()
             flowlines = geoutils.json2geodf(resp)
@@ -212,24 +211,24 @@
         to further filter the data on the server side.
         
         We can also submit a query based on IDs of any valid field in the database. If the measure
         property is desired you can pass ``return_m`` as ``True`` to the ``get_features`` class method:
         
         .. code-block:: python
         
-            hr.oids_byfield("NHDPLUSID", [5000500013223, 5000400039708, 5000500004825])
+            hr.oids_byfield("PERMANENT_IDENTIFIER", ["103455178", "103454362", "103453218"])
             resp = hr.get_features(return_m=True)
             flowlines = geoutils.json2geodf(resp)
         
         Additionally, any valid SQL 92 WHERE clause can be used. For more details look
         `here <https://developers.arcgis.com/rest/services-reference/query-feature-service-.htm#ESRI_SECTION2_07DD2C5127674F6A814CE6C07D39AD46>`__.
         
         .. code-block:: python
         
-            hr.oids_bysql("NHDPLUSID IN (5000500013223, 5000400039708, 5000500004825)")
+            hr.oids_bysql("PERMANENT_IDENTIFIER IN ('103455178', '103454362', '103453218')")
             resp = hr.get_features()
             flowlines = geoutils.json2geodf(resp)
         
         A WMS-based example is shown below:
         
         .. code-block:: python
         
@@ -267,14 +266,47 @@
                 outformat="application/json",
                 version="2.0.0",
                 crs="epsg:4269",
             )
             r = wfs.getfeature_byfilter(f"huc8 LIKE '13030%'")
             huc8 = geoutils.json2geodf(r.json(), "epsg:4269", "epsg:4326")
         
+        PyGeoOGC, has a function for asynchronous download which can help speed up sending/receiveing requests. For example, let's use this function to get `NDVI <https://daac.ornl.gov/VEGETATION/guides/US_MODIS_NDVI.html>`_ data from DACC server. The function can be directly passed to ``xarray.open_mfdataset`` to get the data as an xarray Dataset.
+        
+        .. code-block:: python
+        
+            import xarray as xr
+            import pygeoogc as ogc
+            from datetime import datetime
+        
+            west, south, east, north = basin_geom.bounds
+            base_url = "https://thredds.daac.ornl.gov/thredds/ncss/ornldaac/1299"
+            urls = []
+            dates_itr = [(datetime(y, 1, 1), datetime(y, 1, 31)) for y in range(2000, 2005)]
+            urls = (
+                (
+                    f"{base_url}/MCD13.A{s.year}.unaccum.nc4",
+                    {
+                        "var": "NDVI",
+                        "north": f"{north}",
+                        "west": f"{west}",
+                        "east": f"{east}",
+                        "south": f"{south}",
+                        "disableProjSubset": "on",
+                        "horizStride": "1",
+                        "time_start": s.strftime("%Y-%m-%dT%H:%M:%SZ"),
+                        "time_end": e.strftime("%Y-%m-%dT%H:%M:%SZ"),
+                        "timeStride": "1",
+                        "addLatLon": "true",
+                        "accept": "netcdf",
+                    },
+                )
+                for s, e in dates_itr
+            )
+            data = xr.open_mfdataset(ogc.async_requests(urls, "binary", max_workers=8))
         
         Contributing
         ------------
         
         Contributions are appreciated and very welcomed. Please read
         `CONTRIBUTING.rst <https://github.com/cheginit/pygeoogc/blob/master/CONTRIBUTING.rst>`__
         for instructions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygeoogc-0.2.2/pygeoogc.egg-info/SOURCES.txt` & `pygeoogc-0.9.0/pygeoogc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/scripts/generate_pip_deps_from_conda.py` & `pygeoogc-0.9.0/scripts/generate_pip_deps_from_conda.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "matplotlib-base": "matplotlib",
     "seaborn-base": "seaborn",
     "git+https://github.com/cheginit/pygeoogc.git": "pygeoogc",
     "git+https://github.com/cheginit/pygeoutils.git": "pygeoutils",
     "git+https://github.com/cheginit/pynhd.git": "pynhd",
     "git+https://github.com/cheginit/py3dep.git": "py3dep",
     "git+https://github.com/cheginit/pydaymet.git": "pydaymet",
+    "git+https://github.com/cheginit/hydrodata.git": "hydrodata",
 }
 
 
 def conda_package_to_pip(package):
     """Convert a conda package to its pip equivalent.
 
     In most cases they are the same, those are the exceptions:
@@ -93,15 +94,15 @@
 
     pip_deps = []
     for dep in deps:
         if isinstance(dep, str):
             conda_dep = conda_package_to_pip(dep)
             if conda_dep:
                 pip_deps.append(conda_dep)
-        elif isinstance(dep, dict) and len(dep) == 1 and "pip" in dep:
+        elif isinstance(dep, dict) and len(dep) == 1 and "pip" in dep:  # noqa: SIM106
             pip_deps += dep["pip"]
         else:
             raise ValueError(f"Unexpected dependency {dep}")
 
     for i, dep in enumerate(pip_deps):
         if dep in RENAME:
             pip_deps[i] = RENAME[dep]
```

### Comparing `pygeoogc-0.2.2/setup.cfg` & `pygeoogc-0.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,22 @@
 known_first_party = pygeoogc
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 line_length = 100
 
+[mypy]
+python_version = 3.6
+warn_return_any = True
+warn_unused_configs = True
+disallow_untyped_defs = True
+disallow_incomplete_defs = True
+check_untyped_defs = True
+
 [mypy-numpy.*]
 ignore_missing_imports = True
 
 [mypy-xarray.*]
 ignore_missing_imports = True
 
 [mypy-pytest.*]
```

### Comparing `pygeoogc-0.2.2/setup.py` & `pygeoogc-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/tests/test_exceptions.py` & `pygeoogc-0.9.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pygeoogc-0.2.2/tests/test_pygeoogc.py` & `pygeoogc-0.9.0/tests/test_pygeoogc.py`

 * *Files 26% similar despite different names*

```diff
@@ -63,32 +63,52 @@
     assert (
         sum(len(h) for h in huc2) == 15 and ["MultiPolygon"] in geom_type and "areaacres" in fields
     )
 
 
 @pytest.mark.flaky(max_runs=3)
 def test_restful_bygeom(geometry_nat):
-    wbd8 = ArcGISRESTful(f"{ServiceURL().restful.wbd}/4")
-    wbd8.n_threads = 4
-    wbd8.oids_bygeom(geometry_nat.bounds)
-    wbd8.oids_bygeom(geometry_nat)
-    huc8_all = wbd8.get_features()
-    wbd8.oids_bygeom(geometry_nat, sql_clause="areasqkm > 5000")
-    huc8_large = wbd8.get_features()
-    assert len(huc8_all[0]["features"]) - len(huc8_large[0]["features"]) == 2
+    geofab = ArcGISRESTful(f"{ServiceURL().restful.nhd_fabric}/1")
+    geofab.n_threads = 4
+    geofab.oids_bygeom(geometry_nat.bounds)
+    geofab.oids_bygeom(geometry_nat)
+    wb_all = geofab.get_features()
+    geofab.oids_bygeom(geometry_nat, sql_clause="areasqkm > 20")
+    wb_large = geofab.get_features()
+    assert len(wb_all[0]["features"]) - len(wb_large[0]["features"]) == 915
+
+
+@pytest.mark.flaky(max_runs=3)
+def test_restful_bymultipoint():
+    url = "https://watersgeo.epa.gov/arcgis/rest/services/NHDPlus/NHDPlus/MapServer"
+    sql_clause = "FTYPE NOT IN (420,428,566)"
+    geom = [
+        (-97.06138, 32.837),
+        (-97.06133, 32.836),
+        (-97.06124, 32.834),
+        (-97.06127, 32.832),
+    ]
+    geo_crs = "epsg:4269"
+    distance = 1500
+
+    service = ArcGISRESTful(url, outformat="json")
+    service.layer = 2  # network flowline
+    service.oids_bygeom(geom, geo_crs=geo_crs, sql_clause=sql_clause, distance=distance)
+    resp = service.get_features(return_m=True)
+    assert len(resp[0]["features"]) == 3
 
 
 @pytest.mark.flaky(max_runs=3)
 def test_restful_bysql():
-    hr = ArcGISRESTful(ServiceURL().restful.nhdplushr, outformat="json")
+    hr = ArcGISRESTful(ServiceURL().restful.nhdplushr_edits, outformat="json")
     hr.layer = 1
     hr.layer = 2
-    hr.oids_bysql("NHDPLUSID IN (5000500013223, 5000400039708, 5000500004825)")
+    hr.oids_bysql("NHDFlowline.PERMANENT_IDENTIFIER IN ('103455178', '103454362', '103453218')")
     resp_sql = hr.get_features(return_m=True)
-    hr.oids_byfield("NHDPLUSID", [5000500013223, 5000400039708, 5000500004825])
+    hr.oids_byfield("NHDFlowline.PERMANENT_IDENTIFIER", ["103455178", "103454362", "103453218"])
     resp_ids = hr.get_features()
 
     assert len(resp_sql[0]["features"]) == len(resp_ids[0]["features"])
 
 
 @pytest.mark.flaky(max_runs=3)
 def test_wms(geometry_nat):
@@ -174,82 +194,64 @@
 
 @pytest.mark.flaky(max_runs=3)
 def test_async(geometry_nat):
     west, south, east, north = geometry_nat.bounds
     base_url = "https://thredds.daac.ornl.gov/thredds/ncss/ornldaac/1299"
     url_binary = []
     dates_itr = [(datetime(y, 1, 1), datetime(y, 1, 31)) for y in range(2000, 2005)]
-
-    for s, e in dates_itr:
-        url_binary.append(
-            base_url
-            + "&".join(
-                [
-                    f"MCD13.A{s.year}.unaccum.nc4?",
-                    "var=NDVI",
-                    f"north={north}",
-                    f"west={west}",
-                    f"east={east}",
-                    f"south={south}",
-                    "disableProjSubset=on",
-                    "horizStride=1",
-                    f'time_start={s.strftime("%Y-%m-%dT%H:%M:%SZ")}',
-                    f'time_end={e.strftime("%Y-%m-%dT%H:%M:%SZ")}',
-                    "timeStride=1",
-                    "addLatLon=true",
-                    "accept=netcdf",
-                ]
-            )
+    url_binary = (
+        (
+            f"{base_url}/MCD13.A{s.year}.unaccum.nc4",
+            {
+                "var": "NDVI",
+                "north": f"{north}",
+                "west": f"{west}",
+                "east": f"{east}",
+                "south": f"{south}",
+                "disableProjSubset": "on",
+                "horizStride": "1",
+                "time_start": s.strftime("%Y-%m-%dT%H:%M:%SZ"),
+                "time_end": e.strftime("%Y-%m-%dT%H:%M:%SZ"),
+                "timeStride": "1",
+                "addLatLon": "true",
+                "accept": "netcdf",
+            },
         )
+        for s, e in dates_itr
+    )
 
-    url_json = {
-        "https://labs.waterdata.usgs.gov/api/nldi/linked-data/comid/position": {
-            "f": "json",
-            "coords": "POINT(-68.325 45.0369)",
-        }
-    }
+    url_json = [
+        (
+            "https://labs.waterdata.usgs.gov/api/nldi/linked-data/comid/position",
+            {
+                "f": "json",
+                "coords": "POINT(-68.325 45.0369)",
+            },
+        )
+    ]
 
     url_text = [
-        "https://waterservices.usgs.gov/nwis/site/?format=rdb&sites=01646500&siteStatus=all"
+        (
+            "https://waterservices.usgs.gov/nwis/site/",
+            {"format": "rdb", "sites": "01646500", "siteStatus": "all"},
+        )
     ]
 
     r_b = pygeoogc.async_requests(url_binary, "binary")
     r_j = pygeoogc.async_requests(url_json, "json")
     r_t = pygeoogc.async_requests(url_text, "text")
 
     assert (
         sys.getsizeof(r_b[0]) == 986161
         and r_j[0]["features"][0]["properties"]["identifier"] == "2675320"
         and r_t[0].split("\n")[-2].split("\t")[1] == "01646500"
     )
 
 
 def test_urls():
-    urls = ServiceURL()
-    assert (
-        urls.restful.nwis == "https://waterservices.usgs.gov/nwis"
-        and urls.restful.nldi == "https://labs.waterdata.usgs.gov/api/nldi"
-        and urls.restful.daymet_point == "https://daymet.ornl.gov/single-pixel/api/data"
-        and urls.restful.daymet_grid == "https://thredds.daac.ornl.gov/thredds/ncss/ornldaac/1328"
-        and urls.restful.wbd == "https://hydro.nationalmap.gov/arcgis/rest/services/wbd/MapServer"
-        and urls.restful.fws == "https://www.fws.gov/wetlands/arcgis/rest/services"
-        and urls.restful.fema
-        == "https://hazards.fema.gov/gis/nfhl/rest/services/public/NFHL/MapServer"
-        and urls.wms.mrlc == "https://www.mrlc.gov/geoserver/mrlc_download/wms"
-        and urls.wms.fema
-        == "https://hazards.fema.gov/gis/nfhl/rest/services/public/NFHLWMS/MapServer/WMSServer"
-        and urls.wms.nm_3dep
-        == "https://elevation.nationalmap.gov/arcgis/services/3DEPElevation/ImageServer/WMSServer"
-        and urls.wms.fws
-        == "https://www.fws.gov/wetlands/arcgis/services/Wetlands_Raster/ImageServer/WMSServer"
-        and urls.wfs.waterdata == "https://labs.waterdata.usgs.gov/geoserver/wmadata/ows"
-        and urls.wfs.fema
-        == "https://hazards.fema.gov/gis/nfhl/services/public/NFHL/MapServer/WFSServer"
-        and urls.http.ssebopeta
-        == "https://edcintl.cr.usgs.gov/downloads/sciweb1/shared/uswem/web/conus/eta/modis_eta/daily/downloads"
-    )
+    assert len(ServiceURL().__dict__["urls"]) == 4
 
 
 def test_show_versions():
     f = io.StringIO()
     pygeoogc.show_versions(file=f)
     assert "INSTALLED VERSIONS" in f.getvalue()
```

