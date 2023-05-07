# Comparing `tmp/aind-data-schema-0.9.5.tar.gz` & `tmp/aind-data-schema-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-data-schema-0.9.5.tar", last modified: Thu Jan 26 04:55:51 2023, max compression
+gzip compressed data, was "aind-data-schema-0.9.6.tar", last modified: Thu Jan 26 17:48:28 2023, max compression
```

## Comparing `aind-data-schema-0.9.5.tar` & `aind-data-schema-0.9.6.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.199185 aind-data-schema-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.183185 aind-data-schema-0.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.187185 aind-data-schema-0.9.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.187185 aind-data-schema-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/.github/workflows/tag.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-01-26 04:55:51.199185 aind-data-schema-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.187185 aind-data-schema-0.9.5/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.187185 aind-data-schema-0.9.5/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.191185 aind-data-schema-0.9.5/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/aind_data_schema.ephys.rst
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/aind_data_schema.imaging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/aind_data_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/doc_template/source/opendata.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.195185 aind-data-schema-0.9.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/aibs_smartspim_instrument.json
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/aibs_smartspim_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/aind_smartspim_acquisition.json
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/aind_smartspim_instrument.json
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/aind_smartspim_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/data_description.json
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/data_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/ephys_rig.json
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/ephys_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/exaspim_acquisition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/exaspim_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/exaspim_instrument.json
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/exaspim_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/procedures.json
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/procedures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/processing.json
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/subject.json
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/examples/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 04:55:51.199185 aind-data-schema-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.183185 aind-data-schema-0.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.195185 aind-data-schema-0.9.5/src/aind_data_schema/
--rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9343 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/data_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.195185 aind-data-schema-0.9.5/src/aind_data_schema/ephys/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/ephys/ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/ephys/ephys_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.199185 aind-data-schema-0.9.5/src/aind_data_schema/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/imaging/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/imaging/instrument.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.199185 aind-data-schema-0.9.5/src/aind_data_schema/ophys/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/ophys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/ophys/ophys_rig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/ophys/ophys_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/procedures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/subject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.199185 aind-data-schema-0.9.5/src/aind_data_schema/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/src/aind_data_schema/utils/json_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.195185 aind-data-schema-0.9.5/src/aind_data_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-01-26 04:55:51.000000 aind-data-schema-0.9.5/src/aind_data_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-01-26 04:55:51.000000 aind-data-schema-0.9.5/src/aind_data_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 04:55:51.000000 aind-data-schema-0.9.5/src/aind_data_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-26 04:55:51.000000 aind-data-schema-0.9.5/src/aind_data_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-26 04:55:51.000000 aind-data-schema-0.9.5/src/aind_data_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 04:55:51.199185 aind-data-schema-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_data_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_json_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_procedures.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-26 04:55:31.000000 aind-data-schema-0.9.5/tests/test_subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.849227 aind-data-schema-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.837227 aind-data-schema-0.9.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.837227 aind-data-schema-0.9.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.841227 aind-data-schema-0.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/.github/workflows/tag.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-01-26 17:48:28.849227 aind-data-schema-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.841227 aind-data-schema-0.9.6/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.841227 aind-data-schema-0.9.6/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.841227 aind-data-schema-0.9.6/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/aind_data_schema.ephys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/aind_data_schema.imaging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/aind_data_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/doc_template/source/opendata.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.845227 aind-data-schema-0.9.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/aibs_smartspim_instrument.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/aibs_smartspim_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/aind_smartspim_acquisition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/aind_smartspim_instrument.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/aind_smartspim_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/data_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/ephys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/ephys_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/exaspim_acquisition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/exaspim_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/exaspim_instrument.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/exaspim_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/subject.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/examples/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 17:48:28.849227 aind-data-schema-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.837227 aind-data-schema-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.845227 aind-data-schema-0.9.6/src/aind_data_schema/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-01-26 17:48:12.000000 aind-data-schema-0.9.6/src/aind_data_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9343 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/data_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.845227 aind-data-schema-0.9.6/src/aind_data_schema/ephys/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/ephys/ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/ephys/ephys_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.849227 aind-data-schema-0.9.6/src/aind_data_schema/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/imaging/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/imaging/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/imaging/tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.849227 aind-data-schema-0.9.6/src/aind_data_schema/ophys/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/ophys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/ophys/ophys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/ophys/ophys_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.849227 aind-data-schema-0.9.6/src/aind_data_schema/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/src/aind_data_schema/utils/json_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.845227 aind-data-schema-0.9.6/src/aind_data_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-01-26 17:48:28.000000 aind-data-schema-0.9.6/src/aind_data_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-01-26 17:48:28.000000 aind-data-schema-0.9.6/src/aind_data_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 17:48:28.000000 aind-data-schema-0.9.6/src/aind_data_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-26 17:48:28.000000 aind-data-schema-0.9.6/src/aind_data_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-26 17:48:28.000000 aind-data-schema-0.9.6/src/aind_data_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:48:28.849227 aind-data-schema-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_data_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_ephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_json_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-26 17:48:11.000000 aind-data-schema-0.9.6/tests/test_subject.py
```

### Comparing `aind-data-schema-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-data-schema-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-data-schema-0.9.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/.github/ISSUE_TEMPLATE/user-story.md` & `aind-data-schema-0.9.6/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/.github/workflows/ci.yml` & `aind-data-schema-0.9.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/.github/workflows/tag.yml` & `aind-data-schema-0.9.6/.github/workflows/tag.yml`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/.gitignore` & `aind-data-schema-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/LICENSE` & `aind-data-schema-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/PKG-INFO` & `aind-data-schema-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-schema
-Version: 0.9.5
+Version: 0.9.6
 Summary: A library that defines AIND data schema and validates JSON files.
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `aind-data-schema-0.9.5/README.md` & `aind-data-schema-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/Makefile` & `aind-data-schema-0.9.6/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/make.bat` & `aind-data-schema-0.9.6/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/source/_static/dark-logo.svg` & `aind-data-schema-0.9.6/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/source/_static/favicon.ico` & `aind-data-schema-0.9.6/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/source/_static/light-logo.svg` & `aind-data-schema-0.9.6/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/source/aind_data_schema.ephys.rst` & `aind-data-schema-0.9.6/doc_template/source/aind_data_schema.ephys.rst`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/source/aind_data_schema.imaging.rst` & `aind-data-schema-0.9.6/doc_template/source/aind_data_schema.imaging.rst`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/source/aind_data_schema.rst` & `aind-data-schema-0.9.6/doc_template/source/aind_data_schema.rst`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/source/conf.py` & `aind-data-schema-0.9.6/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/doc_template/source/opendata.rst` & `aind-data-schema-0.9.6/doc_template/source/opendata.rst`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/aibs_smartspim_instrument.json` & `aind-data-schema-0.9.6/examples/aibs_smartspim_instrument.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/aibs_smartspim_instrument.py` & `aind-data-schema-0.9.6/examples/aibs_smartspim_instrument.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/aind_smartspim_acquisition.json` & `aind-data-schema-0.9.6/examples/aind_smartspim_acquisition.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/aind_smartspim_instrument.json` & `aind-data-schema-0.9.6/examples/aind_smartspim_instrument.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/aind_smartspim_instrument.py` & `aind-data-schema-0.9.6/examples/aind_smartspim_instrument.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/data_description.json` & `aind-data-schema-0.9.6/examples/data_description.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/ephys_rig.json` & `aind-data-schema-0.9.6/examples/ephys_rig.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/ephys_rig.py` & `aind-data-schema-0.9.6/examples/ephys_rig.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/ephys_session.json` & `aind-data-schema-0.9.6/examples/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/ephys_session.py` & `aind-data-schema-0.9.6/examples/ephys_session.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/exaspim_acquisition.json` & `aind-data-schema-0.9.6/examples/exaspim_acquisition.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -22,23 +22,23 @@
                     "translation": [
                         0.0,
                         0.0,
                         0.0
                     ]
                 }
             ],
