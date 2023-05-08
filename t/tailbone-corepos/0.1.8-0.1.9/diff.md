# Comparing `tmp/tailbone-corepos-0.1.8.tar.gz` & `tmp/tailbone-corepos-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tailbone-corepos-0.1.8.tar", last modified: Sat Nov  6 01:38:23 2021, max compression
+gzip compressed data, was "dist/tailbone-corepos-0.1.9.tar", last modified: Thu Mar  3 03:40:48 2022, max compression
```

## Comparing `tailbone-corepos-0.1.8.tar` & `tailbone-corepos-0.1.9.tar`

### file list

```diff
@@ -1,104 +1,107 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/
--rw-r--r--   0 lance     (1000) lance     (1000)     1811 2021-11-06 01:38:01.000000 tailbone-corepos-0.1.8/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 tailbone-corepos-0.1.8/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       95 2021-08-02 14:05:01.000000 tailbone-corepos-0.1.8/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1196 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      383 2019-07-09 21:36:41.000000 tailbone-corepos-0.1.8/README.rst
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     3738 2019-07-10 04:12:36.000000 tailbone-corepos-0.1.8/setup.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)     1010 2019-07-09 21:38:59.000000 tailbone-corepos-0.1.8/tailbone_corepos/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2021-11-06 01:38:06.000000 tailbone-corepos-0.1.8/tailbone_corepos/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1604 2020-11-20 00:50:35.000000 tailbone-corepos-0.1.8/tailbone_corepos/db.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7657 2021-10-15 03:32:54.000000 tailbone-corepos-0.1.8/tailbone_corepos/menus.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/batch/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/batch/corepos-member/
--rw-r--r--   0 lance     (1000) lance     (1000)     1130 2021-11-05 02:19:35.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/batch/corepos-member/view_row.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/customers/
--rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/customers/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/departments/
--rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/departments/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/employees/
--rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:18.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/employees/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/master/
--rw-r--r--   0 lance     (1000) lance     (1000)      247 2020-03-15 00:36:36.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/master/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/members/
--rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/members/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/origins/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/origins/countries/
--rw-r--r--   0 lance     (1000) lance     (1000)      292 2021-10-15 02:50:33.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/origins/countries/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      636 2021-10-15 03:02:40.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/origins/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/origins/regions/
--rw-r--r--   0 lance     (1000) lance     (1000)      292 2021-10-15 02:50:33.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/origins/regions/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/origins/stateprov/
--rw-r--r--   0 lance     (1000) lance     (1000)      292 2021-10-15 02:50:33.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/origins/stateprov/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/products/
--rw-r--r--   0 lance     (1000) lance     (1000)      315 2020-12-09 19:05:35.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/products/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      308 2020-12-03 20:55:08.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/products/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/products-user/
--rw-r--r--   0 lance     (1000) lance     (1000)      300 2020-12-09 19:06:06.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/products-user/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/purchase-orders/
--rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/purchase-orders/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/vendor-items/
--rw-r--r--   0 lance     (1000) lance     (1000)      297 2020-12-03 21:00:31.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/vendor-items/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)      312 2020-12-03 20:55:28.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/vendors/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/vendors/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      605 2021-02-01 20:58:31.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/corepos-util.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/departments/
--rw-r--r--   0 lance     (1000) lance     (1000)      270 2020-03-15 02:03:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/departments/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/people/
--rw-r--r--   0 lance     (1000) lance     (1000)      841 2021-10-08 01:13:30.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/people/view_profile_buefy.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/products/
--rw-r--r--   0 lance     (1000) lance     (1000)      640 2021-01-21 02:30:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/products/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/purchases/
--rw-r--r--   0 lance     (1000) lance     (1000)     3483 2021-02-02 16:59:45.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/purchases/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)      247 2020-03-15 00:36:36.000000 tailbone-corepos-0.1.8/tailbone_corepos/templates/vendors/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/
--rw-r--r--   0 lance     (1000) lance     (1000)     1031 2019-07-09 21:42:05.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-11-04 23:39:10.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4822 2021-11-06 01:36:22.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/batch/coremember.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)     2360 2021-09-01 22:45:48.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3990 2020-08-16 21:59:05.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/batches.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3555 2020-08-16 21:18:23.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/coupons.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7082 2021-09-30 22:47:29.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/customers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2686 2021-01-01 01:01:09.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/departments.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2523 2020-12-02 04:00:06.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/employees.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3429 2021-05-05 01:11:27.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/likecodes.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4902 2021-02-01 21:35:41.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5151 2021-09-30 22:48:43.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/members.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6805 2021-10-15 03:31:20.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/origins.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1668 2020-03-23 17:29:22.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/parameters.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11771 2021-09-20 02:13:06.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4761 2021-02-01 21:36:03.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/purchaseorders.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2047 2020-09-02 16:31:10.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/scaleitems.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2356 2021-01-28 04:22:46.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1879 2020-04-09 01:56:10.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/subdepartments.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4149 2021-01-01 01:01:00.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/superdepartments.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1408 2021-08-02 13:55:47.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/tablesyncrules.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1662 2020-03-30 18:39:17.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/taxrates.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4206 2020-12-02 03:54:42.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/transactions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2209 2021-09-30 22:49:02.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/users.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3018 2021-02-14 22:05:45.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/vendoritems.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2514 2020-03-31 19:12:57.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/vendors.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2893 2021-10-08 00:43:46.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/customers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2975 2021-01-28 22:40:17.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/departments.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1984 2020-07-07 01:56:46.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/members.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3151 2021-10-08 01:13:52.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4334 2021-10-01 14:07:34.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5070 2021-02-02 18:11:32.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/purchases.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1867 2021-01-28 22:40:48.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2106 2021-01-28 22:41:00.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/subdepartments.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3166 2021-10-01 14:13:54.000000 tailbone-corepos-0.1.8/tailbone_corepos/views/vendors.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1196 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)     3140 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)       37 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       17 2021-11-06 01:38:23.000000 tailbone-corepos-0.1.8/tailbone_corepos.egg-info/top_level.txt
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2070 2022-03-03 03:40:26.000000 tailbone-corepos-0.1.9/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 tailbone-corepos-0.1.9/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       95 2021-08-02 14:05:01.000000 tailbone-corepos-0.1.9/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1196 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      383 2019-07-09 21:36:41.000000 tailbone-corepos-0.1.9/README.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     3738 2019-07-10 04:12:36.000000 tailbone-corepos-0.1.9/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1010 2019-07-09 21:38:59.000000 tailbone-corepos-0.1.9/tailbone_corepos/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2022-03-03 03:40:32.000000 tailbone-corepos-0.1.9/tailbone_corepos/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1604 2020-11-20 00:50:35.000000 tailbone-corepos-0.1.9/tailbone_corepos/db.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7869 2022-01-18 01:00:08.000000 tailbone-corepos-0.1.9/tailbone_corepos/menus.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/batch/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/batch/corepos-member/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1130 2021-11-05 02:19:35.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/batch/corepos-member/view_row.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/customers/
+-rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/customers/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/departments/
+-rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/departments/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/employees/
+-rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:18.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/employees/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/master/
+-rw-r--r--   0 lance     (1000) lance     (1000)      247 2020-03-15 00:36:36.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/master/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/members/
+-rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/members/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/origins/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/origins/countries/
+-rw-r--r--   0 lance     (1000) lance     (1000)      292 2021-10-15 02:50:33.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/origins/countries/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      636 2021-10-15 03:02:40.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/origins/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/origins/regions/
+-rw-r--r--   0 lance     (1000) lance     (1000)      292 2021-10-15 02:50:33.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/origins/regions/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/origins/stateprov/
+-rw-r--r--   0 lance     (1000) lance     (1000)      292 2021-10-15 02:50:33.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/origins/stateprov/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/products/
+-rw-r--r--   0 lance     (1000) lance     (1000)      315 2020-12-09 19:05:35.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/products/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      308 2020-12-03 20:55:08.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/products/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/products-user/
+-rw-r--r--   0 lance     (1000) lance     (1000)      300 2020-12-09 19:06:06.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/products-user/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/purchase-orders/
+-rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/purchase-orders/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/user-groups/
+-rw-r--r--   0 lance     (1000) lance     (1000)      286 2022-01-17 20:52:43.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/user-groups/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/vendor-items/
+-rw-r--r--   0 lance     (1000) lance     (1000)      297 2020-12-03 21:00:31.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/vendor-items/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)      312 2020-12-03 20:55:28.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/vendors/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       90 2020-03-15 01:47:08.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/vendors/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      605 2021-02-01 20:58:31.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/corepos-util.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/departments/
+-rw-r--r--   0 lance     (1000) lance     (1000)      270 2020-03-15 02:03:23.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/departments/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/people/
+-rw-r--r--   0 lance     (1000) lance     (1000)      841 2021-10-08 01:13:30.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/people/view_profile_buefy.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/products/
+-rw-r--r--   0 lance     (1000) lance     (1000)      640 2021-01-21 02:30:23.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/products/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/purchases/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3483 2021-02-02 16:59:45.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/purchases/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)      247 2020-03-15 00:36:36.000000 tailbone-corepos-0.1.9/tailbone_corepos/templates/vendors/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1031 2019-07-09 21:42:05.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-11-04 23:39:10.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5013 2021-11-06 01:44:27.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/batch/coremember.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2420 2022-01-18 01:00:24.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4350 2022-02-18 18:41:27.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/batches.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3709 2022-02-18 18:41:21.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/coupons.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7302 2022-02-18 18:41:14.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/customers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2837 2022-02-18 18:41:07.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/departments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2668 2022-02-18 18:41:01.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/employees.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4706 2022-02-18 18:34:36.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/groups.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3574 2022-02-18 18:40:51.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/likecodes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4902 2021-02-01 21:35:41.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5365 2022-02-18 18:40:45.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/members.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7211 2022-02-18 18:43:13.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/origins.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1816 2022-02-18 18:40:28.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/parameters.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12091 2022-02-18 18:40:20.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4921 2022-02-18 18:40:15.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/purchaseorders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2195 2022-02-18 18:40:08.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/scaleitems.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2492 2022-02-18 18:40:01.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2039 2022-02-18 18:39:54.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/subdepartments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4315 2022-02-18 18:39:47.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/superdepartments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1568 2022-02-18 18:39:39.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/tablesyncrules.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1804 2022-02-18 18:39:33.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/taxrates.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4378 2022-02-18 18:39:25.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/transactions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2342 2022-02-18 18:39:17.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/users.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3169 2022-02-18 18:39:09.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/vendoritems.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2653 2022-02-18 18:38:59.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/vendors.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2893 2021-10-08 00:43:46.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/customers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2975 2021-01-28 22:40:17.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/departments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1984 2020-07-07 01:56:46.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/members.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3151 2021-10-08 01:13:52.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4240 2022-01-18 01:00:55.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5070 2021-02-02 18:11:32.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/purchases.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1867 2021-01-28 22:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2106 2021-01-28 22:41:00.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/subdepartments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3166 2021-10-01 14:13:54.000000 tailbone-corepos-0.1.9/tailbone_corepos/views/vendors.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1196 2022-03-03 03:40:47.000000 tailbone-corepos-0.1.9/tailbone_corepos.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)     3239 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2022-03-03 03:40:47.000000 tailbone-corepos-0.1.9/tailbone_corepos.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)       37 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       17 2022-03-03 03:40:48.000000 tailbone-corepos-0.1.9/tailbone_corepos.egg-info/top_level.txt
```

### Comparing `tailbone-corepos-0.1.8/CHANGELOG.md` & `tailbone-corepos-0.1.9/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 
 # Changelog
 All notable changes to tailbone-corepos will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.1.9] - 2022-03-02
