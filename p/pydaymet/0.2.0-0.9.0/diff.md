# Comparing `tmp/pydaymet-0.2.0.tar.gz` & `tmp/pydaymet-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydaymet-0.2.0.tar", last modified: Mon Dec  7 02:27:12 2020, max compression
+gzip compressed data, was "pydaymet-0.9.0.tar", last modified: Wed Feb 17 18:23:54 2021, max compression
```

## Comparing `pydaymet-0.2.0.tar` & `pydaymet-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.680719 pydaymet-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)      146 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (116)       97 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)      242 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.676719 pydaymet-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.676719 pydaymet-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      923 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (116)      684 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (116)      125 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.676719 pydaymet-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2584 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (116)      288 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1163 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1206 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      163 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1579 2020-12-07 02:27:00.000000 pydaymet-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      157 2020-12-07 02:27:00.000000 pydaymet-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3444 2020-12-07 02:27:00.000000 pydaymet-0.2.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4113 2020-12-07 02:27:00.000000 pydaymet-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1005 2020-12-07 02:27:00.000000 pydaymet-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2020-12-07 02:27:00.000000 pydaymet-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      150 2020-12-07 02:27:00.000000 pydaymet-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2186 2020-12-07 02:27:00.000000 pydaymet-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     9049 2020-12-07 02:27:12.680719 pydaymet-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6910 2020-12-07 02:27:00.000000 pydaymet-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.668718 pydaymet-0.2.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.676719 pydaymet-0.2.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)      568 2020-12-07 02:27:00.000000 pydaymet-0.2.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (116)      471 2020-12-07 02:27:00.000000 pydaymet-0.2.0/ci/requirements/py3.6.yml
--rw-r--r--   0 runner    (1001) docker     (116)      471 2020-12-07 02:27:00.000000 pydaymet-0.2.0/ci/requirements/py3.7.yml
--rw-r--r--   0 runner    (1001) docker     (116)      471 2020-12-07 02:27:00.000000 pydaymet-0.2.0/ci/requirements/py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (116)      471 2020-12-07 02:27:00.000000 pydaymet-0.2.0/ci/requirements/py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.676719 pydaymet-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     8187 2020-12-07 02:27:00.000000 pydaymet-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.676719 pydaymet-0.2.0/docs/_template/
--rw-r--r--   0 runner    (1001) docker     (116)       85 2020-12-07 02:27:00.000000 pydaymet-0.2.0/docs/_template/layout.html
--rw-r--r--   0 runner    (1001) docker     (116)    11895 2020-12-07 02:27:00.000000 pydaymet-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-12-07 02:27:00.000000 pydaymet-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      771 2020-12-07 02:27:00.000000 pydaymet-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       71 2020-12-07 02:27:00.000000 pydaymet-0.2.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (116)      616 2020-12-07 02:27:00.000000 pydaymet-0.2.0/docs/pydaymet.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.676719 pydaymet-0.2.0/pydaymet/
--rw-r--r--   0 runner    (1001) docker     (116)      408 2020-12-07 02:27:00.000000 pydaymet-0.2.0/pydaymet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1989 2020-12-07 02:27:00.000000 pydaymet-0.2.0/pydaymet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     5079 2020-12-07 02:27:00.000000 pydaymet-0.2.0/pydaymet/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (116)    18896 2020-12-07 02:27:00.000000 pydaymet-0.2.0/pydaymet/pydaymet.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.680719 pydaymet-0.2.0/pydaymet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9049 2020-12-07 02:27:12.000000 pydaymet-0.2.0/pydaymet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2020-12-07 02:27:12.000000 pydaymet-0.2.0/pydaymet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 02:27:12.000000 pydaymet-0.2.0/pydaymet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 02:27:12.000000 pydaymet-0.2.0/pydaymet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      182 2020-12-07 02:27:12.000000 pydaymet-0.2.0/pydaymet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-07 02:27:12.000000 pydaymet-0.2.0/pydaymet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      314 2020-12-07 02:27:00.000000 pydaymet-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.680719 pydaymet-0.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)     4671 2020-12-07 02:27:00.000000 pydaymet-0.2.0/scripts/generate_pip_deps_from_conda.py
--rw-r--r--   0 runner    (1001) docker     (116)     1964 2020-12-07 02:27:12.680719 pydaymet-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-12-07 02:27:00.000000 pydaymet-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 02:27:12.680719 pydaymet-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      785 2020-12-07 02:27:00.000000 pydaymet-0.2.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1426 2020-12-07 02:27:00.000000 pydaymet-0.2.0/tests/test_pydaymet.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.255544 pydaymet-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       97 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (116)      242 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.243543 pydaymet-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.247543 pydaymet-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (116)      684 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (116)      321 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.247543 pydaymet-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2719 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1306 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1349 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1226 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      163 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1873 2021-02-17 18:23:48.000000 pydaymet-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      157 2021-02-17 18:23:48.000000 pydaymet-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3444 2021-02-17 18:23:48.000000 pydaymet-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4113 2021-02-17 18:23:48.000000 pydaymet-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2404 2021-02-17 18:23:48.000000 pydaymet-0.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1096 2021-02-17 18:23:48.000000 pydaymet-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      150 2021-02-17 18:23:48.000000 pydaymet-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2186 2021-02-17 18:23:48.000000 pydaymet-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)    12155 2021-02-17 18:23:54.255544 pydaymet-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     9632 2021-02-17 18:23:48.000000 pydaymet-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.239544 pydaymet-0.9.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.251543 pydaymet-0.9.0/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (116)      583 2021-02-17 18:23:48.000000 pydaymet-0.9.0/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      486 2021-02-17 18:23:48.000000 pydaymet-0.9.0/ci/requirements/py3.6.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      486 2021-02-17 18:23:48.000000 pydaymet-0.9.0/ci/requirements/py3.7.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      486 2021-02-17 18:23:48.000000 pydaymet-0.9.0/ci/requirements/py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      486 2021-02-17 18:23:48.000000 pydaymet-0.9.0/ci/requirements/py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.251543 pydaymet-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     8187 2021-02-17 18:23:48.000000 pydaymet-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.251543 pydaymet-0.9.0/docs/_template/
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2021-02-17 18:23:48.000000 pydaymet-0.9.0/docs/_template/layout.html
+-rw-r--r--   0 runner    (1001) docker     (116)    11892 2021-02-17 18:23:48.000000 pydaymet-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2021-02-17 18:23:48.000000 pydaymet-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      771 2021-02-17 18:23:48.000000 pydaymet-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (116)       71 2021-02-17 18:23:48.000000 pydaymet-0.9.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      616 2021-02-17 18:23:48.000000 pydaymet-0.9.0/docs/pydaymet.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.255544 pydaymet-0.9.0/pydaymet/
+-rw-r--r--   0 runner    (1001) docker     (116)      425 2021-02-17 18:23:48.000000 pydaymet-0.9.0/pydaymet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1994 2021-02-17 18:23:48.000000 pydaymet-0.9.0/pydaymet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5251 2021-02-17 18:23:48.000000 pydaymet-0.9.0/pydaymet/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27399 2021-02-17 18:23:48.000000 pydaymet-0.9.0/pydaymet/pydaymet.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.255544 pydaymet-0.9.0/pydaymet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    12155 2021-02-17 18:23:53.000000 pydaymet-0.9.0/pydaymet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1110 2021-02-17 18:23:54.000000 pydaymet-0.9.0/pydaymet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:23:53.000000 pydaymet-0.9.0/pydaymet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 18:23:53.000000 pydaymet-0.9.0/pydaymet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      193 2021-02-17 18:23:53.000000 pydaymet-0.9.0/pydaymet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2021-02-17 18:23:53.000000 pydaymet-0.9.0/pydaymet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      325 2021-02-17 18:23:48.000000 pydaymet-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.255544 pydaymet-0.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4753 2021-02-17 18:23:48.000000 pydaymet-0.9.0/scripts/generate_pip_deps_from_conda.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2130 2021-02-17 18:23:54.255544 pydaymet-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      587 2021-02-17 18:23:48.000000 pydaymet-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 18:23:54.255544 pydaymet-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      785 2021-02-17 18:23:48.000000 pydaymet-0.9.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2466 2021-02-17 18:23:48.000000 pydaymet-0.9.0/tests/test_pydaymet.py
```

### Comparing `pydaymet-0.2.0/.github/ISSUE_TEMPLATE/bug-report.md` & `pydaymet-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/.github/ISSUE_TEMPLATE/feature-request.md` & `pydaymet-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/.github/workflows/codeql-analysis.yml` & `pydaymet-0.9.0/.github/workflows/codeql-analysis.yml`

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

### Comparing `pydaymet-0.2.0/.github/workflows/release.yml` & `pydaymet-0.9.0/.github/workflows/release.yml`

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

### Comparing `pydaymet-0.2.0/.github/workflows/test.yml` & `pydaymet-0.9.0/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

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
           activate-environment: pydaymet
           python-version: ${{ matrix.python-version }}
           environment-file: ci/requirements/py${{ matrix.python-version }}.yml
