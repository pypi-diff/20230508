# Comparing `tmp/audformat-1.0.0.tar.gz` & `tmp/audformat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audformat-1.0.0.tar", last modified: Thu Apr 27 13:00:24 2023, max compression
+gzip compressed data, was "audformat-1.0.1.tar", last modified: Mon May  8 09:08:52 2023, max compression
```

## Comparing `audformat-1.0.0.tar` & `audformat-1.0.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.785670 audformat-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.773670 audformat-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-27 13:00:09.000000 audformat-1.0.0/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 13:00:09.000000 audformat-1.0.0/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-27 13:00:09.000000 audformat-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-27 13:00:09.000000 audformat-1.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-27 13:00:09.000000 audformat-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 13:00:09.000000 audformat-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-04-27 13:00:09.000000 audformat-1.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-27 13:00:09.000000 audformat-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 13:00:09.000000 audformat-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21353 2023-04-27 13:00:24.785670 audformat-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-27 13:00:09.000000 audformat-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/audformat/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/audformat/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    41048 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/define.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/rater.py
--rw-r--r--   0 runner    (1001) docker     (123)    17825 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/split.py
--rw-r--r--   0 runner    (1001) docker     (123)    50292 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    59756 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/audformat/define/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/define/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/audformat/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/audformat/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/audformat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/audformat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21353 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-27 13:00:09.000000 audformat-1.0.0/benchmarks/benchmark_union.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/accessing-data.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.define.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.rst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.define.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.rst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/combine-tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/create-database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-format.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-header.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-misc-tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/emodb-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/map-scheme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/pics/audformat-database.dot
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/pics/audformat-misc-table.dot
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/pics/audformat-table.dot
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/update-database.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 13:00:09.000000 audformat-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-27 13:00:24.785670 audformat-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 13:00:09.000000 audformat-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.785670 audformat-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    46124 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_misc_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    55836 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    85100 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.048183 audformat-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.020183 audformat-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.028183 audformat-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 09:08:30.000000 audformat-1.0.1/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-08 09:08:30.000000 audformat-1.0.1/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-08 09:08:30.000000 audformat-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-08 09:08:30.000000 audformat-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 09:08:30.000000 audformat-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 09:08:30.000000 audformat-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-05-08 09:08:30.000000 audformat-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-08 09:08:30.000000 audformat-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 09:08:30.000000 audformat-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-05-08 09:08:52.048183 audformat-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-08 09:08:30.000000 audformat-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.028183 audformat-1.0.1/audformat/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.032183 audformat-1.0.1/audformat/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41048 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/rater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17825 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50292 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60109 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.032183 audformat-1.0.1/audformat/define/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/define/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.036183 audformat-1.0.1/audformat/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.036183 audformat-1.0.1/audformat/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.036183 audformat-1.0.1/audformat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 09:08:30.000000 audformat-1.0.1/audformat/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.028183 audformat-1.0.1/audformat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-05-08 09:08:51.000000 audformat-1.0.1/audformat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-08 09:08:51.000000 audformat-1.0.1/audformat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:08:51.000000 audformat-1.0.1/audformat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 09:08:51.000000 audformat-1.0.1/audformat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 09:08:51.000000 audformat-1.0.1/audformat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.036183 audformat-1.0.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-08 09:08:30.000000 audformat-1.0.1/benchmarks/benchmark_union.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.040183 audformat-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.024183 audformat-1.0.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.040183 audformat-1.0.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/accessing-data.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.040183 audformat-1.0.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api/audformat.define.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api/audformat.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api/audformat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api/audformat.testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api/audformat.utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.044183 audformat-1.0.1/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api-src/audformat.define.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api-src/audformat.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api-src/audformat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api-src/audformat.testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/api-src/audformat.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/combine-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/create-database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/data-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/data-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/data-format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/data-header.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/data-introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/data-misc-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/data-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/emodb-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/map-scheme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.044183 audformat-1.0.1/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/pics/audformat-database.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/pics/audformat-misc-table.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/pics/audformat-table.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-08 09:08:30.000000 audformat-1.0.1/docs/update-database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 09:08:30.000000 audformat-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-08 09:08:52.048183 audformat-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 09:08:30.000000 audformat-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:08:52.048183 audformat-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46124 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_misc_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55836 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86486 2023-05-08 09:08:30.000000 audformat-1.0.1/tests/test_utils.py
```

### Comparing `audformat-1.0.0/.github/workflows/doc.yml` & `audformat-1.0.1/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/.github/workflows/publish.yml` & `audformat-1.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/.github/workflows/test.yml` & `audformat-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/CHANGELOG.rst` & `audformat-1.0.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.0.1 (2023-05-08)
+--------------------------
+
+* Fixed: ensure ``audformat.utils.to_segmented_index()``
+  and ``audformat.Table.get()``
+  with ``as_segmented=True``
+  uses same precision for ``end`` values
+  as ``audformat.segmented_index()``
+
+
 Version 1.0.0 (2023-04-27)
 --------------------------
 
 * Added: ``audformat.Scheme.labels_as_list`` property
   to list all scheme labels
 * Added: example to the documentation of
   ``audformat.utils.to_filewise_index()``
