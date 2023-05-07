# Comparing `tmp/pynhd-0.2.0.tar.gz` & `tmp/pynhd-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynhd-0.2.0.tar", last modified: Mon Dec  7 02:17:19 2020, max compression
+gzip compressed data, was "pynhd-0.9.0.tar", last modified: Wed Feb 17 18:20:30 2021, max compression
```

## Comparing `pynhd-0.2.0.tar` & `pynhd-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.737782 pynhd-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)      146 2020-12-07 02:17:14.000000 pynhd-0.2.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (116)       91 2020-12-07 02:17:14.000000 pynhd-0.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)      242 2020-12-07 02:17:14.000000 pynhd-0.2.0/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.733782 pynhd-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.733782 pynhd-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      917 2020-12-07 02:17:14.000000 pynhd-0.2.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (116)      684 2020-12-07 02:17:14.000000 pynhd-0.2.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-12-07 02:17:14.000000 pynhd-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (116)      125 2020-12-07 02:17:14.000000 pynhd-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.737782 pynhd-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2584 2020-12-07 02:17:14.000000 pynhd-0.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (116)      288 2020-12-07 02:17:14.000000 pynhd-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (116)      618 2020-12-07 02:17:14.000000 pynhd-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1163 2020-12-07 02:17:14.000000 pynhd-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1193 2020-12-07 02:17:14.000000 pynhd-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-12-07 02:17:14.000000 pynhd-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      163 2020-12-07 02:17:14.000000 pynhd-0.2.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2020-12-07 02:17:14.000000 pynhd-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      157 2020-12-07 02:17:14.000000 pynhd-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3444 2020-12-07 02:17:14.000000 pynhd-0.2.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4080 2020-12-07 02:17:14.000000 pynhd-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1772 2020-12-07 02:17:14.000000 pynhd-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2020-12-07 02:17:14.000000 pynhd-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      150 2020-12-07 02:17:14.000000 pynhd-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2177 2020-12-07 02:17:14.000000 pynhd-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)    14524 2020-12-07 02:17:19.741782 pynhd-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    11292 2020-12-07 02:17:14.000000 pynhd-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.733782 pynhd-0.2.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.737782 pynhd-0.2.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)      501 2020-12-07 02:17:14.000000 pynhd-0.2.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (116)      405 2020-12-07 02:17:14.000000 pynhd-0.2.0/ci/requirements/py3.6.yml
--rw-r--r--   0 runner    (1001) docker     (116)      405 2020-12-07 02:17:14.000000 pynhd-0.2.0/ci/requirements/py3.7.yml
--rw-r--r--   0 runner    (1001) docker     (116)      405 2020-12-07 02:17:14.000000 pynhd-0.2.0/ci/requirements/py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (116)      405 2020-12-07 02:17:14.000000 pynhd-0.2.0/ci/requirements/py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.737782 pynhd-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     8187 2020-12-07 02:17:14.000000 pynhd-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.737782 pynhd-0.2.0/docs/_template/
--rw-r--r--   0 runner    (1001) docker     (116)       85 2020-12-07 02:17:14.000000 pynhd-0.2.0/docs/_template/layout.html
--rw-r--r--   0 runner    (1001) docker     (116)    11832 2020-12-07 02:17:14.000000 pynhd-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-12-07 02:17:14.000000 pynhd-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      771 2020-12-07 02:17:14.000000 pynhd-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       68 2020-12-07 02:17:14.000000 pynhd-0.2.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (116)      571 2020-12-07 02:17:14.000000 pynhd-0.2.0/docs/pynhd.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.737782 pynhd-0.2.0/pynhd/
--rw-r--r--   0 runner    (1001) docker     (116)      485 2020-12-07 02:17:14.000000 pynhd-0.2.0/pynhd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1860 2020-12-07 02:17:14.000000 pynhd-0.2.0/pynhd/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    10378 2020-12-07 02:17:14.000000 pynhd-0.2.0/pynhd/network_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     5079 2020-12-07 02:17:14.000000 pynhd-0.2.0/pynhd/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (116)    19464 2020-12-07 02:17:14.000000 pynhd-0.2.0/pynhd/pynhd.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.737782 pynhd-0.2.0/pynhd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    14524 2020-12-07 02:17:19.000000 pynhd-0.2.0/pynhd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1149 2020-12-07 02:17:19.000000 pynhd-0.2.0/pynhd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 02:17:19.000000 pynhd-0.2.0/pynhd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 02:17:19.000000 pynhd-0.2.0/pynhd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      168 2020-12-07 02:17:19.000000 pynhd-0.2.0/pynhd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-12-07 02:17:19.000000 pynhd-0.2.0/pynhd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      300 2020-12-07 02:17:14.000000 pynhd-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.737782 pynhd-0.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)     4671 2020-12-07 02:17:14.000000 pynhd-0.2.0/scripts/generate_pip_deps_from_conda.py
--rw-r--r--   0 runner    (1001) docker     (116)     1944 2020-12-07 02:17:19.741782 pynhd-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-12-07 02:17:14.000000 pynhd-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:17:19.737782 pynhd-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       39 2020-12-07 02:17:14.000000 pynhd-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      773 2020-12-07 02:17:14.000000 pynhd-0.2.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3809 2020-12-07 02:17:14.000000 pynhd-0.2.0/tests/test_pynhd.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.779678 pynhd-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2021-02-17 18:20:24.000000 pynhd-0.9.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       91 2021-02-17 18:20:24.000000 pynhd-0.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (116)      242 2021-02-17 18:20:24.000000 pynhd-0.9.0/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.763678 pynhd-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.767678 pynhd-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (116)      917 2021-02-17 18:20:24.000000 pynhd-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (116)      684 2021-02-17 18:20:24.000000 pynhd-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (116)      321 2021-02-17 18:20:24.000000 pynhd-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2021-02-17 18:20:24.000000 pynhd-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.767678 pynhd-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2719 2021-02-17 18:20:24.000000 pynhd-0.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2021-02-17 18:20:24.000000 pynhd-0.9.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1306 2021-02-17 18:20:24.000000 pynhd-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1336 2021-02-17 18:20:24.000000 pynhd-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1226 2021-02-17 18:20:24.000000 pynhd-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      163 2021-02-17 18:20:24.000000 pynhd-0.9.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1867 2021-02-17 18:20:24.000000 pynhd-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      157 2021-02-17 18:20:24.000000 pynhd-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3444 2021-02-17 18:20:24.000000 pynhd-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4080 2021-02-17 18:20:24.000000 pynhd-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3421 2021-02-17 18:20:24.000000 pynhd-0.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1096 2021-02-17 18:20:24.000000 pynhd-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      150 2021-02-17 18:20:24.000000 pynhd-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2177 2021-02-17 18:20:24.000000 pynhd-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)    16280 2021-02-17 18:20:30.779678 pynhd-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    12816 2021-02-17 18:20:24.000000 pynhd-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.755678 pynhd-0.9.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.771678 pynhd-0.9.0/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (116)      528 2021-02-17 18:20:24.000000 pynhd-0.9.0/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      431 2021-02-17 18:20:24.000000 pynhd-0.9.0/ci/requirements/py3.6.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      431 2021-02-17 18:20:24.000000 pynhd-0.9.0/ci/requirements/py3.7.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      431 2021-02-17 18:20:24.000000 pynhd-0.9.0/ci/requirements/py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      431 2021-02-17 18:20:24.000000 pynhd-0.9.0/ci/requirements/py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.771678 pynhd-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     8187 2021-02-17 18:20:24.000000 pynhd-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.771678 pynhd-0.9.0/docs/_template/
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2021-02-17 18:20:24.000000 pynhd-0.9.0/docs/_template/layout.html
+-rw-r--r--   0 runner    (1001) docker     (116)    11832 2021-02-17 18:20:24.000000 pynhd-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2021-02-17 18:20:24.000000 pynhd-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      771 2021-02-17 18:20:24.000000 pynhd-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (116)       68 2021-02-17 18:20:24.000000 pynhd-0.9.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      571 2021-02-17 18:20:24.000000 pynhd-0.9.0/docs/pynhd.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.775678 pynhd-0.9.0/pynhd/
+-rw-r--r--   0 runner    (1001) docker     (116)      509 2021-02-17 18:20:24.000000 pynhd-0.9.0/pynhd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1860 2021-02-17 18:20:24.000000 pynhd-0.9.0/pynhd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10679 2021-02-17 18:20:24.000000 pynhd-0.9.0/pynhd/network_tools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5251 2021-02-17 18:20:24.000000 pynhd-0.9.0/pynhd/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    31910 2021-02-17 18:20:24.000000 pynhd-0.9.0/pynhd/pynhd.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.779678 pynhd-0.9.0/pynhd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    16280 2021-02-17 18:20:30.000000 pynhd-0.9.0/pynhd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1094 2021-02-17 18:20:30.000000 pynhd-0.9.0/pynhd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:20:30.000000 pynhd-0.9.0/pynhd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:20:30.000000 pynhd-0.9.0/pynhd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      187 2021-02-17 18:20:30.000000 pynhd-0.9.0/pynhd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2021-02-17 18:20:30.000000 pynhd-0.9.0/pynhd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      319 2021-02-17 18:20:24.000000 pynhd-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.779678 pynhd-0.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4753 2021-02-17 18:20:24.000000 pynhd-0.9.0/scripts/generate_pip_deps_from_conda.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2110 2021-02-17 18:20:30.779678 pynhd-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      587 2021-02-17 18:20:24.000000 pynhd-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:30.779678 pynhd-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      773 2021-02-17 18:20:24.000000 pynhd-0.9.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5227 2021-02-17 18:20:24.000000 pynhd-0.9.0/tests/test_pynhd.py
```

### Comparing `pynhd-0.2.0/.github/ISSUE_TEMPLATE/bug-report.md` & `pynhd-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/.github/ISSUE_TEMPLATE/feature-request.md` & `pynhd-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/.github/workflows/codeql-analysis.yml` & `pynhd-0.9.0/.github/workflows/codeql-analysis.yml`

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

### Comparing `pynhd-0.2.0/.github/workflows/release.yml` & `pynhd-0.9.0/.github/workflows/release.yml`

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

### Comparing `pynhd-0.2.0/.github/workflows/test.yml` & `pynhd-0.9.0/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

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
           activate-environment: pynhd
           python-version: ${{ matrix.python-version }}
           environment-file: ci/requirements/py${{ matrix.python-version }}.yml
