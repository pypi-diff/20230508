# Comparing `tmp/firepit-2.3.8.tar.gz` & `tmp/firepit-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firepit-2.3.8.tar", last modified: Tue Nov 29 13:55:45 2022, max compression
+gzip compressed data, was "firepit-2.3.9.tar", last modified: Fri Dec 16 19:28:37 2022, max compression
```

## Comparing `firepit-2.3.8.tar` & `firepit-2.3.9.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-11-29 13:55:45.906965 firepit-2.3.8/
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      276 2021-07-13 17:45:28.000000 firepit-2.3.8/AUTHORS.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3215 2022-04-20 16:05:40.000000 firepit-2.3.8/CONTRIBUTING.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1253 2022-06-15 19:10:43.000000 firepit-2.3.8/HISTORY.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    11357 2021-05-18 19:04:14.000000 firepit-2.3.8/LICENSE
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      293 2021-03-08 16:01:43.000000 firepit-2.3.8/MANIFEST.in
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4959 2022-11-29 13:55:45.906965 firepit-2.3.8/PKG-INFO
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2033 2022-04-28 18:46:42.000000 firepit-2.3.8/README.rst
-drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-11-29 13:55:45.896965 firepit-2.3.8/docs/
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      608 2021-03-08 15:45:15.000000 firepit-2.3.8/docs/Makefile
-drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-11-29 13:55:45.892965 firepit-2.3.8/docs/_build/
-drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-11-29 13:55:45.892965 firepit-2.3.8/docs/_build/html/
-drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-11-29 13:55:45.897965 firepit-2.3.8/docs/_build/html/_static/
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      286 2022-04-14 12:02:41.000000 firepit-2.3.8/docs/_build/html/_static/file.png
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       90 2022-04-14 12:02:41.000000 firepit-2.3.8/docs/_build/html/_static/minus.png
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       90 2022-04-14 12:02:41.000000 firepit-2.3.8/docs/_build/html/_static/plus.png
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       28 2021-03-08 15:47:24.000000 firepit-2.3.8/docs/authors.rst
--rwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)     4795 2021-11-17 17:46:06.000000 firepit-2.3.8/docs/conf.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       33 2021-03-08 15:47:24.000000 firepit-2.3.8/docs/contributing.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     7010 2022-04-20 16:05:40.000000 firepit-2.3.8/docs/database.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1814 2022-06-07 20:38:25.000000 firepit-2.3.8/docs/firepit.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       28 2021-03-08 15:47:24.000000 firepit-2.3.8/docs/history.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      316 2022-04-20 16:05:40.000000 firepit-2.3.8/docs/index.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1182 2021-07-06 19:55:37.000000 firepit-2.3.8/docs/installation.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      769 2021-03-08 15:59:43.000000 firepit-2.3.8/docs/make.bat
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       58 2022-06-07 20:38:25.000000 firepit-2.3.8/docs/modules.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       27 2021-03-08 15:47:24.000000 firepit-2.3.8/docs/readme.rst
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4107 2022-05-18 12:35:51.000000 firepit-2.3.8/docs/usage.rst
-drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-11-29 13:55:45.899965 firepit-2.3.8/firepit/
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      975 2022-11-29 13:54:58.000000 firepit-2.3.8/firepit/__init__.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    38291 2022-11-29 13:54:58.000000 firepit-2.3.8/firepit/asyncstorage.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    11677 2022-11-29 13:54:58.000000 firepit-2.3.8/firepit/cli.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     8004 2022-09-08 20:16:21.000000 firepit-2.3.8/firepit/deref.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      862 2022-04-20 16:05:40.000000 firepit-2.3.8/firepit/exceptions.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4641 2022-11-07 21:56:26.000000 firepit-2.3.8/firepit/generator.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1289 2022-11-29 13:54:58.000000 firepit-2.3.8/firepit/paramstix.lark
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    24092 2022-11-28 20:35:02.000000 firepit-2.3.8/firepit/pgstorage.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    13860 2022-10-03 16:14:46.000000 firepit-2.3.8/firepit/props.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    20932 2022-09-13 19:03:13.000000 firepit-2.3.8/firepit/query.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    10685 2022-11-29 13:54:58.000000 firepit-2.3.8/firepit/raft.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      365 2022-09-12 17:20:54.000000 firepit-2.3.8/firepit/sdo.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     6424 2022-11-09 19:47:45.000000 firepit-2.3.8/firepit/splint.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    10138 2022-11-29 13:54:58.000000 firepit-2.3.8/firepit/splitter.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    12100 2022-11-09 21:40:20.000000 firepit-2.3.8/firepit/sqlitestorage.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    40306 2022-11-29 13:54:58.000000 firepit-2.3.8/firepit/sqlstorage.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     6158 2022-11-29 13:54:58.000000 firepit-2.3.8/firepit/stix20.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3666 2022-08-15 20:05:08.000000 firepit-2.3.8/firepit/stix21.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      699 2022-11-09 21:40:20.000000 firepit-2.3.8/firepit/timestamp.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      708 2022-11-09 21:40:20.000000 firepit-2.3.8/firepit/validate.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    29190 2022-11-09 21:40:20.000000 firepit-2.3.8/firepit/woodchipper.py
-drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-11-29 13:55:45.900965 firepit-2.3.8/firepit.egg-info/
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4959 2022-11-29 13:55:45.000000 firepit-2.3.8/firepit.egg-info/PKG-INFO
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2067 2022-11-29 13:55:45.000000 firepit-2.3.8/firepit.egg-info/SOURCES.txt
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)        1 2022-11-29 13:55:45.000000 firepit-2.3.8/firepit.egg-info/dependency_links.txt
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       73 2022-11-29 13:55:45.000000 firepit-2.3.8/firepit.egg-info/entry_points.txt
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)        1 2022-11-29 13:55:45.000000 firepit-2.3.8/firepit.egg-info/not-zip-safe
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       79 2022-11-29 13:55:45.000000 firepit-2.3.8/firepit.egg-info/requires.txt
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)        8 2022-11-29 13:55:45.000000 firepit-2.3.8/firepit.egg-info/top_level.txt
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      404 2022-11-29 13:55:45.907965 firepit-2.3.8/setup.cfg
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1770 2022-11-29 13:54:58.000000 firepit-2.3.8/setup.py
-drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-11-29 13:55:45.906965 firepit-2.3.8/tests/
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       37 2021-03-08 15:42:50.000000 firepit-2.3.8/tests/__init__.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)  2654693 2021-07-15 18:54:28.000000 firepit-2.3.8/tests/ccoe_investigator_demo.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1734 2022-11-29 13:54:58.000000 firepit-2.3.8/tests/conftest.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1765 2021-07-27 01:15:30.000000 firepit-2.3.8/tests/conn_a.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1792 2021-07-27 01:15:30.000000 firepit-2.3.8/tests/conn_b.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      102 2021-07-22 13:30:08.000000 firepit-2.3.8/tests/empty_bundle.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      364 2021-10-14 18:09:33.000000 firepit-2.3.8/tests/helpers.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    17283 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/mixed-v4-v6.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     5926 2021-08-23 21:02:01.000000 firepit-2.3.8/tests/one_event.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2483 2022-09-08 20:16:21.000000 firepit-2.3.8/tests/regkey-example.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2199 2022-05-18 12:35:51.000000 firepit-2.3.8/tests/sds_example.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2520 2022-11-29 13:54:58.000000 firepit-2.3.8/tests/service-example.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1295 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/spec_2_1_bundle.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2147 2022-06-15 19:10:43.000000 firepit-2.3.8/tests/test_binning.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)   173638 2021-03-30 23:58:31.000000 firepit-2.3.8/tests/test_bundle.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    11484 2021-07-15 18:54:28.000000 firepit-2.3.8/tests/test_bundle_2.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      842 2022-06-13 20:45:28.000000 firepit-2.3.8/tests/test_cli.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      457 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_custom_objects.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2169 2022-09-08 20:16:21.000000 firepit-2.3.8/tests/test_deref.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3360 2021-01-07 18:40:32.000000 firepit-2.3.8/tests/test_error_bundle.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    12387 2022-10-03 16:14:46.000000 firepit-2.3.8/tests/test_errors.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3068 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_group.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2562 2022-11-29 13:54:58.000000 firepit-2.3.8/tests/test_lookup.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3365 2022-11-29 13:54:58.000000 firepit-2.3.8/tests/test_matching.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      903 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_normalized.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2824 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_null.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2023 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_number_observed.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3372 2020-10-07 20:56:28.000000 firepit-2.3.8/tests/test_procs.csv
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4308 2022-10-03 16:14:46.000000 firepit-2.3.8/tests/test_props.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    16204 2022-06-15 19:10:43.000000 firepit-2.3.8/tests/test_query.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4497 2022-05-18 12:35:51.000000 firepit-2.3.8/tests/test_rewrite.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1910 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_spec_version_2_1.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2212 2022-05-18 12:35:51.000000 firepit-2.3.8/tests/test_splint.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1212 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_stix21.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4200 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_stix21_objects.json
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3514 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_stix_patterns.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    28131 2022-11-29 13:54:58.000000 firepit-2.3.8/tests/test_storage.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2851 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_summary.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1784 2022-11-09 21:40:20.000000 firepit-2.3.8/tests/test_timestamp.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1893 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_timestamped.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2176 2022-11-09 21:40:20.000000 firepit-2.3.8/tests/test_validate.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1272 2022-04-20 16:05:40.000000 firepit-2.3.8/tests/test_value_counts.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2637 2021-08-15 18:46:19.000000 firepit-2.3.8/tests/xtest_dataframe.py
--rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      708 2022-05-18 12:35:51.000000 firepit-2.3.8/tests/zeek_example.log
+drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-12-16 19:28:37.851658 firepit-2.3.9/
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      276 2021-07-13 17:45:28.000000 firepit-2.3.9/AUTHORS.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3215 2022-04-20 16:05:40.000000 firepit-2.3.9/CONTRIBUTING.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1253 2022-06-15 19:10:43.000000 firepit-2.3.9/HISTORY.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    11357 2021-05-18 19:04:14.000000 firepit-2.3.9/LICENSE
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      293 2021-03-08 16:01:43.000000 firepit-2.3.9/MANIFEST.in
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4959 2022-12-16 19:28:37.851658 firepit-2.3.9/PKG-INFO
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2033 2022-04-28 18:46:42.000000 firepit-2.3.9/README.rst
+drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-12-16 19:28:37.740658 firepit-2.3.9/docs/
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      608 2021-03-08 15:45:15.000000 firepit-2.3.9/docs/Makefile
+drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-12-16 19:28:37.733658 firepit-2.3.9/docs/_build/
+drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-12-16 19:28:37.733658 firepit-2.3.9/docs/_build/html/
+drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-12-16 19:28:37.820658 firepit-2.3.9/docs/_build/html/_static/
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      286 2022-04-14 12:02:41.000000 firepit-2.3.9/docs/_build/html/_static/file.png
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       90 2022-04-14 12:02:41.000000 firepit-2.3.9/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       90 2022-04-14 12:02:41.000000 firepit-2.3.9/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       28 2021-03-08 15:47:24.000000 firepit-2.3.9/docs/authors.rst
+-rwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)     4795 2021-11-17 17:46:06.000000 firepit-2.3.9/docs/conf.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       33 2021-03-08 15:47:24.000000 firepit-2.3.9/docs/contributing.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     7010 2022-04-20 16:05:40.000000 firepit-2.3.9/docs/database.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1814 2022-06-07 20:38:25.000000 firepit-2.3.9/docs/firepit.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       28 2021-03-08 15:47:24.000000 firepit-2.3.9/docs/history.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      316 2022-04-20 16:05:40.000000 firepit-2.3.9/docs/index.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1182 2021-07-06 19:55:37.000000 firepit-2.3.9/docs/installation.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      769 2021-03-08 15:59:43.000000 firepit-2.3.9/docs/make.bat
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       58 2022-06-07 20:38:25.000000 firepit-2.3.9/docs/modules.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       27 2021-03-08 15:47:24.000000 firepit-2.3.9/docs/readme.rst
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4107 2022-05-18 12:35:51.000000 firepit-2.3.9/docs/usage.rst
+drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-12-16 19:28:37.828658 firepit-2.3.9/firepit/
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      975 2022-12-16 19:28:25.000000 firepit-2.3.9/firepit/__init__.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    38963 2022-12-16 19:28:25.000000 firepit-2.3.9/firepit/asyncstorage.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    11677 2022-11-29 13:54:58.000000 firepit-2.3.9/firepit/cli.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     8004 2022-09-08 20:16:21.000000 firepit-2.3.9/firepit/deref.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      950 2022-12-16 19:28:25.000000 firepit-2.3.9/firepit/exceptions.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4641 2022-11-07 21:56:26.000000 firepit-2.3.9/firepit/generator.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1289 2022-11-29 13:54:58.000000 firepit-2.3.9/firepit/paramstix.lark
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    24092 2022-11-28 20:35:02.000000 firepit-2.3.9/firepit/pgstorage.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    13860 2022-10-03 16:14:46.000000 firepit-2.3.9/firepit/props.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    20932 2022-09-13 19:03:13.000000 firepit-2.3.9/firepit/query.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    10685 2022-11-29 13:54:58.000000 firepit-2.3.9/firepit/raft.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      365 2022-09-12 17:20:54.000000 firepit-2.3.9/firepit/sdo.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     6424 2022-11-09 19:47:45.000000 firepit-2.3.9/firepit/splint.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    10138 2022-11-29 13:54:58.000000 firepit-2.3.9/firepit/splitter.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    12100 2022-11-09 21:40:20.000000 firepit-2.3.9/firepit/sqlitestorage.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    40325 2022-12-16 19:28:25.000000 firepit-2.3.9/firepit/sqlstorage.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     6158 2022-11-29 13:54:58.000000 firepit-2.3.9/firepit/stix20.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3666 2022-08-15 20:05:08.000000 firepit-2.3.9/firepit/stix21.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      699 2022-11-09 21:40:20.000000 firepit-2.3.9/firepit/timestamp.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      708 2022-11-09 21:40:20.000000 firepit-2.3.9/firepit/validate.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    30139 2022-12-16 19:28:25.000000 firepit-2.3.9/firepit/woodchipper.py
+drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-12-16 19:28:37.830659 firepit-2.3.9/firepit.egg-info/
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4959 2022-12-16 19:28:37.000000 firepit-2.3.9/firepit.egg-info/PKG-INFO
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2094 2022-12-16 19:28:37.000000 firepit-2.3.9/firepit.egg-info/SOURCES.txt
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)        1 2022-12-16 19:28:37.000000 firepit-2.3.9/firepit.egg-info/dependency_links.txt
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       73 2022-12-16 19:28:37.000000 firepit-2.3.9/firepit.egg-info/entry_points.txt
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)        1 2022-12-16 19:28:37.000000 firepit-2.3.9/firepit.egg-info/not-zip-safe
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       79 2022-12-16 19:28:37.000000 firepit-2.3.9/firepit.egg-info/requires.txt
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)        8 2022-12-16 19:28:37.000000 firepit-2.3.9/firepit.egg-info/top_level.txt
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      404 2022-12-16 19:28:37.852658 firepit-2.3.9/setup.cfg
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1769 2022-12-16 19:28:25.000000 firepit-2.3.9/setup.py
+drwxrwxr-x   0 pcoccoli  (1000) pcoccoli  (1000)        0 2022-12-16 19:28:37.851658 firepit-2.3.9/tests/
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)       37 2021-03-08 15:42:50.000000 firepit-2.3.9/tests/__init__.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)  2654693 2021-07-15 18:54:28.000000 firepit-2.3.9/tests/ccoe_investigator_demo.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1734 2022-11-29 13:54:58.000000 firepit-2.3.9/tests/conftest.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1765 2021-07-27 01:15:30.000000 firepit-2.3.9/tests/conn_a.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1792 2021-07-27 01:15:30.000000 firepit-2.3.9/tests/conn_b.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      102 2021-07-22 13:30:08.000000 firepit-2.3.9/tests/empty_bundle.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      364 2021-10-14 18:09:33.000000 firepit-2.3.9/tests/helpers.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    17283 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/mixed-v4-v6.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     5926 2021-08-23 21:02:01.000000 firepit-2.3.9/tests/one_event.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2483 2022-09-08 20:16:21.000000 firepit-2.3.9/tests/regkey-example.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2199 2022-05-18 12:35:51.000000 firepit-2.3.9/tests/sds_example.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2520 2022-11-29 13:54:58.000000 firepit-2.3.9/tests/service-example.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1295 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/spec_2_1_bundle.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1361 2022-12-16 19:28:25.000000 firepit-2.3.9/tests/test_asyncstorage.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2147 2022-06-15 19:10:43.000000 firepit-2.3.9/tests/test_binning.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)   173638 2021-03-30 23:58:31.000000 firepit-2.3.9/tests/test_bundle.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    11484 2021-07-15 18:54:28.000000 firepit-2.3.9/tests/test_bundle_2.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      842 2022-06-13 20:45:28.000000 firepit-2.3.9/tests/test_cli.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      457 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_custom_objects.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2169 2022-09-08 20:16:21.000000 firepit-2.3.9/tests/test_deref.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3360 2021-01-07 18:40:32.000000 firepit-2.3.9/tests/test_error_bundle.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    12387 2022-10-03 16:14:46.000000 firepit-2.3.9/tests/test_errors.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3068 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_group.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2562 2022-11-29 13:54:58.000000 firepit-2.3.9/tests/test_lookup.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3365 2022-11-29 13:54:58.000000 firepit-2.3.9/tests/test_matching.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      903 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_normalized.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2824 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_null.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2023 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_number_observed.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3372 2020-10-07 20:56:28.000000 firepit-2.3.9/tests/test_procs.csv
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4308 2022-10-03 16:14:46.000000 firepit-2.3.9/tests/test_props.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    16204 2022-06-15 19:10:43.000000 firepit-2.3.9/tests/test_query.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4497 2022-05-18 12:35:51.000000 firepit-2.3.9/tests/test_rewrite.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1910 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_spec_version_2_1.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2212 2022-05-18 12:35:51.000000 firepit-2.3.9/tests/test_splint.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1212 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_stix21.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     4200 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_stix21_objects.json
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     3514 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_stix_patterns.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)    28131 2022-11-29 13:54:58.000000 firepit-2.3.9/tests/test_storage.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2851 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_summary.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1784 2022-11-09 21:40:20.000000 firepit-2.3.9/tests/test_timestamp.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1893 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_timestamped.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2176 2022-11-09 21:40:20.000000 firepit-2.3.9/tests/test_validate.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     1272 2022-04-20 16:05:40.000000 firepit-2.3.9/tests/test_value_counts.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)     2637 2021-08-15 18:46:19.000000 firepit-2.3.9/tests/xtest_dataframe.py
+-rw-rw-r--   0 pcoccoli  (1000) pcoccoli  (1000)      708 2022-05-18 12:35:51.000000 firepit-2.3.9/tests/zeek_example.log
```

### Comparing `firepit-2.3.8/CONTRIBUTING.rst` & `firepit-2.3.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/HISTORY.rst` & `firepit-2.3.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/LICENSE` & `firepit-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/PKG-INFO` & `firepit-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: firepit
-Version: 2.3.8
+Version: 2.3.9
 Summary: Columnar storage for STIX 2.0 observations.
 Home-page: https://github.com/opencybersecurityalliance/firepit
 Author: IBM Security
 Author-email: pcoccoli@us.ibm.com
 License: Apache Software License 2.0
 Description: ===============================
         Firepit - STIX Columnar Storage
