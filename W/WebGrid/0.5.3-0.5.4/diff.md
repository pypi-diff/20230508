# Comparing `tmp/WebGrid-0.5.3.tar.gz` & `tmp/WebGrid-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebGrid-0.5.3.tar", last modified: Thu Mar  2 19:26:50 2023, max compression
+gzip compressed data, was "WebGrid-0.5.4.tar", last modified: Mon May  8 14:10:51 2023, max compression
```

## Comparing `WebGrid-0.5.3.tar` & `WebGrid-0.5.4.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.141039 WebGrid-0.5.3/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       94 2018-11-14 14:19:49.000000 WebGrid-0.5.3/MANIFEST.in
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26280 2023-03-02 19:26:50.141039 WebGrid-0.5.3/PKG-INFO
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/WebGrid.egg-info/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26280 2023-03-02 19:26:49.000000 WebGrid-0.5.3/WebGrid.egg-info/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2363 2023-03-02 19:26:50.000000 WebGrid-0.5.3/WebGrid.egg-info/SOURCES.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-03-02 19:26:49.000000 WebGrid-0.5.3/WebGrid.egg-info/dependency_links.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       62 2023-03-02 19:26:49.000000 WebGrid-0.5.3/WebGrid.egg-info/entry_points.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2017-06-09 12:44:59.000000 WebGrid-0.5.3/WebGrid.egg-info/not-zip-safe
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      352 2023-03-02 19:26:49.000000 WebGrid-0.5.3/WebGrid.egg-info/requires.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        8 2023-03-02 19:26:49.000000 WebGrid-0.5.3/WebGrid.egg-info/top_level.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    23423 2023-03-02 19:26:33.000000 WebGrid-0.5.3/changelog.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2191 2021-02-01 15:18:26.000000 WebGrid-0.5.3/readme.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      504 2023-03-02 19:26:50.141039 WebGrid-0.5.3/setup.cfg
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2188 2023-03-02 18:13:49.000000 WebGrid-0.5.3/setup.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    69063 2023-03-02 19:26:02.000000 WebGrid-0.5.3/webgrid/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2404 2021-09-10 16:32:05.000000 WebGrid-0.5.3/webgrid/blazeweb.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19193 2022-11-07 21:26:35.000000 WebGrid-0.5.3/webgrid/extensions.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    65251 2023-01-21 00:19:49.000000 WebGrid-0.5.3/webgrid/filters.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11174 2022-07-25 15:25:24.000000 WebGrid-0.5.3/webgrid/flask.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/i18n/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      114 2018-11-14 14:19:49.000000 WebGrid-0.5.3/webgrid/i18n/babel.cfg
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5320 2023-01-21 00:19:49.000000 WebGrid-0.5.3/webgrid/i18n/es/LC_MESSAGES/webgrid.mo
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9220 2023-01-21 00:19:49.000000 WebGrid-0.5.3/webgrid/i18n/es/LC_MESSAGES/webgrid.po
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7103 2023-01-21 00:19:49.000000 WebGrid-0.5.3/webgrid/i18n/webgrid.pot
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    62177 2023-02-24 14:00:14.000000 WebGrid-0.5.3/webgrid/renderers.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/static/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      714 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/application_form_edit.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      238 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/b_firstpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      236 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/b_lastpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      221 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/b_nextpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      225 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/b_prevpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      238 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/bd_firstpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      236 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/bd_lastpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      221 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/bd_nextpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      225 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/bd_prevpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      715 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/delete.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3430 2018-11-14 14:19:49.000000 WebGrid-0.5.3/webgrid/static/gettext.min.js
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/static/i18n/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/static/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/static/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4694 2023-01-21 00:19:49.000000 WebGrid-0.5.3/webgrid/static/i18n/es/LC_MESSAGES/webgrid.json
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    14611 2019-11-26 15:27:36.000000 WebGrid-0.5.3/webgrid/static/jquery.multiple.select.js
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4149 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/multiple-select.css
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3342 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/multiple-select.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      528 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/th_arrow_down.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      514 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/static/th_arrow_up.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6503 2020-12-09 21:12:41.000000 WebGrid-0.5.3/webgrid/static/webgrid.css
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    16355 2022-12-12 16:06:22.000000 WebGrid-0.5.3/webgrid/static/webgrid.js
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/templates/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      570 2020-05-15 19:26:27.000000 WebGrid-0.5.3/webgrid/templates/grid.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2101 2023-01-20 13:59:08.000000 WebGrid-0.5.3/webgrid/templates/grid_footer.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1180 2021-09-10 16:32:05.000000 WebGrid-0.5.3/webgrid/templates/grid_header.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      388 2020-05-15 19:26:27.000000 WebGrid-0.5.3/webgrid/templates/grid_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      351 2020-11-04 20:29:48.000000 WebGrid-0.5.3/webgrid/templates/header_filtering.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      517 2020-10-09 20:16:24.000000 WebGrid-0.5.3/webgrid/templates/header_paging.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      331 2020-10-09 20:16:24.000000 WebGrid-0.5.3/webgrid/templates/header_sorting.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19686 2023-01-20 13:59:08.000000 WebGrid-0.5.3/webgrid/testing.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/tests/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid/tests/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      271 2021-09-10 16:32:05.000000 WebGrid-0.5.3/webgrid/tests/conftest.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid/tests/data/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1483 2020-10-09 20:16:24.000000 WebGrid-0.5.3/webgrid/tests/data/basic_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1788 2019-09-04 13:29:02.000000 WebGrid-0.5.3/webgrid/tests/data/people_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4262 2020-04-09 13:05:21.000000 WebGrid-0.5.3/webgrid/tests/data/stopwatch_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1532 2021-09-10 16:32:05.000000 WebGrid-0.5.3/webgrid/tests/helpers.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     8796 2022-10-18 13:32:21.000000 WebGrid-0.5.3/webgrid/tests/test_api.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    13006 2023-03-02 19:26:02.000000 WebGrid-0.5.3/webgrid/tests/test_columns.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    75691 2023-01-21 00:19:49.000000 WebGrid-0.5.3/webgrid/tests/test_filters.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    50216 2023-02-24 14:00:14.000000 WebGrid-0.5.3/webgrid/tests/test_rendering.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7880 2023-01-20 13:59:08.000000 WebGrid-0.5.3/webgrid/tests/test_testing.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3123 2023-02-24 14:00:14.000000 WebGrid-0.5.3/webgrid/tests/test_types.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    48965 2023-01-20 13:59:08.000000 WebGrid-0.5.3/webgrid/tests/test_unit.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3882 2022-10-18 13:32:21.000000 WebGrid-0.5.3/webgrid/types.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1845 2018-11-14 14:19:49.000000 WebGrid-0.5.3/webgrid/utils.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-03-02 19:26:26.000000 WebGrid-0.5.3/webgrid/version.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.141039 WebGrid-0.5.3/webgrid_ta/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid_ta/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1644 2021-09-10 16:32:05.000000 WebGrid-0.5.3/webgrid_ta/app.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.141039 WebGrid-0.5.3/webgrid_ta/data/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1479 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid_ta/data/basic_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1634 2017-06-09 12:44:51.000000 WebGrid-0.5.3/webgrid_ta/data/people_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      980 2018-11-14 14:19:49.000000 WebGrid-0.5.3/webgrid_ta/extensions.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5073 2023-01-20 13:59:08.000000 WebGrid-0.5.3/webgrid_ta/grids.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2030 2021-09-10 16:32:05.000000 WebGrid-0.5.3/webgrid_ta/helpers.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.141039 WebGrid-0.5.3/webgrid_ta/i18n/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      114 2018-11-14 14:19:49.000000 WebGrid-0.5.3/webgrid_ta/i18n/babel.cfg
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.137039 WebGrid-0.5.3/webgrid_ta/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.141039 WebGrid-0.5.3/webgrid_ta/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1336 2018-11-14 14:19:49.000000 WebGrid-0.5.3/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.mo
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2255 2018-11-14 14:19:49.000000 WebGrid-0.5.3/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.po
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1897 2018-11-14 14:19:49.000000 WebGrid-0.5.3/webgrid_ta/i18n/webgrid_ta.pot
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1382 2021-09-10 16:32:05.000000 WebGrid-0.5.3/webgrid_ta/manage.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.141039 WebGrid-0.5.3/webgrid_ta/model/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1704 2020-04-09 13:05:21.000000 WebGrid-0.5.3/webgrid_ta/model/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4307 2023-02-24 14:00:14.000000 WebGrid-0.5.3/webgrid_ta/model/entities.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    17708 2020-01-10 14:33:11.000000 WebGrid-0.5.3/webgrid_ta/model/helpers.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 19:26:50.141039 WebGrid-0.5.3/webgrid_ta/templates/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      829 2020-04-09 13:05:21.000000 WebGrid-0.5.3/webgrid_ta/templates/groups.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1772 2018-11-14 14:19:49.000000 WebGrid-0.5.3/webgrid_ta/templates/index.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1080 2020-10-09 20:16:24.000000 WebGrid-0.5.3/webgrid_ta/views.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.830541 WebGrid-0.5.4/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       94 2018-11-14 14:19:49.000000 WebGrid-0.5.4/MANIFEST.in
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26462 2023-05-08 14:10:51.830541 WebGrid-0.5.4/PKG-INFO
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.802541 WebGrid-0.5.4/WebGrid.egg-info/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26462 2023-05-08 14:10:51.000000 WebGrid-0.5.4/WebGrid.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2363 2023-05-08 14:10:51.000000 WebGrid-0.5.4/WebGrid.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-08 14:10:51.000000 WebGrid-0.5.4/WebGrid.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       62 2023-05-08 14:10:51.000000 WebGrid-0.5.4/WebGrid.egg-info/entry_points.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2017-06-09 12:44:59.000000 WebGrid-0.5.4/WebGrid.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      352 2023-05-08 14:10:51.000000 WebGrid-0.5.4/WebGrid.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        8 2023-05-08 14:10:51.000000 WebGrid-0.5.4/WebGrid.egg-info/top_level.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    23605 2023-05-08 14:10:35.000000 WebGrid-0.5.4/changelog.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2191 2021-02-01 15:18:26.000000 WebGrid-0.5.4/readme.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      504 2023-05-08 14:10:51.830541 WebGrid-0.5.4/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2188 2023-03-02 18:13:49.000000 WebGrid-0.5.4/setup.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.810541 WebGrid-0.5.4/webgrid/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    69063 2023-03-02 19:26:02.000000 WebGrid-0.5.4/webgrid/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2404 2021-09-10 16:32:05.000000 WebGrid-0.5.4/webgrid/blazeweb.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19193 2022-11-07 21:26:35.000000 WebGrid-0.5.4/webgrid/extensions.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    65646 2023-05-08 14:09:53.000000 WebGrid-0.5.4/webgrid/filters.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11174 2022-07-25 15:25:24.000000 WebGrid-0.5.4/webgrid/flask.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.810541 WebGrid-0.5.4/webgrid/i18n/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      114 2018-11-14 14:19:49.000000 WebGrid-0.5.4/webgrid/i18n/babel.cfg
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.794541 WebGrid-0.5.4/webgrid/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.814541 WebGrid-0.5.4/webgrid/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5320 2023-01-21 00:19:49.000000 WebGrid-0.5.4/webgrid/i18n/es/LC_MESSAGES/webgrid.mo
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9220 2023-01-21 00:19:49.000000 WebGrid-0.5.4/webgrid/i18n/es/LC_MESSAGES/webgrid.po
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7103 2023-01-21 00:19:49.000000 WebGrid-0.5.4/webgrid/i18n/webgrid.pot
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    62177 2023-02-24 14:00:14.000000 WebGrid-0.5.4/webgrid/renderers.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.818541 WebGrid-0.5.4/webgrid/static/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      714 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/application_form_edit.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      238 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/b_firstpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      236 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/b_lastpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      221 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/b_nextpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      225 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/b_prevpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      238 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/bd_firstpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      236 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/bd_lastpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      221 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/bd_nextpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      225 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/bd_prevpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      715 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/delete.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3430 2018-11-14 14:19:49.000000 WebGrid-0.5.4/webgrid/static/gettext.min.js
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.794541 WebGrid-0.5.4/webgrid/static/i18n/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.794541 WebGrid-0.5.4/webgrid/static/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.818541 WebGrid-0.5.4/webgrid/static/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4694 2023-01-21 00:19:49.000000 WebGrid-0.5.4/webgrid/static/i18n/es/LC_MESSAGES/webgrid.json
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    14611 2019-11-26 15:27:36.000000 WebGrid-0.5.4/webgrid/static/jquery.multiple.select.js
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4149 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/multiple-select.css
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3342 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/multiple-select.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      528 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/th_arrow_down.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      514 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/static/th_arrow_up.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6503 2020-12-09 21:12:41.000000 WebGrid-0.5.4/webgrid/static/webgrid.css
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    16355 2022-12-12 16:06:22.000000 WebGrid-0.5.4/webgrid/static/webgrid.js
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.818541 WebGrid-0.5.4/webgrid/templates/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      570 2020-05-15 19:26:27.000000 WebGrid-0.5.4/webgrid/templates/grid.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2101 2023-01-20 13:59:08.000000 WebGrid-0.5.4/webgrid/templates/grid_footer.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1180 2021-09-10 16:32:05.000000 WebGrid-0.5.4/webgrid/templates/grid_header.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      388 2020-05-15 19:26:27.000000 WebGrid-0.5.4/webgrid/templates/grid_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      351 2020-11-04 20:29:48.000000 WebGrid-0.5.4/webgrid/templates/header_filtering.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      517 2020-10-09 20:16:24.000000 WebGrid-0.5.4/webgrid/templates/header_paging.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      331 2020-10-09 20:16:24.000000 WebGrid-0.5.4/webgrid/templates/header_sorting.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19686 2023-01-20 13:59:08.000000 WebGrid-0.5.4/webgrid/testing.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.822541 WebGrid-0.5.4/webgrid/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid/tests/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      271 2021-09-10 16:32:05.000000 WebGrid-0.5.4/webgrid/tests/conftest.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.822541 WebGrid-0.5.4/webgrid/tests/data/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1483 2020-10-09 20:16:24.000000 WebGrid-0.5.4/webgrid/tests/data/basic_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1788 2019-09-04 13:29:02.000000 WebGrid-0.5.4/webgrid/tests/data/people_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4262 2020-04-09 13:05:21.000000 WebGrid-0.5.4/webgrid/tests/data/stopwatch_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1532 2021-09-10 16:32:05.000000 WebGrid-0.5.4/webgrid/tests/helpers.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     8796 2022-10-18 13:32:21.000000 WebGrid-0.5.4/webgrid/tests/test_api.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    13006 2023-03-02 19:26:02.000000 WebGrid-0.5.4/webgrid/tests/test_columns.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    76066 2023-05-08 14:09:53.000000 WebGrid-0.5.4/webgrid/tests/test_filters.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    50216 2023-02-24 14:00:14.000000 WebGrid-0.5.4/webgrid/tests/test_rendering.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7880 2023-01-20 13:59:08.000000 WebGrid-0.5.4/webgrid/tests/test_testing.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3123 2023-02-24 14:00:14.000000 WebGrid-0.5.4/webgrid/tests/test_types.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    48965 2023-01-20 13:59:08.000000 WebGrid-0.5.4/webgrid/tests/test_unit.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3882 2022-10-18 13:32:21.000000 WebGrid-0.5.4/webgrid/types.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1845 2018-11-14 14:19:49.000000 WebGrid-0.5.4/webgrid/utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-05-08 14:10:08.000000 WebGrid-0.5.4/webgrid/version.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.826541 WebGrid-0.5.4/webgrid_ta/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid_ta/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1644 2021-09-10 16:32:05.000000 WebGrid-0.5.4/webgrid_ta/app.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.826541 WebGrid-0.5.4/webgrid_ta/data/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1479 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid_ta/data/basic_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1634 2017-06-09 12:44:51.000000 WebGrid-0.5.4/webgrid_ta/data/people_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      980 2018-11-14 14:19:49.000000 WebGrid-0.5.4/webgrid_ta/extensions.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5073 2023-01-20 13:59:08.000000 WebGrid-0.5.4/webgrid_ta/grids.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2030 2021-09-10 16:32:05.000000 WebGrid-0.5.4/webgrid_ta/helpers.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.826541 WebGrid-0.5.4/webgrid_ta/i18n/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      114 2018-11-14 14:19:49.000000 WebGrid-0.5.4/webgrid_ta/i18n/babel.cfg
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.798541 WebGrid-0.5.4/webgrid_ta/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.826541 WebGrid-0.5.4/webgrid_ta/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1336 2018-11-14 14:19:49.000000 WebGrid-0.5.4/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.mo
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2255 2018-11-14 14:19:49.000000 WebGrid-0.5.4/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.po
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1897 2018-11-14 14:19:49.000000 WebGrid-0.5.4/webgrid_ta/i18n/webgrid_ta.pot
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1382 2021-09-10 16:32:05.000000 WebGrid-0.5.4/webgrid_ta/manage.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.826541 WebGrid-0.5.4/webgrid_ta/model/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1704 2020-04-09 13:05:21.000000 WebGrid-0.5.4/webgrid_ta/model/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4307 2023-02-24 14:00:14.000000 WebGrid-0.5.4/webgrid_ta/model/entities.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    17708 2020-01-10 14:33:11.000000 WebGrid-0.5.4/webgrid_ta/model/helpers.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-08 14:10:51.830541 WebGrid-0.5.4/webgrid_ta/templates/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      829 2020-04-09 13:05:21.000000 WebGrid-0.5.4/webgrid_ta/templates/groups.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1772 2018-11-14 14:19:49.000000 WebGrid-0.5.4/webgrid_ta/templates/index.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1080 2020-10-09 20:16:24.000000 WebGrid-0.5.4/webgrid_ta/views.py
```

### Comparing `WebGrid-0.5.3/PKG-INFO` & `WebGrid-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebGrid
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library for rendering HTML tables and Excel files from SQLAlchemy models.
 Home-page: https://github.com/level12/webgrid
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -84,14 +84,22 @@
 * Issue tracker: https://github.com/level12/webgrid/issues
 * Questions & comments: http://groups.google.com/group/blazelibs
 
 
 Changelog
 =========
 