```

### Comparing `pynhd-0.2.0/.gitignore` & `pynhd-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/.pre-commit-config.yaml` & `pynhd-0.9.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,72 @@
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
+        exclude: tests
         files: pynhd
 
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
         args: [-lll, --recursive, pynhd]
         files: .py$
-
```

### Comparing `pynhd-0.2.0/CODE_OF_CONDUCT.rst` & `pynhd-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/CONTRIBUTING.rst` & `pynhd-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/LICENSE` & `pynhd-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/Makefile` & `pynhd-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/PKG-INFO` & `pynhd-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: pynhd
-Version: 0.2.0
+Version: 0.9.0
 Summary: Process and access NHDPlus V2 data through NLDI and WaterData web services.
 Home-page: https://github.com/cheginit/pynhd
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT license
 Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pynhd_logo.png
             :target: https://github.com/cheginit/pynhd
             :align: center
         
         |
         
-        .. |hydrodata| image:: https://github.com/cheginit/hydrodata/workflows/build/badge.svg
-            :target: https://github.com/cheginit/hydrodata/actions?query=workflow%3Abuild
+        .. |hydrodata| image:: https://github.com/cheginit/hydrodata/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/hydrodata/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |pygeoogc| image:: https://github.com/cheginit/pygeoogc/workflows/build/badge.svg
-            :target: https://github.com/cheginit/pygeoogc/actions?query=workflow%3Abuild
+        .. |pygeoogc| image:: https://github.com/cheginit/pygeoogc/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/pygeoogc/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |pygeoutils| image:: https://github.com/cheginit/pygeoutils/workflows/build/badge.svg
-            :target: https://github.com/cheginit/pygeoutils/actions?query=workflow%3Abuild
+        .. |pygeoutils| image:: https://github.com/cheginit/pygeoutils/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/pygeoutils/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |pynhd| image:: https://github.com/cheginit/pynhd/workflows/build/badge.svg
-            :target: https://github.com/cheginit/pynhd/actions?query=workflow%3Abuild
+        .. |pynhd| image:: https://github.com/cheginit/pynhd/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/pynhd/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |py3dep| image:: https://github.com/cheginit/py3dep/workflows/build/badge.svg
-            :target: https://github.com/cheginit/py3dep/actions?query=workflow%3Abuild
+        .. |py3dep| image:: https://github.com/cheginit/py3dep/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/py3dep/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |pydaymet| image:: https://github.com/cheginit/pydaymet/workflows/build/badge.svg
-            :target: https://github.com/cheginit/pydaymet/actions?query=workflow%3Abuild
+        .. |pydaymet| image:: https://github.com/cheginit/pydaymet/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/pydaymet/actions?query=workflow%3Apytest
             :alt: Github Actions
         
         =========== ==================================================================== ============
         Package     Description                                                          Status
         =========== ==================================================================== ============
         Hydrodata_  Access NWIS, HCDN 2009, NLCD, and SSEBop databases                   |hydrodata|
         PyGeoOGC_   Send queries to any ArcGIS RESTful-, WMS-, and WFS-based services    |pygeoogc|