```

### Comparing `audformat-1.0.0/CONTRIBUTING.rst` & `audformat-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/LICENSE` & `audformat-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/PKG-INFO` & `audformat-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audformat
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python implementation of audformat
 Home-page: https://github.com/audeering/audformat/
 Author: Johannes Wagner, Hagen Wierstorf, Baha Eddine Abrougui
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com, beddine@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audformat/
 Description: =========
@@ -61,14 +61,24 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.0.1 (2023-05-08)
+        --------------------------
+        
+        * Fixed: ensure ``audformat.utils.to_segmented_index()``
+          and ``audformat.Table.get()``
+          with ``as_segmented=True``
+          uses same precision for ``end`` values
+          as ``audformat.segmented_index()``
+        
+        
         Version 1.0.0 (2023-04-27)
         --------------------------
         
         * Added: ``audformat.Scheme.labels_as_list`` property
           to list all scheme labels
         * Added: example to the documentation of
           ``audformat.utils.to_filewise_index()``
```

### Comparing `audformat-1.0.0/README.rst` & `audformat-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/__init__.py` & `audformat-1.0.1/audformat/__init__.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/attachment.py` & `audformat-1.0.1/audformat/core/attachment.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/column.py` & `audformat-1.0.1/audformat/core/column.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/common.py` & `audformat-1.0.1/audformat/core/common.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/conftest.py` & `audformat-1.0.1/audformat/core/conftest.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/database.py` & `audformat-1.0.1/audformat/core/database.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/define.py` & `audformat-1.0.1/audformat/core/define.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/errors.py` & `audformat-1.0.1/audformat/core/errors.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/index.py` & `audformat-1.0.1/audformat/core/index.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/media.py` & `audformat-1.0.1/audformat/core/media.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/rater.py` & `audformat-1.0.1/audformat/core/rater.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/scheme.py` & `audformat-1.0.1/audformat/core/scheme.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/split.py` & `audformat-1.0.1/audformat/core/split.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/table.py` & `audformat-1.0.1/audformat/core/table.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/testing.py` & `audformat-1.0.1/audformat/core/testing.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/audformat/core/utils.py` & `audformat-1.0.1/audformat/core/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1585,14 +1585,17 @@
     if not allow_nat:
 
         ends = index.get_level_values(define.IndexField.END)
         has_nat = pd.isna(ends)
 
         if any(has_nat):
 
+            # Gather duration values
+            # for all NaT end entries
+
             idx_nat = np.where(has_nat)[0]
             files = index.get_level_values(define.IndexField.FILE)
             starts = index.get_level_values(define.IndexField.START)
 
             def job(file: str) -> pd.Timedelta:
 
                 if root is not None and not os.path.isabs(file):
@@ -1618,16 +1621,24 @@
             durs = audeer.run_tasks(
                 job,
                 params,
                 num_workers=num_workers,
                 progress_bar=verbose,
                 task_description='Read duration',
             )
-            ends.values[idx_nat] = durs
 
+            # Replace all NaT entries in end
+            # by the collected duration values.
+            # We have to convert ends to a series first
+            # in order to preserve precision of duration values
+
+            ends = ends.to_series()
+            ends[idx_nat] = durs
+
+            # Create a new index
             index = segmented_index(files, starts, ends)
 
     if isinstance(obj, pd.Index):
         return index
 
     obj = obj.reset_index(drop=True)
     obj.index = index
```

### Comparing `audformat-1.0.0/audformat.egg-info/PKG-INFO` & `audformat-1.0.1/audformat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audformat
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python implementation of audformat
 Home-page: https://github.com/audeering/audformat/
 Author: Johannes Wagner, Hagen Wierstorf, Baha Eddine Abrougui
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com, beddine@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audformat/
 Description: =========
@@ -61,14 +61,24 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.0.1 (2023-05-08)
+        --------------------------
+        
+        * Fixed: ensure ``audformat.utils.to_segmented_index()``
+          and ``audformat.Table.get()``
+          with ``as_segmented=True``
+          uses same precision for ``end`` values
+          as ``audformat.segmented_index()``
+        
+        
         Version 1.0.0 (2023-04-27)
         --------------------------
         
         * Added: ``audformat.Scheme.labels_as_list`` property
           to list all scheme labels
         * Added: example to the documentation of
           ``audformat.utils.to_filewise_index()``
