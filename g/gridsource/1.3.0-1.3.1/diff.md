# Comparing `tmp/gridsource-1.3.0.tar.gz` & `tmp/gridsource-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridsource-1.3.0.tar", last modified: Tue Oct 18 10:23:34 2022, max compression
+gzip compressed data, was "gridsource-1.3.1.tar", last modified: Mon May  8 05:48:48 2023, max compression
```

## Comparing `gridsource-1.3.0.tar` & `gridsource-1.3.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.613900 gridsource-1.3.0/
--rw-r--r--   0 nic       (1000) nic       (1000)      153 2020-10-29 10:19:52.000000 gridsource-1.3.0/AUTHORS.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      221 2020-10-26 10:06:34.000000 gridsource-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       89 2020-10-26 10:06:34.000000 gridsource-1.3.0/HISTORY.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1074 2020-10-26 10:06:34.000000 gridsource-1.3.0/LICENSE
--rw-r--r--   0 nic       (1000) nic       (1000)      316 2020-10-26 10:06:34.000000 gridsource-1.3.0/MANIFEST.in
--rw-rw-r--   0 nic       (1000) nic       (1000)     1019 2022-10-18 10:23:34.613900 gridsource-1.3.0/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)      138 2020-10-29 10:07:21.000000 gridsource-1.3.0/README.rst
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.605900 gridsource-1.3.0/docs/
--rw-r--r--   0 nic       (1000) nic       (1000)      611 2020-10-26 10:06:34.000000 gridsource-1.3.0/docs/Makefile
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.597900 gridsource-1.3.0/docs/_build/
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.597900 gridsource-1.3.0/docs/_build/html/
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.605900 gridsource-1.3.0/docs/_build/html/_static/
--rw-r--r--   0 nic       (1000) nic       (1000)      286 2020-08-14 11:51:16.000000 gridsource-1.3.0/docs/_build/html/_static/file.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2020-08-14 11:51:16.000000 gridsource-1.3.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2020-08-14 11:51:16.000000 gridsource-1.3.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2020-10-26 10:06:34.000000 gridsource-1.3.0/docs/authors.rst
--rwxr-xr-x   0 nic       (1000) nic       (1000)     4926 2020-10-26 10:06:34.000000 gridsource-1.3.0/docs/conf.py
--rw-r--r--   0 nic       (1000) nic       (1000)       33 2020-10-26 10:06:34.000000 gridsource-1.3.0/docs/contributing.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      130 2020-10-29 09:13:53.000000 gridsource-1.3.0/docs/gridsource.cli.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      127 2020-10-29 09:13:53.000000 gridsource-1.3.0/docs/gridsource.io.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      267 2020-10-29 09:19:10.000000 gridsource-1.3.0/docs/gridsource.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      151 2020-10-29 09:13:53.000000 gridsource-1.3.0/docs/gridsource.validation.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2020-10-26 10:06:34.000000 gridsource-1.3.0/docs/history.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      307 2020-10-26 10:06:34.000000 gridsource-1.3.0/docs/index.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      102 2020-10-26 10:06:34.000000 gridsource-1.3.0/docs/installation.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      772 2020-10-26 10:06:34.000000 gridsource-1.3.0/docs/make.bat
--rw-r--r--   0 nic       (1000) nic       (1000)       67 2020-10-29 09:19:10.000000 gridsource-1.3.0/docs/modules.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       27 2020-10-26 10:06:34.000000 gridsource-1.3.0/docs/readme.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      185 2020-10-29 09:22:30.000000 gridsource-1.3.0/docs/usage.rst
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.605900 gridsource-1.3.0/gridsource/
--rw-r--r--   0 nic       (1000) nic       (1000)     1314 2022-10-18 10:23:18.000000 gridsource-1.3.0/gridsource/__init__.py
--rw-rw-r--   0 nic       (1000) nic       (1000)    28558 2022-07-08 10:22:51.000000 gridsource-1.3.0/gridsource/autodoc.py
--rw-r--r--   0 nic       (1000) nic       (1000)     5975 2022-01-29 10:13:41.000000 gridsource-1.3.0/gridsource/cli.py
--rw-r--r--   0 nic       (1000) nic       (1000)    13827 2022-08-02 07:33:15.000000 gridsource-1.3.0/gridsource/io.py
--rw-r--r--   0 nic       (1000) nic       (1000)    34585 2022-09-28 08:00:58.000000 gridsource-1.3.0/gridsource/validation.py
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.609900 gridsource-1.3.0/gridsource.egg-info/
--rw-rw-r--   0 nic       (1000) nic       (1000)     1019 2022-10-18 10:23:34.000000 gridsource-1.3.0/gridsource.egg-info/PKG-INFO
--rw-rw-r--   0 nic       (1000) nic       (1000)     1936 2022-10-18 10:23:34.000000 gridsource-1.3.0/gridsource.egg-info/SOURCES.txt
--rw-rw-r--   0 nic       (1000) nic       (1000)        1 2022-10-18 10:23:34.000000 gridsource-1.3.0/gridsource.egg-info/dependency_links.txt
--rw-rw-r--   0 nic       (1000) nic       (1000)       49 2022-10-18 10:23:34.000000 gridsource-1.3.0/gridsource.egg-info/entry_points.txt
--rw-rw-r--   0 nic       (1000) nic       (1000)        1 2022-10-18 10:23:34.000000 gridsource-1.3.0/gridsource.egg-info/not-zip-safe
--rw-rw-r--   0 nic       (1000) nic       (1000)      103 2022-10-18 10:23:34.000000 gridsource-1.3.0/gridsource.egg-info/requires.txt
--rw-rw-r--   0 nic       (1000) nic       (1000)       11 2022-10-18 10:23:34.000000 gridsource-1.3.0/gridsource.egg-info/top_level.txt
--rw-rw-r--   0 nic       (1000) nic       (1000)      103 2021-12-22 07:57:34.000000 gridsource-1.3.0/requirements.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      201 2020-10-29 10:04:15.000000 gridsource-1.3.0/requirements_dev.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      530 2022-10-18 10:23:34.617900 gridsource-1.3.0/setup.cfg
--rw-r--r--   0 nic       (1000) nic       (1000)     1498 2022-10-18 10:23:18.000000 gridsource-1.3.0/setup.py
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.609900 gridsource-1.3.0/tests/
--rw-r--r--   0 nic       (1000) nic       (1000)       65 2020-10-26 10:06:34.000000 gridsource-1.3.0/tests/__init__.py
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.609900 gridsource-1.3.0/tests/_out/
--rw-rw-r--   0 nic       (1000) nic       (1000)      541 2022-10-18 10:22:13.000000 gridsource-1.3.0/tests/_out/test_00.ini
--rw-rw-r--   0 nic       (1000) nic       (1000)     6467 2022-10-18 10:22:13.000000 gridsource-1.3.0/tests/_out/test_00.xlsx
-drwxrwxr-x   0 nic       (1000) nic       (1000)        0 2022-10-18 10:23:34.613900 gridsource-1.3.0/tests/data/
--rw-rw-r--   0 nic       (1000) nic       (1000)     7979 2021-06-09 06:25:13.000000 gridsource-1.3.0/tests/data/ftools_example.yaml
--rw-rw-r--   0 nic       (1000) nic       (1000)      631 2021-06-09 06:25:13.000000 gridsource-1.3.0/tests/data/ftools_example_units.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      643 2020-10-26 10:06:34.000000 gridsource-1.3.0/tests/data/test_00.schema.json
--rw-r--r--   0 nic       (1000) nic       (1000)      443 2020-11-10 07:39:01.000000 gridsource-1.3.0/tests/data/test_00.schema.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      445 2020-10-26 10:06:34.000000 gridsource-1.3.0/tests/data/test_00.schema2.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     7247 2020-11-09 16:30:17.000000 gridsource-1.3.0/tests/data/test_00.xlsx
--rw-r--r--   0 nic       (1000) nic       (1000)      521 2020-10-29 15:08:45.000000 gridsource-1.3.0/tests/data/test_01.schema2.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     7218 2020-10-29 14:49:03.000000 gridsource-1.3.0/tests/data/test_01.xlsx
--rw-r--r--   0 nic       (1000) nic       (1000)      541 2020-11-10 14:25:36.000000 gridsource-1.3.0/tests/data/test_02.schema.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     7396 2020-10-30 11:55:37.000000 gridsource-1.3.0/tests/data/test_02.xlsx
--rw-r--r--   0 nic       (1000) nic       (1000)      320 2020-11-11 11:19:15.000000 gridsource-1.3.0/tests/data/test_03_units.ini
--rw-r--r--   0 nic       (1000) nic       (1000)      301 2020-11-11 06:24:14.000000 gridsource-1.3.0/tests/data/test_03_units.schema.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     5233 2020-11-11 11:02:26.000000 gridsource-1.3.0/tests/data/test_03_units.xlsx
--rw-r--r--   0 nic       (1000) nic       (1000)      196 2020-11-23 12:07:46.000000 gridsource-1.3.0/tests/data/test_04_IMP.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      170 2020-11-20 09:01:17.000000 gridsource-1.3.0/tests/data/test_04_SI.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     1253 2020-11-23 10:28:32.000000 gridsource-1.3.0/tests/data/test_04_data.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     9964 2020-11-20 18:02:34.000000 gridsource-1.3.0/tests/data/test_04_units.xlsx
--rw-r--r--   0 nic       (1000) nic       (1000)     9603 2020-11-20 11:48:10.000000 gridsource-1.3.0/tests/data/test_04_units_failing.xlsx
--rw-r--r--   0 nic       (1000) nic       (1000)      170 2020-11-20 09:01:17.000000 gridsource-1.3.0/tests/data/test_05_SI.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      342 2020-11-24 08:51:21.000000 gridsource-1.3.0/tests/data/test_05_data.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     4994 2020-11-22 08:26:19.000000 gridsource-1.3.0/tests/data/test_05_units_failing.xlsx
--rw-r--r--   0 nic       (1000) nic       (1000)      541 2021-01-26 14:44:56.000000 gridsource-1.3.0/tests/data/test_06_data.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     3396 2021-01-26 14:53:27.000000 gridsource-1.3.0/tests/data/test_06_multi-columns_uniqueness.ini
--rw-rw-r--   0 nic       (1000) nic       (1000)     7793 2021-07-16 06:59:37.000000 gridsource-1.3.0/tests/data/test_06_must_exist_in.xlsx
--rw-r--r--   0 nic       (1000) nic       (1000)      565 2021-10-18 12:23:26.000000 gridsource-1.3.0/tests/data/test_06_must_exist_in.yaml
--rw-rw-r--   0 nic       (1000) nic       (1000)     8205 2022-01-29 09:42:56.000000 gridsource-1.3.0/tests/data/test_10_mandatory_if.xlsx
--rw-r--r--   0 nic       (1000) nic       (1000)      689 2022-01-29 09:42:39.000000 gridsource-1.3.0/tests/data/test_10_mandatory_if.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      643 2020-10-26 10:06:34.000000 gridsource-1.3.0/tests/data/test_11.schema.json
--rw-r--r--   0 nic       (1000) nic       (1000)      443 2020-11-10 07:39:01.000000 gridsource-1.3.0/tests/data/test_11.schema.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     7140 2022-03-16 09:59:37.000000 gridsource-1.3.0/tests/data/test_11.xlsx
--rw-rw-r--   0 nic       (1000) nic       (1000)     1816 2022-01-29 10:13:41.000000 gridsource-1.3.0/tests/test_autodoc.py
--rw-r--r--   0 nic       (1000) nic       (1000)     2255 2022-01-02 11:00:58.000000 gridsource-1.3.0/tests/test_io.py
--rw-r--r--   0 nic       (1000) nic       (1000)    29431 2022-09-28 08:00:42.000000 gridsource-1.3.0/tests/test_validation.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.153242 gridsource-1.3.1/
+-rw-r--r--   0 nic       (1001) nic       (1001)      153 2020-10-29 10:19:52.000000 gridsource-1.3.1/AUTHORS.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      221 2020-10-26 10:06:34.000000 gridsource-1.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       89 2020-10-26 10:06:34.000000 gridsource-1.3.1/HISTORY.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)     1074 2020-10-26 10:06:34.000000 gridsource-1.3.1/LICENSE
+-rw-r--r--   0 nic       (1001) nic       (1001)      316 2020-10-26 10:06:34.000000 gridsource-1.3.1/MANIFEST.in
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1019 2023-05-08 05:48:48.153242 gridsource-1.3.1/PKG-INFO
+-rw-r--r--   0 nic       (1001) nic       (1001)      138 2020-10-29 10:07:21.000000 gridsource-1.3.1/README.rst
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.141242 gridsource-1.3.1/docs/
+-rw-r--r--   0 nic       (1001) nic       (1001)      611 2020-10-26 10:06:34.000000 gridsource-1.3.1/docs/Makefile
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.133242 gridsource-1.3.1/docs/_build/
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.133242 gridsource-1.3.1/docs/_build/html/
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.141242 gridsource-1.3.1/docs/_build/html/_static/
+-rw-r--r--   0 nic       (1001) nic       (1001)      286 2020-08-14 11:51:16.000000 gridsource-1.3.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 nic       (1001) nic       (1001)       90 2020-08-14 11:51:16.000000 gridsource-1.3.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 nic       (1001) nic       (1001)       90 2020-08-14 11:51:16.000000 gridsource-1.3.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 nic       (1001) nic       (1001)       28 2020-10-26 10:06:34.000000 gridsource-1.3.1/docs/authors.rst
+-rwxr-xr-x   0 nic       (1001) nic       (1001)     4926 2020-10-26 10:06:34.000000 gridsource-1.3.1/docs/conf.py
+-rw-r--r--   0 nic       (1001) nic       (1001)       33 2020-10-26 10:06:34.000000 gridsource-1.3.1/docs/contributing.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      130 2020-10-29 09:13:53.000000 gridsource-1.3.1/docs/gridsource.cli.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      127 2020-10-29 09:13:53.000000 gridsource-1.3.1/docs/gridsource.io.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      267 2020-10-29 09:19:10.000000 gridsource-1.3.1/docs/gridsource.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      151 2020-10-29 09:13:53.000000 gridsource-1.3.1/docs/gridsource.validation.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       28 2020-10-26 10:06:34.000000 gridsource-1.3.1/docs/history.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      307 2020-10-26 10:06:34.000000 gridsource-1.3.1/docs/index.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      102 2020-10-26 10:06:34.000000 gridsource-1.3.1/docs/installation.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      772 2020-10-26 10:06:34.000000 gridsource-1.3.1/docs/make.bat
+-rw-r--r--   0 nic       (1001) nic       (1001)       67 2020-10-29 09:19:10.000000 gridsource-1.3.1/docs/modules.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       27 2020-10-26 10:06:34.000000 gridsource-1.3.1/docs/readme.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      185 2020-10-29 09:22:30.000000 gridsource-1.3.1/docs/usage.rst
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.141242 gridsource-1.3.1/gridsource/
+-rw-r--r--   0 nic       (1001) nic       (1001)     1314 2023-04-18 08:54:44.000000 gridsource-1.3.1/gridsource/__init__.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    28558 2022-07-08 10:22:51.000000 gridsource-1.3.1/gridsource/autodoc.py
+-rw-r--r--   0 nic       (1001) nic       (1001)     5975 2022-01-29 10:13:41.000000 gridsource-1.3.1/gridsource/cli.py
+-rw-r--r--   0 nic       (1001) nic       (1001)    13827 2022-08-02 07:33:15.000000 gridsource-1.3.1/gridsource/io.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    34649 2023-05-02 09:42:07.000000 gridsource-1.3.1/gridsource/validation.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.141242 gridsource-1.3.1/gridsource.egg-info/
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1019 2023-05-08 05:48:48.000000 gridsource-1.3.1/gridsource.egg-info/PKG-INFO
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1936 2023-05-08 05:48:48.000000 gridsource-1.3.1/gridsource.egg-info/SOURCES.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-05-08 05:48:48.000000 gridsource-1.3.1/gridsource.egg-info/dependency_links.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)       49 2023-05-08 05:48:48.000000 gridsource-1.3.1/gridsource.egg-info/entry_points.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-05-08 05:48:48.000000 gridsource-1.3.1/gridsource.egg-info/not-zip-safe
+-rw-rw-r--   0 nic       (1001) nic       (1001)      103 2023-05-08 05:48:48.000000 gridsource-1.3.1/gridsource.egg-info/requires.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)       11 2023-05-08 05:48:48.000000 gridsource-1.3.1/gridsource.egg-info/top_level.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)      103 2021-12-22 07:57:34.000000 gridsource-1.3.1/requirements.txt
+-rw-r--r--   0 nic       (1001) nic       (1001)      201 2020-10-29 10:04:15.000000 gridsource-1.3.1/requirements_dev.txt
+-rw-r--r--   0 nic       (1001) nic       (1001)      530 2023-05-08 05:48:48.153242 gridsource-1.3.1/setup.cfg
+-rw-r--r--   0 nic       (1001) nic       (1001)     1498 2023-04-18 08:54:44.000000 gridsource-1.3.1/setup.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.141242 gridsource-1.3.1/tests/
+-rw-r--r--   0 nic       (1001) nic       (1001)       65 2020-10-26 10:06:34.000000 gridsource-1.3.1/tests/__init__.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.145242 gridsource-1.3.1/tests/_out/
+-rw-rw-r--   0 nic       (1001) nic       (1001)      541 2023-05-02 08:33:21.000000 gridsource-1.3.1/tests/_out/test_00.ini
+-rw-rw-r--   0 nic       (1001) nic       (1001)     6467 2023-05-02 08:33:21.000000 gridsource-1.3.1/tests/_out/test_00.xlsx
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-08 05:48:48.153242 gridsource-1.3.1/tests/data/
+-rw-rw-r--   0 nic       (1001) nic       (1001)     7979 2021-06-09 06:25:13.000000 gridsource-1.3.1/tests/data/ftools_example.yaml
+-rw-rw-r--   0 nic       (1001) nic       (1001)      631 2021-06-09 06:25:13.000000 gridsource-1.3.1/tests/data/ftools_example_units.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)      643 2020-10-26 10:06:34.000000 gridsource-1.3.1/tests/data/test_00.schema.json
+-rw-r--r--   0 nic       (1001) nic       (1001)      443 2020-11-10 07:39:01.000000 gridsource-1.3.1/tests/data/test_00.schema.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)      445 2020-10-26 10:06:34.000000 gridsource-1.3.1/tests/data/test_00.schema2.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)     7247 2020-11-09 16:30:17.000000 gridsource-1.3.1/tests/data/test_00.xlsx
+-rw-r--r--   0 nic       (1001) nic       (1001)      521 2020-10-29 15:08:45.000000 gridsource-1.3.1/tests/data/test_01.schema2.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)     7218 2020-10-29 14:49:03.000000 gridsource-1.3.1/tests/data/test_01.xlsx
+-rw-r--r--   0 nic       (1001) nic       (1001)      541 2020-11-10 14:25:36.000000 gridsource-1.3.1/tests/data/test_02.schema.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)     7396 2020-10-30 11:55:37.000000 gridsource-1.3.1/tests/data/test_02.xlsx
+-rw-r--r--   0 nic       (1001) nic       (1001)      320 2020-11-11 11:19:15.000000 gridsource-1.3.1/tests/data/test_03_units.ini
+-rw-r--r--   0 nic       (1001) nic       (1001)      301 2020-11-11 06:24:14.000000 gridsource-1.3.1/tests/data/test_03_units.schema.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)     5233 2020-11-11 11:02:26.000000 gridsource-1.3.1/tests/data/test_03_units.xlsx
+-rw-r--r--   0 nic       (1001) nic       (1001)      196 2020-11-23 12:07:46.000000 gridsource-1.3.1/tests/data/test_04_IMP.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)      170 2020-11-20 09:01:17.000000 gridsource-1.3.1/tests/data/test_04_SI.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)     1253 2020-11-23 10:28:32.000000 gridsource-1.3.1/tests/data/test_04_data.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)     9964 2020-11-20 18:02:34.000000 gridsource-1.3.1/tests/data/test_04_units.xlsx
+-rw-r--r--   0 nic       (1001) nic       (1001)     9603 2020-11-20 11:48:10.000000 gridsource-1.3.1/tests/data/test_04_units_failing.xlsx
+-rw-r--r--   0 nic       (1001) nic       (1001)      170 2020-11-20 09:01:17.000000 gridsource-1.3.1/tests/data/test_05_SI.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)      342 2020-11-24 08:51:21.000000 gridsource-1.3.1/tests/data/test_05_data.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)     4994 2020-11-22 08:26:19.000000 gridsource-1.3.1/tests/data/test_05_units_failing.xlsx
+-rw-r--r--   0 nic       (1001) nic       (1001)      541 2021-01-26 14:44:56.000000 gridsource-1.3.1/tests/data/test_06_data.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)     3396 2021-01-26 14:53:27.000000 gridsource-1.3.1/tests/data/test_06_multi-columns_uniqueness.ini
+-rw-rw-r--   0 nic       (1001) nic       (1001)     7793 2021-07-16 06:59:37.000000 gridsource-1.3.1/tests/data/test_06_must_exist_in.xlsx
+-rw-r--r--   0 nic       (1001) nic       (1001)      565 2021-10-18 12:23:26.000000 gridsource-1.3.1/tests/data/test_06_must_exist_in.yaml
+-rw-rw-r--   0 nic       (1001) nic       (1001)     8205 2022-01-29 09:42:56.000000 gridsource-1.3.1/tests/data/test_10_mandatory_if.xlsx
+-rw-r--r--   0 nic       (1001) nic       (1001)      689 2022-01-29 09:42:39.000000 gridsource-1.3.1/tests/data/test_10_mandatory_if.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)      643 2020-10-26 10:06:34.000000 gridsource-1.3.1/tests/data/test_11.schema.json
+-rw-r--r--   0 nic       (1001) nic       (1001)      443 2020-11-10 07:39:01.000000 gridsource-1.3.1/tests/data/test_11.schema.yaml
+-rw-r--r--   0 nic       (1001) nic       (1001)     7140 2022-03-16 09:59:37.000000 gridsource-1.3.1/tests/data/test_11.xlsx
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1816 2022-01-29 10:13:41.000000 gridsource-1.3.1/tests/test_autodoc.py
+-rw-r--r--   0 nic       (1001) nic       (1001)     2255 2022-01-02 11:00:58.000000 gridsource-1.3.1/tests/test_io.py
+-rw-r--r--   0 nic       (1001) nic       (1001)    29431 2022-09-28 08:00:42.000000 gridsource-1.3.1/tests/test_validation.py
```

### Comparing `gridsource-1.3.0/LICENSE` & `gridsource-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/PKG-INFO` & `gridsource-1.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gridsource
-Version: 1.3.0
+Version: 1.3.1
 Summary: Data mining with XLSX, cfg, json, etc.
 Home-page: https://framagit.org/numenic/gridsource
 Author: numenic
 Author-email: info@numeric-gmbh.ch
 License: MIT license
 Description: ==========
         GridSource
