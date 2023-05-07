# Comparing `tmp/pygeoutils-0.2.0.tar.gz` & `tmp/pygeoutils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygeoutils-0.2.0.tar", last modified: Mon Dec  7 00:41:26 2020, max compression
+gzip compressed data, was "pygeoutils-0.9.0.tar", last modified: Wed Feb 17 18:20:01 2021, max compression
```

## Comparing `pygeoutils-0.2.0.tar` & `pygeoutils-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.202984 pygeoutils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)      146 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (116)      101 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)      242 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.198984 pygeoutils-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.198984 pygeoutils-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      927 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (116)      684 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (116)      125 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.198984 pygeoutils-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2584 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (116)      288 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1163 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1208 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      163 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1583 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      157 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3444 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4111 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1702 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      150 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2192 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     8896 2020-12-07 00:41:26.202984 pygeoutils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6680 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.198984 pygeoutils-0.2.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.198984 pygeoutils-0.2.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)      364 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (116)      360 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/ci/requirements/py3.6.yml
--rw-r--r--   0 runner    (1001) docker     (116)      344 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/ci/requirements/py3.7.yml
--rw-r--r--   0 runner    (1001) docker     (116)      344 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/ci/requirements/py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (116)      344 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/ci/requirements/py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.198984 pygeoutils-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     8187 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.202984 pygeoutils-0.2.0/docs/_template/
--rw-r--r--   0 runner    (1001) docker     (116)       85 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/docs/_template/layout.html
--rw-r--r--   0 runner    (1001) docker     (116)    11937 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      771 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       73 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (116)      646 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/docs/pygeoutils.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.202984 pygeoutils-0.2.0/pygeoutils/
--rw-r--r--   0 runner    (1001) docker     (116)      503 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/pygeoutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1945 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/pygeoutils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     5079 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/pygeoutils/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (116)    17987 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/pygeoutils/pygeoutils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.202984 pygeoutils-0.2.0/pygeoutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8896 2020-12-07 00:41:26.000000 pygeoutils-0.2.0/pygeoutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1136 2020-12-07 00:41:26.000000 pygeoutils-0.2.0/pygeoutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 00:41:26.000000 pygeoutils-0.2.0/pygeoutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 00:41:26.000000 pygeoutils-0.2.0/pygeoutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      160 2020-12-07 00:41:26.000000 pygeoutils-0.2.0/pygeoutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2020-12-07 00:41:26.000000 pygeoutils-0.2.0/pygeoutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      292 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.202984 pygeoutils-0.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)     4671 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/scripts/generate_pip_deps_from_conda.py
--rw-r--r--   0 runner    (1001) docker     (116)     1959 2020-12-07 00:41:26.206984 pygeoutils-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 00:41:26.202984 pygeoutils-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      428 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     5099 2020-12-07 00:41:21.000000 pygeoutils-0.2.0/tests/test_pygeoutils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      101 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (116)      242 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (116)      927 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (116)      684 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (116)      321 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2719 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1306 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1351 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1226 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      163 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1867 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      157 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3444 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4111 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2097 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1096 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      150 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2192 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)     9380 2021-02-17 18:20:01.825861 pygeoutils-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     7084 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.817861 pygeoutils-0.9.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (116)      379 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      374 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/ci/requirements/py3.6.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      358 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/ci/requirements/py3.7.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      358 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/ci/requirements/py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      358 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/ci/requirements/py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     8187 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/docs/_template/
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/docs/_template/layout.html
+-rw-r--r--   0 runner    (1001) docker     (116)    11937 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      771 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (116)       73 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      646 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/docs/pygeoutils.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/pygeoutils/
+-rw-r--r--   0 runner    (1001) docker     (116)      519 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/pygeoutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1945 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/pygeoutils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5251 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/pygeoutils/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21482 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/pygeoutils/pygeoutils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/pygeoutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     9380 2021-02-17 18:20:01.000000 pygeoutils-0.9.0/pygeoutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1136 2021-02-17 18:20:01.000000 pygeoutils-0.9.0/pygeoutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:20:01.000000 pygeoutils-0.9.0/pygeoutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:20:01.000000 pygeoutils-0.9.0/pygeoutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      171 2021-02-17 18:20:01.000000 pygeoutils-0.9.0/pygeoutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2021-02-17 18:20:01.000000 pygeoutils-0.9.0/pygeoutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      303 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4753 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/scripts/generate_pip_deps_from_conda.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2125 2021-02-17 18:20:01.825861 pygeoutils-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      587 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:01.821861 pygeoutils-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      428 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5754 2021-02-17 18:19:55.000000 pygeoutils-0.9.0/tests/test_pygeoutils.py
```

### Comparing `pygeoutils-0.2.0/.github/ISSUE_TEMPLATE/bug-report.md` & `pygeoutils-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/.github/ISSUE_TEMPLATE/feature-request.md` & `pygeoutils-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/.github/workflows/codeql-analysis.yml` & `pygeoutils-0.9.0/.github/workflows/codeql-analysis.yml`

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

### Comparing `pygeoutils-0.2.0/.github/workflows/release.yml` & `pygeoutils-0.9.0/.github/workflows/release.yml`

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

### Comparing `pygeoutils-0.2.0/.github/workflows/test.yml` & `pygeoutils-0.9.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

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
           activate-environment: pygeoutils
           python-version: ${{ matrix.python-version }}
           environment-file: ci/requirements/py${{ matrix.python-version }}.yml
