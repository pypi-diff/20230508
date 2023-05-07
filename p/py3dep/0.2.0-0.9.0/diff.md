# Comparing `tmp/py3dep-0.2.0.tar.gz` & `tmp/py3dep-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py3dep-0.2.0.tar", last modified: Mon Dec  7 02:05:21 2020, max compression
+gzip compressed data, was "py3dep-0.9.0.tar", last modified: Wed Feb 17 18:20:08 2021, max compression
```

## Comparing `py3dep-0.2.0.tar` & `py3dep-0.9.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.661944 py3dep-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)      146 2020-12-07 02:05:15.000000 py3dep-0.2.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (116)       90 2020-12-07 02:05:15.000000 py3dep-0.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)      242 2020-12-07 02:05:15.000000 py3dep-0.2.0/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.657944 py3dep-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.657944 py3dep-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      919 2020-12-07 02:05:15.000000 py3dep-0.2.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (116)      684 2020-12-07 02:05:15.000000 py3dep-0.2.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-12-07 02:05:15.000000 py3dep-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (116)      125 2020-12-07 02:05:15.000000 py3dep-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.657944 py3dep-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2584 2020-12-07 02:05:15.000000 py3dep-0.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (116)      288 2020-12-07 02:05:15.000000 py3dep-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (116)      618 2020-12-07 02:05:15.000000 py3dep-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1163 2020-12-07 02:05:15.000000 py3dep-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1196 2020-12-07 02:05:15.000000 py3dep-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-12-07 02:05:15.000000 py3dep-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      163 2020-12-07 02:05:15.000000 py3dep-0.2.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1581 2020-12-07 02:05:15.000000 py3dep-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      157 2020-12-07 02:05:15.000000 py3dep-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3444 2020-12-07 02:05:15.000000 py3dep-0.2.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4091 2020-12-07 02:05:15.000000 py3dep-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1162 2020-12-07 02:05:15.000000 py3dep-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2020-12-07 02:05:15.000000 py3dep-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      150 2020-12-07 02:05:15.000000 py3dep-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2180 2020-12-07 02:05:15.000000 py3dep-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)    10579 2020-12-07 02:05:21.661944 py3dep-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8162 2020-12-07 02:05:15.000000 py3dep-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.657944 py3dep-0.2.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.657944 py3dep-0.2.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)      489 2020-12-07 02:05:15.000000 py3dep-0.2.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (116)      393 2020-12-07 02:05:15.000000 py3dep-0.2.0/ci/requirements/py3.6.yml
--rw-r--r--   0 runner    (1001) docker     (116)      393 2020-12-07 02:05:15.000000 py3dep-0.2.0/ci/requirements/py3.7.yml
--rw-r--r--   0 runner    (1001) docker     (116)      393 2020-12-07 02:05:15.000000 py3dep-0.2.0/ci/requirements/py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (116)      393 2020-12-07 02:05:15.000000 py3dep-0.2.0/ci/requirements/py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.657944 py3dep-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     8187 2020-12-07 02:05:15.000000 py3dep-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.661944 py3dep-0.2.0/docs/_template/
--rw-r--r--   0 runner    (1001) docker     (116)       85 2020-12-07 02:05:15.000000 py3dep-0.2.0/docs/_template/layout.html
--rw-r--r--   0 runner    (1001) docker     (116)    11853 2020-12-07 02:05:15.000000 py3dep-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-12-07 02:05:15.000000 py3dep-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      771 2020-12-07 02:05:15.000000 py3dep-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       69 2020-12-07 02:05:15.000000 py3dep-0.2.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (116)      586 2020-12-07 02:05:15.000000 py3dep-0.2.0/docs/py3dep.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.661944 py3dep-0.2.0/py3dep/
--rw-r--r--   0 runner    (1001) docker     (116)      420 2020-12-07 02:05:15.000000 py3dep-0.2.0/py3dep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      760 2020-12-07 02:05:15.000000 py3dep-0.2.0/py3dep/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     5079 2020-12-07 02:05:15.000000 py3dep-0.2.0/py3dep/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (116)    11653 2020-12-07 02:05:15.000000 py3dep-0.2.0/py3dep/py3dep.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.661944 py3dep-0.2.0/py3dep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    10579 2020-12-07 02:05:21.000000 py3dep-0.2.0/py3dep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1121 2020-12-07 02:05:21.000000 py3dep-0.2.0/py3dep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 02:05:21.000000 py3dep-0.2.0/py3dep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 02:05:21.000000 py3dep-0.2.0/py3dep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      159 2020-12-07 02:05:21.000000 py3dep-0.2.0/py3dep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-07 02:05:21.000000 py3dep-0.2.0/py3dep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      291 2020-12-07 02:05:15.000000 py3dep-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.661944 py3dep-0.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)     4671 2020-12-07 02:05:15.000000 py3dep-0.2.0/scripts/generate_pip_deps_from_conda.py
--rw-r--r--   0 runner    (1001) docker     (116)     1940 2020-12-07 02:05:21.661944 py3dep-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-12-07 02:05:15.000000 py3dep-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:05:21.661944 py3dep-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      286 2020-12-07 02:05:15.000000 py3dep-0.2.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2193 2020-12-07 02:05:15.000000 py3dep-0.2.0/tests/test_py3dep.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.758157 py3dep-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2021-02-17 18:20:04.000000 py3dep-0.9.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       90 2021-02-17 18:20:04.000000 py3dep-0.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (116)      242 2021-02-17 18:20:04.000000 py3dep-0.9.0/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.754157 py3dep-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.754157 py3dep-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (116)      919 2021-02-17 18:20:04.000000 py3dep-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (116)      684 2021-02-17 18:20:04.000000 py3dep-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (116)      321 2021-02-17 18:20:04.000000 py3dep-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2021-02-17 18:20:04.000000 py3dep-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.754157 py3dep-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2719 2021-02-17 18:20:04.000000 py3dep-0.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2021-02-17 18:20:04.000000 py3dep-0.9.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1306 2021-02-17 18:20:04.000000 py3dep-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1339 2021-02-17 18:20:04.000000 py3dep-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1226 2021-02-17 18:20:04.000000 py3dep-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      163 2021-02-17 18:20:04.000000 py3dep-0.9.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1867 2021-02-17 18:20:04.000000 py3dep-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      157 2021-02-17 18:20:04.000000 py3dep-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3444 2021-02-17 18:20:04.000000 py3dep-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4091 2021-02-17 18:20:04.000000 py3dep-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1578 2021-02-17 18:20:04.000000 py3dep-0.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1096 2021-02-17 18:20:04.000000 py3dep-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      150 2021-02-17 18:20:04.000000 py3dep-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2180 2021-02-17 18:20:04.000000 py3dep-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2021-02-17 18:20:08.758157 py3dep-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     8844 2021-02-17 18:20:04.000000 py3dep-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.754157 py3dep-0.9.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.758157 py3dep-0.9.0/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (116)      504 2021-02-17 18:20:04.000000 py3dep-0.9.0/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      407 2021-02-17 18:20:04.000000 py3dep-0.9.0/ci/requirements/py3.6.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      407 2021-02-17 18:20:04.000000 py3dep-0.9.0/ci/requirements/py3.7.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      407 2021-02-17 18:20:04.000000 py3dep-0.9.0/ci/requirements/py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      407 2021-02-17 18:20:04.000000 py3dep-0.9.0/ci/requirements/py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.758157 py3dep-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     8187 2021-02-17 18:20:04.000000 py3dep-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.758157 py3dep-0.9.0/docs/_template/
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2021-02-17 18:20:04.000000 py3dep-0.9.0/docs/_template/layout.html
+-rw-r--r--   0 runner    (1001) docker     (116)    11853 2021-02-17 18:20:04.000000 py3dep-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2021-02-17 18:20:04.000000 py3dep-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      771 2021-02-17 18:20:04.000000 py3dep-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (116)       69 2021-02-17 18:20:04.000000 py3dep-0.9.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      586 2021-02-17 18:20:04.000000 py3dep-0.9.0/docs/py3dep.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.758157 py3dep-0.9.0/py3dep/
+-rw-r--r--   0 runner    (1001) docker     (116)      403 2021-02-17 18:20:04.000000 py3dep-0.9.0/py3dep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      760 2021-02-17 18:20:04.000000 py3dep-0.9.0/py3dep/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5079 2021-02-17 18:20:04.000000 py3dep-0.9.0/py3dep/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10354 2021-02-17 18:20:04.000000 py3dep-0.9.0/py3dep/py3dep.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.758157 py3dep-0.9.0/py3dep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2021-02-17 18:20:08.000000 py3dep-0.9.0/py3dep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1084 2021-02-17 18:20:08.000000 py3dep-0.9.0/py3dep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:20:08.000000 py3dep-0.9.0/py3dep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:20:08.000000 py3dep-0.9.0/py3dep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      170 2021-02-17 18:20:08.000000 py3dep-0.9.0/py3dep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2021-02-17 18:20:08.000000 py3dep-0.9.0/py3dep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      302 2021-02-17 18:20:04.000000 py3dep-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.758157 py3dep-0.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4753 2021-02-17 18:20:04.000000 py3dep-0.9.0/scripts/generate_pip_deps_from_conda.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1940 2021-02-17 18:20:08.758157 py3dep-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      587 2021-02-17 18:20:04.000000 py3dep-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:20:08.758157 py3dep-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      286 2021-02-17 18:20:04.000000 py3dep-0.9.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2107 2021-02-17 18:20:04.000000 py3dep-0.9.0/tests/test_py3dep.py
```

### Comparing `py3dep-0.2.0/.github/ISSUE_TEMPLATE/bug-report.md` & `py3dep-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/.github/ISSUE_TEMPLATE/feature-request.md` & `py3dep-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/.github/workflows/codeql-analysis.yml` & `py3dep-0.9.0/.github/workflows/codeql-analysis.yml`

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

### Comparing `py3dep-0.2.0/.github/workflows/release.yml` & `py3dep-0.9.0/.github/workflows/release.yml`

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

### Comparing `py3dep-0.2.0/.github/workflows/test.yml` & `py3dep-0.9.0/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

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
           activate-environment: py3dep
           python-version: ${{ matrix.python-version }}
           environment-file: ci/requirements/py${{ matrix.python-version }}.yml