+### Changed
+- Show input filename column in CORE member batches grid.
+- Include views for PendingProduct model.
+- Tweak exposure for some fields.
+- Add basic views for CORE user groups.
+- Update config defaults for all corepos views.
+
 ## [0.1.8] - 2021-11-05
 ### Changed
 - Show member type names for CORE member batch.
 
 ## [0.1.7] - 2021-11-04
 ### Changed
 - Add views for CORE "Users" and "Suspensions".
```

### Comparing `tailbone-corepos-0.1.8/COPYING.txt` & `tailbone-corepos-0.1.9/COPYING.txt`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/PKG-INFO` & `tailbone-corepos-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailbone-corepos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tailbone interfaces for CORE POS
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tailbone-corepos-0.1.8/setup.py` & `tailbone-corepos-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/__init__.py` & `tailbone-corepos-0.1.9/tailbone_corepos/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/db.py` & `tailbone-corepos-0.1.9/tailbone_corepos/db.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/menus.py` & `tailbone-corepos-0.1.9/tailbone_corepos/menus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -64,14 +64,19 @@
                         'perm': 'corepos.employees.list',
                     },
                     {
                         'title': "Users",
                         'url': url('corepos.users'),
                         'perm': 'corepos.users.list',
                     },
+                    {
+                        'title': "User Groups",
+                        'url': url('corepos.user_groups'),
+                        'perm': 'corepos.user_groups.list',
+                    },
                 ],
             },
             {
                 'title': "Products",
                 'type': 'menu',
                 'items': [
                     {
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/templates/batch/corepos-member/view_row.mako` & `tailbone-corepos-0.1.9/tailbone_corepos/templates/batch/corepos-member/view_row.mako`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/templates/core-pos/origins/index.mako` & `tailbone-corepos-0.1.9/tailbone_corepos/templates/core-pos/origins/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/templates/corepos-util.mako` & `tailbone-corepos-0.1.9/tailbone_corepos/templates/corepos-util.mako`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/templates/people/view_profile_buefy.mako` & `tailbone-corepos-0.1.9/tailbone_corepos/templates/people/view_profile_buefy.mako`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/templates/products/view.mako` & `tailbone-corepos-0.1.9/tailbone_corepos/templates/products/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/templates/purchases/view.mako` & `tailbone-corepos-0.1.9/tailbone_corepos/templates/purchases/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/__init__.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/batch/coremember.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/batch/coremember.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,25 @@
     model_row_class = CoreMemberBatchRow
     batch_handler_class = CoreMemberBatchHandler
     route_prefix = 'batch.coremember'
     url_prefix = '/batch/corepos-member'
     downloadable = True
     rows_bulk_deletable = True
 
