# Comparing `tmp/rattail_corepos-0.1.8.tar.gz` & `tmp/rattail_corepos-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rattail_corepos-0.1.8.tar", last modified: Fri Nov  5 02:28:38 2021, max compression
+gzip compressed data, was "dist/rattail_corepos-0.1.9.tar", last modified: Sat Nov  6 01:37:44 2021, max compression
```

## Comparing `rattail_corepos-0.1.8.tar` & `rattail_corepos-0.1.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/
--rw-r--r--   0 lance     (1000) lance     (1000)     1155 2021-11-05 02:28:19.000000 rattail_corepos-0.1.8/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 rattail_corepos-0.1.8/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       93 2020-09-17 00:57:42.000000 rattail_corepos-0.1.8/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1201 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      345 2018-06-01 04:09:00.000000 rattail_corepos-0.1.8/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)     1070 2018-06-01 04:33:19.000000 rattail_corepos-0.1.8/rattail_corepos/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2021-11-05 02:28:23.000000 rattail_corepos-0.1.8/rattail_corepos/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-09 20:26:04.000000 rattail_corepos-0.1.8/rattail_corepos/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8709 2021-11-05 02:18:17.000000 rattail_corepos-0.1.8/rattail_corepos/batch/coremember.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6505 2021-02-09 21:31:06.000000 rattail_corepos-0.1.8/rattail_corepos/batch/vendorcatalog.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3667 2020-03-15 17:44:02.000000 rattail_corepos-0.1.8/rattail_corepos/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3244 2021-07-22 01:02:53.000000 rattail_corepos-0.1.8/rattail_corepos/config.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1168 2021-02-06 22:45:25.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/api.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6461 2020-03-27 23:34:20.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/commands.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/common/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/common/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2498 2021-07-22 01:03:31.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/common/importing.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)      993 2020-03-04 05:05:54.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     1005 2020-03-04 05:01:24.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4856 2021-01-30 02:05:34.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/corepos.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1711 2020-03-04 05:00:32.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/csv.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/exporters/
--rw-r--r--   0 lance     (1000) lance     (1000)      984 2020-03-27 23:33:53.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/exporters/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    27835 2020-04-16 01:54:35.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/exporters/catapult_inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7020 2020-07-21 20:07:49.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/exporters/catapult_membership.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1642 2020-03-28 00:11:26.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/exporters/csv.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4728 2021-01-30 02:05:22.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6231 2020-03-04 05:02:05.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/square.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14030 2021-02-09 21:41:22.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10715 2021-01-22 00:15:49.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/importing/rattail.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/lane/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/lane/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/lane/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-07-22 00:10:59.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/lane/importing/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/lane/importing/op/
--rw-r--r--   0 lance     (1000) lance     (1000)     1008 2021-07-22 00:13:03.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/lane/importing/op/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1724 2021-11-04 22:15:41.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/lane/importing/op/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6393 2021-11-04 22:30:07.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/lane/importing/op/office.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/office/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/office/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2884 2021-07-22 01:03:08.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/office/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2682 2020-07-07 02:09:12.000000 rattail_corepos-0.1.8/rattail_corepos/corepos/util.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/datasync/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-03-15 18:37:54.000000 rattail_corepos-0.1.8/rattail_corepos/datasync/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11303 2020-07-09 21:43:01.000000 rattail_corepos-0.1.8/rattail_corepos/datasync/corepos.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7008 2021-02-09 22:10:46.000000 rattail_corepos-0.1.8/rattail_corepos/datasync/rattail.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     1057 2018-06-01 04:32:57.000000 rattail_corepos-0.1.8/rattail_corepos/db/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/db/alembic/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/
--rw-r--r--   0 lance     (1000) lance     (1000)     2292 2020-09-04 23:30:43.000000 rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/130e4632a28a_add_corepos_product_cost.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4955 2021-11-05 01:44:47.000000 rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/50961b4b854a_add_corepos_member_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2190 2021-01-28 03:02:23.000000 rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/7fea5aebddfb_add_store_extension.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9679 2020-07-07 01:23:08.000000 rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/9c5029effe93_more_model_extensions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2191 2020-03-04 20:24:30.000000 rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/b43e93d32275_initial_core_pos_integration_tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2188 2020-03-16 21:57:07.000000 rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/c61f78243ff3_add_person_extension.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/db/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     1273 2021-11-04 23:26:04.000000 rattail_corepos-0.1.8/rattail_corepos/db/model/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/db/model/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-11-04 23:20:13.000000 rattail_corepos-0.1.8/rattail_corepos/db/model/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3611 2021-11-05 01:44:43.000000 rattail_corepos-0.1.8/rattail_corepos/db/model/batch/coremember.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4253 2020-07-31 02:07:27.000000 rattail_corepos-0.1.8/rattail_corepos/db/model/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6396 2020-09-04 23:29:54.000000 rattail_corepos-0.1.8/rattail_corepos/db/model/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2085 2021-01-28 03:09:50.000000 rattail_corepos-0.1.8/rattail_corepos/db/model/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1786 2021-07-22 16:43:47.000000 rattail_corepos-0.1.8/rattail_corepos/emails.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)      992 2020-03-04 20:32:59.000000 rattail_corepos-0.1.8/rattail_corepos/importing/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/importing/corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-03-15 17:33:25.000000 rattail_corepos-0.1.8/rattail_corepos/importing/corepos/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    28359 2021-02-06 22:46:00.000000 rattail_corepos-0.1.8/rattail_corepos/importing/corepos/api.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7254 2021-01-21 23:39:47.000000 rattail_corepos-0.1.8/rattail_corepos/importing/corepos/db.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5555 2021-01-28 03:09:22.000000 rattail_corepos-0.1.8/rattail_corepos/importing/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3037 2021-01-28 04:20:06.000000 rattail_corepos-0.1.8/rattail_corepos/importing/versions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1830 2021-01-21 23:40:04.000000 rattail_corepos-0.1.8/rattail_corepos/products.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/trainwreck/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-17 18:51:19.000000 rattail_corepos-0.1.8/rattail_corepos/trainwreck/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1243 2021-02-19 00:01:32.000000 rattail_corepos-0.1.8/rattail_corepos/trainwreck/commands.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos/trainwreck/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-17 18:51:19.000000 rattail_corepos-0.1.8/rattail_corepos/trainwreck/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9071 2021-02-19 01:54:43.000000 rattail_corepos-0.1.8/rattail_corepos/trainwreck/importing/corepos.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1201 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)     3026 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      910 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)       18 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/rattail_corepos.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2021-11-05 02:28:38.000000 rattail_corepos-0.1.8/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     4947 2021-07-22 00:36:59.000000 rattail_corepos-0.1.8/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1255 2021-11-06 01:37:19.000000 rattail_corepos-0.1.9/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 rattail_corepos-0.1.9/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       93 2020-09-17 00:57:42.000000 rattail_corepos-0.1.9/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1201 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      345 2018-06-01 04:09:00.000000 rattail_corepos-0.1.9/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1070 2018-06-01 04:33:19.000000 rattail_corepos-0.1.9/rattail_corepos/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2021-11-06 01:37:23.000000 rattail_corepos-0.1.9/rattail_corepos/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-09 20:26:04.000000 rattail_corepos-0.1.9/rattail_corepos/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10044 2021-11-06 01:35:33.000000 rattail_corepos-0.1.9/rattail_corepos/batch/coremember.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6505 2021-02-09 21:31:06.000000 rattail_corepos-0.1.9/rattail_corepos/batch/vendorcatalog.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3667 2020-03-15 17:44:02.000000 rattail_corepos-0.1.9/rattail_corepos/commands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3244 2021-07-22 01:02:53.000000 rattail_corepos-0.1.9/rattail_corepos/config.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1168 2021-02-06 22:45:25.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/api.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6461 2020-03-27 23:34:20.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/commands.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/common/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/common/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2498 2021-07-22 01:03:31.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/common/importing.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      993 2020-03-04 05:05:54.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1005 2020-03-04 05:01:24.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4856 2021-01-30 02:05:34.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/corepos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1711 2020-03-04 05:00:32.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/csv.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/
+-rw-r--r--   0 lance     (1000) lance     (1000)      984 2020-03-27 23:33:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    27835 2020-04-16 01:54:35.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/catapult_inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7020 2020-07-21 20:07:49.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/catapult_membership.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1642 2020-03-28 00:11:26.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/csv.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4728 2021-01-30 02:05:22.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6231 2020-03-04 05:02:05.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/square.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14030 2021-02-09 21:41:22.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10715 2021-01-22 00:15:49.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/rattail.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-07-22 00:10:59.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1008 2021-07-22 00:13:03.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1724 2021-11-04 22:15:41.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6393 2021-11-04 22:30:07.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/office.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/office/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/office/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2884 2021-07-22 01:03:08.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/office/commands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2682 2020-07-07 02:09:12.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/datasync/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-03-15 18:37:54.000000 rattail_corepos-0.1.9/rattail_corepos/datasync/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11303 2020-07-09 21:43:01.000000 rattail_corepos-0.1.9/rattail_corepos/datasync/corepos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7008 2021-02-09 22:10:46.000000 rattail_corepos-0.1.9/rattail_corepos/datasync/rattail.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1057 2018-06-01 04:32:57.000000 rattail_corepos-0.1.9/rattail_corepos/db/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2292 2020-09-04 23:30:43.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/130e4632a28a_add_corepos_product_cost.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4955 2021-11-05 01:44:47.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/50961b4b854a_add_corepos_member_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2190 2021-01-28 03:02:23.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/7fea5aebddfb_add_store_extension.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9679 2020-07-07 01:23:08.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/9c5029effe93_more_model_extensions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2191 2020-03-04 20:24:30.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/b43e93d32275_initial_core_pos_integration_tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2188 2020-03-16 21:57:07.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/c61f78243ff3_add_person_extension.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1273 2021-11-04 23:26:04.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-11-04 23:20:13.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3611 2021-11-05 01:44:43.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/batch/coremember.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4253 2020-07-31 02:07:27.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6396 2020-09-04 23:29:54.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2085 2021-01-28 03:09:50.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1786 2021-07-22 16:43:47.000000 rattail_corepos-0.1.9/rattail_corepos/emails.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      992 2020-03-04 20:32:59.000000 rattail_corepos-0.1.9/rattail_corepos/importing/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/importing/corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-03-15 17:33:25.000000 rattail_corepos-0.1.9/rattail_corepos/importing/corepos/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    28359 2021-02-06 22:46:00.000000 rattail_corepos-0.1.9/rattail_corepos/importing/corepos/api.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7254 2021-01-21 23:39:47.000000 rattail_corepos-0.1.9/rattail_corepos/importing/corepos/db.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5555 2021-01-28 03:09:22.000000 rattail_corepos-0.1.9/rattail_corepos/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3037 2021-01-28 04:20:06.000000 rattail_corepos-0.1.9/rattail_corepos/importing/versions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1830 2021-01-21 23:40:04.000000 rattail_corepos-0.1.9/rattail_corepos/products.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-17 18:51:19.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1243 2021-02-19 00:01:32.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/commands.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-17 18:51:19.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9071 2021-02-19 01:54:43.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/importing/corepos.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1201 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)     3026 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      910 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)       18 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     4947 2021-07-22 00:36:59.000000 rattail_corepos-0.1.9/setup.py
```

### Comparing `rattail_corepos-0.1.8/CHANGELOG.md` & `rattail_corepos-0.1.9/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
 # Changelog
 All notable changes to rattail-corepos will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.1.9] - 2021-11-05