```

### Comparing `py3dep-0.2.0/.gitignore` & `py3dep-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/.pre-commit-config.yaml` & `py3dep-0.9.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

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
-      name: Autoformat docs with doc8
+      name: Autoformat with doc8
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
-        files: py3dep
+        exclude: tests
+        files: pynhd
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.7.4
+    rev: v2.10.0
     hooks:
       - id: pyupgrade
-        name: Upgrade syntax to python 3.6+ with pyupgrade
+        name: Upgrade synax to python 3.6+ with pyupgrade
         args: [--py36-plus]
 
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.6.3
+    rev: 1.7.0
     hooks:
       - id: bandit
         name: Check for security issues with bandit
-        args: [-lll, --recursive, py3dep]
+        args: [-lll, --recursive, pynhd]
         files: .py$
```

### Comparing `py3dep-0.2.0/CODE_OF_CONDUCT.rst` & `py3dep-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/CONTRIBUTING.rst` & `py3dep-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/HISTORY.rst` & `py3dep-0.9.0/HISTORY.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =======
 History
 =======
 
+0.9.0 (2021-02-14)
+------------------
+
+- Bump version to the same version as Hydrodata.
+- Add support for saving maps as ``geotiff`` file(s).
+- Replace ``Elevation Point Query Service`` service with ``AirMap`` for getting
+  elevations for a list of coordinates in bulk since ``AirMap`` is much faster.
+  The resolution of ``AirMap`` is 30 m.
+- Use ``cytoolz`` for some of the operations for improving performance.
+
 0.2.0 (2020-12-06)
 ------------------
 
 - Add support for multipolygon.
 - Remove the ``fill_hole`` argument.
 - Add a new function to get elevations for a list of coordinates called ``elevation_bycoords``.
 - Refactor ``elevation_bygrid`` function for increasing readability and performance.
