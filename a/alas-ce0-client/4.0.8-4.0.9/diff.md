# Comparing `tmp/alas-ce0-client-4.0.8.tar.gz` & `tmp/alas-ce0-client-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alas-ce0-client-4.0.8.tar", last modified: Wed Aug 17 23:48:02 2022, max compression
+gzip compressed data, was "dist/alas-ce0-client-4.0.9.tar", last modified: Thu Aug 18 00:04:33 2022, max compression
```

## Comparing `alas-ce0-client-4.0.8.tar` & `alas-ce0-client-4.0.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/
--rw-r--r--   0 lzambra    (501) staff       (20)      950 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/PKG-INFO
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0/
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0/clients/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/clients/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      748 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/clients/core.py
--rw-r--r--   0 lzambra    (501) staff       (20)     6223 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/clients/api_client.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0/reporting/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/reporting/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      323 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/reporting/regional_partner_report.py
--rw-r--r--   0 lzambra    (501) staff       (20)      311 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/reporting/report_manager.py
--rw-r--r--   0 lzambra    (501) staff       (20)      495 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/reporting/report.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0/scheduling/
--rw-r--r--   0 lzambra    (501) staff       (20)     2412 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/scheduling/route.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/scheduling/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0/integration/
--rw-r--r--   0 lzambra    (501) staff       (20)      274 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/integration/shipper.py
--rw-r--r--   0 lzambra    (501) staff       (20)      283 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/integration/whatsapp.py
--rw-r--r--   0 lzambra    (501) staff       (20)      596 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/integration/device_magic.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/integration/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0/management/
--rw-r--r--   0 lzambra    (501) staff       (20)      349 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/distribution_zone.py
--rw-r--r--   0 lzambra    (501) staff       (20)      462 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/geographic_coverage_active.py
--rw-r--r--   0 lzambra    (501) staff       (20)      531 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/configuration.py
--rw-r--r--   0 lzambra    (501) staff       (20)      584 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/user.py
--rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/task.py
--rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/shelf.py
--rw-r--r--   0 lzambra    (501) staff       (20)      336 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/service_level.py
--rw-r--r--   0 lzambra    (501) staff       (20)      160 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/roles_group.py
--rw-r--r--   0 lzambra    (501) staff       (20)     1130 2022-07-17 21:07:20.000000 alas-ce0-client-4.0.8/alas_ce0/management/bulk.py
--rw-r--r--   0 lzambra    (501) staff       (20)      337 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/maintenance.py
--rw-r--r--   0 lzambra    (501) staff       (20)      757 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/notification.py
--rw-r--r--   0 lzambra    (501) staff       (20)      316 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/vehicle.py
--rw-r--r--   0 lzambra    (501) staff       (20)      155 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/resource.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      169 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/product_template.py
--rw-r--r--   0 lzambra    (501) staff       (20)      147 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/role.py
--rw-r--r--   0 lzambra    (501) staff       (20)      153 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/feature.py
--rw-r--r--   0 lzambra    (501) staff       (20)      352 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/packaging.py
--rw-r--r--   0 lzambra    (501) staff       (20)      917 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/employee.py
--rw-r--r--   0 lzambra    (501) staff       (20)      609 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/barcode.py
--rw-r--r--   0 lzambra    (501) staff       (20)      362 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/cross_docking.py
--rw-r--r--   0 lzambra    (501) staff       (20)      298 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/package_template.py
--rw-r--r--   0 lzambra    (501) staff       (20)     1066 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/delivery_entity.py
--rw-r--r--   0 lzambra    (501) staff       (20)      492 2022-08-17 20:26:11.000000 alas-ce0-client-4.0.8/alas_ce0/management/geographic_coverage.py
--rw-r--r--   0 lzambra    (501) staff       (20)      152 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/management/contact.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0/common/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/common/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)    12200 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/common/client_base.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0/task/
--rw-r--r--   0 lzambra    (501) staff       (20)      289 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/task/data_job.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/task/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0/delivery/
--rw-r--r--   0 lzambra    (501) staff       (20)      307 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/delivery/b2c.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/alas_ce0/delivery/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)    34405 2022-08-17 23:46:58.000000 alas-ce0-client-4.0.8/alas_ce0/delivery/delivery_order.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0_client.egg-info/
--rw-r--r--   0 lzambra    (501) staff       (20)      950 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0_client.egg-info/PKG-INFO
--rw-r--r--   0 lzambra    (501) staff       (20)     1758 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0_client.egg-info/SOURCES.txt
--rw-r--r--   0 lzambra    (501) staff       (20)       55 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0_client.egg-info/requires.txt
--rw-r--r--   0 lzambra    (501) staff       (20)        9 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0_client.egg-info/top_level.txt
--rw-r--r--   0 lzambra    (501) staff       (20)        1 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/alas_ce0_client.egg-info/dependency_links.txt
--rw-r--r--   0 lzambra    (501) staff       (20)      238 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/MANIFEST.in
--rw-r--r--   0 lzambra    (501) staff       (20)     3892 2022-08-17 23:46:33.000000 alas-ce0-client-4.0.8/setup.py
--rw-r--r--   0 lzambra    (501) staff       (20)       67 2022-08-17 23:48:02.000000 alas-ce0-client-4.0.8/setup.cfg
--rw-r--r--   0 lzambra    (501) staff       (20)      260 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/README.rst
--rw-r--r--   0 lzambra    (501) staff       (20)       23 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.8/LICENSE.txt
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/
+-rw-r--r--   0 lzambra    (501) staff       (20)      950 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/PKG-INFO
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/clients/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/clients/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      748 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/clients/core.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     6223 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/clients/api_client.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      323 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/regional_partner_report.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      311 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/report_manager.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      495 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/report.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/scheduling/
+-rw-r--r--   0 lzambra    (501) staff       (20)     2412 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/scheduling/route.py
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/scheduling/__init__.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/integration/
+-rw-r--r--   0 lzambra    (501) staff       (20)      274 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/integration/shipper.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      283 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/integration/whatsapp.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      596 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/integration/device_magic.py
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/integration/__init__.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/management/
+-rw-r--r--   0 lzambra    (501) staff       (20)      349 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/distribution_zone.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      462 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/geographic_coverage_active.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      531 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/configuration.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      584 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/user.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/task.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/shelf.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      336 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/service_level.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      160 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/roles_group.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     1130 2022-07-17 21:07:20.000000 alas-ce0-client-4.0.9/alas_ce0/management/bulk.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      337 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/maintenance.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      757 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/notification.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      316 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/vehicle.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      155 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/resource.py
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      169 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/product_template.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      147 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/role.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      153 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/feature.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      352 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/packaging.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      917 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/employee.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      609 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/barcode.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      362 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/cross_docking.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      298 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/package_template.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     1066 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/delivery_entity.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      492 2022-08-17 20:26:11.000000 alas-ce0-client-4.0.9/alas_ce0/management/geographic_coverage.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      152 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/contact.py
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/__init__.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/common/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/common/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)    12200 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/common/client_base.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/task/
+-rw-r--r--   0 lzambra    (501) staff       (20)      289 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/task/data_job.py
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/task/__init__.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/delivery/
+-rw-r--r--   0 lzambra    (501) staff       (20)      307 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/delivery/b2c.py
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/delivery/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)    34402 2022-08-18 00:03:42.000000 alas-ce0-client-4.0.9/alas_ce0/delivery/delivery_order.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/
+-rw-r--r--   0 lzambra    (501) staff       (20)      950 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/PKG-INFO
+-rw-r--r--   0 lzambra    (501) staff       (20)     1758 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/SOURCES.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)       55 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/requires.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)        9 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/top_level.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)        1 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/dependency_links.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)      238 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/MANIFEST.in
+-rw-r--r--   0 lzambra    (501) staff       (20)     3892 2022-08-18 00:04:09.000000 alas-ce0-client-4.0.9/setup.py
+-rw-r--r--   0 lzambra    (501) staff       (20)       67 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/setup.cfg
+-rw-r--r--   0 lzambra    (501) staff       (20)      260 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/README.rst
+-rw-r--r--   0 lzambra    (501) staff       (20)       23 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/LICENSE.txt
```

### Comparing `alas-ce0-client-4.0.8/PKG-INFO` & `alas-ce0-client-4.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alas-ce0-client
-Version: 4.0.8
+Version: 4.0.9
 Summary: API client for Alas.Ce0 project
 Home-page: https://github.com/pypa/alas-ce0-client
 Author: Leonardo Zambra
 Author-email: lzambra@alasxpress.com
 License: MIT
 Description: Alas Ce0 Client API
         =======================