@@ -85,33 +85,33 @@
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
             :target: https://github.com/pre-commit/pre-commit
             :alt: pre-commit
         
         |
         
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
         Features
         --------
         
         PyNHD is a part of Hydrodata software stack and provides access to
         `WaterData <https://labs.waterdata.usgs.gov/geoserver/web/wicket/bookmarkable/org.geoserver.web.demo.MapPreviewPage?1>`__
         and `NLDI <https://labs.waterdata.usgs.gov/about-nldi/>`_ web services. These two web services
         can be used to navigate and extract vector data from NHDPlus V2 database such as
-        catchments, HUC8, HUC12, GagesII, flowlines, and water bodies. Moreover, the NLDI service
-        includes more than 30 NHDPlus catchment-scale attributes that are associated with NHDPlus
-        ComIDs. Values of these attributes are provided in three characteristic types:
-        
-        1. ``local``: For individual reach catchments,
-        2. ``tot``: For network-accumulated values using total cumulative drainage area,
-        3. ``div``: For network-accumulated values using divergence-routed.
+        catchments, HUC8, HUC12, GagesII, flowlines, and water bodies. Moreover, PyNHD gives access to
+        an item on `ScienceBase <https://sciencebase.usgs.gov>`_ called
+        `Select Attributes for NHDPlus Version 2.1 Reach Catchments and Modified Network Routed Upstream Watersheds for the Conterminous United States <https://www.sciencebase.gov/catalog/item/5669a79ee4b08895842a1d47>`_.
+        This item prvoides over 30 attributes at catchment-scale based on NHDPlus ComIDs.
+        These attributes are avilable in three categories:
+        
+        1. Local (`local`): For individual reach catchments,
+        2. Total (`upstream_acc`): For network-accumulated values using total cumulative drainage area,
+        3. Divergence (`div_routing`): For network-accumulated values using divergence-routed.
         
-        A list of these attributes for each characteristic type can be accessed using
-        ``NLDI().get_validchars`` class method.
+        A list of these attributes for each characteristic type can be accessed using ``nhdplus_attrs``
+        function.
         
         Additionally, PyNHD offers some extra utilities for processing the flowlines:
         
         - ``prepare_nhdplus``: For cleaning up the dataframe by, for example, removing tiny networks,
           adding a ``to_comid`` column, and finding a terminal flowlines if it doesn't exist.
         - ``topoogical_sort``: For sorting the river network topologically which is useful for routing
           and flow accumulation.
@@ -121,14 +121,18 @@
         These utilities are developed based on an ``R`` package called
         `nhdplusTools <https://github.com/USGS-R/nhdplusTools>`__.
         
         You can try using PyNHD without installing it on you system by clicking on the binder badge
         below the PyNHD banner. A Jupyter notebook instance with the Hydrodata software stack
         pre-installed will be launched in your web browser and you can start coding!
         
+        Please note that since Hydrodata is in early development stages, while the provided
+        functionaities should be stable, changes in APIs are possible in new releases. But we
+        appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+        
         Moreover, requests for additional functionalities can be submitted via
         `issue tracker <https://github.com/cheginit/pynhd/issues>`__.
         
         Installation
         ------------
         
         You can install PyNHD using ``pip`` after installing ``libgdal`` on your system
@@ -157,87 +161,112 @@
         
         First, let’s get the watershed geometry of the contributing basin of a
         USGS station using ``NLDI``:
         
         .. code:: python
         
             nldi = NLDI()
-            station_id = "USGS-01031500"
-            ut = "upstreamTributaries"
-            um = "upstreamMain"
+            station_id = "01031500"
         
-            basin = nldi.getfeature_byid("nwissite", station_id, basin=True)
+            basin = nldi.get_basins(station_id)
         
         The ``navigate_byid`` class method can be used to navigate NHDPlus in
         both upstream and downstream of any point in the database. Let’s get ComIDs and flowlines
         of the tributaries and the main river channel in the upstream of the station.
         
         .. code:: python
         
-            args = {
-                "fsource": "nwissite",
-                "fid": station_id,
-                "navigation": um,
-                "source": "flowlines",
-                "distance": 1000,
-            }
-        
-            flw_main = nldi.navigate_byid(**args)
-        
-            args["navigation"] = ut
-            flw_trib = nldi.navigate_byid(**args)
+            flw_main = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamMain",
+                source="flowlines",
+                distance=1000,
+            )
+        
+            flw_trib = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamTributaries",
+                source="flowlines",
+                distance=1000,
+            )
         
         We can get other USGS stations upstream (or downstream) of the station
         and even set a distance limit (in km):
         
         .. code:: python
         
-            args.update({
-                "source" : "nwissite",
-            })
-            st_all = nldi.navigate_byid(**args)
-        
-            args.update({
-                "distance": 20,
-                "source" : "nwissite",
-            })
-            st_d20 = nldi.navigate_byid(**args)
+            st_all = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamTributaries",
+                source="nwissite",
+                distance=1000,
+            )
+        
+            st_d20 = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamTributaries",
+                source="nwissite",
+                distance=20,
+            )
         
         Now, let’s get the `HUC12 pour
         points <https://www.sciencebase.gov/catalog/item/5762b664e4b07657d19a71ea>`__:
         
         .. code:: python
         
-            args.update({
-                "distance": 1000,
-                "source" : "huc12pp",
-            })
-            pp = nldi.navigate_byid(**args)
+            pp = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamTributaries",
+                source="huc12pp",
+                distance=1000,
+            )
         
         .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_12_0.png
             :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_12_0.png
             :width: 400
             :align: center
         