@@ -16,15 +26,15 @@
 - Added a rename operation to ``get_map`` to automatically rename the variables to a
   more sensible one.
 - Replaced ``simplejson`` with ``orjson`` to speed-up JSON operations.
 
 0.1.6 (2020-08-11)
 ------------------
 
-- Add a new function, ``show_versions``, for getting versions of the installed dependecies
+- Add a new function, ``show_versions``, for getting versions of the installed dependencies
   which is useful for debugging and reporting.
 - Fix typos in the docs and improved the README.
 - Improve testing and coverage.
 
 0.1.5 (2020-08-03)
 ------------------
```

### Comparing `py3dep-0.2.0/LICENSE` & `py3dep-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/Makefile` & `py3dep-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/PKG-INFO` & `py3dep-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: py3dep
-Version: 0.2.0
+Version: 0.9.0
 Summary: Access USGS 3DEP database and get data such as elevation in the US
 Home-page: https://github.com/cheginit/py3dep
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT license
 Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/py3dep_logo.png
             :target: https://github.com/cheginit/py3dep
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
@@ -85,16 +85,14 @@
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
             :target: https://github.com/pre-commit/pre-commit
             :alt: pre-commit
         
         |
         
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
         Features
         --------
         
         Py3DEP is a part of Hydrodata software stack and provides access to the
         `3DEP <https://www.usgs.gov/core-science-systems/ngp/3dep>`__
         database which is a part of the
         `National Map services <https://viewer.nationalmap.gov/services/>`__.
