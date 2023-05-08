# Comparing `tmp/threedi-schema-0.216.4.tar.gz` & `tmp/threedi-schema-0.217.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-schema-0.216.4.tar", last modified: Tue Apr 11 15:14:55 2023, max compression
+gzip compressed data, was "threedi-schema-0.217.0.tar", last modified: Mon May  8 08:44:05 2023, max compression
```

## Comparing `threedi-schema-0.216.4.tar` & `threedi-schema-0.217.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.317389 threedi-schema-0.216.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-11 15:14:55.317389 threedi-schema-0.216.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 15:14:55.321389 threedi-schema-0.216.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.313388 threedi-schema-0.216.4/threedi_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.313388 threedi-schema-0.216.4/threedi_schema/application/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/application/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/application/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/application/threedi_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.313388 threedi-schema-0.216.4/threedi_schema/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/domain/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/domain/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    31610 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.317389 threedi-schema-0.216.4/threedi_schema/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/infrastructure/spatial_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/infrastructure/spatialite_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/infrastructure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.317389 threedi-schema-0.216.4/threedi_schema/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.317389 threedi-schema-0.216.4/threedi_schema/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0200_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0202_remove_unused_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0203_remove_unused_cols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0205_settings_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0206_control_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0208_tables_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0209_remove_surface_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0210_global_raster_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0211_breach_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/0216_vegetation_drag.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.317389 threedi-schema-0.216.4/threedi_schema/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.317389 threedi-schema-0.216.4/threedi_schema/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:46.000000 threedi-schema-0.216.4/threedi_schema/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-11 15:14:47.000000 threedi-schema-0.216.4/threedi_schema/tests/test_gpkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-04-11 15:14:47.000000 threedi-schema-0.216.4/threedi_schema/tests/test_migration_213.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-04-11 15:14:47.000000 threedi-schema-0.216.4/threedi_schema/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-11 15:14:47.000000 threedi-schema-0.216.4/threedi_schema/tests/test_spatalite_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:14:55.313388 threedi-schema-0.216.4/threedi_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-11 15:14:55.000000 threedi-schema-0.216.4/threedi_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-11 15:14:55.000000 threedi-schema-0.216.4/threedi_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:14:55.000000 threedi-schema-0.216.4/threedi_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 15:14:55.000000 threedi-schema-0.216.4/threedi_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:14:55.000000 threedi-schema-0.216.4/threedi_schema.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-11 15:14:55.000000 threedi-schema-0.216.4/threedi_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 15:14:55.000000 threedi-schema-0.216.4/threedi_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.016026 threedi-schema-0.217.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-08 08:44:05.016026 threedi-schema-0.217.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 08:44:05.016026 threedi-schema-0.217.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.008026 threedi-schema-0.217.0/threedi_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.008026 threedi-schema-0.217.0/threedi_schema/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/application/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/application/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/application/threedi_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.012026 threedi-schema-0.217.0/threedi_schema/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/domain/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/domain/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.012026 threedi-schema-0.217.0/threedi_schema/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/infrastructure/spatial_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/infrastructure/spatialite_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/infrastructure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.012026 threedi-schema-0.217.0/threedi_schema/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.012026 threedi-schema-0.217.0/threedi_schema/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0200_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0202_remove_unused_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0203_remove_unused_cols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0205_settings_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0206_control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0208_tables_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0209_remove_surface_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0210_global_raster_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0211_breach_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0216_vegetation_drag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.016026 threedi-schema-0.217.0/threedi_schema/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.016026 threedi-schema-0.217.0/threedi_schema/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:43:58.000000 threedi-schema-0.217.0/threedi_schema/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-08 08:43:59.000000 threedi-schema-0.217.0/threedi_schema/tests/test_gpkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-05-08 08:43:59.000000 threedi-schema-0.217.0/threedi_schema/tests/test_migration_213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-05-08 08:43:59.000000 threedi-schema-0.217.0/threedi_schema/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-08 08:43:59.000000 threedi-schema-0.217.0/threedi_schema/tests/test_spatalite_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:44:05.008026 threedi-schema-0.217.0/threedi_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-08 08:44:04.000000 threedi-schema-0.217.0/threedi_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-08 08:44:05.000000 threedi-schema-0.217.0/threedi_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:44:04.000000 threedi-schema-0.217.0/threedi_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 08:44:04.000000 threedi-schema-0.217.0/threedi_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:44:04.000000 threedi-schema-0.217.0/threedi_schema.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 08:44:04.000000 threedi-schema-0.217.0/threedi_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 08:44:04.000000 threedi-schema-0.217.0/threedi_schema.egg-info/top_level.txt
```

### Comparing `threedi-schema-0.216.4/CHANGES.rst` & `threedi-schema-0.217.0/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog of threedi-schema
 ===================================================
 
+0.217.0 (2023-05-08)
+--------------------
+
+- Rename vegetation columns to match raster options.
+
+
 0.216.4 (2023-04-11)
 --------------------
 
 - Fixed libspatialite 4.3 incompatibility (introduced in 0.216.3).
 
 
 0.216.3 (2023-04-04)
```

### Comparing `threedi-schema-0.216.4/LICENSE` & `threedi-schema-0.217.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/PKG-INFO` & `threedi-schema-0.217.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.216.4
+Version: 0.217.0
 Summary: The schema of 3Di schematization files
 Home-page: https://github.com/nens/threedi-schema
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -81,14 +81,20 @@
 
   $ pip install threedi-schema
 
 
 Changelog of threedi-schema
 ===================================================
 