```

### Comparing `pygeoutils-0.2.0/.gitignore` & `pygeoutils-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/.pre-commit-config.yaml` & `pygeoutils-0.9.0/.pre-commit-config.yaml`

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
-        files: pygeoutils
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
-        args: [-lll, --recursive, pygeoutils]
+        args: [-lll, --recursive, pynhd]
         files: .py$
```

### Comparing `pygeoutils-0.2.0/CODE_OF_CONDUCT.rst` & `pygeoutils-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/CONTRIBUTING.rst` & `pygeoutils-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/HISTORY.rst` & `pygeoutils-0.9.0/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =======
 History
 =======
 
+0.9.0 (2021-02-14)
+------------------
+
+- Bump version to the same version as Hydrodata.
+- Add ``gtiff2file`` for saving raster responses as ``geotiff`` file(s).
+- Fix an error in ``_get_nodata_crs`` for handling nodata value when its value in the source
+  is None.
+- Fix the warning during the ``GeoDataFrame`` generation in ``json2geodf`` when there is
+  no geometry column in the input json.
+
 0.2.0 (2020-12-06)
 -------------------
 
 - Added checking the validity of input arguments in ``gtiff2xarray`` function and provide
   useful messages for debugging.
 - Add support for multipolygon.
 - Remove the ``fill_hole`` argument.
```

### Comparing `pygeoutils-0.2.0/LICENSE` & `pygeoutils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/Makefile` & `pygeoutils-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/PKG-INFO` & `pygeoutils-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: pygeoutils
-Version: 0.2.0
+Version: 0.9.0
 Summary: A set of utilities for manipulating (Geo)JSON and (Geo)TIFF data.
 Home-page: https://github.com/cheginit/pygeoutils
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT license
 Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pygeoutils_logo.png
             :target: https://github.com/cheginit/pygeoutils
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
@@ -85,30 +85,34 @@
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
             :target: https://github.com/pre-commit/pre-commit
             :alt: pre-commit
         
         |
         
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
         Features
         --------
         
         PyGeoUtils is a part of Hydrodata software stack and provides utilities for manipulating
         (Geo)JSON and (Geo)TIFF data. These utilities are:
         
         - ``json2geodf``: For converting (Geo)JSON objects to GroPandas dataframe.
         - ``arcgis2geojson``: For converting ESRIGeoJSON objects to standard GeoJSON format.
         - ``gtiff2xarray``: For converting (Geo)TIFF objects to `xarray <https://xarray.pydata.org/>`__
           datasets.
+        - ``gtiff2file``: For saving (Geo)TIFF objects to a raster file.
         - ``xarray_geomask``: For masking a ``xarray.Dataset`` or ``xarray.DataArray`` using a polygon.
         
-        All these function handle all necessary CRS transformations. Moreover, requests for additional
-        functionalities can be submitted via
+        All these functions handle all necessary CRS transformations.
+        
+        Please note that since Hydrodata is in early development stages, while the provided
+        functionaities should be stable, changes in APIs are possible in new releases. But we
+        appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+        
+        Moreover, requests for additional functionalities can be submitted via
         `issue tracker <https://github.com/cheginit/pygeoutils/issues>`__.
         
         Installation
         ------------
         
         You can install PyGeoUtils using ``pip`` after installing ``libgdal`` on your system
         (for example, in Ubuntu run ``sudo apt install libgdal-dev``):
@@ -127,15 +131,15 @@
         Quick start
         -----------
         
         To demonstrate capabilities of PyGeoUtils lets use
         `PyGeoOGC <https://github.com/cheginit/pygeoogc>`__ to access
         `National Wetlands Inventory <https://www.fws.gov/wetlands/>`__ from WMS, and
         `FEMA National Flood Hazard <https://www.fema.gov/national-flood-hazard-layer-nfhl>`__
