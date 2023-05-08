# Comparing `tmp/xtgeoviz-0.0.6.tar.gz` & `tmp/xtgeoviz-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtgeoviz-0.0.6.tar", last modified: Tue Apr 18 10:31:32 2023, max compression
+gzip compressed data, was "xtgeoviz-0.0.7.tar", last modified: Mon May  8 05:15:29 2023, max compression
```

## Comparing `xtgeoviz-0.0.6.tar` & `xtgeoviz-0.0.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.897888 xtgeoviz-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.github/workflows/ci-xtgeoviz.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.github/workflows/xtgeoviz-publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements_setup.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements_testx.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/scripts/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/scripts/setup_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.897888 xtgeoviz-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/src/xtgeoviz/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/src/xtgeoviz/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/xsectplotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/src/xtgeoviz/mpl/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/_colortables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/_libwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/baseplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/grid3d_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/quickplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    37790 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/xsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/xtmap.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.897888 xtgeoviz-0.0.6/tests/baseline_images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/baseline_images/test_baseplot/
--rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/baseline_images/test_baseplot/canvas.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/baseline_images/test_regularsurface/
--rw-r--r--   0 runner    (1001) docker     (123)    45755 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/baseline_images/test_regularsurface/quickplot1.png
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/test_mpl/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/test_mpl/test_baseplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/test_mpl/test_regularsurface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/test_scripts/test_xsectplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.950380 xtgeoviz-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.954380 xtgeoviz-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/.github/workflows/ci-xtgeoviz.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/.github/workflows/xtgeoviz-publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.954380 xtgeoviz-0.0.7/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.954380 xtgeoviz-0.0.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/requirements/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/requirements/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/requirements/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/requirements/requirements_testx.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.954380 xtgeoviz-0.0.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/scripts/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/scripts/setup_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.954380 xtgeoviz-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.954380 xtgeoviz-0.0.7/src/xtgeoviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/src/xtgeoviz/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/frontends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/frontends/_xsectplotting_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/frontends/_xsectplotting_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/frontends/_xsectplotting_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/frontends/xsectplotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/src/xtgeoviz/mpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/mpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/mpl/_colortables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/mpl/_libwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/mpl/baseplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/mpl/grid3d_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/mpl/quickplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37712 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/mpl/xsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/src/xtgeoviz/mpl/xtmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 05:15:29.000000 xtgeoviz-0.0.7/src/xtgeoviz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/src/xtgeoviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 05:15:29.000000 xtgeoviz-0.0.7/src/xtgeoviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-08 05:15:29.000000 xtgeoviz-0.0.7/src/xtgeoviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 05:15:29.000000 xtgeoviz-0.0.7/src/xtgeoviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-08 05:15:29.000000 xtgeoviz-0.0.7/src/xtgeoviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 05:15:29.000000 xtgeoviz-0.0.7/src/xtgeoviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.954380 xtgeoviz-0.0.7/tests/baseline_images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/tests/baseline_images/test_baseplot/
+-rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/tests/baseline_images/test_baseplot/canvas.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/tests/baseline_images/test_regularsurface/
+-rw-r--r--   0 runner    (1001) docker     (123)    45755 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/tests/baseline_images/test_regularsurface/quickplot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/tests/test_mpl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/tests/test_mpl/test_baseplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/tests/test_mpl/test_regularsurface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:15:29.958380 xtgeoviz-0.0.7/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-08 05:15:11.000000 xtgeoviz-0.0.7/tests/test_scripts/test_xsectplot.py
```

### Comparing `xtgeoviz-0.0.6/.github/workflows/ci-xtgeoviz.yml` & `xtgeoviz-0.0.7/.github/workflows/ci-xtgeoviz.yml`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/.github/workflows/xtgeoviz-publish-pypi.yml` & `xtgeoviz-0.0.7/.github/workflows/xtgeoviz-publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/.gitignore` & `xtgeoviz-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/.pylintrc` & `xtgeoviz-0.0.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/LICENSE` & `xtgeoviz-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/PKG-INFO` & `xtgeoviz-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtgeoviz
-Version: 0.0.6
+Version: 0.0.7
 Summary: Plotting library for xtgeo objects
 Home-page: https://github.com/equinor/xtgeoviz
 Author: Equinor
 Author-email: ____@equinor.com
 License: LGPL-3.0
 Project-URL: Documentation, https://xtgeoviz.notyet_on_readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/equinor/xtgeoviz/issues
```