```

### Comparing `gridsource-1.3.0/docs/Makefile` & `gridsource-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/docs/conf.py` & `gridsource-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/docs/make.bat` & `gridsource-1.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/gridsource/__init__.py` & `gridsource-1.3.1/gridsource/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Top-level package for GridSource."""
 
 from gridsource.io import IOMixin
 from gridsource.validation import ValidatorMixin
 
 __author__ = """Nicolas Cordier"""
 __email__ = "nicolas.cordier@numeric-gmbh.ch"
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 
 class _Base:
     def __init__(self):
         self._data = {}
         possible_mixins_init = ("validator_mixin_init", "io_mixin_init")
         for f in possible_mixins_init:
```

### Comparing `gridsource-1.3.0/gridsource/autodoc.py` & `gridsource-1.3.1/gridsource/autodoc.py`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/gridsource/cli.py` & `gridsource-1.3.1/gridsource/cli.py`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/gridsource/io.py` & `gridsource-1.3.1/gridsource/io.py`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/gridsource/validation.py` & `gridsource-1.3.1/gridsource/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,24 +514,27 @@
             k: v for k, v in _fillnas.items() if k in df.columns and v is not None
         }
         if fillnas:
             df = df.fillna(value=fillnas, downcast="infer")
         if padded_columns:
             df = df.replace({"_pad_": np.nan})
             df[padded_columns] = df[padded_columns].fillna(method="pad")
-            # df = df.fillna(method="pad",
         # =====================================================================
         # build dummy columns if required by the multiple-columns uniqueness
         # =====================================================================
         dummies = []
         for uniqueness_tag, columns in self.uniqueness_sets.items():
             _df = df[columns].fillna(method="ffill").astype(str)
             dummy_col = UNIQUENESS_SEP.join(columns)
             dummies.append(dummy_col)  # to delete them later on
-            df[dummy_col] = _df.apply(UNIQUENESS_SEP.join, axis=1)
+            _c = _df.apply(UNIQUENESS_SEP.join, axis=1)
+            if len(_c) > 0:
+                df[dummy_col] = _c
+            else:
+                df[dummy_col] = None
         # =====================================================================
         # second validation
         # =====================================================================
         # df -> dict -> json -> dict to convert NaN to None
         report = _validate(
             json.loads(json.dumps(df.to_dict(orient="list"), ignore_nan=True)),
             validator=validator,
```

### Comparing `gridsource-1.3.0/gridsource.egg-info/PKG-INFO` & `gridsource-1.3.1/gridsource.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gridsource
-Version: 1.3.0
+Version: 1.3.1
 Summary: Data mining with XLSX, cfg, json, etc.
 Home-page: https://framagit.org/numenic/gridsource
 Author: numenic
 Author-email: info@numeric-gmbh.ch
 License: MIT license
 Description: ==========
         GridSource
```

### Comparing `gridsource-1.3.0/gridsource.egg-info/SOURCES.txt` & `gridsource-1.3.1/gridsource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/setup.cfg` & `gridsource-1.3.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.3.0
+current_version = 1.3.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `gridsource-1.3.0/setup.py` & `gridsource-1.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,11 +45,11 @@
     include_package_data=True,
     keywords="gridsource",
     name="gridsource",
     packages=find_packages(include=["gridsource", "gridsource.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
-    version="1.3.0",
+    version="1.3.1",
     zip_safe=False,
     url="https://framagit.org/numenic/gridsource",
 )
```

### Comparing `gridsource-1.3.0/tests/_out/test_00.ini` & `gridsource-1.3.1/tests/_out/test_00.ini`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/_out/test_00.xlsx` & `gridsource-1.3.1/tests/_out/test_00.xlsx`

 * *Files 8% similar despite different names*

```diff
@@ -300,35 +300,35 @@
 000012b0: 5bfb 519b c2e1 0365 5fd0 b8a9 f0d9 62be  [.Q....e_.....b.
 000012c0: 1df0 0388 3e9a 4f94 0812 f152 ab2c bff9  ....>.O....R.,..
 000012d0: e610 746e 69c6 65ac fed9 316a 1182 d68a  ..tni.e...1j....
 000012e0: 785f e4f0 a939 bbb1 c2d9 678b 7b73 677b  x_...9....g.{sg{
 000012f0: 065f 7b67 bbda 5e2e 515b 3bc8 e4ab a53f  ._{g..^.Q[;....?
 00001300: 9ef8 f03e c8de 8183 d284 2959 bc4d 7a00  ...>......)Y.Mz.
 00001310: 47cd eeec 2f03 e063 2f48 b7fe 0650 4b03  G.../..c/H...PK.
-00001320: 0414 0000 0008 0000 003f 00bd 4caf 8024  .........?..L..$
+00001320: 0414 0000 0008 0000 003f 00be b967 ee24  .........?...g.$
 00001330: 0100 0050 0200 0011 0000 0064 6f63 5072  ...P.......docPr
 00001340: 6f70 732f 636f 7265 2e78 6d6c 9d92 cd6a  ops/core.xml...j
-00001350: c330 1084 ef7d 0aa3 bb2d cb86 1284 ed40  .0...}...-.....@
-00001360: 5b72 6aa0 d094 96de 84b4 4944 ad1f 24b5  [rj.......ID..$.
-00001370: 8edf be8a ed38 09e4 94e3 6a66 bf9d 5d54  .....8....jf..]T
-00001380: 2d0f aa4d fec0 7969 748d 4896 a304 3437  -..M..yit.H...47
-00001390: 42ea 5d8d 3e36 ab74 8112 1f98 16ac 351a  B.].>6.t......5.
-000013a0: 6ad4 8347 cbe6 a1e2 9672 e3e0 cd19 0b2e  j..G.....r......
-000013b0: 48f0 4904 694f b9ad d13e 044b 31f6 7c0f  H.I.iO...>.K1.|.
-000013c0: 8af9 2c3a 7414 b7c6 2916 62e9 76d8 32fe  ..,:t...).b.v.2.
-000013d0: c376 808b 3c7f c40a 0213 2c30 7c04 a676  .v..<.....,0|..v
-000013e0: 26a2 0929 f88c b4bf ae1d 0082 6368 4181  &..)........chA.
-000013f0: 0e1e 938c e0b3 3780 53fe 66c3 a05c 3895  ......7.S.f..\8.
-00001400: 0cbd 859b d693 38bb 0f5e cec6 aeeb b2ae  ......8..^......
-00001410: 1cac 313f c15f ebd7 f761 d554 eae3 a938  ..1?._...a.T...8
-00001420: a0a6 129c 7207 2c18 d754 f8b2 8887 6b99  ....r.,..T....k.
-00001430: 0feb 78e2 ad04 f1d4 47fd c6db b4c8 d807  ..x.....G.......
-00001440: 2289 01e8 18f7 a47c 96cf 2f9b 156a 8abc  "......|../..j..
-00001450: 2852 92a7 64b1 2139 2d0a 4aca efe3 c8ab  (R..d.!9-.J.....
-00001460: fe33 504d 43ee 269e 0063 eeeb 4fd0 fc03  .3PMC.&..c..O...
+00001350: c330 1084 ef7d 0aa3 bb2d d9a6 2508 db81  .0...}...-..%...
+00001360: b6e4 d440 a12e 2dbd 0969 9388 5a3f 486a  ...@..-..i..Z?Hj
+00001370: 1dbf 7d15 2771 12f0 a9c7 d5cc 7e3b bba8  ..}.'q......~;..
+00001380: 5aee 5597 fc82 f3d2 e81a e519 4109 686e  Z.U.........A.hn
+00001390: 84d4 db1a bdb7 ab74 8112 1f98 16ac 331a  .......t......3.
+000013a0: 6a34 8047 cbe6 aee2 9672 e3e0 d519 0b2e  j4.G.....r......
+000013b0: 48f0 4904 694f b9ad d12e 044b 31f6 7c07  H.I.iO.....K1.|.
+000013c0: 8af9 2c3a 7414 37c6 2916 62e9 b6d8 32fe  ..,:t.7.).b...2.
+000013d0: cdb6 800b 421e b082 c004 0b0c 1f80 a99d  ....B...........
+000013e0: 88e8 8414 7c42 da1f d78d 00c1 3174 a040  ....|B......1t.@
+000013f0: 078f f32c c717 6f00 a7fc 6cc3 a85c 3995  ...,..o...l..\9.
+00001400: 0c83 8559 eb59 9cdc 7b2f 2763 dff7 595f  ...Y.Y..{/'c..Y_
+00001410: 8ed6 983f c79f eb97 b771 d554 eac3 a938  ...?.....q.T...8
+00001420: a0a6 129c 7207 2c18 d754 f8ba 8887 eb98  ....r.,..T......
+00001430: 0feb 78e2 8d04 f138 447d e6ed b4c8 b10f  ..x....8D}......
+00001440: 4412 03d0 63dc b3f2 513e 3db7 2bd4 14a4  D...c...Q>=.+...
+00001450: 2853 729f 92a2 250b 5a96 b4c8 bf0e 236f  (Sr...%.Z.....#o
+00001460: fa2f 4075 1af2 6fe2 1970 cc7d fb09 9a3f  ./@u..o..p.}...?
 00001470: 504b 0304 1400 0000 0800 0000 3f00 6494  PK..........?.d.
 00001480: b217 8301 0000 4203 0000 1000 0000 646f  ......B.......do
 00001490: 6350 726f 7073 2f61 7070 2e78 6d6c 9d53  cProps/app.xml.S
 000014a0: 4d6f db30 0cbd ef57 18ba 3772 d361 1802  Mo.0...W..7r.a..
 000014b0: 5945 9176 e861 c302 24ed ce9c 4cc7 4265  YE.v.a..$...L.Be
 000014c0: 4910 5923 d9af 9fec 20ae b3f6 349d 1ec9  I.Y#.... ...4...
 000014d0: 8787 c70f a9db 43e7 8a1e 13d9 e02b 71bd  ......C......+q.
@@ -390,15 +390,15 @@
 00001850: 0d00 0000 0000 0000 0000 0000 8081 160b  ................
 00001860: 0000 786c 2f73 7479 6c65 732e 786d 6c50  ..xl/styles.xmlP
 00001870: 4b01 0214 0314 0000 0008 0000 003f 0018  K............?..
 00001880: fa46 54b0 0500 0052 1b00 0013 0000 0000  .FT....R........
 00001890: 0000 0000 0000 0080 813c 0d00 0078 6c2f  .........<...xl/
 000018a0: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
 000018b0: 504b 0102 1403 1400 0000 0800 0000 3f00  PK............?.
-000018c0: bd4c af80 2401 0000 5002 0000 1100 0000  .L..$...P.......
+000018c0: beb9 67ee 2401 0000 5002 0000 1100 0000  ..g.$...P.......
 000018d0: 0000 0000 0000 0000 8081 1d13 0000 646f  ..............do
 000018e0: 6350 726f 7073 2f63 6f72 652e 786d 6c50  cProps/core.xmlP
 000018f0: 4b01 0214 0314 0000 0008 0000 003f 0064  K............?.d
 00001900: 94b2 1783 0100 0042 0300 0010 0000 0000  .......B........
 00001910: 0000 0000 0000 0080 8170 1400 0064 6f63  .........p...doc
 00001920: 5072 6f70 732f 6170 702e 786d 6c50 4b05  Props/app.xmlPK.
 00001930: 0600 0000 000c 000c 000c 0300 0021 1600  .............!..
```

### Comparing `gridsource-1.3.0/tests/data/ftools_example.yaml` & `gridsource-1.3.1/tests/data/ftools_example.yaml`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/ftools_example_units.yaml` & `gridsource-1.3.1/tests/data/ftools_example_units.yaml`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_00.schema.json` & `gridsource-1.3.1/tests/data/test_00.schema.json`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_00.xlsx` & `gridsource-1.3.1/tests/data/test_00.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_01.schema2.yaml` & `gridsource-1.3.1/tests/data/test_01.schema2.yaml`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_01.xlsx` & `gridsource-1.3.1/tests/data/test_01.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_02.schema.yaml` & `gridsource-1.3.1/tests/data/test_02.schema.yaml`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_02.xlsx` & `gridsource-1.3.1/tests/data/test_02.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_03_units.xlsx` & `gridsource-1.3.1/tests/data/test_03_units.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_04_data.yaml` & `gridsource-1.3.1/tests/data/test_04_data.yaml`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_04_units.xlsx` & `gridsource-1.3.1/tests/data/test_04_units.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_04_units_failing.xlsx` & `gridsource-1.3.1/tests/data/test_04_units_failing.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_05_units_failing.xlsx` & `gridsource-1.3.1/tests/data/test_05_units_failing.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_06_data.yaml` & `gridsource-1.3.1/tests/data/test_06_data.yaml`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_06_multi-columns_uniqueness.ini` & `gridsource-1.3.1/tests/data/test_06_multi-columns_uniqueness.ini`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_06_must_exist_in.xlsx` & `gridsource-1.3.1/tests/data/test_06_must_exist_in.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_06_must_exist_in.yaml` & `gridsource-1.3.1/tests/data/test_06_must_exist_in.yaml`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_10_mandatory_if.xlsx` & `gridsource-1.3.1/tests/data/test_10_mandatory_if.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_10_mandatory_if.yaml` & `gridsource-1.3.1/tests/data/test_10_mandatory_if.yaml`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_11.schema.json` & `gridsource-1.3.1/tests/data/test_11.schema.json`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/data/test_11.xlsx` & `gridsource-1.3.1/tests/data/test_11.xlsx`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/test_autodoc.py` & `gridsource-1.3.1/tests/test_autodoc.py`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/test_io.py` & `gridsource-1.3.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `gridsource-1.3.0/tests/test_validation.py` & `gridsource-1.3.1/tests/test_validation.py`

 * *Files identical despite different names*