-        via WFS, then convert the output to ``GeoDataFrame`` and ``xarray.Dataset`` using PyGeoUtils.
+        via WFS, then convert the output to ``xarray.Dataset`` and ``GeoDataFrame``, respectively.
         
         .. code-block:: python
         
             import pygeoutils as geoutils
             from pygeoogc import WFS, WMS
             from shapely.geometry import Polygon
         
@@ -170,14 +174,20 @@
                 layer="public_NFHL:Base_Flood_Elevations",
                 outformat="esrigeojson",
                 crs="epsg:4269",
             )
             r = wfs.getfeature_bybox(geometry.bounds, box_crs="epsg:4326")
             flood = geoutils.json2geodf(r.json(), "epsg:4269", "epsg:4326")
         
+        We can also save WMS outpus as raster file using ``gtiff2file``:
+        
+        .. code-block:: python
+        
+            geoutils.gtiff2file(r_dict, geometry, "epsg:4326", "raster")
+        
         Contributing
         ------------
         
         Contributions are very welcomed. Please read
         `CONTRIBUTING.rst <https://github.com/cheginit/pygeoogc/blob/master/CONTRIBUTING.rst>`__
         file for instructions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygeoutils-0.2.0/README.rst` & `pygeoutils-0.9.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pygeoutils_logo.png
     :target: https://github.com/cheginit/pygeoutils
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
@@ -77,30 +77,34 @@
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
     :target: https://github.com/pre-commit/pre-commit
     :alt: pre-commit
 
 |
 
-🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-
 Features
 --------
 
 PyGeoUtils is a part of Hydrodata software stack and provides utilities for manipulating
 (Geo)JSON and (Geo)TIFF data. These utilities are:
 
 - ``json2geodf``: For converting (Geo)JSON objects to GroPandas dataframe.
 - ``arcgis2geojson``: For converting ESRIGeoJSON objects to standard GeoJSON format.
 - ``gtiff2xarray``: For converting (Geo)TIFF objects to `xarray <https://xarray.pydata.org/>`__
   datasets.
+- ``gtiff2file``: For saving (Geo)TIFF objects to a raster file.
 - ``xarray_geomask``: For masking a ``xarray.Dataset`` or ``xarray.DataArray`` using a polygon.
 
-All these function handle all necessary CRS transformations. Moreover, requests for additional
-functionalities can be submitted via
+All these functions handle all necessary CRS transformations.
+
+Please note that since Hydrodata is in early development stages, while the provided
+functionaities should be stable, changes in APIs are possible in new releases. But we
+appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+
+Moreover, requests for additional functionalities can be submitted via
 `issue tracker <https://github.com/cheginit/pygeoutils/issues>`__.
 
 Installation
 ------------
 
 You can install PyGeoUtils using ``pip`` after installing ``libgdal`` on your system
 (for example, in Ubuntu run ``sudo apt install libgdal-dev``):
@@ -119,15 +123,15 @@
 Quick start
 -----------
 
 To demonstrate capabilities of PyGeoUtils lets use
 `PyGeoOGC <https://github.com/cheginit/pygeoogc>`__ to access
 `National Wetlands Inventory <https://www.fws.gov/wetlands/>`__ from WMS, and
 `FEMA National Flood Hazard <https://www.fema.gov/national-flood-hazard-layer-nfhl>`__
-via WFS, then convert the output to ``GeoDataFrame`` and ``xarray.Dataset`` using PyGeoUtils.
+via WFS, then convert the output to ``xarray.Dataset`` and ``GeoDataFrame``, respectively.
 
 .. code-block:: python
 
     import pygeoutils as geoutils
     from pygeoogc import WFS, WMS
     from shapely.geometry import Polygon
 
@@ -162,13 +166,19 @@
         layer="public_NFHL:Base_Flood_Elevations",
         outformat="esrigeojson",
         crs="epsg:4269",
     )
     r = wfs.getfeature_bybox(geometry.bounds, box_crs="epsg:4326")
     flood = geoutils.json2geodf(r.json(), "epsg:4269", "epsg:4326")
 
