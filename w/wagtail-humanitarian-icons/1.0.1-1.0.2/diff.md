# Comparing `tmp/wagtail-humanitarian-icons-1.0.1.tar.gz` & `tmp/wagtail-humanitarian-icons-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-humanitarian-icons-1.0.1.tar", last modified: Mon May  8 09:37:24 2023, max compression
+gzip compressed data, was "wagtail-humanitarian-icons-1.0.2.tar", last modified: Mon May  8 09:45:37 2023, max compression
```

## Comparing `wagtail-humanitarian-icons-1.0.1.tar` & `wagtail-humanitarian-icons-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,411 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:24.195824 wagtail-humanitarian-icons-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-08 09:37:24.195824 wagtail-humanitarian-icons-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 09:37:24.199824 wagtail-humanitarian-icons-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:24.191823 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 09:37:24.000000 wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:24.195824 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/icons.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:24.195824 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-08 09:37:05.000000 wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:37.936879 wagtail-humanitarian-icons-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-08 09:45:37.936879 wagtail-humanitarian-icons-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-08 09:45:37.936879 wagtail-humanitarian-icons-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:37.852876 wagtail-humanitarian-icons-1.0.2/wagtail_humanitarian_icons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-08 09:45:37.000000 wagtail-humanitarian-icons-1.0.2/wagtail_humanitarian_icons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32119 2023-05-08 09:45:37.000000 wagtail-humanitarian-icons-1.0.2/wagtail_humanitarian_icons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:45:37.000000 wagtail-humanitarian-icons-1.0.2/wagtail_humanitarian_icons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 09:45:37.000000 wagtail-humanitarian-icons-1.0.2/wagtail_humanitarian_icons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 09:45:37.000000 wagtail-humanitarian-icons-1.0.2/wagtail_humanitarian_icons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:37.852876 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/icons.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:37.852876 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:37.848876 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:37.848876 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:37.936879 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/abduction-kidnapping.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/about.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/add-document.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/advocacy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/affected-population.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/agile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/agriculture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/airport-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/airport-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/airport-destroyed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/airport-military.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/airport-not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/airport.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/analysis.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/apps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/arrest-detention.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/assault.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/assembly-point.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/assessment.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/attack.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bacteria.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/blanket.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/blog.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/boat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bookmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/border-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/border-crossing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/borehole.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bottled-water.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bridge-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bridge-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bridge-destroyed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bridge-not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bridge.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bucket.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/buddhist-temple.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/building-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/building-facility-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/building-facility-destroyed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/building-facility-not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/building.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/bus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/calendar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/camp-coordination-and-camp-management.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/car.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/carjacking.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/case-management.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/cash-transfer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/cell-tower.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/chart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/chat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/checked-mail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/checkpoint.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/child-care-child-friendly.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/child-combatant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/child-protection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/children.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/church.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/civil-military-coordination.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/clinic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/clothing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/cold-wave.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/communal-latrine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/community-building.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/community-engagement.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/computer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/confined.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/conflict.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/coordinated-assessement.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/coordination.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/country.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/covid-19.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/csv-file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/cyclone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/damaged-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/dangerous-area.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/data.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/dead.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/debris-management.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/delete-account.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/deployment.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/destroyed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/detergent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/diplomatic-mission.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/distribution-site.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/doctor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/document.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/docx-file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/drought.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/drowned.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/e-mail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/early-recovery.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/earthmound.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/earthquake.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/education.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/elderly.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/emergency-telecommunications.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/environment.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/epidemic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/exit-cancel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/expand-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/expand-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/expand-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/expand-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/famine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/favourite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/fax.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/ferry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/film.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/filter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/financing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/fire.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/fishery.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/flash-flood.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/flood.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/flour.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/food-security.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/food-warehouse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/food.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/forced-entry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/forced-recruitment.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/fund.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/gap-analysis.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/gas-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/gender-based-violence.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/gender.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/go.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/government-office.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/group.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/handwashing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/harassment-intimidation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/health-facility-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/health-facility-destroyed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/health-facility-not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/health-facility.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/health-post.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/health-worker.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/health.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/heatwave.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/heavy-rain.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/helicopter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/helipad.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/help.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/hidden.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/hindu-temple.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/hospital-bed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/hospital.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/hotel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/house-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/house-burned.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/house-destroyed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/house-lockdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/house-not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/house.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/humanitarian-access.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/humanitarian-programme-cycle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/idp-refugee-camp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/indigenous-people.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/infant-formula.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/infant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/infected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/infection-control.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/information-management.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/information-technology.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/infrastructure.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/injured.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/innovation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/insect-infestation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/internally-displaced.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/internet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/landslide-mudslide.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/laptop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/latrine-cabin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/leadership.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/learning.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/life-saving.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/livelihood.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/livestock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/location-lockdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/location.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/locust-infestation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/logistics.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/map.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/market-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/market.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/mask.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/mattress.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/medical-supply.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/medicine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/meeting.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/menu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/military-gate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/mine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/mobile-clinic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/mobile-phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/monitor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/monitoring.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/more-options.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/mosque.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/mosquito-net.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/multi-cluster-sector.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/murder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/national-army.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/needs-assessment.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/next-item.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/ngo-office.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/non-food-items-2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/non-food-items.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/not-infected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/not-secured.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/notification.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/nutrition.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/observation-tower.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/oil-facility.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/oil.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/out-of-platform.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/partnership.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/password.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/pause.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/pdf-file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/peacekeeping-force.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/people-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/people-covered.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/people-in-need-2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/people-in-need.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/people-reached.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/people-targeted-2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/people-targeted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/people-with-physical-impairments.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/permanent-camp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/person-1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/person-2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/photo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/physical-closure.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/physical-distancing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/plastic-sheeting.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/police-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/policy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/population-growth.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/population-return.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/port-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/port-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/port-destroyed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/port-not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/port.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/potable-water-source.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/potable-water.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/poverty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/power-electricity-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/power-electricity-not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/power-electricity.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/power-outage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/pregnant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/preparedness.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/previous-item.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/print.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/protection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/public-information.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/radio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/rebel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/reconstruction.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/refugee.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/registration.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/relief-goods.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/remote-support.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/remove-document.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/remove.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/report.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/reporting.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/resettlement.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/resilience.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/respiratory.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/response.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/return.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/rice.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/road-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/road-barrier.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/road-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/road-destroyed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/road-not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/road.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/roadblock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/robbery.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/rule-of-law-and-justice.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/rural-exodus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/rural.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/safety-and-security.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/salt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/sanitation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/sanitizer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/satellite-dish.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/save.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/scale-down-operation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/scale-up-operation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/school-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/school-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/school-destroyed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/school-not-affected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/school.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/search-and-rescue.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/secured.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/security.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/see.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/selected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/services-and-tools.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/sex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/sexual-and-reproductive-health.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/sexual-violence.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/share.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/shelter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/ship.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/shower.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/smartphone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/snow-avalanche.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/snowfall.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/soap.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/solid-waste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/spontaneous-site.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/spring-water.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/staff-management.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/storm-surge.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/storm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/stove.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/submersible-pump.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/sugar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/table.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/tarpaulin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/technological-disaster.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/temporary-camp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/tent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/testing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/time.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/toilet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/top-ranking.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/tornado.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/trade-and-market.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/train.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/training.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/transition-site.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/trending.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/truck.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/tsunami.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/tunnel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/un-compound-office.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/un-vehicle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/university.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/urban-rural.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/urban.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/user.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/users.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/vaccine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/validate-account.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/ventilator.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/violent-wind.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/virus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/volcano.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/walkie-talkie.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/warning-error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/water-sanitation-and-hygiene.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/water-source.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/water-trucking.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/work-from-home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/worm-infestation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/xlsx-file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/icons/zip-compressed.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:37.936879 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/templates/wagtailhumanitarianicons/widgets/icon_chooser.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-08 09:45:18.000000 wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/widgets.py
```

### Comparing `wagtail-humanitarian-icons-1.0.1/PKG-INFO` & `wagtail-humanitarian-icons-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-humanitarian-icons
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ocha Humanitarian Icons, for use in  Wagtail projects, with an icon chooser widget.
 Home-page: https://github.com/wmo-raf/wagtail-humanitarian-icons
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-humanitarian-icons-1.0.1/README.md` & `wagtail-humanitarian-icons-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-humanitarian-icons-1.0.1/setup.cfg` & `wagtail-humanitarian-icons-1.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-humanitarian-icons
-version = 1.0.1
+version = 1.0.2
 description = Ocha Humanitarian Icons, for use in  Wagtail projects, with an icon chooser widget.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-humanitarian-icons
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
@@ -18,19 +18,16 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find:
-include_package_data = true
+include_package_data = True
 python_requires = >=3.9
 install_requires = 
 	wagtail>=4.2.2
 
-[options.package_data]
-* = *.json, static/*, templates/*
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wagtail-humanitarian-icons-1.0.1/wagtail_humanitarian_icons.egg-info/PKG-INFO` & `wagtail-humanitarian-icons-1.0.2/wagtail_humanitarian_icons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-humanitarian-icons
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ocha Humanitarian Icons, for use in  Wagtail projects, with an icon chooser widget.
 Home-page: https://github.com/wmo-raf/wagtail-humanitarian-icons
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/icons.json` & `wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/icons.json`

 * *Files identical despite different names*

### Comparing `wagtail-humanitarian-icons-1.0.1/wagtailhumanitarianicons/utils.py` & `wagtail-humanitarian-icons-1.0.2/wagtailhumanitarianicons/utils.py`

 * *Files identical despite different names*