```

### Comparing `firepit-2.3.8/README.rst` & `firepit-2.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/docs/Makefile` & `firepit-2.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/docs/conf.py` & `firepit-2.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/docs/database.rst` & `firepit-2.3.9/docs/database.rst`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/docs/firepit.rst` & `firepit-2.3.9/docs/firepit.rst`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/docs/installation.rst` & `firepit-2.3.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/docs/make.bat` & `firepit-2.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/docs/usage.rst` & `firepit-2.3.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/__init__.py` & `firepit-2.3.9/firepit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for STIX Columnar Storage."""
 
 __author__ = """IBM Security"""
 __email__ = 'pcoccoli@us.ibm.com'
-__version__ = '2.3.8'
+__version__ = '2.3.9'
 
 
 import re
 
 from importlib import import_module
 from urllib.parse import urlparse
```

### Comparing `firepit-2.3.8/firepit/asyncstorage.py` & `firepit-2.3.9/firepit/asyncstorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 from random import randrange
 
 import asyncpg
 import pandas as pd
 
 import ujson
 from firepit import get_storage, pgstorage
-from firepit.deref import auto_deref
-from firepit.exceptions import InvalidAttr, InvalidStixPath, UnknownViewname
+from firepit.deref import auto_deref_cached
+from firepit.exceptions import (InvalidAttr, InvalidStixPath, UnknownViewname,
+                                SessionNotFound)
 from firepit.pgstorage import (CHECK_FOR_COMMON_SCHEMA,
                                CHECK_FOR_QUERIES_TABLE, INTERNAL_TABLES,
                                LIKE_BIN, MATCH_BIN, MATCH_FUN, SUBNET_FUN,
                                _rewrite_view_def)
 from firepit.props import parse_prop, prop_metadata
 from firepit.query import Column, Limit, Offset, Order, Projection, Query
 from firepit.splitter import RecordList, shorten_extension_name
 from firepit.sqlstorage import (DB_VERSION, SqlStorage, _format_query,
-                                _get_col_dict, _make_aggs, _transform,
-                                get_path_joins)
+                                _make_aggs, _transform, get_path_joins)
 from firepit.validate import validate_name, validate_path
 
 logger = logging.getLogger(__name__)
 
 
 def get_placeholders(n):
     return [f'${i}' for i in range(1, n + 1)]
@@ -64,14 +64,15 @@
             if not res:
                 await self.conn.execute('CREATE SCHEMA IF NOT EXISTS "firepit_common";')
                 await self.conn.execute(MATCH_FUN)
                 await self.conn.execute(MATCH_BIN)
                 await self.conn.execute(LIKE_BIN)
                 await self.conn.execute(SUBNET_FUN)
 
+        #TODO: fail if it already exists
         await self.conn.execute(f'CREATE SCHEMA IF NOT EXISTS "{self.session_id}"')
         await self.conn.execute(f'SET search_path TO "{self.session_id}", firepit_common')
 
         async with self.conn.transaction():
             # create tables, etc.
             for stmt in INTERNAL_TABLES:
                 logger.debug('%s', stmt)
@@ -82,14 +83,15 @@
     async def attach(self):
         """
         Attach/connect to an existing session.  Fail if it doesn't exist.
         """
         logger.debug('Attaching to storage for session %s', self.session_id)
         self.conn = await asyncpg.connect(self.connstring)
         await self.conn.execute(f'SET search_path TO "{self.session_id}", firepit_common')
+        #TODO: fail if it doesn't exist
 
     async def cache(self,
                     query_id: str,
                     bundle: dict):
         """
         Ingest a single, in-memory STIX bundle, labelled with `query_id`.
         """
@@ -161,16 +163,19 @@
                     " FROM information_schema.columns"
                     " WHERE table_schema = $1")
             rows = await self.conn.fetch(stmt, self.session_id)
         return [dict(row) for row in rows]
 
     async def delete(self):
         """Delete ALL data in this store"""
-        stmt = (f'DROP SCHEMA "{self.session_id}" CASCADE')
-        await self.conn.execute(stmt)
+        try:
+            stmt = (f'DROP SCHEMA "{self.session_id}" CASCADE')
+            await self.conn.execute(stmt)
+        except asyncpg.exceptions.InvalidSchemaNameError as e:
+            raise SessionNotFound(self.session_id) from e
 
     async def set_appdata(self, viewname, data):
         """Attach app-specific data to a viewname"""
         validate_name(viewname)
         stmt = ('UPDATE "__symtable" SET appdata = $1'
                 ' WHERE name = $2')
         await self.conn.execute(stmt, data, viewname)
@@ -284,16 +289,17 @@
                     qry.extend(joins)
                     proj.append(Column(target_column, table=target_table, alias=col))
                 else:
                     proj.append(Column(col, viewname))
             qry.append(Projection(proj))
         else:
             if not col_dict:
-                col_dict = _get_col_dict(self)
-            joins, proj = auto_deref(col_dict, viewname, self.types())
+                col_dict = await self._get_col_dict()
+            dbcols = await self.columns(viewname)
+            joins, proj = auto_deref_cached(viewname, dbcols, col_dict)
             if joins:
                 qry.extend(joins)
             if proj:
                 qry.append(proj)
         if sort:
             qry.append(Order([sort]))
         if limit:
@@ -355,20 +361,30 @@
                 select = re.sub(f'FROM "{viewname}"', f'FROM ({slct}) AS tmp', select, count=1)
                 select = re.sub(f'"{viewname}"', 'tmp', select)
             await self.conn.execute(f'CREATE OR REPLACE VIEW "{viewname}" AS {select}')
             if is_new:
                 await self._new_name(viewname, sco_type)
 
     async def _is_sql_view(self, name):
-        viewdef = self.conn.fetchone("SELECT definition"
-                                     " FROM pg_views"
-                                     " WHERE schemaname = %s"
-                                     " AND viewname = %s", self.session_id, name)
+        viewdef = await self.conn.fetchrow(
+            "SELECT definition"
+            " FROM pg_views"
+            " WHERE schemaname = $1"
+            " AND viewname = $2",
+            self.session_id, name)
         return viewdef is not None
 
+    async def _get_col_dict(self):
+        q = Query('__columns')
+        col_dict = defaultdict(list)
+        results = await self.run_query(q)
+        for result in results:
+            col_dict[result['otype']].append(result['path'])
+        return col_dict
+
 
 class AsyncSplitWriter:
     """
     Writes STIX objects using `writer`.  This class will track schema
     changes and store `batchsize` objects in memory before passing to
     `writer`.
 