@@ -123,14 +121,18 @@
           Map's `Elevation Point Query Service <https://nationalmap.gov/epqs/>`__.
         - ``deg2mpm``: For converting slope dataset from degree to meter per meter.
         
         You can try using Py3DEP without installing it on you system by clicking on the binder badge
         below the Py3DEP banner. A Jupyter notebook instance with the Hydrodata software stack
         pre-installed will be launched in your web browser and you can start coding!
         
+        Please note that since Hydrodata is in early development stages, while the provided
+        functionaities should be stable, changes in APIs are possible in new releases. But we
+        appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+        
         Moreover, requests for additional functionalities can be submitted via
         `issue tracker <https://github.com/cheginit/py3dep/issues>`__.
         
         
         Installation
         ------------
         
@@ -164,15 +166,15 @@
         these spatial references.
         
         .. code-block:: python
         
             import py3dep
             from pynhd import NLDI
         
-            geom = NLDI().getfeature_byid("nwissite", "USGS-01031500", basin=True).geometry[0]
+            geom = NLDI().get_basins("01031500").geometry[0]
             dem = py3dep.get_map("DEM", geom, resolution=30, geo_crs="epsg:4326", crs="epsg:3857")
             slope = py3dep.get_map("Slope Degrees", geom, resolution=30)
             slope = py3dep.deg2mpm(slope)
         
         .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_py3dep.png
             :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_py3dep.png
             :align: center
@@ -190,19 +192,29 @@
         .. code-block:: python
         
             import pydaymet as daymet
             import xarray as xr
             import numpy as np
         
             clm = daymet.get_bygeom(geom, ("2005-01-01", "2005-01-31"), variables="tmin")
-            gridxy = (clm.x.values, clm.y.values)
-            elev = py3dep.elevation_bygrid(gridxy, clm.crs, clm.res[0] * 1000)
+            elev = py3dep.elevation_bygrid(clm.x.values, clm.y.values, clm.crs, clm.res[0] * 1000)
             clm = xr.merge([clm, elev], combine_attrs="override")
             clm["elevation"] = clm.elevation.where(~np.isnan(clm.isel(time=0).tmin), drop=True)
         
+        Now, let's get street network data using [osmnx](https://github.com/gboeing/osmnx) package
+        and add elevation data for its nodes using ``elevation_bycoords`` function.
+        
+        .. code-block:: python
+        
+            import osmnx as ox
+        
+            G = ox.graph_from_place("Piedmont, California, USA", network_type="drive")
+            x, y = nx.get_node_attributes(G, "x").values(), nx.get_node_attributes(G, "y").values()
+            elevation = py3dep.elevation_bycoords(list(zip(x, y)), crs="epsg:4326", resolution=90)
+            nx.set_node_attributes(G, dict(zip(G.nodes(), elevation)), "elevation")
         
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

### Comparing `py3dep-0.2.0/README.rst` & `py3dep-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/py3dep_logo.png
     :target: https://github.com/cheginit/py3dep
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
@@ -77,16 +77,14 @@
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
     :target: https://github.com/pre-commit/pre-commit
     :alt: pre-commit
 
 |
 
-🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-
 Features
 --------
 
 Py3DEP is a part of Hydrodata software stack and provides access to the
 `3DEP <https://www.usgs.gov/core-science-systems/ngp/3dep>`__
 database which is a part of the
 `National Map services <https://viewer.nationalmap.gov/services/>`__.
@@ -115,14 +113,18 @@
   Map's `Elevation Point Query Service <https://nationalmap.gov/epqs/>`__.
 - ``deg2mpm``: For converting slope dataset from degree to meter per meter.
 
 You can try using Py3DEP without installing it on you system by clicking on the binder badge
 below the Py3DEP banner. A Jupyter notebook instance with the Hydrodata software stack
 pre-installed will be launched in your web browser and you can start coding!
 
+Please note that since Hydrodata is in early development stages, while the provided
+functionaities should be stable, changes in APIs are possible in new releases. But we
+appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+
 Moreover, requests for additional functionalities can be submitted via
 `issue tracker <https://github.com/cheginit/py3dep/issues>`__.
 
 
 Installation
 ------------
 
@@ -156,15 +158,15 @@
 these spatial references.
 
 .. code-block:: python
 
     import py3dep
     from pynhd import NLDI
 
-    geom = NLDI().getfeature_byid("nwissite", "USGS-01031500", basin=True).geometry[0]
+    geom = NLDI().get_basins("01031500").geometry[0]
     dem = py3dep.get_map("DEM", geom, resolution=30, geo_crs="epsg:4326", crs="epsg:3857")
     slope = py3dep.get_map("Slope Degrees", geom, resolution=30)
     slope = py3dep.deg2mpm(slope)
 
 .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_py3dep.png
     :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_py3dep.png
     :align: center