+We can also save WMS outpus as raster file using ``gtiff2file``:
+
+.. code-block:: python
+
+    geoutils.gtiff2file(r_dict, geometry, "epsg:4326", "raster")
+
 Contributing
 ------------
 
 Contributions are very welcomed. Please read
 `CONTRIBUTING.rst <https://github.com/cheginit/pygeoogc/blob/master/CONTRIBUTING.rst>`__
 file for instructions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygeoutils-0.2.0/docs/Makefile` & `pygeoutils-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/docs/conf.py` & `pygeoutils-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/docs/make.bat` & `pygeoutils-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/docs/pygeoutils.rst` & `pygeoutils-0.9.0/docs/pygeoutils.rst`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/pygeoutils/exceptions.py` & `pygeoutils-0.9.0/pygeoutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/pygeoutils/print_versions.py` & `pygeoutils-0.9.0/pygeoutils/print_versions.py`

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

### Comparing `pygeoutils-0.2.0/pygeoutils/pygeoutils.py` & `pygeoutils-0.9.0/pygeoutils/pygeoutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Some utilities for manipulating GeoSpatial data."""
+import contextlib
 import numbers
+import os
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 from warnings import warn
 
 import affine
 import geopandas as gpd
 import numpy as np
 import orjson as json
@@ -44,22 +47,31 @@
     """
     if not isinstance(content, (list, dict)):
         raise InvalidInputType("content", "list or list of dict ((geo)json)")
 
     content = content if isinstance(content, list) else [content]
     try:
         geodf = gpd.GeoDataFrame.from_features(content[0], crs=in_crs)
+    except AttributeError:
+        geodf = gpd.GeoDataFrame.from_features(content[0])
     except TypeError:
         content = [arcgis2geojson(c) for c in content]
-        geodf = gpd.GeoDataFrame.from_features(content[0], crs=in_crs)
+        try:
+            geodf = gpd.GeoDataFrame.from_features(content[0], crs=in_crs)
+        except AttributeError:
+            geodf = gpd.GeoDataFrame.from_features(content[0])
 
     if len(content) > 1:
-        geodf = geodf.append([gpd.GeoDataFrame.from_features(c, crs=in_crs) for c in content[1:]])
+        for c in content[1:]:
+            try:
+                geodf = geodf.append(gpd.GeoDataFrame.from_features(c, crs=in_crs))
+            except AttributeError:
+                geodf = gpd.GeoDataFrame.from_features(c)
 
-    if in_crs != crs:
+    if in_crs != crs and "geometry" in geodf:
         geodf = geodf.to_crs(crs)
 
     return geodf
 
 
 def arcgis2geojson(arcgis: Dict[str, Any], id_attr: Optional[str] = None) -> Dict[str, Any]:
     """Convert ESRIGeoJSON format to GeoJSON.
@@ -77,17 +89,17 @@
 
     Returns
     -------
     dict
         A GeoJSON file readable by GeoPandas
     """
 
-    def convert(arcgis, id_attr=None):
+    def convert(arcgis: Dict[str, Any], id_attr: Optional[str] = None) -> Dict[str, Any]:
         """Convert an ArcGIS JSON object to a GeoJSON object."""
-        geojson = {}
+        geojson: Dict[str, Any] = {}
 
         if "features" in arcgis and arcgis["features"]:
             geojson["type"] = "FeatureCollection"
             geojson["features"] = [convert(feature, id_attr) for feature in arcgis["features"]]
 
         if (
             "x" in arcgis
@@ -160,15 +172,15 @@
                 geojson["properties"] = None
 
         if "geometry" in geojson and not geojson["geometry"]:
             geojson["geometry"] = None
 
         return geojson
 
-    def rings2geojson(rings):
+    def rings2geojson(rings: List[List[List[float]]]) -> Dict[str, Any]:
         """Check for holes in the ring and fill them."""
         outer_rings = []
         holes = []
         x = None  # iterable
         outer_ring = None  # current outer ring being evaluated
         hole = None  # current hole being evaluated
 
@@ -247,14 +259,44 @@
 
     if isinstance(arcgis, str):
         return json.dumps(convert(json.loads(arcgis), id_attr))
 
     return convert(arcgis, id_attr)
 
 
+def _get_nodata_crs(resp: bytes, driver: str) -> Tuple[np.float64, pyproj.crs.crs.CRS]:
+    """Get nodata and crs value of a raster in bytes.
+
+    Parameters
+    ----------
+    resp : bytes
+        Raster response returned from a wed service request such as WMS
+    driver : str
+        A GDAL driver for reading the content, defaults to GTiff. A list of the drivers
+        can be found here: https://gdal.org/drivers/raster/index.html
+
+    Returns
+    -------
+    tuple
+        (NoData, CRS)
+    """
+    with rio.MemoryFile() as memfile:
+        memfile.write(resp)
+        with memfile.open(driver=driver) as src:
+            r_crs = pyproj.CRS.from_user_input(src.crs)
+            if src.nodata is None:
+                try:
+                    nodata = np.iinfo(src.dtypes[0]).max
+                except ValueError:
+                    nodata = np.nan
+            else:
+                nodata = np.dtype(src.dtypes[0]).type(src.nodata)
+    return nodata, r_crs
+
+
 def gtiff2xarray(
     r_dict: Dict[str, bytes],
     geometry: Union[Polygon, MultiPolygon, Tuple[float, float, float, float]],
     geo_crs: str,
     ds_dims: Tuple[str, str] = ("y", "x"),
     driver: str = "GTiff",
 ) -> Union[xr.DataArray, xr.Dataset]:
@@ -282,41 +324,25 @@
     """
     if not isinstance(r_dict, dict):
         raise InvalidInputType("r_dict", "dict", '{"name": Response.content}')
 
     key1 = next(iter(r_dict.keys()))
     if len(r_dict) == 1 and "dd" not in key1:
         r_dict = {f"{key1}_dd_0_0": r_dict[key1]}