### Comparing `xtgeoviz-0.0.6/docs/conf.py` & `xtgeoviz-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/pyproject.toml` & `xtgeoviz-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/scripts/setup_functions.py` & `xtgeoviz-0.0.7/scripts/setup_functions.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/setup.py` & `xtgeoviz-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_config.py` & `xtgeoviz-0.0.7/src/xtgeoviz/frontends/_xsectplotting_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 """Config option for xsections"""
 import logging
+import re
 from copy import deepcopy
 from typing import Optional, Union
 
 import six
 import yaml
 
 logger = logging.getLogger(__name__)
@@ -244,21 +245,38 @@
         newcfg_plt["wells"]["perflog"]["colordict"] = ddict
 
     if not oldcfg_plt["wells"]["zonelog"]["colordict"]:
         newcfg_plt["wells"]["zonelog"]["colordict"] = ddict
 
     # PROCESSING SMARTIES
     # ----------------------------------------------------------------------------------
-    if not newcfg_plt["design"]["zrange"]:
-        newcfg_plt["design"]["zrange"] = _config_smart0_zrange(prm)
+    _zrange = deepcopy(newcfg_plt["design"]["zrange"])
+    if not _zrange:
+        _zrange = "smart0"
+
+    if isinstance(_zrange, str):
+        if _zrange == "smart0":
+            newcfg_plt["design"]["zrange"] = _config_smart0_zrange(prm)
+        elif _zrange == "smart1":
+            newcfg_plt["design"]["zrange"] = _config_smart1_zrange(
+                self.wells["wlist"], prm
+            )
+    elif isinstance(_zrange, dict):
+        # process zrange per well, with a global default
+        newcfg_plt["design"]["zrange"] = _config_userdefined_zrange(
+            self.wells["wlist"], _zrange
+        )
+
+    elif isinstance(_zrange, list) and len(_zrange) == 2:
+        logger.info("Keep zrange as is")
 
-    if newcfg_plt["design"]["zrange"] == "smart1":
-        newcfg_plt["design"]["zrange"] = _config_smart1_zrange(self.wells["wlist"], prm)
+    else:
+        raise RuntimeError("Cannot process/understand the zrange for unknown reasons")
 