@@ -182,19 +184,29 @@
 .. code-block:: python
 
     import pydaymet as daymet
     import xarray as xr
     import numpy as np
 
     clm = daymet.get_bygeom(geom, ("2005-01-01", "2005-01-31"), variables="tmin")
-    gridxy = (clm.x.values, clm.y.values)
-    elev = py3dep.elevation_bygrid(gridxy, clm.crs, clm.res[0] * 1000)
+    elev = py3dep.elevation_bygrid(clm.x.values, clm.y.values, clm.crs, clm.res[0] * 1000)
     clm = xr.merge([clm, elev], combine_attrs="override")
     clm["elevation"] = clm.elevation.where(~np.isnan(clm.isel(time=0).tmin), drop=True)
 
+Now, let's get street network data using [osmnx](https://github.com/gboeing/osmnx) package
+and add elevation data for its nodes using ``elevation_bycoords`` function.
+
+.. code-block:: python
+
+    import osmnx as ox
+
+    G = ox.graph_from_place("Piedmont, California, USA", network_type="drive")
+    x, y = nx.get_node_attributes(G, "x").values(), nx.get_node_attributes(G, "y").values()
+    elevation = py3dep.elevation_bycoords(list(zip(x, y)), crs="epsg:4326", resolution=90)
+    nx.set_node_attributes(G, dict(zip(G.nodes(), elevation)), "elevation")
 
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

### Comparing `py3dep-0.2.0/docs/Makefile` & `py3dep-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/docs/conf.py` & `py3dep-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/docs/make.bat` & `py3dep-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/docs/py3dep.rst` & `py3dep-0.9.0/docs/py3dep.rst`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/py3dep/exceptions.py` & `py3dep-0.9.0/py3dep/exceptions.py`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/py3dep/print_versions.py` & `py3dep-0.9.0/py3dep/print_versions.py`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/py3dep/py3dep.py` & `py3dep-0.9.0/py3dep/py3dep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Get data from 3DEP database."""
 from itertools import product
+from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
+import cytoolz as tlz
 import numpy as np
 import pygeoutils as geoutils
 import rasterio as rio
 import rasterio.warp as rio_warp
 import xarray as xr
 from pygeoogc import WMS, MatchCRS, RetrySession, ServiceURL
 from shapely.geometry import MultiPolygon, Polygon
@@ -17,14 +19,15 @@
 
 def get_map(
     layers: Union[str, List[str]],
     geometry: Union[Polygon, Tuple[float, float, float, float]],
     resolution: float,
     geo_crs: str = DEF_CRS,
     crs: str = DEF_CRS,
+    output_dir: Optional[Union[str, Path]] = None,
 ) -> Dict[str, bytes]:
     """Access to `3DEP <https://www.usgs.gov/core-science-systems/ngp/3dep>`__ service.
 
     The 3DEP service has multi-resolution sources so depending on the user
     provided resolution the data is resampled on server-side based
     on all the available data sources. The following layers are available:
     - "DEM"
@@ -51,14 +54,16 @@
         based on the geometry bounds and the given resolution.
     geo_crs : str, optional
         The spatial reference system of the input geometry, defaults to
         epsg:4326.
     crs : str, optional
         The spatial reference system to be used for requesting the data, defaults to
         epsg:4326.
+    output_dir : str or Path, optional
+        The output directory to also save the map as GTiff file(s), defaults to None.
 
     Returns
     -------
     dict
         A dict where the keys are the layer name and values are the returned response
         from the WMS service as bytes. You can use ``utils.create_dataset`` function
         to convert the responses to ``xarray.Dataset``.
@@ -73,14 +78,17 @@
         _layers[_layers.index("DEM")] = "None"
 
     _layers = [f"3DEPElevation:{lyr}" for lyr in _layers]
 
     wms = WMS(ServiceURL().wms.nm_3dep, layers=_layers, outformat="image/tiff", crs=crs)
     r_dict = wms.getmap_bybox(_geometry.bounds, resolution, box_crs=crs)
 
+    if output_dir:
+        geoutils.gtiff2file(r_dict, _geometry, crs, output_dir)
+
     ds = geoutils.gtiff2xarray(r_dict, _geometry, crs)
 
     valid_layers = wms.get_validlayers()
     rename = {lyr: lyr.split(":")[-1].replace(" ", "_").lower() for lyr in valid_layers}
     rename.update({"3DEPElevation:None": "elevation"})
 
     if isinstance(ds, xr.DataArray):
@@ -128,65 +136,26 @@
         An data array with name elevation and the given dim names.
     """
     if dim_names is None:
         dim_names = ("x", "y")
 
     bbox = (min(xcoords), min(ycoords), max(xcoords), max(ycoords))
     r_dict = _elevation_bybox(bbox, crs, resolution)
