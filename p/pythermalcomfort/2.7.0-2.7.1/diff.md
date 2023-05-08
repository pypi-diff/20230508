# Comparing `tmp/pythermalcomfort-2.7.0.tar.gz` & `tmp/pythermalcomfort-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythermalcomfort-2.7.0.tar", last modified: Wed Feb 15 23:07:17 2023, max compression
+gzip compressed data, was "pythermalcomfort-2.7.1.tar", last modified: Mon May  8 04:25:15 2023, max compression
```

## Comparing `pythermalcomfort-2.7.0.tar` & `pythermalcomfort-2.7.1.tar`

### file list

```diff
@@ -1,67 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.819342 pythermalcomfort-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-02-15 23:07:17.819342 pythermalcomfort-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.815342 pythermalcomfort-2.7.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/ci/appveyor-with-compiler.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.815342 pythermalcomfort-2.7.0/ci/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/ci/templates/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/ci/templates/.travis.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.815342 pythermalcomfort-2.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.815342 pythermalcomfort-2.7.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/reference/pythermalcomfort.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.815342 pythermalcomfort-2.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/examples/calc_adaptive_ASHRAE.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/examples/calc_adaptive_EN.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/examples/calc_phs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/examples/calc_pmv_ppd.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/examples/calc_set_tmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/examples/calc_utci.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-15 23:07:17.819342 pythermalcomfort-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.811342 pythermalcomfort-2.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.819342 pythermalcomfort-2.7.0/src/pythermalcomfort/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/src/pythermalcomfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/src/pythermalcomfort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/src/pythermalcomfort/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   118878 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/src/pythermalcomfort/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/src/pythermalcomfort/optimized_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/src/pythermalcomfort/psychrometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/src/pythermalcomfort/shared_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/src/pythermalcomfort/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.819342 pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-02-15 23:07:17.000000 pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-15 23:07:17.000000 pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 23:07:17.000000 pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-15 23:07:17.000000 pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 23:07:17.000000 pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-15 23:07:17.000000 pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-15 23:07:17.000000 pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:07:17.819342 pythermalcomfort-2.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    41005 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/tests/test_pythermalcomfort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-02-15 23:07:09.000000 pythermalcomfort-2.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/appveyor-with-compiler.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/ci/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/templates/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/templates/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/contact_us.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/reference/pythermalcomfort.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_adaptive_ASHRAE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_adaptive_EN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_jos3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_phs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_pmv_ppd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_set_tmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_utci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/src/pythermalcomfort/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37644 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/thermoregulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176008 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/optimized_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/psychrometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/shared_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/tests/test_jos3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41005 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/tests/test_pythermalcomfort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/tox.ini
```

### Comparing `pythermalcomfort-2.7.0/.appveyor.yml` & `pythermalcomfort-2.7.1/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/.cookiecutterrc` & `pythermalcomfort-2.7.1/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/.readthedocs.yml` & `pythermalcomfort-2.7.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/.travis.yml` & `pythermalcomfort-2.7.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/AUTHORS.rst` & `pythermalcomfort-2.7.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/CHANGELOG.rst` & `pythermalcomfort-2.7.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/CONTRIBUTING.rst` & `pythermalcomfort-2.7.1/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 3. Create a branch for local development::
 
     git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-4. When you're done making changes run all the checks and docs builder with `tox <https://tox.readthedocs.io/en/latest/install.html>`_ one command::
+4. When you're done making changes run all the checks and docs builder with tox one command::
 
     tox
 
 5. Commit your changes and push your branch to GitHub::
 
     git add .
     git commit -m "Your detailed description of your changes."
```

### Comparing `pythermalcomfort-2.7.0/LICENSE` & `pythermalcomfort-2.7.1/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
 
-Copyright (c) 2019-2020, Federico Tartarini
+Copyright (c) 2019 Federico Tartarini
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice (including the next paragraph) shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pythermalcomfort-2.7.0/PKG-INFO` & `pythermalcomfort-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pythermalcomfort
-Version: 2.7.0
+Version: 2.7.1
 Summary: Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET, adaptive) and convert physical variables. Please cite us if you use this package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python package for thermal comfort research. SoftwareX 12, 100578. https://doi.org/10.1016/j.softx.2020.100578
 Home-page: https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort
 Author: Federico Tartarini
 Author-email: cbecomforttool@gmail.com
 License: MIT
 Project-URL: Documentation, https://pythermalcomfort.readthedocs.io/
 Project-URL: Changelog, https://pythermalcomfort.readthedocs.io/en/latest/changelog.html
```

### Comparing `pythermalcomfort-2.7.0/README.rst` & `pythermalcomfort-2.7.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     * - docs
       - |docs|
     * - license
       - |license|
     * - downloads
       - |downloads|
     * - tests
-      - | |travis| |appveyor|
-        | |codecov| |requires|
+      - | |appveyor| |codecov|
     * - package
       - | |version| |wheel|
         | |supported-ver|
         | |package-health|
 
 .. |package-health| image:: https://snyk.io/advisor/python/pythermalcomfort/badge.svg
     :target: https://snyk.io/advisor/python/pythermalcomfort
@@ -32,26 +31,18 @@
 .. |docs| image:: https://readthedocs.org/projects/pythermalcomfort/badge/?style=flat
     :target: https://readthedocs.org/projects/pythermalcomfort
     :alt: Documentation Status
 
 .. |downloads| image:: https://img.shields.io/pypi/dm/pythermalcomfort?color=brightgreen
     :alt: PyPI - Downloads
 
-.. |travis| image:: https://api.travis-ci.org/CenterForTheBuiltEnvironment/pythermalcomfort.svg?branch=master
-    :alt: Travis-CI Build Status
-    :target: https://travis-ci.org/CenterForTheBuiltEnvironment/pythermalcomfort
-
 .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/CenterForTheBuiltEnvironment/pythermalcomfort?branch=master&svg=true
     :alt: AppVeyor Build Status
     :target: https://ci.appveyor.com/project/CenterForTheBuiltEnvironment/pythermalcomfort
 
-.. |requires| image:: https://requires.io/github/CenterForTheBuiltEnvironment/pythermalcomfort/requirements.svg?branch=master
-    :alt: Requirements Status
-    :target: https://requires.io/github/CenterForTheBuiltEnvironment/pythermalcomfort/requirements/?branch=master
-
 .. |codecov| image:: https://codecov.io/github/CenterForTheBuiltEnvironment/pythermalcomfort/coverage.svg?branch=master
     :alt: Coverage Status
     :target: https://codecov.io/github/CenterForTheBuiltEnvironment/pythermalcomfort
 
 .. |version| image:: https://img.shields.io/pypi/v/pythermalcomfort.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/pythermalcomfort
```

### Comparing `pythermalcomfort-2.7.0/ci/appveyor-with-compiler.cmd` & `pythermalcomfort-2.7.1/ci/appveyor-with-compiler.cmd`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/ci/bootstrap.py` & `pythermalcomfort-2.7.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/ci/templates/.appveyor.yml` & `pythermalcomfort-2.7.1/ci/templates/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/ci/templates/.travis.yml` & `pythermalcomfort-2.7.1/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/docs/conf.py` & `pythermalcomfort-2.7.1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "pythermalcomfort"
-year = "2019-2020"
+year = "2019"
 author = "Federico Tartarini"
 copyright = "{0}, {1}".format(year, author)
-version = release = "2.7.0"
+version = release = "2.7.1"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": (
         "https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort/issues/%s",
         "#",
```

### Comparing `pythermalcomfort-2.7.0/docs/reference/pythermalcomfort.rst` & `pythermalcomfort-2.7.1/docs/reference/pythermalcomfort.rst`

 * *Files 13% similar despite different names*