+    grid_columns = [
+        'id',
+        'description',
+        'input_file',
+        'created',
+        'created_by',
+        'rowcount',
+        'executed',
+        'executed_by',
+    ]
+
     form_fields = [
         'id',
         'input_file',
         'description',
         'notes',
         'params',
         'created',
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/__init__.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -27,14 +27,15 @@
 from .master import CoreOfficeMasterView
 
 
 def includeme(config):
     config.include('tailbone_corepos.views.corepos.parameters')
     config.include('tailbone_corepos.views.corepos.tablesyncrules')
     config.include('tailbone_corepos.views.corepos.users')
+    config.include('tailbone_corepos.views.corepos.groups')
     config.include('tailbone_corepos.views.corepos.stores')
     config.include('tailbone_corepos.views.corepos.departments')
     config.include('tailbone_corepos.views.corepos.subdepartments')
     config.include('tailbone_corepos.views.corepos.superdepartments')
     config.include('tailbone_corepos.views.corepos.vendors')
     config.include('tailbone_corepos.views.corepos.vendoritems')
     config.include('tailbone_corepos.views.corepos.origins')
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/batches.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/batches.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -139,15 +139,28 @@
         return item.batch
 
     def configure_row_grid(self, g):
         super(BatchView, self).configure_row_grid(g)
 
         g.set_type('sale_price', 'currency')
         g.set_type('group_sale_price', 'currency')
-        g.set_type('cost', 'currency')
+        # TODO: some older installs don't have this field
+        if hasattr(corepos.BatchItem, 'cost'):
+            g.set_type('cost', 'currency')
+        else:
+            g.remove('cost')
 
         g.set_sort_defaults('id')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    BatchTypeView = kwargs.get('BatchTypeView', base['BatchTypeView'])
     BatchTypeView.defaults(config)
+
+    BatchView = kwargs.get('BatchView', base['BatchView'])
     BatchView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/coupons.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/coupons.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -111,9 +111,16 @@
         f.set_type('start_date', 'date_jquery')
 
         f.set_renderer('end_date', self.render_local_date)
         f.set_readonly('end_date') # TODO
         f.set_type('end_date', 'date_jquery')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    HouseCouponView = kwargs.get('HouseCouponView', base['HouseCouponView'])
     HouseCouponView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/customers.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/customers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -226,10 +226,19 @@
 
         f.set_type('charge_limit', 'currency')
 
     def render_member_info(self, custdata, field):
         return render_member_info(self.request, custdata, field)
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    CustomerView = kwargs.get('CustomerView', base['CustomerView'])
     CustomerView.defaults(config)
+
+    SuspensionView = kwargs.get('SuspensionView', base['SuspensionView'])
     SuspensionView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/departments.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/departments.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -84,9 +84,16 @@
         f.set_type('modified', 'datetime_local')
 
     def core_office_object_url(self, office_url, department):
         return '{}/item/departments/DepartmentEditor.php?did={}'.format(
             office_url, department.number)
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    DepartmentView = kwargs.get('DepartmentView', base['DepartmentView'])
     DepartmentView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/employees.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/employees.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -76,9 +76,16 @@
         f.set_readonly('birth_date')
 
     def core_office_object_url(self, office_url, employee):
         return '{}/admin/Cashiers/CashierEditor.php?emp_no={}'.format(
             office_url, employee.number)
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    EmployeeView = kwargs.get('EmployeeView', base['EmployeeView'])
     EmployeeView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/likecodes.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/likecodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -120,9 +120,16 @@
 
         g.set_sort_defaults('upc')
 
         g.set_link('upc')
         g.set_link('description')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    LikeCodeView = kwargs.get('LikeCodeView', base['LikeCodeView'])
     LikeCodeView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/master.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/master.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/members.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/members.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -176,10 +176,19 @@
 
     def core_office_object_url(self, office_url, member):
         return core_office_customer_account_url(self.rattail_config,
                                                 member.card_number,
                                                 office_url=office_url)
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    MemberTypeView = kwargs.get('MemberTypeView', base['MemberTypeView'])
     MemberTypeView.defaults(config)
+
+    MemberView = kwargs.get('MemberView', base['MemberView'])
     MemberView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/origins.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/origins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -200,12 +200,25 @@
             text = str(region)
             if self.request.has_perm('corepos.origin_regions.view'):
                 url = self.request.route_url('corepos.origin_regions.view', id=region.id)
                 return tags.link_to(text, url)
             return text
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    OriginCountryView = kwargs.get('OriginCountryView', base['OriginCountryView'])
     OriginCountryView.defaults(config)
+
+    OriginStateProvinceView = kwargs.get('OriginStateProvinceView', base['OriginStateProvinceView'])
     OriginStateProvinceView.defaults(config)
+
+    OriginRegionView = kwargs.get('OriginRegionView', base['OriginRegionView'])
     OriginRegionView.defaults(config)
+
+    OriginView = kwargs.get('OriginView', base['OriginView'])
     OriginView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/parameters.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -49,9 +49,16 @@
     def configure_grid(self, g):
         super(ParameterView, self).configure_grid(g)
 
         g.set_link('param_key')
         g.set_link('param_value')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    ParameterView = kwargs.get('ParameterView', base['ParameterView'])
     ParameterView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/products.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/products.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -348,14 +348,15 @@
         'description',
         'brand',
         'sizing',
         'long_text',
         'photo',
         'enable_online',
         'sold_out',
+        'sign_count',
     ]
 
     def configure_grid(self, g):
         super(ProductUserView, self).configure_grid(g)
 
         g.filters['upc'].default_active = True
         g.filters['upc'].default_verb = 'contains'