+### Changed
+- Add support for 2nd "member type" file in CORE member batch.
+
 ## [0.1.8] - 2021-11-04
 ### Changed
 - Add `custdata` importer for CORE Office -> Lane.
 - Add batch to update CORE member records directly via SQL.
 
 ## [0.1.7] - 2021-08-31
 ### Changed
```

### Comparing `rattail_corepos-0.1.8/COPYING.txt` & `rattail_corepos-0.1.9/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/PKG-INFO` & `rattail_corepos-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail_corepos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Rattail Software Interfaces for CORE POS
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rattail_corepos-0.1.8/rattail_corepos/__init__.py` & `rattail_corepos-0.1.9/rattail_corepos/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/batch/coremember.py` & `rattail_corepos-0.1.9/rattail_corepos/batch/coremember.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,25 +39,14 @@
 
 class CoreMemberBatchHandler(BatchHandler):
     """
     Handler for CORE member batches.
     """
     batch_model_class = CoreMemberBatch
 
-    importing_fields = [
-        'first_name',
-        'last_name',
-        'street',
-        'city',
-        'state',
-        'zipcode',
-        'phone',
-        'email1',
-    ]
-
     def should_populate(self, batch):
         if batch.input_file:
             return True
         return False
 
     def setup(self, batch, progress=None):
         self.core_session = CoreSession()