-    # RANGES
+    # Z RANGES
     # ----------------------------------------------------------------------------------
     if self.cube and not newcfg_plt["cube"]["range"]:
         newcfg_plt["cube"]["range"] = [self.cube.values.min(), self.cube.values.max()]
 
     if self.grid and not newcfg_plt["grid"]["range"]:
         newcfg_plt["grid"]["range"] = [
             self.gridproperty.values.min(),
@@ -296,14 +314,37 @@
 
     if maxwell < maxv:
         maxv = maxwell
 
     return [minv, maxv]
 
 
+def _config_userdefined_zrange(wlist: list, _zrange: dict) -> dict:
+    zrange_dict = {}
+
+    # first set default
+    for well in wlist:
+        zrange_dict[well.name] = _zrange["default"]
+        logger.info("Default: set %s zrange to %s", well.name, _zrange["default"])
+
+    # well name may be a regular expression
+    for wreg, intv in _zrange.items():
+        for well in wlist:
+            if re.match(wreg + "$", well.name):
+                zrange_dict[well.name] = intv
+                logger.info(
+                    "Override default: set %s zrange to %s, based on regex (%s$)",
+                    well.name,
+                    intv,
+                    wreg,
+                )
+
+    return zrange_dict
+
+
 def _config_default_surf_names(primary):
     """Config default surface name"""
     snames = []
     for ino, _surf in enumerate(primary):
         snames.append("SURF" + str(ino + 1))
 
     return snames
```

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_load.py` & `xtgeoviz-0.0.7/src/xtgeoviz/frontends/_xsectplotting_load.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,22 +107,27 @@
         logger.info("Read outline: %s", outline)
         self.outline = xtgeo.polygons_from_file(outline)
     elif isinstance(outline, xtgeo.Polygons):
         self.outline = outline
 
 
 def load_cube(self):
-    """Load a cube as XTGeo Cube object."""
+    """Apply a current cube or load a cube, both as XTGeo Cube"""
 
-    cubename = self.config["input"]["cube"]
+    cube = self.config["input"]["cube"]
 
-    if cubename:
-        logger.info("Reading cube: %s", cubename)
-        self.cube = xtgeo.cube_from_file(cubename)
+    if cube and isinstance(cube, str):
+        logger.info("Reading cube: %s", cube)
+        self.cube = xtgeo.cube_from_file(cube)
         logger.info("Reading cube done")
+    elif cube and isinstance(cube, xtgeo.Cube):
+        self.cube = cube
+        logger.info("Apply an existing Cube instance: %s", type(cube))
+    else:
+        self.cube = None
 
 
 def load_grid(self):
     """Load a grid with property"""
 
     gfile = self.config["input"]["grid"]["geometry"]
     pfile = self.config["input"]["grid"]["property"]["file"]
```

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_plotting.py` & `xtgeoviz-0.0.7/src/xtgeoviz/frontends/_xsectplotting_plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,17 +38,23 @@
 
     wellcross = _compute_wellcrossings(pset)
 
     plotfiles = []
 
     for well in self.wells["wlist"]:
         logger.info("Plot cross section for well %s", well.name)
+
+        if isinstance(pset.design_zrange, dict):
+            zrange_min, zrange_max = pset.design_zrange[well.name]
+        else:
+            zrange_min, zrange_max = pset.design_zrange
+
         xplot = XSection(
-            zmin=pset.design_zrange[0],
-            zmax=pset.design_zrange[1],
+            zmin=zrange_min,
+            zmax=zrange_max,
             well=well,
             surfaces=self.surfaces["primary"],
             zonelogshift=pset.wells_zonelog_zoneshift,
             outline=self.outline,
             colormap=pset.surf_primary_colors,
             cube=self.cube,
             grid=self.grid,
```

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/frontends/xsectplotting.py` & `xtgeoviz-0.0.7/src/xtgeoviz/frontends/xsectplotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argparse
 import json
 import logging
 import os.path
 import sys
 from dataclasses import dataclass, field
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 import xtgeo
 import yaml
 
 import xtgeoviz
 
 from . import _xsectplotting_config as _cfg
@@ -36,15 +36,15 @@
     """Class for storing plot settings for the plots"""
 
     title: str = "Generic Title"
 
     general_engine: str = "matplotlib"
 
     design_style: int = 1
-    design_zrange: tuple = (1000, 2000)
+    design_zrange: Union[tuple, list, dict] = (1000, 2000)
     design_gridlines: str = "both"
     design_subtitle: Optional[str] = None
     design_legendsize: int = 6
     design_legends: bool = True
     design_dpi: int = 100
 
     wellmap_otherwells: bool = False
@@ -284,15 +284,15 @@
     """
 
     app = _Xsections(args, inputdata, plotsettings, output, verbosity)
 
     # load what to xsect (and show):
     app.load_wells()
     app.load_surfaces()
-    # app.load_cube()
+    app.load_cube()
     # app.load_grid()
     app.load_outline()
 
     app.config_complete()
 
     app.plotsettings.update_plotsettings(app.config)
```

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/mpl/_colortables.py` & `xtgeoviz-0.0.7/src/xtgeoviz/mpl/_colortables.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/mpl/_libwrapper.py` & `xtgeoviz-0.0.7/src/xtgeoviz/mpl/_libwrapper.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/mpl/baseplot.py` & `xtgeoviz-0.0.7/src/xtgeoviz/mpl/baseplot.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/mpl/grid3d_slice.py` & `xtgeoviz-0.0.7/src/xtgeoviz/mpl/grid3d_slice.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/mpl/quickplot.py` & `xtgeoviz-0.0.7/src/xtgeoviz/mpl/quickplot.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/mpl/xsection.py` & `xtgeoviz-0.0.7/src/xtgeoviz/mpl/xsection.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,16 +267,15 @@
             plt.rcParams["axes.titlecolor"] = (0, 0, 0, 0)
             plt.rcParams["axes.edgecolor"] = (0, 0, 0, 0)
             plt.rcParams["axes.labelcolor"] = (0, 0, 0, 0)
             plt.rcParams["axes.titlecolor"] = (0, 0, 0, 0)
             plt.rcParams["xtick.color"] = (0, 0, 0, 0)
             plt.rcParams["ytick.color"] = (0, 0, 0, 0)
 
-        # self._fig, (ax1, ax2) = plt.subplots(2, figsize=(11.69, 8.27))
-        self._fig, _ = plt.subplots(figsize=(11.69 * figscaling, 8.27 * figscaling))
+        self._fig = plt.figure(figsize=(11.69 * figscaling, 8.27 * figscaling))
         ax1 = OrderedDict()
 
         ax1["main"] = plt.subplot2grid((20, 28), (0, 0), rowspan=20, colspan=23)
 
         ax2 = plt.subplot2grid(
             (20, 28), (10, 23), rowspan=5, colspan=5, frame_on=self._has_legend
         )
```

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz/mpl/xtmap.py` & `xtgeoviz-0.0.7/src/xtgeoviz/mpl/xtmap.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz.egg-info/PKG-INFO` & `xtgeoviz-0.0.7/src/xtgeoviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtgeoviz
-Version: 0.0.6
+Version: 0.0.7
 Summary: Plotting library for xtgeo objects
 Home-page: https://github.com/equinor/xtgeoviz
 Author: Equinor
 Author-email: ____@equinor.com
 License: LGPL-3.0
 Project-URL: Documentation, https://xtgeoviz.notyet_on_readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/equinor/xtgeoviz/issues
```

### Comparing `xtgeoviz-0.0.6/src/xtgeoviz.egg-info/SOURCES.txt` & `xtgeoviz-0.0.7/src/xtgeoviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/tests/baseline_images/test_baseplot/canvas.png` & `xtgeoviz-0.0.7/tests/baseline_images/test_baseplot/canvas.png`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/tests/baseline_images/test_regularsurface/quickplot1.png` & `xtgeoviz-0.0.7/tests/baseline_images/test_regularsurface/quickplot1.png`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/tests/test_mpl/test_baseplot.py` & `xtgeoviz-0.0.7/tests/test_mpl/test_baseplot.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/tests/test_mpl/test_regularsurface.py` & `xtgeoviz-0.0.7/tests/test_mpl/test_regularsurface.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.6/tests/test_scripts/test_xsectplot.py` & `xtgeoviz-0.0.7/tests/test_scripts/test_xsectplot.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from xtgeoviz.frontends._xsectplotting_config import config_defaults, data_merge
 from xtgeoviz.frontends.xsectplotting import _Xsections, _XsectSettings
 
 # testdata (xtgeo-testdata), relative to testdir
 WELLSET1 = "wells/drogon/1"
 SURFACESET1 = "surfaces/drogon/1"
 OUTLINE = "polygons/reek/1/closedpoly1.pol"
+CUBE = "cubes/drogon/ampl_local_a4.segy"
 
 
 def test_xsectplotting_config_defaults():
     """Test _xsectplottings_config() config_defaults method."""
 
     yamlresult = config_defaults()
     assert isinstance(yamlresult, str)
@@ -175,12 +176,80 @@
         },
     }
 
     outputs = {
         "plotfolder": str(tmp_path),
         "format": "png",
     }