```

### Comparing `pydaymet-0.2.0/.gitignore` & `pydaymet-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/.pre-commit-config.yaml` & `pydaymet-0.9.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

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
+        exclude: tests
         files: pydaymet
 
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
         args: [-lll, --recursive, pydaymet]
         files: .py$
```

### Comparing `pydaymet-0.2.0/CODE_OF_CONDUCT.rst` & `pydaymet-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/CONTRIBUTING.rst` & `pydaymet-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/LICENSE` & `pydaymet-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/Makefile` & `pydaymet-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/PKG-INFO` & `pydaymet-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: pydaymet
-Version: 0.2.0
+Version: 0.9.0
 Summary: Access the climate data from the Daymet database through ORNL's RESTful service.
 Home-page: https://github.com/cheginit/pydaymet
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT license
 Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pydaymet_logo.png
             :target: https://github.com/cheginit/pydaymet
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
@@ -85,31 +85,47 @@
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
             :target: https://github.com/pre-commit/pre-commit
             :alt: pre-commit
         
         |
         
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
         Features
         --------
         
         PyDaymet is a part of Hydrodata software stack and provides an interface to access to daily
         climate data through the `Daymet <https://daymet.ornl.gov/>`__ RESTful service. Both single
-        pixel and gridded data can be requested which are returned as ``pandas.DataFrame`` for
-        single pixel requests and ``xarray.Dataset`` for gridded data requests. Additionally, it
-        can compute Potential EvapoTranspiration (PET) using
+        pixel and gridded data can be requested which are returned as ``pandas.DataFrame`` and
+        ``xarray.Dataset``, respectively. Climate data is avaiable for CONUS, Hawaii, and Puerto Rico.
+        Additionally, PyDaymet can compute Potential EvapoTranspiration (PET) using
         `UN-FAO 56 paper <http://www.fao.org/docrep/X0490E/X0490E00.htm>`__
         method for both single pixel and gridded data.
         