@@ -77,32 +66,46 @@
             return self.populate_from_file(batch, progress=progress)
         raise NotImplementedError("do not know how to populate this batch")
 
     def populate_from_file(self, batch, progress=None):
         """
         Populate member batch from input data file.
         """
-        # TODO: should detect what type of input file we have, but for
-        # now we only support one kind..
+        # TODO: how should we detect what type of input file we have?
+        # this way is pretty lame but sort of works for testing
+        if 'member-status' in batch.input_file:
+            return self.populate_from_member_file(batch, progress=progress)
+
         return self.populate_from_contact_file(batch, progress=progress)
 
     def populate_from_contact_file(self, batch, progress=None):
         """
         Populate member batch from "contact" CSV input data file.
         """
         input_path = batch.filepath(self.config, batch.input_file)
         input_file = open(input_path, 'rt')
         reader = csv.DictReader(input_file)
         data = list(reader)
         input_file.close()
 
-        batch.set_param('fields', self.importing_fields)
+        fields = [
+            'first_name',
+            'last_name',
+            'street',
+            'city',
+            'state',
+            'zipcode',
+            'phone',
+            'email1',
+        ]
+
+        batch.set_param('fields', fields)
 
         maxlens = {}
-        for field in self.importing_fields:
+        for field in fields:
             maxlens[field] = maxlen(getattr(CoreMemberBatchRow, field))
 
         def append(csvrow, i):
             row = self.make_row()
             row.card_number = int(csvrow['external_id'])
             row.first_name = csvrow['first_name']
             row.last_name = csvrow['last_name']