+        key1 = f"{key1}_dd_0_0"
 
     var_name = {lyr: "_".join(lyr.split("_")[:-3]) for lyr in r_dict.keys()}
 
-    with rio.MemoryFile() as memfile:
-        memfile.write(r_dict[next(iter(r_dict.keys()))])
-        with memfile.open(driver=driver) as src:
-            r_crs = pyproj.CRS.from_user_input(src.crs)
-            if src.nodata is None:
-                try:
-                    nodata = np.iinfo(src.dtypes[0]).max
-                except ValueError:
-                    nodata = np.nan
-            else:
-                nodata = np.dtype(src.dtypes[0]).type(src.nodata)
-
-            ds = xr.open_rasterio(src)
-            valid_dims = list(ds.sizes)
-            if any(d not in valid_dims for d in ds_dims):
-                raise InvalidInputValue("ds_dims", valid_dims)
+    nodata, r_crs = _get_nodata_crs(r_dict[key1], driver)
 
     _geometry = geo2polygon(geometry, geo_crs, r_crs)
-    if not _geometry.is_valid:
-        _geometry = _geometry.buffer(0.0)
 
-    def to_dataset(lyr: str) -> xr.DataArray:
+    def to_dataset(lyr: str, resp: bytes) -> xr.DataArray:
         with rio.MemoryFile() as memfile:
-            memfile.write(r_dict[lyr])
+            memfile.write(resp)
             with memfile.open(driver=driver) as src:
                 geom = [_geometry.intersection(box(*src.bounds))]
                 if geom[0].is_empty:
                     msk, transform, _ = rio_mask.raster_geometry_mask(src, [_geometry], invert=True)
                 else:
                     msk, transform, _ = rio_mask.raster_geometry_mask(src, geom, invert=True)
                 meta = src.meta
@@ -328,39 +354,103 @@
                         "transform": transform,
                         "nodata": nodata,
                     }
                 )
 
                 with rio.vrt.WarpedVRT(src, **meta) as vrt:
                     ds = xr.open_rasterio(vrt)
-                    try:
+                    valid_dims = list(ds.sizes)
+                    if any(d not in valid_dims for d in ds_dims):
+                        raise InvalidInputValue("ds_dims", valid_dims)
+                    with contextlib.suppress(ValueError):
                         ds = ds.squeeze("band", drop=True)
-                    except ValueError:
-                        pass
+
                     coords = {ds_dims[0]: ds.coords[ds_dims[0]], ds_dims[1]: ds.coords[ds_dims[1]]}
                     msk_da = xr.DataArray(msk, coords, dims=ds_dims)
                     ds = ds.where(msk_da, drop=True)
                     ds.attrs["crs"] = r_crs.to_string()
                     ds.name = var_name[lyr]
                     return ds
 
-    ds = xr.merge(to_dataset(lyr) for lyr in r_dict.keys())
+    ds = xr.merge(to_dataset(lyr, resp) for lyr, resp in r_dict.items())
     ds.attrs["crs"] = r_crs.to_string()
 
     if len(ds.variables) - len(ds.dims) == 1:
         ds = ds[list(ds.keys())[0]]
     return ds
 
 