-        Now, let's get the medium- and high-resolution flowlines within the bounding box of this watershed
-        and compare them.
+        Next, we retrieve the medium- and high-resolution flowlines within the bounding box of our
+        watershed and compare them. Moreover, Since serveral web services offer access to NHDPlus database,
+        ``NHDPlusHR`` has an argument for selecting a service and also an argument for automatically
+        switching between services.
         
         .. code:: python
         
             mr = WaterData("nhdflowline_network")
             nhdp_mr = mr.bybox(basin.geometry[0].bounds)
         
-            hr = NHDPlusHR("networknhdflowline")
+            hr = NHDPlusHR("networknhdflowline", service="hydro", auto_switch=True)
             nhdp_hr = hr.bygeom(basin.geometry[0].bounds)
         
         .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hr_mr.png
             :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hr_mr.png
             :width: 400
             :align: center
         
+        Moreover, ``WaterData`` can find features within a given radius (in meters) of a point:
+        
+        .. code:: python
+        
+            eck4 = "+proj=eck4 +lon_0=0 +x_0=0 +y_0=0 +datum=WGS84 +units=m +no_defs"
+            coords = (-5727797.427596455, 5584066.49330473)
+            rad = 5e3
+            flw_rad = mr.bydistance(coords, rad, loc_crs=eck4)
+            flw_rad = flw_rad.to_crs(eck4)
+        
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_radius.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_radius.png
+            :width: 400
+            :align: center
+        
         Since NHDPlus HR is still at the pre-release stage let's use the MR flowlines to
         demonstrate the vector-based accumulation.
         Based on a topological sorted river network
         ``pynhd.vector_accumulation`` computes flow accumulation in the network.
         It returns a dataframe which is sorted from upstream to downstream that
         shows the accumulated flow in each node.
         
@@ -253,16 +282,16 @@
         
             wd = WaterData("nhdflowline_network")
         
             comids = flw_trib.nhdplus_comid.to_list()
             nhdp_trib = wd.byid("comid", comids)
             flw = nhd.prepare_nhdplus(nhdp_trib, 0, 0, purge_non_dendritic=False)
         
-        Now, let’s get Mean Annual Groundwater Recharge using ``getcharacteristic_byid``
-        class method and carry out the accumulation.
+        To demostrate the use of routing, let's use ``nhdplus_attrs`` function to get list of available
+        NHDPlus attributes
         
         .. code:: python
         
             char = "CAT_RECHG"
             area = "areasqkm"
         
             local = nldi.getcharacteristic_byid(comids, "local", char_ids=char)
```

### Comparing `pynhd-0.2.0/README.rst` & `pynhd-0.9.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pynhd_logo.png
     :target: https://github.com/cheginit/pynhd
     :align: center
 
 |
 
-.. |hydrodata| image:: https://github.com/cheginit/hydrodata/workflows/build/badge.svg
-    :target: https://github.com/cheginit/hydrodata/actions?query=workflow%3Abuild
+.. |hydrodata| image:: https://github.com/cheginit/hydrodata/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/hydrodata/actions?query=workflow%3Apytest
     :alt: Github Actions
 
-.. |pygeoogc| image:: https://github.com/cheginit/pygeoogc/workflows/build/badge.svg
-    :target: https://github.com/cheginit/pygeoogc/actions?query=workflow%3Abuild
+.. |pygeoogc| image:: https://github.com/cheginit/pygeoogc/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/pygeoogc/actions?query=workflow%3Apytest
     :alt: Github Actions
 
-.. |pygeoutils| image:: https://github.com/cheginit/pygeoutils/workflows/build/badge.svg
-    :target: https://github.com/cheginit/pygeoutils/actions?query=workflow%3Abuild
+.. |pygeoutils| image:: https://github.com/cheginit/pygeoutils/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/pygeoutils/actions?query=workflow%3Apytest
     :alt: Github Actions
 
-.. |pynhd| image:: https://github.com/cheginit/pynhd/workflows/build/badge.svg
-    :target: https://github.com/cheginit/pynhd/actions?query=workflow%3Abuild
+.. |pynhd| image:: https://github.com/cheginit/pynhd/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/pynhd/actions?query=workflow%3Apytest
     :alt: Github Actions
 
-.. |py3dep| image:: https://github.com/cheginit/py3dep/workflows/build/badge.svg
-    :target: https://github.com/cheginit/py3dep/actions?query=workflow%3Abuild
+.. |py3dep| image:: https://github.com/cheginit/py3dep/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/py3dep/actions?query=workflow%3Apytest
     :alt: Github Actions
 
-.. |pydaymet| image:: https://github.com/cheginit/pydaymet/workflows/build/badge.svg
-    :target: https://github.com/cheginit/pydaymet/actions?query=workflow%3Abuild
+.. |pydaymet| image:: https://github.com/cheginit/pydaymet/workflows/pytest/badge.svg
+    :target: https://github.com/cheginit/pydaymet/actions?query=workflow%3Apytest
     :alt: Github Actions
 
 =========== ==================================================================== ============
 Package     Description                                                          Status
 =========== ==================================================================== ============
 Hydrodata_  Access NWIS, HCDN 2009, NLCD, and SSEBop databases                   |hydrodata|
 PyGeoOGC_   Send queries to any ArcGIS RESTful-, WMS-, and WFS-based services    |pygeoogc|
@@ -77,33 +77,33 @@
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
     :target: https://github.com/pre-commit/pre-commit
     :alt: pre-commit
 
 |
 
-🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-
 Features
 --------
 
 PyNHD is a part of Hydrodata software stack and provides access to
 `WaterData <https://labs.waterdata.usgs.gov/geoserver/web/wicket/bookmarkable/org.geoserver.web.demo.MapPreviewPage?1>`__
 and `NLDI <https://labs.waterdata.usgs.gov/about-nldi/>`_ web services. These two web services
 can be used to navigate and extract vector data from NHDPlus V2 database such as