+0.5.4 released 2023-05-08
+-------------------------
+
+- match datetime filter granularity to filter input (029d7e3_)
+
+.. _029d7e3: https://github.com/level12/webgrid/commit/029d7e3
+
+
 0.5.3 released 2023-03-02
 -------------------------
 
 - fix column attribute extraction for non-SQLAlchemy records (a090491_)
 
 .. _a090491: https://github.com/level12/webgrid/commit/a090491
```

### Comparing `WebGrid-0.5.3/WebGrid.egg-info/PKG-INFO` & `WebGrid-0.5.4/WebGrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebGrid
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library for rendering HTML tables and Excel files from SQLAlchemy models.
 Home-page: https://github.com/level12/webgrid
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -84,14 +84,22 @@
 * Issue tracker: https://github.com/level12/webgrid/issues
 * Questions & comments: http://groups.google.com/group/blazelibs
 
 
 Changelog
 =========
 
+0.5.4 released 2023-05-08
+-------------------------
+
+- match datetime filter granularity to filter input (029d7e3_)
+
+.. _029d7e3: https://github.com/level12/webgrid/commit/029d7e3
+
+
 0.5.3 released 2023-03-02
 -------------------------
 
 - fix column attribute extraction for non-SQLAlchemy records (a090491_)
 
 .. _a090491: https://github.com/level12/webgrid/commit/a090491