-    coords = [(x, y) for x, y in product(xcoords, ycoords)]
+    coords = product(xcoords, ycoords)
     elev_arr = _sample_tiff(r_dict["3DEPElevation:None_dd_0_0"], coords, crs, resampling)
 
     return xr.DataArray(
         elev_arr.reshape((len(xcoords), len(ycoords))),
         dims=dim_names,
         coords=[xcoords, ycoords],
         name="elevation",
         attrs={"units": "meters"},
     )
 
 
-def elevation_bycoords(
-    coords: List[Tuple[float, float]],
-    crs: str,
-    resolution: float,
-    resampling: rio_warp.Resampling = rio_warp.Resampling.bilinear,
-) -> np.ndarray:
-    """Get elevation from DEM data for a list of coordinates.
-
-    This function is intended for getting elevations for a gridded dataset.
-
-    Parameters
-    ----------
-    coords : list of tuples
-        A list containing x- and y-coordinates of a mesh, [(x, y), ...].
-    crs : str
-        The spatial reference system of the input grid, defaults to epsg:4326.
-    resolution : float
-        The accuracy of the output, defaults to 10 m which is the highest
-        available resolution that covers CONUS. Note that higher resolution
-        increases computation time so chose this value with caution.
-    resampling : rasterio.warp.Resampling
-        The reasmpling method to use if the input crs is not in the supported
-        3DEP's CRS list which are epsg:4326 and epsg:3857. It defaults to bilinear.
-        The available methods can be found `here <https://rasterio.readthedocs.io/en/latest/api/rasterio.enums.html#rasterio.enums.Resampling>`__
-
-    Returns
-    -------
-    numpy.ndarray
-        An array of elevations where its index matches the input gridxy list
-    """
-    if not isinstance(coords, list) or len(coords[0]) != 2:
-        raise InvalidInputType("coords", "list of tuples of length two")
-
-    gx, gy = zip(*coords)
-    bbox = (min(gx), min(gy), max(gx), max(gy))
-    r_dict = _elevation_bybox(bbox, crs, resolution)
-    return _sample_tiff(r_dict["3DEPElevation:None_dd_0_0"], coords, crs, resampling)
-
-
 def _sample_tiff(
     content: bytes, coords: List[Tuple[float, float]], crs: str, resampling: rio_warp.Resampling
 ) -> np.ndarray:
     """Sample a tiff response for a list of coordinates.
 
     Parameters
     ----------
@@ -268,46 +237,43 @@
     req_crs = crs if crs.lower() in [DEF_CRS, "epsg:3857"] else DEF_CRS
     wms = WMS(
         ServiceURL().wms.nm_3dep, layers="3DEPElevation:None", outformat="image/tiff", crs=req_crs
     )
     return wms.getmap_bybox(bbox, resolution, box_crs=crs)
 
 
-def elevation_byloc(coord: Tuple[float, float], crs: str = DEF_CRS):
-    """Get elevation from USGS 3DEP service for a coordinate.
+def elevation_bycoords(coords: List[Tuple[float, float]], crs: str = DEF_CRS) -> List[int]:
+    """Get elevation from Airmap for a list of coordinates.
 
     Parameters
     ----------
-    coord : tuple
+    coords : list of tuples
         Coordinates of the location as a tuple
     crs : str, optional
         The spatial reference of the input coord, defaults to epsg:4326 (lon, lat)
 
     Returns
     -------
-    float
+    list of int
         Elevation in meter
     """
-    if not isinstance(coord, tuple) or len(coord) != 2:
-        raise InvalidInputType("coord", "tuple of length 2", "(x, y)")
+    if not isinstance(coords, list) and all(len(c) == 2 for c in coords):
+        raise InvalidInputType("coord", "list of tuples of length 2", "[(x, y), ...]")
 
-    lon, lat = MatchCRS.coords(([coord[0]], [coord[1]]), crs, DEF_CRS)
+    coords_reproj = zip(*MatchCRS.coords(tuple(zip(*coords)), crs, DEF_CRS))
+    coords_reproj = tlz.partition_all(100, coords_reproj)
 
