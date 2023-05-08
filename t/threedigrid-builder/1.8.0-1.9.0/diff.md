# Comparing `tmp/threedigrid-builder-1.8.0.tar.gz` & `tmp/threedigrid-builder-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedigrid-builder-1.8.0.tar", last modified: Thu Jan 19 14:52:56 2023, max compression
+gzip compressed data, was "threedigrid-builder-1.9.0.tar", last modified: Mon Mar  6 14:48:44 2023, max compression
```

## Comparing `threedigrid-builder-1.8.0.tar` & `threedigrid-builder-1.9.0.tar`

### file list

```diff
@@ -1,105 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:56.823770 threedigrid-builder-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35274 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-01-19 14:52:56.823770 threedigrid-builder-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:56.811770 threedigrid-builder-1.8.0/libthreedigrid/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/libthreedigrid/_fgrid.pyf
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/libthreedigrid/array_utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/libthreedigrid/cells.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/libthreedigrid/geo_utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/libthreedigrid/parameters.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/libthreedigrid/quadtree.f90
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-01-19 14:52:56.823770 threedigrid-builder-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:56.811770 threedigrid-builder-1.8.0/threedigrid_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:56.811770 threedigrid-builder-1.8.0/threedigrid_builder/base/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14163 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)    17762 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/linestrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/pumps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/base/surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:56.815770 threedigrid-builder-1.8.0/threedigrid_builder/grid/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/boundary_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/connection_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/cross_section_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/dem_average_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/exchange_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:56.815770 threedigrid-builder-1.8.0/threedigrid_builder/grid/fgrid/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/fgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34704 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/grid_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/groundwater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/initial_waterlevels.py
--rw-r--r--   0 runner    (1001) docker     (123)    15754 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/obstacles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/potential_breaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/quadtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/windshielding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/grid/zero_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:56.815770 threedigrid-builder-1.8.0/threedigrid_builder/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30945 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/interface/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/interface/dict_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/interface/geopackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    31388 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/interface/gridadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/interface/raster_gdal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:56.823770 threedigrid-builder-1.8.0/threedigrid_builder/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-01-19 14:52:52.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_boundary_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_connection_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_cross_section_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_dem_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_dict_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_exchange_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_grid_refinements.py
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_gridadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_groundwater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_initial_waterlevels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_linestrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_obstacles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_potential_breaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_pumps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_quadtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_raster_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_windshielding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-01-19 14:52:53.000000 threedigrid-builder-1.8.0/threedigrid_builder/tests/test_zero_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:52:56.811770 threedigrid-builder-1.8.0/threedigrid_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-01-19 14:52:56.000000 threedigrid-builder-1.8.0/threedigrid_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-01-19 14:52:56.000000 threedigrid-builder-1.8.0/threedigrid_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 14:52:56.000000 threedigrid-builder-1.8.0/threedigrid_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-19 14:52:56.000000 threedigrid-builder-1.8.0/threedigrid_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 14:52:56.000000 threedigrid-builder-1.8.0/threedigrid_builder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-19 14:52:56.000000 threedigrid-builder-1.8.0/threedigrid_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-19 14:52:56.000000 threedigrid-builder-1.8.0/threedigrid_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:44.062993 threedigrid-builder-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35274 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-06 14:48:44.062993 threedigrid-builder-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:44.054993 threedigrid-builder-1.9.0/libthreedigrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/libthreedigrid/_fgrid.pyf
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/libthreedigrid/array_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/libthreedigrid/cells.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/libthreedigrid/geo_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/libthreedigrid/parameters.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/libthreedigrid/quadtree.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-06 14:48:44.062993 threedigrid-builder-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:44.054993 threedigrid-builder-1.9.0/threedigrid_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:44.054993 threedigrid-builder-1.9.0/threedigrid_builder/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/line_halfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17762 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/linestrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/pumps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/base/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:44.058993 threedigrid-builder-1.9.0/threedigrid_builder/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/boundary_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/connection_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/cross_section_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/dem_average_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19977 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/exchange_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:44.058993 threedigrid-builder-1.9.0/threedigrid_builder/grid/fgrid/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/fgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36443 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/grid_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/groundwater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/initial_waterlevels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16319 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21502 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/lines_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/obstacles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/potential_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/quadtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/windshielding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/grid/zero_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:44.058993 threedigrid-builder-1.9.0/threedigrid_builder/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31284 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/interface/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/interface/dict_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/interface/geopackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31328 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/interface/gridadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/interface/raster_gdal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:44.062993 threedigrid-builder-1.9.0/threedigrid_builder/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-03-06 14:48:40.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_boundary_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_connection_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_cross_section_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_dem_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_dict_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_exchange_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_grid_refinements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_gridadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_groundwater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_initial_waterlevels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_line_halfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_lines_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_linestrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_obstacles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_potential_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_pumps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_quadtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_raster_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_windshielding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-03-06 14:48:41.000000 threedigrid-builder-1.9.0/threedigrid_builder/tests/test_zero_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:48:44.054993 threedigrid-builder-1.9.0/threedigrid_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-06 14:48:44.000000 threedigrid-builder-1.9.0/threedigrid_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-03-06 14:48:44.000000 threedigrid-builder-1.9.0/threedigrid_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:48:44.000000 threedigrid-builder-1.9.0/threedigrid_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-06 14:48:44.000000 threedigrid-builder-1.9.0/threedigrid_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:48:44.000000 threedigrid-builder-1.9.0/threedigrid_builder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-06 14:48:44.000000 threedigrid-builder-1.9.0/threedigrid_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-06 14:48:44.000000 threedigrid-builder-1.9.0/threedigrid_builder.egg-info/top_level.txt
```

### Comparing `threedigrid-builder-1.8.0/CMakeLists.txt` & `threedigrid-builder-1.9.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/LICENSE` & `threedigrid-builder-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/README.rst` & `threedigrid-builder-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/libthreedigrid/_fgrid.pyf` & `threedigrid-builder-1.9.0/libthreedigrid/_fgrid.pyf`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/libthreedigrid/array_utils.f90` & `threedigrid-builder-1.9.0/libthreedigrid/array_utils.f90`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/libthreedigrid/cells.f90` & `threedigrid-builder-1.9.0/libthreedigrid/cells.f90`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/libthreedigrid/geo_utils.f90` & `threedigrid-builder-1.9.0/libthreedigrid/geo_utils.f90`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/libthreedigrid/parameters.f90` & `threedigrid-builder-1.9.0/libthreedigrid/parameters.f90`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/libthreedigrid/quadtree.f90` & `threedigrid-builder-1.9.0/libthreedigrid/quadtree.f90`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/pyproject.toml` & `threedigrid-builder-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/setup.py` & `threedigrid-builder-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,19 +48,19 @@
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 install_requires = [
     "numpy>=1.15",
-    "threedi-schema==0.214.*",
+    "threedi-schema>=0.214.5",
     "shapely>=2",
     "pyproj>=3",
     "condenser[geo]>=0.1.1",
-    "sqlalchemy>=1.3.12",
+    "sqlalchemy>=1.4.1",
 ]
 
 test_requires = ["pytest", "pytest-cov"]
 
 setup(
     name="threedigrid-builder",
     version=get_version(),
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/application.py` & `threedigrid-builder-1.9.0/threedigrid_builder/application.py`

 * *Files 11% similar despite different names*

```diff
@@ -188,14 +188,24 @@
             pipes=pipes,
             locations=locations,
             culverts=culverts,
             potential_breaches=potential_breaches,
             line_id_counter=line_id_counter,
         )
 
+        if grid.meta.has_groundwater:
+            channels.apply_has_groundwater_exchange(grid.nodes, grid.lines)
+            pipes.apply_has_groundwater_exchange(grid.nodes, grid.lines)
+            grid.add_1d2d_groundwater_lines(
+                line_id_counter,
+                connection_nodes=connection_nodes,
+                channels=channels,
+                pipes=pipes,
+            )
+
     if grid_settings.use_0d_inflow in (
         InflowType.IMPERVIOUS_SURFACE.value,
         InflowType.SURFACE.value,
     ):
         # process zero-d information, either using the 'v2_surfaces'
         # or 'v2_impervious_surfaces' table.
         progress_callback(0.95, "Processing 0D domain...")
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/base/array.py` & `threedigrid-builder-1.9.0/threedigrid_builder/base/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,19 +182,20 @@
 
         # convert each field to an array and set it to self
         fields = typing.get_type_hints(self.data_class)
         for name, elem_type in fields.items():
             if name == "id":
                 continue
             value = kwargs.pop(name, None)
-            try:
-                arr = _to_ndarray(value, elem_type, id.size)
-            except ValueError as e:
-                raise ValueError(f"Error parsing {name} to array: {e}")
-            setattr(self, name, arr)
+            if value is not None:
+                try:
+                    arr = _to_ndarray(value, elem_type, id.size)
+                except ValueError as e:
+                    raise ValueError(f"Error parsing {name} to array: {e}")
+                setattr(self, name, arr)
 
         # call the init of the wrapped class
         if len(kwargs) > 0:
             raise TypeError(
                 f"{self.__class__.__name__} got unexpected arguments {list(kwargs)}"
             )
         super().__init__(**kwargs)
@@ -252,14 +253,23 @@
 
         Returns:
             int or array_like: the ids from self.id
         """
         index = np.asarray(index)
         return self.take("id", index)
 
+    def __getattr__(self, name):
+        try:
+            elem_type = typing.get_type_hints(self.data_class)[name]
+        except KeyError:
+            raise AttributeError
+        arr = _to_ndarray(None, elem_type, len(self))
+        setattr(self, name, arr)
+        return arr
+
     def take(self, name, index, fill_value=None):
         """Take values from a column, returing 'fill_value' where index == -9999.
 
         Args:
             name (str): the column name to take values from
             index (int or array_like): The indices to return from self.id
             fill_value: what to return for -9999 indices (defaults to -9999/NaN/None)
@@ -276,15 +286,15 @@
         return np.where(index != -9999, np.take(values, index, mode="clip"), fill_value)
 
     def to_dict(self):
         fields = typing.get_type_hints(self.data_class)
         return {field: getattr(self, field) for field in fields}
 
     def __getitem__(self, idx) -> T:
-        """Create a masked copy of this arraay dataclass"""
+        """Create a masked copy of this array dataclass"""
         args = {}
         for field in typing.get_type_hints(self.data_class):
             args[field] = getattr(self, field)[idx]
         for scalar_arg in self.scalars:
             args[scalar_arg] = getattr(self, scalar_arg)
         return self.__class__(**args)
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/base/interfaces.py` & `threedigrid-builder-1.9.0/threedigrid_builder/base/interfaces.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/base/lines.py` & `threedigrid-builder-1.9.0/threedigrid_builder/base/lines.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     dpumax: float  # bottom_level at the velocity point
     invert_level_start_point: float  # bottom level at line start
     invert_level_end_point: float  # bottom level at line end
     flod: float  # obstacle height
     flou: float  # obstacle height
     cross_id1: int  # the id of the cross section definition
     cross_id2: int  # the id of the cross section definition
-    frict_type1: int  # Friction type
-    frict_type2: int  # Friction type
-    frict_value1: float  # Friction type
-    frict_value2: float  # Friction type
-    cross_weight: float
+    frict_type1: int
+    frict_type2: int
+    frict_value1: float  # For 1D-2Dgw: resistance factor-out (hydr. cond / thickness)
+    frict_value2: float  # For 1D-2Dgw: resistance factor-in (hydr. cond / thickness)
+    cross_weight: float  # For 1D-2Dgw: the exchange length (tables: cross_width)
     discharge_coefficient_positive: float
     discharge_coefficient_negative: float
     is_1d_boundary: int  # internal flag
     zoom_category: int
     connection_node_start_id: int
     connection_node_end_id: int
     crest_level: float
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/base/linestrings.py` & `threedigrid-builder-1.9.0/threedigrid_builder/base/linestrings.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/base/nodes.py` & `threedigrid-builder-1.9.0/threedigrid_builder/base/nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     initial_waterlevel: float
     zoom_category: int
     # extra info, for manhole only:
     manhole_indicator: int
     surface_level: float
     shape: str  # enum with classes "00", "01", "02"
     width: float
+    has_groundwater_exchange: bool  # internal
 
 
 class Nodes(Array[Node]):
     """Calculation node."""
 
     @property
     def has_1d(self):
@@ -68,14 +69,18 @@
             self.node_type, (NodeType.NODE_1D_NO_STORAGE, NodeType.NODE_1D_STORAGE)
         ).any()
 
     @property
     def has_2d(self):
         return np.any(self.node_type == NodeType.NODE_2D_OPEN_WATER)
 
+    @property
+    def n_groundwater_cells(self):
+        return np.count_nonzero(self.node_type == NodeType.NODE_2D_GROUNDWATER)
+
     def get_extent_1d(self):
         is_1d = np.isin(
             self.node_type, (NodeType.NODE_1D_NO_STORAGE, NodeType.NODE_1D_STORAGE)
         )
         if not is_1d.any():
             return
         x, y = self.coordinates[is_1d].T
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/base/pumps.py` & `threedigrid-builder-1.9.0/threedigrid_builder/base/pumps.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/base/settings.py` & `threedigrid-builder-1.9.0/threedigrid_builder/base/settings.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/base/surfaces.py` & `threedigrid-builder-1.9.0/threedigrid_builder/base/surfaces.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/cli.py` & `threedigrid-builder-1.9.0/threedigrid_builder/cli.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/constants.py` & `threedigrid-builder-1.9.0/threedigrid_builder/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,28 +37,31 @@
     LINE_1D_DOUBLE_CONNECTED = int(CalculationType.DOUBLE_CONNECTED)
     LINE_1D2D_SINGLE_CONNECTED_CLOSED = 51
     LINE_1D2D_SINGLE_CONNECTED_OPEN_WATER = 52
     LINE_1D2D_DOUBLE_CONNECTED_CLOSED = 53
     LINE_1D2D_DOUBLE_CONNECTED_OPEN_WATER = 54
     LINE_1D2D_POSSIBLE_BREACH = 55  # not used in gridbuilder
     LINE_1D2D_ACTIVE_BREACH = 56  # not used in gridbuilder
-    LINE_1D2D_GROUNDWATER_OPEN_WATER = 57
-    LINE_1D2D_GROUNDWATER_SEWER = 58  # diff to 57?
+    LINE_1D2D_GROUNDWATER = 57
     LINE_2D_U = 98  # for internal use
     LINE_2D_V = 99  # for internal use
     LINE_2D = 100
     LINE_2D_OBSTACLE = 101
     LINE_2D_OBSTACLE_U = 102
     LINE_2D_OBSTACLE_V = 103
     LINE_2D_VERTICAL = 150
     LINE_2D_GROUNDWATER = -150
     LINE_2D_BOUNDARY_WEST = 200
     LINE_2D_BOUNDARY_EAST = 300
     LINE_2D_BOUNDARY_SOUTH = 400
     LINE_2D_BOUNDARY_NORTH = 500