+0.217.0 (2023-05-08)
+--------------------
+
+- Rename vegetation columns to match raster options.
+
+
 0.216.4 (2023-04-11)
 --------------------
 
 - Fixed libspatialite 4.3 incompatibility (introduced in 0.216.3).
 
 
 0.216.3 (2023-04-04)
```

### Comparing `threedi-schema-0.216.4/README.rst` & `threedi-schema-0.217.0/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/setup.py` & `threedi-schema-0.217.0/setup.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/application/schema.py` & `threedi-schema-0.217.0/threedi_schema/application/schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/application/threedi_database.py` & `threedi-schema-0.217.0/threedi_schema/application/threedi_database.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/beta_features.py` & `threedi-schema-0.217.0/threedi_schema/beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/domain/constants.py` & `threedi-schema-0.217.0/threedi_schema/domain/constants.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/domain/custom_types.py` & `threedi-schema-0.217.0/threedi_schema/domain/custom_types.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/domain/indexes.py` & `threedi-schema-0.217.0/threedi_schema/domain/indexes.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/domain/models.py` & `threedi-schema-0.217.0/threedi_schema/domain/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,25 +361,25 @@
 
 
 class VegetationDrag(Base):
     __tablename__ = "v2_vegetation_drag"
     id = Column(Integer, primary_key=True)
     display_name = Column(String(255))
 
-    height = Column(Float)
-    height_file = Column(String(255))
+    vegetation_height = Column(Float)
+    vegetation_height_file = Column(String(255))
 
-    stem_count = Column(Float)
-    stem_count_file = Column(String(255))
+    vegetation_stem_count = Column(Float)
+    vegetation_stem_count_file = Column(String(255))
 
-    stem_diameter = Column(Float)
-    stem_diameter_file = Column(String(255))
+    vegetation_stem_diameter = Column(Float)
+    vegetation_stem_diameter_file = Column(String(255))
 
-    drag_coefficient = Column(Float)
-    drag_coefficient_file = Column(String(255))
+    vegetation_drag_coefficient = Column(Float)
+    vegetation_drag_coefficient_file = Column(String(255))
 
     global_settings = relationship(
         "GlobalSetting", back_populates="vegetation_drag_settings"
     )
 
 
 class GlobalSetting(Base):
```

### Comparing `threedi-schema-0.216.4/threedi_schema/domain/views.py` & `threedi-schema-0.217.0/threedi_schema/domain/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/infrastructure/spatial_index.py` & `threedi-schema-0.217.0/threedi_schema/infrastructure/spatial_index.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/infrastructure/spatialite_versions.py` & `threedi-schema-0.217.0/threedi_schema/infrastructure/spatialite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/infrastructure/views.py` & `threedi-schema-0.217.0/threedi_schema/infrastructure/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/env.py` & `threedi-schema-0.217.0/threedi_schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0200_initial.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0200_initial.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0202_remove_unused_tables.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0202_remove_unused_tables.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0203_remove_unused_cols.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0203_remove_unused_cols.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0205_settings_defaults.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0205_settings_defaults.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0206_control_structures.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0206_control_structures.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0207_fix_schema_constraints.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0207_fix_schema_constraints.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0208_tables_settings.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0208_tables_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0209_remove_surface_type.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0209_remove_surface_type.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0210_global_raster_values.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0210_global_raster_values.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0211_breach_and_exchange.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0211_breach_and_exchange.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0215_groundwater_1d2d.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0215_groundwater_1d2d.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/migrations/versions/0216_vegetation_drag.py` & `threedi-schema-0.217.0/threedi_schema/migrations/versions/0216_vegetation_drag.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/scripts.py` & `threedi-schema-0.217.0/threedi_schema/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/tests/conftest.py` & `threedi-schema-0.217.0/threedi_schema/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/tests/test_migration_213.py` & `threedi-schema-0.217.0/threedi_schema/tests/test_migration_213.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/tests/test_schema.py` & `threedi-schema-0.217.0/threedi_schema/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema/tests/test_spatalite_versions.py` & `threedi-schema-0.217.0/threedi_schema/tests/test_spatalite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.216.4/threedi_schema.egg-info/PKG-INFO` & `threedi-schema-0.217.0/threedi_schema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.216.4
+Version: 0.217.0
 Summary: The schema of 3Di schematization files
 Home-page: https://github.com/nens/threedi-schema
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -81,14 +81,20 @@
 
   $ pip install threedi-schema
 
 
 Changelog of threedi-schema
 ===================================================
 
+0.217.0 (2023-05-08)
+--------------------
+
+- Rename vegetation columns to match raster options.
+
+
 0.216.4 (2023-04-11)
 --------------------
 
 - Fixed libspatialite 4.3 incompatibility (introduced in 0.216.3).
 
 
 0.216.3 (2023-04-04)
```

### Comparing `threedi-schema-0.216.4/threedi_schema.egg-info/SOURCES.txt` & `threedi-schema-0.217.0/threedi_schema.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 threedi_schema/migrations/versions/0210_global_raster_values.py
 threedi_schema/migrations/versions/0211_breach_and_exchange.py
 threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
 threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
 threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
 threedi_schema/migrations/versions/0215_groundwater_1d2d.py
 threedi_schema/migrations/versions/0216_vegetation_drag.py
+threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
 threedi_schema/migrations/versions/__init__.py
 threedi_schema/tests/__init__.py
 threedi_schema/tests/conftest.py
 threedi_schema/tests/test_gpkg.py
 threedi_schema/tests/test_migration_213.py
 threedi_schema/tests/test_schema.py
 threedi_schema/tests/test_spatalite_versions.py
```