+
+    # call the top plotter routine
+    xsectplot(inputdata=inputs, plotsettings=psettings, output=outputs)
+    myplot = tmp_path / "55_33-A-4.png"
+    assert myplot.is_file()
+
+
+def test_xsectplot_function_include_cube(testdir, tmp_path):
+    """Make plots using python input, where wells and surfaces are preloaded."""
+
+    wells = ["55_33-A-4.rmswell"]
+    surfaces = [
+        "01_topvolantis.gri",
+        "02_toptherys.gri",
+        "03_topvolon.gri",
+        "04_basevolantis.gri",
+    ]
+
+    wlist = []
+    for well in wells:
+        wlist.append(xtgeo.well_from_file(testdir / WELLSET1 / well))
+
+    slist = []
+    for surf in surfaces:
+        slist.append(xtgeo.surface_from_file(testdir / SURFACESET1 / surf))
+
+    cube = xtgeo.cube_from_file(testdir / CUBE)
+
+    inputs = {
+        "wells": {
+            "objects": wlist,
+            "zonelog": "Zone",
+        },
+        "surfaces": {
+            "primary": {
+                "objects": slist,
+                "names": ["TopVolantis", "TopTherys", "TopVolon", "BaseVolantis"],
+            },
+        },
+        "cube": cube,
+    }
+    psettings = {
+        "design": {
+            "zrange": {
+                "default": [1000, 2000],
+                "55_33.*": [1450, 1750],  # use a python regex for multiple wells
+            },
+        },
+        "wells": {
+            "zonelog": {
+                "zoneshift": 0,
+            }
+        },
+        "surfaces": {
+            "primary": {
+                "fill": False,
+            },
+        },
+        "cube": {
+            "range": [-0.33, 0.33],
+            "sampling": "trilinear",
+        },
+    }
+
+    outputs = {
+        "plotfolder": str(tmp_path),
+        "format": "png",
+    }
 
     # call the top plotter routine
     xsectplot(inputdata=inputs, plotsettings=psettings, output=outputs)
     myplot = tmp_path / "55_33-A-4.png"
     assert myplot.is_file()
```