+def gtiff2file(
+    r_dict: Dict[str, bytes],
+    geometry: Union[Polygon, MultiPolygon, Tuple[float, float, float, float]],
+    geo_crs: str,
+    output: Union[str, Path] = ".",
+    driver: str = "GTiff",
+) -> None:
+    """Save responses from ``pygeoogc.wms_bybox`` to raster file(s).
+
+    Parameters
+    ----------
+    r_dict : dict
+        The output of ``wms_bybox`` function.
+    geometry : Polygon, MultiPolygon, or tuple
+        The geometry to mask the data that should be in the same CRS as the r_dict.
+    geo_crs : str
+        The spatial reference of the input geometry.
+    output : str
+        Path to a folder saving files. File names are keys of the input dictionary, so
+        each layer becomes one file. Defaults to current directory.
+    driver : str, optional
+        A GDAL driver for reading the content, defaults to GTiff. A list of the drivers
+        can be found here: https://gdal.org/drivers/raster/index.html
+    """
+    os.makedirs(output, exist_ok=True)
+
+    if not isinstance(r_dict, dict):
+        raise InvalidInputType("r_dict", "dict", '{"name": Response.content}')
+
+    key1 = next(iter(r_dict.keys()))
+    if len(r_dict) == 1 and "dd" not in key1:
+        r_dict = {f"{key1}_dd_0_0": r_dict[key1]}
+        key1 = f"{key1}_dd_0_0"
+
+    nodata, r_crs = _get_nodata_crs(r_dict[key1], driver)
+
+    _geometry = geo2polygon(geometry, geo_crs, r_crs)
+
+    for lyr, resp in r_dict.items():
+        with rio.MemoryFile() as memfile:
+            memfile.write(resp)
+            with memfile.open(driver=driver) as src:
+                geom = [_geometry.intersection(box(*src.bounds))]
+                if geom[0].is_empty:
+                    data, transform = rio_mask.mask(src, [_geometry], crop=True)
+                else:
+                    data, transform = rio_mask.mask(src, geom, crop=True)
+                meta = src.meta
+                meta.update(
+                    {
+                        "driver": "GTiff",
+                        "height": data.shape[1],
+                        "width": data.shape[2],
+                        "transform": transform,
+                        "nodata": nodata,
+                    }
+                )
+
+                with rio.open(Path(output, f"{lyr}.gtiff"), "w", **meta) as dest:
+                    dest.write(data)
+
+
 def xarray_geomask(
     ds: Union[xr.Dataset, xr.DataArray],
     geometry: Union[Polygon, MultiPolygon, Tuple[float, float, float, float]],
     geo_crs: str,
     ds_dims: Tuple[str, str] = ("y", "x"),
-):
+) -> Union[xr.Dataset, xr.DataArray]:
     """Mask a ``xarray.Dataset`` based on a geometry.
 
     Parameters
     ----------
     ds : xarray.Dataset or xarray.DataArray
         The dataset(array) to be masked
     geometry : Polygon, MultiPolygon, or tuple of length 4
@@ -461,15 +551,15 @@
         geom: Tuple[float, float, float, float], in_crs: str, out_crs: str
     ) -> Tuple[float, float, float, float]:
         """Transform a bounding box ``(west, south, east, north)``."""
         if not isinstance(geom, tuple) and len(geom) != 4:
             raise InvalidInputType("geom", "tuple of length 4", "(west, south, east, north)")
 
         project = pyproj.Transformer.from_crs(in_crs, out_crs, always_xy=True).transform
-        return ops.transform(project, box(*geom)).bounds
+        return ops.transform(project, box(*geom)).bounds  # type: ignore
 
     @staticmethod
     def coords(
         geom: Tuple[Tuple[float, ...], Tuple[float, ...]], in_crs: str, out_crs: str
     ) -> Tuple[Any, ...]:
         """Transform a set of coordinates in form of ((xs), (ys))."""
         if not isinstance(geom, tuple) and len(geom) != 2:
@@ -502,14 +592,18 @@
         The target spatial reference.
 
     Returns
     -------
     Polygon
         A Polygon in the target CRS.
     """
-    if isinstance(geometry, tuple):
-        return box(*MatchCRS.bounds(geometry, geo_crs, crs))  # type: ignore
+    if not isinstance(geometry, (Polygon, MultiPolygon, tuple)):
+        raise InvalidInputType("geometry", "Polygon, MultiPolygon, or tuple of length 4")
 