@@ -462,16 +478,15 @@
         if add_table:
             self.schemas[obj_type] = schema
             try:
                 await self.writer.new_type(obj_type, schema)
                 logger.debug('Added new type %s', obj_type)
             except (asyncpg.exceptions.DuplicateTableError,
                     asyncpg.exceptions.UniqueViolationError,
-                    asyncpg.exceptions.DuplicateObjectError) as e:
-                logger.error('TEMP: %s', e)
+                    asyncpg.exceptions.DuplicateObjectError):
                 logger.debug('Failed to add %s; refreshing schemas', obj_type)
                 # Refresh schemas
                 loaded_schema = await self._load_schema(obj_type)
                 new_columns = {}
                 # We only need the new columns we discovered
                 # Don't care if we loaded new ones
                 for key in set(schema) - set(loaded_schema):
@@ -594,20 +609,22 @@
         logger.debug('new_property: %s', stmt)
         await self.conn.execute(stmt)
 
     async def write_records(self, obj_type, records, schema, replace, query_id):
         logger.debug('Writing %d %s objects (%d props)', len(records), obj_type, len(schema))
         tablename = f'{self.prefix}{obj_type}'
 
+        # Load records into dataframe and do type conversions as required
+        df = pd.DataFrame(records)
+        await self.write_df(tablename, df, query_id, schema)
+
+    async def write_df(self, tablename, df, query_id, schema):
         # Generate random tmp table name
         r = randrange(0, 1000000)
         tmp = f'tmp{r}_{tablename}'