+    LINE_2D_GROUNDWATER_BOUNDARY_WEST = 600
+    LINE_2D_GROUNDWATER_BOUNDARY_EAST = 700
+    LINE_2D_GROUNDWATER_BOUNDARY_SOUTH = 800
+    LINE_2D_GROUNDWATER_BOUNDARY_NORTH = 900
 
 
 @unique
 class ContentType(IntEnum):
     TYPE_V2_PIPE = 1
     TYPE_V2_CHANNEL = 2
     TYPE_V2_CULVERT = 3
@@ -109,14 +112,16 @@
 @unique
 class BoundaryType(IntEnum):
     WATERLEVEL = 1
     VELOCITY = 2
     DISCHARGE = 3
     RIEMANN = 4
     SOMMERFELD = 5
+    GROUNDWATERLEVEL = 6
+    GROUNDWATERDISCHARGE = 7
 
 
 @unique
 class InfiltrationSurfaceOption(IntEnum):
     RAIN = 0
     WHOLE_SURFACE = 1
     WET_SURFACE = 2
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/__init__.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .cross_section_definitions import *  # NOQA
 from .cross_section_locations import *  # NOQA
 from .dem_average_area import *  # NOQA
 from .embedded import *  # NOQA
 from .exchange_lines import *  # NOQA
 from .grid import *  # NOQA
 from .grid_refinement import *  # NOQA
+from .lines_1d2d import *  # NOQA
 from .obstacles import *  # NOQA
 from .pipes import *  # NOQA
 from .potential_breaches import *  # NOQA
 from .quadtree import *  # NOQA
 from .structures import *  # NOQA
 from .windshielding import *  # NOQA
 from .zero_d import *  # NOQA
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/channels.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/pipes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,72 @@
+import numpy as np
 import shapely
 
 from threedigrid_builder.base import Array
-from threedigrid_builder.constants import CalculationType, ContentType
+from threedigrid_builder.constants import CalculationType, ContentType, FrictionType
 from threedigrid_builder.grid import linear
-from threedigrid_builder.grid.cross_section_locations import compute_bottom_level
 
-__all__ = ["Channels"]
+__all__ = ["Pipes"]
 
 
-class Channel:
+class Pipe:
     id: int
     code: str
-    the_geom: shapely.Geometry
     dist_calc_points: float
+    calculation_type: CalculationType
     connection_node_start_id: int
     connection_node_end_id: int
-    calculation_type: CalculationType
-    display_name: str
+    cross_section_definition_id: int
+    invert_level_start_point: float
+    invert_level_end_point: float
+    sewerage_type: int
+    friction_type: FrictionType
+    friction_value: float
+    the_geom: shapely.Geometry
     zoom_category: int
+    display_name: str
+    # profile_num
+    # original_length
+    material: int
+    exchange_thickness: float
+    hydraulic_conductivity_out: float
+    hydraulic_conductivity_in: float
+
+
+class Pipes(Array[Pipe], linear.BaseLinear):
+    content_type = ContentType.TYPE_V2_PIPE
 
+    def is_closed(self, content_pk):
+        """Whether objects are 'closed' or 'open water'.
+
+        This is relevant for 1D-2D connections.
+        """
+        return np.full(len(content_pk), True, dtype=bool)
 
-class Channels(Array[Channel], linear.BaseLinear):
-    content_type = ContentType.TYPE_V2_CHANNEL
+    def get_1d2d_exchange_levels(self, content_pk, s1d, connection_nodes, **kwargs):
+        """Compute the exchange level (dpumax) for 1D-2D flowlines.
 
-    def get_1d2d_properties(self, nodes, node_idx, locations, **kwargs):
-        """Compute properties (is_closed, dpumax) of 1D-2D channel flowlines.
+        For pipes and culverts 1D2D exchange levels are interpololated between
+        connection node drain levels.
 
         Args:
-            nodes (Nodes): All nodes
-            node_idx (array of int): indices into nodes for which to compute properties
-            locations (CrossSectionLocations): for the bank_levels
+            content_pk (array of int): object ids for which to compute levels
+            s1d (array of int): distance on the objects where to compute levels
+            connection_nodes (ConnectionNodes): for the drain_levels
 
         Returns:
-            tuple of:
-            - is_closed (bool): always False
-            - dpumax (array of float): interpolated between CS location bank_levels
+            exchange levels a.k.a. dpumax (array of float)
         """
-        # dpumax is interpolated between cross section location bank levels
-        dpumax = compute_bottom_level(
-            nodes.content_pk[node_idx],
-            nodes.s1d[node_idx],
-            locations,
-            self,
-            "bank_level",
+        return self.compute_drain_level(
+            ids=content_pk,
+            s=s1d,
+            connection_nodes=connection_nodes,
         )
 
-        return False, dpumax
+    @property
+    def has_groundwater_exchange(self):
+        with np.errstate(invalid="ignore"):
+            return (
+                (self.exchange_thickness > 0)
+                & np.isfinite(self.hydraulic_conductivity_out)
+                & np.isfinite(self.hydraulic_conductivity_in)
+            )
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/connection_nodes.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/connection_nodes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 import logging
 
 import numpy as np
 import shapely
 
-from threedigrid_builder.base import Array, Endpoints, Lines, Nodes, replace
+from threedigrid_builder.base import Array, LineHalfs, Lines, Nodes, replace
 from threedigrid_builder.constants import (
     CalculationType,
     ContentType,
     LineType,
     NodeType,
 )
 
@@ -31,14 +31,17 @@
     drain_level: float
     surface_level: float
     shape: str  # enum with classes "00", "01", "02"
     width: float
     initial_waterlevel: float
     display_name: str
     zoom_category: int
+    exchange_thickness: float
+    hydraulic_conductivity_out: float
+    hydraulic_conductivity_in: float
 
 
 class ConnectionNodes(Array[ConnectionNode]):
     content_type = ContentType.TYPE_V2_CONNECTION_NODES
 
     def get_nodes(self, node_id_counter):
         """Convert connection nodes to a nodes instance
@@ -62,48 +65,53 @@
         """
         node_type = np.where(
             self.storage_area >= 0,
             int(NodeType.NODE_1D_STORAGE),
             int(NodeType.NODE_1D_NO_STORAGE),
         )
 
-        nodes = Nodes(
+        return Nodes(
             id=itertools.islice(node_id_counter, len(self)),
             coordinates=shapely.get_coordinates(self.the_geom),
             content_type=ContentType.TYPE_V2_CONNECTION_NODES,
             content_pk=self.id,
             node_type=node_type,
             calculation_type=self.calculation_type,
             dmax=self.bottom_level,
             manhole_id=self.manhole_id,
             drain_level=self.drain_level,
             storage_area=self.storage_area,
             display_name=self.display_name,
             zoom_category=self.zoom_category,
+            has_groundwater_exchange=self.has_groundwater_exchange,
         )
-        return nodes
 
-    def get_1d2d_properties(self, nodes, node_idx, channels, locations, **kwargs):
-        """Compute properties (is_closed, dpumax) of 1D-2D connection node flowlines.
+    def is_closed(self, content_pk):
+        """Whether object are 'closed' or 'open water' object.
+
+        This is relevant for 1D-2D connections.
+        """
+        return self.storage_area[self.id_to_index(content_pk)] >= 0
+
+    def get_1d2d_exchange_levels(self, content_pk, channels, locations, **kwargs):
+        """Compute the exchange level (dpumax) for 1D-2D flowlines.
+
+        For connection nodes 1D2D exchange levels are the drain levels. Where
+        there is no drain level, the bank levels are taken from connected channels.
 
         Args:
-            nodes (Nodes): All nodes
-            node_idx (array of int): indices into nodes for which to compute properties
-            channels (Channels): required for nodes without drain_level
-            locations (CrossSectionLocations): to take drain_level from for nodes
-                without drain_level but with channel(s)
+            content_pk (array of int): object ids for which to compute levels
+            channels (Channels): for the drain_levels
+            locations (CrossSectionLocations): for the bank_levels
 
         Returns:
-            tuple of:
-            - is_closed (array of bool): based on self.storage_area
-            - dpumax (array of float): based on self.drain_level or locations.bank_level
+            exchange levels a.k.a. dpumax (array of float)
         """
         # get the corresponding connection_node ids and indexes
-        connection_node_id = nodes.content_pk[node_idx]
-        connection_node_idx = self.id_to_index(connection_node_id)
+        connection_node_idx = self.id_to_index(content_pk)
         is_manhole = self.manhole_id[connection_node_idx] != -9999
         is_manhole_idx = connection_node_idx[is_manhole]
 
         # Check if manhole has drain_level below bottom_level
         has_lower_drn_lvl = (
             self.drain_level[is_manhole_idx] < self.bottom_level[is_manhole_idx]
         )
@@ -111,18 +119,18 @@
             ids = self.manhole_id[is_manhole_idx[has_lower_drn_lvl]]
             logger.warning(
                 f"Manholes {sorted(ids.tolist())} have a "
                 f"bottom_level that is above drain_level."
             )
 
         # for open water nodes, compute drain level from channel bank levels
-        open_water = node_idx[~is_manhole]
+        open_water = ~is_manhole
         dpumax = np.full(len(self), np.nan)  # easier to initialize for all conn. nodes
         for name in ("connection_node_start_id", "connection_node_end_id"):
-            has_node = np.isin(getattr(channels, name), nodes.content_pk[open_water])
+            has_node = np.isin(getattr(channels, name), content_pk[open_water])
             cn_idx_with_channel = self.id_to_index(getattr(channels, name)[has_node])
             if name == "connection_node_start_id":
                 ds = 0.0
             else:
                 ds = shapely.length(channels.the_geom[has_node])
             drain_level = compute_bottom_level(
                 channels.id[has_node],
@@ -133,17 +141,25 @@
             )
             _put_if_less(dpumax, cn_idx_with_channel, drain_level)
         # filter out connection nodes that were not in node_idx (non-connected ones)
         dpumax = dpumax[connection_node_idx]
 
         # for manholes: put in the drain level
         dpumax[is_manhole] = self.drain_level[is_manhole_idx]
+        return dpumax
 
-        is_closed = self.storage_area[connection_node_idx] >= 0
-        return is_closed, dpumax
+    @property
+    def has_groundwater_exchange(self):
+        with np.errstate(invalid="ignore"):
+            return (
+                (self.storage_area > 0)
+                & (self.exchange_thickness > 0)
+                & np.isfinite(self.hydraulic_conductivity_out)
+                & np.isfinite(self.hydraulic_conductivity_in)
+            )
 
 
 def set_calculation_types(nodes: Nodes, lines: Lines):
     """Set the calculation types for connection nodes that do not yet have one.
 
     The calculation_type of a connection nodes is based on
       - connection_node.manhole.calculation_type (set in ConnectionNode.get_nodes)
@@ -163,38 +179,40 @@
         LineType.LINE_1D_DOUBLE_CONNECTED: 2,
         LineType.LINE_1D_CONNECTED: 3,
     }
 
     node_mask = (nodes.content_type == ContentType.TYPE_V2_CONNECTION_NODES) & (
         nodes.calculation_type == -9999
     )
-    endpoints = Endpoints.for_connection_nodes(
+    line_halfs = LineHalfs.for_connection_nodes(
         nodes,
         lines,
         line_mask=np.isin(
             lines.content_type,
             [
                 ContentType.TYPE_V2_CHANNEL,
                 ContentType.TYPE_V2_PIPE,
                 ContentType.TYPE_V2_CULVERT,
             ],
         )
         & (lines.kcu != -9999),
         node_mask=node_mask,
     )
-    endpoints.reorder(np.lexsort([replace(endpoints.kcu, PRIORITY), endpoints.node_id]))
+    line_halfs.reorder(
+        np.lexsort([replace(line_halfs.kcu, PRIORITY), line_halfs.node_id])
+    )
 
-    calculation_type = endpoints.first_per_node(endpoints.kcu)
+    calculation_type = line_halfs.first(line_halfs.kcu)
 
     # start off with ISOLATED
     nodes.calculation_type[node_mask] = CalculationType.ISOLATED
-    # overwrite with the one derived from the line endpoints
+    # overwrite with the one derived from the line line_halfs
     nodes.calculation_type[
-        nodes.id_to_index(calculation_type.id)
-    ] = calculation_type.value
+        nodes.id_to_index(line_halfs.get_reduce_id())
+    ] = calculation_type
 
 
 def _put_if_less(a, ind, v):
     """Replaces specified elements of an array with given values if  they are less."""
     # values can occur multiple times for the same index. sort descending by value so
     # that the lowest (latest) one will take precedence
     sorter = np.argsort(-v)
@@ -225,34 +243,34 @@
 
     Args:
         nodes (Nodes): the nodes, those with content_type == TYPE_V2_CONNECTION_NODES
           and without a dmax will get a new dmax
         lines (Lines): the lines, including channels, pipes, weirs, and culverts
     """
     # Compute the lowest invert level for each node connection node dmax will be the lowest of these object types:
-    endpoints = Endpoints.for_connection_nodes(
+    line_halfs = LineHalfs.for_connection_nodes(
         nodes,
         lines,
         line_mask=np.isin(
             lines.content_type,
             [
                 ContentType.TYPE_V2_CHANNEL,
                 ContentType.TYPE_V2_PIPE,
                 ContentType.TYPE_V2_CULVERT,
                 ContentType.TYPE_V2_WEIR,
                 ContentType.TYPE_V2_ORIFICE,
             ],
         ),
     )
-    endpoints.reorder_by("node_id")
-    dmax_per_node = endpoints.nanmin_per_node(endpoints.invert_level)
-    node_idx = nodes.id_to_index(dmax_per_node.id)
+    line_halfs.reorder_by("node_id")
+    dmax_per_node = line_halfs.nanmin(line_halfs.invert_level)
+    node_idx = nodes.id_to_index(line_halfs.get_reduce_id())
 
     # The new dmax is the minimum of the existing one and the one from above computation
-    dmax = np.fmin(nodes.dmax[node_idx], dmax_per_node.value)
+    dmax = np.fmin(nodes.dmax[node_idx], dmax_per_node)
 
     # Check if the new node dmax is below the original manhole dmax
     is_manhole = nodes.manhole_id[node_idx] != -9999
     has_lower_dmax = dmax[is_manhole] < nodes.dmax[node_idx[is_manhole]]
     if np.any(has_lower_dmax):
         ids = nodes.manhole_id[node_idx[is_manhole][has_lower_dmax]]
         logger.warning(
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/cross_section_definitions.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/cross_section_locations.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/cross_section_locations.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/dem_average_area.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/dem_average_area.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/embedded.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/embedded.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,24 +359,24 @@
             mult_ch_idx != np.roll(mult_ch_idx, 1)
         )
         is_first[0] = True
         is_last = np.roll(is_first, -1)
 
         # Iterate over consecutive ranges (and keep a global mask of vpoints to keep)
         vpoints_to_keep = np.ones(n_vpoints, dtype=bool)
-        for (_first, _last) in zip(mult_vpoint_idx[is_first], mult_vpoint_idx[is_last]):
+        for _first, _last in zip(mult_vpoint_idx[is_first], mult_vpoint_idx[is_last]):
             vpoints_to_keep[_first : _last + 1] = False
 
             # Construct the graph (e.g. {"c2": ["v1", "v2"], "v2": ["c1"], ...}
             graph = defaultdict(list)
             mask_a = np.where((vpoint_idx_a >= _first) & (vpoint_idx_a <= _last))[0]
-            for (vpoint_idx, cell_idx) in zip(vpoint_idx_a[mask_a], cell_idx_a[mask_a]):
+            for vpoint_idx, cell_idx in zip(vpoint_idx_a[mask_a], cell_idx_a[mask_a]):
                 graph[f"c{cell_idx}"].append(f"v{vpoint_idx}")
             mask_b = np.where((vpoint_idx_b >= _first) & (vpoint_idx_b <= _last))[0]
-            for (vpoint_idx, cell_idx) in zip(vpoint_idx_b[mask_b], cell_idx_b[mask_b]):
+            for vpoint_idx, cell_idx in zip(vpoint_idx_b[mask_b], cell_idx_b[mask_b]):
                 graph[f"v{vpoint_idx}"].append(f"c{cell_idx}")
 
             # Get the shortest path (e.g. ['c2', 'v2', 'c1'])
             # Note: There could be multiple cell options to start/end with, loop over
             # combinations and take the shortest outcome.
             path = None
             for a, b in itertools.product(
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/exchange_lines.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/lines_1d2d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,29 @@
 import itertools
+import logging
 from typing import Iterator
 
 import numpy as np
 import shapely
 
-from threedigrid_builder.base import Array, Endpoints, Lines, Nodes, replace, search
+from threedigrid_builder.base import LineHalfs, Lines, Nodes, replace, search
 from threedigrid_builder.constants import CalculationType, ContentType, LineType
+from threedigrid_builder.exceptions import SchematisationError
 
+from .channels import Channels
+from .connection_nodes import ConnectionNodes
+from .exchange_lines import ExchangeLines
+from .linear import BaseLinear
 from .obstacles import Obstacles
+from .pipes import Pipes
 from .potential_breaches import PotentialBreaches
 
-__all__ = ["ExchangeLines", "Lines1D2D"]
+logger = logging.getLogger(__name__)
 
-
-class ExchangeLine:
-    id: int
-    the_geom: shapely.Geometry
-    channel_id: int
-    exchange_level: float
-
-
-class ExchangeLines(Array[ExchangeLine]):
-    @property
-    def channel_mapping(self) -> "ExchangeLineChannels":
-        """Return 2 exchange lines ids for each channel id"""
-        if not hasattr(self, "_channel_mapping"):
-            channel_ids = np.unique(self.channel_id)
-            result = np.full((len(channel_ids), 2), fill_value=-9999, dtype=np.int32)
-            for i, mask in enumerate(self.split_in_two(self.channel_id)):
-                result[:, i] = self.index_to_id(
-                    search(
-                        self.channel_id,
-                        channel_ids,
-                        mask=mask,
-                        assume_ordered=False,
-                        check_exists=False,
-                    )
-                )
-            self._channel_mapping = ExchangeLineChannels(
-                id=channel_ids,
-                exchange_line_id=result[:, 0],
-                secondary_exchange_line_id=result[:, 1],
-            )
-        return self._channel_mapping
-
-    def get_for_channel_id(self, channel_id, is_primary):
-        if len(self) == 0:
-            return np.full_like(channel_id, fill_value=-9999)
-        index = self.channel_mapping.id_to_index(channel_id)
-        if is_primary:
-            ids = self.channel_mapping.exchange_line_id
-        else:
-            ids = self.channel_mapping.secondary_exchange_line_id
-        return np.where(index != -9999, np.take(ids, index, mode="clip"), -9999)
-
-
-class ExchangeLineChannel:
-    id: int
-    exchange_line_id: int
-    secondary_exchange_line_id: int
-
-
-class ExchangeLineChannels(Array[ExchangeLineChannel]):
-    pass
+__all__ = ["Lines1D2D"]
 
 
 class Lines1D2D(Lines):
     @classmethod
     def create(cls, nodes: Nodes, line_id_counter: Iterator[int]) -> "Lines1D2D":
         """Create the 1D-2D lines
 
@@ -78,15 +35,15 @@
             [np.where(is_single | is_double)[0], np.where(is_double)[0]]
         )
         node_idx.sort()
 
         # Merge the arrays
         line = np.full((len(node_idx), 2), -9999, dtype=np.int32)
         line[:, 1] = nodes.index_to_id(node_idx)
-        return Lines1D2D(
+        return cls(
             id=itertools.islice(line_id_counter, len(node_idx)),
             line=line,
             content_type=nodes.content_type[node_idx],
             content_pk=nodes.content_pk[node_idx],
         )
 
     @property
@@ -135,41 +92,44 @@
         PRIORITY = {LineType.LINE_1D_DOUBLE_CONNECTED: 0, LineType.LINE_1D_CONNECTED: 1}
 
         is_connection_node = np.where(
             self.content_type == ContentType.TYPE_V2_CONNECTION_NODES
         )[0]
         node_ids = self.line[is_connection_node, 1]
 
-        endpoints = Endpoints.for_connection_nodes(
+        line_halfs = LineHalfs.for_connection_nodes(
             nodes,
             lines,
             line_mask=(
                 (lines.content_type == ContentType.TYPE_V2_CHANNEL)
                 & (np.isin(lines.kcu, list(PRIORITY.keys())))
             ),
             node_mask=np.isin(nodes.id, node_ids),
         )
-        # Order the endpoints by (channel_id, calc type) and pick the first
-        endpoints.reorder(
+        # Order the line_halfs by (channel_id, calc type) and pick the first
+        line_halfs.reorder(
             np.lexsort(
                 [
-                    endpoints.content_pk,
-                    replace(endpoints.kcu, PRIORITY),
-                    endpoints.node_id,
+                    line_halfs.content_pk,
+                    replace(line_halfs.kcu, PRIORITY),
+                    line_halfs.node_id,
                 ]
             )
         )
-        channel_id_per_node = endpoints.first_per_node(endpoints.content_pk)
+        channel_id_per_node = line_halfs.first(line_halfs.content_pk)
         # Use the node_id -> channel_id map to set channel_id on self
         idx = search(
-            channel_id_per_node.id, node_ids, check_exists=False, assume_ordered=True
+            line_halfs.get_reduce_id(),
+            node_ids,
+            check_exists=False,
+            assume_ordered=True,
         )
         mask = idx != -9999
 
-        self.content_pk[is_connection_node[mask]] = channel_id_per_node.value[idx[mask]]
+        self.content_pk[is_connection_node[mask]] = channel_id_per_node[idx[mask]]
         self.content_type[is_connection_node[mask]] = ContentType.TYPE_V2_CHANNEL
 
     def assign_exchange_lines(self, exchange_lines: ExchangeLines) -> None:
         """Assign exchange lines to the 1D-2D lines.
 
         Resets all content_type / content_pk.
 
@@ -200,42 +160,43 @@
             content_pk != -9999, ContentType.TYPE_V2_EXCHANGE_LINE, -9999
         )
 
     def get_1d_node_idx(self, nodes: Nodes):
         """Get the 1D node index based on line[:, 1]"""
         return nodes.id_to_index(self.line[:, 1])
 
-    def assign_2d_side(self, nodes: Nodes, exchange_lines: ExchangeLines):
-        """Compute a Point on the (user-requested) 2D side for each line
-
-        If there is no exchange line this is the 1D node location. If there is
-        an exchange line, it is the closest point on the exchange line.
+    def assign_line_coords(self, nodes: Nodes):
+        """Copy the 1D node location to the 2D side for non-exchange line lines.
 
         Returns an array of shapely Point geometries
         Requires: line[:, 1], content_pk, content_type
-        Sets: line_coords[:, :2] (the 2D side), line_geometries
+        Sets: line_coords (side_1d and side_2d)
+        """
+        self.line_coords[:, 2:] = nodes.coordinates[self.get_1d_node_idx(nodes)]
+        self.line_coords[:, :2] = self.line_coords[:, 2:]
+
+    def assign_2d_side_from_exchange_lines(self, exchange_lines: ExchangeLines):
+        """Compute the closest Point on exchange line for each 1D2D line
+
+        Requires: line_coords[:, 2:] (side_1d), content_pk, content_type
+        Sets: line_coords[:, :2] (side_2d)
         """
         # Create an array of node indices & corresponding exchange line indices
         has_exc = self.content_type == ContentType.TYPE_V2_EXCHANGE_LINE
 
-        # Collect the 1D sides of the 1D2D line
-        coords_1d = nodes.coordinates[self.get_1d_node_idx(nodes)]
-
         # Find the closest points on the exchange lines
         exc_geoms = exchange_lines.the_geom[
             exchange_lines.id_to_index(self.content_pk[has_exc])
         ]
         shapely.prepare(exc_geoms)
-        line_geom = shapely.shortest_line(exc_geoms, shapely.points(coords_1d[has_exc]))
+        line_geom = shapely.shortest_line(exc_geoms, self.side_1d[has_exc])
 
-        self.line_coords[~has_exc, :2] = coords_1d[~has_exc]
         self.line_coords[has_exc, :2] = shapely.get_coordinates(
             shapely.get_point(line_geom, 0)
         )
-        self.line_geometries[has_exc] = line_geom
 
     def assign_breaches(self, nodes: Nodes, potential_breaches: PotentialBreaches):
         """Assign breaches to the 1D-2D lines.
 
         It is assumed that the breach ids match the calculation type of the nodes.
         This is done in PotentialBreachPoints.match_breach_ids_with_calculation_types.
 
@@ -306,24 +267,50 @@
         self.content_type[line_idx] = ContentType.TYPE_V2_BREACH
         self.content_pk[line_idx] = potential_breaches.id[breach_idx]
 
     def assign_2d_node(self, cell_tree: shapely.STRtree) -> None:
         """Assigns the 2D node id based on the line_coords
 
         Requires: line_coords[:, :2] (the 2D side)
-        Sets: line[:, 0], line_coords[:, :2] (clears)
+        Sets: line[:, 0], line_coords[:] (clears)
         """
         # The query returns 2 1D arrays: one with indices into the supplied node
         # geometries and one with indices into the tree of cells.
         idx = cell_tree.query(self.side_2d)
         # Address edge cases of multiple 1D-2D lines per node: just take the one
         _, unique_matches = np.unique(idx[0], return_index=True)
         line_idx, cell_idx = idx[:, unique_matches]
         self.line[line_idx, 0] = cell_idx
-        self.line_coords[:, :2] = np.nan
+        self.line_coords[:] = np.nan
+
+    def check_unassigned(self, nodes) -> None:
+        """Checks 1D-2D lines where any of the required nodes is set to null, represented as -9999
+        This is the case when the nodes are outside the 2D domain.
+        """
+        invalid_rows = self.line[:, 0] == -9999
+        if invalid_rows.any():
+            invalid_node_ids = self.line[invalid_rows, 1]
+            invalid_nodes = nodes.id_to_index(invalid_node_ids)
+            invalid_nodes_formatted = nodes.format_message(invalid_nodes)
+
+            raise SchematisationError(
+                f"The following objects are connected but are (partially) outside of the 2D model domain: {invalid_nodes_formatted}."
+            )
+
+    def transfer_2d_node_to_groundwater(self, offset: int):
+        """Transfers the 1D-2D line to a groundwater node
+
+        Sets: line[:, 0]
+        """
+        has_2d_node = np.where(self.line[:, 0] != -9999)[0]
+        if offset == 0:
+            # no groundwater cells; reset the node id (will raise error later)
+            self.line[has_2d_node, 0] = -9999
+        else:
+            self.line[has_2d_node, 0] += offset
 
     def assign_kcu(self, mask, is_closed) -> None:
         """Set kcu where it is not set already"""
         node_id = self.line[mask, 1]
         node_id_unique, counts = np.unique(node_id, return_counts=True)
         line_is_double = np.isin(self.line[mask, 1], node_id_unique[counts == 2])
         self.kcu[mask] = np.choose(
@@ -355,30 +342,31 @@
                 exchange_lines.id_to_index(self.content_pk[has_exc])
             ],
         )
 
     def assign_dpumax_from_obstacles(self, obstacles: Obstacles):
         """Set the dpumax based on intersected obstacles
 
-        Only for (open) connections that are computed via an exchange line or breach.
-
-        Requires line_geometries.
+        Only for open connections. Requires line_geometries.
         """
-        is_displaced = np.isin(
-            self.content_type,
-            [ContentType.TYPE_V2_EXCHANGE_LINE, ContentType.TYPE_V2_BREACH],
+        is_open_water = np.isin(
+            self.kcu,
+            [
+                LineType.LINE_1D2D_SINGLE_CONNECTED_OPEN_WATER,
+                LineType.LINE_1D2D_DOUBLE_CONNECTED_OPEN_WATER,
+            ],
         )
-        is_displaced_idx = np.where(is_displaced)[0]
+        is_open_water_idx = np.where(is_open_water)[0]
         obstacle_crest_levels, obstacle_idx = obstacles.compute_dpumax(
-            self, where=is_displaced_idx
+            self, where=is_open_water_idx
         )
-        self.assign_dpumax(is_displaced, obstacle_crest_levels)
+        self.assign_dpumax(is_open_water, obstacle_crest_levels)
         mask = obstacle_idx != -9999
         self.assign_ds1d_half_from_obstacles(
-            obstacles, is_displaced_idx[mask], obstacle_idx[mask]
+            obstacles, is_open_water_idx[mask], obstacle_idx[mask]
         )
 
     def assign_ds1d_half_from_obstacles(
         self, obstacles: Obstacles, line_idx, obstacle_idx
     ):
         if len(line_idx) == 0:
             return
@@ -444,7 +432,107 @@
             content_pk=breaches.id[breach_idx],
             maximum_breach_depth=breaches.maximum_breach_depth[breach_idx],
             levee_material=breaches.levee_material[breach_idx],
             the_geom=self.get_velocity_points(line_idx),
             code=breaches.code[breach_idx],
             display_name=breaches.display_name[breach_idx],
         )