+        Note that starting from version ``0.9.0``, the recently released version of Daymet database
+        is used. You can check the release information `here <https://daac.ornl.gov/DAYMET/guides/Daymet_Daily_V4.html>`_
+        Moreover, there's a new function called ``get_bycoords`` that is an alternative to ``get_byloc``
+        for getting climate data at a single pixel. This new function uses THREDDS data server
+        with NetCDF Subset Service (NCSS), and supports getting monthly and annual summaries directly
+        from the server. You can pass ``time_scale`` as ``daily``, ``monthly``, or ``annual``
+        to ``get_bygeom`` or ``get_bycoords`` functions to download the respective summaries.
+        ``get_bycoords`` will replace ``get_byloc`` in  the future.
+        So, please consider migrating your code by replacing ``get_byloc`` with ``get_bycoords``. The
+        input arguments of ``get_bycoords`` is identical to ``get_bygeom``. Another difference
+        between ``get_byloc`` and ``get_bycoords`` is column names where ``get_bycoords`` uses
+        the units that are returned by NCSS server. Moreover, both ``get_bygeom`` and ``get_bycoords``
+        accept an additional argument called ``region`` for passing the region of interest.
+        
         You can try using PyDaymet without installing it on you system by clicking on the binder badge
         below the PyDaymet banner. A Jupyter notebook instance with the Hydrodata software stack
         pre-installed will be launched in your web browser and you can start coding!
         
