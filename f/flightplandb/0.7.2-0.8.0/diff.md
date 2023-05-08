# Comparing `tmp/flightplandb-0.7.2.tar.gz` & `tmp/flightplandb-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightplandb-0.7.2.tar", last modified: Mon Mar 27 20:11:19 2023, max compression
+gzip compressed data, was "flightplandb-0.8.0.tar", last modified: Mon May  8 18:44:14 2023, max compression
```

## Comparing `flightplandb-0.7.2.tar` & `flightplandb-0.8.0.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.064639 flightplandb-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.036639 flightplandb-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.044638 flightplandb-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-27 20:10:58.000000 flightplandb-0.7.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-27 20:10:58.000000 flightplandb-0.7.2/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-27 20:10:58.000000 flightplandb-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-27 20:10:58.000000 flightplandb-0.7.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-27 20:10:58.000000 flightplandb-0.7.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-27 20:10:58.000000 flightplandb-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 20:10:58.000000 flightplandb-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-27 20:11:19.060639 flightplandb-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-27 20:10:58.000000 flightplandb-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.036639 flightplandb-0.7.2/artwork/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.044638 flightplandb-0.7.2/artwork/ico/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-27 20:10:58.000000 flightplandb-0.7.2/artwork/ico/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.044638 flightplandb-0.7.2/artwork/png/
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-03-27 20:10:58.000000 flightplandb-0.7.2/artwork/png/120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-03-27 20:10:58.000000 flightplandb-0.7.2/artwork/png/240x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-27 20:10:58.000000 flightplandb-0.7.2/artwork/png/32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-03-27 20:10:58.000000 flightplandb-0.7.2/artwork/png/480x480.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.044638 flightplandb-0.7.2/artwork/svg/
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-03-27 20:10:58.000000 flightplandb-0.7.2/artwork/svg/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.044638 flightplandb-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.044638 flightplandb-0.7.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.036639 flightplandb-0.7.2/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.048639 flightplandb-0.7.2/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   118473 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/_static/css/colourscheme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.052639 flightplandb-0.7.2/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/datatypes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/internal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/nav.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/plan.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/api/weather.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.052639 flightplandb-0.7.2/docs/source/user/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/user/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/user/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/user/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-27 20:10:58.000000 flightplandb-0.7.2/docs/source/user/userdocs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-27 20:10:58.000000 flightplandb-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 20:11:19.064639 flightplandb-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.040639 flightplandb-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.056639 flightplandb-0.7.2/src/flightplandb/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-27 20:10:58.000000 flightplandb-0.7.2/src/flightplandb/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.060639 flightplandb-0.7.2/src/flightplandb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-27 20:11:19.000000 flightplandb-0.7.2/src/flightplandb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-27 20:11:19.000000 flightplandb-0.7.2/src/flightplandb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:11:19.000000 flightplandb-0.7.2/src/flightplandb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-27 20:11:19.000000 flightplandb-0.7.2/src/flightplandb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 20:11:19.000000 flightplandb-0.7.2/src/flightplandb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:11:19.060639 flightplandb-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-27 20:10:58.000000 flightplandb-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-03-27 20:10:58.000000 flightplandb-0.7.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-03-27 20:10:58.000000 flightplandb-0.7.2/tests/test_nav.py
--rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-03-27 20:10:58.000000 flightplandb-0.7.2/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-27 20:10:58.000000 flightplandb-0.7.2/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-03-27 20:10:58.000000 flightplandb-0.7.2/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-27 20:10:58.000000 flightplandb-0.7.2/tests/test_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.637191 flightplandb-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-08 18:43:57.000000 flightplandb-0.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 18:43:57.000000 flightplandb-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 18:43:57.000000 flightplandb-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-08 18:44:14.637191 flightplandb-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-08 18:43:57.000000 flightplandb-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/artwork/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/artwork/ico/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/ico/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/artwork/png/
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/png/120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/png/240x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/png/32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/png/480x480.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/artwork/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/svg/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   118473 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/_static/css/colourscheme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/datatypes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/internal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/nav.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/plan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/weather.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/source/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/user/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/user/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/user/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/user/userdocs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-08 18:43:57.000000 flightplandb-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:44:14.637191 flightplandb-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/src/flightplandb/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26569 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.637191 flightplandb-0.8.0/src/flightplandb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.637191 flightplandb-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26129 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_weather.py
```

### Comparing `flightplandb-0.7.2/.github/workflows/release.yml` & `flightplandb-0.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/.github/workflows/test_and_lint.yml` & `flightplandb-0.8.0/.github/workflows/test.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,10 @@
-name: Tests and lint
+name: Tests
 on: [push, workflow_dispatch]
 jobs:
-  # no need to set up a matrix for the lint
-  flake8-lint:
-    runs-on: ubuntu-latest
-    name: Flake8 Lint
-    steps:
-      - name: Check out source repository
-        uses: actions/checkout@v2
-      - name: Set up Python environment
-        uses: actions/setup-python@v2
-        with:
-          python-version: "3.9"
-      - name: flake8 Lint
-        uses: py-actions/flake8@v1
-        with:
-          max-line-length: "120"
-
-  # but we do want to run unittests on many python versions
   unittests:
     strategy:
       matrix:
         python-version: [ '3.8', '3.9', '3.10', '3.11']
     runs-on: ubuntu-latest
 
     name: Unit tests, Python ${{ matrix.python-version }}
@@ -32,8 +15,8 @@
       - name: Set up Python environment
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install packages
         run: python -m pip install .[test]
       - name: Run unittests
-        run: python -m pytest tests
+        run: python -m pytest tests
```

### Comparing `flightplandb-0.7.2/.readthedocs.yaml` & `flightplandb-0.8.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/LICENSE` & `flightplandb-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/PKG-INFO` & `flightplandb-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightplandb
-Version: 0.7.2
+Version: 0.8.0
 Summary: Python wrapper for the Flight Plan Database API
 Author-email: PH-KDX <smtp.python.email.sender@gmail.com>
 License: GPL v3
 Project-URL: Homepage, https://github.com/PH-KDX/flightplandb-py/
 Project-URL: Documentation, https://flightplandb-py.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/PH-KDX/flightplandb-py/issues
 Project-URL: Changelog, https://github.com/PH-KDX/flightplandb-py/blob/main/CHANGELOG.rst
@@ -22,24 +22,26 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Games/Entertainment :: Simulation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/PH-KDX/flightplandb-py/main/artwork/png/240x240.png" alt="FlightPlanDB-py logo">
 </p>
 
 # FlightplanDB-py
 
 ## Project status