@@ -111,15 +114,15 @@
             row.state = csvrow['primary_state']
             row.zipcode = csvrow['primary_zip']
             row.phone = csvrow['phone_number']
             # TODO: this seems useful, but maybe in another step?
             # row.phone = self.app.format_phone_number(csvrow['phone_number'])
             row.email1 = csvrow['email']
 
-            for field in self.importing_fields:
+            for field in fields:
                 if len(getattr(row, field)) > maxlens[field]:
                     log.warning("%s field is %s and will be truncated to %s "
                                 "for row #%s in CSV data: %s",
                                 field,
                                 len(getattr(row, field)),
                                 maxlens[field],
                                 i + 1,
@@ -128,15 +131,45 @@
                     setattr(row, field, value[:maxlens[field]])
 
             self.add_row(batch, row)
 
         self.progress_loop(append, data, progress,
                            message="Adding initial rows to batch")
 
+    def populate_from_member_file(self, batch, progress=None):
+        """
+        Populate member batch from "member" CSV input data file.
+        """
+        input_path = batch.filepath(self.config, batch.input_file)
+        input_file = open(input_path, 'rt')
+        reader = csv.DictReader(input_file)
+        data = list(reader)
+        input_file.close()
+
+        fields = [
+            'first_name',
+            'last_name',
+            'member_type_id',
+        ]
+
+        batch.set_param('fields', fields)
+
+        def append(csvrow, i):
+            row = self.make_row()
+            row.card_number = int(csvrow['signup_external_id'])
+            row.first_name = csvrow['signup_first_name']
+            row.last_name = csvrow['signup_last_name']
+            row.member_type_id = int(csvrow['member_type'])
+            self.add_row(batch, row)
+
+        self.progress_loop(append, data, progress,
+                           message="Adding initial rows to batch")
+
     def refresh_row(self, row):
+        batch = row.batch
 
         # clear these first in case they are set
         row.first_name_old = None
         row.last_name_old = None
         row.street_old = None
         row.city_old = None
         row.state_old = None
@@ -170,15 +203,16 @@
 
         if core_customer:
             row.first_name_old = core_customer.first_name
             row.last_name_old = core_customer.last_name
             row.member_type_id_old = core_customer.member_type_id
 
         diffs = []
-        for field in self.importing_fields:
+        fields = batch.get_param('fields')
+        for field in fields:
             if getattr(row, field) != getattr(row, '{}_old'.format(field)):
                 diffs.append(field)
 
         if diffs:
             row.status_code = row.STATUS_FIELDS_CHANGED
             row.status_text = ', '.join(diffs)
         else:
@@ -237,12 +271,16 @@
             if core_customer:
 
                 if 'first_name' in fields:
                     core_customer.first_name = row.first_name
                 if 'last_name' in fields:
                     core_customer.last_name = row.last_name
 
+            if 'member_type_id' in fields:
+                for core_customer in core_member.customers:
+                    core_customer.member_type_id = row.member_type_id
+
         self.progress_loop(update, rows, progress,
                            message="Updating members in CORE-POS")
 
         core_session.commit()
         core_session.close()
```

### Comparing `rattail_corepos-0.1.8/rattail_corepos/batch/vendorcatalog.py` & `rattail_corepos-0.1.9/rattail_corepos/batch/vendorcatalog.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/commands.py` & `rattail_corepos-0.1.9/rattail_corepos/commands.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/config.py` & `rattail_corepos-0.1.9/rattail_corepos/config.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/api.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/api.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/commands.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/commands.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/common/importing.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/common/importing.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/__init__.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/__init__.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/corepos.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/corepos.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/csv.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/csv.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/exporters/__init__.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/exporters/catapult_inventory.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/catapult_inventory.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/exporters/catapult_membership.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/catapult_membership.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/exporters/csv.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/csv.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/model.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/model.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/db/square.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/square.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/model.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/model.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/importing/rattail.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/rattail.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/lane/importing/op/__init__.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/lane/importing/op/model.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/model.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/lane/importing/op/office.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/office.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/office/commands.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/office/commands.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/corepos/util.py` & `rattail_corepos-0.1.9/rattail_corepos/corepos/util.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/datasync/corepos.py` & `rattail_corepos-0.1.9/rattail_corepos/datasync/corepos.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/datasync/rattail.py` & `rattail_corepos-0.1.9/rattail_corepos/datasync/rattail.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/__init__.py` & `rattail_corepos-0.1.9/rattail_corepos/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/130e4632a28a_add_corepos_product_cost.py` & `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/130e4632a28a_add_corepos_product_cost.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/50961b4b854a_add_corepos_member_batch.py` & `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/50961b4b854a_add_corepos_member_batch.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/7fea5aebddfb_add_store_extension.py` & `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/7fea5aebddfb_add_store_extension.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/9c5029effe93_more_model_extensions.py` & `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/9c5029effe93_more_model_extensions.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/b43e93d32275_initial_core_pos_integration_tables.py` & `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/b43e93d32275_initial_core_pos_integration_tables.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/alembic/versions/c61f78243ff3_add_person_extension.py` & `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/c61f78243ff3_add_person_extension.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/model/__init__.py` & `rattail_corepos-0.1.9/rattail_corepos/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/model/batch/coremember.py` & `rattail_corepos-0.1.9/rattail_corepos/db/model/batch/coremember.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/model/people.py` & `rattail_corepos-0.1.9/rattail_corepos/db/model/people.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/model/products.py` & `rattail_corepos-0.1.9/rattail_corepos/db/model/products.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/db/model/stores.py` & `rattail_corepos-0.1.9/rattail_corepos/db/model/stores.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/emails.py` & `rattail_corepos-0.1.9/rattail_corepos/emails.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/importing/__init__.py` & `rattail_corepos-0.1.9/rattail_corepos/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/importing/corepos/__init__.py` & `rattail_corepos-0.1.9/rattail_corepos/importing/corepos/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/importing/corepos/api.py` & `rattail_corepos-0.1.9/rattail_corepos/importing/corepos/api.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/importing/corepos/db.py` & `rattail_corepos-0.1.9/rattail_corepos/importing/corepos/db.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/importing/model.py` & `rattail_corepos-0.1.9/rattail_corepos/importing/model.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/importing/versions.py` & `rattail_corepos-0.1.9/rattail_corepos/importing/versions.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/products.py` & `rattail_corepos-0.1.9/rattail_corepos/products.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/trainwreck/commands.py` & `rattail_corepos-0.1.9/rattail_corepos/trainwreck/commands.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos/trainwreck/importing/corepos.py` & `rattail_corepos-0.1.9/rattail_corepos/trainwreck/importing/corepos.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos.egg-info/PKG-INFO` & `rattail_corepos-0.1.9/rattail_corepos.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-corepos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Rattail Software Interfaces for CORE POS
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rattail_corepos-0.1.8/rattail_corepos.egg-info/SOURCES.txt` & `rattail_corepos-0.1.9/rattail_corepos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/rattail_corepos.egg-info/entry_points.txt` & `rattail_corepos-0.1.9/rattail_corepos.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.8/setup.py` & `rattail_corepos-0.1.9/setup.py`

 * *Files identical despite different names*