+        Please note that since Hydrodata is in early development stages, while the provided
+        functionaities should be stable, changes in APIs are possible in new releases. But we
+        appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+        
         Moreover, requests for additional functionalities can be submitted via
         `issue tracker <https://github.com/cheginit/pydaymet/issues>`__.
         
         Installation
         ------------
         
         You can install PyDaymet using ``pip`` after installing ``libgdal`` on your system
@@ -125,42 +141,74 @@
         .. code-block:: console
         
             $ conda install -c conda-forge pydaymet
         
         Quick start
         -----------
         
-        PyDaymet offers two functions for getting climate data; ``get_byloc`` and ``get_bygeom``.
+        PyDaymet offers two functions for getting climate data; ``get_bycoords`` and ``get_bygeom``.
         The arguments of these functions are identical except the first argument where the latter
         should be polygon and the former should be a coordinate (a tuple of length two as in (x, y)).
         The input geometry or coordinate can be in any valid CRS (defaults to EPSG:4326). The ``dates``
         argument can be either a tuple of length two like ``(start_str, end_str)`` or a list of years
         like ``[2000, 2005]``. It is noted that both functions have a ``pet`` flag for computing PET.
+        Additionally, we can pass ``time_scale`` to get daily, monthly or annual summaries. This flag
+        by default is set to daily.
         
         .. code-block:: python
         
             from pynhd import NLDI
             import pydaymet as daymet
         
-            dates = ("2000-01-01", "2000-06-12")
-            variables = ["prcp", "tmin"]
+            geometry = NLDI().get_basins("01031500").geometry[0]
+        
+            var = ["prcp", "tmin"]
+            dates = ("2000-01-01", "2000-06-30")
+        
+            daily = daymet.get_bygeom(geometry, dates, variables=var, pet=True)
+            monthly = daymet.get_bygeom(geometry, dates, variables=var, time_scale="monthly")
+        
+        If the input geometry (or coordinate) is in a CRS other than EPSG:4326, we should pass
+        it to the functions.
         
-            geometry = NLDI.getfeature_byid("nwissite", "USGS-01031500", basin=True).geometry[0]
-            clm_g = daymet.get_bygeom(geometry, dates, variables=variables, pet=True)
+        .. code-block:: python
         
             coords = (-1431147.7928, 318483.4618)
             crs = "epsg:3542"
-            clm_p = daymet.get_byloc(coords, dates, crs=crs, variables=variables, pet=True)
+            dates = ("2000-01-01", "2006-12-31")
+            annual = daymet.get_bycoords(
+                coords, dates, variables=var, loc_crs=crs, time_scale="annual"
+            )
+        
+        Next, let's get annual total precipitation for Hawaii and Puerto Rico for 2010.
+        
+        .. code-block:: python
+        
+            hi_ext = (-160.3055, 17.9539, -154.7715, 23.5186)
+            pr_ext = (-67.9927, 16.8443, -64.1195, 19.9381)
+            hi = daymet.get_bygeom(hi_ext, 2010, variables="prcp", region="hi", time_scale="annual")
+            pr = daymet.get_bygeom(pr_ext, 2010, variables="prcp", region="pr", time_scale="annual")
         
         Some example plots are shown below:
         
-        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_pydaymet.png
-            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_pydaymet.png
-            :width: 600
-            :align: center
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_grid.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_grid.png
+            :width: 45%
+        
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_loc.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_loc.png
+            :width: 45%
+        
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hi.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hi.png
+            :width: 45%
+        
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pr.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pr.png
+            :width: 45%
         
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

### Comparing `pydaymet-0.2.0/README.rst` & `pydaymet-0.9.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pydaymet_logo.png
     :target: https://github.com/cheginit/pydaymet
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
@@ -77,31 +77,47 @@
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
     :target: https://github.com/pre-commit/pre-commit
     :alt: pre-commit
 
 |
 
-🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-
 Features
 --------
 
 PyDaymet is a part of Hydrodata software stack and provides an interface to access to daily
 climate data through the `Daymet <https://daymet.ornl.gov/>`__ RESTful service. Both single
-pixel and gridded data can be requested which are returned as ``pandas.DataFrame`` for
-single pixel requests and ``xarray.Dataset`` for gridded data requests. Additionally, it
-can compute Potential EvapoTranspiration (PET) using
+pixel and gridded data can be requested which are returned as ``pandas.DataFrame`` and
+``xarray.Dataset``, respectively. Climate data is avaiable for CONUS, Hawaii, and Puerto Rico.
+Additionally, PyDaymet can compute Potential EvapoTranspiration (PET) using
 `UN-FAO 56 paper <http://www.fao.org/docrep/X0490E/X0490E00.htm>`__
 method for both single pixel and gridded data.
 
+Note that starting from version ``0.9.0``, the recently released version of Daymet database
+is used. You can check the release information `here <https://daac.ornl.gov/DAYMET/guides/Daymet_Daily_V4.html>`_
+Moreover, there's a new function called ``get_bycoords`` that is an alternative to ``get_byloc``
+for getting climate data at a single pixel. This new function uses THREDDS data server
+with NetCDF Subset Service (NCSS), and supports getting monthly and annual summaries directly
+from the server. You can pass ``time_scale`` as ``daily``, ``monthly``, or ``annual``
+to ``get_bygeom`` or ``get_bycoords`` functions to download the respective summaries.
+``get_bycoords`` will replace ``get_byloc`` in  the future.
+So, please consider migrating your code by replacing ``get_byloc`` with ``get_bycoords``. The
+input arguments of ``get_bycoords`` is identical to ``get_bygeom``. Another difference
+between ``get_byloc`` and ``get_bycoords`` is column names where ``get_bycoords`` uses
+the units that are returned by NCSS server. Moreover, both ``get_bygeom`` and ``get_bycoords``
+accept an additional argument called ``region`` for passing the region of interest.
+
 You can try using PyDaymet without installing it on you system by clicking on the binder badge
 below the PyDaymet banner. A Jupyter notebook instance with the Hydrodata software stack
 pre-installed will be launched in your web browser and you can start coding!
 
+Please note that since Hydrodata is in early development stages, while the provided
+functionaities should be stable, changes in APIs are possible in new releases. But we
+appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+
 Moreover, requests for additional functionalities can be submitted via
 `issue tracker <https://github.com/cheginit/pydaymet/issues>`__.
 
 Installation
 ------------
 
 You can install PyDaymet using ``pip`` after installing ``libgdal`` on your system
@@ -117,42 +133,74 @@
 .. code-block:: console
 
     $ conda install -c conda-forge pydaymet
 
 Quick start
 -----------
 
-PyDaymet offers two functions for getting climate data; ``get_byloc`` and ``get_bygeom``.
+PyDaymet offers two functions for getting climate data; ``get_bycoords`` and ``get_bygeom``.
 The arguments of these functions are identical except the first argument where the latter
 should be polygon and the former should be a coordinate (a tuple of length two as in (x, y)).
 The input geometry or coordinate can be in any valid CRS (defaults to EPSG:4326). The ``dates``
 argument can be either a tuple of length two like ``(start_str, end_str)`` or a list of years
 like ``[2000, 2005]``. It is noted that both functions have a ``pet`` flag for computing PET.
+Additionally, we can pass ``time_scale`` to get daily, monthly or annual summaries. This flag
+by default is set to daily.
 
 .. code-block:: python
 
     from pynhd import NLDI
     import pydaymet as daymet
 