-
-        # Load records into dataframe and do type conversions as required
-        df = pd.DataFrame(records)
         columns = df.columns
         for col in columns:
             if col not in schema:
                 #df = df.drop(columns=col)
                 continue
             stype = schema[col].lower()
             if stype == 'text':
@@ -668,15 +685,15 @@
             else:
                 stmt += f' ORDER BY "{colnames[0]}"'  # Any port in a storm...
                 stmt += ' ON CONFLICT DO NOTHING'
             logger.debug('upsert: %s', stmt)
             try:
                 await self.conn.execute(stmt)
             except asyncpg.exceptions.CardinalityViolationError as e:
-                logger.error('CardinalityViolationError for %s', obj_type)
+                logger.error('CardinalityViolationError for %s', tablename)
                 logger.critical('%s', e, exc_info=e)
                 raise e
 
             # Don't need the temp table anymore
             await self.conn.execute(f'DROP TABLE "{tmp}"')
 
         if query_id and 'id' in colnames:
@@ -974,11 +991,14 @@
         """
         return self.store.assign_query(viewname, query, sco_type)
 
     async def lookup(self, viewname, cols="*", limit=None, offset=None, col_dict=None):
         """Get the value of `viewname`"""
         return self.store.lookup(viewname, cols, limit, offset, col_dict)
 
+    async def _is_sql_view(self, name):
+        return self.store._is_sql_view(name)
+
 
 async def get_async_storage(store: SqlStorage) -> SyncWrapper:
     """Wrap a sync SqlStorage object with an async interface"""
     return SyncWrapper(store=store)
```

### Comparing `firepit-2.3.8/firepit/cli.py` & `firepit-2.3.9/firepit/cli.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/deref.py` & `firepit-2.3.9/firepit/deref.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/exceptions.py` & `firepit-2.3.9/firepit/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,7 +45,15 @@
 class UnexpectedError(Exception):
     pass
 
 
 class DatabaseMismatch(Exception):
     def __init__(self, dbversion, expected):
         super().__init__(f'got version {dbversion}; expected {expected}')
+
+
+class SessionNotFound(Exception):
+    pass
+
+
+class SessionExists(Exception):
+    pass
```

### Comparing `firepit-2.3.8/firepit/generator.py` & `firepit-2.3.9/firepit/generator.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/paramstix.lark` & `firepit-2.3.9/firepit/paramstix.lark`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/pgstorage.py` & `firepit-2.3.9/firepit/pgstorage.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/props.py` & `firepit-2.3.9/firepit/props.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/query.py` & `firepit-2.3.9/firepit/query.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/raft.py` & `firepit-2.3.9/firepit/raft.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/splint.py` & `firepit-2.3.9/firepit/splint.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/splitter.py` & `firepit-2.3.9/firepit/splitter.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/sqlitestorage.py` & `firepit-2.3.9/firepit/sqlitestorage.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/sqlstorage.py` & `firepit-2.3.9/firepit/sqlstorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             aggs.append(agg)
     return Aggregation(aggs)
 
 
 def infer_type(key, value):
     if key == 'id':
         rtype = 'TEXT UNIQUE'
-    elif key in ['src_port', 'dst_port', 'x_firepit_rank']:
+    elif key in ['number_observed', 'src_port', 'dst_port', 'x_firepit_rank']:
         rtype = 'INTEGER'
     elif key == 'ipfix.flowId':
         rtype = 'TEXT'  # Should be uint64, but that's not supported anywhere!
     elif isinstance(value, int):
         rtype = 'BIGINT'
     elif isinstance(value, float):
         rtype = 'REAL'
```

### Comparing `firepit-2.3.8/firepit/stix20.py` & `firepit-2.3.9/firepit/stix20.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/stix21.py` & `firepit-2.3.9/firepit/stix21.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/timestamp.py` & `firepit-2.3.9/firepit/timestamp.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/validate.py` & `firepit-2.3.9/firepit/validate.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/firepit/woodchipper.py` & `firepit-2.3.9/firepit/woodchipper.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,19 @@
     event_id = int(event_id)
     return [
         ('x-oca-event:code', event_id),
         ('x-oca-event:action', windows_events.get(event_id)),
     ]
 
 
+def to_cat_list(category):
+    value = category if isinstance(category, list) else [category]
+    return [('x-oca-event:category', value)]
+
+
 def to_payload_bin(value):
     return [
         ('artifact:payload_bin', base64.b64encode(value.encode()).decode('ascii'))
     ]
 
 
 PROTO_TABLE = {num:name[8:] for name, num in vars(socket).items() if name.startswith("IPPROTO")}
@@ -322,28 +327,40 @@
     ]
 
 
 def is_file_event(event_id):
     return event_id in {6, 7, 9, 11, 15}
 
 
-def split_hash(hash_string: str):
+def split_hash(hash_string: str, prefix: str, tag: str = ''):
     token_dict = {
-        "SHA1=": "process:binary_ref.hashes.'SHA-1'",
-        "MD5=": "process:binary_ref.hashes.MD5",
-        "SHA256=": "process:binary_ref.hashes.'SHA-256'"
+        "SHA1=": f"{prefix}hashes.'SHA-1'{tag}",
+        "MD5=": f"{prefix}hashes.MD5{tag}",
+        "SHA256=": f"{prefix}hashes.'SHA-256'{tag}"
     }
     hashes = []
     for hstr in hash_string.split(','):
         for hash_token, _stix_key in token_dict.items():
             if hash_token in hstr:
                 hashes += [(token_dict[hash_token], hstr[len(hash_token):])]
     return hashes
 
 
+def split_image_hash(hash_string: str):
+    return split_hash(hash_string, 'process:binary_ref.')
+
+
+def split_file_hash(hash_string: str):
+    return split_hash(hash_string, 'file:')
+
+
+def split_loaded_hash(hash_string: str):
+    return split_hash(hash_string, 'file:', '#loaded')
+
+
 def split_image(abs_name: str, prefix='process:'):
     name = ntpath.basename(abs_name)
     path = ntpath.dirname(abs_name)
     return [
         (prefix + 'name', name),
         (prefix + 'binary_ref.name', name),
         (prefix + 'binary_ref.parent_directory_ref.path', path)
@@ -359,14 +376,23 @@
     path = ntpath.dirname(abs_name)
     return [
         ('file:name#loaded', name),
         ('file:parent_directory_ref.path#loaded', path)
     ]
 
 
+def split_file_path(abs_name: str, prefix='file:'):
+    name = ntpath.basename(abs_name)
+    path = ntpath.dirname(abs_name)
+    return [
+        (prefix + 'name', name),
+        (prefix + 'parent_directory_ref.path', path)
+    ]
+
+
 def split_reg_key_value(path: str):
     key, _, value = path.rpartition('\\')
     return [
         ('windows-registry-key:key', key),
         ('windows-registry-key:values', [{'name': value}]),
     ]
 
@@ -412,15 +438,15 @@
         "ParentImage": split_parent_image,
         "ParentProcessId": "process:parent_ref.pid",
         "ParentProcessGuid": "process:parent_ref.x_unique_id",
         "ParentCommandLine": "process:parent_ref.command_line",
         #"UserID": "process:creator_user_ref.user_id",
         #"User": "process:creator_user_ref.account_login",
         "User": "process:creator_user_ref.user_id",
-        "Hashes": split_hash,
+        "Hashes": split_image_hash,
     },
     3: {
         "UtcTime": ["first_observed", "last_observed"],
         "Image": split_image,
         "ProcessId": "process:pid",
         "ProcessGuid": "process:x_unique_id",
         "SourceIp": "process:opened_connection_refs[0].src_ref.value",
@@ -438,15 +464,22 @@
     7: {
         "UtcTime": ["first_observed", "last_observed"],
         "Image": split_image,
         "ImageLoaded": split_image_loaded,
         "ProcessId": "process:pid",
         "ProcessGuid": "process:x_unique_id",
         "CommandLine": ["process:command_line"],
-        "Hashes": split_hash,
+        "Hashes": split_loaded_hash,
+    },
+    11: {
+        "UtcTime": ["first_observed", "last_observed"],
+        "Image": split_image,
+        "ProcessId": "process:pid",
+        "ProcessGuid": "process:x_unique_id",
+        "TargetFilename": split_file_path,
     },
     12: {
         "UtcTime": ["first_observed", "last_observed"],
         "Image": split_image,
         "ProcessId": "process:pid",
         "ProcessGuid": "process:x_unique_id",
         "TargetObject": "windows-registry-key:key",  # OR: "process:x_created_key_ref.key"?
@@ -564,15 +597,15 @@
     common_mapping = {
         "@timestamp": ["first_observed", "last_observed"],
         "TimeCreated": ["first_observed", "last_observed"],
         "Channel": "x-oca-event:module",
         "SourceName": "x-oca-event:provider",
         "Hostname": "x-oca-asset:hostname",
         "EventID": to_action_code,
-        "Category": "x-oca-event:category",
+        "Category": to_cat_list,  # "x-oca-event:category" is defined to be a list
         "Message": lambda x: SdsMapper.enhanced_action(x),
         #"Message": to_payload_bin,
         "ProcessName": split_image,  # At least some events use this instead of Image
         "ProcessId": "process:pid",
         "ProcessGuid": "process:x_unique_id",
         "Application": split_image,  # At least some events use this instead of Image
     }
```

### Comparing `firepit-2.3.8/firepit.egg-info/PKG-INFO` & `firepit-2.3.9/firepit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: firepit
-Version: 2.3.8
+Version: 2.3.9
 Summary: Columnar storage for STIX 2.0 observations.
 Home-page: https://github.com/opencybersecurityalliance/firepit
 Author: IBM Security
 Author-email: pcoccoli@us.ibm.com
 License: Apache Software License 2.0
 Description: ===============================
         Firepit - STIX Columnar Storage
```

### Comparing `firepit-2.3.8/firepit.egg-info/SOURCES.txt` & `firepit-2.3.9/firepit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 tests/helpers.py
 tests/mixed-v4-v6.json
 tests/one_event.json
 tests/regkey-example.json
 tests/sds_example.json
 tests/service-example.json
 tests/spec_2_1_bundle.json
+tests/test_asyncstorage.py
 tests/test_binning.py
 tests/test_bundle.json
 tests/test_bundle_2.json
 tests/test_cli.py
 tests/test_custom_objects.py
 tests/test_deref.py
 tests/test_error_bundle.json
```

### Comparing `firepit-2.3.8/setup.py` & `firepit-2.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'tabulate',
     'typer',
     'ujson'
 ]
 
 setup_requirements = ['pytest-runner', 'wheel']
 
-test_requirements = ['pytest>=3', ]
+test_requirements = ['pytest>=3',]
 
 setup(
     author="IBM Security",
     author_email='pcoccoli@us.ibm.com',
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 4 - Beta',
@@ -55,10 +55,10 @@
     keywords='stix stix-shifter sql python',
     name='firepit',
     packages=find_packages(include=['firepit', 'firepit.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opencybersecurityalliance/firepit',
-    version='2.3.8',
+    version='2.3.9',
     zip_safe=False,
 )
```

### Comparing `firepit-2.3.8/tests/ccoe_investigator_demo.json` & `firepit-2.3.9/tests/ccoe_investigator_demo.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/conftest.py` & `firepit-2.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/conn_a.json` & `firepit-2.3.9/tests/conn_a.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/conn_b.json` & `firepit-2.3.9/tests/conn_b.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/mixed-v4-v6.json` & `firepit-2.3.9/tests/mixed-v4-v6.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/one_event.json` & `firepit-2.3.9/tests/one_event.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/regkey-example.json` & `firepit-2.3.9/tests/regkey-example.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/sds_example.json` & `firepit-2.3.9/tests/sds_example.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/service-example.json` & `firepit-2.3.9/tests/service-example.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/spec_2_1_bundle.json` & `firepit-2.3.9/tests/spec_2_1_bundle.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_binning.py` & `firepit-2.3.9/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_bundle.json` & `firepit-2.3.9/tests/test_bundle.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_bundle_2.json` & `firepit-2.3.9/tests/test_bundle_2.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_cli.py` & `firepit-2.3.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_deref.py` & `firepit-2.3.9/tests/test_deref.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_error_bundle.json` & `firepit-2.3.9/tests/test_error_bundle.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_errors.py` & `firepit-2.3.9/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_group.py` & `firepit-2.3.9/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_lookup.py` & `firepit-2.3.9/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_matching.py` & `firepit-2.3.9/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_normalized.py` & `firepit-2.3.9/tests/test_normalized.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_null.py` & `firepit-2.3.9/tests/test_null.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_number_observed.py` & `firepit-2.3.9/tests/test_number_observed.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_procs.csv` & `firepit-2.3.9/tests/test_procs.csv`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_props.py` & `firepit-2.3.9/tests/test_props.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_query.py` & `firepit-2.3.9/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_rewrite.py` & `firepit-2.3.9/tests/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_spec_version_2_1.py` & `firepit-2.3.9/tests/test_spec_version_2_1.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_splint.py` & `firepit-2.3.9/tests/test_splint.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_stix21.py` & `firepit-2.3.9/tests/test_stix21.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_stix21_objects.json` & `firepit-2.3.9/tests/test_stix21_objects.json`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_stix_patterns.py` & `firepit-2.3.9/tests/test_stix_patterns.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_storage.py` & `firepit-2.3.9/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_summary.py` & `firepit-2.3.9/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_timestamp.py` & `firepit-2.3.9/tests/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_timestamped.py` & `firepit-2.3.9/tests/test_timestamped.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_validate.py` & `firepit-2.3.9/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/test_value_counts.py` & `firepit-2.3.9/tests/test_value_counts.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/xtest_dataframe.py` & `firepit-2.3.9/tests/xtest_dataframe.py`

 * *Files identical despite different names*

### Comparing `firepit-2.3.8/tests/zeek_example.log` & `firepit-2.3.9/tests/zeek_example.log`

 * *Files identical despite different names*