-    url = "https://nationalmap.gov/epqs/pqs.php"
-    payload = {"output": "json", "x": lon[0], "y": lat[0], "units": "Meters"}
-    r = RetrySession().get(url, payload)
-    root = r.json()["USGS_Elevation_Point_Query_Service"]
-    elevation = float(root["Elevation_Query"]["Elevation"])
-
-    if abs(elevation - (-1000000)) < 1e-3:
-        raise ValueError(
-            f"The elevation of the requested coordinate ({coord[0]}, {coord[1]}) cannot be found."
-        )
+    headers = {"Content-Type": "application/json", "charset": "utf-8"}
+    elevations = []
+    for chunk in coords_reproj:
+        payload = {"points": ",".join(f"{lat},{lon}" for lon, lat in chunk)}
+        resp = RetrySession().get(ServiceURL().restful.airmap, payload=payload, headers=headers)
+        elevations.append(resp.json()["data"])
 
-    return elevation
+    return list(tlz.concat(elevations))
 
 
 def deg2mpm(da: xr.DataArray) -> xr.DataArray:
     """Convert ``xarray.Data[Array,set]`` from degree to meter/meter."""
     attrs = da.attrs
     da = np.tan(np.deg2rad(da))
     da.attrs = attrs
```

### Comparing `py3dep-0.2.0/py3dep.egg-info/PKG-INFO` & `py3dep-0.9.0/py3dep.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: py3dep
-Version: 0.2.0
+Version: 0.9.0
 Summary: Access USGS 3DEP database and get data such as elevation in the US
 Home-page: https://github.com/cheginit/py3dep
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT license
 Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/py3dep_logo.png
             :target: https://github.com/cheginit/py3dep
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
@@ -85,16 +85,14 @@
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
             :target: https://github.com/pre-commit/pre-commit
             :alt: pre-commit
         
         |
         
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
         Features
         --------
         
         Py3DEP is a part of Hydrodata software stack and provides access to the
         `3DEP <https://www.usgs.gov/core-science-systems/ngp/3dep>`__
         database which is a part of the
         `National Map services <https://viewer.nationalmap.gov/services/>`__.
@@ -123,14 +121,18 @@
           Map's `Elevation Point Query Service <https://nationalmap.gov/epqs/>`__.
         - ``deg2mpm``: For converting slope dataset from degree to meter per meter.
         
         You can try using Py3DEP without installing it on you system by clicking on the binder badge
         below the Py3DEP banner. A Jupyter notebook instance with the Hydrodata software stack
         pre-installed will be launched in your web browser and you can start coding!
         
+        Please note that since Hydrodata is in early development stages, while the provided
+        functionaities should be stable, changes in APIs are possible in new releases. But we
+        appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+        
         Moreover, requests for additional functionalities can be submitted via
         `issue tracker <https://github.com/cheginit/py3dep/issues>`__.
         
         
         Installation
         ------------
         
@@ -164,15 +166,15 @@
         these spatial references.
         
         .. code-block:: python
         
             import py3dep
             from pynhd import NLDI
         
-            geom = NLDI().getfeature_byid("nwissite", "USGS-01031500", basin=True).geometry[0]
+            geom = NLDI().get_basins("01031500").geometry[0]
             dem = py3dep.get_map("DEM", geom, resolution=30, geo_crs="epsg:4326", crs="epsg:3857")
             slope = py3dep.get_map("Slope Degrees", geom, resolution=30)
             slope = py3dep.deg2mpm(slope)
         
         .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_py3dep.png
             :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_py3dep.png
             :align: center
@@ -190,19 +192,29 @@
         .. code-block:: python
         
             import pydaymet as daymet
             import xarray as xr
             import numpy as np
         
             clm = daymet.get_bygeom(geom, ("2005-01-01", "2005-01-31"), variables="tmin")
-            gridxy = (clm.x.values, clm.y.values)
-            elev = py3dep.elevation_bygrid(gridxy, clm.crs, clm.res[0] * 1000)
+            elev = py3dep.elevation_bygrid(clm.x.values, clm.y.values, clm.crs, clm.res[0] * 1000)
             clm = xr.merge([clm, elev], combine_attrs="override")
             clm["elevation"] = clm.elevation.where(~np.isnan(clm.isel(time=0).tmin), drop=True)
         
+        Now, let's get street network data using [osmnx](https://github.com/gboeing/osmnx) package
+        and add elevation data for its nodes using ``elevation_bycoords`` function.
+        
+        .. code-block:: python
+        
+            import osmnx as ox
+        
+            G = ox.graph_from_place("Piedmont, California, USA", network_type="drive")
+            x, y = nx.get_node_attributes(G, "x").values(), nx.get_node_attributes(G, "y").values()
+            elevation = py3dep.elevation_bycoords(list(zip(x, y)), crs="epsg:4326", resolution=90)
+            nx.set_node_attributes(G, dict(zip(G.nodes(), elevation)), "elevation")
         
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