-    dates = ("2000-01-01", "2000-06-12")
-    variables = ["prcp", "tmin"]
+    geometry = NLDI().get_basins("01031500").geometry[0]
+
+    var = ["prcp", "tmin"]
+    dates = ("2000-01-01", "2000-06-30")
+
+    daily = daymet.get_bygeom(geometry, dates, variables=var, pet=True)
+    monthly = daymet.get_bygeom(geometry, dates, variables=var, time_scale="monthly")
+
+If the input geometry (or coordinate) is in a CRS other than EPSG:4326, we should pass
+it to the functions.
 
-    geometry = NLDI.getfeature_byid("nwissite", "USGS-01031500", basin=True).geometry[0]
-    clm_g = daymet.get_bygeom(geometry, dates, variables=variables, pet=True)
+.. code-block:: python
 
     coords = (-1431147.7928, 318483.4618)
     crs = "epsg:3542"
-    clm_p = daymet.get_byloc(coords, dates, crs=crs, variables=variables, pet=True)
+    dates = ("2000-01-01", "2006-12-31")
+    annual = daymet.get_bycoords(
+        coords, dates, variables=var, loc_crs=crs, time_scale="annual"
+    )
+
+Next, let's get annual total precipitation for Hawaii and Puerto Rico for 2010.
+
+.. code-block:: python
+
+    hi_ext = (-160.3055, 17.9539, -154.7715, 23.5186)
+    pr_ext = (-67.9927, 16.8443, -64.1195, 19.9381)
+    hi = daymet.get_bygeom(hi_ext, 2010, variables="prcp", region="hi", time_scale="annual")
+    pr = daymet.get_bygeom(pr_ext, 2010, variables="prcp", region="pr", time_scale="annual")
 
 Some example plots are shown below:
 
-.. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_pydaymet.png
-    :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_pydaymet.png
-    :width: 600
-    :align: center
+.. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_grid.png
+    :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_grid.png
+    :width: 45%
+
+.. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_loc.png
+    :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_loc.png
+    :width: 45%
+
+.. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hi.png
+    :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hi.png
+    :width: 45%
+
+.. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pr.png
+    :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pr.png
+    :width: 45%
 
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

### Comparing `pydaymet-0.2.0/ci/requirements/environment.yml` & `pydaymet-0.9.0/ci/requirements/environment.yml`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
   - xarray
   - scipy
   - netCDF4
   - geopandas
   - rasterio
   - shapely
   - orjson
+  - simplejson
   - lxml
   - dask
 
   - setuptools_scm
   - pytest-cov
   - pytest-xdist
   - pre-commit
```

### Comparing `pydaymet-0.2.0/docs/Makefile` & `pydaymet-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/docs/conf.py` & `pydaymet-0.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 if "conda" in sys.executable:
     print("conda environment:")
     subprocess.run(["conda", "list"])
 else:
     print("pip environment:")
     subprocess.run(["pip", "list"])
 
-print(f"Hydrodata: {pydaymet.__version__}, {pydaymet.__file__}")
+print(f"PyDaymet: {pydaymet.__version__}, {pydaymet.__file__}")
 
 with suppress(ImportError):
     import matplotlib
 
     matplotlib.use("Agg")
 
 
 # -- Project information -----------------------------------------------------
 
-project = "Hydrodata"
+project = "PyDaymet"
 author = "Taher Chegini"
 copyright = f"2019-{datetime.datetime.now().year}, {author}"
-html_title = "Hydrodata"
+html_title = "PyDaymet"
 
 # The full version, including alpha/beta/rc tags
 release = LooseVersion(pydaymet.__version__).vstring
 
 # try:
 #     import rasterio
 # except ImportError:
```

### Comparing `pydaymet-0.2.0/docs/make.bat` & `pydaymet-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/docs/pydaymet.rst` & `pydaymet-0.9.0/docs/pydaymet.rst`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/pydaymet/exceptions.py` & `pydaymet-0.9.0/pydaymet/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Customized PyDaymet exceptions."""
-from typing import Generator, List, Optional, Union
+from typing import Any, Generator, List, Optional, Union
 
 
 class ZeroMatched(ValueError):
     """Exception raised when a function argument is missing."""
 
 
 class InvalidInputValue(Exception):
@@ -14,15 +14,15 @@
     inp : str
         Name of the input parameter
     valid_inputs : tuple
         List of valid inputs
     """
 
     def __init__(
-        self, inp: str, valid_inputs: Union[List[str], Generator[str, None, None]]
+        self, inp: str, valid_inputs: Union[List[Any], Generator[str, None, None]]
     ) -> None:
         self.message = f"Given {inp} is invalid. Valid {inp}s are:\n" + ", ".join(
             str(i) for i in valid_inputs
         )
         super().__init__(self.message)
 
     def __str__(self) -> str:
```