-    if isinstance(geometry, (Polygon, MultiPolygon)):
-        return MatchCRS.geometry(geometry, geo_crs, crs)
-
-    raise InvalidInputType("geometry", "Polygon, MultiPolygon, or tuple of length 4")
+    if isinstance(geometry, tuple):
+        geom = box(*MatchCRS.bounds(geometry, geo_crs, crs))  # type: ignore
+    elif isinstance(geometry, (Polygon, MultiPolygon)):
+        geom = MatchCRS.geometry(geometry, geo_crs, crs)
+
+    if not geom.is_valid:
+        geom = geom.buffer(0.0)
+    return geom
```

### Comparing `pygeoutils-0.2.0/pygeoutils.egg-info/PKG-INFO` & `pygeoutils-0.9.0/pygeoutils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: pygeoutils
-Version: 0.2.0
+Version: 0.9.0
 Summary: A set of utilities for manipulating (Geo)JSON and (Geo)TIFF data.
 Home-page: https://github.com/cheginit/pygeoutils
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT license
 Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pygeoutils_logo.png
             :target: https://github.com/cheginit/pygeoutils
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
@@ -85,30 +85,34 @@
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
             :target: https://github.com/pre-commit/pre-commit
             :alt: pre-commit
         
         |
         
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
         Features
         --------
         
         PyGeoUtils is a part of Hydrodata software stack and provides utilities for manipulating
         (Geo)JSON and (Geo)TIFF data. These utilities are:
         
         - ``json2geodf``: For converting (Geo)JSON objects to GroPandas dataframe.
         - ``arcgis2geojson``: For converting ESRIGeoJSON objects to standard GeoJSON format.
         - ``gtiff2xarray``: For converting (Geo)TIFF objects to `xarray <https://xarray.pydata.org/>`__
           datasets.
+        - ``gtiff2file``: For saving (Geo)TIFF objects to a raster file.
         - ``xarray_geomask``: For masking a ``xarray.Dataset`` or ``xarray.DataArray`` using a polygon.
         
-        All these function handle all necessary CRS transformations. Moreover, requests for additional
-        functionalities can be submitted via
+        All these functions handle all necessary CRS transformations.
+        
+        Please note that since Hydrodata is in early development stages, while the provided
+        functionaities should be stable, changes in APIs are possible in new releases. But we
+        appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+        
+        Moreover, requests for additional functionalities can be submitted via
         `issue tracker <https://github.com/cheginit/pygeoutils/issues>`__.
         
         Installation
         ------------
         
         You can install PyGeoUtils using ``pip`` after installing ``libgdal`` on your system
         (for example, in Ubuntu run ``sudo apt install libgdal-dev``):
@@ -127,15 +131,15 @@
         Quick start
         -----------
         
         To demonstrate capabilities of PyGeoUtils lets use
         `PyGeoOGC <https://github.com/cheginit/pygeoogc>`__ to access
         `National Wetlands Inventory <https://www.fws.gov/wetlands/>`__ from WMS, and
         `FEMA National Flood Hazard <https://www.fema.gov/national-flood-hazard-layer-nfhl>`__
-        via WFS, then convert the output to ``GeoDataFrame`` and ``xarray.Dataset`` using PyGeoUtils.
+        via WFS, then convert the output to ``xarray.Dataset`` and ``GeoDataFrame``, respectively.
         
         .. code-block:: python
         
             import pygeoutils as geoutils
             from pygeoogc import WFS, WMS
             from shapely.geometry import Polygon
         
@@ -170,14 +174,20 @@
                 layer="public_NFHL:Base_Flood_Elevations",
                 outformat="esrigeojson",
                 crs="epsg:4269",
             )
             r = wfs.getfeature_bybox(geometry.bounds, box_crs="epsg:4326")
             flood = geoutils.json2geodf(r.json(), "epsg:4269", "epsg:4326")
         
+        We can also save WMS outpus as raster file using ``gtiff2file``:
+        
+        .. code-block:: python
+        
+            geoutils.gtiff2file(r_dict, geometry, "epsg:4326", "raster")
+        
         Contributing
         ------------
         
         Contributions are very welcomed. Please read
         `CONTRIBUTING.rst <https://github.com/cheginit/pygeoogc/blob/master/CONTRIBUTING.rst>`__
         file for instructions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygeoutils-0.2.0/pygeoutils.egg-info/SOURCES.txt` & `pygeoutils-0.9.0/pygeoutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/scripts/generate_pip_deps_from_conda.py` & `pygeoutils-0.9.0/scripts/generate_pip_deps_from_conda.py`

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

### Comparing `pygeoutils-0.2.0/setup.cfg` & `pygeoutils-0.9.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -65,14 +65,22 @@
 known_first_party = pygeoutils
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

### Comparing `pygeoutils-0.2.0/setup.py` & `pygeoutils-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pygeoutils-0.2.0/tests/test_pygeoutils.py` & `pygeoutils-0.9.0/tests/test_pygeoutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Tests for PyGeoUtils"""
 import io