-catchments, HUC8, HUC12, GagesII, flowlines, and water bodies. Moreover, the NLDI service
-includes more than 30 NHDPlus catchment-scale attributes that are associated with NHDPlus
-ComIDs. Values of these attributes are provided in three characteristic types:
-
-1. ``local``: For individual reach catchments,
-2. ``tot``: For network-accumulated values using total cumulative drainage area,
-3. ``div``: For network-accumulated values using divergence-routed.
+catchments, HUC8, HUC12, GagesII, flowlines, and water bodies. Moreover, PyNHD gives access to
+an item on `ScienceBase <https://sciencebase.usgs.gov>`_ called
+`Select Attributes for NHDPlus Version 2.1 Reach Catchments and Modified Network Routed Upstream Watersheds for the Conterminous United States <https://www.sciencebase.gov/catalog/item/5669a79ee4b08895842a1d47>`_.
+This item prvoides over 30 attributes at catchment-scale based on NHDPlus ComIDs.
+These attributes are avilable in three categories:
+
+1. Local (`local`): For individual reach catchments,
+2. Total (`upstream_acc`): For network-accumulated values using total cumulative drainage area,
+3. Divergence (`div_routing`): For network-accumulated values using divergence-routed.
 
-A list of these attributes for each characteristic type can be accessed using
-``NLDI().get_validchars`` class method.
+A list of these attributes for each characteristic type can be accessed using ``nhdplus_attrs``
+function.
 
 Additionally, PyNHD offers some extra utilities for processing the flowlines:
 
 - ``prepare_nhdplus``: For cleaning up the dataframe by, for example, removing tiny networks,
   adding a ``to_comid`` column, and finding a terminal flowlines if it doesn't exist.
 - ``topoogical_sort``: For sorting the river network topologically which is useful for routing
   and flow accumulation.
@@ -113,14 +113,18 @@
 These utilities are developed based on an ``R`` package called
 `nhdplusTools <https://github.com/USGS-R/nhdplusTools>`__.
 
 You can try using PyNHD without installing it on you system by clicking on the binder badge
 below the PyNHD banner. A Jupyter notebook instance with the Hydrodata software stack
 pre-installed will be launched in your web browser and you can start coding!
 
+Please note that since Hydrodata is in early development stages, while the provided
+functionaities should be stable, changes in APIs are possible in new releases. But we
+appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+
 Moreover, requests for additional functionalities can be submitted via
 `issue tracker <https://github.com/cheginit/pynhd/issues>`__.
 
 Installation
 ------------
 
 You can install PyNHD using ``pip`` after installing ``libgdal`` on your system
@@ -149,87 +153,112 @@
 
 First, let’s get the watershed geometry of the contributing basin of a
 USGS station using ``NLDI``:
 
 .. code:: python
 
     nldi = NLDI()
-    station_id = "USGS-01031500"
-    ut = "upstreamTributaries"
-    um = "upstreamMain"
+    station_id = "01031500"
 
-    basin = nldi.getfeature_byid("nwissite", station_id, basin=True)
+    basin = nldi.get_basins(station_id)
 
 The ``navigate_byid`` class method can be used to navigate NHDPlus in
 both upstream and downstream of any point in the database. Let’s get ComIDs and flowlines
 of the tributaries and the main river channel in the upstream of the station.
 
 .. code:: python
 
-    args = {
-        "fsource": "nwissite",
-        "fid": station_id,
-        "navigation": um,
-        "source": "flowlines",
-        "distance": 1000,
-    }
-
-    flw_main = nldi.navigate_byid(**args)
-
-    args["navigation"] = ut
-    flw_trib = nldi.navigate_byid(**args)
+    flw_main = nldi.navigate_byid(
+        fsource="nwissite",
+        fid=f"USGS-{station_id}",
+        navigation="upstreamMain",
+        source="flowlines",
+        distance=1000,
+    )
+
+    flw_trib = nldi.navigate_byid(
+        fsource="nwissite",
+        fid=f"USGS-{station_id}",
+        navigation="upstreamTributaries",
+        source="flowlines",
+        distance=1000,
+    )
 
 We can get other USGS stations upstream (or downstream) of the station
 and even set a distance limit (in km):
 
 .. code:: python
 
-    args.update({
-        "source" : "nwissite",
-    })
-    st_all = nldi.navigate_byid(**args)
-
-    args.update({
-        "distance": 20,
-        "source" : "nwissite",
-    })
-    st_d20 = nldi.navigate_byid(**args)
+    st_all = nldi.navigate_byid(
+        fsource="nwissite",
+        fid=f"USGS-{station_id}",
+        navigation="upstreamTributaries",
+        source="nwissite",
+        distance=1000,
+    )
+
+    st_d20 = nldi.navigate_byid(
+        fsource="nwissite",
+        fid=f"USGS-{station_id}",
+        navigation="upstreamTributaries",
+        source="nwissite",
+        distance=20,
+    )
 
 Now, let’s get the `HUC12 pour
 points <https://www.sciencebase.gov/catalog/item/5762b664e4b07657d19a71ea>`__:
 
 .. code:: python
 
-    args.update({
-        "distance": 1000,
-        "source" : "huc12pp",
-    })
-    pp = nldi.navigate_byid(**args)
+    pp = nldi.navigate_byid(
+        fsource="nwissite",
+        fid=f"USGS-{station_id}",
+        navigation="upstreamTributaries",
+        source="huc12pp",
+        distance=1000,
+    )
 
 .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_12_0.png
     :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_12_0.png
     :width: 400
     :align: center
 
-Now, let's get the medium- and high-resolution flowlines within the bounding box of this watershed
-and compare them.
+Next, we retrieve the medium- and high-resolution flowlines within the bounding box of our
+watershed and compare them. Moreover, Since serveral web services offer access to NHDPlus database,
+``NHDPlusHR`` has an argument for selecting a service and also an argument for automatically
+switching between services.
 
 .. code:: python
 
     mr = WaterData("nhdflowline_network")
     nhdp_mr = mr.bybox(basin.geometry[0].bounds)
 
-    hr = NHDPlusHR("networknhdflowline")
+    hr = NHDPlusHR("networknhdflowline", service="hydro", auto_switch=True)
     nhdp_hr = hr.bygeom(basin.geometry[0].bounds)
 
 .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hr_mr.png
     :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hr_mr.png
     :width: 400
     :align: center
 
+Moreover, ``WaterData`` can find features within a given radius (in meters) of a point:
+
+.. code:: python
+
+    eck4 = "+proj=eck4 +lon_0=0 +x_0=0 +y_0=0 +datum=WGS84 +units=m +no_defs"
+    coords = (-5727797.427596455, 5584066.49330473)
+    rad = 5e3
+    flw_rad = mr.bydistance(coords, rad, loc_crs=eck4)
+    flw_rad = flw_rad.to_crs(eck4)
+
+.. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_radius.png
+    :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_radius.png
+    :width: 400
+    :align: center
+
 Since NHDPlus HR is still at the pre-release stage let's use the MR flowlines to
 demonstrate the vector-based accumulation.
 Based on a topological sorted river network
 ``pynhd.vector_accumulation`` computes flow accumulation in the network.
 It returns a dataframe which is sorted from upstream to downstream that
 shows the accumulated flow in each node.
 