### Comparing `pydaymet-0.2.0/pydaymet/print_versions.py` & `pydaymet-0.9.0/pydaymet/print_versions.py`

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

### Comparing `pydaymet-0.2.0/pydaymet.egg-info/PKG-INFO` & `pydaymet-0.9.0/pydaymet.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: pydaymet
-Version: 0.2.0
+Version: 0.9.0
 Summary: Access the climate data from the Daymet database through ORNL's RESTful service.
 Home-page: https://github.com/cheginit/pydaymet
 Author: Taher Chegini
 Author-email: cheginit@gmail.com
 License: MIT license
 Description: .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pydaymet_logo.png
             :target: https://github.com/cheginit/pydaymet
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
@@ -85,31 +85,47 @@
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
             :target: https://github.com/pre-commit/pre-commit
             :alt: pre-commit
         
         |
         
-        🚨 **This package is under heavy development and breaking changes are likely to happen.** 🚨
-        
         Features
         --------
         
         PyDaymet is a part of Hydrodata software stack and provides an interface to access to daily
         climate data through the `Daymet <https://daymet.ornl.gov/>`__ RESTful service. Both single
-        pixel and gridded data can be requested which are returned as ``pandas.DataFrame`` for
-        single pixel requests and ``xarray.Dataset`` for gridded data requests. Additionally, it
-        can compute Potential EvapoTranspiration (PET) using
+        pixel and gridded data can be requested which are returned as ``pandas.DataFrame`` and
+        ``xarray.Dataset``, respectively. Climate data is avaiable for CONUS, Hawaii, and Puerto Rico.
+        Additionally, PyDaymet can compute Potential EvapoTranspiration (PET) using
         `UN-FAO 56 paper <http://www.fao.org/docrep/X0490E/X0490E00.htm>`__
         method for both single pixel and gridded data.
         
+        Note that starting from version ``0.9.0``, the recently released version of Daymet database
+        is used. You can check the release information `here <https://daac.ornl.gov/DAYMET/guides/Daymet_Daily_V4.html>`_
+        Moreover, there's a new function called ``get_bycoords`` that is an alternative to ``get_byloc``
+        for getting climate data at a single pixel. This new function uses THREDDS data server
+        with NetCDF Subset Service (NCSS), and supports getting monthly and annual summaries directly
+        from the server. You can pass ``time_scale`` as ``daily``, ``monthly``, or ``annual``
+        to ``get_bygeom`` or ``get_bycoords`` functions to download the respective summaries.
+        ``get_bycoords`` will replace ``get_byloc`` in  the future.
+        So, please consider migrating your code by replacing ``get_byloc`` with ``get_bycoords``. The
+        input arguments of ``get_bycoords`` is identical to ``get_bygeom``. Another difference
+        between ``get_byloc`` and ``get_bycoords`` is column names where ``get_bycoords`` uses
+        the units that are returned by NCSS server. Moreover, both ``get_bygeom`` and ``get_bycoords``
+        accept an additional argument called ``region`` for passing the region of interest.
+        
         You can try using PyDaymet without installing it on you system by clicking on the binder badge
         below the PyDaymet banner. A Jupyter notebook instance with the Hydrodata software stack
         pre-installed will be launched in your web browser and you can start coding!
         
+        Please note that since Hydrodata is in early development stages, while the provided
+        functionaities should be stable, changes in APIs are possible in new releases. But we
+        appreciate it if you give this project a try and provide feedback. Contributions are most welcome.
+        
         Moreover, requests for additional functionalities can be submitted via
         `issue tracker <https://github.com/cheginit/pydaymet/issues>`__.
         
         Installation
         ------------
         
         You can install PyDaymet using ``pip`` after installing ``libgdal`` on your system