```

### Comparing `audformat-1.0.0/audformat.egg-info/SOURCES.txt` & `audformat-1.0.1/audformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/benchmarks/benchmark_union.py` & `audformat-1.0.1/benchmarks/benchmark_union.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/_templates/autosummary/class.rst` & `audformat-1.0.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/accessing-data.rst` & `audformat-1.0.1/docs/accessing-data.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/api/audformat.define.rst` & `audformat-1.0.1/docs/api/audformat.define.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/api/audformat.testing.rst` & `audformat-1.0.1/docs/api/audformat.testing.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/api-src/audformat.define.rst` & `audformat-1.0.1/docs/api-src/audformat.define.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/api-src/audformat.testing.rst` & `audformat-1.0.1/docs/api-src/audformat.testing.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/combine-tables.rst` & `audformat-1.0.1/docs/combine-tables.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/conf.py` & `audformat-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/create-database.rst` & `audformat-1.0.1/docs/create-database.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/data-conventions.rst` & `audformat-1.0.1/docs/data-conventions.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/data-example.rst` & `audformat-1.0.1/docs/data-example.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/data-format.rst` & `audformat-1.0.1/docs/data-format.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/data-header.rst` & `audformat-1.0.1/docs/data-header.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/data-introduction.rst` & `audformat-1.0.1/docs/data-introduction.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/data-misc-tables.rst` & `audformat-1.0.1/docs/data-misc-tables.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/data-tables.rst` & `audformat-1.0.1/docs/data-tables.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/emodb-example.rst` & `audformat-1.0.1/docs/emodb-example.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/index.rst` & `audformat-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/map-scheme.rst` & `audformat-1.0.1/docs/map-scheme.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/pics/audformat-database.dot` & `audformat-1.0.1/docs/pics/audformat-database.dot`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/docs/update-database.rst` & `audformat-1.0.1/docs/update-database.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/setup.cfg` & `audformat-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/conftest.py` & `audformat-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_attachment.py` & `audformat-1.0.1/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_column.py` & `audformat-1.0.1/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_common.py` & `audformat-1.0.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_database.py` & `audformat-1.0.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_eq.py` & `audformat-1.0.1/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_errors.py` & `audformat-1.0.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_index.py` & `audformat-1.0.1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_misc_table.py` & `audformat-1.0.1/tests/test_misc_table.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_scheme.py` & `audformat-1.0.1/tests/test_scheme.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_table.py` & `audformat-1.0.1/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `audformat-1.0.0/tests/test_utils.py` & `audformat-1.0.1/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2505,14 +2505,56 @@
             pytest.DB_ROOT,
             audformat.segmented_index(
                 pytest.DB.files[:2],
                 [0.1, 0.5],
                 [pytest.FILE_DUR, pytest.FILE_DUR * 2],
             ),
         ),
+        # file duration with high precision
+        # covering https://github.com/audeering/audformat/issues/379
+        (
+            audformat.segmented_index(
+                [pytest.DB.files[0]],
+                [0],
+                [pd.NaT],
+            ),
+            False,
+            {
+                os.path.join(pytest.DB_ROOT, pytest.DB.files[0]):
+                pd.to_timedelta(2.5225, unit='s'),
+            },
+            pytest.DB_ROOT,
+            audformat.segmented_index(
+                [pytest.DB.files[0]],
+                [0],
+                [2.5225],
+            ),
+        ),
+        (
+            audformat.segmented_index(
+                pytest.DB.files[:3],
+                [1, 0, 0],
+                [pd.NaT, 2.37485, pd.NaT],
+            ),
+            False,
+            {
+                os.path.join(pytest.DB_ROOT, pytest.DB.files[0]):
+                pd.to_timedelta(2.5225, unit='s'),
+                os.path.join(pytest.DB_ROOT, pytest.DB.files[1]):
+                pd.to_timedelta(2.37485, unit='s'),
+                os.path.join(pytest.DB_ROOT, pytest.DB.files[2]):
+                pd.to_timedelta(3.458697083, unit='s'),
+            },
+            pytest.DB_ROOT,
+            audformat.segmented_index(
+                pytest.DB.files[:3],
+                [1, 0, 0],
+                [2.5225, 2.37485, 3.458697083],
+            ),
+        ),
         # file not found
         pytest.param(
             audformat.filewise_index(pytest.DB.files[:2]),
             False,
             None,
             None,
             None,
```