@@ -245,16 +274,16 @@
 
     wd = WaterData("nhdflowline_network")
 
     comids = flw_trib.nhdplus_comid.to_list()
     nhdp_trib = wd.byid("comid", comids)
     flw = nhd.prepare_nhdplus(nhdp_trib, 0, 0, purge_non_dendritic=False)
 
-Now, let’s get Mean Annual Groundwater Recharge using ``getcharacteristic_byid``
-class method and carry out the accumulation.
+To demostrate the use of routing, let's use ``nhdplus_attrs`` function to get list of available
+NHDPlus attributes
 
 .. code:: python
 
     char = "CAT_RECHG"
     area = "areasqkm"
 
     local = nldi.getcharacteristic_byid(comids, "local", char_ids=char)
```

### Comparing `pynhd-0.2.0/docs/Makefile` & `pynhd-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/docs/conf.py` & `pynhd-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/docs/make.bat` & `pynhd-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/docs/pynhd.rst` & `pynhd-0.9.0/docs/pynhd.rst`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/pynhd/exceptions.py` & `pynhd-0.9.0/pynhd/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/pynhd/network_tools.py` & `pynhd-0.9.0/pynhd/network_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Access NLDI and WaterData databases."""
 import numbers
-from typing import Callable, Dict, Iterable, List, Tuple, Union
+from typing import Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import geopandas as gpd
 import networkx as nx
 import numpy as np
 import pandas as pd
 from pandas._libs.missing import NAType
 
@@ -63,19 +63,19 @@
         "ftype",
     ]
 
     check_requirements(req_cols, flw)
     flw[req_cols[:-1]] = flw[req_cols[:-1]].astype("Int64")
 
     if not any(flw.terminalfl == 1):
-        if all(flw.terminalpa == flw.terminalpa.iloc[0]):
-            flw.loc[flw.hydroseq == flw.hydroseq.min(), "terminalfl"] = 1
-        else:
+        if not all(flw.terminalpa == flw.terminalpa.iloc[0]):
             raise ZeroMatched("No terminal flag were found in the dataframe.")
 
+        flw.loc[flw.hydroseq == flw.hydroseq.min(), "terminalfl"] = 1
+
     if purge_non_dendritic:
         flw = flw[
             ((flw.ftype != "Coastline") | (flw.ftype != 566)) & (flw.streamorde == flw.streamcalc)
         ]
     else:
         flw = flw[(flw.ftype != "Coastline") | (flw.ftype != 566)]
         flw.loc[flw.divergence == 2, "fromnode"] = pd.NA
@@ -170,53 +170,56 @@
         The input dataframe With an additional column named ``tocomid``.
     """
     req_cols = ["comid", "terminalpa", "fromnode", "tonode"]
     check_requirements(req_cols, flw)
 
     flw[req_cols] = flw[req_cols].astype("Int64")
 
-    def tocomid(group):
-        def toid(row):
+    def tocomid(group: pd.core.groupby.generic.DataFrameGroupBy) -> pd.DataFrame:
+        def toid(row: pd.DataFrame) -> pd.Int64Dtype:
             try:
                 return group[group.fromnode == row.tonode].comid.to_numpy()[0]
             except IndexError:
                 return pd.NA
 
         return group.apply(toid, axis=1)
 
     flw["tocomid"] = pd.concat([tocomid(g) for _, g in flw.groupby("terminalpa")])
     return flw
 
 
 def topoogical_sort(
-    flowlines: pd.DataFrame,
+    flowlines: pd.DataFrame, edge_attr: Optional[Union[str, List[str]]] = None
 ) -> Tuple[List[Union[str, NAType]], Dict[Union[str, NAType], List[str]], nx.DiGraph]:
     """Topological sorting of a river network.
 
     Parameters
     ----------
     flowlines : pandas.DataFrame
         A dataframe with columns ID and toID
+    edge_attr : str or list, optional
+        Names of the columns in the dataframe to be used as edge attributes, defaults to None.
 
     Returns
     -------
     (list, dict , networkx.DiGraph)
         A list of topologically sorted IDs, a dictionary
         with keys as IDs and values as its upstream nodes,
         and the generated networkx object. Note that the
         terminal node ID is set to pd.NA.
     """
     upstream_nodes = {i: flowlines[flowlines.toID == i].ID.tolist() for i in flowlines.ID.tolist()}
     upstream_nodes[pd.NA] = flowlines[flowlines.toID.isna()].ID.tolist()
 
     netwrok = nx.from_pandas_edgelist(
-        flowlines[["ID", "toID"]],
+        flowlines,
         source="ID",
         target="toID",
         create_using=nx.DiGraph,
+        edge_attr=edge_attr,
     )
     topo_sorted = list(nx.topological_sort(netwrok))
     return topo_sorted, upstream_nodes, netwrok
 
 
 def vector_accumulation(
     flowlines: pd.DataFrame,
@@ -267,20 +270,21 @@
         flowlines[[id_col, toid_col]].rename(columns={id_col: "ID", toid_col: "toID"})
     )
     topo_sorted = sorted_nodes[:-1]
 
     outflow = flowlines.set_index(id_col)[attr_col].to_dict()
 
     init = flowlines.iloc[0][attr_col]
+    if not isinstance(init, (np.ndarray, list, numbers.Number)):
+        raise InvalidInputType("values of attr_col", "a scalar or an array")
+
     if isinstance(init, numbers.Number):
         outflow["0"] = 0.0
-    elif isinstance(init, (np.ndarray, list)):
-        outflow["0"] = np.zeros_like(init)
     else:
-        raise InvalidInputType("values of attr_col", "a scalar or an array")
+        outflow["0"] = np.zeros_like(init)
 
     upstream_nodes.update({k: ["0"] for k, v in upstream_nodes.items() if len(v) == 0})
 
     for i in topo_sorted:
         outflow[i] = func(
             np.sum([outflow[u] for u in upstream_nodes[i]], axis=0),
             *flowlines.loc[flowlines[id_col] == i, arg_cols].to_numpy()[0],
```