```diff
@@ -36,54 +36,15 @@
 -------------------
 
 .. autofunction:: pythermalcomfort.models.cooling_effect
 
 Joint system thermoregulation model (JOS-3)
 -------------------------------------------
 
-    JOS-3 is a numeric model to simulate a human thermoregulation [19]_.
-    The JOS-3 model consists of 83 nodes. Human physiological responses and body temperatures are calculated using the backward difference method. JOS-3 uses brown adipose tissue activity, aging effects, and heat gain by shortwave solar radiation at the skin to predict human physiological responses. It also considers personal characteristics in transient and non-uniform thermal environments. The JOS-3 was validated by comparing the results with those of human subject tests conducted under stable and transient conditions [19]_.
-
-    To read the JOS-3 official documentation please use the following commands:
-
-    .. code-block:: python
-
-        >>> import jos3
-        >>> model = jos3.JOS3()
-
-        >>> # Print documentation:
-        >>> print(model.__doc__)
-
-        >>> # Show the documentation of the output parameters:
-        >>> print(jos3.show_outparam_docs())
-
-
-    Below an example on how to use the JOS-3 model
-
-    .. code-block:: python
-
-        >>> import pandas as pd
-        >>> import jos3
-
-        >>> model = jos3.JOS3(height=1.7, weight=60, age=30)  # Builds a model
-
-        >>> # Set the first condition
-        >>> model.To = 28  # Operative temperature [oC]
-        >>> model.RH = 40  # Relative humidity [%]
-        >>> model.Va = 0.2  # Air velocity [m/s]
-        >>> model.PAR = 1.2  # Physical activity ratio [-]
-        >>> model.simulate(60)  # Exposure time = 60 [min]
-
-        >>> # Set the next condition
-        >>> model.To = 20  # Changes only operative temperature
-        >>> model.simulate(60)  # Additional exposure time = 60 [min]
-
-        >>> # Show the results
-        >>> df = pd.DataFrame(model.dict_results())  # Make pandas.DataFrame
-        >>> df.TskMean.plot()  # Show the graph of mean skin temp.
+.. autofunction:: pythermalcomfort.models.JOS3
 
 
 Adaptive Thermal Heat Balance (ATHB)
 ------------------------------------
 
 .. autofunction:: pythermalcomfort.models.athb
 
@@ -275,15 +236,14 @@
 .. [12] Rothfusz LP (1990) The heat index equation. NWS Southern Region Technical Attachment, SR/SSD 90–23, Fort Worth, Texas
 .. [13] Steadman RG (1979) The assessment of sultriness. Part I: A temperature-humidity index based on human physiology and clothing science. J Appl Meteorol 18:861–873
 .. [14] Masterton JM, Richardson FA. Humidex, a method of quantifying human discomfort due to excessive heat and humidity. Downsview, Ontario: CLI 1-79, Environment Canada, Atmospheric Environment Service, 1979
 .. [15] Havenith, G., Fiala, D., 2016. Thermal indices and thermophysiological modeling for heat stress. Compr. Physiol. 6, 255–302. https://doi.org/10.1002/cphy.c140051
 .. [16] Blazejczyk, K., Epstein, Y., Jendritzky, G., Staiger, H., Tinz, B., 2012. Comparison of UTCI to selected thermal indices. Int. J. Biometeorol. 56, 515–535. https://doi.org/10.1007/s00484-011-0453-2
 .. [17] Steadman RG (1984) A universal scale of apparent temperature. J Appl Meteorol Climatol 23:1674–1687
 .. [18] ASHRAE, 2017. 2017 ASHRAE Handbook Fundamentals. Atlanta.
-.. [19] Takahashi, Y., Nomoto, A., Yoda, S., Hisayama, R., Ogata, M., Ozeki, Y., & Tanabe, S. ichi. (2021). Thermoregulation model JOS-3 with new open source code. Energy and Buildings, 231, 110575. https://doi.org/10.1016/j.enbuild.2020.110575
 .. [20] Höppe P. The physiological equivalent temperature - a universal index for the biometeorological assessment of the thermal environment. Int J Biometeorol. 1999 Oct;43(2):71-5. doi: 10.1007/s004840050118. PMID: 10552310.
 .. [21] Walther, E. and Goestchel, Q., 2018. The PET comfort index: Questioning the model. Building and Environment, 137, pp.1-10. https://doi.org/10.1016/j.buildenv.2018.03.054
 .. [22] Teitelbaum, E., Alsaad, H., Aviv, D., Kim, A., Voelker, C., Meggers, F., & Pantelic, J. (2022). Addressing a systematic error correcting for free and mixed convection when measuring mean radiant temperature with globe thermometers. Scientific Reports, 12(1), 1–18. https://doi.org/10.1038/s41598-022-10172-5
 .. [23] Liu, S., Schiavon, S., Kabanshi, A., Nazaroff, W.W., 2017. Predicted percentage dissatisfied with ankle draft. Indoor Air 27, 852–862. https://doi.org/10.1111/ina.12364
 .. [24] Polydoros, Anastasios & Cartalis, Constantinos. (2015). Use of Earth Observation based indices for the monitoring of built-up area features and dynamics in support of urban energy studies. Energy and Buildings. 98. 92-99. 10.1016/j.enbuild.2014.09.060.
 .. [25] Yao, Runming & Li, Baizhan & Liu, Jing. (2009). A theoretical adaptive model of thermal comfort – Adaptive Predicted Mean Vote (aPMV). Building and Environment. 44. 2089-2096. 10.1016/j.buildenv.2009.02.014.
 .. [26] Fanger, P. & Toftum, Jorn. (2002). Extension of the PMV model to non-air-conditioned buildings in warm climates. Energy and Buildings. 34. 533-536. 10.1016/S0378-7788(02)00003-8.
```

### Comparing `pythermalcomfort-2.7.0/docs/usage.rst` & `pythermalcomfort-2.7.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/examples/calc_adaptive_ASHRAE.py` & `pythermalcomfort-2.7.1/examples/calc_adaptive_ASHRAE.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/examples/calc_adaptive_EN.py` & `pythermalcomfort-2.7.1/examples/calc_adaptive_EN.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/examples/calc_phs.py` & `pythermalcomfort-2.7.1/examples/calc_phs.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/examples/calc_pmv_ppd.py` & `pythermalcomfort-2.7.1/examples/calc_pmv_ppd.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/examples/calc_utci.py` & `pythermalcomfort-2.7.1/examples/calc_utci.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/setup.cfg` & `pythermalcomfort-2.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/setup.py` & `pythermalcomfort-2.7.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,23 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="pythermalcomfort",
-    version="2.7.0",
+    version="2.7.1",
     license="MIT",
-    description="Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET, adaptive) and convert physical variables. Please cite us if you use this package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python package for thermal comfort research. SoftwareX 12, 100578. https://doi.org/10.1016/j.softx.2020.100578",
+    description=(
+        "Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET,"
+        " adaptive) and convert physical variables. Please cite us if you use this"
+        " package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python"
+        " package for thermal comfort research. SoftwareX 12, 100578."
+        " https://doi.org/10.1016/j.softx.2020.100578"
+    ),
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
@@ -63,30 +69,31 @@
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Scientific/Engineering",
         "Topic :: Utilities",
     ],
     project_urls={
         "Documentation": "https://pythermalcomfort.readthedocs.io/",
         "Changelog": "https://pythermalcomfort.readthedocs.io/en/latest/changelog.html",
-        "Issue Tracker": "https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort/issues",
+        "Issue Tracker": (
+            "https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort/issues"
+        ),
     },
     keywords=[
         "thermal comfort",
         "pmv",
         "ppd",
         "building design",
         "compliance",
         "thermal environment",
         "built environment",
     ],
     python_requires=">=3.6.0",
     install_requires=[
         "scipy",
         "numba",
-        "jos3",
         "numpy",
     ],  # eg: 'aspectlib==1.1.1', 'six>=1.7',
     extras_require={
         # eg:
         #   'rst': ['docutils>=0.11'],
         #   ':python_version=="2.6"': ['argparse'],
     },
```

### Comparing `pythermalcomfort-2.7.0/src/pythermalcomfort/cli.py` & `pythermalcomfort-2.7.1/src/pythermalcomfort/cli.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/src/pythermalcomfort/models.py` & `pythermalcomfort-2.7.1/src/pythermalcomfort/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import numpy as np
+import re
 import warnings
+import csv
+import datetime as dt
+import os
 from pythermalcomfort.psychrometrics import t_o, p_sat_torr, p_sat, psy_ta_rh
 from pythermalcomfort.utilities import (
     units_converter,
     transpose_sharp_altitude,
     check_standard_compliance,
     mapping,
     check_standard_compliance_array,
@@ -16,14 +20,29 @@
     two_nodes_optimized,
     phs_optimized,
     pmv_ppd_optimized,
     utci_optimized,
     two_nodes_optimized_return_set,
 )
 
+# import functions and valuables from "jos3_functions" folder
+from pythermalcomfort.jos3_functions import thermoregulation as threg
+from pythermalcomfort.jos3_functions import matrix
+from pythermalcomfort.jos3_functions.matrix import (
+    NUM_NODES,
+    INDEX,
+    VINDEX,
+    BODY_NAMES,
+    remove_body_name,
+)
+from pythermalcomfort.jos3_functions import construction as cons
+from pythermalcomfort.jos3_functions.construction import _BSAst, _to17array
+from pythermalcomfort.jos3_functions.parameters import ALL_OUT_PARAMS
+from pythermalcomfort.__init__ import __version__
+
 
 def cooling_effect(tdb, tr, vr, rh, met, clo, wme=0, units="SI"):
     """Returns the value of the Cooling Effect (`CE`_) calculated in compliance
     with the ASHRAE 55 2020 Standard [1]_. The `CE`_ of the elevated air speed
     is the value that, when subtracted equally from both the average air
     temperature and the mean radiant temperature, yields the same `SET`_ under
     still air as in the first `SET`_ calculation under elevated air speed. The
@@ -905,16 +924,14 @@
         True if heat strain is caused by skin blood flow (m_bl) reaching its maximum value
     heat_strain_w : bool
         True if heat strain is caused by skin wettedness (w) reaching its maximum value
     heat_strain_sweating : bool
         True if heat strain is caused by regulatory sweating (m_rsw) reaching its
         maximum value
     """
-    from pythermalcomfort.models import use_fans_heatwaves
-
     # If the SET function is used to calculate the cooling effect then the h_c is
     # calculated in a slightly different way
     default_kwargs = {"round": True, "max_sweating": 500, "limit_inputs": True}
     kwargs = {**default_kwargs, **kwargs}
 
     tdb = np.array(tdb)
     tr = np.array(tr)
@@ -1449,15 +1466,14 @@
         all_valid = ~(np.isnan(tdb_valid) | np.isnan(diff_valid) | np.isnan(v_valid))
         utci_approx = np.where(all_valid, utci_approx, np.nan)
 
     if units.lower() == "ip":
         utci_approx = units_converter(tmp=utci_approx, from_units="si")[0]
 
     if return_stress_category:
-
         stress_categories = {
             -40.0: "extreme cold stress",
             -27.0: "very strong cold stress",
             -13.0: "strong cold stress",
             0.0: "moderate cold stress",
             9.0: "slight cold stress",
             26.0: "no thermal stress",
@@ -1625,15 +1641,15 @@
         relative humidity, [%]
     met : float
         metabolic rate, [met]
     clo : float
         clothing insulation, [clo]
 
         Note: The activity as well as the air speed modify the insulation characteristics
-        of the clothing and the adjacent air layer. Consequently the ISO 7730 states that
+        of the clothing and the adjacent air layer. Consequently, the ISO 7730 states that
         the clothing insulation shall be corrected [2]_. The ASHRAE 55 Standard corrects
         for the effect of the body movement for met equal or higher than 1.2 met using
         the equation clo = Icl × (0.6 + 0.4/met) The dynamic clothing insulation, clo,
         can be calculated using the function
         :py:meth:`pythermalcomfort.utilities.clo_dynamic`.
     v_ankle : float
         air speed at the 0.1 m (4 in.) above the floor, default in [m/s] in [fps] if
@@ -1915,15 +1931,15 @@
     t_sk : float, default 34.1
         mean skin temperature when worker starts working, [°C]
     t_cr : float, default 36.8
         mean core temperature when worker starts working, [°C]
     t_re : float, default False
         mean rectal temperature when worker starts working, [°C]
     t_cr_eq : float, default False
-        mean core temperature as a funtion of met when worker starts working, [°C]
+        mean core temperature as a function of met when worker starts working, [°C]
     sweat_rate : float, default 0
 
     Returns
     -------
     t_re : float
         rectal temperature, [°C]
     d_lim_loss_50 : float
@@ -3189,15 +3205,15 @@
         :py:meth:`pythermalcomfort.utilities.running_mean_outdoor_temperature`.
 
     Returns
     -------
     athb_pmv : float or array-like
         Predicted Mean Vote calculated with the Adaptive Thermal Heat Balance framework
 
-        Examples
+    Examples
     --------
     .. code-block:: python
 
         >>> from pythermalcomfort.models import athb
         >>> print(athb( tdb=[25, 27], tr=25, vr=0.1, rh=50, met=1.1, t_running_mean=20))
         [0.2, 0.209]
     """
@@ -3256,15 +3272,15 @@
 #     z = np.polyfit(rh_array, t_lim, 4)
 #     p = np.poly1d(z)
 #     y_new = p(rh_array)
 #     # plt.plot(rh_array, t_lim, "o")
 #     plt.plot(rh_array, y_new, "-", label=person)
 # ax.set(
 #     ylabel="Temperature [°C]",
-#     xlabel="Relative Humidity [RH]",
+#     xlabel="Relative Humidity [Rh]",
 #     ylim=(24, 52),
 #     xlim=(5, 70),
 # )
 # plt.legend()
 
 
 # include also the following models:
@@ -3272,7 +3288,1538 @@
 #  draft
 #  floor_surface_tmp
 #  Perceived temperature (Blazejczyk2012)
 #  Physiological subjective temperature and physiological strain (Blazejczyk2012)
 #  more models here: https://www.rdocumentation.org/packages/comf/versions/0.1.9
 #  more models here: https://rdrr.io/cran/comf/man/
 #  to print the R source code use comf::pmv
+
+
+class JOS3:
+    """JOS-3 model simulates human thermal physiology including skin
+    temperature, core temperature, sweating rate, etc. for the whole body and
+    17 local body parts.
+
+    This model was developed at Shin-ichi Tanabe Laboratory, Waseda University
+    and was derived from 65 Multi-Node model (https://doi.org/10.1016/S0378-7788(02)00014-2)
+    and JOS-2 model (https://doi.org/10.1016/j.buildenv.2013.04.013).
+
+    To use this model, create an instance of the JOS3 class with optional body parameters
+    such as body height, weight, age, sex, etc.
+
+    Environmental conditions such as air temperature, mean radiant temperature, air velocity, etc.
+    can be set using the setter methods. (ex. X.tdb, X.tr X.v)
+    If you want to set the different conditons in each body part, set them
+    as a 17 lengths of list, dictionaly, or numpy array format.
+
+    List or numpy array format input must be 17 lengths and means the order of "head", "neck", "chest",
+    "back", "pelvis", "left_shoulder", "left_arm", "left_hand", "right_shoulder", "right_arm",
+    "right_hand", "left_thigh", "left_leg", "left_foot", "right_thigh", "right_leg" and "right_foot".
+
+    The model output includes local and mean skin temperature, local core temperature,
+    local and mean skin wettedness, and heat loss from the skin etc. which can be accessed using getter methods.
+    (ex. X.t_skin, X.t_skin_mean, X.t_core)
+
+    If you use this package, please cite us as follows and mention the version of pythermalcomfort used:
+    Y. Takahashi, A. Nomoto, S. Yoda, R. Hisayama, M. Ogata, Y. Ozeki, S. Tanabe,
+    Thermoregulation Model JOS-3 with New Open Source Code, Energy & Buildings (2020),
+    doi: https://doi.org/10.1016/j.enbuild.2020.110575
+
+    Note: To maintain consistency in variable names for pythermalcomfort,
+    some variable names differ from those used in the original paper.
+
+    Parameters
+    ----------
+    height : float, optional
+        body height, in [m]. The default is 1.72.
+    weight : float, optional
+        body weight, in [kg]. The default is 74.43.
+    fat : float, optional
+        fat percentage, in [%]. The default is 15.
+    age : int, optional
+        age, in [years]. The default is 20.
+    sex : str, optional
+        sex ("male" or "female"). The default is "male".
+    ci : float, optional
+        Cardiac index, in [L/min/m2]. The default is 2.6432.
+    bmr_equation : str, optional
+        The equation used to calculate basal metabolic rate (BMR). Choose a BMR equation.
+        The default is "harris-benedict" equation created uding Caucasian's data. (https://doi.org/10.1073/pnas.4.12.370)
+        If the Ganpule's equation (https://doi.org/10.1038/sj.ejcn.1602645) for Japanese people is used, input "japanese".
+    bsa_equation : str, optional
+        The equation used to calculate body surface area (bsa). Choose a bsa equation.
+        You can choose "dubois", "fujimoto", "kruazumi", or "takahira". The default is "dubois".
+        The body surface area can be calculated using the function
+        :py:meth:`pythermalcomfort.utilities.body_surface_area`.
+    ex_output : None, list or "all", optional
+        This is used when you want to display results other than the default output parameters (ex.skin temperature);
+        by default, JOS outputs only the most necessary parameters in order to reduce the computational load.
+        If the parameters other than the default output parameters are needed,
+        specify the list of the desired parameter names in string format like ["bf_skin", "bf_core", "t_artery"].
+        If you want to display all output results, set ex_output is "all".
+
+    Setter & Getter
+    ---------------
+    tdb : float or array-like
+        dry bulb air temperature [°C].
+    tr : float or list-like
+        Mean radiant temperature [°C].
+    to : float or list-like
+        Operative temperature [°C].
+    v : float or list-like
+        Air speed [m/s].
+    rh : float or list-like
+        Relative humidity [%].
+    clo : float or list-like
+        Clothing insulation [clo].
+        Note: If you want to input clothing insulation to each body part,
+        it can be input using the dictionaly in utilities.py.
+        :py:meth:`pythermalcomfort.utilities.local_clo_typical_ensembles`.
+    par : float
+        Physical activity ratio [-].
+        This equals the ratio of metaboric rate to basal metablic rate.
+        The par of sitting quietly is 1.2.
+    posture : str
+        Choose a posture from standing, sitting or lying.
+    bodytemp : numpy.ndarray (85,)
+        All segment temperatures of JOS-3
+
+    Getter
+    -------
+    bsa : numpy.ndarray (17,)
+        Body surface areas by local body segments [m2].
+    Rt : numpy.ndarray (17,)
+        Dry heat resistances between the skin and ambience areas by local body segments [K.m2/W].
+    Ret : numpy.ndarray (17,)
+        Wet (Evaporative) heat resistances between the skin and ambience areas by local body segments [Pa.m2/W].
+    w : numpy.ndarray (17,)
+        Skin wettedness on local body segments [-].
+    w_mean : float
+        Mean skin wettedness of the whole body [-].
+    t_skin_mean : float
+        Mean skin temperature of the whole body [°C].
+    t_skin : numpy.ndarray (17,)
+        Skin temperatures by the local body segments [°C].
+    t_core : numpy.ndarray (17,)
+        Skin temperatures by the local body segments [°C].
+    t_cb : numpy.ndarray (1,)
+        Core temperatures by the local body segments [°C].
+    t_artery : numpy.ndarray (17,)
+        Arterial temperatures by the local body segments [°C].
+    t_vein : numpy.ndarray (17,)
+        Vein temperatures by the local body segments [°C].
+    t_superficial_vein : numpy.ndarray (12,)
+        Superfical vein temperatures by the local body segments [°C].
+    t_muscle : numpy.ndarray (2,)
+        Muscle temperatures of head and pelvis [°C].
+    t_fat : numpy.ndarray (2,)
+        fat temperatures of head and pelvis  [°C].
+    BMR : float
+        Basal metabolic rate [W/m2].
+    body_names : list (17)
+        JOS3 body names [-].
+        "head", "neck", "chest", "back", "pelvis",
+        "left_shoulder", "left_arm", "left_hand", "right_shoulder", "right_arm", "right_hand",
+        "left_thigh", "left_leg", "left_hand", "right_thigh", "right_leg" and "right_hand".
+    results : dict
+        output as dictionaly format
+
+    Methods
+    -------
+    _reset_setpt():
+        Reset set-point temperature under steady state calculation.
+    simulate(times, dtime, output):
+        Run JOS-3 model for given times.
+    _run(dtime, passive=False, output=True):
+        Run JOS-3 model once and gets the model parameters.
+    dict_results():
+        Get results as a dictionary with pandas.DataFrame values.
+    to_csv(path=None, folder=None, unit=True, meaning=True):
+        Export results as csv format.
+    _set_ex_q(tissue, value):
+        Set extra heat gain by tissue name.
+
+    Returns (default)
+    -----------------
+    output_params : dict
+        A dictionary including the following output parameters:
+        Q_total : total heat production of the whole body [W]
+        cardiac_output: cardiac output (the sum of the whole blood flow) [L/h]
+        cycle_time: the counts of executing one cycle calculation [-]
+        dt      : time step [sec]
+        pythermalcomfort_version: version of pythermalcomfort [-]
+        q_res   : heat loss by respiration [W]
+        q_skin  : total heat loss from the skin (each body part) [W]
+        simulation_time: simulation times [sec]
+        t_core  : core temperature (each body part) [°C]
+        t_skin  : skin temperature (each body part) [°C]
+        t_skin_mean: mean skin temperature [°C]
+        w       : skin wettedness (each body part) [-]
+        w_mean  : mean skin wettedness [-]
+        weight_loss_by_evap_and_res: weight loss by the evaporation and respiration of the whole body [g/sec]
+
+    Returns (optional)
+    ------------------
+    output_params : dict
+        A dictionary including the following parameters:
+        Q_bmr_core: core heat production by basal metabolism (each body part) [W]
+        Q_bmr_muscle: muscle heat production by basal metabolism (each body part) [W]
+        Q_bmr_skin: skin heat production by basal metabolism (each body part) [W]
+        Q_core  : core total heat production (each body part) [W]
+        Q_fat   : fat total heat production (each body part) [W]
+        Q_muscle: muscle total heat production (each body part) [W]
+        Q_nst   : core heat production by non-shivering thermogenesis (each body part) [W]
+        Q_shiv  : core or muscle heat production by shivering thermogenesis (each body part) [W]
+        Q_skin  : skin total heat production (each body part) [W]
+        Q_work  : core or muscle heat production by work (each body part) [W]
+        Ret     : total clothing evaporative heat resistance (each body part) [m2.kPa/W]
+        Rt      : total clothing heat resistance (each body part) [m2.K/W]
+        age     : age [years]
+        bf_ava_foot: AVA blood flow rate of one foot [L/h]
+        bf_ava_hand: AVA blood flow rate of one hand [L/h]
+        bf_core : core blood flow rate (each body part) [L/h]
+        bf_fat  : fat blood flow rate (each body part) [L/h]
+        bf_muscle: muscle blood flow rate (each body part) [L/h]
+        bf_skin : skin blood flow rate (each body part) [L/h]
+        bsa     : body surface area (each body part) [m2]
+        clo     : clothing insulation (each body part) [clo]
+        e_max   : maximum evaporative heat loss from the skin (each body part) [W]
+        e_skin  : evaporative heat loss from the skin (each body part) [W]
+        e_sweat : evaporative heat loss from the skin by only sweating (each body part) [W]
+        fat     : body fat rate [%]
+        height  : body height [m]
+        met_base_fat: fat heat production by basal metabolism (each body part) [W]
+        name    : name of the model [-]
+        par     : physical activity ratio [-]
+        q_res_latent: latent heat loss by respiration (each body part) [W]
+        q_res_sensible: sensible heat loss by respiration (each body part) [W]
+        q_skin_latent: latent heat loss from the skin (each body part) [W]
+        q_skin_sensible: sensible heat loss from the skin (each body part) [W]
+        rh      : relative humidity (each body part) [%]
+        sex     : sex [-]
+        t_artery: arterial temperature (each body part) [°C]
+        t_cb    : central blood temperature [°C]
+        t_core_set: skin set point temperature (each body part) [°C]
+        t_fat   : fat temperature (each body part) [°C]
+        t_muscle: muscle temperature (each body part) [°C]
+        t_skin_set: core set point temperature (each body part) [°C]
+        t_superficial_vein: superficial vein temperature (each body part) [°C]
+        t_vein  : vein temperature (each body part) [°C]
+        tdb     : dry bulb air temperature (each body part) [°C]
+        to      : operative temperature (each body part) [°C]
+        tr      : mean radiant temperature (each body part) [°C]
+        v       : air velocity (each body part) [m/s]
+        weight  : body weight [kg]
+
+
+    Examples
+    --------
+    # Build a model and set a body built
+    # Create an instance of the JOS3 class with optional body parameters such as body height, weight, age, sex, etc.
+
+    .. code-block:: python
+
+        >>> import numpy as np
+        >>> import pandas as pd
+        >>> import matplotlib.pyplot as plt
+        >>> import os
+        >>> from pythermalcomfort.models import JOS3
+        >>> from pythermalcomfort.jos3_functions.utilities import local_clo_typical_ensembles
+        >>>
+        >>> directory_name = "jos3_output_example"
+        >>> current_directory = os.getcwd()
+        >>> jos3_example_directory = os.path.join(current_directory, directory_name)
+        >>> if not os.path.exists(jos3_example_directory):
+        >>>     os.makedirs(jos3_example_directory)
+        >>>
+        >>> model = JOS3(
+        >>>     height=1.7,
+        >>>     weight=60,
+        >>>     fat=20,
+        >>>     age=30,
+        >>>     sex="male",
+        >>>     bmr_equation="japanese",
+        >>>     bsa_equation="fujimoto",
+        >>>     ex_output="all",
+        >>> )
+        >>> # Set environmental conditions such as air temperature, mean radiant temperature using the setter methods.
+        >>> # Set the first condition
+        >>> # Environmental parameters can be input as int, float, list, dict, numpy array format.
+        >>> model.tdb = 28  # Air temperature [°C]
+        >>> model.tr = 30  # Mean radiant temperature [°C]
+        >>> model.rh = 40  # Relative humidity [%]
+        >>> model.v = np.array( # Air velocity [m/s]
+        >>>     [
+        >>>         0.2,  # head
+        >>>         0.4,  # neck
+        >>>         0.4,  # chest
+        >>>         0.1,  # back
+        >>>         0.1,  # pelvis
+        >>>         0.4,  # left shoulder
+        >>>         0.4,  # left arm
+        >>>         0.4,  # left hand
+        >>>         0.4,  # right shoulder
+        >>>         0.4,  # right arm
+        >>>         0.4,  # right hand
+        >>>         0.1,  # left thigh
+        >>>         0.1,  # left leg
+        >>>         0.1,  # left foot
+        >>>         0.1,  # right thigh
+        >>>         0.1,  # right leg
+        >>>         0.1,  # right foot
+        >>>     ]
+        >>> )
+        >>> model.clo = local_clo_typical_ensembles["briefs, socks, undershirt, work jacket, work pants, safety shoes"]["local_body_part"]
+        >>> # par should be input as int, float.
+        >>> model.par = 1.2  # Physical activity ratio [-], assuming a sitting position
+        >>> # posture should be input as int (0, 1, or 2) or str ("standing", "sitting" or "lying").
+        >>> # (0="standing", 1="sitting" or 2="lying")
+        >>> model.posture = "sitting"  # Posture [-], assuming a sitting position
+        >>>
+        >>> # Run JOS-3 model
+        >>> model.simulate(
+        >>>     times=30,  # Number of loops of a simulation
+        >>>     dtime=60,  # Time delta [sec]. The default is 60.
+        >>> )  # Exposure time = 30 [loops] * 60 [sec] = 30 [min]
+        >>> # Set the next condition (You only need to change the parameters that you want to change)
+        >>> model.to = 20  # Change operative temperature
+        >>> model.v = { # Air velocity [m/s], assuming to use a desk fan
+        >>>     'head' : 0.2,
+        >>>     'neck' : 0.4,
+        >>>     'chest' : 0.4,
+        >>>     'back': 0.1,
+        >>>     'pelvis' : 0.1,
+        >>>     'left_shoulder' : 0.4,
+        >>>     'left_arm' : 0.4,
+        >>>     'left_hand' : 0.4,
+        >>>     'right_shoulder' : 0.4,
+        >>>     'right_arm' : 0.4,
+        >>>     'right_hand' : 0.4,
+        >>>     'left_thigh' : 0.1,
+        >>>     'left_leg' : 0.1,
+        >>>     'left_foot' : 0.1,
+        >>>     'right_thigh' : 0.1,
+        >>>     'right_leg' : 0.1,
+        >>>     'right_foot' : 0.1
+        >>>     }
+        >>> # Run JOS-3 model
+        >>> model.simulate(
+        >>>     times=60,  # Number of loops of a simulation
+        >>>     dtime=60,  # Time delta [sec]. The default is 60.
+        >>> )  # Additional exposure time = 60 [loops] * 60 [sec] = 60 [min]
+        >>> # Set the next condition (You only need to change the parameters that you want to change)
+        >>> model.tdb = 30  # Change air temperature [°C]
+        >>> model.tr = 35  # Change mean radiant temperature [°C]
+        >>> # Run JOS-3 model
+        >>> model.simulate(
+        >>>     times=30,  # Number of loops of a simulation
+        >>>     dtime=60,  # Time delta [sec]. The default is 60.
+        >>> )  # Additional exposure time = 30 [loops] * 60 [sec] = 30 [min]
+        >>> # Show the results
+        >>> df = pd.DataFrame(model.dict_results())  # Make pandas.DataFrame
+        >>> df[["t_skin_mean", "t_skin_head", "t_skin_chest", "t_skin_left_hand"]].plot()  # Plot time series of local skin temperature.
+        >>> plt.legend(["Mean", "Head", "Chest", "Left hand"])  # Reset the legends
+        >>> plt.ylabel("Skin temperature [°C]")  # Set y-label as 'Skin temperature [°C]'
+        >>> plt.xlabel("Time [min]")  # Set x-label as 'Time [min]'
+        >>> plt.savefig(os.path.join(jos3_example_directory, "jos3_example2_skin_temperatures.png"))  # Save plot at the current directory
+        >>> plt.show()  # Show the plot
+        >>> # Exporting the results as csv
+        >>> model.to_csv(os.path.join(jos3_example_directory, "jos3_example2 (all output).csv"))
+    """
+
+    def __init__(
+        self,
+        height=1.72,
+        weight=74.43,
+        fat=15,
+        age=20,
+        sex="male",
+        ci=2.59,
+        bmr_equation="harris-benedict",
+        bsa_equation="dubois",
+        ex_output=None,
+    ):
+        """Initialize a new instance of JOS3 class, which is designed to model
+        and simulate various physiological parameters related to human
+        thermoregulation. This class uses mathematical models to calculate and
+        predict body temperature, basal metabolic rate, body surface area, and
+        other related parameters.
+
+        Parameters
+        ----------
+        height float, optional
+            Body height, in [m].
+            The default is 1.72.
+        weight : float, optional
+            Body weight, in [kg]. The default is 74.43.
+        fat : float, optional
+            fat percentage, in [%]. The default is 15.
+        age : int, optional
+            age, in [years]. The default is 20.
+        sex : str, optional
+            sex ("male" or "female"). The default is "male".
+        ci : float, optional
+            Cardiac index, in [L/min/m2]. The default is 2.6432.
+        bmr_equation : str, optional
+            The equation used to calculate basal metabolic rate (BMR). Choose a BMR equation.
+            The default is "harris-benedict" equation created uding Caucasian's data. (https://doi.org/10.1073/pnas.4.12.370)
+            If the Ganpule's equation (https://doi.org/10.1038/sj.ejcn.1602645) for Japanese people is used, input "japanese".
+        bsa_equation : str, optional
+            The equation used to calculate body surface area (bsa). Choose a bsa equation.
+            You can choose "dubois", "fujimoto", "kruazumi", or "takahira". The default is "dubois".
+        ex_output : None, list or "all", optional
+            This is used when you want to display results other than the default output parameters (ex.skin temperature);
+            by default, JOS outputs only the most necessary parameters in order to reduce the computational load.
+            If the parameters other than the default output parameters are needed,
+            specify the list of the desired parameter names in string format like ["bf_skin", "bf_core", "t_artery"].
+            If you want to display all output results, set ex_output is "all".
+
+        Returns
+        -------
+        None.
+        """
+
+        # Version of pythermalcomfort
+        version_string = (
+            __version__  # get the current version of pythermalcomfort package
+        )
+        version_number_string = re.findall("\d+\.\d+\.\d+", version_string)[0]
+        self._version = version_number_string  # (ex. 'X.Y.Z')
+
+        # Initialize basic attributes
+        self._height = height
+        self._weight = weight
+        self._fat = fat
+        self._sex = sex
+        self._age = age
+        self._ci = ci
+        self._bmr_equation = bmr_equation
+        self._bsa_equation = bsa_equation
+        self._ex_output = ex_output
+
+        # Calculate body surface area (bsa) rate
+        self._bsa_rate = cons.bsa_rate(height, weight, bsa_equation)
+
+        # Calculate local body surface area
+        self._bsa = cons.local_bsa(height, weight, bsa_equation)
+
+        # Calculate basal blood flow (BFB) rate [-]
+        self._bfb_rate = cons.bfb_rate(height, weight, bsa_equation, age, ci)
+
+        # Calculate thermal conductance (CDT) [W/K]
+        self._cdt = cons.conductance(height, weight, bsa_equation, fat)
+
+        # Calculate thermal capacity [J/K]
+        self._cap = cons.capacity(height, weight, bsa_equation, age, ci)
+
+        # Set initial core and skin temperature set points [°C]
+        self.setpt_cr = np.ones(17) * 37  # core
+        self.setpt_sk = np.ones(17) * 34  # skin
+
+        # Initialize body temperature [°C]
+        self._bodytemp = np.ones(NUM_NODES) * 36
+
+        # Initialize environmental conditions and other factors
+        # (Default values of input conditions)
+        self._ta = np.ones(17) * 28.8  # Air temperature [°C]
+        self._tr = np.ones(17) * 28.8  # Radiant temperature [°C]
+        self._rh = np.ones(17) * 50  # Relative humidity [%]
+        self._va = np.ones(17) * 0.1  # Air velocity [m/s]
+        self._clo = np.zeros(17)  # Clothing insulation
+        self._iclo = np.ones(17) * 0.45  # Clothing vapor permeation efficiency [-]
+        self._par = 1.25  # Physical activity ratio [-]
+        self._posture = "standing"  # Body posture [-]
+        self._hc = None  # Convective heat transfer coefficient
+        self._hr = None  # Radiative heat transfer coefficient
+        self.ex_q = np.zeros(NUM_NODES)  # External heat production
+        self._t = dt.timedelta(0)  # Elapsed time
+        self._cycle = 0  # Cycle time
+        self.model_name = "JOS3"  # Model name
+        self.options = {
+            "nonshivering_thermogenesis": True,
+            "cold_acclimated": False,
+            "shivering_threshold": False,
+            "limit_dshiv/dt": False,
+            "bat_positive": False,
+            "ava_zero": False,
+            "shivering": False,
+        }
+
+        # Set shivering threshold = 0
+        threg.PRE_SHIV = 0
+
+        # Initialize history to store model parameters
+        self._history = []
+
+        # Set elapsed time and cycle time to 0
+        self._t = dt.timedelta(0)  # Elapsed time
+        self._cycle = 0  # Cycle time
+
+        # Reset set-point temperature and save the last model parameters
+        dictout = self._reset_setpt()
+        self._history.append(dictout)
+
+    def _calculate_operative_temp_when_pmv_is_zero(self, va=0.1, rh=50, met=1, clo=0):
+        """
+        Calculate operative temperature [°C] when PMV=0.
+        Parameters
+        ----------
+        va : float, optional
+            Air velocity [m/s]. The default is 0.1.
+        rh : float, optional
+            Relative humidity [%]. The default is 50.
+        met : float, optional
+            Metabolic rate [met]. The default is 1.
+        clo : float, optional
+            Clothing insulation [clo]. The default is 0.
+        Returns
+        -------
+        to : float
+            Operative temperature [°C].
+        """
+
+        to = 28  # initial operative temperature
+        # Iterate until the PMV (Predicted Mean Vote) value is less than 0.001
+        for _ in range(100):
+            vpmv = pmv(tdb=to, tr=to, vr=va, rh=rh, met=met, clo=clo)
+            # Break the loop if the absolute value of PMV is less than 0.001
+            if abs(vpmv) < 0.001:
+                break
+            # Update the temperature based on the PMV value
+            else:
+                to = to - vpmv / 3
+        return to
+
+    def _reset_setpt(self):
+        """Reset set-point temperature under steady state calculation. Be
+        careful, input parameters (tdb, tr, rh, v, clo, par) and body
+        temperatures are also reset.
+
+        Returns
+        -------
+        dict
+            Parameters of JOS-3 model.
+        """
+        # Set operative temperature under PMV=0 environment
+        # par = 1.25
+        # 1 met = 58.15 W/m2
+        met = self.bmr * 1.25 / 58.15  # [met]
+        self.to = self._calculate_operative_temp_when_pmv_is_zero(met=met)
+        self.rh = 50  # Relative humidity
+        self.v = 0.1  # Air velocity
+        self.clo = 0  # Clothing insulation
+        self.par = 1.25  # Physical activity ratio
+
+        # Steady-calculation
+        self.options["ava_zero"] = True
+        for _ in range(10):
+            dict_out = self._run(dtime=60000, passive=True)
+
+        # Set new set-point temperatures for core and skin
+        self.setpt_cr = self.t_core
+        self.setpt_sk = self.t_skin
+        self.options["ava_zero"] = False
+
+        return dict_out
+
+    def simulate(self, times, dtime=60, output=True):
+        """Run JOS-3 model.
+
+        Parameters
+        ----------
+        times : int
+            Number of loops of a simulation.
+        dtime : int or float, optional
+            Time delta in seconds. The default is 60.
+        output : bool, optional
+            If you don't want to record parameters, set False. The default is True.
+
+        Returns
+        -------
+        None.
+        """
+        # Loop through the simulation for the given number of times
+        for _ in range(times):
+            # Increment the elapsed time by the time delta
+            self._t += dt.timedelta(0, dtime)
+
+            # Increment the cycle counter
+            self._cycle += 1
+
+            # Execute the simulation step
+            dict_data = self._run(dtime=dtime, output=output)
+
+            # If output is True, append the results to the history
+            if output:
+                self._history.append(dict_data)
+
+    def _run(self, dtime=60, passive=False, output=True):
+        """Runs the model once and gets the model parameters.
+
+        The function then calculates several thermoregulation parameters using the input data,
+        such as convective and radiative heat transfer coefficients, operative temperature, heat resistance,
+        and blood flow rates.
+
+        It also calculates the thermogenesis by shivering and non-shivering, basal thermogenesis, and thermogenesis by work.
+
+        The function then calculates the total heat loss and gains, including respiratory,
+        sweating, and extra heat gain, and builds the matrices required
+        to solve for the new body temperature.
+
+        It then calculates the new body temperature by solving the matrices using numpy's linalg library.
+
+        Finally, the function returns a dictionary of the simulation results.
+        The output parameters include cycle time, model time, t_skin_mean, t_skin, t_core, w_mean, w, weight_loss_by_evap_and_res, cardiac_output, Q_total, q_res, and q_skin.
+
+        Additionally, if the _ex_output variable is set to "all" or is a list of keys,
+        the function also returns a detailed dictionary of all the thermoregulation parameters
+        and other variables used in the simulation.
+
+        Parameters
+        ----------
+        dtime : int or float, optional
+            Time delta [sec]. Default is 60.
+        passive : bool, optional
+            If you run a passive model, set to True. Default is False.
+        output : bool, optional
+            If you don't need parameters, set to False. Default is True.
+
+        Returns
+        -------
+        dict_out : dictionary
+            Output parameters.
+        """
+
+        # Compute convective and radiative heat transfer coefficient [W/(m2*K)]
+        # based on posture, air velocity, air temperature, and skin temperature.
+        # Manual setting is possible by setting self._hc and self._hr.
+        # Compute heat and evaporative heat resistance [m2.K/W], [m2.kPa/W]
+
+        # Get core and skin temperatures
+        tcr = self.t_core
+        tsk = self.t_skin
+
+        # Convective and radiative heat transfer coefficients [W/(m2*K)]
+        hc = threg.fixed_hc(
+            threg.conv_coef(
+                self._posture,
+                self._va,
+                self._ta,
+                tsk,
+            ),
+            self._va,
+        )
+        hr = threg.fixed_hr(
+            threg.rad_coef(
+                self._posture,
+            )
+        )
+
+        # Manually set convective and radiative heat transfer coefficients if necessary
+        if self._hc is not None:
+            hc = self._hc
+        if self._hr is not None:
+            hr = self._hr
+
+        # Compute operative temp. [°C], clothing heat and evaporative resistance [m2.K/W], [m2.kPa/W]
+        # Operative temp. [°C]
+        to = threg.operative_temp(
+            self._ta,
+            self._tr,
+            hc,
+            hr,
+        )
+        # Clothing heat resistance [m2.K/W]
+        r_t = threg.dry_r(hc, hr, self._clo)
+        # Clothing evaporative resistance [m2.kPa/W]
+        r_et = threg.wet_r(hc, self._clo, self._iclo)
+
+        # ------------------------------------------------------------------
+        # Thermoregulation
+        # 1) Sweating
+        # 2) Vasoconstriction, Vasodilation
+        # 3) Shivering and non-shivering thermogenesis
+        # ------------------------------------------------------------------
+
+        # Compute the difference between the set-point temperature and body temperatures
+        # and other thermoregulation parameters.
+        # If running a passive model, the set-point temperature of thermoregulation is
+        # set to the current body temperature.
+
+        # set-point temperature for thermoregulation
+        if passive:
+            setpt_cr = tcr.copy()
+            setpt_sk = tsk.copy()
+        else:
+            setpt_cr = self.setpt_cr.copy()
+            setpt_sk = self.setpt_sk.copy()
+
+        # Error signal = Difference between set-point and body temperatures
+        err_cr = tcr - setpt_cr
+        err_sk = tsk - setpt_sk
+
+        # SWEATING THERMOREGULATION
+        # Skin wettedness [-], e_skin, e_max, e_sweat [W]
+        # Calculate skin wettedness, sweating heat loss, maximum sweating rate, and total sweat rate
+        wet, e_sk, e_max, e_sweat = threg.evaporation(
+            err_cr,
+            err_sk,
+            tsk,
+            self._ta,
+            self._rh,
+            r_et,
+            self._height,
+            self._weight,
+            self._bsa_equation,
+            self._age,
+        )
+
+        # VASOCONSTRICTION, VASODILATION
+        # Calculate skin blood flow and basal skin blood flow [L/h]
+        bf_skin = threg.skin_blood_flow(
+            err_cr,
+            err_sk,
+            self._height,
+            self._weight,
+            self._bsa_equation,
+            self._age,
+            self._ci,
+        )
+
+        # Calculate hands and feet's AVA blood flow [L/h]
+        bf_ava_hand, bf_ava_foot = threg.ava_blood_flow(
+            err_cr,
+            err_sk,
+            self._height,
+            self._weight,
+            self._bsa_equation,
+            self._age,
+            self._ci,
+        )
+        if self.options["ava_zero"] and passive:
+            bf_ava_hand = 0
+            bf_ava_foot = 0
+
+        # SHIVERING AND NON-SHIVERING
+        # Calculate shivering thermogenesis [W]
+        q_shiv = threg.shivering(
+            err_cr,
+            err_sk,
+            tcr,
+            tsk,
+            self._height,
+            self._weight,
+            self._bsa_equation,
+            self._age,
+            self._sex,
+            dtime,
+            self.options,
+        )
+
+        # Calculate non-shivering thermogenesis (NST) [W]
+        if self.options["nonshivering_thermogenesis"]:
+            q_nst = threg.nonshivering(
+                err_sk,
+                self._height,
+                self._weight,
+                self._bsa_equation,
+                self._age,
+                self.options["cold_acclimated"],
+                self.options["bat_positive"],
+            )
+        else:  # not consider NST
+            q_nst = np.zeros(17)
+
+        # ------------------------------------------------------------------
+        # Thermogenesis
+        # ------------------------------------------------------------------
+
+        # Calculate local basal metabolic rate (BMR) [W]
+        m_base = threg.local_mbase(
+            self._height,
+            self._weight,
+            self._age,
+            self._sex,
+            self._bmr_equation,
+        )
+        # Calculate overall basal metabolic rate (BMR) [W]
+        m_base_all = sum([m.sum() for m in m_base])
+
+        # Calculate thermogenesis by work [W]
+        q_work = threg.local_q_work(m_base_all, self._par)
+
+        # Calculate the sum of thermogenesis in core, muscle, fat, skin [W]
+        q_core, q_muscle, q_fat, q_skin = threg.sum_m(
+            m_base,
+            q_work,
+            q_shiv,
+            q_nst,
+        )
+        qall = q_core.sum() + q_muscle.sum() + q_fat.sum() + q_skin.sum()
+
+        # ------------------------------------------------------------------
+        # Others
+        # ------------------------------------------------------------------
+        # Calculate blood flow in core, muscle, fat [L/h]
+        bf_core, bf_muscle, bf_fat = threg.cr_ms_fat_blood_flow(
+            q_work,
+            q_shiv,
+            self._height,
+            self._weight,
+            self._bsa_equation,
+            self._age,
+            self._ci,
+        )
+
+        # Calculate heat loss by respiratory
+        p_a = threg.antoine(self._ta) * self._rh / 100
+        res_sh, res_lh = threg.resp_heat_loss(self._ta[0], p_a[0], qall)
+
+        # Calculate sensible heat loss [W]
+        shlsk = (tsk - to) / r_t * self._bsa
+
+        # Calculate cardiac output [L/h]
+        co = threg.sum_bf(bf_core, bf_muscle, bf_fat, bf_skin, bf_ava_hand, bf_ava_foot)
+
+        # Calculate weight loss rate by evaporation [g/sec]
+        wlesk = (e_sweat + 0.06 * e_max) / 2418
+        wleres = res_lh / 2418
+
+        # ------------------------------------------------------------------
+        # Matrix
+        # This code section is focused on constructing and calculating
+        # various matrices required for modeling the thermoregulation
+        # of the human body.
+        # Since JOS-3 has 85 thermal nodes, the determinant of 85*85 is to be solved.
+        # ------------------------------------------------------------------
+
+        # Matrix A = Matrix for heat exchange due to blood flow and conduction occurring between tissues
+        # (85, 85,) ndarray
+
+        # Calculates the blood flow in arteries and veins for core, muscle, fat, skin,
+        # and arteriovenous anastomoses (AVA) in hands and feet,
+        # and combines them into two arrays:
+        # 1) bf_local for the local blood flow and 2) bf_whole for the whole-body blood flow.
+        # These arrays are then combined to form arr_bf.
+        bf_art, bf_vein = matrix.vessel_blood_flow(
+            bf_core, bf_muscle, bf_fat, bf_skin, bf_ava_hand, bf_ava_foot
+        )
+        bf_local = matrix.local_arr(
+            bf_core, bf_muscle, bf_fat, bf_skin, bf_ava_hand, bf_ava_foot
+        )
+        bf_whole = matrix.whole_body(bf_art, bf_vein, bf_ava_hand, bf_ava_foot)
+        arr_bf = np.zeros((NUM_NODES, NUM_NODES))
+        arr_bf += bf_local
+        arr_bf += bf_whole
+
+        # Adjusts the units of arr_bf from [W/K] to [/sec] and then to [-]
+        # by dividing by the heat capacity self._cap and multiplying by the time step dtime.
+        arr_bf /= self._cap.reshape((NUM_NODES, 1))  # Change unit [W/K] to [/sec]
+        arr_bf *= dtime  # Change unit [/sec] to [-]
+
+        # Performs similar unit conversions for the convective heat transfer coefficient array arr_cdt
+        # (also divided by self._cap and multiplied by dtime).
+        arr_cdt = self._cdt.copy()
+        arr_cdt /= self._cap.reshape((NUM_NODES, 1))  # Change unit [W/K] to [/sec]
+        arr_cdt *= dtime  # Change unit [/sec] to [-]
+
+        # Matrix B = Matrix for heat transfer between skin and environment
+        arr_b = np.zeros(NUM_NODES)
+        arr_b[INDEX["skin"]] += 1 / r_t * self._bsa
+        arr_b /= self._cap  # Change unit [W/K] to [/sec]
+        arr_b *= dtime  # Change unit [/sec] to [-]
+
+        # Calculates the off-diagonal and diagonal elements of the matrix A,
+        # which represents the heat transfer coefficients between different parts of the body,
+        # and combines them to form the full matrix A (arrA).
+        # Then, the inverse of matrix A is computed (arrA_inv).
+        arr_a_tria = -(arr_cdt + arr_bf)
+
+        arr_a_dia = arr_cdt + arr_bf
+        arr_a_dia = arr_a_dia.sum(axis=1) + arr_b
+        arr_a_dia = np.diag(arr_a_dia)
+        arr_a_dia += np.eye(NUM_NODES)
+
+        arr_a = arr_a_tria + arr_a_dia
+        arr_a_inv = np.linalg.inv(arr_a)
+
+        # Matrix Q = Matrix for heat generation rate from thermogenesis, respiratory, sweating,
+        # and extra heat gain processes in different body parts.
+
+        # Matrix Q [W] / [J/K] * [sec] = [-]
+        # Thermogensis
+        arr_q = np.zeros(NUM_NODES)
+        arr_q[INDEX["core"]] += q_core
+        arr_q[INDEX["muscle"]] += q_muscle[VINDEX["muscle"]]
+        arr_q[INDEX["fat"]] += q_fat[VINDEX["fat"]]
+        arr_q[INDEX["skin"]] += q_skin
+
+        # Respiratory [W]
+        arr_q[INDEX["core"][2]] -= res_sh + res_lh  # chest core
+
+        # Sweating [W]
+        arr_q[INDEX["skin"]] -= e_sk
+
+        # Extra heat gain [W]
+        arr_q += self.ex_q.copy()
+
+        arr_q /= self._cap  # Change unit [W]/[J/K] to [K/sec]
+        arr_q *= dtime  # Change unit [K/sec] to [K]
+
+        # Boundary batrix [℃]
+        arr_to = np.zeros(NUM_NODES)
+        arr_to[INDEX["skin"]] += to
+
+        # Combines the current body temperature, the boundary matrix, and the heat generation matrix
+        # to calculate the new body temperature distribution (arr).
+        arr = self._bodytemp + arr_b * arr_to + arr_q
+
+        # ------------------------------------------------------------------
+        # New body temp. [°C]
+        # ------------------------------------------------------------------
+        self._bodytemp = np.dot(arr_a_inv, arr)
+
+        # ------------------------------------------------------------------
+        # Output parameters
+        # ------------------------------------------------------------------
+        dict_out = {}
+        if output:  # Default output
+            dict_out["pythermalcomfort_version"] = self._version
+            dict_out["cycle_time"] = self._cycle
+            dict_out["simulation_time"] = self._t
+            dict_out["dt"] = dtime
+            dict_out["t_skin_mean"] = self.t_skin_mean
+            dict_out["t_skin"] = self.t_skin
+            dict_out["t_core"] = self.t_core
+            dict_out["w_mean"] = np.average(wet, weights=_BSAst)
+            dict_out["w"] = wet
+            dict_out["weight_loss_by_evap_and_res"] = wlesk.sum() + wleres
+            dict_out["cardiac_output"] = co
+            dict_out["Q_total"] = qall
+            dict_out["q_res"] = res_sh + res_lh
+            dict_out["q_skin"] = shlsk + e_sk
+
+        detail_out = {}
+        if self._ex_output and output:
+            detail_out["name"] = self.model_name
+            detail_out["height"] = self._height
+            detail_out["weight"] = self._weight
+            detail_out["bsa"] = self._bsa
+            detail_out["fat"] = self._fat
+            detail_out["sex"] = self._sex
+            detail_out["age"] = self._age
+            detail_out["t_core_set"] = setpt_cr
+            detail_out["t_skin_set"] = setpt_sk
+            detail_out["t_cb"] = self.t_cb
+            detail_out["t_artery"] = self.t_artery
+            detail_out["t_vein"] = self.t_vein
+            detail_out["t_superficial_vein"] = self.t_superficial_vein
+            detail_out["t_muscle"] = self.t_muscle
+            detail_out["t_fat"] = self.t_fat
+            detail_out["to"] = to
+            detail_out["Rt"] = r_t
+            detail_out["Ret"] = r_et
+            detail_out["tdb"] = self._ta.copy()
+            detail_out["tr"] = self._tr.copy()
+            detail_out["rh"] = self._rh.copy()
+            detail_out["v"] = self._va.copy()
+            detail_out["par"] = self._par
+            detail_out["clo"] = self._clo.copy()
+            detail_out["e_skin"] = e_sk
+            detail_out["e_max"] = e_max
+            detail_out["e_sweat"] = e_sweat
+            detail_out["bf_core"] = bf_core
+            detail_out["bf_muscle"] = bf_muscle[VINDEX["muscle"]]
+            detail_out["bf_fat"] = bf_fat[VINDEX["fat"]]
+            detail_out["bf_skin"] = bf_skin
+            detail_out["bf_ava_hand"] = bf_ava_hand
+            detail_out["bf_ava_foot"] = bf_ava_foot
+            detail_out["Q_bmr_core"] = m_base[0]
+            detail_out["Q_bmr_muscle"] = m_base[1][VINDEX["muscle"]]
+            detail_out["met_base_fat"] = m_base[2][VINDEX["fat"]]
+            detail_out["Q_bmr_skin"] = m_base[3]
+            detail_out["Q_work"] = q_work
+            detail_out["Q_shiv"] = q_shiv
+            detail_out["Q_nst"] = q_nst
+            detail_out["Q_core"] = q_core
+            detail_out["Q_muscle"] = q_muscle[VINDEX["muscle"]]
+            detail_out["Q_fat"] = q_fat[VINDEX["fat"]]
+            detail_out["Q_skin"] = q_skin
+            dict_out["q_skin_sensible"] = shlsk
+            dict_out["q_skin_latent"] = e_sk
+            dict_out["q_res_sensible"] = res_sh
+            dict_out["q_res_latent"] = res_lh
+
+        if self._ex_output == "all":
+            dict_out.update(detail_out)
+        elif isinstance(self._ex_output, list):  # if ex_out type is list
+            out_keys = detail_out.keys()
+            for key in self._ex_output:
+                if key in out_keys:
+                    dict_out[key] = detail_out[key]
+        return dict_out
+
+    def dict_results(self):
+        """Get results as a dictionary with pandas.DataFrame values.
+
+        Returns
+        -------
+        dict
+            A dictionary of the results, with keys as column names and values as pandas.DataFrame objects.
+        """
+        if not self._history:
+            print("The model has no data.")
+            return None
+
+        def check_word_contain(word, *args):
+            """Check if word contains *args."""
+            boolfilter = False
+            for arg in args:
+                if arg in word:
+                    boolfilter = True
+            return boolfilter
+
+        # Set column titles
+        # If the values are iter, add the body names as suffix words.
+        # If the values are not iter and the single value data, convert it to iter.
+        key2keys = {}  # Column keys
+        for key, value in self._history[0].items():
+            try:
+                length = len(value)
+                if isinstance(value, str):
+                    keys = [key]  # str is iter. Convert to list without suffix
+                elif check_word_contain(key, "sve", "sfv", "superficialvein"):
+                    keys = [key + "_" + BODY_NAMES[i] for i in VINDEX["sfvein"]]
+                elif check_word_contain(key, "ms", "muscle"):
+                    keys = [key + "_" + BODY_NAMES[i] for i in VINDEX["muscle"]]
+                elif check_word_contain(key, "fat"):
+                    keys = [key + "_" + BODY_NAMES[i] for i in VINDEX["fat"]]
+                elif length == 17:  # if data contains 17 values
+                    keys = [key + "_" + bn for bn in BODY_NAMES]
+                else:
+                    keys = [key + "_" + BODY_NAMES[i] for i in range(length)]
+            except TypeError:  # if the value is not iter.
+                keys = [key]  # convert to iter
+            key2keys.update({key: keys})
+
+        data = []
+        for i, dictout in enumerate(self._history):
+            row = {}
+            for key, value in dictout.items():
+                keys = key2keys[key]
+                if len(keys) == 1:
+                    values = [value]  # make list if value is not iter
+                else:
+                    values = value
+                row.update(dict(zip(keys, values)))
+            data.append(row)
+
+        out_dict = dict(zip(data[0].keys(), [[] for _ in range(len(data[0].keys()))]))
+        for row in data:
+            for k in data[0].keys():
+                out_dict[k].append(row[k])
+        return out_dict
+
+    def to_csv(self, path=None, folder=None, unit=True, meaning=True):
+        """Export results as csv format.
+
+        Parameters
+        ----------
+        path : str, optional
+            Output path. If you don't use the default file name, set a name.
+            The default is None.
+        folder : str, optional
+            Output folder. If you use the default file name with the current time,
+            set a only folder path.
+            The default is None.
+        unit : bool, optional
+            Write units in csv file. The default is True.
+        meaning : bool, optional
+            Write meanings of the parameters in csv file. The default is True.
+
+        Examples
+        ----------
+        >>> from pythermalcomfort.models import JOS3
+        >>> model = JOS3()
+        >>> model.simulate(60)
+        >>> model.to_csv()
+        """
+
+        # Use the model name and current time as default output file name
+        if path is None:
+            nowtime = dt.datetime.now().strftime("%Y%m%d-%H%M%S")
+            path = "{}_{}.csv".format(self.model_name, nowtime)
+            if folder:
+                os.makedirs(folder, exist_ok=True)
+                path = folder + os.sep + path
+        elif not ((path[-4:] == ".csv") or (path[-4:] == ".txt")):
+            path += ".csv"
+
+        # Get simulation results as a dictionary
+        dictout = self.dict_results()
+
+        # Get column names, units and meanings
+        columns = [k for k in dictout.keys()]
+        units = []
+        meanings = []
+        for col in columns:
+            param, body_name = remove_body_name(col)
+            if param in ALL_OUT_PARAMS:
+                u = ALL_OUT_PARAMS[param]["unit"]
+                units.append(u)
+
+                m = ALL_OUT_PARAMS[param]["meaning"]
+                if body_name:
+                    # Replace underscores with spaces
+                    body_name_with_spaces = body_name.replace("_", " ")
+                    meanings.append(m.replace("each body part", body_name_with_spaces))
+                else:
+                    meanings.append(m)
+            else:
+                units.append("")
+                meanings.append("")
+
+        # Write to csv file
+        with open(path, "wt", newline="", encoding="utf-8-sig") as f:
+            writer = csv.writer(f)
+            writer.writerow(list(columns))
+            if unit:
+                writer.writerow(units)
+            if meaning:
+                writer.writerow(meanings)
+            for i in range(len(dictout["cycle_time"])):
+                row = []
+                for k in columns:
+                    row.append(dictout[k][i])
+                writer.writerow(row)
+
+    # --------------------------------------------------------------------------
+    # Setter
+    # --------------------------------------------------------------------------
+    def _set_ex_q(self, tissue, value):
+        """Set extra heat gain by tissue name.
+
+        Parameters
+        ----------
+        tissue : str
+            Tissue name. "core", "skin", or "artery".... If you set value to
+            head muscle and other segment's core, set "all_muscle".
+        value : int, float, array
+            Heat gain [W]
+
+        Returns
+        -------
+        array
+            Extra heat gain of model.
+        """
+        self.ex_q[INDEX[tissue]] = value
+        return self.ex_q
+
+    # --------------------------------------------------------------------------
+    # Setter & getter
+    # --------------------------------------------------------------------------
+
+    @property
+    def tdb(self):
+        """
+        Getter
+        Returns
+        -------
+        tdb : numpy.ndarray (17,)
+            Air temperature [°C].
+        """
+        return self._ta
+
+    @tdb.setter
+    def tdb(self, inp):
+        self._ta = _to17array(inp)
+
+    @property
+    def tr(self):
+        """
+        Getter
+        Returns
+        -------
+        tr : numpy.ndarray (17,)
+            Mean radiant temperature [°C].
+        """
+        return self._tr
+
+    @tr.setter
+    def tr(self, inp):
+        self._tr = _to17array(inp)
+
+    @property
+    def to(self):
+        """
+        Getter
+        Returns
+        -------
+        to : numpy.ndarray (17,)
+            Operative temperature [°C].
+        """
+        hc = threg.fixed_hc(
+            threg.conv_coef(
+                self._posture,
+                self._va,
+                self._ta,
+                self.t_skin,
+            ),
+            self._va,
+        )
+        hr = threg.fixed_hr(
+            threg.rad_coef(
+                self._posture,
+            )
+        )
+        to = threg.operative_temp(
+            self._ta,
+            self._tr,
+            hc,
+            hr,
+        )
+        return to
+
+    @to.setter
+    def to(self, inp):
+        self._ta = _to17array(inp)
+        self._tr = _to17array(inp)
+
+    @property
+    def rh(self):
+        """
+        Getter
+        Returns
+        -------
+        rh : numpy.ndarray (17,)
+            Relative humidity [%].
+        """
+        return self._rh
+
+    @rh.setter
+    def rh(self, inp):
+        self._rh = _to17array(inp)
+
+    @property
+    def v(self):
+        """
+        Getter
+        Returns
+        -------
+        v : numpy.ndarray (17,)
+            Air velocity [m/s].
+        """
+        return self._va
+
+    @v.setter
+    def v(self, inp):
+        self._va = _to17array(inp)
+
+    @property
+    def posture(self):
+        """
+        Getter
+        Returns
+        -------
+        posture : str
+            Current JOS3 posture.
+        """
+        return self._posture
+
+    @posture.setter
+    def posture(self, inp):
+        if inp == 0:
+            self._posture = "standing"
+        elif inp == 1:
+            self._posture = "sitting"
+        elif inp == 2:
+            self._posture = "lying"
+        elif type(inp) == str:
+            if inp.lower() == "standing":
+                self._posture = "standing"
+            elif inp.lower() in ["sitting", "sedentary"]:
+                self._posture = "sitting"
+            elif inp.lower() in ["lying", "supine"]:
+                self._posture = "lying"
+        else:
+            self._posture = "standing"
+            print('posture must be 0="standing", 1="sitting" or 2="lying".')
+            print('posture was set "standing".')
+
+    @property
+    def clo(self):
+        """
+        Getter
+        Returns
+        -------
+        clo : numpy.ndarray (17,)
+            Clothing insulation [clo].
+        """
+        return self._clo
+
+    @clo.setter
+    def clo(self, inp):
+        self._clo = _to17array(inp)
+
+    @property
+    def par(self):
+        """
+        Getter
+        Returns
+        -------
+        par : float
+            Physical activity ratio [-].
+            This equals the ratio of metabolic rate to basal metabolic rate.
+            par of sitting quietly is 1.2.
+        """
+        return self._par
+
+    @par.setter
+    def par(self, inp):
+        self._par = inp
+
+    @property
+    def body_temp(self):
+        """
+        Getter
+        Returns
+        -------
+        bodytemp : numpy.ndarray (85,)
+            All segment temperatures of JOS-3
+        """
+        return self._bodytemp
+
+    @body_temp.setter
+    def body_temp(self, inp):
+        self._bodytemp = inp.copy()
+
+    # --------------------------------------------------------------------------
+    # Getter
+    # --------------------------------------------------------------------------
+
+    @property
+    def bsa(self):
+        """
+        Getter
+        Returns
+        -------
+        bsa : numpy.ndarray (17,)
+            Body surface areas by local body segments [m2].
+        """
+        return self._bsa.copy()
+
+    @property
+    def r_dry(self):
+        """
+        Getter
+        Returns
+        -------
+        r_dry : numpy.ndarray (17,)
+            Dry heat resistances between the skin and ambience areas by local body segments [K.m2/W].
+        """
+        hc = threg.fixed_hc(
+            threg.conv_coef(
+                self._posture,
+                self._va,
+                self._ta,
+                self.t_skin,
+            ),
+            self._va,
+        )
+        hr = threg.fixed_hr(
+            threg.rad_coef(
+                self._posture,
+            )
+        )
+        return threg.dry_r(hc, hr, self._clo)
+
+    @property
+    def r_lat(self):
+        """
+        Getter
+        Returns
+        -------
+        r_lat : numpy.ndarray (17,)
+            w (Evaporative) heat resistances between the skin and ambience areas by local body segments [Pa.m2/W].
+        """
+        hc = threg.fixed_hc(
+            threg.conv_coef(
+                self._posture,
+                self._va,
+                self._ta,
+                self.t_skin,
+            ),
+            self._va,
+        )
+        return threg.wet_r(hc, self._clo, self._iclo)
+
+    @property
+    def w(self):
+        """
+        Getter
+        Returns
+        -------
+        w : numpy.ndarray (17,)
+            Skin wettedness on local body segments [-].
+        """
+        err_cr = self.t_core - self.setpt_cr
+        err_sk = self.t_skin - self.setpt_sk
+        wet, *_ = threg.evaporation(
+            err_cr, err_sk, self._ta, self._rh, self.r_lat, self._bsa_rate, self._age
+        )
+        return wet
+
+    @property
+    def w_mean(self):
+        """
+        Getter
+        Returns
+        -------
+        w_mean : float
+            Mean skin wettedness of the whole body [-].
+        """
+        wet = self.w
+        return np.average(wet, weights=_BSAst)
+
+    @property
+    def t_skin_mean(self):
+        """
+        Getter
+        Returns
+        -------
+        t_skin_mean : float
+            Mean skin temperature of the whole body [°C].
+        """
+        return np.average(self._bodytemp[INDEX["skin"]], weights=_BSAst)
+
+    @property
+    def t_skin(self):
+        """
+        Getter
+        Returns
+        -------
+        t_skin : numpy.ndarray (17,)
+            Skin temperatures by the local body segments [°C].
+        """
+        return self._bodytemp[INDEX["skin"]].copy()
+
+    @property
+    def t_core(self):
+        """
+        Getter
+        Returns
+        -------
+        t_core : numpy.ndarray (17,)
+            Skin temperatures by the local body segments [°C].
+        """
+        return self._bodytemp[INDEX["core"]].copy()
+
+    @property
+    def t_cb(self):
+        """
+        Getter
+        Returns
+        -------
+        t_cb : numpy.ndarray (1,)
+            Temperature at central blood pool [°C].
+        """
+        return self._bodytemp[0].copy()
+
+    @property
+    def t_artery(self):
+        """
+        Getter
+        Returns
+        -------
+        t_artery : numpy.ndarray (17,)
+            Arterial temperatures by the local body segments [°C].
+        """
+        return self._bodytemp[INDEX["artery"]].copy()
+
+    @property
+    def t_vein(self):
+        """
+        Getter
+        Returns
+        -------
+        t_vein : numpy.ndarray (17,)
+            Vein temperatures by the local body segments [°C].
+        """
+        return self._bodytemp[INDEX["vein"]].copy()
+
+    @property
+    def t_superficial_vein(self):
+        """
+        Getter
+        Returns
+        -------
+        t_superficial_vein : numpy.ndarray (12,)
+            Superfical vein temperatures by the local body segments [°C].
+        """
+        return self._bodytemp[INDEX["sfvein"]].copy()
+
+    @property
+    def t_muscle(self):
+        """
+        Getter
+        Returns
+        -------
+        t_muscle : numpy.ndarray (2,)
+            Muscle temperatures of head and pelvis [°C].
+        """
+        return self._bodytemp[INDEX["muscle"]].copy()
+
+    @property
+    def t_fat(self):
+        """
+        Getter
+        Returns
+        -------
+        t_fat : numpy.ndarray (2,)
+            fat temperatures of head and pelvis  [°C].
+        """
+        return self._bodytemp[INDEX["fat"]].copy()
+
+    @property
+    def body_names(self):
+        """
+        Getter
+        Returns
+        -------
+        body_names : list
+            JOS3 body names
+        """
+        return BODY_NAMES
+
+    @property
+    def results(self):
+        return self.dict_results()
+
+    @property
+    def bmr(self):
+        """
+        Getter
+        Returns
+        -------
+        bmr : float
+            Basal metabolic rate [W/m2].
+        """
+        tcr = threg.basal_met(
+            self._height,
+            self._weight,
+            self._age,
+            self._sex,
+            self._bmr_equation,
+        )
+        return tcr / self.bsa.sum()
+
+    @property
+    def version(self):
+        """
+        Getter
+        Returns
+        -------
+        version : float
+            The current version of pythermalcomfort.
+        """
+
+        return self._version
```

### Comparing `pythermalcomfort-2.7.0/src/pythermalcomfort/optimized_functions.py` & `pythermalcomfort-2.7.1/src/pythermalcomfort/optimized_functions.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/src/pythermalcomfort/psychrometrics.py` & `pythermalcomfort-2.7.1/src/pythermalcomfort/psychrometrics.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/src/pythermalcomfort/utilities.py` & `pythermalcomfort-2.7.1/src/pythermalcomfort/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import warnings
 import math
+import re
 from pythermalcomfort.psychrometrics import p_sat, t_o
 from pythermalcomfort.shared_functions import valid_range
 
 warnings.simplefilter("always")
 
 
 def transpose_sharp_altitude(sharp, altitude):
@@ -206,25 +207,32 @@
 
     Parameters
     ----------
     weight : float
         body weight, [kg]
     height : float
         height, [m]
-    formula : {"dubois"}, default="dubois"
-        formula used to calculate the body surface area
+    formula : str, optional,
+        formula used to calculate the body surface area. default="dubois"
+        Choose a name from "dubois", "takahira", "fujimoto", or "kurazumi".
 
     Returns
     -------
     body_surface_area : float
         body surface area, [m2]
     """
 
     if formula == "dubois":
         return 0.202 * (weight**0.425) * (height**0.725)
+    elif formula == "takahira":
+        return 0.2042 * (weight**0.425) * (height**0.725)
+    elif formula == "fujimoto":
+        return 0.1882 * (weight**0.444) * (height**0.663)
+    elif formula == "kurazumi":
+        return 0.2440 * (weight**0.383) * (height**0.693)
 
 
 def f_svv(w, h, d):
     """Calculates the sky-vault view fraction.
 
     Parameters
     ----------
```

### Comparing `pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/PKG-INFO` & `pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pythermalcomfort
-Version: 2.7.0
+Version: 2.7.1
 Summary: Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET, adaptive) and convert physical variables. Please cite us if you use this package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python package for thermal comfort research. SoftwareX 12, 100578. https://doi.org/10.1016/j.softx.2020.100578
 Home-page: https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort
 Author: Federico Tartarini
 Author-email: cbecomforttool@gmail.com
 License: MIT
 Project-URL: Documentation, https://pythermalcomfort.readthedocs.io/
 Project-URL: Changelog, https://pythermalcomfort.readthedocs.io/en/latest/changelog.html
```

### Comparing `pythermalcomfort-2.7.0/src/pythermalcomfort.egg-info/SOURCES.txt` & `pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -18,25 +18,27 @@
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.appveyor.yml
 ci/templates/.travis.yml
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
+docs/contact_us.rst
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/readme.rst
 docs/requirements.txt
 docs/spelling_wordlist.txt
 docs/usage.rst
 docs/reference/index.rst
 docs/reference/pythermalcomfort.rst
 examples/calc_adaptive_ASHRAE.py
 examples/calc_adaptive_EN.py
+examples/calc_jos3.py
 examples/calc_phs.py
 examples/calc_pmv_ppd.py
 examples/calc_set_tmp.py
 examples/calc_utci.py
 src/pythermalcomfort/__init__.py
 src/pythermalcomfort/__main__.py
 src/pythermalcomfort/cli.py
@@ -48,9 +50,15 @@
 src/pythermalcomfort.egg-info/PKG-INFO
 src/pythermalcomfort.egg-info/SOURCES.txt
 src/pythermalcomfort.egg-info/dependency_links.txt
 src/pythermalcomfort.egg-info/entry_points.txt
 src/pythermalcomfort.egg-info/not-zip-safe
 src/pythermalcomfort.egg-info/requires.txt
 src/pythermalcomfort.egg-info/top_level.txt
+src/pythermalcomfort/jos3_functions/construction.py
+src/pythermalcomfort/jos3_functions/matrix.py
+src/pythermalcomfort/jos3_functions/parameters.py
+src/pythermalcomfort/jos3_functions/thermoregulation.py
+src/pythermalcomfort/jos3_functions/utilities.py
+tests/test_jos3.py
 tests/test_models.py
 tests/test_pythermalcomfort.py
```

### Comparing `pythermalcomfort-2.7.0/tests/test_models.py` & `pythermalcomfort-2.7.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.0/tox.ini` & `pythermalcomfort-2.7.1/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
     py36: {env:TOXPYTHON:python3.6}
     py37: {env:TOXPYTHON:python3.7}
-    {py38,docs}: {env:TOXPYTHON:python3.8}
-    py39: {env:TOXPYTHON:python3.9}
+    py39: {env:TOXPYTHON:python3.8}
+    {py39,docs}: {env:TOXPYTHON:python3.9}
     py310: {env:TOXPYTHON:python3.10}
     {bootstrap,clean,check,report,codecov}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
@@ -36,15 +36,14 @@
 deps =
     pytest<7
     requests
     pytest-travis-fold
     pytest-cov
     scipy
     numba
-    jos3
 commands =
     {posargs:pytest --cov --cov-report=term-missing -vv tests}
 
 [testenv:check]
 deps =
     docutils
     check-manifest
```