+            "file_name": "tile_X_0000_Y_0000_Z_0000_CH_488.ims",
             "channel": {
                 "channel_name": "488",
                 "laser_wavelength": 488,
                 "laser_wavelength_unit": "nanometer",
                 "laser_power": 200.0,
                 "laser_power_unit": "milliwatt",
                 "filter_wheel_index": 0
             },
-            "file_name": "tile_X_0000_Y_0000_Z_0000_CH_488.ims",
             "notes": "these are my notes",
             "imaging_angle": 0,
             "imaging_angle_unit": "degree"
         },
         {
             "coordinate_transformations": [
                 {
@@ -54,23 +54,23 @@
                     "translation": [
                         0.0,
                         0.0,
                         0.0
                     ]
                 }
             ],
+            "file_name": "tile_X_0000_Y_0000_Z_0000_CH_561.ims",
             "channel": {
                 "channel_name": "561",
                 "laser_wavelength": 561,
                 "laser_wavelength_unit": "nanometer",
                 "laser_power": 200.0,
                 "laser_power_unit": "milliwatt",
                 "filter_wheel_index": 0
             },
-            "file_name": "tile_X_0000_Y_0000_Z_0000_CH_561.ims",
             "notes": "these are my notes",
             "imaging_angle": 0,
             "imaging_angle_unit": "degree"
         }
     ],
     "axes": [
         {
```

### Comparing `aind-data-schema-0.9.5/examples/exaspim_acquisition.py` & `aind-data-schema-0.9.6/examples/exaspim_acquisition.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ example ExaSPIM acquisition """
 
 import datetime
 
-from aind_data_schema.imaging import acquisition
+from aind_data_schema.imaging import acquisition, tile
 
 t = datetime.datetime(2022, 11, 22, 8, 43, 00)
 
 acq = acquisition.Acquisition(
     experimenter_full_name="###",
     subject_id="###",
     instrument_id="###",
@@ -29,35 +29,35 @@
         acquisition.Axis(
             name="Z",
             dimension=0,
             direction="Inferior_to_superior",
         ),
     ],
     tiles=[
-        acquisition.Tile(
+        tile.AcquisitionTile(
             file_name="tile_X_0000_Y_0000_Z_0000_CH_488.ims",
             coordinate_transformations=[
-                acquisition.Scale3dTransform(scale=[0.748, 0.748, 1.0]),
-                acquisition.Translation3dTransform(translation=[0, 0, 0]),
+                tile.Scale3dTransform(scale=[0.748, 0.748, 1.0]),
+                tile.Translation3dTransform(translation=[0, 0, 0]),
             ],
-            channel=acquisition.Channel(
+            channel=tile.Channel(
                 channel_name="488",
                 laser_wavelength=488,
                 laser_power=200,
                 filter_wheel_index=0,
             ),
             notes="these are my notes",
         ),
-        acquisition.Tile(
+        tile.AcquisitionTile(
             file_name="tile_X_0000_Y_0000_Z_0000_CH_561.ims",
             coordinate_transformations=[
-                acquisition.Scale3dTransform(scale=[0.748, 0.748, 1.0]),
-                acquisition.Translation3dTransform(translation=[0, 0, 0]),
+                tile.Scale3dTransform(scale=[0.748, 0.748, 1.0]),
+                tile.Translation3dTransform(translation=[0, 0, 0]),
             ],
-            channel=acquisition.Channel(
+            channel=tile.Channel(
                 channel_name="561",
                 laser_wavelength=561,
                 laser_power=200,
                 filter_wheel_index=0,
             ),
             notes="these are my notes",
         ),
```

### Comparing `aind-data-schema-0.9.5/examples/exaspim_instrument.json` & `aind-data-schema-0.9.6/examples/exaspim_instrument.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/exaspim_instrument.py` & `aind-data-schema-0.9.6/examples/exaspim_instrument.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/procedures.json` & `aind-data-schema-0.9.6/examples/procedures.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/procedures.py` & `aind-data-schema-0.9.6/examples/procedures.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 """ ephys procedure mouse 625100 """
 import datetime
+
 from aind_data_schema import Procedures
-from aind_data_schema.procedures import (
-    Craniotomy,
-    NanojectInjection,
-    Anaesthetic,
-    InjectionMaterial,
-)
+from aind_data_schema.procedures import Anaesthetic, Craniotomy, InjectionMaterial, NanojectInjection
 
 t = datetime.datetime(2022, 7, 12, 7, 00, 00)
 
 p = Procedures(
     subject_id="625100",
     craniotomies=[
         Craniotomy(
```

### Comparing `aind-data-schema-0.9.5/examples/processing.json` & `aind-data-schema-0.9.6/examples/processing.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/processing.py` & `aind-data-schema-0.9.6/examples/processing.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/examples/subject.json` & `aind-data-schema-0.9.6/examples/subject.json`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/pyproject.toml` & `aind-data-schema-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/__init__.py` & `aind-data-schema-0.9.6/src/aind_data_schema/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ imports for AindModel subclasses
 """
 
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 
 from .data_description import DataDescription, DerivedDataDescription, Funding, RawDataDescription
 from .ephys.ephys_rig import EphysRig
 from .ephys.ephys_session import EphysSession
 from .imaging.acquisition import Acquisition, Axis
 from .imaging.instrument import Instrument
```

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/base.py` & `aind-data-schema-0.9.6/src/aind_data_schema/base.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/data_description.py` & `aind-data-schema-0.9.6/src/aind_data_schema/data_description.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/device.py` & `aind-data-schema-0.9.6/src/aind_data_schema/device.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/ephys/ephys_rig.py` & `aind-data-schema-0.9.6/src/aind_data_schema/ephys/ephys_rig.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/ephys/ephys_session.py` & `aind-data-schema-0.9.6/src/aind_data_schema/ephys/ephys_session.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/imaging/instrument.py` & `aind-data-schema-0.9.6/src/aind_data_schema/imaging/instrument.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/ophys/ophys_rig.py` & `aind-data-schema-0.9.6/src/aind_data_schema/ophys/ophys_rig.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/ophys/ophys_session.py` & `aind-data-schema-0.9.6/src/aind_data_schema/ophys/ophys_session.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/procedures.py` & `aind-data-schema-0.9.6/src/aind_data_schema/procedures.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from enum import Enum
 from typing import List, Optional, Union
 
 from pydantic import Field
 
 from .base import AindCoreModel, AindModel
 
+
 class Side(Enum):
     """Side of animal"""
 
     LEFT = "Left"
     RIGHT = "Right"
 
 
@@ -118,15 +119,15 @@
     )
     prep_type: Optional[VirusPrepType] = Field(None, title="Viral prep type")
 
 
 class Injection(Procedure):
     """Description of an injection procedure"""
 
-    injection_materials: List[InjectionMaterial] = Field(None, title="Injection material", unique_items=True)    
+    injection_materials: List[InjectionMaterial] = Field(None, title="Injection material", unique_items=True)
     recovery_time: float = Field(..., title="Recovery time (min)", units="min")
     injection_duration: Optional[time] = Field(None, title="Injection duration")
     workstation_id: Optional[str] = Field(None, title="Workstation ID")
     instrument_id: Optional[str] = Field(None, title="Instrument ID")
 
 
 class RetroOrbitalInjection(Injection):
```

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/processing.py` & `aind-data-schema-0.9.6/src/aind_data_schema/processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from pydantic import Field
 
-from .base import AindCoreModel, AindModel
+from aind_data_schema.base import AindCoreModel, AindModel
+from aind_data_schema.imaging.tile import Tile
 
 
 class ProcessName(Enum):
     """Data processing type labels"""
 
     EPHYS_PREPROCESSING = "Ephys preprocessing"
     EPHYS_POSTPROCESSING = "Ephys postprocessing"
@@ -50,7 +51,15 @@
         description="Schema version",
         title="Schema version",
         const=True,
     )
     pipeline_version: Optional[str] = Field(None, description="Version of the pipeline", title="Pipeline version")
     pipeline_url: Optional[str] = Field(None, description="URL to the pipeline code", title="Pipeline URL")
     data_processes: List[DataProcess] = Field(..., title="Data processing", unique_items=True)
+
+
+class Stitching(DataProcess):
+    """Description of an imaging acquisition session"""
+
+    schema_version: str = Field("0.1.0", description="schema version for stitching", title="Version", const=True)
+
+    tiles: List[Tile] = Field(..., title="Data tiles")
```

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/subject.py` & `aind-data-schema-0.9.6/src/aind_data_schema/subject.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema/utils/json_writer.py` & `aind-data-schema-0.9.6/src/aind_data_schema/utils/json_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,15 @@
             "--output",
             required=False,
             default=self.DEFAULT_FILE_PATH,
             help=help_message,
         )
 
         parser.add_argument(
-            "--attach-version",
-            action="store_true",
-            help="Add extra directory with schema version number"
+            "--attach-version", action="store_true", help="Add extra directory with schema version number"
         )
         parser.set_defaults(attach_version=False)
 
         optional_args = parser.parse_args(args)
 
         return optional_args
 
@@ -70,15 +68,15 @@
             schema_filename = filename.replace(".json", "_schema.json")
             if self.configs.attach_version:
                 schema_version = schema.construct().schema_version
                 model_directory_name = schema_filename.replace("_schema.json", "")
                 sub_directory = Path(output_path) / model_directory_name / schema_version
                 if not os.path.exists(sub_directory):
                     os.makedirs(sub_directory)
-                output_file = sub_directory /schema_filename
+                output_file = sub_directory / schema_filename
             else:
                 output_file = Path(output_path) / schema_filename
 
             with open(output_file, "w") as f:
                 f.write(schema.schema_json(indent=3))
```

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema.egg-info/PKG-INFO` & `aind-data-schema-0.9.6/src/aind_data_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-schema
-Version: 0.9.5
+Version: 0.9.6
 Summary: A library that defines AIND data schema and validates JSON files.
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `aind-data-schema-0.9.5/src/aind_data_schema.egg-info/SOURCES.txt` & `aind-data-schema-0.9.6/src/aind_data_schema.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 src/aind_data_schema.egg-info/top_level.txt
 src/aind_data_schema/ephys/__init__.py
 src/aind_data_schema/ephys/ephys_rig.py
 src/aind_data_schema/ephys/ephys_session.py
 src/aind_data_schema/imaging/__init__.py
 src/aind_data_schema/imaging/acquisition.py
 src/aind_data_schema/imaging/instrument.py
+src/aind_data_schema/imaging/tile.py
 src/aind_data_schema/ophys/__init__.py
 src/aind_data_schema/ophys/ophys_rig.py
 src/aind_data_schema/ophys/ophys_session.py
 src/aind_data_schema/utils/__init__.py
 src/aind_data_schema/utils/json_writer.py
 tests/__init__.py
 tests/test_base.py
```

### Comparing `aind-data-schema-0.9.5/tests/test_base.py` & `aind-data-schema-0.9.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/tests/test_data_description.py` & `aind-data-schema-0.9.6/tests/test_data_description.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/tests/test_ephys.py` & `aind-data-schema-0.9.6/tests/test_ephys.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/tests/test_examples.py` & `aind-data-schema-0.9.6/tests/test_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ testing examples """
 
 import glob
-import importlib
+import importlib.util
 import logging
 import sys
 import unittest
 from pathlib import Path
 from unittest.mock import mock_open, patch
 
 EXAMPLES_DIR = Path(__file__).parents[1] / "examples"
```

### Comparing `aind-data-schema-0.9.5/tests/test_imaging.py` & `aind-data-schema-0.9.6/tests/test_imaging.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import datetime
 import unittest
 
 from pydantic import ValidationError
 
 from aind_data_schema.imaging import acquisition as acq
 from aind_data_schema.imaging import instrument as inst
+from aind_data_schema.imaging import tile
+from aind_data_schema.processing import Stitching
 
 
 class ImagingTests(unittest.TestCase):
     """test imaging schemas"""
 
     def test_constructors(self):
         """testing constructors"""
@@ -21,20 +23,20 @@
             experimenter_full_name="alice",
             session_start_time=datetime.datetime.now(),
             subject_id="1234",
             instrument_id="1234",
             session_end_time=datetime.datetime.now(),
             chamber_immersion=acq.Immersion(medium="PBS", refractive_index=1),
             tiles=[
-                acq.Tile(
+                tile.AcquisitionTile(
                     coordinate_transformations=[
-                        acq.Scale3dTransform(scale=[1, 1, 1]),
-                        acq.Translation3dTransform(translation=[1, 1, 1]),
+                        tile.Scale3dTransform(scale=[1, 1, 1]),
+                        tile.Translation3dTransform(translation=[1, 1, 1]),
                     ],
-                    channel=acq.Channel(
+                    channel=tile.Channel(
                         channel_name="488",
                         laser_wavelength=488,
                         laser_power=0.1,
                         filter_wheel_index=0,
                     ),
                 )
             ],
@@ -61,10 +63,40 @@
         """test the axis class"""
         # test that a few work
         test_codes = ["RAS", "LSP", "RAI", "PAR"]
         for test_code in test_codes:
             axes = acq.Axis.from_direction_code(test_code)
             assert len(axes) == 3
 
+    def test_stitching(self):
+        """test the tile models"""
+
+        t = Stitching(
+            name="Image tile stitching",
+            version="1.0",
+            start_date_time=datetime.datetime.now(),
+            end_date_time=datetime.datetime.now(),
+            input_location="/some/path",
+            output_location="/some/path",
+            code_url="http://foo",
+            parameters={},
+            tiles=[
+                tile.Tile(
+                    coordinate_transformations=[
+                        tile.Affine3dTransform(affine_transform=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11])
+                    ]
+                ),
+                tile.Tile(
+                    coordinate_transformations=[
+                        tile.Translation3dTransform(translation=[0, 1, 2]),
+                        tile.Rotation3dTransform(rotation=[1, 2, 3, 4, 5, 6, 7, 8, 9]),
+                        tile.Scale3dTransform(scale=[1, 2, 3]),
+                    ]
+                ),
+            ],
+        )
+
+        assert t is not None
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aind-data-schema-0.9.5/tests/test_json_writer.py` & `aind-data-schema-0.9.6/tests/test_json_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module to test json_writer classes."""
 
 import os
 import unittest
 from pathlib import Path
-from unittest.mock import call, mock_open, patch, MagicMock
+from unittest.mock import MagicMock, call, mock_open, patch
 
 from aind_data_schema.utils.json_writer import SchemaWriter
 
 
 class SchemaWriterTests(unittest.TestCase):
     """Tests for SchemaWriter methods"""
```

### Comparing `aind-data-schema-0.9.5/tests/test_ophys.py` & `aind-data-schema-0.9.6/tests/test_ophys.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/tests/test_procedures.py` & `aind-data-schema-0.9.6/tests/test_procedures.py`

 * *Files identical despite different names*

### Comparing `aind-data-schema-0.9.5/tests/test_subject.py` & `aind-data-schema-0.9.6/tests/test_subject.py`

 * *Files identical despite different names*