### Comparing `py3dep-0.2.0/py3dep.egg-info/SOURCES.txt` & `py3dep-0.9.0/py3dep.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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
```

### Comparing `py3dep-0.2.0/scripts/generate_pip_deps_from_conda.py` & `py3dep-0.9.0/scripts/generate_pip_deps_from_conda.py`

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

### Comparing `py3dep-0.2.0/setup.cfg` & `py3dep-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/setup.py` & `py3dep-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `py3dep-0.2.0/tests/test_py3dep.py` & `py3dep-0.9.0/tests/test_py3dep.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import io
+import shutil
 
 import numpy as np
 import pytest
+import rasterio
 from pygeoogc import MatchCRS
 from shapely.geometry import Polygon
 
 import py3dep
 
 DEF_CRS = "epsg:4326"
 ALT_CRS = "epsg:3857"
@@ -26,47 +28,45 @@
     dem_1e3 = py3dep.get_map(lyr[0], geometry, 1e3, geo_crs=DEF_CRS, crs=ALT_CRS)
     assert (
         sorted(ds.keys()) == ["elevation", "slope_degrees"]
         and abs(dem_10.mean().item() - dem_1e3.mean().item()) < 7e-2
     )
 
 
-def test_loc():
-    elev = py3dep.elevation_byloc((-7766049.664788851, 5691929.739021257), ALT_CRS)
-    assert abs(elev - 356.59) < 1e-3
+@pytest.mark.flaky(max_runs=3)
+def test_getmap_2file(geometry):
+    dem = py3dep.get_map("DEM", geometry, 1e3, geo_crs=DEF_CRS, crs=ALT_CRS, output_dir="raster")
+    with rasterio.open("raster/3DEPElevation:None_dd_0_0.gtiff") as f:
+        mean = f.read().mean()
+
+    shutil.rmtree("raster")
+    assert abs(dem.mean().item() - mean) < 7e-2
+
+
+def test_coords():
+    elev = py3dep.elevation_bycoords([(-7766049.664788851, 5691929.739021257)] * 3, ALT_CRS)
+    assert elev == [363] * 3
 
 
 @pytest.mark.flaky(max_runs=3)
 def test_deg2mpm(geometry):
     slope = py3dep.get_map("Slope Degrees", geometry, 1e3)
     slope = py3dep.deg2mpm(slope)
     assert abs(slope.mean().item() - 0.05) < 1e-3
 
 
 def test_grid(geometry):
     geo_crs = DEF_CRS
-    crs = "+proj=lcc +lat_1=25 +lat_2=60 +lat_0=42.5 +lon_0=-100 +x_0=0 +y_0=0 +ellps=WGS84 +units=km +no_defs"
+    crs = "+proj=lcc +lat_1=25 +lat_2=60 +lat_0=42.5 +lon_0=-100 +x_0=0 +y_0=0 +ellps=WGS84 +units=m +no_defs"
     geom = MatchCRS.geometry(geometry, geo_crs, crs)
     xmin, ymin, xmax, ymax = geom.bounds
-    res = 1
+    res = 1e3
     gx = np.arange(xmin, xmax, res)
     gy = np.arange(ymin, ymax, res)
-    elev = py3dep.elevation_bygrid(gx, gy, crs, res * 1e3)
+    elev = py3dep.elevation_bygrid(gx, gy, crs, res)
     assert abs(elev.mean().item() - 295.763) < 1e-3
 
 
-def test_coords(geometry):
-    geo_crs = DEF_CRS
-    crs = "+proj=lcc +lat_1=25 +lat_2=60 +lat_0=42.5 +lon_0=-100 +x_0=0 +y_0=0 +ellps=WGS84 +units=km +no_defs"
-    geom = MatchCRS.geometry(geometry, geo_crs, crs)
-    xmin, ymin, xmax, ymax = geom.bounds
-    res = 1
-    gx = np.arange(xmin, xmax, res)
-    gy = np.arange(ymin, ymax, res)
-    elev = py3dep.elevation_bycoords(list(zip(gx, gy)), crs, res * 1e3)
-    assert abs(elev.mean() - 282.006) < 1e-3
-
-
 def test_show_versions():
     f = io.StringIO()
     py3dep.show_versions(file=f)
     assert "INSTALLED VERSIONS" in f.getvalue()
```