+import shutil
 
 import pytest
+import rasterio
 from pygeoogc import WFS, WMS
 from shapely.geometry import Polygon
 
 import pygeoutils as geoutils
 from pygeoutils import MatchCRS
 
 DEF_CRS = "epsg:4326"
@@ -29,37 +31,59 @@
             [-118.72, 34.118],
         ]
     )
 
 
 @pytest.mark.flaky(max_runs=3)
 def test_gtiff2array(geometry_nat):
-    url_wms = "https://www.fws.gov/wetlands/arcgis/services/Wetlands_Raster/ImageServer/WMSServer"
+    url_wms = "https://www.mrlc.gov/geoserver/mrlc_download/wms"
     wms = WMS(
         url_wms,
-        layers="0",
-        outformat="image/tiff",
-        crs="epsg:3857",
+        layers="NLCD_Land_Cover_Change_Index_Science_product_L48",
+        outformat="image/geotiff",
+        crs=DEF_CRS,
     )
     r_dict = wms.getmap_bybox(
         geometry_nat.bounds,
         1e3,
         box_crs=DEF_CRS,
     )
-    wetlands_box = geoutils.gtiff2xarray(r_dict, geometry_nat.bounds, DEF_CRS)
-    wetlands_msk = geoutils.xarray_geomask(wetlands_box, geometry_nat, DEF_CRS)
-    wetlands = geoutils.gtiff2xarray(r_dict, geometry_nat, DEF_CRS)
+    cover_box = geoutils.gtiff2xarray(r_dict, geometry_nat.bounds, DEF_CRS)
+    cover_msk = geoutils.xarray_geomask(cover_box, geometry_nat, DEF_CRS)
+    cover = geoutils.gtiff2xarray(r_dict, geometry_nat, DEF_CRS)
 
     assert (
-        abs(wetlands_msk.isel(band=0).mean().values.item() - 16.542) < 1e-3
-        and abs(wetlands.isel(band=0).mean().values.item() - 16.542) < 1e-3
+        abs(cover_msk.mean().values.item() - 2.444) < 1e-3
+        and abs(cover.mean().values.item() - 2.444) < 1e-3
     )
 
 
 @pytest.mark.flaky(max_runs=3)
+def test_gtiff2file(geometry_nat):
+    url_wms = "https://www.mrlc.gov/geoserver/mrlc_download/wms"
+    wms = WMS(
+        url_wms,
+        layers="NLCD_Land_Cover_Change_Index_Science_product_L48",
+        outformat="image/geotiff",
+        crs=DEF_CRS,
+    )
+    r_dict = wms.getmap_bybox(
+        geometry_nat.bounds,
+        1e3,
+        box_crs=DEF_CRS,
+    )
+    geoutils.gtiff2file(r_dict, geometry_nat, DEF_CRS, "raster")
+    with rasterio.open("raster/NLCD_Land_Cover_Change_Index_Science_product_L48_dd_0_0.gtiff") as f:
+        mean = f.read().mean()
+
+    shutil.rmtree("raster")
+    assert abs(mean - 2.444) < 1e-3
+
+
+@pytest.mark.flaky(max_runs=3)
 def test_json2geodf(geometry_urb):
     url_wfs = "https://hazards.fema.gov/gis/nfhl/services/public/NFHL/MapServer/WFSServer"
 
     wfs = WFS(
         url_wfs,
         layer="public_NFHL:Base_Flood_Elevations",
         outformat="esrigeojson",
@@ -170,17 +194,17 @@
     bounds = geometry_urb.bounds
     crs = "epsg:2149"
     points = ((bounds[0], bounds[2]), (bounds[1], bounds[3]))
     geom = MatchCRS.geometry(geometry_urb, DEF_CRS, crs)
     bbox = MatchCRS.bounds(geometry_urb.bounds, DEF_CRS, crs)
     coords = MatchCRS.coords(points, DEF_CRS, crs)
     assert (
-        abs(geom.area - 2475726907.644) < 1e-3
-        and abs(bbox[0] - (-3654031.190)) < 1e-3
-        and abs(coords[0][-1] == (-2877067.244)) < 1e-3
+        abs(geom.area - 2475725967.465) < 1e-3
+        and abs(bbox[0] - (-3654030.292)) < 1e-3
+        and abs(coords[0][-1] == (-3588088.81)) < 1e-3
     )
 
 
 def test_show_versions():
     f = io.StringIO()
     geoutils.show_versions(file=f)
     assert "INSTALLED VERSIONS" in f.getvalue()
```