@@ -388,11 +389,22 @@
         g.set_link('description')
 
     def grid_extra_class(self, flag, i):
         if not flag.active:
             return 'warning'
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    ProductView = kwargs.get('ProductView', base['ProductView'])
     ProductView.defaults(config)
+
+    ProductUserView = kwargs.get('ProductUserView', base['ProductUserView'])
     ProductUserView.defaults(config)
+
+    ProductFlagView = kwargs.get('ProductFlagView', base['ProductFlagView'])
     ProductFlagView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/purchaseorders.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/purchaseorders.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -155,9 +155,16 @@
         g.set_type('unit_cost', 'currency')
         g.set_type('case_size', 'quantity')
         g.set_type('quantity', 'quantity')
         g.set_type('received_quantity', 'quantity')
         g.set_type('received_total_cost', 'currency')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    PurchaseOrderView = kwargs.get('PurchaseOrderView', base['PurchaseOrderView'])
     PurchaseOrderView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/scaleitems.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/scaleitems.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -66,9 +66,16 @@
 
     def configure_form(self, f):
         super(ScaleItemView, self).configure_form(f)
 
         f.set_renderer('product', self.render_corepos_product)
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    ScaleItemView = kwargs.get('ScaleItemView', base['ScaleItemView'])
     ScaleItemView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/stores.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/stores.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -80,9 +80,16 @@
 
         g.set_sort_defaults('id')
 
         g.set_link('id')
         g.set_link('description')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    StoreView = kwargs.get('StoreView', base['StoreView'])
     StoreView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/subdepartments.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/subdepartments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -55,9 +55,16 @@
 
         g.set_sort_defaults('number')
 
         g.set_link('number')
         g.set_link('name')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    SubdepartmentView = kwargs.get('SubdepartmentView', base['SubdepartmentView'])
     SubdepartmentView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/superdepartments.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/superdepartments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -131,9 +131,16 @@
         super(SuperDepartmentView, self).configure_row_grid(g)
 
         g.set_type('modified', 'datetime_local')
 
         g.set_sort_defaults('number')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    SuperDepartmentView = kwargs.get('SuperDepartmentView', base['SuperDepartmentView'])
     SuperDepartmentView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/tablesyncrules.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/tablesyncrules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -35,9 +35,16 @@
     """
     model_class = corepos.TableSyncRule
     model_title = "CORE-POS Table Sync Rule"
     url_prefix = '/core-pos/table-sync-rules'
     route_prefix = 'corepos.table_sync_rules'
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    TableSyncRuleView = kwargs.get('TableSyncRuleView', base['TableSyncRuleView'])
     TableSyncRuleView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/taxrates.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/taxrates.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -53,9 +53,16 @@
     def configure_grid(self, g):
         super(TaxRateView, self).configure_grid(g)
 
         g.set_link('id')
         g.set_link('description')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    TaxRateView = kwargs.get('TaxRateView', base['TaxRateView'])
     TaxRateView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/transactions.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/transactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -123,9 +123,16 @@
         config.add_route('{}.import_square'.format(route_prefix), '{}/import-square'.format(url_prefix))
         config.add_view(cls, attr='import_square', route_name='{}.import_square'.format(route_prefix),
                         permission='{}.import_file'.format(permission_prefix))
 
         cls._defaults(config)
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    TransactionDetailView = kwargs.get('TransactionDetailView', base['TransactionDetailView'])
     TransactionDetailView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/users.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/users.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -78,9 +78,16 @@
     def configure_form(self, f):
         super(UserView, self).configure_form(f)
 
         if not hasattr(corepos.User, 'email'):
             f.remove('email')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    UserView = kwargs.get('UserView', base['UserView'])
     UserView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/vendoritems.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/vendoritems.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -109,9 +109,16 @@
 
         if self.creating or self.editing:
             f.remove('modified')
         else:
             f.set_readonly('modified')
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    VendorItemView = kwargs.get('VendorItemView', base['VendorItemView'])
     VendorItemView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/corepos/vendors.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/corepos/vendors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -87,9 +87,16 @@
             f.remove_field('contact')
 
     def core_office_object_url(self, office_url, vendor):
         return '{}/item/vendors/VendorIndexPage.php?vid={}'.format(
             office_url, vendor.id)
 
 
-def includeme(config):
+def defaults(config, **kwargs):
+    base = globals()
+
+    VendorView = kwargs.get('VendorView', base['VendorView'])
     VendorView.defaults(config)
+
+
+def includeme(config):
+    defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/customers.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/customers.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/departments.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/departments.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/members.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/members.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/people.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/people.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/products.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/products.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         else:
             kwargs['core_office_url'] = '{}/item/ItemEditorPage.php?searchupc={}'.format(
                 office_url, product.item_id)
 
         return kwargs
 
 
-def includeme(config):
+# TODO: this seems awkward here, but makes things less awkward to
+# modules using this one as their base
+PendingProductView = base.PendingProductView
 
-    # TODO: getting pretty tired of copy/pasting this extra config...
-    config.add_route('products.print_labels', '/products/labels')
-    config.add_view(base.print_labels, route_name='products.print_labels',
-                    renderer='json', permission='products.print_labels')
 
+def includeme(config):
     ProductView.defaults(config)
+    PendingProductView.defaults(config)
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/purchases.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/purchases.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/stores.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/stores.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/subdepartments.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/subdepartments.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos/views/vendors.py` & `tailbone-corepos-0.1.9/tailbone_corepos/views/vendors.py`

 * *Files identical despite different names*

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos.egg-info/PKG-INFO` & `tailbone-corepos-0.1.9/tailbone_corepos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailbone-corepos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tailbone interfaces for CORE POS
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tailbone-corepos-0.1.8/tailbone_corepos.egg-info/SOURCES.txt` & `tailbone-corepos-0.1.9/tailbone_corepos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 tailbone_corepos/templates/core-pos/origins/countries/index.mako
 tailbone_corepos/templates/core-pos/origins/regions/index.mako
 tailbone_corepos/templates/core-pos/origins/stateprov/index.mako
 tailbone_corepos/templates/core-pos/products/index.mako
 tailbone_corepos/templates/core-pos/products/view.mako
 tailbone_corepos/templates/core-pos/products-user/index.mako
 tailbone_corepos/templates/core-pos/purchase-orders/view.mako
+tailbone_corepos/templates/core-pos/user-groups/view.mako
 tailbone_corepos/templates/core-pos/vendor-items/index.mako
 tailbone_corepos/templates/core-pos/vendors/index.mako
 tailbone_corepos/templates/core-pos/vendors/view.mako
 tailbone_corepos/templates/departments/view.mako
 tailbone_corepos/templates/people/view_profile_buefy.mako
 tailbone_corepos/templates/products/view.mako
 tailbone_corepos/templates/purchases/view.mako
@@ -50,14 +51,15 @@
 tailbone_corepos/views/batch/coremember.py
 tailbone_corepos/views/corepos/__init__.py
 tailbone_corepos/views/corepos/batches.py
 tailbone_corepos/views/corepos/coupons.py
 tailbone_corepos/views/corepos/customers.py
 tailbone_corepos/views/corepos/departments.py
 tailbone_corepos/views/corepos/employees.py
+tailbone_corepos/views/corepos/groups.py
 tailbone_corepos/views/corepos/likecodes.py
 tailbone_corepos/views/corepos/master.py
 tailbone_corepos/views/corepos/members.py
 tailbone_corepos/views/corepos/origins.py
 tailbone_corepos/views/corepos/parameters.py
 tailbone_corepos/views/corepos/products.py
 tailbone_corepos/views/corepos/purchaseorders.py
```