+
+    @classmethod
+    def create_groundwater(
+        cls, nodes: Nodes, line_id_counter: Iterator[int]
+    ) -> "Lines1D2D":
+        """Create a 1D-2D groundwater lines for each 1D node.
+
+        Sets: id, line[:, 1], kcu
+        """
+        node_idx = np.where(nodes.has_groundwater_exchange)[0]
+        line = np.full((len(node_idx), 2), -9999, dtype=np.int32)
+        line[:, 1] = nodes.index_to_id(node_idx)
+        return cls(
+            id=itertools.islice(line_id_counter, len(node_idx)),
+            line=line,
+            kcu=LineType.LINE_1D2D_GROUNDWATER,
+        )
+
+    def _assign_groundwater_exchange_from_connection_nodes(
+        self, nodes: Nodes, cn: ConnectionNodes
+    ):
+        node_idx = self.get_1d_node_idx(nodes)
+        idx = np.where(
+            nodes.content_type[node_idx] == ContentType.TYPE_V2_CONNECTION_NODES
+        )[0]
+        cn_idx = cn.id_to_index(nodes.content_pk[node_idx[idx]])
+        mask = cn.has_groundwater_exchange[cn_idx]
+        idx = idx[mask]
+        cn_idx = cn_idx[mask]
+
+        length = np.sqrt(cn.storage_area[cn_idx])
+        factor = length / cn.exchange_thickness[cn_idx]
+
+        self.cross_weight[idx] += length
+        self.frict_value1[idx] += factor * cn.hydraulic_conductivity_out[cn_idx]
+        self.frict_value2[idx] += factor * cn.hydraulic_conductivity_in[cn_idx]
+
+    def _assign_groundwater_exchange_from_linear_objects(
+        self, nodes: Nodes, lines_1d: Lines, objs: BaseLinear
+    ):
+        line_has_gw = (lines_1d.content_type == objs.content_type) & np.isin(
+            lines_1d.content_pk, objs.id[objs.has_groundwater_exchange]
+        )
+        line_halfs = LineHalfs.from_nodes_lines(
+            nodes,
+            lines_1d,
+            line_mask=line_has_gw,
+        )
+        line_halfs.reorder_by("node_id")
+        idx = search(
+            self.line[:, 1],
+            line_halfs.get_reduce_id(),
+            check_exists=True,
+            assume_ordered=False,
+        )
+        objs_idx = objs.id_to_index(line_halfs.content_pk)
+
+        factor = line_halfs.ds1d / objs.exchange_thickness[objs_idx]
+
+        self.cross_weight[idx] += line_halfs.sum(line_halfs.ds1d)
+        self.frict_value1[idx] += line_halfs.sum(
+            factor * objs.hydraulic_conductivity_out[objs_idx]
+        )
+        self.frict_value2[idx] += line_halfs.sum(
+            factor * objs.hydraulic_conductivity_in[objs_idx]
+        )
+
+    def assign_groundwater_exchange(
+        self,
+        nodes: Nodes,
+        lines: Lines,
+        connection_nodes: ConnectionNodes,
+        channels: Channels,
+        pipes: Pipes,
+    ):
+        """Compute the friction values for groundwater exchange
+
+        Sets:
+        - cross_weight (length of objects and sqrt of manhole area)
+        - frict_value1 (average from hydr. cond. out, thickness and length)
+        - frict_value2 (average from hydr. cond. in, thickness and length)
+        - dpumax (from 1D nodes dmax)
+        """
+        self.cross_weight[:] = 0.0
+        self.frict_value1[:] = 0.0
+        self.frict_value2[:] = 0.0
+
+        self._assign_groundwater_exchange_from_connection_nodes(nodes, connection_nodes)
+        self._assign_groundwater_exchange_from_linear_objects(nodes, lines, channels)
+        self._assign_groundwater_exchange_from_linear_objects(nodes, lines, pipes)
+
+        # change 'weighted sum' to 'weighted average' (avoiding div by 0)
+        has_weight = self.cross_weight > 0.0
+        self.frict_value1[has_weight] /= self.cross_weight[has_weight]
+        self.frict_value1[~has_weight] = np.nan
+
+        self.frict_value2[has_weight] /= self.cross_weight[has_weight]
+        self.frict_value2[~has_weight] = np.nan
+
+        self.dpumax = nodes[self.get_1d_node_idx(nodes)].dmax
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/grid.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 from . import connection_nodes as connection_nodes_module
 from . import dem_average_area as dem_average_area_module
 from . import embedded as embedded_module
 from . import groundwater as groundwater_module
 from . import initial_waterlevels as initial_waterlevels_module
 from .cross_section_definitions import CrossSections
-from .exchange_lines import Lines1D2D
 from .linear import BaseLinear
+from .lines_1d2d import Lines1D2D
 from .obstacles import Obstacles
 from .potential_breaches import PotentialBreaches, PotentialBreachPoints
 
 osr.UseExceptions()
 
 
 __all__ = ["Grid", "GridMeta", "QuadtreeStats"]
@@ -67,15 +67,17 @@
     ],
     [
         LineType.LINE_1D2D_SINGLE_CONNECTED_CLOSED,
         LineType.LINE_1D2D_SINGLE_CONNECTED_OPEN_WATER,
         LineType.LINE_1D2D_DOUBLE_CONNECTED_CLOSED,
         LineType.LINE_1D2D_DOUBLE_CONNECTED_OPEN_WATER,
     ],
-    [LineType.LINE_1D2D_GROUNDWATER_OPEN_WATER, LineType.LINE_1D2D_GROUNDWATER_SEWER],
+    [
+        LineType.LINE_1D2D_GROUNDWATER,
+    ],
     [
         LineType.LINE_2D_BOUNDARY_WEST,
         LineType.LINE_2D_BOUNDARY_EAST,
         LineType.LINE_2D_BOUNDARY_SOUTH,
         LineType.LINE_2D_BOUNDARY_NORTH,
     ],
     # [LineType.LINE_2D_GROUNDWATER_BOUNDARY], (to be implemented)
@@ -679,49 +681,86 @@
 
         In addition to id and line attributes, also the kcu (line type) and dpumax
         (bottom level) are computed.
 
         Sets self.breaches and appends self.lines.
         """
         lines_1d2d = Lines1D2D.create(self.nodes, line_id_counter)
+        if len(lines_1d2d) == 0:
+            return
+        lines_1d2d.assign_line_coords(self.nodes)
         lines_1d2d.assign_connection_nodes_to_channels_from_breaches(
             self.nodes, potential_breaches=potential_breaches
         )
         lines_1d2d.assign_connection_nodes_to_channels_from_lines(
             self.nodes, lines=self.lines
         )
         lines_1d2d.assign_exchange_lines(exchange_lines)
-        lines_1d2d.assign_2d_side(self.nodes, exchange_lines)
+        lines_1d2d.assign_2d_side_from_exchange_lines(exchange_lines)
         lines_1d2d.assign_breaches(self.nodes, potential_breaches)
         lines_1d2d.assign_2d_node(self.cell_tree)
+        lines_1d2d.check_unassigned(self.nodes)
         lines_1d2d.set_line_coords(self.nodes)
         lines_1d2d.fix_line_geometries()
+        # Go through objects and dispatch to get_1d2d_properties
+        node_idx = lines_1d2d.get_1d_node_idx(self.nodes)
+        for objects in (channels, connection_nodes, pipes, culverts):
+            mask = self.nodes.content_type[node_idx] == objects.content_type
+            content_pk = self.nodes.content_pk[node_idx[mask]]
+            lines_1d2d.assign_kcu(mask, objects.is_closed(content_pk))
         lines_1d2d.assign_dpumax_from_breaches(potential_breaches)
         lines_1d2d.assign_dpumax_from_exchange_lines(exchange_lines)
         lines_1d2d.assign_dpumax_from_obstacles(self.obstacles)
         # Go through objects and dispatch to get_1d2d_properties
-        node_idx = lines_1d2d.get_1d_node_idx(self.nodes)
         for objects in (channels, connection_nodes, pipes, culverts):
             mask = self.nodes.content_type[node_idx] == objects.content_type
-            is_closed, dpumax = objects.get_1d2d_properties(
-                self.nodes,
-                node_idx[mask],
-                locations=locations,
-                channels=channels,
-                connection_nodes=connection_nodes,
+            content_pk = self.nodes.content_pk[node_idx[mask]]
+            lines_1d2d.assign_dpumax(
+                mask,
+                objects.get_1d2d_exchange_levels(
+                    content_pk,
+                    s1d=self.nodes.s1d[node_idx[mask]],
+                    locations=locations,
+                    channels=channels,
+                    connection_nodes=connection_nodes,
+                ),
             )
-            lines_1d2d.assign_kcu(mask, is_closed)
-            lines_1d2d.assign_dpumax(mask, dpumax)
 
         lines_1d2d.assign_ds1d(self.nodes)
         lines_1d2d.assign_ds1d_half()
 
         self.breaches = lines_1d2d.output_breaches(potential_breaches)
         self.lines += lines_1d2d
 
+    def add_1d2d_groundwater_lines(
+        self,
+        line_id_counter,
+        connection_nodes,
+        channels,
+        pipes,
+    ) -> Lines1D2D:
+        """Connect 1D and 2D groundwater elements by computing 1D-2D lines.
+
+        Appends self.lines.
+        """
+        lines_1d2d_gw = Lines1D2D.create_groundwater(self.nodes, line_id_counter)
+        if len(lines_1d2d_gw) == 0:
+            return
+        lines_1d2d_gw.assign_groundwater_exchange(
+            self.nodes,
+            self.lines,
+            connection_nodes=connection_nodes,
+            channels=channels,
+            pipes=pipes,
+        )
+        lines_1d2d_gw.assign_line_coords(self.nodes)
+        lines_1d2d_gw.assign_2d_node(self.cell_tree)
+        lines_1d2d_gw.transfer_2d_node_to_groundwater(self.nodes.n_groundwater_cells)
+        self.lines += lines_1d2d_gw
+
     def set_breach_ids(self, breach_points: PotentialBreachPoints):
         breach_points.assign_to_connection_nodes(self.nodes, self.lines)
         breach_points.match_breach_ids_with_calculation_types(self.nodes)
 
     def add_0d(self, surfaces: Union[zero_d.Surfaces, zero_d.ImperviousSurfaces]):
         """
         Zero dimension admin derived from 'v2_surfaces' and 'v2_impervious_surfaces'.
@@ -763,14 +802,21 @@
         """Sort the nodes and lines into the order required by the calculation core.
 
         Resets the nodes and lines ids to consecutive indices starting from 0.
         Also maps lines.line and pumps.line according to the new nodes indices.
 
         See NODE_ORDER and LINE_ORDER for the order.
         """