### Comparing `pynhd-0.2.0/pynhd/print_versions.py` & `pynhd-0.9.0/pynhd/print_versions.py`

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

### Comparing `pynhd-0.2.0/pynhd.egg-info/PKG-INFO` & `pynhd-0.9.0/pynhd.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: pynhd
-Version: 0.2.0
+Version: 0.9.0
 Summary: Process and access NHDPlus V2 data through NLDI and WaterData web services.
 Home-page: https://github.com/cheginit/pynhd
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT license
 Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pynhd_logo.png
             :target: https://github.com/cheginit/pynhd
             :align: center
         
         |
         
-        .. |hydrodata| image:: https://github.com/cheginit/hydrodata/workflows/build/badge.svg
-            :target: https://github.com/cheginit/hydrodata/actions?query=workflow%3Abuild
+        .. |hydrodata| image:: https://github.com/cheginit/hydrodata/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/hydrodata/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |pygeoogc| image:: https://github.com/cheginit/pygeoogc/workflows/build/badge.svg
-            :target: https://github.com/cheginit/pygeoogc/actions?query=workflow%3Abuild
+        .. |pygeoogc| image:: https://github.com/cheginit/pygeoogc/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/pygeoogc/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |pygeoutils| image:: https://github.com/cheginit/pygeoutils/workflows/build/badge.svg
-            :target: https://github.com/cheginit/pygeoutils/actions?query=workflow%3Abuild
+        .. |pygeoutils| image:: https://github.com/cheginit/pygeoutils/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/pygeoutils/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |pynhd| image:: https://github.com/cheginit/pynhd/workflows/build/badge.svg
-            :target: https://github.com/cheginit/pynhd/actions?query=workflow%3Abuild
+        .. |pynhd| image:: https://github.com/cheginit/pynhd/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/pynhd/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |py3dep| image:: https://github.com/cheginit/py3dep/workflows/build/badge.svg
-            :target: https://github.com/cheginit/py3dep/actions?query=workflow%3Abuild
+        .. |py3dep| image:: https://github.com/cheginit/py3dep/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/py3dep/actions?query=workflow%3Apytest
             :alt: Github Actions
         
-        .. |pydaymet| image:: https://github.com/cheginit/pydaymet/workflows/build/badge.svg
-            :target: https://github.com/cheginit/pydaymet/actions?query=workflow%3Abuild
+        .. |pydaymet| image:: https://github.com/cheginit/pydaymet/workflows/pytest/badge.svg
+            :target: https://github.com/cheginit/pydaymet/actions?query=workflow%3Apytest
             :alt: Github Actions
         
         =========== ==================================================================== ============
         Package     Description                                                          Status
         =========== ==================================================================== ============
         Hydrodata_  Access NWIS, HCDN 2009, NLCD, and SSEBop databases                   |hydrodata|
         PyGeoOGC_   Send queries to any ArcGIS RESTful-, WMS-, and WFS-based services    |pygeoogc|
@@ -85,33 +85,33 @@
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
             :target: https://github.com/pre-commit/pre-commit
             :alt: pre-commit
         
         |
         
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
         Features
         --------
         
         PyNHD is a part of Hydrodata software stack and provides access to
         `WaterData <https://labs.waterdata.usgs.gov/geoserver/web/wicket/bookmarkable/org.geoserver.web.demo.MapPreviewPage?1>`__
         and `NLDI <https://labs.waterdata.usgs.gov/about-nldi/>`_ web services. These two web services
         can be used to navigate and extract vector data from NHDPlus V2 database such as
-        catchments, HUC8, HUC12, GagesII, flowlines, and water bodies. Moreover, the NLDI service
-        includes more than 30 NHDPlus catchment-scale attributes that are associated with NHDPlus
-        ComIDs. Values of these attributes are provided in three characteristic types:
-        
-        1. ``local``: For individual reach catchments,
-        2. ``tot``: For network-accumulated values using total cumulative drainage area,
-        3. ``div``: For network-accumulated values using divergence-routed.
+        catchments, HUC8, HUC12, GagesII, flowlines, and water bodies. Moreover, PyNHD gives access to
+        an item on `ScienceBase <https://sciencebase.usgs.gov>`_ called
+        `Select Attributes for NHDPlus Version 2.1 Reach Catchments and Modified Network Routed Upstream Watersheds for the Conterminous United States <https://www.sciencebase.gov/catalog/item/5669a79ee4b08895842a1d47>`_.
+        This item prvoides over 30 attributes at catchment-scale based on NHDPlus ComIDs.
+        These attributes are avilable in three categories:
+        
+        1. Local (`local`): For individual reach catchments,
+        2. Total (`upstream_acc`): For network-accumulated values using total cumulative drainage area,
+        3. Divergence (`div_routing`): For network-accumulated values using divergence-routed.
         
-        A list of these attributes for each characteristic type can be accessed using
-        ``NLDI().get_validchars`` class method.
+        A list of these attributes for each characteristic type can be accessed using ``nhdplus_attrs``
+        function.
         
         Additionally, PyNHD offers some extra utilities for processing the flowlines:
         
         - ``prepare_nhdplus``: For cleaning up the dataframe by, for example, removing tiny networks,
           adding a ``to_comid`` column, and finding a terminal flowlines if it doesn't exist.
         - ``topoogical_sort``: For sorting the river network topologically which is useful for routing
           and flow accumulation.
@@ -121,14 +121,18 @@
         These utilities are developed based on an ``R`` package called
         `nhdplusTools <https://github.com/USGS-R/nhdplusTools>`__.
         
         You can try using PyNHD without installing it on you system by clicking on the binder badge
         below the PyNHD banner. A Jupyter notebook instance with the Hydrodata software stack
         pre-installed will be launched in your web browser and you can start coding!
         
+        Please note that since Hydrodata is in early development stages, while the provided
+        functionaities should be stable, changes in APIs are possible in new releases. But we
+        appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+        
         Moreover, requests for additional functionalities can be submitted via
         `issue tracker <https://github.com/cheginit/pynhd/issues>`__.
         
         Installation
         ------------
         
         You can install PyNHD using ``pip`` after installing ``libgdal`` on your system
@@ -157,87 +161,112 @@
         
         First, let’s get the watershed geometry of the contributing basin of a
         USGS station using ``NLDI``:
         
         .. code:: python
         
             nldi = NLDI()