@@ -125,42 +141,74 @@
         .. code-block:: console
         
             $ conda install -c conda-forge pydaymet
         
         Quick start
         -----------
         
-        PyDaymet offers two functions for getting climate data; ``get_byloc`` and ``get_bygeom``.
+        PyDaymet offers two functions for getting climate data; ``get_bycoords`` and ``get_bygeom``.
         The arguments of these functions are identical except the first argument where the latter
         should be polygon and the former should be a coordinate (a tuple of length two as in (x, y)).
         The input geometry or coordinate can be in any valid CRS (defaults to EPSG:4326). The ``dates``
         argument can be either a tuple of length two like ``(start_str, end_str)`` or a list of years
         like ``[2000, 2005]``. It is noted that both functions have a ``pet`` flag for computing PET.
+        Additionally, we can pass ``time_scale`` to get daily, monthly or annual summaries. This flag
+        by default is set to daily.
         
         .. code-block:: python
         
             from pynhd import NLDI
             import pydaymet as daymet
         
-            dates = ("2000-01-01", "2000-06-12")
-            variables = ["prcp", "tmin"]
+            geometry = NLDI().get_basins("01031500").geometry[0]
+        
+            var = ["prcp", "tmin"]
+            dates = ("2000-01-01", "2000-06-30")
+        
+            daily = daymet.get_bygeom(geometry, dates, variables=var, pet=True)
+            monthly = daymet.get_bygeom(geometry, dates, variables=var, time_scale="monthly")
+        
+        If the input geometry (or coordinate) is in a CRS other than EPSG:4326, we should pass
+        it to the functions.
         
-            geometry = NLDI.getfeature_byid("nwissite", "USGS-01031500", basin=True).geometry[0]
-            clm_g = daymet.get_bygeom(geometry, dates, variables=variables, pet=True)
+        .. code-block:: python
         
             coords = (-1431147.7928, 318483.4618)
             crs = "epsg:3542"
-            clm_p = daymet.get_byloc(coords, dates, crs=crs, variables=variables, pet=True)
+            dates = ("2000-01-01", "2006-12-31")
+            annual = daymet.get_bycoords(
+                coords, dates, variables=var, loc_crs=crs, time_scale="annual"
+            )
+        
+        Next, let's get annual total precipitation for Hawaii and Puerto Rico for 2010.
+        
+        .. code-block:: python
+        
+            hi_ext = (-160.3055, 17.9539, -154.7715, 23.5186)
+            pr_ext = (-67.9927, 16.8443, -64.1195, 19.9381)
+            hi = daymet.get_bygeom(hi_ext, 2010, variables="prcp", region="hi", time_scale="annual")
+            pr = daymet.get_bygeom(pr_ext, 2010, variables="prcp", region="pr", time_scale="annual")
         
         Some example plots are shown below:
         
-        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_pydaymet.png
-            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/example_plots_pydaymet.png
-            :width: 600
-            :align: center
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_grid.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_grid.png
+            :width: 45%
+        
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_loc.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/daymet_loc.png
+            :width: 45%
+        
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hi.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/hi.png
+            :width: 45%
+        
+        .. image:: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pr.png
+            :target: https://raw.githubusercontent.com/cheginit/hydrodata/master/docs/_static/pr.png
+            :width: 45%
         
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

### Comparing `pydaymet-0.2.0/pydaymet.egg-info/SOURCES.txt` & `pydaymet-0.9.0/pydaymet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/scripts/generate_pip_deps_from_conda.py` & `pydaymet-0.9.0/scripts/generate_pip_deps_from_conda.py`

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

### Comparing `pydaymet-0.2.0/setup.cfg` & `pydaymet-0.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,22 @@
 known_first_party = pydaymet
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

### Comparing `pydaymet-0.2.0/setup.py` & `pydaymet-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pydaymet-0.2.0/tests/test_exceptions.py` & `pydaymet-0.9.0/tests/test_exceptions.py`

 * *Files identical despite different names*