+        # if one of the nodes is null, the numpy id reset will silently overflow and assign a
+        # different new id, leading to an incorrect result
+        if np.any(self.lines.line == -9999):
+            raise ValueError(
+                "Some lines are not fully connected to nodes, causing a null value to be set for the line node"
+            )
+
         node_sorter = np.concatenate(
             [np.where(np.isin(self.nodes.node_type, group))[0] for group in NODE_ORDER]
         )
         is_1d_boundary = self.lines.is_1d_boundary == 1
         line_sorter = np.concatenate(
             [
                 np.where(np.isin(self.lines.kcu, group) & ~is_1d_boundary)[0]
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/grid_refinement.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/grid_refinement.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/groundwater.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/groundwater.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/initial_waterlevels.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/initial_waterlevels.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/linear.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/linear.py`

 * *Files 5% similar despite different names*

```diff
@@ -370,7 +370,26 @@
 
         result = weights * right + (1 - weights) * left
 
         # fix cases with nan on one side
         result[np.isnan(result)] = left[np.isnan(result)]
         result[np.isnan(result)] = right[np.isnan(result)]
         return result
+
+    @property
+    def has_groundwater_exchange(self):
+        return np.full(len(self), False, dtype=bool)
+
+    def apply_has_groundwater_exchange(self, nodes: Nodes, lines: Lines):
+        content_pk = self.id[self.has_groundwater_exchange]
+
+        if len(content_pk) == 0:
+            return
+
+        node_ids = np.unique(
+            lines.line[
+                (lines.content_type == self.content_type)
+                & np.isin(lines.content_pk, content_pk)
+            ]
+        )
+
+        nodes.has_groundwater_exchange[np.isin(nodes.id, node_ids)] = True
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/obstacles.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/obstacles.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/potential_breaches.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/potential_breaches.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 import numpy as np
 import shapely
 
 from threedigrid_builder.base import (
     Array,
-    Endpoints,
+    LineHalfs,
     Lines,
     Nodes,
     PointsOnLine,
     search,
 )
 from threedigrid_builder.constants import CalculationType, ContentType, Material
 from threedigrid_builder.exceptions import SchematisationError
@@ -73,56 +73,56 @@
             id=np.delete(self.id, to_delete),
             content_pk=np.delete(self.content_pk, to_delete),
             secondary_content_pk=np.delete(secondary_content_pk, to_delete),
             linestring_idx=np.delete(self.linestring_idx, to_delete),
             s1d=np.delete(s1d, to_delete),
         )
 
-    def find_for_endpoints(self, endpoints: Endpoints):
-        """Return a breach for each endpoint by matching against channel id.
+    def find_for_line_halfs(self, line_halfs: LineHalfs):
+        """Return a breach for each line_half by matching against channel id.
 
-        It is assumed there is exactly 1 breach per endpoint. This is ensured
+        It is assumed there is exactly 1 breach per line_half. This is ensured
         by PotentialBreachPoints.merge().
         """
-        # per (is_start) endpoint, look for a breach point (at start)
-        idx = np.full(len(endpoints), fill_value=-9999, dtype=np.int32)
-        idx[endpoints.is_start] = search(
+        # per (is_start) line_half, look for a breach point (at start)
+        idx = np.full(len(line_halfs), fill_value=-9999, dtype=np.int32)
+        idx[line_halfs.is_start] = search(
             self.linestring_id,  # channel id
-            endpoints.content_pk[endpoints.is_start],  # lines.content_pk
+            line_halfs.content_pk[line_halfs.is_start],  # lines.content_pk
             mask=self.at_start,
             check_exists=False,
         )
-        # per (is_end) endpoint, look for a breach point (at end)
-        idx[endpoints.is_end] = search(
+        # per (is_end) line_half, look for a breach point (at end)
+        idx[line_halfs.is_end] = search(
             self.linestring_id,
-            endpoints.content_pk[endpoints.is_end],
+            line_halfs.content_pk[line_halfs.is_end],
             mask=self.at_end,
             check_exists=False,
         )
         has_breach_point = idx != -9999
         idx = idx[has_breach_point]
-        return endpoints.node_id[has_breach_point], idx
+        return line_halfs.node_id[has_breach_point], idx
 
     def assign_to_connection_nodes(self, nodes: Nodes, lines: Lines):
         """Per connection node, assign max two potential breach ids.
 
         The priority is as follows:
         - Take the breach points of the first channel that has 2 breach
           points at the node.
         - If there are no double breach points: take the breach points of
           the first channel.
         """
-        # disassemble lines into Channel - Connection Node endpoints
-        endpoints = Endpoints.for_connection_nodes(
+        # disassemble lines into Channel - Connection Node line_halfs
+        line_halfs = LineHalfs.for_connection_nodes(
             nodes, lines, line_mask=lines.content_type == ContentType.TYPE_V2_CHANNEL
         )
-        endpoints.reorder_by("node_id")
+        line_halfs.reorder_by("node_id")
 
-        # per endpoint, match a breach point by their channel ids
-        node_ids, breach_point_idx = self.find_for_endpoints(endpoints)
+        # per line_half, match a breach point by their channel ids
+        node_ids, breach_point_idx = self.find_for_line_halfs(line_halfs)
         node_idx = nodes.id_to_index(node_ids)
 
         # iterate over nodes with a breach point and assign (if present)
         # the first double breach point
         for node_idx_ in np.unique(node_idx):
             options = breach_point_idx[node_idx == node_idx_]
             # sort by linestring (channel) id for reproducibility:
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/quadtree.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/quadtree.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     lg: int
     quad_idx: int
     transform: float
 
     def __init__(
         self, subgrid_meta, num_refine_levels, min_gridsize, use_2d_flow, refinements
     ):
-
         pixel_size = subgrid_meta["pixel_size"]
         min_num_pix = min_gridsize / pixel_size
         if min_num_pix % 2 == 0:
             self.lgrmin = int(min_num_pix)
         else:
             raise SchematisationError(
                 f"Smallest 2D grid cell does not contain an even number of pixels. "
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/structures.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/structures.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,36 +28,41 @@
     zoom_category: int
     display_name: str
 
 
 class Culverts(Array[Culvert], linear.BaseLinear):
     content_type = ContentType.TYPE_V2_CULVERT
 
-    def get_1d2d_properties(self, nodes, node_idx, connection_nodes, **kwargs):
-        """Compute properties (is_closed, dpumax) of 1D-2D culvert flowlines.
+    def is_closed(self, content_pk):
+        """Whether objects are 'closed' or 'open water'.
+
+        This is relevant for 1D-2D connections.
+        """
+        return np.full(len(content_pk), True, dtype=bool)
+
+    def get_1d2d_exchange_levels(self, content_pk, s1d, connection_nodes, **kwargs):
+        """Compute the exchange level (dpumax) for 1D-2D flowlines.
+
+        For pipes and culverts 1D2D exchange levels are interpololated between
+        connection node drain levels.
 
         Args:
-            nodes (Nodes): All nodes
-            node_idx (array of int): indices into nodes for which to compute properties
-            connection_nodes (ConnectionNodes): for the drain_level
+            content_pk (array of int): object ids for which to compute levels
+            s1d (array of int): distance on the objects where to compute levels
+            connection_nodes (ConnectionNodes): for the drain_levels
 
         Returns:
-            tuple of:
-            - is_closed (bool): always True
-            - dpumax (array of float): interpolated between CN drain_level
+            exchange levels a.k.a. dpumax (array of float)
         """
-        # dpumax is interpolated between drain levels of adjacent manholes (conn nodes)
-        dpumax = self.compute_drain_level(
-            ids=nodes.content_pk[node_idx],
-            s=nodes.s1d[node_idx],
+        return self.compute_drain_level(
+            ids=content_pk,
+            s=s1d,
             connection_nodes=connection_nodes,
         )
 
-        return True, dpumax
-
 
 class WeirOrifice:  # NL: stuw / doorlaat
     id: int
     code: str
     connection_node_start_id: int
     connection_node_end_id: int
     crest_level: float
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/windshielding.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/windshielding.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/grid/zero_d.py` & `threedigrid-builder-1.9.0/threedigrid_builder/grid/zero_d.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/interface/db.py` & `threedigrid-builder-1.9.0/threedigrid_builder/interface/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,61 +363,77 @@
         arr["the_geom"] = self.reproject(arr["the_geom"])
 
         # transform to a BoundaryConditions1D object
         return BoundaryConditions2D(**{name: arr[name] for name in arr.dtype.names})
 
     def get_channels(self) -> Channels:
         """Return Channels"""
+        cols = [
+            models.Channel.the_geom,
+            models.Channel.dist_calc_points,
+            models.Channel.id,
+            models.Channel.code,
+            models.Channel.connection_node_start_id,
+            models.Channel.connection_node_end_id,
+            models.Channel.calculation_type,
+            models.Channel.display_name,
+            models.Channel.zoom_category,
+        ]
+
+        try:
+            cols += [
+                models.Channel.exchange_thickness,
+                models.Channel.hydraulic_conductivity_out,
+                models.Channel.hydraulic_conductivity_in,
+            ]
+        except AttributeError:
+            pass
+
         with self.get_session() as session:
-            arr = (
-                session.query(
-                    models.Channel.the_geom,
-                    models.Channel.dist_calc_points,
-                    models.Channel.id,
-                    models.Channel.code,
-                    models.Channel.connection_node_start_id,
-                    models.Channel.connection_node_end_id,
-                    models.Channel.calculation_type,
-                    models.Channel.display_name,
-                    models.Channel.zoom_category,
-                )
-                .order_by(models.Channel.id)
-                .as_structarray()
-            )
+            arr = session.query(*cols).order_by(models.Channel.id).as_structarray()
 
         arr["the_geom"] = self.reproject(arr["the_geom"])
         # map "old" calculation types (100, 101, 102, 105) to (0, 1, 2, 5)
         arr["calculation_type"][arr["calculation_type"] >= 100] -= 100
 
         # transform to a Channels object
         return Channels(**{name: arr[name] for name in arr.dtype.names})
 
     def get_connection_nodes(self) -> ConnectionNodes:
         """Return ConnectionNodes (which are enriched using the manhole table)"""
+        cols = [
+            models.ConnectionNode.the_geom,
+            models.ConnectionNode.id,
+            models.ConnectionNode.code,
+            models.ConnectionNode.storage_area,
+            models.ConnectionNode.initial_waterlevel,
+            models.Manhole.id.label("manhole_id"),
+            models.Manhole.calculation_type,
+            models.Manhole.bottom_level,
+            models.Manhole.drain_level,
+            models.Manhole.manhole_indicator,
+            models.Manhole.surface_level,
+            models.Manhole.shape,
+            models.Manhole.width,
+            models.Manhole.display_name,
+            models.Manhole.zoom_category,
+        ]
+        try:
+            cols += [
+                models.Manhole.exchange_thickness,
+                models.Manhole.hydraulic_conductivity_out,
+                models.Manhole.hydraulic_conductivity_in,
+            ]
+        except AttributeError:
+            pass
+
         with self.get_session() as session:
             arr = (
-                session.query(
-                    models.ConnectionNode.the_geom,
-                    models.ConnectionNode.id,
-                    models.ConnectionNode.code,
-                    models.ConnectionNode.storage_area,
-                    models.ConnectionNode.initial_waterlevel,
-                    models.Manhole.id.label("manhole_id"),
-                    models.Manhole.calculation_type,
-                    models.Manhole.bottom_level,
-                    models.Manhole.drain_level,
-                    models.Manhole.manhole_indicator,
-                    models.Manhole.surface_level,
-                    models.Manhole.shape,
-                    models.Manhole.width,
-                    models.Manhole.display_name,
-                    models.Manhole.zoom_category,
-                )
+                session.query(*cols)
                 .join(models.ConnectionNode.manholes, isouter=True)
-                .distinct(models.ConnectionNode.id)
                 .order_by(models.ConnectionNode.id)
                 .as_structarray()
             )
 
         arr["the_geom"] = self.reproject(arr["the_geom"])
 
         # replace -9999.0 with NaN in initial_waterlevel
@@ -633,36 +649,42 @@
         # map friction_type 4 to friction_type 2 to match crosssectionlocation enum
         arr["friction_type"][arr["friction_type"] == 4] = 2
 
         return Orifices(**{name: arr[name] for name in arr.dtype.names})
 
     def get_pipes(self) -> Pipes:
         """Return Pipes"""
+        cols = [
+            models.Pipe.id,
+            models.Pipe.code,
+            models.Pipe.sewerage_type,
+            models.Pipe.calculation_type,
+            models.Pipe.invert_level_start_point,
+            models.Pipe.invert_level_end_point,
+            models.Pipe.friction_type,
+            models.Pipe.friction_value,
+            models.Pipe.dist_calc_points,
+            models.Pipe.connection_node_start_id,
+            models.Pipe.connection_node_end_id,
+            models.Pipe.cross_section_definition_id,
+            models.Pipe.display_name,
+            models.Pipe.zoom_category,
+            models.Pipe.material,
+        ]
+        try:
+            cols += [
+                models.Pipe.exchange_thickness,
+                models.Pipe.hydraulic_conductivity_out,
+                models.Pipe.hydraulic_conductivity_in,
+            ]
+        except AttributeError:
+            pass
+
         with self.get_session() as session:
-            arr = (
-                session.query(
-                    models.Pipe.id,
-                    models.Pipe.code,
-                    models.Pipe.sewerage_type,
-                    models.Pipe.calculation_type,
-                    models.Pipe.invert_level_start_point,
-                    models.Pipe.invert_level_end_point,
-                    models.Pipe.friction_type,
-                    models.Pipe.friction_value,
-                    models.Pipe.dist_calc_points,
-                    models.Pipe.connection_node_start_id,
-                    models.Pipe.connection_node_end_id,
-                    models.Pipe.cross_section_definition_id,
-                    models.Pipe.display_name,
-                    models.Pipe.zoom_category,
-                    models.Pipe.material,
-                )
-                .order_by(models.Pipe.id)
-                .as_structarray()
-            )
+            arr = session.query(*cols).order_by(models.Pipe.id).as_structarray()
 
         # map friction_type 4 to friction_type 2 to match crosssectionlocation enum
         arr["friction_type"][arr["friction_type"] == 4] = 2
 
         # transform to a Pipes object
         return Pipes(**{name: arr[name] for name in arr.dtype.names})
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/interface/dict_out.py` & `threedigrid-builder-1.9.0/threedigrid_builder/interface/dict_out.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/interface/geopackage.py` & `threedigrid-builder-1.9.0/threedigrid_builder/interface/geopackage.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/interface/gridadmin.py` & `threedigrid-builder-1.9.0/threedigrid_builder/interface/gridadmin.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,15 @@
 LINE_TYPES_1D2D = (
     LineType.LINE_1D2D_SINGLE_CONNECTED_CLOSED,
     LineType.LINE_1D2D_SINGLE_CONNECTED_OPEN_WATER,
     LineType.LINE_1D2D_DOUBLE_CONNECTED_CLOSED,
     LineType.LINE_1D2D_DOUBLE_CONNECTED_OPEN_WATER,
 )
 
-LINE_TYPES_1D2D_GW = (
-    LineType.LINE_1D2D_GROUNDWATER_OPEN_WATER,
-    LineType.LINE_1D2D_GROUNDWATER_SEWER,
-)
+LINE_TYPES_1D2D_GW = (LineType.LINE_1D2D_GROUNDWATER,)
 
 LINE_TYPES_2D = (
     LineType.LINE_2D_U,
     LineType.LINE_2D_V,
     LineType.LINE_2D,
     LineType.LINE_2D_OBSTACLE,
     LineType.LINE_2D_OBSTACLE_U,
@@ -575,15 +572,14 @@
         self.write_dataset(group, "upper_stop_level", pumps.upper_stop_level)
         self.write_dataset(
             group, "display_name", to_bytes_array(pumps.display_name, 64)
         )
         self.write_dataset(group, "zoom_category", pumps.zoom_category)
 
     def write_surfaces(self, surfaces: Surfaces, surface_maps: SurfaceMaps):
-
         # For now use 0 instead of NaN as fill value for surfaces
         # The calcore does not support NaN (for surfaces) yet
         default_fill_value = 0
 
         group = self._file.create_group("surface")
         self.write_dataset(group, "id", surfaces.id, fill=default_fill_value)
         self.write_dataset(group, "code", to_bytes_array(surfaces.code, 100))
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/interface/raster_gdal.py` & `threedigrid-builder-1.9.0/threedigrid_builder/interface/raster_gdal.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/conftest.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_array.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,7 +487,15 @@
 )
 def test_take(name, index, expected):
     records = Records(
         id=range(3), name=["a", "b", "c"], animal=[1, 2, 3], number=[1.2, 2.3, 3.4]
     )
 
     assert_equal(records.take(name, index), expected)
+
+
+def test_empty_column():
+    records = Records(id=[1, 2, 3])
+    assert "number" not in records.__dict__
+    arr = records.number
+    assert records.__dict__["number"] is arr
+    assert_equal(arr, np.nan)
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_boundary_conditions.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_boundary_conditions.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 import pytest
 import shapely
 from numpy.testing import assert_array_equal
 
 from threedigrid_builder.base import Lines, Nodes
 from threedigrid_builder.constants import (
+    BoundaryType,
     CalculationType,
     ContentType,
     LineType,
     NodeType,
 )
 from threedigrid_builder.exceptions import SchematisationError
 from threedigrid_builder.grid import BoundaryConditions1D, BoundaryConditions2D, Grid
@@ -326,7 +327,119 @@
         boundary_conditions_2d.get_nodes_and_lines(
             grid2d.nodes,
             grid2d.cell_tree,
             grid2d.quadtree,
             itertools.count(),
             itertools.count(),
         )
+
+
+@pytest.fixture
+def grid2d_gw():
+    nodes = Nodes(
+        id=range(4),
+        node_type=([NodeType.NODE_2D_OPEN_WATER] * 2)
+        + ([NodeType.NODE_2D_GROUNDWATER] * 2),
+        bounds=[(2.0, 3.0, 7.0, 8.0), (7.0, 3.0, 12.0, 8.0)] * 2,
+        pixel_coords=[(0, 0, 10, 10), (10, 0, 20, 10)] * 2,
+        nodk=[1, 1, 1, 1],
+        nodm=[1, 2, 1, 2],
+        nodn=[1, 1, 1, 1],
+    )
+    grid = Grid(nodes=nodes, lines=Lines(id=[]))
+    grid.quadtree = mock.Mock()
+    grid.quadtree.quad_idx = np.array([[1, 2]])[::-1].T
+    return grid
+
+
+@pytest.mark.parametrize(
+    "boundary_type,node_type,kcu,line",
+    [
+        (
+            BoundaryType.WATERLEVEL,
+            NodeType.NODE_2D_BOUNDARIES,
+            LineType.LINE_2D_BOUNDARY_EAST,
+            (1, 9),
+        ),
+        (
+            BoundaryType.DISCHARGE,
+            NodeType.NODE_2D_BOUNDARIES,
+            LineType.LINE_2D_BOUNDARY_EAST,
+            (1, 9),
+        ),
+        (
+            BoundaryType.GROUNDWATERLEVEL,
+            NodeType.NODE_2D_GROUNDWATER_BOUNDARIES,
+            LineType.LINE_2D_GROUNDWATER_BOUNDARY_EAST,
+            (3, 9),
+        ),
+        (
+            BoundaryType.GROUNDWATERDISCHARGE,
+            NodeType.NODE_2D_GROUNDWATER_BOUNDARIES,
+            LineType.LINE_2D_GROUNDWATER_BOUNDARY_EAST,
+            (3, 9),
+        ),
+    ],
+)
+def test_2d_boundary_condition_types(grid2d_gw, boundary_type, node_type, kcu, line):
+    boundary_conditions_2d = BoundaryConditions2D(
+        id=[1],
+        boundary_type=[boundary_type],
+        the_geom=[shapely.linestrings([(12.0, 3.0), (12.0, 8.0)])],
+    )
+    nodes, lines = boundary_conditions_2d.get_nodes_and_lines(
+        grid2d_gw.nodes,
+        grid2d_gw.cell_tree,
+        grid2d_gw.quadtree,
+        itertools.count(9),
+        itertools.count(7),
+    )
+
+    assert_array_equal(nodes.id, [9])
+    assert_array_equal(nodes.node_type, [node_type])
+    assert_array_equal(nodes.boundary_id, [1])
+    assert_array_equal(nodes.boundary_type, [boundary_type])
+    assert_array_equal(nodes.bounds, [(12.0, 3.0, 17, 8.0)])
+    assert_array_equal(nodes.pixel_coords, -9999)
+    assert_array_equal(nodes.nodm, [3])
+    assert_array_equal(nodes.nodn, [1])
+    assert_array_equal(lines.id, [7])
+    assert_array_equal(lines.kcu, [kcu])
+    assert_array_equal(lines.line, [line])
+    assert_array_equal(lines.cross_pix_coords, [(20, 0, 20, 10)])
+
+
+def test_2d_boundary_condition_combined(grid2d_gw):
+    boundary_conditions_2d = BoundaryConditions2D(
+        id=[1, 2],
+        boundary_type=[BoundaryType.WATERLEVEL, BoundaryType.GROUNDWATERLEVEL],
+        the_geom=[shapely.linestrings([(12.0, 3.0), (12.0, 8.0)])] * 2,
+    )
+
+    nodes, lines = boundary_conditions_2d.get_nodes_and_lines(
+        grid2d_gw.nodes,
+        grid2d_gw.cell_tree,
+        grid2d_gw.quadtree,
+        itertools.count(9),
+        itertools.count(7),
+    )
+
+    assert_array_equal(nodes.id, [9, 10])
+    assert_array_equal(
+        nodes.node_type,
+        [NodeType.NODE_2D_BOUNDARIES, NodeType.NODE_2D_GROUNDWATER_BOUNDARIES],
+    )
+    assert_array_equal(nodes.boundary_id, [1, 2])
+    assert_array_equal(
+        nodes.boundary_type, [BoundaryType.WATERLEVEL, BoundaryType.GROUNDWATERLEVEL]
+    )
+    assert_array_equal(nodes.bounds, [(12.0, 3.0, 17, 8.0)] * 2)
+    assert_array_equal(nodes.pixel_coords, -9999)
+    assert_array_equal(nodes.nodm, 3)
+    assert_array_equal(nodes.nodn, 1)
+    assert_array_equal(lines.id, [7, 8])
+    assert_array_equal(
+        lines.kcu,
+        [LineType.LINE_2D_BOUNDARY_EAST, LineType.LINE_2D_GROUNDWATER_BOUNDARY_EAST],
+    )
+    assert_array_equal(lines.line, [(1, 9), (3, 10)])
+    assert_array_equal(lines.cross_pix_coords, [(20, 0, 20, 10)] * 2)
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_channels.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_pumps.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 import numpy as np
 import pytest
-import shapely
 from numpy.testing import assert_array_equal
 
-from threedigrid_builder.base import Nodes
+from threedigrid_builder.base import Nodes, Pumps
 from threedigrid_builder.constants import ContentType
-from threedigrid_builder.grid import Channels, CrossSectionLocations
+from threedigrid_builder.exceptions import SchematisationError
 
 
 @pytest.fixture
-def channels():
-    return Channels(
-        the_geom=shapely.linestrings([[(0, 0), (6, 0), (6, 6)]]),
-        dist_calc_points=np.array([5.0]),
-        id=np.array([1]),
-        code=np.array(["one"]),
-        connection_node_start_id=np.array([21]),
-        connection_node_end_id=np.array([42]),
-        calculation_type=np.array([2]),
+def nodes():
+    CN = ContentType.TYPE_V2_CONNECTION_NODES
+    CH = ContentType.TYPE_V2_CHANNEL
+    return Nodes(
+        id=[0, 1, 3, 4],
+        content_type=[CH, CN, CN, CH],
+        content_pk=[21, 21, 33, 42],
+        coordinates=[(0, 21), (1, 25), (2, 33), (3, 42)],
+        dmax=[1.0, 2.0, 3.0, 4.0],
     )
 
 
-def test_1d2d_properties(channels):
-    nodes = Nodes(
-        id=[0, 2, 5],
-        s1d=[3, np.nan, 6],
-        content_type=[
-            ContentType.TYPE_V2_CHANNEL,
-            ContentType.TYPE_V2_CONNECTION_NODES,
-            ContentType.TYPE_V2_CHANNEL,
-        ],
-        content_pk=[1, 3, 1],
-    )
-    locations = CrossSectionLocations(
-        id=[2, 5],
-        the_geom=shapely.points([(0, 0), [6, 6]]),
-        bank_level=[1.0, 13.0],
-        channel_id=[1, 1],
+@pytest.fixture
+def pumps():
+    return Pumps(
+        id=[2, 35],
+        line=[(1, 3), (1, -9999)],
+        connection_node_start_id=[21, 21],
+        connection_node_end_id=[33, -9999],
     )
-    node_idx = [0, 2]
-
-    is_closed, dpumax = channels.get_1d2d_properties(nodes, node_idx, locations)
 
-    # channels are no sewerage
-    assert_array_equal(is_closed, False)
 
-    # bank levels are interpolated
-    assert_array_equal(dpumax, [4.0, 7.0])
+def test_renumber(pumps):
+    pumps.renumber()
+    assert_array_equal(pumps.id, [0, 1])
+    assert_array_equal(pumps.content_pk, [2, 35])
+
+
+def test_set_lines(pumps, nodes):
+    pumps.line[:] = -9999
+    pumps.set_lines(nodes)
+    assert_array_equal(pumps.line, [(1, 3), (1, -9999)])
+
+
+@pytest.mark.parametrize(
+    "start,end",
+    [
+        ([-9999, 21], [33, 33]),
+        ([42, 21], [33, 33]),
+        ([21, 21], [33, 42]),
+    ],
+)
+def test_set_lines_error(start, end, pumps, nodes):
+    pumps.connection_node_start_id[:] = start
+    pumps.connection_node_end_id[:] = end
+    with pytest.raises(SchematisationError):
+        pumps.set_lines(nodes)
+
+
+def test_set_node_data(pumps, nodes):
+    pumps.set_node_data(nodes)
+    assert_array_equal(pumps.line_coords, [(1, 25, 2, 33), (1, 25, np.nan, np.nan)])
+    assert_array_equal(pumps.coordinates, [(1.5, 29.0), (1.0, 25.0)])
+    assert_array_equal(pumps.bottom_level, [2.0, 2.0])
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_connection_nodes.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_connection_nodes.py`

 * *Files 9% similar despite different names*

```diff
@@ -215,35 +215,22 @@
     set_bottom_levels(nodes, lines)
     assert caplog.messages[0].startswith("Manholes [3] have a bottom_level")
 
     # assert the resulting value of dmax
     assert_almost_equal(nodes.dmax, [3.0, 20.0])
 
 
-def test_1d2d_properties(connection_nodes, caplog):
+def test_get_1d2d_exchange_levels(connection_nodes: ConnectionNodes, caplog):
     """Test setup:
 
-    - node 0: this has storage_area, drain_level is copied
-    - node 1: this is skipped (not in node_idx)
-    - node 2: this has no storage_area, it has 2 channels, lowest bank_level is taken
-    - node 3: this has no storage_area, it has no channels: outcome is NaN
-    - node 4: this has no storage_area, it 1 channel with no bank level: outcome is NaN
-    - node 5: this has storage_area == 0, drain_level is copied
+    - conn. node 1: drain_level is copied
+    - conn. node 3: it has 2 channels, lowest bank_level is taken
+    - conn. node 4: it has no channels: outcome is NaN
+    - conn. node 9: it 1 channel with no bank level: outcome is NaN
     """
-    caplog.set_level(
-        logging.WARNING, logger="threedigrid_builder.grid.connection_nodes"
-    )
-
-    nodes = Nodes(
-        id=[0, 1, 2, 3, 4, 5],
-        content_pk=[1, 3, 99, 4, 9, 10],
-        dmax=[1.0, 3.0, 2.0, 4.0, 2.3, 5.2],
-    )
-    node_idx = np.array([0, 1, 3, 4, 5])
-
     # channels & cs locations are so that:
     # - channel 32 (CN 1 -> 3, N 0 -> 1), start is 4.0 and end is 0.0
     # - channel 33 (CN 3 -> 9, N 1 -> 4), start&end are 1.0
     # - channel 34 (CN 3 -> 9, N 1 -> 4), 1 bank_level is nan so start&end are nan
     channels = Channels(
         id=[32, 33, 34, 35],
         connection_node_start_id=[1, 3, 3, 3],
@@ -262,18 +249,58 @@
         channel_id=[32, 32, 33, 34, 34, 35],
         the_geom=shapely.points(
             [(0, 0), (10, 0), (10, 25), (10, 22), (10, 28), (0, 0)]
         ),
         bank_level=[4.0, 0.0, 1.0, -10.0, np.nan, 3.4],
     )
 
-    is_closed, dpumax = connection_nodes.get_1d2d_properties(
-        nodes, node_idx, channels, locations
+    caplog.set_level(
+        logging.WARNING, logger="threedigrid_builder.grid.connection_nodes"
     )
 
-    assert_array_equal(is_closed, [True, False, False, False, True])
-    assert_array_equal(dpumax, [1.2, np.nan, np.nan, 1.0, 3.4])
+    content_pk = np.array([1, 3, 4, 9])
+    actual = connection_nodes.get_1d2d_exchange_levels(
+        content_pk,
+        channels=channels,
+        locations=locations,
+        s1d=None,
+        connection_nodes=None,
+    )
+
+    assert_array_equal(actual, [1.2, np.nan, np.nan, 1.0])
 
     assert (
         caplog.record_tuples[0][2]
         == "Manholes [42] have a bottom_level that is above drain_level."
     )
+
+
+def test_is_closed(connection_nodes):
+    actual = connection_nodes.is_closed(content_pk=[1, 3, 4, 9, 10])
+    assert_array_equal(actual, [True, False, False, False, True])
+
+
+@pytest.mark.parametrize(
+    "area,thickness,hc_out,hc_in,expected",
+    [
+        (9.0, 0.1, 3.0, 2.0, True),
+        (0.0, 0.1, 3.0, 2.0, False),
+        (np.nan, 0.1, 3.0, 2.0, False),
+        (9.0, 0.0, 3.0, 2.0, False),
+        (9.0, np.nan, 3.0, 2.0, False),
+        (9.0, 0.1, np.nan, 2.0, False),
+        (9.0, 0.1, 3.0, np.nan, False),
+    ],
+)
+def test_has_groundwater_exchange(area, thickness, hc_out, hc_in, expected):
+    connection_nodes = ConnectionNodes(
+        id=[1],
+        storage_area=area,
+        exchange_thickness=thickness,
+        hydraulic_conductivity_out=hc_out,
+        hydraulic_conductivity_in=hc_in,
+    )
+
+    actual = connection_nodes.has_groundwater_exchange
+
+    assert len(actual) == 1
+    assert actual[0] == expected
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_cross_section_definitions.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_cross_section_locations.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_cross_section_locations.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_db.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_dem_average.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_dem_average.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_dict_out.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_dict_out.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_embedded.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_embedded.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_exchange_lines.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_lines_1d2d.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 import itertools
+import re
+from contextlib import nullcontext as does_not_raise
 from unittest import mock
 
 import numpy as np
 import pytest
 import shapely
 from numpy.testing import assert_almost_equal, assert_array_equal
 from shapely.testing import assert_geometries_equal
 
 from threedigrid_builder.base import Lines, Nodes
 from threedigrid_builder.constants import CalculationType, ContentType, LineType
+from threedigrid_builder.exceptions import SchematisationError
 from threedigrid_builder.grid import (
+    Channels,
+    ConnectionNodes,
     ExchangeLines,
     Lines1D2D,
     Obstacles,
+    Pipes,
     PotentialBreaches,
 )
 
 ISO = CalculationType.ISOLATED
 C1 = CalculationType.CONNECTED
 C2 = CalculationType.DOUBLE_CONNECTED
 CN = ContentType.TYPE_V2_CONNECTION_NODES
 CH = ContentType.TYPE_V2_CHANNEL
+PIPE = ContentType.TYPE_V2_PIPE
 EXC = ContentType.TYPE_V2_EXCHANGE_LINE
 BREACH = ContentType.TYPE_V2_BREACH
 
 
 @pytest.mark.parametrize(
     "calculation_type,expected_line",
     [
@@ -103,30 +110,38 @@
     )
     lines.assign_exchange_lines(exchange_lines)
 
     assert_array_equal(lines.content_pk, expected_content_pk)
     assert_array_equal(lines.content_type, expected_content_type)
 
 
-def test_assign_2d_side():
+def test_assign_line_coords():
     nodes = Nodes(
         id=[1, 2, 3],
         coordinates=[(2, 5), (4, 5), (6, 5)],
     )
+    lines = Lines1D2D(id=range(2), line=[[-9999, 1], [-9999, 3]])
+    lines.assign_line_coords(nodes)
+
+    assert_array_equal(lines.line_coords, [[2, 5, 2, 5], [6, 5, 6, 5]])
+
+
+def test_assign_2d_side_from_exchange_lines():
     exchange_lines = ExchangeLines(
         id=[1, 2],
         the_geom=shapely.linestrings([[[0, 0], [10, 0]], [[0, 10], [10, 10]]]),
     )
     lines = Lines1D2D(
         id=range(4),
         line=[[-9999, 1], [-9999, 1], [-9999, 2], [-9999, 3]],
+        line_coords=[[2, 5, 2, 5], [2, 5, 2, 5], [4, 5, 4, 5], [6, 5, 6, 5]],
         content_pk=[1, 2, 1, -9999],
         content_type=[EXC, EXC, EXC, -9999],
     )
-    lines.assign_2d_side(nodes, exchange_lines)
+    lines.assign_2d_side_from_exchange_lines(exchange_lines)
 
     assert_array_equal(lines.line_coords[:, :2], [[2, 0], [2, 10], [4, 0], [6, 5]])
 
 
 @pytest.fixture
 def cell_tree():
     return shapely.STRtree([shapely.box(0, 0, 1, 1), shapely.box(1, 0, 3, 2)])
@@ -163,14 +178,51 @@
 
     lines.assign_2d_node(cell_tree)
 
     assert_array_equal(lines.line[:, 0], expected_2d_node_id)
     assert_array_equal(lines.line_coords, np.nan)  # is cleared
 
 
+@pytest.mark.parametrize(
+    "nodes,lines,expectation",
+    [
+        (
+            Nodes(
+                id=[1, 2], content_type=[12, 12], content_pk=[5, 6], node_type=[4, 4]
+            ),
+            Lines1D2D(
+                id=[3, 4],
+                line=[(-9999, 1), (1, 2)],
+                line_coords=[(10, 0, 0, 0), (5, 2, 3, 8)],
+            ),
+            pytest.raises(
+                SchematisationError,
+                match=re.escape(
+                    "The following objects are connected but are (partially) outside of the 2D model domain: connection nodes [5]."
+                ),
+            ),
+        ),
+        (
+            Nodes(
+                id=[1, 2], content_type=[12, 12], content_pk=[5, 6], node_type=[4, 4]
+            ),
+            Lines1D2D(
+                id=[3, 4],
+                line=[(2, 1), (1, 2)],
+                line_coords=[(10, 0, 0, 0), (5, 2, 3, 8)],
+            ),
+            does_not_raise(),
+        ),
+    ],
+)
+def test_check_line_unassigned_nodes(nodes, lines, expectation):
+    with expectation:
+        lines.check_unassigned(nodes)
+
+
 def test_assign_kcu():
     lines = Lines1D2D(id=range(7), line=[[-9999] + [x] for x in [1, 1, 2, 2, 3, 4, 5]])
     lines.content_type[0] = ContentType.TYPE_V2_BREACH
 
     lines.assign_kcu(
         mask=np.array([1, 1, 1, 1, 0, 1, 1], dtype=bool),
         is_closed=np.array([0, 0, 1, 1, 0, 1], dtype=bool),
@@ -259,15 +311,22 @@
 ):
     obstacles = mock.Mock()
     obstacles.compute_dpumax.return_value = (
         np.array([1.2, np.nan]),
         np.array([1, -9999]),
     )
 
-    lines = Lines1D2D(id=range(3), content_type=[EXC, -9999, EXC])
+    lines = Lines1D2D(
+        id=range(3),
+        kcu=[
+            LineType.LINE_1D2D_SINGLE_CONNECTED_OPEN_WATER,
+            LineType.LINE_1D2D_SINGLE_CONNECTED_CLOSED,
+            LineType.LINE_1D2D_SINGLE_CONNECTED_OPEN_WATER,
+        ],
+    )
 
     lines.assign_dpumax_from_obstacles(obstacles)
 
     args, kwargs = obstacles.compute_dpumax.call_args
     assert len(args) == 1
     assert args[0] is lines
     assert len(kwargs) == 1
@@ -429,53 +488,28 @@
         content_pk=[1, 2, 3, 4],
     )
     lines = Lines(
         id=range(3),
         line=[(1, 2), (1, 3), (4, 1)],
         content_type=ContentType.TYPE_V2_CHANNEL,
         content_pk=[11, 12, 13],
+        ds1d=[1.2, 2.3, 3.4],
+        ds1d_half=[0.6, 1.0, 1.7],
     )
     return nodes, lines
 
 
 @pytest.fixture
 def potential_breaches():
     return PotentialBreaches(
         id=[5, 6, 7],
         channel_id=[11, 12, 13],
     )
 
 
-def test_channel_mapping():
-    exchange_lines = ExchangeLines(id=range(1, 6), channel_id=[15, 2, 3, 15, 3])
-    actual = exchange_lines.channel_mapping
-
-    assert_array_equal(actual.id, [2, 3, 15])
-    assert_array_equal(actual.exchange_line_id, [2, 3, 1])
-    assert_array_equal(actual.secondary_exchange_line_id, [-9999, 5, 4])
-
-
-@pytest.mark.parametrize(
-    "channel_id,expected,is_primary",
-    [
-        (np.array([]), [], True),
-        (np.array([1]), [-9999], True),
-        (np.array([2]), [2], True),
-        (np.array([2]), [-9999], False),
-        (np.array([3]), [3], True),
-        (np.array([3]), [5], False),
-    ],
-)
-def test_get_for_channel_id(channel_id, expected, is_primary):
-    exchange_lines = ExchangeLines(id=range(1, 6), channel_id=[15, 2, 3, 15, 3])
-    actual = exchange_lines.get_for_channel_id(channel_id, is_primary)
-
-    assert_array_equal(actual, expected)
-
-
 @pytest.mark.parametrize(
     "kcu,expected",
     [
         ([ISO, ISO, ISO], 33),
         ([C1, ISO, ISO], 11),
         ([ISO, ISO, C1], 13),
         ([ISO, C1, C1], 12),
@@ -527,7 +561,161 @@
 
     assert_geometries_equal(actual.the_geom, get_velocity_points.return_value)
 
     assert_array_equal(actual.code, ["b"])
     assert_array_equal(actual.display_name, ["bb"])
 
     get_velocity_points.assert_called_once()
+
+
+@pytest.mark.parametrize("has_groundwater_exchange", [True, False])
+def test_create_lines_1d2d_groundwater(has_groundwater_exchange):
+    nodes = Nodes(
+        id=[1], content_pk=3, has_groundwater_exchange=has_groundwater_exchange
+    )
+    actual = Lines1D2D.create_groundwater(nodes, itertools.count())
+
+    if has_groundwater_exchange:
+        assert_array_equal(actual.line, [[-9999, 1]])
+        assert_array_equal(actual.kcu, LineType.LINE_1D2D_GROUNDWATER)
+    else:
+        assert len(actual) == 0
+
+
+@pytest.mark.parametrize(
+    "n_groundwater_cells,expected", [(0, [-9999, -9999]), (3, [-9999, 5])]
+)
+def test_transfer_2d_node_to_groundwater(n_groundwater_cells, expected):
+    lines_1d2d = Lines1D2D(id=range(1, 3), line=[[-9999, 6], [2, 9]])
+    lines_1d2d.transfer_2d_node_to_groundwater(n_groundwater_cells)
+    assert_array_equal(lines_1d2d.line[:, 0], expected)  # 2d side
+    assert_array_equal(lines_1d2d.line[:, 1], [6, 9])  # 1d side
+
+
+def test_assign_groundwater_exchange_from_connection_nodes():
+    nodes = Nodes(
+        id=[1, 2, 3],
+        content_type=[CN, CN, CH],
+        content_pk=[3, 5, 3],
+    )
+    connection_nodes = ConnectionNodes(
+        id=[3, 5],
+        storage_area=[9.0, np.nan],
+        exchange_thickness=[0.1, np.nan],
+        hydraulic_conductivity_out=[3.0, np.nan],
+        hydraulic_conductivity_in=[2.0, np.nan],
+    )
+    lines_1d2d = Lines1D2D(
+        id=[1, 2, 3],
+        line=[[-9999, 1], [-9999, 2], [-9999, 3]],
+        cross_weight=0.1,
+        frict_value1=0.2,
+        frict_value2=0.3,
+    )
+    lines_1d2d._assign_groundwater_exchange_from_connection_nodes(
+        nodes, connection_nodes
+    )
+
+    expected_frict1 = 3.0 / 0.1 * 3.0
+    expected_frict2 = 2.0 / 0.1 * 3.0
+    assert_almost_equal(lines_1d2d.cross_weight, [3.1, 0.1, 0.1])
+    assert_almost_equal(lines_1d2d.frict_value1, [expected_frict1 + 0.2, 0.2, 0.2])
+    assert_almost_equal(lines_1d2d.frict_value2, [expected_frict2 + 0.3, 0.3, 0.3])
+
+
+def test_assign_groundwater_exchange_from_linear_objects(threeway_junction):
+    nodes, lines = threeway_junction
+
+    channels = Channels(
+        id=[11, 12, 13],
+        exchange_thickness=[0.1, 0.2, np.nan],
+        hydraulic_conductivity_out=[2.0, 3.0, np.nan],
+        hydraulic_conductivity_in=[4.0, 5.0, np.nan],
+    )
+
+    lines_1d2d = Lines1D2D(
+        id=range(4),
+        line=[[-9999, 1], [-9999, 2], [-9999, 3], [-9999, 4]],
+        cross_weight=0.1,
+        frict_value1=0.2,
+        frict_value2=0.3,
+    )
+    lines_1d2d._assign_groundwater_exchange_from_linear_objects(nodes, lines, channels)
+
+    assert_almost_equal(
+        lines_1d2d.cross_weight, [0.1 + 0.6 + 1.0, 0.1 + 0.6, 0.1 + 1.3, 0.1]
+    )
+    assert_almost_equal(
+        lines_1d2d.frict_value1,
+        [
+            0.2 + 0.6 * 2.0 / 0.1 + 1.0 * 3.0 / 0.2,
+            0.2 + 0.6 * 2.0 / 0.1,
+            0.2 + 1.3 * 3.0 / 0.2,
+            0.2,
+        ],
+    )
+    assert_almost_equal(
+        lines_1d2d.frict_value2,
+        [
+            0.3 + 0.6 * 4.0 / 0.1 + 1.0 * 5.0 / 0.2,
+            0.3 + 0.6 * 4.0 / 0.1,
+            0.3 + 1.3 * 5.0 / 0.2,
+            0.3,
+        ],
+    )
+
+
+def test_assign_groundwater_exchange(threeway_junction):
+    nodes, lines = threeway_junction
+    dmax = np.array([-2.0, -3.0, -4.0, -5.0])
+    nodes.dmax = dmax
+
+    nodes.content_type[1:] = -9999
+    lines.content_type[2] = ContentType.TYPE_V2_PIPE
+    connection_nodes = ConnectionNodes(
+        id=[1],
+        storage_area=[9.0],
+        exchange_thickness=[0.1],
+        hydraulic_conductivity_out=[3.0],
+        hydraulic_conductivity_in=[2.0],
+    )
+    channels = Channels(
+        id=[11, 12],
+        exchange_thickness=[0.15, np.nan],
+        hydraulic_conductivity_out=[2.0, np.nan],
+        hydraulic_conductivity_in=[4.0, np.nan],
+    )
+    pipes = Pipes(
+        id=[13],
+        exchange_thickness=[0.2],
+        hydraulic_conductivity_out=[3.0],
+        hydraulic_conductivity_in=[5.0],
+    )
+
+    lines_1d2d = Lines1D2D(
+        id=range(4),
+        line=[[-9999, 1], [-9999, 2], [-9999, 3], [-9999, 4]],
+    )
+    lines_1d2d.assign_groundwater_exchange(
+        nodes, lines, connection_nodes=connection_nodes, channels=channels, pipes=pipes
+    )
+
+    assert_almost_equal(lines_1d2d.cross_weight, [3.0 + 0.6 + 1.7, 0.6, 0.0, 1.7])
+    assert_almost_equal(
+        lines_1d2d.frict_value1,
+        [
+            (3.0 * 3.0 / 0.1 + 0.6 * 2.0 / 0.15 + 1.7 * 3.0 / 0.2) / (3.0 + 0.6 + 1.7),
+            2.0 / 0.15,
+            np.nan,
+            3.0 / 0.2,
+        ],
+    )
+    assert_almost_equal(
+        lines_1d2d.frict_value2,
+        [
+            (3.0 * 2.0 / 0.1 + 0.6 * 4.0 / 0.15 + 1.7 * 5.0 / 0.2) / (3.0 + 0.6 + 1.7),
+            4.0 / 0.15,
+            np.nan,
+            5.0 / 0.2,
+        ],
+    )
+    assert_almost_equal(lines_1d2d.dpumax, dmax)
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_grid.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,14 @@
     grid2d.meta.crs_wkt = None
     grid2d.set_crs(crs_wkt_28992_legacy)
     assert grid2d.meta.epsg_code == 28992
     assert grid2d.meta.crs_wkt == crs_wkt_28992_legacy.srs
 
 
 def test_from_quadtree():
-
     quadtree = mock.Mock()
     area_mask = mock.Mock()
     counter = mock.Mock()
     nodes = Nodes(id=[])
     lines = Lines(id=[])
 
     quadtree.origin = (0.0, 0.0)
@@ -284,14 +283,20 @@
     grid_for_sorting.lines = grid_for_sorting.lines[:0]
     grid_for_sorting.pumps = grid_for_sorting.pumps[:0]
     grid_for_sorting.breaches = grid_for_sorting.breaches[:0]
 
     grid_for_sorting.sort()
 
 
+def test_sort_null_lines_err(grid_for_sorting):
+    grid_for_sorting.lines.line[0] = (-9999, 2)
+    with pytest.raises(ValueError):
+        grid_for_sorting.sort()
+
+
 def test_sort_boundary_conditions():
     grid = Grid(
         Nodes(
             id=[0, 1, 2, 3, 4, 5, 6],
             node_type=[
                 NodeType.NODE_2D_OPEN_WATER,
                 NodeType.NODE_1D_BOUNDARIES,
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_grid_refinements.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_grid_refinements.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_gridadmin.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_gridadmin.py`

 * *Files 3% similar despite different names*

```diff
@@ -289,36 +289,14 @@
     assert h5_out.attrs[attr].shape == shape
     actual = h5_out.attrs[attr].dtype
     if dtype == "S":
         actual = actual.char
     assert np.dtype(actual) == np.dtype(dtype)
 
 
-@pytest.mark.xfail
-@pytest.mark.parametrize(
-    "group,attr",
-    [
-        ("breaches", "prepared"),
-        ("levees", "prepared"),
-        ("lines", "channels_prepared"),
-        ("lines", "culverts_prepared"),
-        ("lines", "lines_prepared"),
-        ("lines", "orifices_prepared"),
-        ("lines", "pipes_prepared"),
-        ("lines", "weirs_prepared"),
-        ("nodes", "connectionnodes_prepared"),
-        ("nodes", "manholes_prepared"),
-        ("nodes", "prepared"),
-        ("pumps", "prepared"),
-    ],
-)  # [(x, y) for x in list(f) for y in list(f[x].attrs)]
-def test_write_sub_attrs(h5_out, group, attr):
-    assert h5_out[group].attrs[attr] == 1
-
-
 # obtained from bergermeer gridadmin.h5, edited:
 # - 20 pumps to 4
 # - int64 to int32
 @pytest.mark.parametrize(
     "dataset,shape,dtype",
     [
         ("bottom_level", (4,), "float64"),
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_groundwater.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_groundwater.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_initial_waterlevels.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_initial_waterlevels.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_linear.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_linear.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pytest
 import shapely
 from numpy.testing import assert_almost_equal, assert_array_equal
 from shapely.testing import assert_geometries_equal
 
-from threedigrid_builder.base import Array, Nodes, PointsOnLine
+from threedigrid_builder.base import Array, Lines, Nodes, PointsOnLine
 from threedigrid_builder.constants import CalculationType, ContentType, NodeType
 from threedigrid_builder.grid import ConnectionNodes, linear
 
 
 @pytest.fixture(scope="session")
 def random_lines():
     n_lines = 10  # approximate value
@@ -62,15 +62,15 @@
     display_name: str
     zoom_category: int
     material: int
     sewerage_type: int
 
 
 class LinearObjects(Array[LinearObject], linear.BaseLinear):
-    content_type = ContentType.TYPE_V2_CONNECTION_NODES  # just pick one for the test
+    content_type = ContentType.TYPE_V2_1D_LATERAL  # just pick one for the test
 
 
 @pytest.fixture
 def one_linear_object():
     return LinearObjects(
         the_geom=shapely.linestrings([[(0, 0), (6, 0), (6, 6)]]),
         dist_calc_points=np.array([5.0]),
@@ -134,15 +134,15 @@
     (dists,), _ = linestrings.segmentize().interpolate_points.call_args
     assert_almost_equal(dists, expected_dists)
 
     assert_array_equal(nodes.id, range(2, 2 + len(dummy_points)))
     assert_almost_equal(
         nodes.coordinates, shapely.get_coordinates(dummy_points.the_geom)
     )
-    assert_array_equal(nodes.content_type, ContentType.TYPE_V2_CONNECTION_NODES)
+    assert_array_equal(nodes.content_type, ContentType.TYPE_V2_1D_LATERAL)
     assert_array_equal(nodes.content_pk, [1, 1, 2])
     assert_array_equal(nodes.node_type, NodeType.NODE_1D_NO_STORAGE)
     assert_array_equal(nodes.calculation_type, [2, 2, 1])
     assert_array_equal(nodes.s1d, dummy_points.s1d)
 
 
 def test_interpolate_nodes_skips_embedded(two_linear_objects):
@@ -190,15 +190,15 @@
     assert_array_equal(arg.s1d, fixed_nodes.s1d)
 
     (dists,), _ = linestrings.segmentize().interpolate_points.call_args
     assert_almost_equal(dists, [5.0, 74.0, 74.0, 74.0])
 
     assert_array_equal(nodes.id, [2, 3, 4, 5])
     assert_almost_equal(nodes.coordinates, [(10, 0), (0, 30), (0, 50), (25, 100)])
-    assert_array_equal(nodes.content_type, ContentType.TYPE_V2_CONNECTION_NODES)
+    assert_array_equal(nodes.content_type, ContentType.TYPE_V2_1D_LATERAL)
     assert_array_equal(nodes.content_pk, [1, 2, 2, 2])
     assert_array_equal(nodes.calculation_type, [2, 1, 1, 1])
     assert_array_equal(nodes.s1d, [10.0, 30.0, 50.0, 125.0])
     assert_array_equal(
         nodes.breach_ids, [(-9999, -9999), (1, -9999), (2, 4), (-9999, -9999)]
     )
 
@@ -241,15 +241,15 @@
 
     expected_line = [(100, 10), (10, 103), (101, 11), (11, 12), (12, 102)]
     expected_centers = [5.0, 15.0, 25.0, 100.0, 175.0]
     expected_sizes = [10.0, 10.0, 50.0, 100.0, 50.0]
 
     assert_array_equal(lines.id, range(5))
     assert_array_equal(lines.line, expected_line)
-    assert_array_equal(lines.content_type, ContentType.TYPE_V2_CONNECTION_NODES)
+    assert_array_equal(lines.content_type, ContentType.TYPE_V2_1D_LATERAL)
     assert_array_equal(lines.content_pk, [1, 1, 2, 2, 2])
     assert_array_equal(lines.kcu, [2, 2, 1, 1, 1])
     assert_array_equal(lines.cross_id1, [17, 17, 18, 18, 18])
     assert_array_equal(lines.cross_id2, [17, 17, 18, 18, 18])
     assert_array_equal(lines.cross_weight, 1.0)
     assert_array_equal(lines.discharge_coefficient_positive, [0.8, 1.0, 0.5, 1.0, 1.0])
     assert_array_equal(lines.discharge_coefficient_negative, [1.0, 0.5, 1.0, 1.0, 0.8])
@@ -415,7 +415,24 @@
 def test_compute_drain_level_with_two_nan(two_linear_objects, connection_nodes):
     connection_nodes.drain_level[:] = [np.nan, 1.0, 1.0, np.nan]
     actual = two_linear_objects.compute_drain_level(
         [1, 2], [3.0, 4.0], connection_nodes
     )
 
     assert_almost_equal(actual, [np.nan, 1.0])
+
+
+@mock.patch.object(LinearObjects, "has_groundwater_exchange", np.array([False, True]))
+def test_apply_has_groundwater_exchange(two_linear_objects):
+    nodes = Nodes(
+        id=[1, 2, 3, 4],
+    )
+    lines = Lines(
+        id=range(3),
+        content_pk=[1, 2, 2],
+        content_type=LinearObjects.content_type,
+        line=[[2, 1], [1, 3], [3, 4]],
+    )
+
+    two_linear_objects.apply_has_groundwater_exchange(nodes, lines)
+
+    assert_array_equal(nodes.has_groundwater_exchange, [1, 0, 1, 1])
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_lines.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_lines.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_linestrings.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_linestrings.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_nodes.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_obstacles.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_obstacles.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_pipes.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_pipes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from unittest import mock
 
 import numpy as np
 import pytest
 import shapely
 from numpy.testing import assert_almost_equal, assert_array_equal
 
-from threedigrid_builder.base import Nodes
 from threedigrid_builder.grid import ConnectionNodes, Pipes
 
 
 @pytest.fixture
 def connection_nodes():
     # Used to map connection_node_start/end_id to an index (sequence id)
     return ConnectionNodes(
@@ -67,31 +66,55 @@
 )
 def test_compute_bottom_level_raises_out_of_bounds(pipe_ids, ds, pipes):
     pipes.the_geom = shapely.linestrings([[(0, 0), (0, 10)], [(2, 2), (3, 2)]])
     with pytest.raises(ValueError, match=".*outside of the linear object bounds.*"):
         pipes.compute_bottom_level(pipe_ids, ds)
 
 
-def test_1d2d_properties(pipes):
-    nodes = Nodes(
-        id=[0, 2, 5, 7],
-        content_pk=[1, 1, 2, 2],
-        s1d=[12.0, 13.0, 14.0, 15.0],
-    )
-    node_idx = [0, 1, 3]
-
+def test_get_1d2d_exchange_levels(pipes):
+    content_pk = np.array([1, 1, 2])
+    s1d = np.array([12.0, 13.0, 15.0])
     connection_nodes = mock.Mock()
 
     with mock.patch.object(pipes, "compute_drain_level") as compute_drain_level:
         compute_drain_level.return_value = np.array([1.8, 2.5, 3.2])
-        is_closed, dpumax = pipes.get_1d2d_properties(nodes, node_idx, connection_nodes)
+        actual = pipes.get_1d2d_exchange_levels(
+            content_pk=content_pk, s1d=s1d, connection_nodes=connection_nodes
+        )
 
         _, kwargs = compute_drain_level.call_args
-        assert_array_equal(kwargs["ids"], [1, 1, 2])  # the content pk
-        assert_array_equal(kwargs["s"], [12.0, 13.0, 15.0])  # the s1d
+        assert_array_equal(kwargs["ids"], content_pk)
+        assert_array_equal(kwargs["s"], s1d)
         assert kwargs["connection_nodes"] is connection_nodes
 
-    # pipes are closed
-    assert_array_equal(is_closed, True)
-
     # interpolation between manhole drain levels is further tested elsewhere
-    assert_array_equal(dpumax, [1.8, 2.5, 3.2])
+    assert_array_equal(actual, compute_drain_level.return_value)
+
+
+def test_is_closed(pipes):
+    actual = pipes.is_closed(np.array([1, 3]))
+
+    assert_array_equal(actual, [True, True])
+
+
+@pytest.mark.parametrize(
+    "thickness,hc_out,hc_in,expected",
+    [
+        (0.1, 3.0, 2.0, True),
+        (0.0, 3.0, 2.0, False),
+        (np.nan, 3.0, 2.0, False),
+        (0.1, np.nan, 2.0, False),
+        (0.1, 3.0, np.nan, False),
+    ],
+)
+def test_has_groundwater_exchange(thickness, hc_out, hc_in, expected):
+    pipes = Pipes(
+        id=[1],
+        exchange_thickness=thickness,
+        hydraulic_conductivity_out=hc_out,
+        hydraulic_conductivity_in=hc_in,
+    )
+
+    actual = pipes.has_groundwater_exchange
+
+    assert len(actual) == 1
+    assert actual[0] == expected
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_potential_breaches.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_potential_breaches.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_quadtree.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_quadtree.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_raster_interfaces.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_raster_interfaces.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_structures.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_structures.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from unittest import mock
 
 import numpy as np
 import pytest
 import shapely
 from numpy.testing import assert_almost_equal, assert_array_equal
 
-from threedigrid_builder.base import Nodes
 from threedigrid_builder.constants import ContentType
 from threedigrid_builder.grid import ConnectionNodes, Culverts, Orifices, Weirs
 
 
 @pytest.fixture
 def connection_nodes():
     # Used to map connection_node_start/end_id to an index (sequence id)
@@ -116,33 +115,31 @@
 )
 def test_culverts_compute_bottom_level_raises_out_of_bounds(culvert_ids, ds, culverts):
     culverts.the_geom = shapely.linestrings([[(0, 0), (0, 10)], [(2, 2), (3, 2)]])
     with pytest.raises(ValueError, match=".*outside of the linear object bounds.*"):
         culverts.compute_bottom_level(culvert_ids, ds)
 
 
-def test_culverts_1d2d_properties(culverts):
-    nodes = Nodes(
-        id=[0, 2, 5, 7],
-        content_pk=[1, 1, 2, 2],
-        s1d=[12.0, 13.0, 14.0, 15.0],
-    )
-    node_idx = [0, 1, 3]
-
+def test_culverts_get_1d2d_exchange_levels(culverts):
+    content_pk = np.array([1, 1, 2])
+    s1d = np.array([12.0, 13.0, 15.0])
     connection_nodes = mock.Mock()
 
     with mock.patch.object(culverts, "compute_drain_level") as compute_drain_level:
         compute_drain_level.return_value = np.array([1.8, 2.5, 3.2])
-        is_closed, dpumax = culverts.get_1d2d_properties(
-            nodes, node_idx, connection_nodes
+        actual = culverts.get_1d2d_exchange_levels(
+            content_pk=content_pk, s1d=s1d, connection_nodes=connection_nodes
         )
 
         _, kwargs = compute_drain_level.call_args
-        assert_array_equal(kwargs["ids"], [1, 1, 2])  # the content pk
-        assert_array_equal(kwargs["s"], [12.0, 13.0, 15.0])  # the s1d
+        assert_array_equal(kwargs["ids"], content_pk)
+        assert_array_equal(kwargs["s"], s1d)
         assert kwargs["connection_nodes"] is connection_nodes
 
-    # culverts are closed
-    assert_array_equal(is_closed, True)
-
     # interpolation between manhole drain levels is further tested elsewhere
-    assert_array_equal(dpumax, [1.8, 2.5, 3.2])
+    assert_array_equal(actual, compute_drain_level.return_value)
+
+
+def test_is_closed(culverts):
+    actual = culverts.is_closed(np.array([1, 3]))
+
+    assert_array_equal(actual, [True, True])
```

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_windshielding.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_windshielding.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder/tests/test_zero_d.py` & `threedigrid-builder-1.9.0/threedigrid_builder/tests/test_zero_d.py`

 * *Files identical despite different names*

### Comparing `threedigrid-builder-1.8.0/threedigrid_builder.egg-info/SOURCES.txt` & `threedigrid-builder-1.9.0/threedigrid_builder.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 threedigrid_builder.egg-info/dependency_links.txt
 threedigrid_builder.egg-info/entry_points.txt
 threedigrid_builder.egg-info/not-zip-safe
 threedigrid_builder.egg-info/requires.txt
 threedigrid_builder.egg-info/top_level.txt
 threedigrid_builder/base/__init__.py
 threedigrid_builder/base/array.py
-threedigrid_builder/base/endpoints.py
 threedigrid_builder/base/interfaces.py
+threedigrid_builder/base/line_halfs.py
 threedigrid_builder/base/lines.py
 threedigrid_builder/base/linestrings.py
 threedigrid_builder/base/nodes.py
 threedigrid_builder/base/pumps.py
 threedigrid_builder/base/settings.py
 threedigrid_builder/base/surfaces.py
 threedigrid_builder/grid/__init__.py
@@ -43,14 +43,15 @@
 threedigrid_builder/grid/embedded.py
 threedigrid_builder/grid/exchange_lines.py
 threedigrid_builder/grid/grid.py
 threedigrid_builder/grid/grid_refinement.py
 threedigrid_builder/grid/groundwater.py
 threedigrid_builder/grid/initial_waterlevels.py
 threedigrid_builder/grid/linear.py
+threedigrid_builder/grid/lines_1d2d.py
 threedigrid_builder/grid/obstacles.py
 threedigrid_builder/grid/pipes.py
 threedigrid_builder/grid/potential_breaches.py
 threedigrid_builder/grid/quadtree.py
 threedigrid_builder/grid/structures.py
 threedigrid_builder/grid/windshielding.py
 threedigrid_builder/grid/zero_d.py
@@ -69,23 +70,24 @@
 threedigrid_builder/tests/test_connection_nodes.py
 threedigrid_builder/tests/test_cross_section_definitions.py
 threedigrid_builder/tests/test_cross_section_locations.py
 threedigrid_builder/tests/test_db.py
 threedigrid_builder/tests/test_dem_average.py
 threedigrid_builder/tests/test_dict_out.py
 threedigrid_builder/tests/test_embedded.py
-threedigrid_builder/tests/test_endpoints.py
 threedigrid_builder/tests/test_exchange_lines.py
 threedigrid_builder/tests/test_grid.py
 threedigrid_builder/tests/test_grid_refinements.py
 threedigrid_builder/tests/test_gridadmin.py
 threedigrid_builder/tests/test_groundwater.py
 threedigrid_builder/tests/test_initial_waterlevels.py
+threedigrid_builder/tests/test_line_halfs.py
 threedigrid_builder/tests/test_linear.py
 threedigrid_builder/tests/test_lines.py
+threedigrid_builder/tests/test_lines_1d2d.py
 threedigrid_builder/tests/test_linestrings.py
 threedigrid_builder/tests/test_nodes.py
 threedigrid_builder/tests/test_obstacles.py
 threedigrid_builder/tests/test_pipes.py
 threedigrid_builder/tests/test_potential_breaches.py
 threedigrid_builder/tests/test_pumps.py
 threedigrid_builder/tests/test_quadtree.py
```