-            station_id = "USGS-01031500"
-            ut = "upstreamTributaries"
-            um = "upstreamMain"
+            station_id = "01031500"
         
-            basin = nldi.getfeature_byid("nwissite", station_id, basin=True)
+            basin = nldi.get_basins(station_id)
         
         The ``navigate_byid`` class method can be used to navigate NHDPlus in
         both upstream and downstream of any point in the database. Let’s get ComIDs and flowlines
         of the tributaries and the main river channel in the upstream of the station.
         
         .. code:: python
         
-            args = {
-                "fsource": "nwissite",
-                "fid": station_id,
-                "navigation": um,
-                "source": "flowlines",
-                "distance": 1000,
-            }
-        
-            flw_main = nldi.navigate_byid(**args)
-        
-            args["navigation"] = ut
-            flw_trib = nldi.navigate_byid(**args)
+            flw_main = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamMain",
+                source="flowlines",
+                distance=1000,
+            )
+        
+            flw_trib = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamTributaries",
+                source="flowlines",
+                distance=1000,
+            )
         
         We can get other USGS stations upstream (or downstream) of the station
         and even set a distance limit (in km):
         
         .. code:: python
         
-            args.update({
-                "source" : "nwissite",
-            })
-            st_all = nldi.navigate_byid(**args)
-        
-            args.update({
-                "distance": 20,
-                "source" : "nwissite",
-            })
-            st_d20 = nldi.navigate_byid(**args)
+            st_all = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamTributaries",
+                source="nwissite",
+                distance=1000,
+            )
+        
+            st_d20 = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamTributaries",
+                source="nwissite",
+                distance=20,
+            )
         
         Now, let’s get the `HUC12 pour
         points <https://www.sciencebase.gov/catalog/item/5762b664e4b07657d19a71ea>`__:
         
         .. code:: python
         
-            args.update({
-                "distance": 1000,
-                "source" : "huc12pp",
-            })
-            pp = nldi.navigate_byid(**args)
+            pp = nldi.navigate_byid(
+                fsource="nwissite",
+                fid=f"USGS-{station_id}",
+                navigation="upstreamTributaries",
+                source="huc12pp",
+                distance=1000,
+            )
         
         .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_12_0.png
             :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_12_0.png
             :width: 400
             :align: center
         
-        Now, let's get the medium- and high-resolution flowlines within the bounding box of this watershed
-        and compare them.
+        Next, we retrieve the medium- and high-resolution flowlines within the bounding box of our
+        watershed and compare them. Moreover, Since serveral web services offer access to NHDPlus database,
+        ``NHDPlusHR`` has an argument for selecting a service and also an argument for automatically
+        switching between services.
         
         .. code:: python
         
             mr = WaterData("nhdflowline_network")
             nhdp_mr = mr.bybox(basin.geometry[0].bounds)
         
-            hr = NHDPlusHR("networknhdflowline")
+            hr = NHDPlusHR("networknhdflowline", service="hydro", auto_switch=True)
             nhdp_hr = hr.bygeom(basin.geometry[0].bounds)
         
         .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hr_mr.png
             :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hr_mr.png
             :width: 400
             :align: center
         
+        Moreover, ``WaterData`` can find features within a given radius (in meters) of a point:
+        
+        .. code:: python
+        
+            eck4 = "+proj=eck4 +lon_0=0 +x_0=0 +y_0=0 +datum=WGS84 +units=m +no_defs"
+            coords = (-5727797.427596455, 5584066.49330473)
+            rad = 5e3
+            flw_rad = mr.bydistance(coords, rad, loc_crs=eck4)
+            flw_rad = flw_rad.to_crs(eck4)
+        
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_radius.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/nhdplus_radius.png
+            :width: 400
+            :align: center
+        
         Since NHDPlus HR is still at the pre-release stage let's use the MR flowlines to
         demonstrate the vector-based accumulation.
         Based on a topological sorted river network
         ``pynhd.vector_accumulation`` computes flow accumulation in the network.
         It returns a dataframe which is sorted from upstream to downstream that
         shows the accumulated flow in each node.
         
@@ -253,16 +282,16 @@
         
             wd = WaterData("nhdflowline_network")
         
             comids = flw_trib.nhdplus_comid.to_list()
             nhdp_trib = wd.byid("comid", comids)
             flw = nhd.prepare_nhdplus(nhdp_trib, 0, 0, purge_non_dendritic=False)
         
-        Now, let’s get Mean Annual Groundwater Recharge using ``getcharacteristic_byid``
-        class method and carry out the accumulation.
+        To demostrate the use of routing, let's use ``nhdplus_attrs`` function to get list of available
+        NHDPlus attributes
         
         .. code:: python
         
             char = "CAT_RECHG"
             area = "areasqkm"
         
             local = nldi.getcharacteristic_byid(comids, "local", char_ids=char)
```

### Comparing `pynhd-0.2.0/pynhd.egg-info/SOURCES.txt` & `pynhd-0.9.0/pynhd.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug-report.md
 .github/ISSUE_TEMPLATE/feature-request.md
 .github/workflows/codeql-analysis.yml
 .github/workflows/lint.yml
-.github/workflows/python-publish.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 ci/requirements/environment.yml
 ci/requirements/py3.6.yml
 ci/requirements/py3.7.yml
 ci/requirements/py3.8.yml
 ci/requirements/py3.9.yml
@@ -44,10 +43,9 @@
 pynhd.egg-info/PKG-INFO
 pynhd.egg-info/SOURCES.txt
 pynhd.egg-info/dependency_links.txt
 pynhd.egg-info/not-zip-safe
 pynhd.egg-info/requires.txt
 pynhd.egg-info/top_level.txt
 scripts/generate_pip_deps_from_conda.py
-tests/__init__.py
 tests/test_exceptions.py
 tests/test_pynhd.py
```

### Comparing `pynhd-0.2.0/scripts/generate_pip_deps_from_conda.py` & `pynhd-0.9.0/scripts/generate_pip_deps_from_conda.py`

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

### Comparing `pynhd-0.2.0/setup.cfg` & `pynhd-0.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,22 @@
 known_first_party = pynhd
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

### Comparing `pynhd-0.2.0/setup.py` & `pynhd-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pynhd-0.2.0/tests/test_exceptions.py` & `pynhd-0.9.0/tests/test_exceptions.py`

 * *Files identical despite different names*