```

### Comparing `WebGrid-0.5.3/WebGrid.egg-info/SOURCES.txt` & `WebGrid-0.5.4/WebGrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/changelog.rst` & `WebGrid-0.5.4/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.5.4 released 2023-05-08
+-------------------------
+
+- match datetime filter granularity to filter input (029d7e3_)
+
+.. _029d7e3: https://github.com/level12/webgrid/commit/029d7e3
+
+
 0.5.3 released 2023-03-02
 -------------------------
 
 - fix column attribute extraction for non-SQLAlchemy records (a090491_)
 
 .. _a090491: https://github.com/level12/webgrid/commit/a090491
```

### Comparing `WebGrid-0.5.3/readme.rst` & `WebGrid-0.5.4/readme.rst`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/setup.py` & `WebGrid-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/__init__.py` & `WebGrid-0.5.4/webgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/blazeweb.py` & `WebGrid-0.5.4/webgrid/blazeweb.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/extensions.py` & `WebGrid-0.5.4/webgrid/extensions.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/filters.py` & `WebGrid-0.5.4/webgrid/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1416,24 +1416,30 @@
                 # !!!: localize
                 self.value2_set_with = self.value2.strftime('%Y-%m-%dT23:59')
 
     def _between_clause(self):
         if self._has_date_only2:
             right_side = ensure_datetime(self.value2.date(),
                                          time_part=dt.time(23, 59, 59, 999999))
+        elif self.value2.second == 0 and self.value2.microsecond == 0:
+            right_side = self.value2 + dt.timedelta(seconds=59, microseconds=999999)
         else:
             right_side = self.value2
         return self.sa_col.between(ensure_datetime(self.value1), right_side)
 
     def _eq_clause(self):
         if self._has_date_only1:
             left_side = ensure_datetime(self.value1.date())
             right_side = ensure_datetime(self.value1.date(), time_part=dt.time(23, 59, 59, 999999))
             return self.sa_col.between(left_side, right_side)
-        if self.value1 and self.value1.microsecond == 0:
+        elif self.value1 and self.value1.second == 0:
+            left_side = self.value1
+            right_side = self.value1 + dt.timedelta(seconds=59, microseconds=999999)
+            return self.sa_col.between(left_side, right_side)
+        elif self.value1 and self.value1.microsecond == 0:
             left_side = self.value1
             right_side = self.value1 + dt.timedelta(microseconds=999999)
             return self.sa_col.between(left_side, right_side)
 
     def _process_datetime(self, value, is_value2):
         try:
             dt_value = parse(value)
```