```

### Comparing `alas-ce0-client-4.0.8/alas_ce0/clients/core.py` & `alas-ce0-client-4.0.9/alas_ce0/clients/core.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/clients/api_client.py` & `alas-ce0-client-4.0.9/alas_ce0/clients/api_client.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/scheduling/route.py` & `alas-ce0-client-4.0.9/alas_ce0/scheduling/route.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/integration/device_magic.py` & `alas-ce0-client-4.0.9/alas_ce0/integration/device_magic.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/management/configuration.py` & `alas-ce0-client-4.0.9/alas_ce0/management/configuration.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/management/user.py` & `alas-ce0-client-4.0.9/alas_ce0/management/user.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/management/bulk.py` & `alas-ce0-client-4.0.9/alas_ce0/management/bulk.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/management/notification.py` & `alas-ce0-client-4.0.9/alas_ce0/management/notification.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/management/employee.py` & `alas-ce0-client-4.0.9/alas_ce0/management/employee.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/management/barcode.py` & `alas-ce0-client-4.0.9/alas_ce0/management/barcode.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/management/delivery_entity.py` & `alas-ce0-client-4.0.9/alas_ce0/management/delivery_entity.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/common/client_base.py` & `alas-ce0-client-4.0.9/alas_ce0/common/client_base.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/alas_ce0/delivery/delivery_order.py` & `alas-ce0-client-4.0.9/alas_ce0/delivery/delivery_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
         return event_info['schedule_rejected_1_comments']
     if 'schedule_rejected_2_comments' in event_info and event_info['schedule_rejected_2_comments']:
         return event_info['schedule_rejected_2_comments']
     if 'schedule_rejected_3_comments' in event_info and event_info['schedule_rejected_3_comments']:
         return event_info['schedule_rejected_3_comments']
     return None
 
-def get_status_details(delivery_order):
+def get_status_info(delivery_order):
     events_info, status, description, last_event_timestamp = None, None, None, None
 
     if delivery_order['status'] == DeliveryOrderStatusType.Planning.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
```

### Comparing `alas-ce0-client-4.0.8/alas_ce0_client.egg-info/PKG-INFO` & `alas-ce0-client-4.0.9/alas_ce0_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alas-ce0-client
-Version: 4.0.8
+Version: 4.0.9
 Summary: API client for Alas.Ce0 project
 Home-page: https://github.com/pypa/alas-ce0-client
 Author: Leonardo Zambra
 Author-email: lzambra@alasxpress.com
 License: MIT
 Description: Alas Ce0 Client API
         =======================
```

### Comparing `alas-ce0-client-4.0.8/alas_ce0_client.egg-info/SOURCES.txt` & `alas-ce0-client-4.0.9/alas_ce0_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.8/setup.py` & `alas-ce0-client-4.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
-API_CLIENT_VERSION = '4.0.8'
+API_CLIENT_VERSION = '4.0.9'
 
 setup(
     name='alas-ce0-client',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
```