-![Unittests and lint](https://github.com/PH-KDX/flightplandb-py/actions/workflows/test_and_lint.yml/badge.svg)
+![Unittests and lint](https://github.com/PH-KDX/flightplandb-py/actions/workflows/test.yml/badge.svg)
+![Lint](https://github.com/PH-KDX/flightplandb-py/actions/workflows/lint.yml/badge.svg)
 [![PyPi](https://img.shields.io/pypi/v/flightplandb.svg)](https://pypi.org/project/flightplandb/)
 ![Python](https://img.shields.io/pypi/pyversions/flightplandb.svg)
 
 ## Introduction
 This is a Python 3 wrapper for the [Flight Plan Database API](https://flightplandatabase.com/dev/api). Flight Plan Database is a website for creating and sharing flight plans for use in flight simulation.
 
 For more information on Flight Plan Database, see their excellent [About page](https://flightplandatabase.com/about).
```

### Comparing `flightplandb-0.7.2/README.md` & `flightplandb-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <p align="center">
     <img src="https://raw.githubusercontent.com/PH-KDX/flightplandb-py/main/artwork/png/240x240.png" alt="FlightPlanDB-py logo">
 </p>
 
 # FlightplanDB-py
 
 ## Project status
-![Unittests and lint](https://github.com/PH-KDX/flightplandb-py/actions/workflows/test_and_lint.yml/badge.svg)
+![Unittests and lint](https://github.com/PH-KDX/flightplandb-py/actions/workflows/test.yml/badge.svg)
+![Lint](https://github.com/PH-KDX/flightplandb-py/actions/workflows/lint.yml/badge.svg)
 [![PyPi](https://img.shields.io/pypi/v/flightplandb.svg)](https://pypi.org/project/flightplandb/)
 ![Python](https://img.shields.io/pypi/pyversions/flightplandb.svg)
 
 ## Introduction
 This is a Python 3 wrapper for the [Flight Plan Database API](https://flightplandatabase.com/dev/api). Flight Plan Database is a website for creating and sharing flight plans for use in flight simulation.
 
 For more information on Flight Plan Database, see their excellent [About page](https://flightplandatabase.com/about).
```

### Comparing `flightplandb-0.7.2/artwork/ico/favicon.ico` & `flightplandb-0.8.0/artwork/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/artwork/png/120x120.png` & `flightplandb-0.8.0/artwork/png/120x120.png`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/artwork/png/240x240.png` & `flightplandb-0.8.0/artwork/png/240x240.png`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/artwork/png/32x32.png` & `flightplandb-0.8.0/artwork/png/32x32.png`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/artwork/png/480x480.png` & `flightplandb-0.8.0/artwork/png/480x480.png`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/artwork/svg/logo.svg` & `flightplandb-0.8.0/artwork/svg/logo.svg`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/docs/Makefile` & `flightplandb-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/docs/source/_static/css/colourscheme.css` & `flightplandb-0.8.0/docs/source/_static/css/colourscheme.css`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/docs/source/api/plan.rst` & `flightplandb-0.8.0/docs/source/api/plan.rst`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/docs/source/conf.py` & `flightplandb-0.8.0/docs/source/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,75 +7,78 @@
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 import os
 import sys
+
 from flightplandb import __version__
-sys.path.insert(0, os.path.abspath('../../'))
+
+sys.path.insert(0, os.path.abspath("../../"))
 
 
 # -- Project information -----------------------------------------------------
 
-project = 'FlightplanDB-py'
-copyright = '2022, PH-KDX'
-author = 'PH-KDX'
+project = "FlightplanDB-py"
+copyright = "2022, PH-KDX"
+author = "PH-KDX"
 
 # The full version, including alpha/beta/rc tags
 release = __version__
 # readthedocs.io insists on the version field being filled for epub builds
 version = release
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 
-extensions = ['sphinx.ext.autodoc',  # HTML generation from docstrings
-              'sphinx.ext.napoleon',  # Read NumPy style docstrings
-              'sphinx.ext.autosummary',  # Create neat summary tables
-              ]
+extensions = [
+    "sphinx.ext.autodoc",  # HTML generation from docstrings
+    "sphinx.ext.napoleon",  # Read NumPy style docstrings
+    "sphinx.ext.autosummary",  # Create neat summary tables
+]
 
 autosummary_generate = True  # Turn on sphinx.ext.autosummary
 
-autodoc_member_order = 'bysource'
+autodoc_member_order = "bysource"
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 html_logo = "../../artwork/png/120x120.png"
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 html_favicon = "../../artwork/ico/favicon.ico"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 smartquotes = False
 
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 
 def setup(app):
     app.add_css_file("css/colourscheme.css")
```

### Comparing `flightplandb-0.7.2/docs/source/index.rst` & `flightplandb-0.8.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/docs/source/user/introduction.rst` & `flightplandb-0.8.0/docs/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/docs/source/user/quickstart.rst` & `flightplandb-0.8.0/docs/source/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flightplandb-0.7.2/pyproject.toml` & `flightplandb-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -32,25 +32,33 @@
     "aiohttp >= 3.8.4; python_version >= '3.11'",
     "aiohttp >= 3.5.2; python_version < '3.11'",
     "python-dateutil~=2.8.2",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-docs = ["Sphinx==6.1.3", "sphinx-rtd-theme==1.2.0"]
-test = ["pytest~=7.2.1", "pytest-socket~=0.6.0", "pytest-asyncio~=0.20.3"]
+docs = ["Sphinx==6.2.1", "sphinx-rtd-theme==1.2.0"]
+test = ["pytest~=7.3.1", "pytest-socket~=0.6.0", "pytest-asyncio~=0.21.0"]
+dev = ["pre-commit"]
 
 [project.urls]
 "Homepage" = "https://github.com/PH-KDX/flightplandb-py/"
 "Documentation" = "https://flightplandb-py.readthedocs.io/"
 "Issue tracker" = "https://github.com/PH-KDX/flightplandb-py/issues"
 "Changelog" = "https://github.com/PH-KDX/flightplandb-py/blob/main/CHANGELOG.rst"
 
 [tool.setuptools.dynamic]
 version = {attr = "flightplandb.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools.package-data]
+flightplandb = ['py.typed']
+
 [tool.pytest.ini_options]
 addopts = "-vv --disable-socket"
 asyncio_mode = "auto"
+
+[tool.isort]
+profile = "black"
+line_length = 88
```

### Comparing `flightplandb-0.7.2/src/flightplandb/__init__.py` & `flightplandb-0.8.0/src/flightplandb/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 For more information on Flight Plan Database, read their excellent About page
 at https://flightplandatabase.com/about. For more information about this
 library, read the documentation at https://flightplandb-py.readthedocs.io/.
 """
 
 
 # Version of the flightplandb package
-__version__ = "0.7.2"
+__version__ = "0.8.0"
 
-from . import (
-    internal, exceptions, datatypes,
-    api, nav, plan, tags, user, weather
-    )
+from . import api, datatypes, exceptions, internal, nav, plan, tags, user, weather
 
 __all__ = [
-    "internal", "exceptions", "datatypes", "api",
-    "nav", "plan", "tags", "user", "weather"
-    ]
+    "internal",
+    "exceptions",
+    "datatypes",
+    "api",
+    "nav",
+    "plan",
+    "tags",
+    "user",
+    "weather",
+]
```

### Comparing `flightplandb-0.7.2/src/flightplandb/api.py` & `flightplandb-0.8.0/src/flightplandb/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """These functions return information about the API."""
 from typing import Optional
+
 from flightplandb import internal
 from flightplandb.datatypes import StatusResponse
 
 
 async def header_value(header_key: str, key: Optional[str] = None) -> str:
     """Gets header value for key. Do not call directly.
```

### Comparing `flightplandb-0.7.2/src/flightplandb/datatypes.py` & `flightplandb-0.8.0/src/flightplandb/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,36 +13,38 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with FlightplanDB-py.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from typing import List, Union, Optional
 from dataclasses import dataclass
 from datetime import datetime
+from typing import List, Optional, Union
+
 from dateutil.parser import isoparse
 
 
 def _datetime_to_iso(timestamp: datetime):
-    return timestamp.strftime('%Y-%m-%dT%H:%M:%S.%f')[:-3] + 'Z'
+    return timestamp.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z"
 
 
 @dataclass
 class StatusResponse:
     """
     Returned for some functions to indicate execution status
 
     Attributes
     ----------
     message : str
         The message associated with the status returned
     errors : Optional[List[str]]
         A list of any errors raised
     """
+
     message: str
     errors: Optional[List[str]]
 
     def to_api_dict(self):
         return self.__dict__
 
 
@@ -69,14 +71,15 @@
     plansDistance : Optional[float]
         Total distance of all user's flight plans
     plansDownloads : Optional[int]
         Total download count of all user's plans
     plansLikes : Optional[int]
         Total like count of all user's plans
     """
+
     id: int
     username: str
     location: Optional[str] = None
     gravatarHash: Optional[str] = None
     joined: Optional[datetime] = None
     lastSeen: Optional[datetime] = None
     plansCount: Optional[int] = 0
@@ -110,14 +113,15 @@
     username : str
         Username
     location : Optional[str]
         User provided location information. ``None`` if not available
     gravatarHash : Optional[str]
         Gravatar hash based on user's account email address.
     """
+
     id: int
     username: str
     location: Optional[str] = None
     gravatarHash: Optional[str] = None
 
     def to_api_dict(self):
         return self.__dict__
@@ -132,14 +136,15 @@
     id : int
         Unique application identifier number
     name : Optional[str]
         Application name
     url : Optional[str]
         Application URL
     """
+
     id: int
     name: Optional[str] = None
     url: Optional[str] = None
 
     def to_api_dict(self):
         return self.__dict__
 
@@ -153,18 +158,19 @@
     ident : str
         desc
     type : str
         Type of Via; must be one of :py:obj:`Via.validtypes`
     validtypes : List[str]
         Do not change. Valid Via types.
     """
+
     ident: str
     type: str
 
-    validtypes = ['SID', 'STAR', 'AWY-HI', 'AWY-LO', 'NAT', 'PACOT']
+    validtypes = ["SID", "STAR", "AWY-HI", "AWY-LO", "NAT", "PACOT"]
 
     def __post_init__(self):
         if self.type not in self.validtypes:
             raise ValueError(f"{self.type} is not a valid Via type")
 
     def to_api_dict(self):
         return self.__dict__
@@ -193,24 +199,25 @@
     name : Optional[str]
         Node name.
     via : Optional[Via]
         Route to node.
     validtypes : List[str]
         Do not change. Valid RouteNode types.
     """
+
     ident: str
     type: str
     lat: float
     lon: float
     id: Optional[int] = None
     alt: Optional[float] = None
     name: Optional[str] = None
     via: Optional[Via] = None
 
-    validtypes = ['UKN', 'APT', 'NDB', 'VOR', 'FIX', 'DME', 'LATLON']
+    validtypes = ["UKN", "APT", "NDB", "VOR", "FIX", "DME", "LATLON"]
 
     def __post_init__(self):
         if self.type not in self.validtypes:
             raise ValueError(f"{self.type} is not a valid RouteNode type")
         self.via = Via(**self.via) if isinstance(self.via, dict) else self.via
 
     def to_api_dict(self):
@@ -229,28 +236,32 @@
     nodes : List[RouteNode]
         A list of :class:`RouteNode` s. A route must have at least 2 nodes.
     eastLevels : Optional[List[str]]
         Valid eastbound flightlevels. Only used inside a NATS :class:`Track`.
     westLevels : Optional[List[str]]
         Valid westbound flightlevels. Only used inside a NATS :class:`Track`.
     """
+
     nodes: List[RouteNode]
     eastLevels: Optional[List[str]] = None
     westLevels: Optional[List[str]] = None
 
     def __post_init__(self):
-        self.nodes = list(map(
-            lambda node: (
-                RouteNode(**node) if (isinstance(node, dict)) else node),
-            self.nodes))
+        self.nodes = list(
+            map(
+                lambda node: (RouteNode(**node) if (isinstance(node, dict)) else node),
+                self.nodes,
+            )
+        )
 
     def to_api_dict(self):
         resp_dict = self.__dict__
-        resp_dict["nodes"] = list(map(
-            lambda node: node.to_api_dict(), resp_dict["nodes"]))
+        resp_dict["nodes"] = list(
+            map(lambda node: node.to_api_dict(), resp_dict["nodes"])
+        )
         return resp_dict
 
 
 @dataclass
 class Cycle:
     """Navdata cycle
 
@@ -261,14 +272,15 @@
     ident : str
         AIP-style cycle id
     year : int
         Last two digits of cycle year
     release : int
         Cycle release
     """
+
     id: int
     ident: str
     year: int
     release: int
 
     def to_api_dict(self):
         return self.__dict__
@@ -320,14 +332,15 @@
         Application associated with the item. ``None`` if no application linked
     route : Optional[Route]
         The flight plan route
     cycle : Optional[Cycle]
         Navigation data cycle associated with the item.
         ``None`` if no cycle linked
     """
+
     fromICAO: Optional[str]
     toICAO: Optional[str]
     fromName: Optional[str]
     toName: Optional[str]
     id: Optional[int] = None
     flightNumber: Optional[str] = None
     distance: Optional[float] = None
@@ -343,20 +356,19 @@
     tags: Optional[List[str]] = None
     user: Optional[User] = None
     application: Optional[Application] = None
     route: Optional[Route] = None
     cycle: Optional[Cycle] = None
 
     def __post_init__(self):
-
         if self.createdAt and type(self.createdAt) != datetime:
-            self.createdAt = (isoparse(self.createdAt))
+            self.createdAt = isoparse(self.createdAt)
 
         if self.updatedAt and type(self.updatedAt) != datetime:
-            self.updatedAt = (isoparse(self.updatedAt))
+            self.updatedAt = isoparse(self.updatedAt)
 
         if self.user and isinstance(self.user, dict):
             self.user = User(**self.user)
 
         if self.application and isinstance(self.application, dict):
             self.application = Application(**self.application)
 
@@ -401,32 +413,36 @@
         Matches destination airport name
     flightNumber : Optional[str]
         Matches flight number
     distanceMin : Optional[str]
         Minimum route distance
     distanceMax : Optional[str]
         Maximum route distance, with units determined by the X-Units header
-    tags : Optional[str]
-        Tag names to search, comma separated
+    tags : Optional[List[str]]
+        List of tag names to search
     """
+
     q: Optional[str] = None
     From: Optional[str] = None
     to: Optional[str] = None
     fromICAO: Optional[str] = None
     toICAO: Optional[str] = None
     fromName: Optional[str] = None
     toName: Optional[str] = None
     flightNumber: Optional[str] = None
     distanceMin: Optional[str] = None
     distanceMax: Optional[str] = None
-    tags: Optional[str] = None
+    tags: Optional[List[str]] = None
     includeRoute: Optional[bool] = None
 
     def to_api_dict(self):
-        return self.__dict__
+        plan_query_dict = self.__dict__
+        if self.tags:
+            plan_query_dict["tags"] = ", ".join(self.tags)
+        return plan_query_dict
 
 
 @dataclass
 class GenerateQuery:
     """Generate plan query.
 
     Attributes
@@ -452,14 +468,15 @@
     ascentSpeed : Optional[float]
         Basic flight profile ascent speed (speed)
     descentRate : Optional[float]
         Basic flight profile descent rate (climb rate)
     descentSpeed : Optional[float]
         Basic flight profile descent speed (speed)
     """
+
     fromICAO: str
     toICAO: str
     useNAT: Optional[bool] = True
     usePACOT: Optional[bool] = True
     useAWYLO: Optional[bool] = True
     useAWYHI: Optional[bool] = True
     cruiseAlt: Optional[float] = 35000
@@ -484,14 +501,15 @@
     description : Optional[str]
         Description of the tag. ``None`` if no description is available
     planCount : int
         Number of plans with this tag
     popularity: int
         Popularity index of the tag
     """
+
     name: str
     description: Optional[str]
     planCount: int
     popularity: int
 
     def to_api_dict(self):
         return self.__dict__
@@ -505,14 +523,15 @@
     ----------
     name : Optional[str]
         The IANA timezone the airport is located in. ``None`` if not available
     offset : Optional[float]
         The number of seconds the airport timezone is currently
         offset from UTC. Positive is ahead of UTC. ``None`` if not available
     """
+
     name: Optional[str]
     offset: Optional[float]
 
     def to_api_dict(self):
         return self.__dict__
 
 
@@ -527,32 +546,37 @@
     sunset : datetime
         Time of sunset
     dawn : datetime
         Time of dawn
     dusk : datetime
         Time of dusk
     """
+
     sunrise: datetime
     sunset: datetime
     dawn: datetime
     dusk: datetime
 
     def __post_init__(self):
-        self.sunrise = (isoparse(self.sunrise)
-                        if not isinstance(self.sunrise, datetime)
-                        else self.sunrise)
-        self.sunset = (isoparse(self.sunset)
-                       if not isinstance(self.sunset, datetime)
-                       else self.sunset)
-        self.dawn = (isoparse(self.dawn)
-                     if not isinstance(self.dawn, datetime)
-                     else self.dawn)
-        self.dusk = (isoparse(self.dusk)
-                     if not isinstance(self.dusk, datetime)
-                     else self.dusk)
+        self.sunrise = (
+            isoparse(self.sunrise)
+            if not isinstance(self.sunrise, datetime)
+            else self.sunrise
+        )
+        self.sunset = (
+            isoparse(self.sunset)
+            if not isinstance(self.sunset, datetime)
+            else self.sunset
+        )
+        self.dawn = (
+            isoparse(self.dawn) if not isinstance(self.dawn, datetime) else self.dawn
+        )
+        self.dusk = (
+            isoparse(self.dusk) if not isinstance(self.dusk, datetime) else self.dusk
+        )
 
     def to_api_dict(self):
         plan_dict = self.__dict__
         plan_dict["sunrise"] = _datetime_to_iso(plan_dict["sunrise"])
         plan_dict["sunset"] = _datetime_to_iso(plan_dict["sunset"])
         plan_dict["dawn"] = _datetime_to_iso(plan_dict["dawn"])
         plan_dict["dusk"] = _datetime_to_iso(plan_dict["dusk"])
@@ -568,14 +592,15 @@
     ident : str
         The identifier of the runway end
     lat : float
         The latitude of the runway end
     lon : float
         The longitude of the runway end
     """
+
     ident: str
     lat: float
     lon: float
 
     def to_api_dict(self):
         return self.__dict__
 
@@ -609,28 +634,29 @@
     elevation: float
         The navaid elevation above mean sea level (elevation)
     range: float
         The navaid range; units determined by the X-Units header (distance)
     validtypes : List[str]
         Do not change. Valid Navaid types.
     """
+
     ident: str
     type: str
     lat: float
     lon: float
     airport: str
     runway: str
     frequency: Optional[float]
     slope: Optional[float]
     bearing: Optional[float]
     name: Optional[str]
     elevation: float
     range: float
 
-    validtypes = ['LOC-ILS', 'LOC-LOC', 'GS', 'DME', 'OM', 'MM', 'IM']
+    validtypes = ["LOC-ILS", "LOC-LOC", "GS", "DME", "OM", "MM", "IM"]
 
     def __post_init__(self):
         if self.type not in self.validtypes:
             raise ValueError(f"{self.type} is not a valid Navaid type")
 
     def to_api_dict(self):
         return self.__dict__
@@ -661,14 +687,15 @@
     overrunLength: float
         The runway overrun length, with units determined by the X-Units header
     ends: List[RunwayEnds]
         Two element List containing the location of the two ends of the runway
     navaids: List[Navaid]
         List of navaids associated with the current runway
     """
+
     ident: str
     width: float
     length: float
     bearing: float
     surface: str
     markings: List[str]
     lighting: List[str]
@@ -681,18 +708,18 @@
         if self.ends and (isinstance(self.ends[0], dict)):
             self.ends = list(map(lambda rw: RunwayEnds(**rw), self.ends))
         if self.navaids and (isinstance(self.navaids[0], dict)):
             self.navaids = list(map(lambda n: Navaid(**n), self.navaids))
 
     def to_api_dict(self):
         resp_dict = self.__dict__
-        resp_dict["ends"] = list(map(lambda end: end.to_api_dict(),
-                                     resp_dict["ends"]))
-        resp_dict["navaids"] = list(map(lambda aid: aid.to_api_dict(),
-                                        resp_dict["navaids"]))
+        resp_dict["ends"] = list(map(lambda end: end.to_api_dict(), resp_dict["ends"]))
+        resp_dict["navaids"] = list(
+            map(lambda aid: aid.to_api_dict(), resp_dict["navaids"])
+        )
         return resp_dict
 
 
 @dataclass
 class Frequency:
     """Holds frequency information
 
@@ -702,14 +729,15 @@
         The frequency type
     frequency : float
         The frequency in Hz
     name : Optional[str]
         The frequency name. ``None`` if not available
 
     """
+
     type: str
     frequency: float
     name: Optional[str]
 
     def to_api_dict(self):
         return self.__dict__
 
@@ -721,14 +749,15 @@
     Attributes
     ----------
     METAR : Optional[str]
         Current METAR report for the airport
     TAF : Optional[str]
         Current TAF report for the airport
     """
+
     METAR: Optional[str]
     TAF: Optional[str]
 
     def to_api_dict(self):
         return self.__dict__
 
 
@@ -767,14 +796,15 @@
         List of runways.
         Note: each physical runway will appear twice, once from each end
     frequencies: List[Frequency]
         List of frequencies associated with the airport
     weather: Weather
         Airport weather information
     """
+
     ICAO: str
     IATA: Optional[str]
     name: str
     regionName: Optional[str]
     elevation: float
     lat: float
     lon: float
@@ -793,28 +823,29 @@
         if self.times and isinstance(self.times, dict):
             self.times = Times(**self.times)
 
         if self.runways and isinstance(self.runways[0], dict):
             self.runways = list(map(lambda rw: Runway(**rw), self.runways))
 
         if self.frequencies and isinstance(self.frequencies[0], dict):
-            self.frequencies = list(
-                map(lambda rw: Frequency(**rw), self.frequencies))
+            self.frequencies = list(map(lambda rw: Frequency(**rw), self.frequencies))
 
         if self.weather and isinstance(self.weather, dict):
             self.weather = Weather(**self.weather)
 
     def to_api_dict(self):
         resp_dict = self.__dict__
         resp_dict["timezone"] = resp_dict["timezone"].to_api_dict()
         resp_dict["times"] = resp_dict["times"].to_api_dict()
-        resp_dict["runways"] = list(map(lambda rwy: rwy.to_api_dict(),
-                                        resp_dict["runways"]))
-        resp_dict["frequencies"] = list(map(lambda freq: freq.to_api_dict(),
-                                            resp_dict["frequencies"]))
+        resp_dict["runways"] = list(
+            map(lambda rwy: rwy.to_api_dict(), resp_dict["runways"])
+        )
+        resp_dict["frequencies"] = list(
+            map(lambda freq: freq.to_api_dict(), resp_dict["frequencies"])
+        )
         resp_dict["weather"] = resp_dict["weather"].to_api_dict()
         return resp_dict
 
 
 @dataclass
 class Track:
     """Used for NATS and PACOTS tracks
@@ -826,14 +857,15 @@
     route : Route
         Route of the track
     validFrom : datetime
         UTC datetime the track is valid from
     validTo : datetime
         UTC datetime the track is valid to
     """
+
     ident: Union[str, int]
     route: Route
     validFrom: datetime
     validTo: datetime
 
     def __post_init__(self):
         if self.route and isinstance(self.route, dict):
@@ -874,24 +906,25 @@
         The ICAO of the airport associated with the navaid.
         ``None`` if not available
     name: Optional[float]
         The navaid name. ``None`` if not available
     validtypes : List[str]
         Do not change. Valid SearchNavaid types
     """
+
     ident: str
     type: str
     lat: float
     lon: float
     elevation: float
     runwayIdent: Optional[str] = None
     airportICAO: Optional[str] = None
     name: Optional[float] = None
 
-    validtypes = ['UKN', 'APT', 'NDB', 'VOR', 'FIX', 'DME', 'LATLON']
+    validtypes = ["UKN", "APT", "NDB", "VOR", "FIX", "DME", "LATLON"]
 
     def __post_init__(self):
         if self.type not in self.validtypes:
             raise ValueError(f"{self.type} is not a valid SearchNavaid type")
 
     def to_api_dict(self):
         return self.__dict__
```

### Comparing `flightplandb-0.7.2/src/flightplandb/exceptions.py` & `flightplandb-0.8.0/src/flightplandb/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,43 +102,42 @@
 def status_handler(status_code, ignore_statuses=None):
     "Raises correct custom exception for appropriate HTTP status code."
     if status_code not in ignore_statuses and status_code >= 400:
         if status_code == 400:
             raise BadRequestException(
                 status_code=status_code,
                 message="The request could not be understood by "
-                "the server due to malformed syntax."
+                "the server due to malformed syntax.",
             )
         if status_code == 401:
             raise UnauthorizedException(
                 status_code=status_code,
                 message="You are incorrectly authorised and "
-                "may not make this request."
+                "may not make this request.",
             )
         elif status_code == 403:
             raise ForbiddenException(
                 status_code=status_code,
                 message="The server understood the request, "
-                "but is refusing to fulfill it."
+                "but is refusing to fulfill it.",
             )
         elif status_code == 404:
             raise NotFoundException(
                 status_code=status_code,
                 message="The server has not found anything "
-                "matching the Request-URI."
+                "matching the Request-URI.",
             )
         elif status_code == 429:
             raise TooManyRequestsException(
                 status_code=status_code,
-                message="Your requests limit for the server has been exceeded."
+                message="Your requests limit for the server has been exceeded.",
             )
         elif status_code == 500:
             raise InternalServerException(
                 status_code=status_code,
                 message="The server encountered an unexpected condition "
-                "which prevented it from fulfilling the request."
+                "which prevented it from fulfilling the request.",
             )
         else:
             raise BaseErrorHandler(
-                status_code=status_code,
-                message="Unknown Error Occurred."
+                status_code=status_code, message="Unknown Error Occurred."
             )
```

### Comparing `flightplandb-0.7.2/src/flightplandb/internal.py` & `flightplandb-0.8.0/src/flightplandb/internal.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,56 +15,154 @@
 #
 # You should have received a copy of the GNU General Public License along
 # with FlightplanDB-py.  If not, see <https://www.gnu.org/licenses/>.
 
 """This file mostly contains internal functions called by the API,
 so you're unlikely to ever use them."""
 
-from typing import AsyncIterable, List, Dict, Union, Optional
-
+import json
 from base64 import b64encode
+from typing import (
+    Any,
+    AsyncIterable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    overload,
+)
 from urllib.parse import urljoin
-import json
-import aiohttp
 
-from multidict import CIMultiDict
+import aiohttp
+from multidict import CIMultiDictProxy
 
 from flightplandb.exceptions import status_handler
 
-
 # https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#directive-autoclass
 # https://github.com/python/cpython/blob/main/Lib/random.py#L792
 
 url_base: str = "https://api.flightplandatabase.com"
 
 
 def _auth_str(key):
     """Returns a API auth string."""
 
     if isinstance(key, str):
         key = key.encode("latin1")
     else:
         raise ValueError("API key must be a string!")
 
-    authstr = "Basic " + (
-        b64encode(key + b":").strip().decode()
-    )
+    authstr = "Basic " + (b64encode(key + b":").strip().decode())
 
     return authstr
 
 
+format_return_types = {
+    # if a dict is requested, the JSON will later be converted to that
+    "native": "application/vnd.fpd.v1+json",
+    # otherwise, pure JSON will be returned
+    "json": "application/vnd.fpd.v1+json",
+    "xml": "application/vnd.fpd.v1+xml",
+    "csv": "text/vnd.fpd.export.v1.csv+csv",
+    "pdf": "application/vnd.fpd.export.v1.pdf",
+    "kml": "application/vnd.fpd.export.v1.kml+xml",
+    "xplane": "application/vnd.fpd.export.v1.xplane",
+    "xplane11": "application/vnd.fpd.export.v1.xplane11",
+    "fs9": "application/vnd.fpd.export.v1.fs9",
+    "fsx": "application/vnd.fpd.export.v1.fsx",
+    "squawkbox": "application/vnd.fpd.export.v1.squawkbox",
+    "xfmc": "application/vnd.fpd.export.v1.xfmc",
+    "pmdg": "application/vnd.fpd.export.v1.pmdg",
+    "airbusx": "application/vnd.fpd.export.v1.airbusx",
+    "qualitywings": "application/vnd.fpd.export.v1.qualitywings",
+    "ifly747": "application/vnd.fpd.export.v1.ifly747",
+    "flightgear": "application/vnd.fpd.export.v1.flightgear",
+    "tfdi717": "application/vnd.fpd.export.v1.tfdi717",
+    "infiniteflight": "application/vnd.fpd.export.v1.infiniteflight",
+}
+native_return_types_hints = Literal["native"]
+bytes_return_types_hints = Literal["pdf"]
+str_return_types_hints = Literal[
+    "json",
+    "xml",
+    "csv",
+    "kml",
+    "xplane",
+    "xplane11",
+    "fs9",
+    "fsx",
+    "squawkbox",
+    "xfmc",
+    "pmdg",
+    "airbusx",
+    "qualitywings",
+    "ifly747",
+    "flightgear",
+    "tfdi717",
+    "infiniteflight",
+]
+all_return_types_hints = Union[
+    native_return_types_hints, bytes_return_types_hints, str_return_types_hints
+]
+native_return_values = get_args(native_return_types_hints)
+bytes_return_values = get_args(bytes_return_types_hints)
+str_return_values = get_args(str_return_types_hints)
+
+
+@overload
 async def request(
     method: str,
     path: str,
-    return_format="native",
+    return_format: native_return_types_hints = "native",
     ignore_statuses: Optional[List] = None,
     params: Optional[Dict] = None,
     json_data: Optional[Dict] = None,
-    key: Optional[str] = None
-) -> Union[Dict, bytes]:
+    key: Optional[str] = None,
+) -> Tuple[CIMultiDictProxy[str], Dict]:
+    ...
+
+
+@overload
+async def request(
+    method: str,
+    path: str,
+    return_format: bytes_return_types_hints,
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    json_data: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Tuple[CIMultiDictProxy[str], bytes]:
+    ...
+
+
+@overload
+async def request(
+    method: str,
+    path: str,
+    return_format: str_return_types_hints,
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    json_data: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Tuple[CIMultiDictProxy[str], str]:
+    ...
+
+
+async def request(
+    method: str,
+    path: str,
+    return_format: all_return_types_hints = "native",
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    json_data: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Tuple[CIMultiDictProxy[str], Union[Any, bytes, str]]:
     """General HTTP requests function for non-paginated results.
 
     Parameters
     ----------
     method : str
         An HTTP request type. One of GET, POST, PATCH, or DELETE
     path : str
@@ -79,50 +177,29 @@
     json_data : `Dict`, optional
         Custom JSON data to be formatted into the request body
     key : str
         API token, defaults to None (which makes it unauthenticated)
 
     Returns
     -------
-    Union[Dict, bytes]
-        A ``dataclass`` if ``return_format`` is ``"native"``,
-        otherwise ``bytes``
+    Tuple[CIMultiDict, Union[Dict, str, bytes]]
+        | A tuple of:
+        | 1. A dict of the response headers, but the keys are case-insensitive
+        | 2. A ``Dict`` if ``return_format`` is ``"native"``,
+                otherwise ``str`` or ``bytes`` depending on if
+                the return format is UTF-8 or something else.
 
     Raises
     ------
     ValueError
         Invalid return_format option
     HTTPError
         Invalid HTTP status in response
     """
 
-    format_return_types = {
-        # if a dict is requested, the JSON will later be converted to that
-        "native": "application/vnd.fpd.v1+json",
-        # otherwise, pure JSON will be returned
-        "json": "application/vnd.fpd.v1+json",
-        "xml": "application/vnd.fpd.v1+xml",
-        "csv": "text/vnd.fpd.export.v1.csv+csv",
-        "pdf": "application/vnd.fpd.export.v1.pdf",
-        "kml": "application/vnd.fpd.export.v1.kml+xml",
-        "xplane": "application/vnd.fpd.export.v1.xplane",
-        "xplane11": "application/vnd.fpd.export.v1.xplane11",
-        "fs9": "application/vnd.fpd.export.v1.fs9",
-        "fsx": "application/vnd.fpd.export.v1.fsx",
-        "squawkbox": "application/vnd.fpd.export.v1.squawkbox",
-        "xfmc": "application/vnd.fpd.export.v1.xfmc",
-        "pmdg": "application/vnd.fpd.export.v1.pmdg",
-        "airbusx": "application/vnd.fpd.export.v1.airbusx",
-        "qualitywings": "application/vnd.fpd.export.v1.qualitywings",
-        "ifly747": "application/vnd.fpd.export.v1.ifly747",
-        "flightgear": "application/vnd.fpd.export.v1.flightgear",
-        "tfdi717": "application/vnd.fpd.export.v1.tfdi717",
-        "infiniteflight": "application/vnd.fpd.export.v1.infiniteflight"
-    }
-
     if not ignore_statuses:
         ignore_statuses = []
     if not params:
         params = {}
     request_headers = {}
 
     # the API only takes "true" or "false", not True or False
@@ -142,73 +219,103 @@
     # convert the API content return_format to an HTTP Accept type
     try:
         return_format_encoded = format_return_types[return_format]
     # unless it's not a valid return_format
     except KeyError as exc:
         raise ValueError(
             f"'{return_format}' is not a valid data return type option"
-            ) from exc
+        ) from exc
 
     # then add it to the request headers
-    params["Accept"] = return_format_encoded
+    request_headers["Accept"] = return_format_encoded
 
     # set auth in headers if key is provided
     if key is not None:
         request_headers["Authorization"] = _auth_str(key=key)
 
     async with aiohttp.ClientSession() as session:
         async with session.request(
             method=method,
             url=urljoin(url_base, path),
             params=params,
             headers=request_headers,
-            json=json_data
+            json=json_data,
         ) as resp:
-
             status_handler(resp.status, ignore_statuses)
 
             header = resp.headers
+            if return_format in native_return_values:
+                response_content = await resp.json()
+            # if the format is not a dict
+            elif return_format in str_return_values:
+                response_content = await resp.text()
+            elif return_format in bytes_return_values:
+                response_content = await resp.read()
 
-            if return_format == "native":
-                return header, await resp.json()
-            else:
-                return header, await resp.text()  # if the format is not a dict
+            return header, response_content
 
 
 # and here go the specific non-paginated HTTP calls
-async def get_headers(
-    key: Optional[str] = None
-) -> CIMultiDict:
+async def get_headers(key: Optional[str] = None) -> CIMultiDictProxy[str]:
     """Calls :meth:`request()` for request headers.
 
     Parameters
     ----------
     key : `str`, optional
         API token, defaults to None (which makes it unauthenticated)
 
     Returns
     -------
-    CaseInsensitiveDict
-        A dict of headers, but the keys are case-insensitive.
+    CIMultiDictProxy
+        A dict of the response headers, but the keys are case-insensitive.
     """
-    headers, _ = await request(
-        method="get",
-        path="",
-        key=key
-    )
+    headers, _ = await request(method="get", path="", key=key)
     return headers
 
 
+@overload
+async def get(
+    path: str,
+    return_format: native_return_types_hints = "native",
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Dict:
+    ...
+
+
+@overload
+async def get(
+    path: str,
+    return_format: bytes_return_types_hints,
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> bytes:
+    ...
+
+
+@overload
 async def get(
     path: str,
-    return_format="native",
+    return_format: str_return_types_hints,
     ignore_statuses: Optional[List] = None,
     params: Optional[Dict] = None,
-    key: Optional[str] = None
-) -> Union[Dict, bytes]:
+    key: Optional[str] = None,
+) -> str:
+    ...
+
+
+async def get(
+    path: str,
+    return_format: all_return_types_hints = "native",
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Union[Dict, str, bytes]:
     """Calls :meth:`request()` for get requests.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
     return_format : `str`, optional
@@ -220,43 +327,79 @@
         Any other HTTP request parameters, defaults to None
     key : `str`, optional
         API token, defaults to None (which makes it unauthenticated)
 
     Returns
     -------
     Union[Dict, bytes]
-        A ``dataclass`` if ``return_format`` is ``"native"``,
-        otherwise ``bytes``
+        A ``Dict`` if ``return_format`` is ``"native"``, otherwise ``str`` or ``bytes``
+        depending on if the return format is UTF-8 or something else.
     """
 
     # I HATE not being able to set empty lists as default arguments
     if not ignore_statuses:
         ignore_statuses = []
     if not params:
         params = {}
 
     _, resp = await request(
         method="get",
         path=path,
         return_format=return_format,
         ignore_statuses=ignore_statuses,
         params=params,
-        key=key
+        key=key,
     )
     return resp
 
 
+@overload
+async def post(
+    path: str,
+    return_format: native_return_types_hints = "native",
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    json_data: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Dict:
+    ...
+
+
+@overload
+async def post(
+    path: str,
+    return_format: bytes_return_types_hints,
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    json_data: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> bytes:
+    ...
+
+
+@overload
 async def post(
     path: str,
-    return_format="native",
+    return_format: str_return_types_hints,
     ignore_statuses: Optional[List] = None,
     params: Optional[Dict] = None,
     json_data: Optional[Dict] = None,
-    key: Optional[str] = None
-) -> Union[Dict, bytes]:
+    key: Optional[str] = None,
+) -> str:
+    ...
+
+
+async def post(
+    path: str,
+    return_format: all_return_types_hints = "native",
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    json_data: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Union[Dict, str, bytes]:
     """Calls :meth:`request()` for post requests.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
     return_format : `str`, optional
@@ -270,42 +413,78 @@
         Custom JSON data to be formatted into the request body
     key : `str`, optional
         API token, defaults to None (which makes it unauthenticated)
 
     Returns
     -------
     Union[Dict, bytes]
-        A ``dataclass`` if ``return_format`` is ``"native"``,
-        otherwise ``bytes``
+        A ``Dict`` if ``return_format`` is ``"native"``, otherwise ``str`` or ``bytes``
+        depending on if the return format is UTF-8 or something else.
     """
     if not ignore_statuses:
         ignore_statuses = []
     if not params:
         params = {}
 
     _, resp = await request(
         method="post",
         path=path,
         return_format=return_format,
         ignore_statuses=ignore_statuses,
         params=params,
         json_data=json_data,
-        key=key
+        key=key,
     )
     return resp
 
 
+@overload
 async def patch(
     path: str,
-    return_format="native",
+    return_format: native_return_types_hints = "native",
     ignore_statuses: Optional[List] = None,
     params: Optional[Dict] = None,
     json_data: Optional[Dict] = None,
-    key: Optional[str] = None
-) -> Union[Dict, bytes]:
+    key: Optional[str] = None,
+) -> Dict:
+    ...
+
+
+@overload
+async def patch(
+    path: str,
+    return_format: bytes_return_types_hints,
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    json_data: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> bytes:
+    ...
+
+
+@overload
+async def patch(
+    path: str,
+    return_format: str_return_types_hints,
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    json_data: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> str:
+    ...
+
+
+async def patch(
+    path: str,
+    return_format: all_return_types_hints = "native",
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    json_data: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Union[Dict, str, bytes]:
     """Calls :meth:`request()` for patch requests.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
     return_format : `str`, optional
@@ -319,42 +498,75 @@
         Custom JSON data to be formatted into the request body
     key : `str`, optional
         API token, defaults to None (which makes it unauthenticated)
 
     Returns
     -------
     Union[Dict, bytes]
-        A ``dataclass`` if ``return_format`` is ``"native"``,
-        otherwise ``bytes``
+        A ``Dict`` if ``return_format`` is ``"native"``, otherwise ``str`` or ``bytes``
+        depending on if the return format is UTF-8 or something else.
     """
 
     if not ignore_statuses:
         ignore_statuses = []
     if not params:
         params = {}
 
     _, resp = await request(
         method="patch",
         path=path,
         return_format=return_format,
         ignore_statuses=ignore_statuses,
         params=params,
         key=key,
-        json_data=json_data
+        json_data=json_data,
     )
     return resp
 
 
+@overload
+async def delete(
+    path: str,
+    return_format: native_return_types_hints = "native",
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Dict:
+    ...
+
+
+@overload
+async def delete(
+    path: str,
+    return_format: bytes_return_types_hints,
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> bytes:
+    ...
+
+
+@overload
 async def delete(
     path: str,
-    return_format="native",
+    return_format: str_return_types_hints,
     ignore_statuses: Optional[List] = None,
     params: Optional[Dict] = None,
-    key: Optional[str] = None
-) -> Union[Dict, bytes]:
+    key: Optional[str] = None,
+) -> str:
+    ...
+
+
+async def delete(
+    path: str,
+    return_format: all_return_types_hints = "native",
+    ignore_statuses: Optional[List] = None,
+    params: Optional[Dict] = None,
+    key: Optional[str] = None,
+) -> Union[Dict, str, bytes]:
     """Calls :meth:`request()` for delete requests.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
     return_format : `str`, optional
@@ -366,41 +578,41 @@
         Any other HTTP request parameters, defaults to None
     key : `str`, optional
         API token, defaults to None (which makes it unauthenticated)
 
     Returns
     -------
     Union[Dict, bytes]
-        A ``dataclass`` if ``return_format`` is ``"native"``,
-        otherwise ``bytes``
+        A ``Dict`` if ``return_format`` is ``"native"``, otherwise ``str`` or ``bytes``
+        depending on if the return format is UTF-8 or something else.
     """
 
     if not ignore_statuses:
         ignore_statuses = []
     if not params:
         params = {}
 
     _, resp = await request(
         method="delete",
         path=path,
         return_format=return_format,
         ignore_statuses=ignore_statuses,
         params=params,
-        key=key
+        key=key,
     )
     return resp
 
 
 async def getiter(
     path: str,
     limit: int = 100,
     sort: str = "created",
     ignore_statuses: Optional[List] = None,
     params: Optional[Dict] = None,
-    key: Optional[str] = None
+    key: Optional[str] = None,
 ) -> AsyncIterable[Dict]:
     """Get :meth:`request()` for paginated results.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
@@ -427,16 +639,15 @@
         ignore_statuses = []
     if not params:
         params = {}
     request_headers = {}
 
     valid_sort_orders = ["created", "updated", "popularity", "distance"]
     if sort not in valid_sort_orders:
-        raise ValueError(
-            f"sort argument must be one of {', '.join(valid_sort_orders)}")
+        raise ValueError(f"sort argument must be one of {', '.join(valid_sort_orders)}")
     else:
         params["sort"] = sort
 
     url = urljoin(url_base, path)
 
     # set auth in headers if key is provided
     if key is not None:
@@ -466,26 +677,24 @@
             headers=request_headers,
         ) as r_fpdb:
             status_handler(r_fpdb.status, ignore_statuses)
 
             # I detest responses which "may" be paginated
             # therefore I choose to pretend that all pages are paginated
             # if it is unpaginated I say it is paginated with 1 page
-            if 'X-Page-Count' in r_fpdb.headers:
-                num_pages = int(r_fpdb.headers['X-Page-Count'])
+            if "X-Page-Count" in r_fpdb.headers:
+                num_pages = int(r_fpdb.headers["X-Page-Count"])
             else:
                 num_pages = 1
 
         # while page <= num_pages...
         for page in range(0, num_pages):
-            params['page'] = page
+            params["page"] = page
             async with session.get(
-                url=url,
-                params=params,
-                headers=request_headers
+                url=url, params=params, headers=request_headers
             ) as r_fpdb:
                 status_handler(r_fpdb.status, ignore_statuses)
                 # ...keep cycling through pages...
                 for i in await r_fpdb.json():
                     # ...and return every dictionary in there...
                     yield i
                     num_results += 1
```

### Comparing `flightplandb-0.7.2/src/flightplandb/nav.py` & `flightplandb-0.8.0/src/flightplandb/nav.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Commands related to navigation aids and airports."""
 from typing import AsyncIterable, List, Optional
-from flightplandb.datatypes import Airport, Track, SearchNavaid
+
 from flightplandb import internal
+from flightplandb.datatypes import Airport, SearchNavaid, Track
 
 
 async def airport(icao: str, key: Optional[str] = None) -> Airport:
     """Fetches information about an airport.
 
     Parameters
     ----------
@@ -40,17 +41,15 @@
     Returns
     -------
     List[Track]
         List of NATs
     """
 
     return list(
-        map(
-            lambda n: Track(**n), await internal.get(path="/nav/NATS", key=key)
-        )
+        map(lambda n: Track(**n), await internal.get(path="/nav/NATS", key=key))
     )
 
 
 async def pacots(key: Optional[str] = None) -> List[Track]:
     """Fetches current Pacific Organized Track System tracks.
 
     Parameters
@@ -61,26 +60,21 @@
     Returns
     -------
     List[Track]
         List of PACOTs
     """
 
     return list(
-        map(
-            lambda t: Track(**t), await internal.get(
-                path="/nav/PACOTS", key=key
-            )
-        )
+        map(lambda t: Track(**t), await internal.get(path="/nav/PACOTS", key=key))
     )
 
 
 async def search(
-        query: str,
-        type_: Optional[str] = None, key: Optional[str] = None
-        ) -> AsyncIterable[SearchNavaid]:
+    query: str, type_: Optional[str] = None, key: Optional[str] = None
+) -> AsyncIterable[SearchNavaid]:
     r"""Searches navaids using a query.
 
     Parameters
     ----------
     query : str
         The search query. Searches the navaid identifier and navaid name
     type\_ : `str`, optional
@@ -99,11 +93,9 @@
 
     params = {"q": query}
     if type_:
         if type_ in SearchNavaid.validtypes:
             params["types"] = type_
         else:
             raise ValueError(f"{type_} is not a valid Navaid type")
-    async for i in internal.getiter(
-        path="/search/nav", params=params, key=key
-    ):
+    async for i in internal.getiter(path="/search/nav", params=params, key=key):
         yield SearchNavaid(**i)
```

### Comparing `flightplandb-0.7.2/src/flightplandb/plan.py` & `flightplandb-0.8.0/src/flightplandb/plan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,44 @@
 """Flightplan-related commands."""
-from typing import AsyncIterable, Union, Optional
-from flightplandb.datatypes import (
-    StatusResponse, PlanQuery,
-    Plan, GenerateQuery
-)
+from typing import AsyncIterable, Dict, Optional, Union, overload
+
 from flightplandb import internal
+from flightplandb.datatypes import GenerateQuery, Plan, PlanQuery, StatusResponse
+
+
+@overload
+async def fetch(
+    id_: int,
+    return_format: internal.native_return_types_hints = "native",
+    key: Optional[str] = None,
+) -> Plan:
+    ...
 
 
+@overload
 async def fetch(
     id_: int,
-    return_format: str = "native",
-    key: Optional[str] = None
-) -> Union[Plan, None, bytes]:
+    return_format: internal.bytes_return_types_hints,
+    key: Optional[str] = None,
+) -> bytes:
+    ...
+
+
+@overload
+async def fetch(
+    id_: int, return_format: internal.str_return_types_hints, key: Optional[str] = None
+) -> str:
+    ...
+
+
+async def fetch(
+    id_: int,
+    return_format: internal.all_return_types_hints = "native",
+    key: Optional[str] = None,
+) -> Union[Plan, Dict, str, bytes]:
     # Underscore for id_ must be escaped as id\_ so sphinx shows the _.
     # However, this would raise W605. To fix this, a raw string is used.
     r"""
     Fetches a flight plan and its associated attributes by ID.
     Returns it in specified format.
 
     Parameters
@@ -26,43 +49,70 @@
         The API response format, defaults to ``"native"``.
         Must be one of the keys in the :ref:`permitted-return-types`.
     key : `str`, optional
         API authentication key.
 
     Returns
     -------
-    Union[Plan, None, bytes]
-        :class:`~flightplandb.datatypes.Plan` by default or if ``"native"``
-        is specified as the ``return_format``.
+    Union[Plan, Dict, bytes, str]
+        :class:`~flightplandb.datatypes.Plan` of the specified plan
+        if ``"native"`` is specified as the ``return_format`` (default).
+
+        ``bytes`` if PDF was specified as the ``return_format``.
 
-        ``bytes`` if a different format than ``"native"`` was specified.
+        ``str`` if a different ``return_format`` was specified.
 
     Raises
     ------
     :class:`~flightplandb.exceptions.NotFoundException`
         No plan with the specified id was found.
     """
 
     request = await internal.get(
-        path=f"/plan/{id_}",
-        return_format=return_format,
-        key=key
+        path=f"/plan/{id_}", return_format=return_format, key=key
     )
 
-    if return_format == "native":
+    if isinstance(request, dict) and return_format in internal.native_return_values:
         return Plan(**request)
+    else:
+        return request
 
-    return request  # if the format is not a dict
+
+@overload
+async def create(
+    plan: Plan,
+    return_format: internal.native_return_types_hints = "native",
+    key: Optional[str] = None,
+) -> Plan:
+    ...
+
+
+@overload
+async def create(
+    plan: Plan,
+    return_format: internal.bytes_return_types_hints,
+    key: Optional[str] = None,
+) -> bytes:
+    ...
 
 
+@overload
 async def create(
     plan: Plan,
-    return_format: str = "native",
-    key: Optional[str] = None
-) -> Union[Plan, bytes]:
+    return_format: internal.str_return_types_hints,
+    key: Optional[str] = None,
+) -> str:
+    ...
+
+
+async def create(
+    plan: Plan,
+    return_format: internal.all_return_types_hints = "native",
+    key: Optional[str] = None,
+) -> Union[Plan, Dict, bytes, str]:
     """Creates a new flight plan.
 
     Requires authentication.
 
     Parameters
     ----------
     plan : Plan
@@ -71,41 +121,75 @@
         The API response format, defaults to ``"native"``.
         Must be one of the keys in the :ref:`permitted-return-types`.
     key : `str`, optional
         API authentication key.
 
     Returns
     -------
-    Plan
-        The registered flight plan created on flight plan database
+    Union[Plan, Dict, bytes, str]
+        :class:`~flightplandb.datatypes.Plan` of the registered plan
+        created on Flight Plan Database if ``"native"`` is specified
+        as the ``return_format`` (default).
+
+        ``bytes`` if PDF was specified as the ``return_format``.
+
+        ``str`` if a different ``return_format`` was specified.
 
     Raises
     ------
     :class:`~flightplandb.exceptions.BadRequestException`
         The plan submitted had incorrect arguments or was
         otherwise unusable.
     """
 
     request = await internal.post(
         path="/plan/",
         return_format=return_format,
         json_data=plan.to_api_dict(),
-        key=key)
+        key=key,
+    )
 
-    if return_format == "native":
+    if isinstance(request, dict) and return_format in internal.native_return_values:
         return Plan(**request)
+    else:
+        return request
 
-    return request
+
+@overload
+async def edit(
+    plan: Plan,
+    return_format: internal.native_return_types_hints = "native",
+    key: Optional[str] = None,
+) -> Plan:
+    ...
 
 
+@overload
 async def edit(
     plan: Plan,
-    return_format: str = "native",
-    key: Optional[str] = None
-) -> Union[Plan, bytes]:
+    return_format: internal.bytes_return_types_hints,
+    key: Optional[str] = None,
+) -> bytes:
+    ...
+
+
+@overload
+async def edit(
+    plan: Plan,
+    return_format: internal.str_return_types_hints,
+    key: Optional[str] = None,
+) -> str:
+    ...
+
+
+async def edit(
+    plan: Plan,
+    return_format: internal.all_return_types_hints = "native",
+    key: Optional[str] = None,
+) -> Union[Plan, Dict, bytes, str]:
     """Edits a flight plan linked to your account.
 
     Requires authentication.
 
     Parameters
     ----------
     plan : Plan
@@ -114,17 +198,23 @@
         The API response format, defaults to ``"native"``.
         Must be one of the keys in the :ref:`permitted-return-types`.
     key : `str`, optional
         API authentication key.
 
     Returns
     -------
-    Plan
-        The registered flight plan created on flight plan database,
-        corresponding to the route after being edited
+    Union[Plan, Dict, bytes, str]
+        :class:`~flightplandb.datatypes.Plan` of the registered flight
+        plan created on flight plan database, corresponding to the
+        route after being edited if ``"native"`` is specified
+        as the ``return_format`` (default).
+
+        ``bytes`` if PDF was specified as the ``return_format``.
+
+        ``str`` if a different ``return_format`` was specified.
 
     Raises
     ------
     :class:`~flightplandb.exceptions.BadRequestException`
         The plan submitted had incorrect arguments
         or was otherwise unusable.
     :class:`~flightplandb.exceptions.NotFoundException`
@@ -132,26 +222,26 @@
     """
 
     plan_data = plan.to_api_dict()
     request = await internal.patch(
         path=f"/plan/{plan_data['id']}",
         return_format=return_format,
         json_data=plan_data,
-        key=key)
+        key=key,
+    )
 
-    if return_format == "native":
+    if isinstance(request, dict) and return_format in internal.native_return_values:
         return Plan(**request)
+    else:
+        return request
 
     return request
 
 
-async def delete(
-    id_: int,
-    key: Optional[str] = None
-) -> StatusResponse:
+async def delete(id_: int, key: Optional[str] = None) -> StatusResponse:
     r"""Deletes a flight plan that is linked to your account.
 
     Requires authentication.
 
     Parameters
     ----------
     id\_ : int
@@ -173,17 +263,17 @@
     resp = await internal.delete(path=f"/plan/{id_}", key=key)
     return StatusResponse(**resp)
 
 
 async def search(
     plan_query: PlanQuery,
     sort: str = "created",
-    include_route: bool = False,
+    include_route: Optional[bool] = False,
     limit: int = 100,
-    key: Optional[str] = None
+    key: Optional[str] = None,
 ) -> AsyncIterable[Plan]:
     """Searches for flight plans.
     A number of search parameters are available.
     They will be combined to form a search request.
 
     Requires authentication if route is included in results
 
@@ -192,15 +282,15 @@
     plan_query : PlanQuery
         A dataclass containing multiple options for plan searches
     sort : str
         Sort order to return results in. Valid sort orders are
         created, updated, popularity, and distance
     limit : int
         Maximum number of plans to return, defaults to 100
-    include_route : bool
+    include_route : bool, optional
         Include route in response, defaults to False
     key : `str`, optional
         API authentication key.
 
     Yields
     -------
     AsyncIterable[Plan]
@@ -208,27 +298,20 @@
         objects.
     """
 
     request_json = plan_query.to_api_dict()
     request_json["includeRoute"] = include_route
 
     async for i in internal.getiter(
-        path="/search/plans",
-        sort=sort,
-        params=request_json,
-        limit=limit,
-        key=key
+        path="/search/plans", sort=sort, params=request_json, limit=limit, key=key
     ):
         yield Plan(**i)
 
 
-async def has_liked(
-    id_: int,
-    key: Optional[str] = None
-) -> bool:
+async def has_liked(id_: int, key: Optional[str] = None) -> bool:
     r"""Fetches your like status for a flight plan.
 
     Requires authentication.
 
     Parameters
     ----------
     id\_ : int
@@ -238,27 +321,20 @@
 
     Returns
     -------
     bool
         ``True``/``False`` to indicate that the plan was liked / not liked
     """
 
-    resp = await internal.get(
-        path=f"/plan/{id_}/like",
-        ignore_statuses=[404],
-        key=key
-    )
+    resp = await internal.get(path=f"/plan/{id_}/like", ignore_statuses=[404], key=key)
     status_response = StatusResponse(**resp)
     return status_response.message != "Not Found"
 
 
-async def like(
-    id_: int,
-    key: Optional[str] = None
-) -> StatusResponse:
+async def like(id_: int, key: Optional[str] = None) -> StatusResponse:
     r"""Likes a flight plan.
 
     Requires authentication.
 
     Parameters
     ----------
     id\_ : int
@@ -278,18 +354,15 @@
         No plan with the specified id was found.
     """
 
     resp = await internal.post(path=f"/plan/{id_}/like", key=key)
     return StatusResponse(**resp)
 
 
-async def unlike(
-    id_: int,
-    key: Optional[str] = None
-) -> bool:
+async def unlike(id_: int, key: Optional[str] = None) -> bool:
     r"""Removes a flight plan like.
 
     Requires authentication.
 
     Parameters
     ----------
     id\_ : int
@@ -311,56 +384,47 @@
 
     await internal.delete(path=f"/plan/{id_}/like", key=key)
     return True
 
 
 async def generate(
     gen_query: GenerateQuery,
-    include_route: bool = False,
-    key: Optional[str] = None
-) -> Union[Plan, bytes]:
+    include_route: Optional[bool] = False,
+    key: Optional[str] = None,
+) -> Plan:
     """Creates a new flight plan using the route generator.
 
     Requires authentication.
 
     Parameters
     ----------
     gen_query : GenerateQuery
         A dataclass with options for flight plan generation
-    include_route : bool
+    include_route : bool, optional
         Include route in response, defaults to False
     key : `str`, optional
         API authentication key.
 
     Returns
     -------
     Plan
         The registered flight plan created on flight plan database,
         corresponding to the generated route
-    include_route : bool, optional
-        Include route in response, defaults to false
     """
 
     request_json = gen_query.to_api_dict()
 
     # due to an API bug this must be a string instead of a boolean
     request_json["includeRoute"] = "true" if include_route else "false"
 
-    resp = await internal.post(
-        path="/auto/generate",
-        json_data=request_json,
-        key=key
-    )
+    resp = await internal.post(path="/auto/generate", json_data=request_json, key=key)
     return Plan(**resp)
 
 
-async def decode(
-    route: str,
-    key: Optional[str] = None
-) -> Plan:
+async def decode(route: str, key: Optional[str] = None) -> Plan:
     """Creates a new flight plan using the route decoder.
 
     Requires authentication.
 
     Parameters
     ----------
     route : str
@@ -383,10 +447,9 @@
     Raises
     ------
     :class:`~flightplandb.exceptions.BadRequestException`
         The encoded plan submitted had incorrect
         arguments or was otherwise unusable.
     """
 
-    resp = await internal.post(
-        path="/auto/decode", json_data={"route": route}, key=key)
+    resp = await internal.post(path="/auto/decode", json_data={"route": route}, key=key)
     return Plan(**resp)
```

### Comparing `flightplandb-0.7.2/src/flightplandb/tags.py` & `flightplandb-0.8.0/src/flightplandb/tags.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Contains the command for fetching flight plan tags."""
 from typing import List, Optional
-from flightplandb.datatypes import Tag
+
 from flightplandb import internal
+from flightplandb.datatypes import Tag
 
 
 async def fetch(key: Optional[str] = None) -> List[Tag]:
     """Fetches current popular tags from all flight plans.
     Only tags with sufficient popularity are included.
 
     Parameters
@@ -15,10 +16,8 @@
 
     Returns
     ----------
     List[Tag]
         A list of the current popular tags.
     """
 
-    return list(
-        map(lambda t: Tag(**t), await internal.get(path="/tags", key=key))
-    )
+    return list(map(lambda t: Tag(**t), await internal.get(path="/tags", key=key)))
```

### Comparing `flightplandb-0.7.2/src/flightplandb/user.py` & `flightplandb-0.8.0/src/flightplandb/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Commands related to registered users."""
 from typing import AsyncIterable, Optional
-from flightplandb.datatypes import Plan, User, UserSmall
+
 from flightplandb import internal
+from flightplandb.datatypes import Plan, User, UserSmall
 
 
 async def me(key: Optional[str] = None) -> User:
     """Fetches profile information for the currently authenticated user.
 
     Requires authentication.
 
@@ -51,18 +52,15 @@
     """
 
     resp = await internal.get(path=f"/user/{username}", key=key)
     return User(**resp)
 
 
 async def plans(
-    username: str,
-    sort: str = "created",
-    limit: int = 100,
-    key: Optional[str] = None
+    username: str, sort: str = "created", limit: int = 100, key: Optional[str] = None
 ) -> AsyncIterable[Plan]:
     """Fetches flight plans created by a user.
 
     Parameters
     ----------
     username : str
         Username of the user who created the flight plans
@@ -77,27 +75,21 @@
     Yields
     -------
     AsyncIterable[Plan]
         An iterator with all the flight plans a user created,
         limited by ``limit``
     """
     async for i in internal.getiter(
-        path=f"/user/{username}/plans",
-        sort=sort,
-        limit=limit,
-        key=key
+        path=f"/user/{username}/plans", sort=sort, limit=limit, key=key
     ):
         yield Plan(**i)
 
 
 async def likes(
-    username: str,
-    sort: str = "created",
-    limit: int = 100,
-    key: Optional[str] = None
+    username: str, sort: str = "created", limit: int = 100, key: Optional[str] = None
 ) -> AsyncIterable[Plan]:
     """Fetches flight plans liked by a user.
 
     Parameters
     ----------
     username : str
         Username of the user who liked the flight plans
@@ -113,26 +105,21 @@
     -------
     AsyncIterable[Plan]
         An iterable with all the flight plans a user liked,
         limited by ``limit``
     """
 
     async for i in internal.getiter(
-        path=f"/user/{username}/likes",
-        sort=sort,
-        limit=limit,
-        key=key
+        path=f"/user/{username}/likes", sort=sort, limit=limit, key=key
     ):
         yield Plan(**i)
 
 
 async def search(
-    username: str,
-    limit=100,
-    key: Optional[str] = None
+    username: str, limit=100, key: Optional[str] = None
 ) -> AsyncIterable[UserSmall]:
     """Searches for users by username. For more detailed info on a
     specific user, use :meth:`fetch`
 
     Parameters
     ----------
     username : str
@@ -147,13 +134,10 @@
     AsyncIterable[UserSmall]
         An iterable with a list of users approximately matching
         ``username``, limited by ``limit``. UserSmall is used instead of
         User, because less info is returned.
     """
 
     async for i in internal.getiter(
-        path="/search/users",
-        limit=limit,
-        params={"q": username},
-        key=key
+        path="/search/users", limit=limit, params={"q": username}, key=key
     ):
         yield UserSmall(**i)
```

### Comparing `flightplandb-0.7.2/src/flightplandb/weather.py` & `flightplandb-0.8.0/src/flightplandb/weather.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Weather. I mean, how much is there to say?"""
 from typing import Optional
-from flightplandb.datatypes import Weather
+
 from flightplandb import internal
+from flightplandb.datatypes import Weather
 
 
 async def fetch(icao: str, key: Optional[str] = None) -> Weather:
     """
     Fetches current weather conditions at an airport
 
     Parameters
```

### Comparing `flightplandb-0.7.2/src/flightplandb.egg-info/PKG-INFO` & `flightplandb-0.8.0/src/flightplandb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightplandb
-Version: 0.7.2
+Version: 0.8.0
 Summary: Python wrapper for the Flight Plan Database API
 Author-email: PH-KDX <smtp.python.email.sender@gmail.com>
 License: GPL v3
 Project-URL: Homepage, https://github.com/PH-KDX/flightplandb-py/
 Project-URL: Documentation, https://flightplandb-py.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/PH-KDX/flightplandb-py/issues
 Project-URL: Changelog, https://github.com/PH-KDX/flightplandb-py/blob/main/CHANGELOG.rst
@@ -22,24 +22,26 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Games/Entertainment :: Simulation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/PH-KDX/flightplandb-py/main/artwork/png/240x240.png" alt="FlightPlanDB-py logo">
 </p>
 
 # FlightplanDB-py
 
 ## Project status
-![Unittests and lint](https://github.com/PH-KDX/flightplandb-py/actions/workflows/test_and_lint.yml/badge.svg)
+![Unittests and lint](https://github.com/PH-KDX/flightplandb-py/actions/workflows/test.yml/badge.svg)
+![Lint](https://github.com/PH-KDX/flightplandb-py/actions/workflows/lint.yml/badge.svg)
 [![PyPi](https://img.shields.io/pypi/v/flightplandb.svg)](https://pypi.org/project/flightplandb/)
 ![Python](https://img.shields.io/pypi/pyversions/flightplandb.svg)
 
 ## Introduction
 This is a Python 3 wrapper for the [Flight Plan Database API](https://flightplandatabase.com/dev/api). Flight Plan Database is a website for creating and sharing flight plans for use in flight simulation.
 
 For more information on Flight Plan Database, see their excellent [About page](https://flightplandatabase.com/about).
```

### Comparing `flightplandb-0.7.2/src/flightplandb.egg-info/SOURCES.txt` & `flightplandb-0.8.0/src/flightplandb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yaml
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+.github/workflows/lint.yml
 .github/workflows/release.yml
-.github/workflows/test_and_lint.yml
+.github/workflows/test.yml
 artwork/ico/favicon.ico
 artwork/png/120x120.png
 artwork/png/240x240.png
 artwork/png/32x32.png
 artwork/png/480x480.png
 artwork/svg/logo.svg
 docs/Makefile
@@ -34,14 +36,15 @@
 src/flightplandb/__init__.py
 src/flightplandb/api.py
 src/flightplandb/datatypes.py
 src/flightplandb/exceptions.py
 src/flightplandb/internal.py
 src/flightplandb/nav.py
 src/flightplandb/plan.py
+src/flightplandb/py.typed
 src/flightplandb/tags.py
 src/flightplandb/user.py
 src/flightplandb/weather.py
 src/flightplandb.egg-info/PKG-INFO
 src/flightplandb.egg-info/SOURCES.txt
 src/flightplandb.egg-info/dependency_links.txt
 src/flightplandb.egg-info/requires.txt
```

### Comparing `flightplandb-0.7.2/tests/test_api.py` & `flightplandb-0.8.0/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,144 +1,122 @@
 from unittest import mock
+
 import pytest
+
 import flightplandb
 from flightplandb.datatypes import StatusResponse
 
 
 # parametrise this for key and no key, perhaps
 # localhost is set on every test to allow async loops
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get_headers")
 async def test_api_header_value(patched_get_headers):
-    json_response = {
-        "X-Limit-Cap": "2000",
-        "X-Limit-Used": "150"
-    }
+    json_response = {"X-Limit-Cap": "2000", "X-Limit-Used": "150"}
 
     correct_response = "150"
 
     patched_get_headers.return_value = json_response
 
     response = await flightplandb.api.header_value(
-        header_key="X-Limit-Used",
-        key="qwertyuiop"
+        header_key="X-Limit-Used", key="qwertyuiop"
     )
     # check that API method made correct request of FlightPlanDB
-    patched_get_headers.assert_awaited_once_with(
-        key="qwertyuiop"
-    )
+    patched_get_headers.assert_awaited_once_with(key="qwertyuiop")
     # check that API method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.api.header_value")
 async def test_api_version(patched_header_value):
     header_response = "1"
 
     correct_response = 1
 
     patched_header_value.return_value = header_response
 
     response = await flightplandb.api.version()
     # check that API method made correct request of FlightPlanDB
-    patched_header_value.assert_awaited_once_with(
-        header_key="X-API-Version", key=None
-    )
+    patched_header_value.assert_awaited_once_with(header_key="X-API-Version", key=None)
     # check that API method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.api.header_value")
 async def test_api_units(patched_header_value):
     header_response = "AVIATION"
 
     correct_response = "AVIATION"
 
     patched_header_value.return_value = header_response
 
     response = await flightplandb.api.units()
     # check that API method made correct request of FlightPlanDB
-    patched_header_value.assert_awaited_once_with(
-        header_key="X-Units", key=None
-    )
+    patched_header_value.assert_awaited_once_with(header_key="X-Units", key=None)
     # check that API method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.api.header_value")
 async def test_api_limit_cap(patched_header_value):
     header_response = "100"
 
     correct_response = 100
 
     patched_header_value.return_value = header_response
 
     response = await flightplandb.api.limit_cap()
     # check that API method made correct request of FlightPlanDB
-    patched_header_value.assert_awaited_once_with(
-        header_key="X-Limit-Cap", key=None
-    )
+    patched_header_value.assert_awaited_once_with(header_key="X-Limit-Cap", key=None)
     # check that API method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.api.header_value")
 async def test_api_limit_used(patched_header_value):
     header_response = "50"
 
     correct_response = 50
 
     patched_header_value.return_value = header_response
 
     response = await flightplandb.api.limit_used()
     # check that API method made correct request of FlightPlanDB
-    patched_header_value.assert_awaited_once_with(
-        header_key="X-Limit-Used", key=None
-    )
+    patched_header_value.assert_awaited_once_with(header_key="X-Limit-Used", key=None)
     # check that API method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_api_ping(patched_internal_get):
-    json_response = {
-        "message": "OK",
-        "errors": None
-        }
+    json_response = {"message": "OK", "errors": None}
 
     correct_response = StatusResponse(message="OK", errors=None)
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.api.ping()
     # check that API method made correct request of FlightPlanDB
-    patched_internal_get.assert_awaited_once_with(
-        path='', key=None
-    )
+    patched_internal_get.assert_awaited_once_with(path="", key=None)
     # check that API method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_key_revoke(patched_internal_get):
-    json_response = {
-        "message": "OK",
-        "errors": None
-        }
+    json_response = {"message": "OK", "errors": None}
 
     correct_response = StatusResponse(message="OK", errors=None)
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.api.revoke(key="qwertyuiop")
     # check that API method made correct request of FlightPlanDB
-    patched_internal_get.assert_awaited_once_with(
-        path='/auth/revoke', key="qwertyuiop"
-    )
+    patched_internal_get.assert_awaited_once_with(path="/auth/revoke", key="qwertyuiop")
     # check that API method decoded data correctly for given response
     assert response == correct_response
```

### Comparing `flightplandb-0.7.2/tests/test_nav.py` & `flightplandb-0.8.0/tests/test_nav.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,495 +1,493 @@
+import datetime
 from unittest import mock
+
 import pytest
+from dateutil.tz import tzutc
+
 import flightplandb
 from flightplandb.datatypes import (
-    Airport, Timezone, Runway, RunwayEnds,
-    Frequency, Weather, Times, Track,
-    Route, RouteNode, SearchNavaid
+    Airport,
+    Frequency,
+    Route,
+    RouteNode,
+    Runway,
+    RunwayEnds,
+    SearchNavaid,
+    Times,
+    Timezone,
+    Track,
+    Weather,
 )
-import datetime
-from dateutil.tz import tzutc
 
 
 class AsyncIter:
     def __init__(self, items):
         self.items = items
 
     async def __aiter__(self):
         for item in self.items:
             yield item
 
 
 # localhost is set on every test to allow async loops
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_airport_info(patched_internal_get):
     json_response = {
-        'ICAO': 'EHAL',
-        'IATA': None,
-        'name': 'Ameland',
-        'regionName': 'Netherlands',
-        'elevation': 11.00000001672,
-        'lat': 53.4536,
-        'lon': 5.67869,
-        'magneticVariation': 1.8677087306751243,
-        'timezone': {
-            'name': 'Europe/Amsterdam',
-            'offset': 7200},
-        'times': {
-            'sunrise': '2021-04-26T04:14:10.584Z',
-            'sunset': '2021-04-26T18:58:16.572Z',
-            'dawn': '2021-04-26T03:34:40.249Z',
-            'dusk': '2021-04-26T19:37:46.907Z'},
-        'runwayCount': 1,
-        'runways': [
+        "ICAO": "EHAL",
+        "IATA": None,
+        "name": "Ameland",
+        "regionName": "Netherlands",
+        "elevation": 11.00000001672,
+        "lat": 53.4536,
+        "lon": 5.67869,
+        "magneticVariation": 1.8677087306751243,
+        "timezone": {"name": "Europe/Amsterdam", "offset": 7200},
+        "times": {
+            "sunrise": "2021-04-26T04:14:10.584Z",
+            "sunset": "2021-04-26T18:58:16.572Z",
+            "dawn": "2021-04-26T03:34:40.249Z",
+            "dusk": "2021-04-26T19:37:46.907Z",
+        },
+        "runwayCount": 1,
+        "runways": [
             {
-                'ident': '08',
-                'width': 97.998687813,
-                'length': 2627.1784816836002,
-                'bearing': 87.4099,
-                'surface': 'GRASS',
-                'markings': ['VISUAL'],
-                'lighting': [''],
-                'thresholdOffset': 0,
-                'overrunLength': 0,
-                'ends': [
-                    {
-                        'ident': '08',
-                        'lat': 53.4534,
-                        'lon': 5.67265},
-                    {
-                        'ident': '26',
-                        'lat': 53.4534,
-                        'lon': 53.4538}],
-                'navaids': []},
-            {
-                'ident': '26',
-                'width': 97.998687813,
-                'length': 2627.1784816836002,
-                'bearing': 267.42,
-                'surface': 'GRASS',
-                'markings': ['NONE'],
-                'lighting': [''],
-                'thresholdOffset': 0,
-                'overrunLength': 0,
-                'ends': [
-                    {
-                        'ident': '26',
-                        'lat': 53.4538,
-                        'lon': 5.68473},
-                    {
-                        'ident': '08',
-                        'lat': 53.4538,
-                        'lon': 53.4534}],
-                'navaids': []}],
-        'frequencies': [
+                "ident": "08",
+                "width": 97.998687813,
+                "length": 2627.1784816836002,
+                "bearing": 87.4099,
+                "surface": "GRASS",
+                "markings": ["VISUAL"],
+                "lighting": [""],
+                "thresholdOffset": 0,
+                "overrunLength": 0,
+                "ends": [
+                    {"ident": "08", "lat": 53.4534, "lon": 5.67265},
+                    {"ident": "26", "lat": 53.4534, "lon": 53.4538},
+                ],
+                "navaids": [],
+            },
             {
-                'type': 'TWR',
-                'frequency': 118350000,
-                'name': 'Ameland Radio'}],
-        'weather': {
-            'METAR': None,
-            'TAF': None}}
+                "ident": "26",
+                "width": 97.998687813,
+                "length": 2627.1784816836002,
+                "bearing": 267.42,
+                "surface": "GRASS",
+                "markings": ["NONE"],
+                "lighting": [""],
+                "thresholdOffset": 0,
+                "overrunLength": 0,
+                "ends": [
+                    {"ident": "26", "lat": 53.4538, "lon": 5.68473},
+                    {"ident": "08", "lat": 53.4538, "lon": 53.4534},
+                ],
+                "navaids": [],
+            },
+        ],
+        "frequencies": [
+            {"type": "TWR", "frequency": 118350000, "name": "Ameland Radio"}
+        ],
+        "weather": {"METAR": None, "TAF": None},
+    }
 
     correct_response = Airport(
-        ICAO='EHAL',
+        ICAO="EHAL",
         IATA=None,
-        name='Ameland',
-        regionName='Netherlands',
+        name="Ameland",
+        regionName="Netherlands",
         elevation=11.00000001672,
         lat=53.4536,
         lon=5.67869,
         magneticVariation=1.8677087306751243,
-        timezone=Timezone(
-            name='Europe/Amsterdam',
-            offset=7200),
+        timezone=Timezone(name="Europe/Amsterdam", offset=7200),
         times=Times(
-            sunrise=datetime.datetime(
-                2021, 4, 26, 4, 14, 10, 584000, tzinfo=tzutc()),
-            sunset=datetime.datetime(
-                2021, 4, 26, 18, 58, 16, 572000, tzinfo=tzutc()),
-            dawn=datetime.datetime(
-                2021, 4, 26, 3, 34, 40, 249000, tzinfo=tzutc()),
-            dusk=datetime.datetime(
-                2021, 4, 26, 19, 37, 46, 907000, tzinfo=tzutc())),
+            sunrise=datetime.datetime(2021, 4, 26, 4, 14, 10, 584000, tzinfo=tzutc()),
+            sunset=datetime.datetime(2021, 4, 26, 18, 58, 16, 572000, tzinfo=tzutc()),
+            dawn=datetime.datetime(2021, 4, 26, 3, 34, 40, 249000, tzinfo=tzutc()),
+            dusk=datetime.datetime(2021, 4, 26, 19, 37, 46, 907000, tzinfo=tzutc()),
+        ),
         runwayCount=1,
         runways=[
             Runway(
-                ident='08',
+                ident="08",
                 width=97.998687813,
                 length=2627.1784816836002,
                 bearing=87.4099,
-                surface='GRASS',
-                markings=['VISUAL'],
-                lighting=[''],
+                surface="GRASS",
+                markings=["VISUAL"],
+                lighting=[""],
                 thresholdOffset=0,
                 overrunLength=0,
                 ends=[
-                    RunwayEnds(
-                        ident='08',
-                        lat=53.4534,
-                        lon=5.67265),
-                    RunwayEnds(
-                        ident='26',
-                        lat=53.4534,
-                        lon=53.4538)],
-                navaids=[]),
+                    RunwayEnds(ident="08", lat=53.4534, lon=5.67265),
+                    RunwayEnds(ident="26", lat=53.4534, lon=53.4538),
+                ],
+                navaids=[],
+            ),
             Runway(
-                ident='26',
+                ident="26",
                 width=97.998687813,
                 length=2627.1784816836002,
                 bearing=267.42,
-                surface='GRASS',
-                markings=['NONE'],
-                lighting=[''],
+                surface="GRASS",
+                markings=["NONE"],
+                lighting=[""],
                 thresholdOffset=0,
                 overrunLength=0,
                 ends=[
-                    RunwayEnds(
-                        ident='26',
-                        lat=53.4538,
-                        lon=5.68473),
-                    RunwayEnds(
-                        ident='08',
-                        lat=53.4538,
-                        lon=53.4534)],
-                navaids=[])],
-        frequencies=[
-            Frequency(
-                type='TWR',
-                frequency=118350000,
-                name='Ameland Radio'
-            )
+                    RunwayEnds(ident="26", lat=53.4538, lon=5.68473),
+                    RunwayEnds(ident="08", lat=53.4538, lon=53.4534),
+                ],
+                navaids=[],
+            ),
         ],
-        weather=Weather(
-            METAR=None,
-            TAF=None
-        )
+        frequencies=[Frequency(type="TWR", frequency=118350000, name="Ameland Radio")],
+        weather=Weather(METAR=None, TAF=None),
     )
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.nav.airport("EHAL")
     # check that NavAPI method decoded data correctly for given response
     assert response == correct_response
     # check that NavAPI method made correct request of FlightPlanDB
-    patched_internal_get.assert_awaited_once_with(
-        path='/nav/airport/EHAL', key=None
-    )
+    patched_internal_get.assert_awaited_once_with(path="/nav/airport/EHAL", key=None)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_nats(patched_internal_get):
     json_response = [
         {
-            'ident': 'A',
-            'route': {
-                'eastLevels': [],
-                'nodes': [
-                    {
-                        'id': 8465100,
-                        'ident': 'RESNO',
-                        'lat': 55,
-                        'lon': -15,
-                        'type': 'FIX'
-                    },
-                    {
-                        'id': 243738,
-                        'ident': '55/20',
-                        'lat': 55,
-                        'lon': -20,
-                        'type': 'LATLON'
-                    },
-                    {
-                        'id': 243581,
-                        'ident': '54/30',
-                        'lat': 54,
-                        'lon': -30,
-                        'type': 'LATLON'
-                    },
-                    {
-                        'id': 243584,
-                        'ident': '53/40',
-                        'lat': 53,
-                        'lon': -40,
-                        'type': 'LATLON'
-                    },
-                    {
-                        'id': 243583,
-                        'ident': '52/50',
-                        'lat': 52,
-                        'lon': -50,
-                        'type': 'LATLON'
-                    },
-                    {
-                        'id': 8423845,
-                        'ident': 'TUDEP',
-                        'lat': 51.1667,
-                        'lon': -53.2333,
-                        'type': 'FIX'
-                    }
+            "ident": "A",
+            "route": {
+                "eastLevels": [],
+                "nodes": [
+                    {
+                        "id": 8465100,
+                        "ident": "RESNO",
+                        "lat": 55,
+                        "lon": -15,
+                        "type": "FIX",
+                    },
+                    {
+                        "id": 243738,
+                        "ident": "55/20",
+                        "lat": 55,
+                        "lon": -20,
+                        "type": "LATLON",
+                    },
+                    {
+                        "id": 243581,
+                        "ident": "54/30",
+                        "lat": 54,
+                        "lon": -30,
+                        "type": "LATLON",
+                    },
+                    {
+                        "id": 243584,
+                        "ident": "53/40",
+                        "lat": 53,
+                        "lon": -40,
+                        "type": "LATLON",
+                    },
+                    {
+                        "id": 243583,
+                        "ident": "52/50",
+                        "lat": 52,
+                        "lon": -50,
+                        "type": "LATLON",
+                    },
+                    {
+                        "id": 8423845,
+                        "ident": "TUDEP",
+                        "lat": 51.1667,
+                        "lon": -53.2333,
+                        "type": "FIX",
+                    },
                 ],
-                'westLevels': ['350', '370', '390']},
-            'validFrom': '2021-04-28T11:30:00.000Z',
-            'validTo': '2021-04-28T19:00:00.000Z'}]
+                "westLevels": ["350", "370", "390"],
+            },
+            "validFrom": "2021-04-28T11:30:00.000Z",
+            "validTo": "2021-04-28T19:00:00.000Z",
+        }
+    ]
 
     correct_response = [
         Track(
-            ident='A',
+            ident="A",
             route=Route(
                 nodes=[
                     RouteNode(
-                        ident='RESNO',
-                        type='FIX',
+                        ident="RESNO",
+                        type="FIX",
                         lat=55,
                         lon=-15,
                         id=8465100,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='55/20',
-                        type='LATLON',
+                        ident="55/20",
+                        type="LATLON",
                         lat=55,
                         lon=-20,
                         id=243738,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='54/30',
-                        type='LATLON',
+                        ident="54/30",
+                        type="LATLON",
                         lat=54,
                         lon=-30,
                         id=243581,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='53/40',
-                        type='LATLON',
+                        ident="53/40",
+                        type="LATLON",
                         lat=53,
                         lon=-40,
                         id=243584,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='52/50',
-                        type='LATLON',
+                        ident="52/50",
+                        type="LATLON",
                         lat=52,
                         lon=-50,
                         id=243583,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='TUDEP',
-                        type='FIX',
+                        ident="TUDEP",
+                        type="FIX",
                         lat=51.1667,
                         lon=-53.2333,
                         id=8423845,
                         alt=None,
                         name=None,
-                        via=None)],
+                        via=None,
+                    ),
+                ],
                 eastLevels=[],
-                westLevels=['350', '370', '390']),
-            validFrom=datetime.datetime(
-                2021, 4, 28, 11, 30, tzinfo=tzutc()),
-            validTo=datetime.datetime(
-                2021, 4, 28, 19, 0, tzinfo=tzutc()))]
+                westLevels=["350", "370", "390"],
+            ),
+            validFrom=datetime.datetime(2021, 4, 28, 11, 30, tzinfo=tzutc()),
+            validTo=datetime.datetime(2021, 4, 28, 19, 0, tzinfo=tzutc()),
+        )
+    ]
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.nav.nats()
     # check that NavAPI method decoded data correctly for given response
     assert response == correct_response
     # check that NavAPI method made correct request of FlightPlanDB
-    patched_internal_get.assert_awaited_once_with(
-        path='/nav/NATS', key=None
-    )
+    patched_internal_get.assert_awaited_once_with(path="/nav/NATS", key=None)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_pacots(patched_internal_get):
     json_response = [
         {
-            'ident': 1,
-            'route': {
-                'nodes': [
-                    {
-                        'id': 8465100,
-                        'ident': 'RESNO',
-                        'lat': 55,
-                        'lon': -15,
-                        'type': 'FIX'
-                    },
-                    {
-                        'id': 243738,
-                        'ident': '55/20',
-                        'lat': 55,
-                        'lon': -20,
-                        'type': 'LATLON'
-                    },
-                    {
-                        'id': 243581,
-                        'ident': '54/30',
-                        'lat': 54,
-                        'lon': -30,
-                        'type': 'LATLON'
-                    },
-                    {
-                        'id': 243584,
-                        'ident': '53/40',
-                        'lat': 53,
-                        'lon': -40,
-                        'type': 'LATLON'
-                    },
-                    {
-                        'id': 243583,
-                        'ident': '52/50',
-                        'lat': 52,
-                        'lon': -50,
-                        'type': 'LATLON'
-                    },
-                    {
-                        'id': 8423845,
-                        'ident': 'TUDEP',
-                        'lat': 51.1667,
-                        'lon': -53.2333,
-                        'type': 'FIX'
-                    }]},
-            'validFrom': '2021-04-28T11:30:00.000Z',
-            'validTo': '2021-04-28T19:00:00.000Z'}]
+            "ident": 1,
+            "route": {
+                "nodes": [
+                    {
+                        "id": 8465100,
+                        "ident": "RESNO",
+                        "lat": 55,
+                        "lon": -15,
+                        "type": "FIX",
+                    },
+                    {
+                        "id": 243738,
+                        "ident": "55/20",
+                        "lat": 55,
+                        "lon": -20,
+                        "type": "LATLON",
+                    },
+                    {
+                        "id": 243581,
+                        "ident": "54/30",
+                        "lat": 54,
+                        "lon": -30,
+                        "type": "LATLON",
+                    },
+                    {
+                        "id": 243584,
+                        "ident": "53/40",
+                        "lat": 53,
+                        "lon": -40,
+                        "type": "LATLON",
+                    },
+                    {
+                        "id": 243583,
+                        "ident": "52/50",
+                        "lat": 52,
+                        "lon": -50,
+                        "type": "LATLON",
+                    },
+                    {
+                        "id": 8423845,
+                        "ident": "TUDEP",
+                        "lat": 51.1667,
+                        "lon": -53.2333,
+                        "type": "FIX",
+                    },
+                ]
+            },
+            "validFrom": "2021-04-28T11:30:00.000Z",
+            "validTo": "2021-04-28T19:00:00.000Z",
+        }
+    ]
 
     correct_response = [
         Track(
             ident=1,
             route=Route(
                 nodes=[
                     RouteNode(
-                        ident='RESNO',
-                        type='FIX',
+                        ident="RESNO",
+                        type="FIX",
                         lat=55,
                         lon=-15,
                         id=8465100,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='55/20',
-                        type='LATLON',
+                        ident="55/20",
+                        type="LATLON",
                         lat=55,
                         lon=-20,
                         id=243738,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='54/30',
-                        type='LATLON',
+                        ident="54/30",
+                        type="LATLON",
                         lat=54,
                         lon=-30,
                         id=243581,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='53/40',
-                        type='LATLON',
+                        ident="53/40",
+                        type="LATLON",
                         lat=53,
                         lon=-40,
                         id=243584,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='52/50',
-                        type='LATLON',
+                        ident="52/50",
+                        type="LATLON",
                         lat=52,
                         lon=-50,
                         id=243583,
                         alt=None,
                         name=None,
-                        via=None),
+                        via=None,
+                    ),
                     RouteNode(
-                        ident='TUDEP',
-                        type='FIX',
+                        ident="TUDEP",
+                        type="FIX",
                         lat=51.1667,
                         lon=-53.2333,
                         id=8423845,
                         alt=None,
                         name=None,
-                        via=None)]),
-            validFrom=datetime.datetime(
-                2021, 4, 28, 11, 30, tzinfo=tzutc()),
-            validTo=datetime.datetime(
-                2021, 4, 28, 19, 0, tzinfo=tzutc()))]
+                        via=None,
+                    ),
+                ]
+            ),
+            validFrom=datetime.datetime(2021, 4, 28, 11, 30, tzinfo=tzutc()),
+            validTo=datetime.datetime(2021, 4, 28, 19, 0, tzinfo=tzutc()),
+        )
+    ]
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.nav.pacots()
     # check that NavAPI method decoded data correctly for given response
     assert response == correct_response
     # check that NavAPI method made correct request of FlightPlanDB
-    patched_internal_get.assert_awaited_once_with(
-        path='/nav/PACOTS', key=None
-    )
+    patched_internal_get.assert_awaited_once_with(path="/nav/PACOTS", key=None)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.getiter")
 async def test_navaid_search(patched_internal_getiter):
     json_response = [
-        {'airportICAO': None,
-            'elevation': 1.0000000015200001,
-            'ident': 'SPY',
-            'lat': 52.5403,
-            'lon': 4.85378,
-            'name': 'SPIJKERBOOR',
-            'runwayIdent': None,
-            'type': 'VOR'},
-        {'airportICAO': None,
-            'elevation': 26.000000039520003,
-            'ident': 'SPY',
-            'lat': 52.5403,
-            'lon': 4.85378,
-            'name': 'SPIJKERBOOR VOR-DME',
-            'runwayIdent': None,
-            'type': 'DME'}
+        {
+            "airportICAO": None,
+            "elevation": 1.0000000015200001,
+            "ident": "SPY",
+            "lat": 52.5403,
+            "lon": 4.85378,
+            "name": "SPIJKERBOOR",
+            "runwayIdent": None,
+            "type": "VOR",
+        },
+        {
+            "airportICAO": None,
+            "elevation": 26.000000039520003,
+            "ident": "SPY",
+            "lat": 52.5403,
+            "lon": 4.85378,
+            "name": "SPIJKERBOOR VOR-DME",
+            "runwayIdent": None,
+            "type": "DME",
+        },
     ]
 
     correct_response_list = [
         SearchNavaid(
-            ident='SPY',
-            type='VOR',
+            ident="SPY",
+            type="VOR",
             lat=52.5403,
             lon=4.85378,
             elevation=1.0000000015200001,
             runwayIdent=None,
             airportICAO=None,
-            name='SPIJKERBOOR'),
+            name="SPIJKERBOOR",
+        ),
         SearchNavaid(
-            ident='SPY',
-            type='DME',
+            ident="SPY",
+            type="DME",
             lat=52.5403,
             lon=4.85378,
             elevation=26.000000039520003,
             runwayIdent=None,
             airportICAO=None,
-            name='SPIJKERBOOR VOR-DME')
+            name="SPIJKERBOOR VOR-DME",
+        ),
     ]
 
-    correct_calls = [mock.call(
-        path='/search/nav',
-        params={'q': 'SPY'},
-        key=None)]
+    correct_calls = [mock.call(path="/search/nav", params={"q": "SPY"}, key=None)]
 
     patched_internal_getiter.return_value = AsyncIter(json_response)
 
     response = flightplandb.nav.search("SPY")
     # check that PlanAPI method decoded data correctly for given response
     response_list = []
     async for i in response:
```

### Comparing `flightplandb-0.7.2/tests/test_plan.py` & `flightplandb-0.8.0/tests/test_plan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,98 +1,103 @@
+import datetime
 from unittest import mock
+
 import pytest
+from dateutil.tz import tzutc
+
 import flightplandb
 from flightplandb.datatypes import (
-    Plan, PlanQuery, User, Route, GenerateQuery,
-    RouteNode, Cycle, StatusResponse
+    Cycle,
+    GenerateQuery,
+    Plan,
+    PlanQuery,
+    Route,
+    RouteNode,
+    StatusResponse,
+    User,
 )
-import datetime
-from dateutil.tz import tzutc
 
 
 class AsyncIter:
     def __init__(self, items):
         self.items = items
 
     async def __aiter__(self):
         for item in self.items:
             yield item
 
 
 # localhost is set on every test to allow async loops
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_plan_fetch(patched_internal_get):
     json_response = {
-            "id": 62373,
-            "fromICAO": "KLAS",
-            "toICAO": "KLAX",
-            "fromName": "Mc Carran Intl",
-            "toName": "Los Angeles Intl",
-            "flightNumber": None,
-            "distance": 206.39578816273502,
-            "maxAltitude": 18000,
-            "waypoints": 8,
-            "likes": 0,
-            "downloads": 1,
-            "popularity": 1,
-            "notes": "",
-            "encodedPolyline": "aaf{E`|y}T|Ftf@px\\hpe@lnCxw Dbsk@r",
-            "createdAt": "2015-08-04T20:48:08.000Z",
-            "updatedAt": "2015-08-04T20:48:08.000Z",
-            "tags": [
-                "generated"
-            ],
-            "user": {
-                "id": 2429,
-                "username": "example",
-                "gravatarHash": "f30b58b998a11b5d417cc2c78df3f764",
-                "location": None
-            }
-        }
+        "id": 62373,
+        "fromICAO": "KLAS",
+        "toICAO": "KLAX",
+        "fromName": "Mc Carran Intl",
+        "toName": "Los Angeles Intl",
+        "flightNumber": None,
+        "distance": 206.39578816273502,
+        "maxAltitude": 18000,
+        "waypoints": 8,
+        "likes": 0,
+        "downloads": 1,
+        "popularity": 1,
+        "notes": "",
+        "encodedPolyline": "aaf{E`|y}T|Ftf@px\\hpe@lnCxw Dbsk@r",
+        "createdAt": "2015-08-04T20:48:08.000Z",
+        "updatedAt": "2015-08-04T20:48:08.000Z",
+        "tags": ["generated"],
+        "user": {
+            "id": 2429,
+            "username": "example",
+            "gravatarHash": "f30b58b998a11b5d417cc2c78df3f764",
+            "location": None,
+        },
+    }
 
     correct_response = Plan(
-            id=62373,
-            fromICAO="KLAS",
-            toICAO="KLAX",
-            fromName="Mc Carran Intl",
-            toName="Los Angeles Intl",
-            flightNumber=None,
-            distance=206.39578816273502,
-            maxAltitude=18000,
-            waypoints=8,
-            likes=0,
-            downloads=1,
-            popularity=1,
-            notes="",
-            encodedPolyline="aaf{E`|y}T|Ftf@px\\hpe@lnCxw Dbsk@r",
-            createdAt="2015-08-04T20:48:08.000Z",
-            updatedAt="2015-08-04T20:48:08.000Z",
-            tags=[
-                "generated"
-            ],
-            user=User(
-                id=2429,
-                username="example",
-                gravatarHash="f30b58b998a11b5d417cc2c78df3f764",
-                location=None
-            ))
+        id=62373,
+        fromICAO="KLAS",
+        toICAO="KLAX",
+        fromName="Mc Carran Intl",
+        toName="Los Angeles Intl",
+        flightNumber=None,
+        distance=206.39578816273502,
+        maxAltitude=18000,
+        waypoints=8,
+        likes=0,
+        downloads=1,
+        popularity=1,
+        notes="",
+        encodedPolyline="aaf{E`|y}T|Ftf@px\\hpe@lnCxw Dbsk@r",
+        createdAt="2015-08-04T20:48:08.000Z",
+        updatedAt="2015-08-04T20:48:08.000Z",
+        tags=["generated"],
+        user=User(
+            id=2429,
+            username="example",
+            gravatarHash="f30b58b998a11b5d417cc2c78df3f764",
+            location=None,
+        ),
+    )
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.plan.fetch(62373)
     # check that PlanAPI method decoded data correctly for given response
     assert response == correct_response
     # check that PlanAPI method made correct request of FlightPlanDB
     patched_internal_get.assert_awaited_once_with(
-        path='/plan/62373', return_format='native', key=None
+        path="/plan/62373", return_format="native", key=None
     )
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.post")
 async def test_plan_create(patched_internal_post):
     json_response = {
         "id": None,
         "fromICAO": "EHAM",
         "toICAO": "KJFK",
         "fromName": "Schiphol",
@@ -102,158 +107,178 @@
                 {
                     "ident": "EHAM",
                     "type": "APT",
                     "lat": 52.31485,
                     "lon": 4.75812,
                     "alt": 0,
                     "name": "Schiphol",
-                    "via": None
+                    "via": None,
                 },
                 {
                     "ident": "KJFK",
                     "type": "APT",
                     "lat": 40.63990,
                     "lon": -73.77666,
                     "alt": 0,
                     "name": "John F Kennedy Intl",
-                    "via": None
-                }
+                    "via": None,
+                },
             ]
-        }
+        },
     }
 
     correct_response = Plan(
         id=None,
         fromICAO="EHAM",
         toICAO="KJFK",
         fromName="Schiphol",
         toName="John F Kennedy Intl",
         user=None,
-        route=Route([
-            RouteNode(**{
-                "ident": "EHAM",
-                "type": "APT",
-                "lat": 52.31485,
-                "lon": 4.75812,
-                "alt": 0,
-                "name": "Schiphol",
-                "via": None}),
-            RouteNode(**{
-                "ident": "KJFK",
-                "type": "APT",
-                "lat": 40.63990,
-                "lon": -73.77666,
-                "alt": 0,
-                "name": "John F Kennedy Intl",
-                "via": None})]))
+        route=Route(
+            [
+                RouteNode(
+                    **{
+                        "ident": "EHAM",
+                        "type": "APT",
+                        "lat": 52.31485,
+                        "lon": 4.75812,
+                        "alt": 0,
+                        "name": "Schiphol",
+                        "via": None,
+                    }
+                ),
+                RouteNode(
+                    **{
+                        "ident": "KJFK",
+                        "type": "APT",
+                        "lat": 40.63990,
+                        "lon": -73.77666,
+                        "alt": 0,
+                        "name": "John F Kennedy Intl",
+                        "via": None,
+                    }
+                ),
+            ]
+        ),
+    )
 
     request_data = Plan(
         id=None,
         fromICAO="EHAM",
         toICAO="KJFK",
         fromName="Schiphol",
         toName="John F Kennedy Intl",
         user=None,
-        route=Route([
-            RouteNode(**{
-                "ident": "EHAM",
-                "type": "APT",
-                "lat": 52.31485,
-                "lon": 4.75812,
-                "alt": 0,
-                "name": "Schiphol",
-                "via": None}),
-            RouteNode(**{
-                "ident": "KJFK",
-                "type": "APT",
-                "lat": 40.63990,
-                "lon": -73.77666,
-                "alt": 0,
-                "name": "John F Kennedy Intl",
-                "via": None})]))
+        route=Route(
+            [
+                RouteNode(
+                    **{
+                        "ident": "EHAM",
+                        "type": "APT",
+                        "lat": 52.31485,
+                        "lon": 4.75812,
+                        "alt": 0,
+                        "name": "Schiphol",
+                        "via": None,
+                    }
+                ),
+                RouteNode(
+                    **{
+                        "ident": "KJFK",
+                        "type": "APT",
+                        "lat": 40.63990,
+                        "lon": -73.77666,
+                        "alt": 0,
+                        "name": "John F Kennedy Intl",
+                        "via": None,
+                    }
+                ),
+            ]
+        ),
+    )
     correct_call = {
-        'path': '/plan/',
-        'json_data': {
-            'id': None,
-            'fromICAO': 'EHAM',
-            'toICAO': 'KJFK',
-            'fromName': 'Schiphol',
-            'toName': 'John F Kennedy Intl',
-            'flightNumber': None,
-            'distance': None,
-            'maxAltitude': None,
-            'waypoints': None,
-            'likes': None,
-            'downloads': None,
-            'popularity': None,
-            'notes': None,
-            'encodedPolyline': None,
-            'createdAt': None,
-            'updatedAt': None,
-            'tags': None,
-            'user': None,
-            'application': None,
-            'route': {
-                'nodes': [
-                    {'ident': 'EHAM',
-                        'type': 'APT',
-                        'lat': 52.31485,
-                        'lon': 4.75812,
-                        'id': None,
-                        'alt': 0,
-                        'name': 'Schiphol',
-                        'via': None},
-                    {'ident': 'KJFK',
-                        'type': 'APT',
-                        'lat': 40.6399,
-                        'lon': -73.77666,
-                        'id': None,
-                        'alt': 0,
-                        'name': 'John F Kennedy Intl',
-                        'via': None}],
-                'eastLevels': None,
-                'westLevels': None},
-            'cycle': None},
-        'return_format': 'native',
-        'key': None
+        "path": "/plan/",
+        "json_data": {
+            "id": None,
+            "fromICAO": "EHAM",
+            "toICAO": "KJFK",
+            "fromName": "Schiphol",
+            "toName": "John F Kennedy Intl",
+            "flightNumber": None,
+            "distance": None,
+            "maxAltitude": None,
+            "waypoints": None,
+            "likes": None,
+            "downloads": None,
+            "popularity": None,
+            "notes": None,
+            "encodedPolyline": None,
+            "createdAt": None,
+            "updatedAt": None,
+            "tags": None,
+            "user": None,
+            "application": None,
+            "route": {
+                "nodes": [
+                    {
+                        "ident": "EHAM",
+                        "type": "APT",
+                        "lat": 52.31485,
+                        "lon": 4.75812,
+                        "id": None,
+                        "alt": 0,
+                        "name": "Schiphol",
+                        "via": None,
+                    },
+                    {
+                        "ident": "KJFK",
+                        "type": "APT",
+                        "lat": 40.6399,
+                        "lon": -73.77666,
+                        "id": None,
+                        "alt": 0,
+                        "name": "John F Kennedy Intl",
+                        "via": None,
+                    },
+                ],
+                "eastLevels": None,
+                "westLevels": None,
+            },
+            "cycle": None,
+        },
+        "return_format": "native",
+        "key": None,
     }
 
     patched_internal_post.return_value = json_response
 
     response = await flightplandb.plan.create(request_data)
     # check that PlanAPI method decoded data correctly for given response
     assert response == correct_response
     # check that PlanAPI method made correct request of FlightPlanDB
-    patched_internal_post.assert_awaited_once_with(
-        **correct_call
-    )
+    patched_internal_post.assert_awaited_once_with(**correct_call)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.delete")
 async def test_plan_delete(patched_internal_delete):
-    json_response = {
-        "message": "OK",
-        "errors": None
-        }
+    json_response = {"message": "OK", "errors": None}
 
     correct_response = StatusResponse(message="OK", errors=None)
 
     patched_internal_delete.return_value = json_response
 
     response = await flightplandb.plan.delete(62493)
     # check that TagsAPI method made correct request of FlightPlanDB
-    patched_internal_delete.assert_awaited_once_with(
-        path='/plan/62493', key=None
-    )
+    patched_internal_delete.assert_awaited_once_with(path="/plan/62493", key=None)
     # check that TagsAPI method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.patch")
 async def test_plan_edit(patched_internal_patch):
     json_response = {
         "id": 23896,
         "fromICAO": "EHAM",
         "toICAO": "KJFK",
         "fromName": "Schiphol",
@@ -263,483 +288,468 @@
                 {
                     "ident": "EHAM",
                     "type": "APT",
                     "lat": 52.31485,
                     "lon": 4.75812,
                     "alt": 0,
                     "name": "Schiphol",
-                    "via": None
+                    "via": None,
                 },
                 {
                     "ident": "KJFK",
                     "type": "APT",
                     "lat": 40.63990,
                     "lon": -73.77666,
                     "alt": 0,
                     "name": "John F Kennedy Intl",
-                    "via": None
-                }
+                    "via": None,
+                },
             ]
-        }
+        },
     }
 
     correct_response = Plan(
         id=23896,
         fromICAO="EHAM",
         toICAO="KJFK",
         fromName="Schiphol",
         toName="John F Kennedy Intl",
         user=None,
-        route=Route([
-            RouteNode(**{
-                "ident": "EHAM",
-                "type": "APT",
-                "lat": 52.31485,
-                "lon": 4.75812,
-                "alt": 0,
-                "name": "Schiphol",
-                "via": None
-            }),
-            RouteNode(**{
-                "ident": "KJFK",
-                "type": "APT",
-                "lat": 40.63990,
-                "lon": -73.77666,
-                "alt": 0,
-                "name": "John F Kennedy Intl",
-                "via": None
-            })
-        ])
+        route=Route(
+            [
+                RouteNode(
+                    **{
+                        "ident": "EHAM",
+                        "type": "APT",
+                        "lat": 52.31485,
+                        "lon": 4.75812,
+                        "alt": 0,
+                        "name": "Schiphol",
+                        "via": None,
+                    }
+                ),
+                RouteNode(
+                    **{
+                        "ident": "KJFK",
+                        "type": "APT",
+                        "lat": 40.63990,
+                        "lon": -73.77666,
+                        "alt": 0,
+                        "name": "John F Kennedy Intl",
+                        "via": None,
+                    }
+                ),
+            ]
+        ),
     )
 
     request_data = Plan(
         id=23896,
         fromICAO="EHAM",
         toICAO="KJFK",
         fromName="Schiphol",
         toName="John F Kennedy Intl",
         user=None,
-        route=Route([
-            RouteNode(**{
-                "ident": "EHAM",
-                "type": "APT",
-                "lat": 52.31485,
-                "lon": 4.75812,
-                "alt": 0,
-                "name": "Schiphol",
-                "via": None
-            }),
-            RouteNode(**{
-                "ident": "KJFK",
-                "type": "APT",
-                "lat": 40.63990,
-                "lon": -73.77666,
-                "alt": 0,
-                "name": "John F Kennedy Intl",
-                "via": None
-            })
-        ])
+        route=Route(
+            [
+                RouteNode(
+                    **{
+                        "ident": "EHAM",
+                        "type": "APT",
+                        "lat": 52.31485,
+                        "lon": 4.75812,
+                        "alt": 0,
+                        "name": "Schiphol",
+                        "via": None,
+                    }
+                ),
+                RouteNode(
+                    **{
+                        "ident": "KJFK",
+                        "type": "APT",
+                        "lat": 40.63990,
+                        "lon": -73.77666,
+                        "alt": 0,
+                        "name": "John F Kennedy Intl",
+                        "via": None,
+                    }
+                ),
+            ]
+        ),
     )
     correct_call = {
-        'path': '/plan/23896',
-        'json_data': {
-            'id': 23896,
-            'fromICAO': 'EHAM',
-            'toICAO': 'KJFK',
-            'fromName': 'Schiphol',
-            'toName': 'John F Kennedy Intl',
-            'flightNumber': None,
-            'distance': None,
-            'maxAltitude': None,
-            'waypoints': None,
-            'likes': None,
-            'downloads': None,
-            'popularity': None,
-            'notes': None,
-            'encodedPolyline': None,
-            'createdAt': None,
-            'updatedAt': None,
-            'tags': None,
-            'user': None,
-            'application': None,
-            'route': {
-                'nodes': [
-                    {'ident': 'EHAM',
-                        'type': 'APT',
-                        'lat': 52.31485,
-                        'lon': 4.75812,
-                        'id': None,
-                        'alt': 0,
-                        'name': 'Schiphol',
-                        'via': None},
-                    {'ident': 'KJFK',
-                        'type': 'APT',
-                        'lat': 40.6399,
-                        'lon': -73.77666,
-                        'id': None,
-                        'alt': 0,
-                        'name': 'John F Kennedy Intl',
-                        'via': None}],
-                'eastLevels': None,
-                'westLevels': None},
-            'cycle': None},
-        'return_format': 'native',
-        'key': None
+        "path": "/plan/23896",
+        "json_data": {
+            "id": 23896,
+            "fromICAO": "EHAM",
+            "toICAO": "KJFK",
+            "fromName": "Schiphol",
+            "toName": "John F Kennedy Intl",
+            "flightNumber": None,
+            "distance": None,
+            "maxAltitude": None,
+            "waypoints": None,
+            "likes": None,
+            "downloads": None,
+            "popularity": None,
+            "notes": None,
+            "encodedPolyline": None,
+            "createdAt": None,
+            "updatedAt": None,
+            "tags": None,
+            "user": None,
+            "application": None,
+            "route": {
+                "nodes": [
+                    {
+                        "ident": "EHAM",
+                        "type": "APT",
+                        "lat": 52.31485,
+                        "lon": 4.75812,
+                        "id": None,
+                        "alt": 0,
+                        "name": "Schiphol",
+                        "via": None,
+                    },
+                    {
+                        "ident": "KJFK",
+                        "type": "APT",
+                        "lat": 40.6399,
+                        "lon": -73.77666,
+                        "id": None,
+                        "alt": 0,
+                        "name": "John F Kennedy Intl",
+                        "via": None,
+                    },
+                ],
+                "eastLevels": None,
+                "westLevels": None,
+            },
+            "cycle": None,
+        },
+        "return_format": "native",
+        "key": None,
     }
 
     patched_internal_patch.return_value = json_response
 
     response = await flightplandb.plan.edit(
         plan=request_data, return_format="native", key=None
     )
     # check that PlanAPI method decoded data correctly for given response
     assert response == correct_response
     # check that PlanAPI method made correct request of FlightPlanDB
     patched_internal_patch.assert_called_once_with(**correct_call)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.getiter")
 async def test_plan_search(patched_internal_getiter):
     json_response = [
         {
-            'application': None,
-            'createdAt': '2020-09-30T21:22:37.000Z',
-            'cycle': {
-                'id': 31,
-                'ident': 'FPD2009',
-                'release': 9,
-                'year': 20},
-            'distance': 76.676565810015,
-            'downloads': 2,
-            'encodedPolyline': 'slg~Haoa\\_fiA{xlAkotC{xcB',
-            'flightNumber': None,
-            'fromICAO': 'EHAM',
-            'fromName': 'Amsterdam Schiphol',
-            'id': 3491827,
-            'likes': 0,
-            'maxAltitude': 9600,
-            'notes': 'foo',
-            'popularity': 1601846557,
-            'tags': ['generated'],
-            'toICAO': 'EHAL',
-            'toName': 'Ameland',
-            'updatedAt': '2020-09-30T21:22:37.000Z',
-            'user': None,
-            'waypoints': 3},
-
+            "application": None,
+            "createdAt": "2020-09-30T21:22:37.000Z",
+            "cycle": {"id": 31, "ident": "FPD2009", "release": 9, "year": 20},
+            "distance": 76.676565810015,
+            "downloads": 2,
+            "encodedPolyline": "slg~Haoa\\_fiA{xlAkotC{xcB",
+            "flightNumber": None,
+            "fromICAO": "EHAM",
+            "fromName": "Amsterdam Schiphol",
+            "id": 3491827,
+            "likes": 0,
+            "maxAltitude": 9600,
+            "notes": "foo",
+            "popularity": 1601846557,
+            "tags": ["generated"],
+            "toICAO": "EHAL",
+            "toName": "Ameland",
+            "updatedAt": "2020-09-30T21:22:37.000Z",
+            "user": None,
+            "waypoints": 3,
+        },
         {
-            'application': None,
-            'createdAt': '2018-09-08T12:23:04.000Z',
-            'cycle': {
-                'id': 5,
-                'ident': 'FPD1809',
-                'release': 9,
-                'year': 18},
-            'distance': 76.44654421193701,
-            'downloads': 0,
-            'encodedPolyline': 'slg~Haoa\\{hlC}|xBolqAytw@',
-            'flightNumber': None,
-            'fromICAO': 'EHAM',
-            'fromName': 'Amsterdam Schiphol Airport',
-            'id': 1295630,
-            'likes': 0,
-            'maxAltitude': 7700,
-            'notes': 'foo',
-            'popularity': 1536409384,
-            'tags': ['generated'],
-            'toICAO': 'EHAL',
-            'toName': 'Ameland',
-            'updatedAt': '2018-09-08T12:23:04.000Z',
-            'user': None,
-            'waypoints': 3}
+            "application": None,
+            "createdAt": "2018-09-08T12:23:04.000Z",
+            "cycle": {"id": 5, "ident": "FPD1809", "release": 9, "year": 18},
+            "distance": 76.44654421193701,
+            "downloads": 0,
+            "encodedPolyline": "slg~Haoa\\{hlC}|xBolqAytw@",
+            "flightNumber": None,
+            "fromICAO": "EHAM",
+            "fromName": "Amsterdam Schiphol Airport",
+            "id": 1295630,
+            "likes": 0,
+            "maxAltitude": 7700,
+            "notes": "foo",
+            "popularity": 1536409384,
+            "tags": ["generated"],
+            "toICAO": "EHAL",
+            "toName": "Ameland",
+            "updatedAt": "2018-09-08T12:23:04.000Z",
+            "user": None,
+            "waypoints": 3,
+        },
     ]
 
     correct_response_list = [
         Plan(
             id=3491827,
-            fromICAO='EHAM',
-            toICAO='EHAL',
-            fromName='Amsterdam Schiphol',
-            toName='Ameland',
+            fromICAO="EHAM",
+            toICAO="EHAL",
+            fromName="Amsterdam Schiphol",
+            toName="Ameland",
             flightNumber=None,
             distance=76.676565810015,
             maxAltitude=9600,
             waypoints=3,
             likes=0,
             downloads=2,
             popularity=1601846557,
-            notes='foo',
-            encodedPolyline='slg~Haoa\\_fiA{xlAkotC{xcB',
-            createdAt=datetime.datetime(2020, 9, 30, 21, 22, 37,
-                                        tzinfo=tzutc()),
-            updatedAt=datetime.datetime(2020, 9, 30, 21, 22, 37,
-                                        tzinfo=tzutc()),
-            tags=['generated'], user=None, application=None,
+            notes="foo",
+            encodedPolyline="slg~Haoa\\_fiA{xlAkotC{xcB",
+            createdAt=datetime.datetime(2020, 9, 30, 21, 22, 37, tzinfo=tzutc()),
+            updatedAt=datetime.datetime(2020, 9, 30, 21, 22, 37, tzinfo=tzutc()),
+            tags=["generated"],
+            user=None,
+            application=None,
             route=None,
-            cycle=Cycle(id=31, ident='FPD2009', year=20, release=9)),
-
+            cycle=Cycle(id=31, ident="FPD2009", year=20, release=9),
+        ),
         Plan(
             id=1295630,
-            fromICAO='EHAM',
-            toICAO='EHAL',
-            fromName='Amsterdam Schiphol Airport',
-            toName='Ameland',
+            fromICAO="EHAM",
+            toICAO="EHAL",
+            fromName="Amsterdam Schiphol Airport",
+            toName="Ameland",
             flightNumber=None,
             distance=76.44654421193701,
             maxAltitude=7700,
             waypoints=3,
             likes=0,
             downloads=0,
             popularity=1536409384,
-            notes='foo',
-            encodedPolyline='slg~Haoa\\{hlC}|xBolqAytw@',
-            createdAt=datetime.datetime(2018, 9, 8, 12, 23, 4,
-                                        tzinfo=tzutc()),
-            updatedAt=datetime.datetime(2018, 9, 8, 12, 23, 4,
-                                        tzinfo=tzutc()),
-            tags=['generated'],
+            notes="foo",
+            encodedPolyline="slg~Haoa\\{hlC}|xBolqAytw@",
+            createdAt=datetime.datetime(2018, 9, 8, 12, 23, 4, tzinfo=tzutc()),
+            updatedAt=datetime.datetime(2018, 9, 8, 12, 23, 4, tzinfo=tzutc()),
+            tags=["generated"],
             user=None,
             application=None,
             route=None,
-            cycle=Cycle(id=5, ident='FPD1809', year=18, release=9))
-
+            cycle=Cycle(id=5, ident="FPD1809", year=18, release=9),
+        ),
     ]
-    correct_calls = [mock.call(
-        path='/search/plans',
-        sort='created',
-        params={
-            'q': None,
-            'From': None,
-            'to': None,
-            'fromICAO': 'EHAM',
-            'toICAO': 'EHAL',
-            'fromName': None,
-            'toName': None,
-            'flightNumber': None,
-            'distanceMin': None,
-            'distanceMax': None,
-            'tags': None,
-            'includeRoute': False
+    correct_calls = [
+        mock.call(
+            path="/search/plans",
+            sort="created",
+            params={
+                "q": None,
+                "From": None,
+                "to": None,
+                "fromICAO": "EHAM",
+                "toICAO": "EHAL",
+                "fromName": None,
+                "toName": None,
+                "flightNumber": None,
+                "distanceMin": None,
+                "distanceMax": None,
+                "tags": None,
+                "includeRoute": False,
             },
-        limit=2,
-        key=None)]
+            limit=2,
+            key=None,
+        )
+    ]
 
     patched_internal_getiter.return_value = AsyncIter(json_response)
 
     response = flightplandb.plan.search(
-            PlanQuery(
-                fromICAO="EHAM",
-                toICAO="EHAL"),
-            limit=2)
+        PlanQuery(fromICAO="EHAM", toICAO="EHAL"), limit=2
+    )
     # check that PlanAPI method decoded data correctly for given response
     response_list = []
     async for i in response:
         response_list.append(i)
     assert response_list == correct_response_list
     # check that PlanAPI method made correct request of FlightPlanDB
     patched_internal_getiter.assert_has_calls(correct_calls)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.post")
 async def test_plan_like(patched_internal_post):
-    json_response = {
-        "message": "Not Found",
-        "errors": None
-        }
+    json_response = {"message": "Not Found", "errors": None}
 
-    correct_response = StatusResponse(message='Not Found', errors=None)
+    correct_response = StatusResponse(message="Not Found", errors=None)
 
     patched_internal_post.return_value = json_response
 
     response = await flightplandb.plan.like(42)
     # check that TagsAPI method made correct request of FlightPlanDB
-    patched_internal_post.assert_awaited_once_with(
-        path='/plan/42/like', key=None
-    )
+    patched_internal_post.assert_awaited_once_with(path="/plan/42/like", key=None)
     # check that TagsAPI method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.delete")
 async def test_plan_unlike(patched_internal_delete):
-    json_response = {
-        "message": "OK",
-        "errors": None
-        }
+    json_response = {"message": "OK", "errors": None}
 
     correct_response = True
 
     patched_internal_delete.return_value = json_response
 
     response = await flightplandb.plan.unlike(42)
     # check that TagsAPI method made correct request of FlightPlanDB
-    patched_internal_delete.assert_awaited_once_with(
-        path='/plan/42/like', key=None
-    )
+    patched_internal_delete.assert_awaited_once_with(path="/plan/42/like", key=None)
     # check that TagsAPI method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_plan_has_liked(patched_internal_get):
-    json_response = {
-        "message": "OK",
-        "errors": None
-        }
+    json_response = {"message": "OK", "errors": None}
 
     correct_response = True
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.plan.has_liked(42)
     # check that TagsAPI method made correct request of FlightPlanDB
     patched_internal_get.assert_awaited_once_with(
-        path='/plan/42/like', ignore_statuses=[404], key=None
+        path="/plan/42/like", ignore_statuses=[404], key=None
     )
     # check that TagsAPI method decoded data correctly for given response
     assert response == correct_response
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.post")
 async def test_plan_generate(patched_internal_post):
     json_response = {
-        'application': None,
-        'createdAt': '2021-04-28T19:55:45.000Z',
-        'cycle': {
-            'id': 38,
-            'ident': 'FPD2104',
-            'release': 4,
-            'year': 21},
-        'distance': 36.666306664518004,
-        'downloads': 0,
-        'encodedPolyline': '_dgeIybta@niaA~vdD',
-        'flightNumber': None,
-        'fromICAO': 'EHAL',
-        'fromName': 'Ameland',
-        'id': 4179148,
-        'likes': 0,
-        'maxAltitude': 0,
-        'notes': 'Basic altitude profile:\n'
-                    '- Ascent Rate: 2500ft/min\n'
-                    '- Ascent Speed: 250kts\n'
-                    '- Cruise Altitude: 35000ft\n'
-                    '- Cruise Speed: 420kts\n'
-                    '- Descent Rate: 1500ft/min\n'
-                    '- Descent Speed: 250kts\n'
-                    '\n'
-                    'Options:\n'
-                    '- Use NATs: yes\n'
-                    '- Use PACOTS: yes\n'
-                    '- Use low airways: yes\n'
-                    '- Use high airways: yes\n',
-        'popularity': 1619639745,
-        'tags': ['generated'],
-        'toICAO': 'EHTX',
-        'toName': 'Texel',
-        'updatedAt': '2021-04-28T19:55:45.000Z',
-        'user': {
-            'gravatarHash': '3bcb4f39a24700e081f49c3d2d43d277',
-            'id': 18990,
-            'location': None,
-            'username': 'discordflightplannerbot'},
-        'waypoints': 2
+        "application": None,
+        "createdAt": "2021-04-28T19:55:45.000Z",
+        "cycle": {"id": 38, "ident": "FPD2104", "release": 4, "year": 21},
+        "distance": 36.666306664518004,
+        "downloads": 0,
+        "encodedPolyline": "_dgeIybta@niaA~vdD",
+        "flightNumber": None,
+        "fromICAO": "EHAL",
+        "fromName": "Ameland",
+        "id": 4179148,
+        "likes": 0,
+        "maxAltitude": 0,
+        "notes": "Basic altitude profile:\n"
+        "- Ascent Rate: 2500ft/min\n"
+        "- Ascent Speed: 250kts\n"
+        "- Cruise Altitude: 35000ft\n"
+        "- Cruise Speed: 420kts\n"
+        "- Descent Rate: 1500ft/min\n"
+        "- Descent Speed: 250kts\n"
+        "\n"
+        "Options:\n"
+        "- Use NATs: yes\n"
+        "- Use PACOTS: yes\n"
+        "- Use low airways: yes\n"
+        "- Use high airways: yes\n",
+        "popularity": 1619639745,
+        "tags": ["generated"],
+        "toICAO": "EHTX",
+        "toName": "Texel",
+        "updatedAt": "2021-04-28T19:55:45.000Z",
+        "user": {
+            "gravatarHash": "3bcb4f39a24700e081f49c3d2d43d277",
+            "id": 18990,
+            "location": None,
+            "username": "discordflightplannerbot",
+        },
+        "waypoints": 2,
     }
 
-    request_data = GenerateQuery(
-        fromICAO="EHAL",
-        toICAO="EHTX"
-    )
+    request_data = GenerateQuery(fromICAO="EHAL", toICAO="EHTX")
 
     correct_response = Plan(
         id=4179148,
-        fromICAO='EHAL',
-        toICAO='EHTX',
-        fromName='Ameland',
-        toName='Texel',
+        fromICAO="EHAL",
+        toICAO="EHTX",
+        fromName="Ameland",
+        toName="Texel",
         flightNumber=None,
         distance=36.666306664518004,
         maxAltitude=0,
         waypoints=2,
         likes=0,
         downloads=0,
         popularity=1619639745,
-        notes='Basic altitude profile:\n'
-        '- Ascent Rate: 2500ft/min\n'
-        '- Ascent Speed: 250kts\n'
-        '- Cruise Altitude: 35000ft\n'
-        '- Cruise Speed: 420kts\n'
-        '- Descent Rate: 1500ft/min\n'
-        '- Descent Speed: 250kts\n\nOptions:\n'
-        '- Use NATs: yes\n'
-        '- Use PACOTS: yes\n'
-        '- Use low airways: yes\n'
-        '- Use high airways: yes\n',
-        encodedPolyline='_dgeIybta@niaA~vdD',
-        createdAt=datetime.datetime(
-            2021, 4, 28, 19, 55, 45, tzinfo=tzutc()),
-        updatedAt=datetime.datetime(
-            2021, 4, 28, 19, 55, 45, tzinfo=tzutc()),
-        tags=['generated'],
+        notes="Basic altitude profile:\n"
+        "- Ascent Rate: 2500ft/min\n"
+        "- Ascent Speed: 250kts\n"
+        "- Cruise Altitude: 35000ft\n"
+        "- Cruise Speed: 420kts\n"
+        "- Descent Rate: 1500ft/min\n"
+        "- Descent Speed: 250kts\n\nOptions:\n"
+        "- Use NATs: yes\n"
+        "- Use PACOTS: yes\n"
+        "- Use low airways: yes\n"
+        "- Use high airways: yes\n",
+        encodedPolyline="_dgeIybta@niaA~vdD",
+        createdAt=datetime.datetime(2021, 4, 28, 19, 55, 45, tzinfo=tzutc()),
+        updatedAt=datetime.datetime(2021, 4, 28, 19, 55, 45, tzinfo=tzutc()),
+        tags=["generated"],
         user=User(
             id=18990,
-            username='discordflightplannerbot',
+            username="discordflightplannerbot",
             location=None,
-            gravatarHash='3bcb4f39a24700e081f49c3d2d43d277',
+            gravatarHash="3bcb4f39a24700e081f49c3d2d43d277",
             joined=None,
             lastSeen=None,
             plansCount=0,
             plansDistance=0.0,
             plansDownloads=0,
-            plansLikes=0),
+            plansLikes=0,
+        ),
         application=None,
         route=None,
-        cycle=Cycle(
-            id=38,
-            ident='FPD2104',
-            year=21,
-            release=4)
+        cycle=Cycle(id=38, ident="FPD2104", year=21, release=4),
     )
 
     correct_call = {
-        "path": '/auto/generate',
+        "path": "/auto/generate",
         "json_data": {
-            'fromICAO': 'EHAL',
-            'toICAO': 'EHTX',
-            'useNAT': True,
-            'usePACOT': True,
-            'useAWYLO': True,
-            'useAWYHI': True,
-            'cruiseAlt': 35000,
-            'cruiseSpeed': 420,
-            'ascentRate': 2500,
-            'ascentSpeed': 250,
-            'descentRate': 1500,
-            'descentSpeed': 250,
-            'includeRoute': 'false'
+            "fromICAO": "EHAL",
+            "toICAO": "EHTX",
+            "useNAT": True,
+            "usePACOT": True,
+            "useAWYLO": True,
+            "useAWYHI": True,
+            "cruiseAlt": 35000,
+            "cruiseSpeed": 420,
+            "ascentRate": 2500,
+            "ascentSpeed": 250,
+            "descentRate": 1500,
+            "descentSpeed": 250,
+            "includeRoute": "false",
         },
-        "key": None
+        "key": None,
     }
 
     patched_internal_post.return_value = json_response
 
     response = await flightplandb.plan.generate(request_data)
     # check that PlanAPI method decoded data correctly for given response
     assert response == correct_response
     # check that PlanAPI method made correct request of FlightPlanDB
-    patched_internal_post.assert_awaited_once_with(
-        **correct_call
-    )
+    patched_internal_post.assert_awaited_once_with(**correct_call)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.post")
 async def test_plan_decode(patched_internal_post):
     json_response = {
         "id": 4708699,
         "fromICAO": "KSAN",
         "toICAO": "KDEN",
         "fromName": "San Diego Intl",
@@ -752,88 +762,67 @@
         "downloads": 0,
         "popularity": 1635191202,
         "notes": "Requested: KSAN BROWS TRM LRAIN KDEN",
         "encodedPolyline": "_hxfEntgjUr_S_`qAgvaEocvBsksPgn_a@_~kSwgbc@",
         "createdAt": "2021-10-25T19:46:42.000Z",
         "updatedAt": "2021-10-25T19:46:42.000Z",
         "tags": ["decoded"],
-        'user': {
-            'gravatarHash': '3bcb4f39a24700e081f49c3d2d43d277',
-            'id': 18990,
-            'location': None,
-            'username': 'discordflightplannerbot'},
+        "user": {
+            "gravatarHash": "3bcb4f39a24700e081f49c3d2d43d277",
+            "id": 18990,
+            "location": None,
+            "username": "discordflightplannerbot",
+        },
         "application": None,
-        "cycle": {
-            "id": 40,
-            "ident": "FPD2106",
-            "year": 21,
-            "release": 6
-            }
-        }
+        "cycle": {"id": 40, "ident": "FPD2106", "year": 21, "release": 6},
+    }
 
     request_data = {"KSAN BROWS TRM LRAIN KDEN"}
 
     correct_response = Plan(
         id=4708699,
-        fromICAO='KSAN',
-        toICAO='KDEN',
-        fromName='San Diego Intl',
-        toName='Denver Intl',
+        fromICAO="KSAN",
+        toICAO="KDEN",
+        fromName="San Diego Intl",
+        toName="Denver Intl",
         flightNumber=None,
         distance=757.3434118878,
         maxAltitude=0,
         waypoints=5,
         likes=0,
         downloads=0,
         popularity=1635191202,
-        notes='Requested: KSAN BROWS TRM LRAIN KDEN',
-        encodedPolyline='_hxfEntgjUr_S_`qAgvaEocvBsksPgn_a@_~kSwgbc@',
-        createdAt=datetime.datetime(
-            2021, 10, 25, 19, 46, 42,
-            tzinfo=tzutc()
-            ),
-        updatedAt=datetime.datetime(
-            2021, 10, 25, 19, 46, 42,
-            tzinfo=tzutc()
-            ),
-        tags=['decoded'],
+        notes="Requested: KSAN BROWS TRM LRAIN KDEN",
+        encodedPolyline="_hxfEntgjUr_S_`qAgvaEocvBsksPgn_a@_~kSwgbc@",
+        createdAt=datetime.datetime(2021, 10, 25, 19, 46, 42, tzinfo=tzutc()),
+        updatedAt=datetime.datetime(2021, 10, 25, 19, 46, 42, tzinfo=tzutc()),
+        tags=["decoded"],
         user=User(
             id=18990,
-            username='discordflightplannerbot',
+            username="discordflightplannerbot",
             location=None,
-            gravatarHash='3bcb4f39a24700e081f49c3d2d43d277',
+            gravatarHash="3bcb4f39a24700e081f49c3d2d43d277",
             joined=None,
             lastSeen=None,
             plansCount=0,
             plansDistance=0.0,
             plansDownloads=0,
-            plansLikes=0
-            ),
+            plansLikes=0,
+        ),
         application=None,
         route=None,
-        cycle=Cycle(
-            id=40,
-            ident='FPD2106',
-            year=21,
-            release=6
-            )
-        )
+        cycle=Cycle(id=40, ident="FPD2106", year=21, release=6),
+    )
 
     correct_call = {
-        "path": '/auto/decode',
-        "json_data": {
-            'route': {
-                'KSAN BROWS TRM LRAIN KDEN'
-                }
-        },
-        "key": None
+        "path": "/auto/decode",
+        "json_data": {"route": {"KSAN BROWS TRM LRAIN KDEN"}},
+        "key": None,
     }
 
     patched_internal_post.return_value = json_response
 
     response = await flightplandb.plan.decode(request_data)
     # check that PlanAPI method decoded data correctly for given response
     assert response == correct_response
     # check that PlanAPI method made correct request of FlightPlanDB
-    patched_internal_post.assert_awaited_once_with(
-        **correct_call
-    )
+    patched_internal_post.assert_awaited_once_with(**correct_call)
```

### Comparing `flightplandb-0.7.2/tests/test_tags.py` & `flightplandb-0.8.0/tests/test_tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 from unittest import mock
+
 import pytest
+
 import flightplandb
 from flightplandb.datatypes import Tag
 
 
 # localhost is set on every test to allow async loops
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_tags_api(patched_internal_get):
     json_response = [
         {
             "name": "Decoded",
             "description": "Flight plans decoded",
             "planCount": 7430,
-            "popularity": 0.010143822356129395
+            "popularity": 0.010143822356129395,
         },
         {
             "name": "Generated",
             "description": "Computer generated plans",
             "planCount": 35343,
-            "popularity": 0.009036140132228622
-        }
-                    ]
+            "popularity": 0.009036140132228622,
+        },
+    ]
 
     correct_response = [
-        Tag(name='Decoded',
-            description='Flight plans decoded',
+        Tag(
+            name="Decoded",
+            description="Flight plans decoded",
             planCount=7430,
-            popularity=0.010143822356129395),
-        Tag(name='Generated',
-            description='Computer generated plans',
+            popularity=0.010143822356129395,
+        ),
+        Tag(
+            name="Generated",
+            description="Computer generated plans",
             planCount=35343,
-            popularity=0.009036140132228622)
-        ]
+            popularity=0.009036140132228622,
+        ),
+    ]
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.tags.fetch()
     # check that TagsAPI method made correct request of FlightPlanDB
-    patched_internal_get.assert_awaited_once_with(
-        path='/tags', key=None
-    )
+    patched_internal_get.assert_awaited_once_with(path="/tags", key=None)
     # check that TagsAPI method decoded data correctly for given response
     assert response == correct_response
```

### Comparing `flightplandb-0.7.2/tests/test_user.py` & `flightplandb-0.8.0/tests/test_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,114 +1,104 @@
+import datetime
 from unittest import mock
+
 import pytest
-import flightplandb
-from flightplandb.datatypes import User, Plan, UserSmall
-import datetime
 from dateutil.tz import tzutc
 
+import flightplandb
+from flightplandb.datatypes import Plan, User, UserSmall
+
 
 class AsyncIter:
     def __init__(self, items):
         self.items = items
 
     async def __aiter__(self):
         for item in self.items:
             yield item
 
 
 # localhost is set on every test to allow async loops
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_self_info(patched_internal_get):
     json_response = {
         "id": 18990,
         "username": "discordflightplannerbot",
         "location": None,
         "gravatarHash": "3bcb4f39a24700e081f49c3d2d43d277",
         "joined": "2020-08-06T17:04:30.000Z",
         "lastSeen": "2020-12-27T12:40:06.000Z",
         "plansCount": 2,
         "plansDistance": 794.0094160460012,
         "plansDownloads": 0,
-        "plansLikes": 0
+        "plansLikes": 0,
     }
 
     correct_response = User(
         id=18990,
         username="discordflightplannerbot",
         location=None,
         gravatarHash="3bcb4f39a24700e081f49c3d2d43d277",
-        joined=datetime.datetime(
-            2020, 8, 6, 17, 4, 30,
-            tzinfo=tzutc()
-        ),
-        lastSeen=datetime.datetime(2020, 12, 27, 12, 40, 6,
-                                   tzinfo=tzutc()),
+        joined=datetime.datetime(2020, 8, 6, 17, 4, 30, tzinfo=tzutc()),
+        lastSeen=datetime.datetime(2020, 12, 27, 12, 40, 6, tzinfo=tzutc()),
         plansCount=2,
         plansDistance=794.0094160460012,
         plansDownloads=0,
-        plansLikes=0
+        plansLikes=0,
     )
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.user.me()
     # check that UserAPI method decoded data correctly for given response
     assert response == correct_response
     # check that UserAPI method made correct request of FlightPlanDB
-    patched_internal_get.assert_awaited_once_with(
-        path='/me', key=None
-    )
+    patched_internal_get.assert_awaited_once_with(path="/me", key=None)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_user_info(patched_internal_get):
     json_response = {
         "id": 1,
         "username": "lemon",
         "location": "\U0001F601",
         "gravatarHash": "7889b0d4380a7194b6b67c8e2765289d",
         "joined": "2008-12-31T15:49:18.000Z",
         "lastSeen": "2021-04-24T00:22:46.000Z",
         "plansCount": 479,
         "plansDistance": 1212799.2736187153,
         "plansDownloads": 10341,
-        "plansLikes": 33
+        "plansLikes": 33,
     }
 
     correct_response = User(
-            id=1,
-            username="lemon",
-            location="\U0001F601",
-            gravatarHash="7889b0d4380a7194b6b67c8e2765289d",
-            joined=datetime.datetime(
-                2008, 12, 31, 15, 49, 18,
-                tzinfo=tzutc()
-            ),
-            lastSeen=datetime.datetime(2021, 4, 24, 0, 22, 46,
-                                       tzinfo=tzutc()),
-            plansCount=479,
-            plansDistance=1212799.2736187153,
-            plansDownloads=10341,
-            plansLikes=33
-        )
+        id=1,
+        username="lemon",
+        location="\U0001F601",
+        gravatarHash="7889b0d4380a7194b6b67c8e2765289d",
+        joined=datetime.datetime(2008, 12, 31, 15, 49, 18, tzinfo=tzutc()),
+        lastSeen=datetime.datetime(2021, 4, 24, 0, 22, 46, tzinfo=tzutc()),
+        plansCount=479,
+        plansDistance=1212799.2736187153,
+        plansDownloads=10341,
+        plansLikes=33,
+    )
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.user.fetch("lemon")
     # check that UserAPI method decoded data correctly for given response
     assert response == correct_response
     # check that UserAPI method made correct request of FlightPlanDB
-    patched_internal_get.assert_awaited_once_with(
-        path='/user/lemon', key=None
-    )
+    patched_internal_get.assert_awaited_once_with(path="/user/lemon", key=None)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.getiter")
 async def test_user_plans(patched_internal_getiter):
     json_response = [
         {
             "id": 62373,
             "fromICAO": "KLAS",
             "toICAO": "KLAX",
@@ -121,23 +111,21 @@
             "likes": 0,
             "downloads": 1,
             "popularity": 1,
             "notes": "",
             "encodedPolyline": r"aaf{E`|y}T|Ftf@px\\hp e@`nnDd~f@zkmH",
             "createdAt": "2015-08-04T20:48:08.000Z",
             "updatedAt": "2015-08-04T20:48:08.000Z",
-            "tags": [
-                "generated"
-            ],
+            "tags": ["generated"],
             "user": {
                 "id": 2429,
                 "username": "example",
                 "gravatarHash": "f30b58b998a11b5d417cc2c78df3f764",
-                "location": None
-            }
+                "location": None,
+            },
         },
         {
             "id": 62493,
             "fromICAO": "EHAM",
             "toICAO": "KJFK",
             "fromName": "Schiphol",
             "toName": "John F Kennedy Intl",
@@ -151,17 +139,17 @@
             "createdAt": "2015-08-05T22:44:34.000Z",
             "updatedAt": "2015-08-05T22:44:34.000Z",
             "tags": ["atlantic"],
             "user": {
                 "id": 1,
                 "username": "example",
                 "gravatarHash": "f30b58b998a11b5d417cc2c78df3f764",
-                "location": None
-            }
-        }
+                "location": None,
+            },
+        },
     ]
 
     correct_response_list = [
         Plan(
             id=62373,
             fromICAO="KLAS",
             toICAO="KLAX",
@@ -174,24 +162,22 @@
             likes=0,
             downloads=1,
             popularity=1,
             notes="",
             encodedPolyline=r"aaf{E`|y}T|Ftf@px\\hp e@`nnDd~f@zkmH",
             createdAt="2015-08-04T20:48:08.000Z",
             updatedAt="2015-08-04T20:48:08.000Z",
-            tags=[
-                "generated"
-            ],
+            tags=["generated"],
             user=User(
                 id=2429,
                 username="example",
                 gravatarHash="f30b58b998a11b5d417cc2c78df3f764",
-                location=None
-                )
+                location=None,
             ),
+        ),
         Plan(
             id=62493,
             fromICAO="EHAM",
             toICAO="KJFK",
             fromName="Schiphol",
             toName="John F Kennedy Intl",
             flightNumber=None,
@@ -204,208 +190,204 @@
             createdAt="2015-08-05T22:44:34.000Z",
             updatedAt="2015-08-05T22:44:34.000Z",
             tags=["atlantic"],
             user=User(
                 id=1,
                 username="example",
                 gravatarHash="f30b58b998a11b5d417cc2c78df3f764",
-                location=None
-                )
-            )
-        ]
-
-    correct_calls = [mock.call(
-        path='/user/lemon/plans',
-        limit=100,
-        sort='created',
-        key=None
-    )]
+                location=None,
+            ),
+        ),
+    ]
+
+    correct_calls = [
+        mock.call(path="/user/lemon/plans", limit=100, sort="created", key=None)
+    ]
 
     patched_internal_getiter.return_value = AsyncIter(json_response)
 
     response = flightplandb.user.plans("lemon")
     # check that UserAPI method decoded data correctly for given response
     response_list = []
     async for i in response:
         response_list.append(i)
     assert response_list == correct_response_list
     # check that UserAPI method made correct request of FlightPlanDB
     patched_internal_getiter.assert_has_calls(correct_calls)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.getiter")
 async def test_user_likes(patched_internal_getiter):
     json_response = [
-            {
-                "id": 62373,
-                "fromICAO": "KLAS",
-                "toICAO": "KLAX",
-                "fromName": "Mc Carran Intl",
-                "toName": "Los Angeles Intl",
-                "flightNumber": None,
-                "distance": 206.39578816273502,
-                "maxAltitude": 18000,
-                "waypoints": 8,
-                "likes": 0,
-                "downloads": 1,
-                "popularity": 1,
-                "notes": "",
-                "encodedPolyline": r"aaf{E`|y}T|Ftf@px\\hp e@`nnDd~f@zkmH",
-                "createdAt": "2015-08-04T20:48:08.000Z",
-                "updatedAt": "2015-08-04T20:48:08.000Z",
-                "tags": [
-                    "generated"
-                ],
-                "user": {
-                    "id": 2429,
-                    "username": "example",
-                    "gravatarHash": "f30b58b998a11b5d417cc2c78df3f764",
-                    "location": None
-                }
+        {
+            "id": 62373,
+            "fromICAO": "KLAS",
+            "toICAO": "KLAX",
+            "fromName": "Mc Carran Intl",
+            "toName": "Los Angeles Intl",
+            "flightNumber": None,
+            "distance": 206.39578816273502,
+            "maxAltitude": 18000,
+            "waypoints": 8,
+            "likes": 0,
+            "downloads": 1,
+            "popularity": 1,
+            "notes": "",
+            "encodedPolyline": r"aaf{E`|y}T|Ftf@px\\hp e@`nnDd~f@zkmH",
+            "createdAt": "2015-08-04T20:48:08.000Z",
+            "updatedAt": "2015-08-04T20:48:08.000Z",
+            "tags": ["generated"],
+            "user": {
+                "id": 2429,
+                "username": "example",
+                "gravatarHash": "f30b58b998a11b5d417cc2c78df3f764",
+                "location": None,
+            },
+        },
+        {
+            "id": 62493,
+            "fromICAO": "EHAM",
+            "toICAO": "KJFK",
+            "fromName": "Schiphol",
+            "toName": "John F Kennedy Intl",
+            "flightNumber": None,
+            "distance": 3157.88876623323,
+            "maxAltitude": 0,
+            "waypoints": 2,
+            "popularity": 0,
+            "notes": None,
+            "encodedPolyline": r"yvh~Hgi`\\lggfAjyi~M",
+            "createdAt": "2015-08-05T22:44:34.000Z",
+            "updatedAt": "2015-08-05T22:44:34.000Z",
+            "tags": ["atlantic"],
+            "user": {
+                "id": 1,
+                "username": "example",
+                "gravatarHash": "f30b58b998a11b5d417cc2c78df3f764",
+                "location": None,
             },
-            {
-                "id": 62493,
-                "fromICAO": "EHAM",
-                "toICAO": "KJFK",
-                "fromName": "Schiphol",
-                "toName": "John F Kennedy Intl",
-                "flightNumber": None,
-                "distance": 3157.88876623323,
-                "maxAltitude": 0,
-                "waypoints": 2,
-                "popularity": 0,
-                "notes": None,
-                "encodedPolyline": r"yvh~Hgi`\\lggfAjyi~M",
-                "createdAt": "2015-08-05T22:44:34.000Z",
-                "updatedAt": "2015-08-05T22:44:34.000Z",
-                "tags": ["atlantic"],
-                "user": {
-                    "id": 1,
-                    "username": "example",
-                    "gravatarHash": "f30b58b998a11b5d417cc2c78df3f764",
-                    "location": None
-                }
-            }
-        ]
+        },
+    ]
 
     correct_response_list = [
-            Plan(
-                id=62373,
-                fromICAO="KLAS",
-                toICAO="KLAX",
-                fromName="Mc Carran Intl",
-                toName="Los Angeles Intl",
-                flightNumber=None,
-                distance=206.39578816273502,
-                maxAltitude=18000,
-                waypoints=8,
-                likes=0,
-                downloads=1,
-                popularity=1,
-                notes="",
-                encodedPolyline=r"aaf{E`|y}T|Ftf@px\\hp e@`nnDd~f@zkmH",
-                createdAt="2015-08-04T20:48:08.000Z",
-                updatedAt="2015-08-04T20:48:08.000Z",
-                tags=[
-                    "generated"
-                ],
-                user=User(
-                    id=2429,
-                    username="example",
-                    gravatarHash="f30b58b998a11b5d417cc2c78df3f764",
-                    location=None
-                    )
-                ),
-            Plan(
-                id=62493,
-                fromICAO="EHAM",
-                toICAO="KJFK",
-                fromName="Schiphol",
-                toName="John F Kennedy Intl",
-                flightNumber=None,
-                distance=3157.88876623323,
-                maxAltitude=0,
-                waypoints=2,
-                popularity=0,
-                notes=None,
-                encodedPolyline=r"yvh~Hgi`\\lggfAjyi~M",
-                createdAt="2015-08-05T22:44:34.000Z",
-                updatedAt="2015-08-05T22:44:34.000Z",
-                tags=["atlantic"],
-                user=User(
-                    id=1,
-                    username="example",
-                    gravatarHash="f30b58b998a11b5d417cc2c78df3f764",
-                    location=None
-                    )
-                )
-        ]
-
-    correct_calls = [mock.call(
-        path='/user/lemon/likes',
-        limit=100,
-        sort='created',
-        key=None
-    )]
+        Plan(
+            id=62373,
+            fromICAO="KLAS",
+            toICAO="KLAX",
+            fromName="Mc Carran Intl",
+            toName="Los Angeles Intl",
+            flightNumber=None,
+            distance=206.39578816273502,
+            maxAltitude=18000,
+            waypoints=8,
+            likes=0,
+            downloads=1,
+            popularity=1,
+            notes="",
+            encodedPolyline=r"aaf{E`|y}T|Ftf@px\\hp e@`nnDd~f@zkmH",
+            createdAt="2015-08-04T20:48:08.000Z",
+            updatedAt="2015-08-04T20:48:08.000Z",
+            tags=["generated"],
+            user=User(
+                id=2429,
+                username="example",
+                gravatarHash="f30b58b998a11b5d417cc2c78df3f764",
+                location=None,
+            ),
+        ),
+        Plan(
+            id=62493,
+            fromICAO="EHAM",
+            toICAO="KJFK",
+            fromName="Schiphol",
+            toName="John F Kennedy Intl",
+            flightNumber=None,
+            distance=3157.88876623323,
+            maxAltitude=0,
+            waypoints=2,
+            popularity=0,
+            notes=None,
+            encodedPolyline=r"yvh~Hgi`\\lggfAjyi~M",
+            createdAt="2015-08-05T22:44:34.000Z",
+            updatedAt="2015-08-05T22:44:34.000Z",
+            tags=["atlantic"],
+            user=User(
+                id=1,
+                username="example",
+                gravatarHash="f30b58b998a11b5d417cc2c78df3f764",
+                location=None,
+            ),
+        ),
+    ]
+
+    correct_calls = [
+        mock.call(path="/user/lemon/likes", limit=100, sort="created", key=None)
+    ]
 
     patched_internal_getiter.return_value = AsyncIter(json_response)
 
     response = flightplandb.user.likes("lemon")
     # check that UserAPI method decoded data correctly for given response
     response_list = []
     async for i in response:
         response_list.append(i)
     assert response_list == correct_response_list
     # check that UserAPI method made correct request of FlightPlanDB
     patched_internal_getiter.assert_has_calls(correct_calls)
 
 
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.getiter")
 async def test_user_search(patched_internal_getiter):
     json_response = [
-            {"id": 1,
-                "username": 'lemon',
-                "location": '\U0001F601',
-                "gravatarHash": '7889b0d4380a7194b6b67c8e2765289d'},
-            {"id": 1851,
-                "username": 'lemon2',
-                "location": None,
-                "gravatarHash": '94ff72a00d4ead8c49abd5a0cf411c6f'},
-            {"id": 1950,
-                "username": 'lemon6',
-                "location": None,
-                "gravatarHash": 'b807060d00c10513ce04b70918dd07a1'}
-        ]
+        {
+            "id": 1,
+            "username": "lemon",
+            "location": "\U0001F601",
+            "gravatarHash": "7889b0d4380a7194b6b67c8e2765289d",
+        },
+        {
+            "id": 1851,
+            "username": "lemon2",
+            "location": None,
+            "gravatarHash": "94ff72a00d4ead8c49abd5a0cf411c6f",
+        },
+        {
+            "id": 1950,
+            "username": "lemon6",
+            "location": None,
+            "gravatarHash": "b807060d00c10513ce04b70918dd07a1",
+        },
+    ]
 
     correct_response_list = [
-            UserSmall(
-                id=1,
-                username='lemon',
-                location='\U0001F601',
-                gravatarHash='7889b0d4380a7194b6b67c8e2765289d'),
-            UserSmall(
-                id=1851,
-                username='lemon2',
-                location=None,
-                gravatarHash='94ff72a00d4ead8c49abd5a0cf411c6f'),
-            UserSmall(
-                id=1950,
-                username='lemon6',
-                location=None,
-                gravatarHash='b807060d00c10513ce04b70918dd07a1')
-        ]
+        UserSmall(
+            id=1,
+            username="lemon",
+            location="\U0001F601",
+            gravatarHash="7889b0d4380a7194b6b67c8e2765289d",
+        ),
+        UserSmall(
+            id=1851,
+            username="lemon2",
+            location=None,
+            gravatarHash="94ff72a00d4ead8c49abd5a0cf411c6f",
+        ),
+        UserSmall(
+            id=1950,
+            username="lemon6",
+            location=None,
+            gravatarHash="b807060d00c10513ce04b70918dd07a1",
+        ),
+    ]
 
-    correct_calls = [mock.call(
-        path='/search/users',
-        limit=100,
-        params={'q': 'lemon'},
-        key=None
-    )]
+    correct_calls = [
+        mock.call(path="/search/users", limit=100, params={"q": "lemon"}, key=None)
+    ]
 
     patched_internal_getiter.return_value = AsyncIter(json_response)
 
     response = flightplandb.user.search("lemon")
     # check that UserAPI method decoded data correctly for given response
     response_list = []
     async for i in response:
```

### Comparing `flightplandb-0.7.2/tests/test_weather.py` & `flightplandb-0.8.0/tests/test_weather.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from unittest import mock
+
 import pytest
+
 import flightplandb
 from flightplandb.datatypes import Weather
 
 
 # localhost is set on every test to allow async loops
-@pytest.mark.allow_hosts(['127.0.0.1', '::1'])
+@pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.get")
 async def test_weather_api(patched_internal_get):
     json_response = {
         "METAR": "EHAM 250755Z 02009KT 330V130 9999\
             BKN033 07/M00 Q1029 NOSIG",
         "TAF": "TAF EHAM 250442Z 2506/2612 02012KT 9999 BKN030 BECMG\
-            2507/2510 CAVOK BECMG 2608/2611 05009KT"
-        }
+            2507/2510 CAVOK BECMG 2608/2611 05009KT",
+    }
 
     correct_response = Weather(
         METAR="EHAM 250755Z 02009KT 330V130 9999\
             BKN033 07/M00 Q1029 NOSIG",
         TAF="TAF EHAM 250442Z 2506/2612 02012KT 9999 BKN030 BECMG\
-            2507/2510 CAVOK BECMG 2608/2611 05009KT"
-        )
+            2507/2510 CAVOK BECMG 2608/2611 05009KT",
+    )
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.weather.fetch("EHAM")
     # check that TagsAPI method made correct request of FlightPlanDB
-    patched_internal_get.assert_awaited_once_with(
-        path='/weather/EHAM', key=None
-    )
+    patched_internal_get.assert_awaited_once_with(path="/weather/EHAM", key=None)
     # check that TagsAPI method decoded data correctly for given response
     assert response == correct_response
```