### Comparing `WebGrid-0.5.3/webgrid/flask.py` & `WebGrid-0.5.4/webgrid/flask.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/i18n/es/LC_MESSAGES/webgrid.mo` & `WebGrid-0.5.4/webgrid/i18n/es/LC_MESSAGES/webgrid.mo`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/i18n/es/LC_MESSAGES/webgrid.po` & `WebGrid-0.5.4/webgrid/i18n/es/LC_MESSAGES/webgrid.po`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/i18n/webgrid.pot` & `WebGrid-0.5.4/webgrid/i18n/webgrid.pot`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/renderers.py` & `WebGrid-0.5.4/webgrid/renderers.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/application_form_edit.png` & `WebGrid-0.5.4/webgrid/static/application_form_edit.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/delete.png` & `WebGrid-0.5.4/webgrid/static/delete.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/gettext.min.js` & `WebGrid-0.5.4/webgrid/static/gettext.min.js`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/i18n/es/LC_MESSAGES/webgrid.json` & `WebGrid-0.5.4/webgrid/static/i18n/es/LC_MESSAGES/webgrid.json`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/jquery.multiple.select.js` & `WebGrid-0.5.4/webgrid/static/jquery.multiple.select.js`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/multiple-select.css` & `WebGrid-0.5.4/webgrid/static/multiple-select.css`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/multiple-select.png` & `WebGrid-0.5.4/webgrid/static/multiple-select.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/th_arrow_down.png` & `WebGrid-0.5.4/webgrid/static/th_arrow_down.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/th_arrow_up.png` & `WebGrid-0.5.4/webgrid/static/th_arrow_up.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/webgrid.css` & `WebGrid-0.5.4/webgrid/static/webgrid.css`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/static/webgrid.js` & `WebGrid-0.5.4/webgrid/static/webgrid.js`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/templates/grid.html` & `WebGrid-0.5.4/webgrid/templates/grid.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/templates/grid_footer.html` & `WebGrid-0.5.4/webgrid/templates/grid_footer.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/templates/grid_header.html` & `WebGrid-0.5.4/webgrid/templates/grid_header.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/templates/header_paging.html` & `WebGrid-0.5.4/webgrid/templates/header_paging.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/testing.py` & `WebGrid-0.5.4/webgrid/testing.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/data/basic_table.html` & `WebGrid-0.5.4/webgrid/tests/data/basic_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/data/people_table.html` & `WebGrid-0.5.4/webgrid/tests/data/people_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/data/stopwatch_table.html` & `WebGrid-0.5.4/webgrid/tests/data/stopwatch_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/helpers.py` & `WebGrid-0.5.4/webgrid/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/test_api.py` & `WebGrid-0.5.4/webgrid/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/test_columns.py` & `WebGrid-0.5.4/webgrid/tests/test_columns.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/test_filters.py` & `WebGrid-0.5.4/webgrid/tests/test_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -952,14 +952,23 @@
         filter.set('eq', '12/31/2010 10:26:27')
         self.assert_filter_query(
             filter,
             "WHERE persons.createdts BETWEEN '2010-12-31 10:26:27.000000' AND "
             "'2010-12-31 10:26:27.999999'")
         assert filter.value1_set_with == '2010-12-31T10:26'
 
+    def test_eq_with_time_minutes(self):
+        filter = DateTimeFilter(Person.createdts)
+        filter.set('eq', '12/31/2010 10:26')
+        self.assert_filter_query(
+            filter,
+            "WHERE persons.createdts BETWEEN '2010-12-31 10:26:00.000000' AND "
+            "'2010-12-31 10:26:59.999999'")
+        assert filter.value1_set_with == '2010-12-31T10:26'
+
     def test_not_eq(self):
         filter = DateTimeFilter(Person.createdts)
         filter.set('!eq', '12/31/2010')
         self.assert_filter_query(
             filter,
             "WHERE persons.createdts NOT BETWEEN '2010-12-31 00:00:00.000000' AND "
             "'2010-12-31 23:59:59.999999'")
@@ -1131,15 +1140,15 @@
 
     def test_between_with_explicit_midnight(self):
         filter = DateTimeFilter(Person.createdts)
         filter.set('between', '1/31/2010 10:00', '12/31/2010 00:00')
         self.assert_filter_query(
             filter,
             "WHERE persons.createdts BETWEEN '2010-01-31 10:00:00.000000' AND "
-            "'2010-12-31 00:00:00.000000'")
+            "'2010-12-31 00:00:59.999999'")
 
     def test_not_between(self):
         filter = DateTimeFilter(Person.createdts)
         filter.set('!between', '1/31/2010', '12/31/2010')
         assert filter.error is False
         self.assert_filter_query(
             filter,
```

### Comparing `WebGrid-0.5.3/webgrid/tests/test_rendering.py` & `WebGrid-0.5.4/webgrid/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/test_testing.py` & `WebGrid-0.5.4/webgrid/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/test_types.py` & `WebGrid-0.5.4/webgrid/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/tests/test_unit.py` & `WebGrid-0.5.4/webgrid/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/types.py` & `WebGrid-0.5.4/webgrid/types.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid/utils.py` & `WebGrid-0.5.4/webgrid/utils.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/app.py` & `WebGrid-0.5.4/webgrid_ta/app.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/data/basic_table.html` & `WebGrid-0.5.4/webgrid_ta/data/basic_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/data/people_table.html` & `WebGrid-0.5.4/webgrid_ta/data/people_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/extensions.py` & `WebGrid-0.5.4/webgrid_ta/extensions.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/grids.py` & `WebGrid-0.5.4/webgrid_ta/grids.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/helpers.py` & `WebGrid-0.5.4/webgrid_ta/helpers.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.mo` & `WebGrid-0.5.4/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.mo`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.po` & `WebGrid-0.5.4/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.po`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/i18n/webgrid_ta.pot` & `WebGrid-0.5.4/webgrid_ta/i18n/webgrid_ta.pot`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/manage.py` & `WebGrid-0.5.4/webgrid_ta/manage.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/model/__init__.py` & `WebGrid-0.5.4/webgrid_ta/model/__init__.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/model/entities.py` & `WebGrid-0.5.4/webgrid_ta/model/entities.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/model/helpers.py` & `WebGrid-0.5.4/webgrid_ta/model/helpers.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/templates/groups.html` & `WebGrid-0.5.4/webgrid_ta/templates/groups.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/templates/index.html` & `WebGrid-0.5.4/webgrid_ta/templates/index.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.3/webgrid_ta/views.py` & `WebGrid-0.5.4/webgrid_ta/views.py`

 * *Files identical despite different names*

