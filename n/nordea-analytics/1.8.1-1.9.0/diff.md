# Comparing `tmp/nordea-analytics-1.8.1.tar.gz` & `tmp/nordea-analytics-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nordea-analytics-1.8.1.tar", last modified: Mon Mar 27 15:32:33 2023, max compression
+gzip compressed data, was "nordea-analytics-1.9.0.tar", last modified: Mon May  8 20:21:08 2023, max compression
```

## Comparing `nordea-analytics-1.8.1.tar` & `nordea-analytics-1.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.619546 nordea-analytics-1.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.607545 nordea-analytics-1.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.607545 nordea-analytics-1.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35801 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-27 15:32:33.619546 nordea-analytics-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-27 15:32:33.619546 nordea-analytics-1.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.607545 nordea-analytics-1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.611545 nordea-analytics-1.8.1/src/nordea_analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/convention_variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/curve_variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/forecast_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/instrument_variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/key_figure_names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.611545 nordea-analytics-1.8.1/src/nordea_analytics/nalib/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/config_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/data_retrieval_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.611545 nordea-analytics-1.8.1/src/nordea_analytics/nalib/http/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/http/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/http/open_banking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.615545 nordea-analytics-1.8.1/src/nordea_analytics/nalib/live_keyfigures/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/live_keyfigures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/live_keyfigures/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/live_keyfigures/open_banking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/live_keyfigures/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/proxy_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.619546 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BenchmarkDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureAdvancedCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18827 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureHorizonCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondStaticData.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/Curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/CurveDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/CurveTimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/DateSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/FXForecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/FXQuotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/IndexComposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/LiveBondKeyFigures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/LiveBondUniverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/Quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/ShiftDate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/ShiftDays.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/YearFraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/YieldForecast.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.619546 nordea-analytics-1.8.1/src/nordea_analytics/nordea_analytics_service/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nordea_analytics_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30809 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nordea_analytics_service/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nordea_analytics_service/open_banking.py
--rw-r--r--   0 runner    (1001) docker     (123)    27146 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/nordea_analytics_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/search_bond_names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.619546 nordea-analytics-1.8.1/src/nordea_analytics/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/shortcuts/open_banking.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/shortcuts/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/src/nordea_analytics/shortcuts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.611545 nordea-analytics-1.8.1/src/nordea_analytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-27 15:32:33.000000 nordea-analytics-1.8.1/src/nordea_analytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-27 15:32:33.000000 nordea-analytics-1.8.1/src/nordea_analytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:32:33.000000 nordea-analytics-1.8.1/src/nordea_analytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-27 15:32:33.000000 nordea-analytics-1.8.1/src/nordea_analytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 15:32:33.000000 nordea-analytics-1.8.1/src/nordea_analytics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:32:33.619546 nordea-analytics-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/tests/test_proxy_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-03-27 15:32:17.000000 nordea-analytics-1.8.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.135180 nordea-analytics-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.123180 nordea-analytics-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.127180 nordea-analytics-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35801 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-08 20:21:08.135180 nordea-analytics-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-08 20:21:08.139180 nordea-analytics-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.123180 nordea-analytics-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.127180 nordea-analytics-1.9.0/src/nordea_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/convention_variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/curve_variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/forecast_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/instrument_variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/key_figure_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.131180 nordea-analytics-1.9.0/src/nordea_analytics/nalib/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/config_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/data_retrieval_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.131180 nordea-analytics-1.9.0/src/nordea_analytics/nalib/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/http/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/http/open_banking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.131180 nordea-analytics-1.9.0/src/nordea_analytics/nalib/live_keyfigures/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/live_keyfigures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/live_keyfigures/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/live_keyfigures/open_banking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/live_keyfigures/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/proxy_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.135180 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BenchmarkDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20927 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13600 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureHorizonCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondKeyFigures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondRepoCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondStaticData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/Curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/CurveDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/CurveTimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/DateSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/FXForecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/FXQuotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/IndexComposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/LiveBondKeyFigures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/LiveBondUniverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/Quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/ShiftDate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/ShiftDays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/YearFraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/YieldForecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.135180 nordea-analytics-1.9.0/src/nordea_analytics/nordea_analytics_service/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nordea_analytics_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32666 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nordea_analytics_service/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nordea_analytics_service/open_banking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26422 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/nordea_analytics_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21718 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/search_bond_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.135180 nordea-analytics-1.9.0/src/nordea_analytics/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/shortcuts/open_banking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/shortcuts/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/src/nordea_analytics/shortcuts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.127180 nordea-analytics-1.9.0/src/nordea_analytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-08 20:21:08.000000 nordea-analytics-1.9.0/src/nordea_analytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-08 20:21:08.000000 nordea-analytics-1.9.0/src/nordea_analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:21:08.000000 nordea-analytics-1.9.0/src/nordea_analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 20:21:08.000000 nordea-analytics-1.9.0/src/nordea_analytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 20:21:08.000000 nordea-analytics-1.9.0/src/nordea_analytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:21:08.135180 nordea-analytics-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/tests/test_proxy_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-08 20:20:55.000000 nordea-analytics-1.9.0/tests/test_util.py
```

### Comparing `nordea-analytics-1.8.1/.github/workflows/python-publish.yml` & `nordea-analytics-1.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.8.1/LICENCE.md` & `nordea-analytics-1.9.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.8.1/PKG-INFO` & `nordea-analytics-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordea-analytics
-Version: 1.8.1
+Version: 1.9.0
 Summary: Nordea Analytics Python library
 Home-page: https://github.com/NordeaOSS/nordea-analytics
 Author: Nordea Desk Quants and Markets Advisory Tools
 Author-email: E-advisorySupport@nordea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nordea-analytics-1.8.1/setup.cfg` & `nordea-analytics-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/__init__.py` & `nordea-analytics-1.9.0/src/nordea_analytics/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-"""The Nordea Analytics Python Project API."""
-from .convention_variable_names import (
-    CashflowType,
-    DateRollConvention,
-    DayCountConvention,
-    Exchange,
-    TimeConvention,
-)
-from .curve_variable_names import CurveDefinitionName, CurveName, CurveType, SpotForward
-from .forecast_names import YieldCountry, YieldHorizon, YieldType
-from .instrument_variable_names import BenchmarkName, BondIndexName
-from .key_figure_names import (
-    BondKeyFigureName,
-    CalculatedBondKeyFigureName,
-    HorizonCalculatedBondKeyFigureName,
-    LiveBondKeyFigureName,
-    TimeSeriesKeyFigureName,
-)
-from .nordea_analytics_service import NordeaAnalyticsService
-from .search_bond_names import (
-    AmortisationType,
-    AssetType,
-    CapitalCentres,
-    CapitalCentreTypes,
-    InstrumentGroup,
-    Issuers,
-)
-from .shortcuts.utils import disable_analytics_warnings
-
-# To distinguish between external and internal packages
-try:
-    from .shortcuts.nordea import get_nordea_analytics_client  # type: ignore
-    from .shortcuts.nordea import get_nordea_analytics_test_client  # type: ignore # noqa: E401
-except (NameError, ModuleNotFoundError):
-    from .shortcuts.open_banking import get_nordea_analytics_client  # type: ignore
-    from .shortcuts.open_banking import get_nordea_analytics_test_client  # type: ignore # noqa: F401
-
-__version__ = "1.8.1"
-__all__ = [
-    "get_nordea_analytics_client",
-    "get_nordea_analytics_test_client",
-    "disable_analytics_warnings",
-    "AmortisationType",
-    "AssetType",
-    "BenchmarkName",
-    "BondIndexName",
-    "BondKeyFigureName",
-    "CalculatedBondKeyFigureName",
-    "CapitalCentreTypes",
-    "CapitalCentres",
-    "CashflowType",
-    "CurveDefinitionName",
-    "CurveName",
-    "CurveType",
-    "DateRollConvention",
-    "DayCountConvention",
-    "Exchange",
-    "HorizonCalculatedBondKeyFigureName",
-    "InstrumentGroup",
-    "Issuers",
-    "LiveBondKeyFigureName",
-    "NordeaAnalyticsService",
-    "SpotForward",
-    "TimeConvention",
-    "TimeSeriesKeyFigureName",
-    "YieldCountry",
-    "YieldHorizon",
-    "YieldType",
-]
+"""The Nordea Analytics Python Project API."""
+from .convention_variable_names import (
+    CashflowType,
+    DateRollConvention,
+    DayCountConvention,
+    Exchange,
+    TimeConvention,
+)
+from .curve_variable_names import CurveDefinitionName, CurveName, CurveType, SpotForward
+from .forecast_names import YieldCountry, YieldHorizon, YieldType
+from .instrument_variable_names import BenchmarkName, BondIndexName
+from .key_figure_names import (
+    BondKeyFigureName,
+    CalculatedBondKeyFigureName,
+    HorizonCalculatedBondKeyFigureName,
+    LiveBondKeyFigureName,
+    TimeSeriesKeyFigureName,
+)
+from .nordea_analytics_service import NordeaAnalyticsService
+from .search_bond_names import (
+    AmortisationType,
+    AssetType,
+    CapitalCentres,
+    CapitalCentreTypes,
+    InstrumentGroup,
+    Issuers,
+)
+from .shortcuts.utils import disable_analytics_warnings
+
+# To distinguish between external and internal packages
+try:
+    from .shortcuts.nordea import get_nordea_analytics_client  # type: ignore
+    from .shortcuts.nordea import get_nordea_analytics_test_client  # type: ignore # noqa: E401
+except (NameError, ModuleNotFoundError):
+    from .shortcuts.open_banking import get_nordea_analytics_client  # type: ignore
+    from .shortcuts.open_banking import get_nordea_analytics_test_client  # type: ignore # noqa: F401
+
+__version__ = "1.9.0"
+__all__ = [
+    "get_nordea_analytics_client",
+    "get_nordea_analytics_test_client",
+    "disable_analytics_warnings",
+    "AmortisationType",
+    "AssetType",
+    "BenchmarkName",
+    "BondIndexName",
+    "BondKeyFigureName",
+    "CalculatedBondKeyFigureName",
+    "CapitalCentreTypes",
+    "CapitalCentres",
+    "CashflowType",
+    "CurveDefinitionName",
+    "CurveName",
+    "CurveType",
+    "DateRollConvention",
+    "DayCountConvention",
+    "Exchange",
+    "HorizonCalculatedBondKeyFigureName",
+    "InstrumentGroup",
+    "Issuers",
+    "LiveBondKeyFigureName",
+    "NordeaAnalyticsService",
+    "SpotForward",
+    "TimeConvention",
+    "TimeSeriesKeyFigureName",
+    "YieldCountry",
+    "YieldHorizon",
+    "YieldType",
+]
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/convention_variable_names.py` & `nordea-analytics-1.9.0/src/nordea_analytics/convention_variable_names.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from enum import Enum
-
-
-class DateRollConvention(Enum):
-    """Date roll conventions available in the service."""
-
-    Follow = "Follow"
-    IMM_Wednesday = "IMM Wednesday"
-    ModFollow = "Mod follow"
-    NoDateRoll = "None"
-    Preceeding = "Preceeding"
-    StartOfMonthUnadjusted = "Start Of Month Unadjusted"
-
-
-class DayCountConvention(Enum):
-    """Day count conventions available in the service."""
-
-    BankDays = "Bank Days"
-    BusinessDays = "Business Days"
-    CalendarDays = "Calendar Days"
-    Days30 = "Days 30"
-    Days30E = "Days 30E"
-    Days30EP = "Days 30EP"
-
-
-class TimeConvention(Enum):
-    """Time conventions available in the service."""
-
-    TC_30360 = "30360"
-    TC_30E360 = "30e360"
-    TC_30EP360 = "30ep360"
-    Act360 = "act360"
-    Act365 = "act365"
-    ISDAAct = "isdaact"
-    ActNL365 = "actnl365"
-    AFB = "afb"
-    ActNL360 = "actnl360"
-
-
-class Exchange(Enum):
-    """Exchanges available in the service."""
-
-    AmericanStockExchange = "AMEX"
-    Amsterdam = "NLG"
-    Ankara = "TRY"
-    Athens = "GRD"
-    AustralianStockExchange = "XASX"
-    Bangkok = "THB"
-    BelgradeStockExchange = "XBEL"
-    BermudaStockExchange = "XBDA"
-    BombayStockExchange = "XBOM"
-    Bratislava = "SKK"
-    BratislavaStockExchange = "XBRA"
-    Brussel = "BEF"
-    BucharestStockExchange = "RON"
-    Budapest = "HUF"
-    BudapestStockExchange = "XBUD"
-    BulgarianStockExchange = "XBUL"
-    CairoandAlexandriaStockExchange = "XCAI"
-    CasablancaStockExchange = "XCAS"
-    ColombiaStockExchange = "XBOG"
-    Copenhagen = "DKK"
-    CopenhagenOTC = "DKKOTC"
-    CyprusStockExchange = "XCYS"
-    Dublin = "IEP"
-    Dusseldorf = "Dusseldorf"
-    Frankfurt = "DEM"
-    GhanaStockExchange = "XGHA"
-    Helsinki = "FIM"
-    HongKong = "HKD"
-    HongKongStockExchange = "XHKG"
-    IcelandStockExchange = "XICE"
-    IndonesiaStockExchange = "XIDX"
-    IstanbulStockExchange = "XIST"
-    JohannesburgStockExchange = "XJSE"
-    KarachiStockExchange = "XKAR"
-    KievInternationalStockExchange = "XKIS"
-    KoreanStockExchange = "XKRX"
-    KuwaitStockExchange = "XKUW"
-    LimaStockExchange = "XLIM"
-    Lisbon = "PTE"
-    LithuaniaStockExchange = "XLIT"
-    Ljubljana = "SIT"
-    London = "GBP"
-    LondonStockExchange = "XLON"
-    Luxembourg = "LUF"
-    Madrid = "ESP"
-    MexicoCity = "MXN"
-    MexicoStockExchange = "XMEX"
-    Milano = "ITL"
-    Montreal = "Montreal"
-    Moscow = "RUB"
-    MoscowStockExchange = "XMOS"
-    NagoyaStockExchange = "XNGO"
-    NasdaqOTC = "Nasdaq OTC"
-    NationalStockExchangeofIndia = "XNSE"
-    NewYork = "USD"
-    NewYorkStockExchange = "XNYS"
-    NewZealandStockExchange = "XNZE"
-    NigerianStockExchange = "XNSA"
-    OsakaStockExchange = "XOSE"
-    Oslo = "NOK"
-    Paris = "FRF"
-    PhilippineStockExchange = "XPHS"
-    Prague = "CZK"
-    PragueStockExchange = "XPRA"
-    Reykjavik = "ISK"
-    Riga = "LVL"
-    RigaStockExchange = "XRIS"
-    Riyadh = "SAR"
-    SantiagoStockExchange = "XSGO"
-    SaudiArabianStockExchange = "XSAU"
-    ShanghaiStockExchange = "XSHG"
-    Singapore = "SGD"
-    SingaporeExchange = "XSES"
-    Stockholm = "SEK"
-    SwissExchange = "XSWX"
-    Sydney = "AUD"
-    TaiwanStockExchange = "XTAI"
-    Tallinn = "EEK"
-    TallinnStockExchange = "XTAL"
-    Target = "EUR"
-    TehranStockExchange = "XTEH"
-    TelAviv = "ILS"
-    TelAvivStockExchange = "XTAE"
-    ThailandStockExchange = "XBKK"
-    Tokyo = "JPY"
-    TokyoStockExchange = "XTKS"
-    Toronto = "Toronto"
-    TorontoStockExchange = "XTSE"
-    Vienna = "ATS"
-    Vilnius = "LTL"
-    Warsaw = "PLN"
-    WarsawStockExchange = "XWAR"
-    Wellington = "NZD"
-    XETRAStockExchange = "XETRA"
-    Zagreb = "HRK"
-    ZagrebStockExchange = "XZAG"
-    Zurich = "CHF"
-
-
-class CashflowType(Enum):
-    """Cashflow types available in the service."""
-
-    CSE = "CSE"
-    MCI = "MCI"
+from enum import Enum
+
+
+class DateRollConvention(Enum):
+    """Date roll conventions available in the service."""
+
+    Follow = "Follow"
+    IMM_Wednesday = "IMM Wednesday"
+    ModFollow = "Mod follow"
+    NoDateRoll = "None"
+    Preceeding = "Preceeding"
+    StartOfMonthUnadjusted = "Start Of Month Unadjusted"
+
+
+class DayCountConvention(Enum):
+    """Day count conventions available in the service."""
+
+    BankDays = "Bank Days"
+    BusinessDays = "Business Days"
+    CalendarDays = "Calendar Days"
+    Days30 = "Days 30"
+    Days30E = "Days 30E"
+    Days30EP = "Days 30EP"
+
+
+class TimeConvention(Enum):
+    """Time conventions available in the service."""
+
+    TC_30360 = "30360"
+    TC_30E360 = "30e360"
+    TC_30EP360 = "30ep360"
+    Act360 = "act360"
+    Act365 = "act365"
+    ISDAAct = "isdaact"
+    ActNL365 = "actnl365"
+    AFB = "afb"
+    ActNL360 = "actnl360"
+
+
+class Exchange(Enum):
+    """Exchanges available in the service."""
+
+    AmericanStockExchange = "AMEX"
+    Amsterdam = "NLG"
+    Ankara = "TRY"
+    Athens = "GRD"
+    AustralianStockExchange = "XASX"
+    Bangkok = "THB"
+    BelgradeStockExchange = "XBEL"
+    BermudaStockExchange = "XBDA"
+    BombayStockExchange = "XBOM"
+    Bratislava = "SKK"
+    BratislavaStockExchange = "XBRA"
+    Brussel = "BEF"
+    BucharestStockExchange = "RON"
+    Budapest = "HUF"
+    BudapestStockExchange = "XBUD"
+    BulgarianStockExchange = "XBUL"
+    CairoandAlexandriaStockExchange = "XCAI"
+    CasablancaStockExchange = "XCAS"
+    ColombiaStockExchange = "XBOG"
+    Copenhagen = "DKK"
+    CopenhagenOTC = "DKKOTC"
+    CyprusStockExchange = "XCYS"
+    Dublin = "IEP"
+    Dusseldorf = "Dusseldorf"
+    Frankfurt = "DEM"
+    GhanaStockExchange = "XGHA"
+    Helsinki = "FIM"
+    HongKong = "HKD"
+    HongKongStockExchange = "XHKG"
+    IcelandStockExchange = "XICE"
+    IndonesiaStockExchange = "XIDX"
+    IstanbulStockExchange = "XIST"
+    JohannesburgStockExchange = "XJSE"
+    KarachiStockExchange = "XKAR"
+    KievInternationalStockExchange = "XKIS"
+    KoreanStockExchange = "XKRX"
+    KuwaitStockExchange = "XKUW"
+    LimaStockExchange = "XLIM"
+    Lisbon = "PTE"
+    LithuaniaStockExchange = "XLIT"
+    Ljubljana = "SIT"
+    London = "GBP"
+    LondonStockExchange = "XLON"
+    Luxembourg = "LUF"
+    Madrid = "ESP"
+    MexicoCity = "MXN"
+    MexicoStockExchange = "XMEX"
+    Milano = "ITL"
+    Montreal = "Montreal"
+    Moscow = "RUB"
+    MoscowStockExchange = "XMOS"
+    NagoyaStockExchange = "XNGO"
+    NasdaqOTC = "Nasdaq OTC"
+    NationalStockExchangeofIndia = "XNSE"
+    NewYork = "USD"
+    NewYorkStockExchange = "XNYS"
+    NewZealandStockExchange = "XNZE"
+    NigerianStockExchange = "XNSA"
+    OsakaStockExchange = "XOSE"
+    Oslo = "NOK"
+    Paris = "FRF"
+    PhilippineStockExchange = "XPHS"
+    Prague = "CZK"
+    PragueStockExchange = "XPRA"
+    Reykjavik = "ISK"
+    Riga = "LVL"
+    RigaStockExchange = "XRIS"
+    Riyadh = "SAR"
+    SantiagoStockExchange = "XSGO"
+    SaudiArabianStockExchange = "XSAU"
+    ShanghaiStockExchange = "XSHG"
+    Singapore = "SGD"
+    SingaporeExchange = "XSES"
+    Stockholm = "SEK"
+    SwissExchange = "XSWX"
+    Sydney = "AUD"
+    TaiwanStockExchange = "XTAI"
+    Tallinn = "EEK"
+    TallinnStockExchange = "XTAL"
+    Target = "EUR"
+    TehranStockExchange = "XTEH"
+    TelAviv = "ILS"
+    TelAvivStockExchange = "XTAE"
+    ThailandStockExchange = "XBKK"
+    Tokyo = "JPY"
+    TokyoStockExchange = "XTKS"
+    Toronto = "Toronto"
+    TorontoStockExchange = "XTSE"
+    Vienna = "ATS"
+    Vilnius = "LTL"
+    Warsaw = "PLN"
+    WarsawStockExchange = "XWAR"
+    Wellington = "NZD"
+    XETRAStockExchange = "XETRA"
+    Zagreb = "HRK"
+    ZagrebStockExchange = "XZAG"
+    Zurich = "CHF"
+
+
+class CashflowType(Enum):
+    """Cashflow types available in the service."""
+
+    CSE = "CSE"
+    MCI = "MCI"
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/curve_variable_names.py` & `nordea-analytics-1.9.0/src/nordea_analytics/curve_variable_names.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-from enum import Enum
-
-
-class CurveName(Enum):
-    """Most common available curves. Availability not limit to this list."""
-
-    ATSGOV = "ATSGOV"
-    BEFGOV = "BEFGOV"
-    CHFGOV = "CHFGOV"
-    CHFSWAP_Disc_OIS = "CHFSWAP DISC OIS"
-    CHFSWAP_Fix_1D_OIS = "CHFSWAP FIX 1D OIS"
-    CHFSWAP_Fix_1Y_OIS = "CHFSWAP FIX 1Y OIS"
-    CHFSWAP_Fix_3M_OIS = "CHFSWAP FIX 3M OIS"
-    CHFSWAP_Fix_6M_OIS = "CHFSWAP FIX 6M OIS"
-    CHFSWAP_Libor = "CHFSWAP LIBOR"
-    DEMGOV = "DEMGOV"
-    DKKGOV = "DKKGOV"
-    DKKMTGNYK = "DKKMTGNYKSOFTBLT"
-    DKKSWAP = "DKKSWAP"
-    DKKSWAP_Disc_OIS = "DKKSWAP DISC OIS"
-    DKKSWAP_Fix_1D_OIS = "DKKSWAP FIX 1D OIS"
-    DKKSWAP_Fix_1M_OIS = "DKKSWAP FIX 1M OIS"
-    DKKSWAP_Fix_1Y_OIS = "DKKSWAP FIX 1Y OIS"
-    DKKSWAP_Fix_3M_OIS = "DKKSWAP FIX 3M OIS"
-    DKKSWAP_Fix_6M_OIS = "DKKSWAP FIX 6M OIS"
-    DKKSWAP_Libor = "DKKSWAP LIBOR"
-    DKKSWAP_Libor_3M = "DKKSWAP LIBOR 3M"
-    ESPGOV = "ESPGOV"
-    EURGOV = "EURGOV"
-    EURSWAP = "EURSWAP"
-    EURSWAP_Disc_ESTR = "EURSWAP DISC ESTR"
-    EURSWAP_Disc_OIS = "EURSWAP DISC OIS"
-    EURSWAP_Fix_1D_ESTR = "EURSWAP FIX 1D ESTR"
-    EURSWAP_Fix_1D_OIS = "EURSWAP FIX 1D OIS"
-    EURSWAP_Fix_1M_ESTR = "EURSWAP FIX 1M ESTR"
-    EURSWAP_Fix_1Y_ESTR = "EURSWAP FIX 1Y ESTR"
-    EURSWAP_Fix_3M_ESTR = "EURSWAP FIX 3M ESTR"
-    EURSWAP_Fix_6M_ESTR = "EURSWAP FIX 6M ESTR"
-    EURSWAP_Libor = "EURSWAP LIBOR"
-    FIMGOV = "FIMGOV"
-    FRFGOV = "FRFGOV"
-    GBPGOV = "GBPGOV"
-    GBPSWAP = "GBPSWAP"
-    GBPSWAP_Disc_OIS = "GBPSWAP DISC OIS"
-    GBPSWAP_Fix_1D_OIS = "GBPSWAP FIX 1D OIS"
-    GBPSWAP_Fix_3M_OIS = "GBPSWAP FIX 3M OIS"
-    GBPSWAP_Fix_6M_OIS = "GBPSWAP FIX 6M OIS"
-    GBPSWAP_Libor = "GBPSWAP LIBOR"
-    ITLGOV = "ITLGOV"
-    JPYGOV = "JPYGOV"
-    JPYSWAP = "JPYSWAP"
-    JPYSWAP_Disc_OIS = "JPYSWAP DISC OIS"
-    JPYSWAP_Fix_1D_OIS = "JPYSWAP FIX 1D OIS"
-    JPYSWAP_Fix_3M_OIS = "JPYSWAP FIX 3M OIS"
-    JPYSWAP_Fix_6M_OIS = "JPYSWAP FIX 6M OIS"
-    JPYSWAP_Libor = "JPYSWAP LIBOR"
-    NLGGOV = "NLGGOV"
-    NOKGOV = "NOKGOV"
-    NOKSWAP = "NOKSWAP"
-    NOKSWAP_Disc_OIS = "NOKSWAP DISC OIS"
-    NOKSWAP_Fix_1D_OIS = "NOKSWAP FIX 1D OIS"
-    NOKSWAP_Fix_1Y_OIS = "NOKSWAP FIX 1Y OIS"
-    NOKSWAP_Fix_3M_OIS = "NOKSWAP FIX 3M OIS"
-    NOKSWAP_Fix_6M_OIS = "NOKSWAP FIX 6M OIS"
-    NOKSWAP_Libor = "NOKSWAP LIBOR"
-    PLNGOV = "PLNGOV"
-    RUBSWAP = "RUBSWAP"
-    RUBSWAP_Disc_OIS = "RUBSWAP DISC OIS"
-    RUBSWAP_Fix_1D_OIS = "RUBSWAP FIX 1D OIS"
-    RUBSWAP_Fix_3M_OIS = "RUBSWAP FIX 3M OIS"
-    RUBSWAP_Fix_6M_OIS = "RUBSWAP FIX 6M OIS"
-    RUBSWAP_Libor = "RUBSWAP LIBOR"
-    SEKGOV = "SEKGOV"
-    SEKMTGBLEND = "SEKMTGBLEND"
-    SEKMTGNBH = "SEKMTGNBH"
-    SEKMTGSEB = "SEKMTGSEB"
-    SEKMTGSHYP = "SEKMTGSHYP"
-    SEKMTGSWED = "SEKMTGSWED"
-    SEKSWAP = "SEKSWAP"
-    SEKSWAP_Disc_OIS = "SEKSWAP DISC OIS"
-    SEKSWAP_Fix_1D_OIS = "SEKSWAP FIX 1D OIS"
-    SEKSWAP_Fix_1Y_OIS = "SEKSWAP FIX 1Y OIS"
-    SEKSWAP_Fix_3M_OIS = "SEKSWAP FIX 3M OIS"
-    SEKSWAP_Fix_6M_OIS = "SEKSWAP FIX 6M OIS"
-    SEKSWAP_Libor = "SEKSWAP LIBOR"
-    USDGOV = "USDGOV"
-    USDSWAP = "USDSWAP"
-    USDSWAP_Disc_OIS = "USDSWAP DISC OIS"
-    USDSWAP_Fix_1D_OIS = "USDSWAP FIX 1D OIS"
-    USDSWAP_Fix_3M_OIS = "USDSWAP FIX 3M OIS"
-    USDSWAP_Fix_6M_OIS = "USDSWAP FIX 6M OIS"
-    USDSWAP_Libor = "USDSWAP LIBOR"
-
-
-class CurveDefinitionName(Enum):
-    """Most common available curves definition. Availability not limit to this list."""
-
-    # Note that curve definition is limited to non-Infinity curves for externals.
-    ATSGOV = "ATSGOV"
-    BEFGOV = "BEFGOV"
-    CHFGOV = "CHFGOV"
-    DEMGOV = "DEMGOV"
-    DKKGOV = "DKKGOV"
-    DKKMTGNYK = "DKKMTGNYKSOFTBLT"
-    DKKSWAP = "DKKSWAP"
-    ESPGOV = "ESPGOV"
-    EURGOV = "EURGOV"
-    EURSWAP = "EURSWAP"
-    FIMGOV = "FIMGOV"
-    FRFGOV = "FRFGOV"
-    GBPGOV = "GBPGOV"
-    GBPSWAP = "GBPSWAP"
-    ITLGOV = "ITLGOV"
-    JPYGOV = "JPYGOV"
-    JPYSWAP = "JPYSWAP"
-    NLGGOV = "NLGGOV"
-    NOKGOV = "NOKGOV"
-    NOKSWAP = "NOKSWAP"
-    NOKSWAP_Libor = "NOKSWAP LIBOR"
-    PLNGOV = "PLNGOV"
-    RUBSWAP = "RUBSWAP"
-    SEKGOV = "SEKGOV"
-    SEKMTGBLEND = "SEKMTGBLEND"
-    SEKMTGNBH = "SEKMTGNBH"
-    SEKMTGSEB = "SEKMTGSEB"
-    SEKMTGSHYP = "SEKMTGSHYP"
-    SEKMTGSWED = "SEKMTGSWED"
-    SEKSWAP = "SEKSWAP"
-    USDGOV = "USDGOV"
-    USDSWAP = "USDSWAP"
-
-
-class CurveType(Enum):
-    """Curve types available in the service."""
-
-    Bootstrap = "bootstrap"
-    NelsonSiegel = "nelsonsiegel"
-    XNelsonSiegel = "xnelsonsiegel"
-    HybridXNS = "hybridxns"
-    HybridNS = "hybridns"
-    YTMCurve = "ytm curve"
-    ParCurve = "par curve"
-    DurationCurve = "duration curve"
-
-
-class SpotForward(Enum):
-    """Spot/forward available in the service."""
-
-    Spot = "Spot"
-    Forward = "Forward"
-    ImpliedForward = "ImpliedForward"
+from enum import Enum
+
+
+class CurveName(Enum):
+    """Most common available curves. Availability not limit to this list."""
+
+    ATSGOV = "ATSGOV"
+    BEFGOV = "BEFGOV"
+    CHFGOV = "CHFGOV"
+    CHFSWAP_Disc_OIS = "CHFSWAP DISC OIS"
+    CHFSWAP_Fix_1D_OIS = "CHFSWAP FIX 1D OIS"
+    CHFSWAP_Fix_1Y_OIS = "CHFSWAP FIX 1Y OIS"
+    CHFSWAP_Fix_3M_OIS = "CHFSWAP FIX 3M OIS"
+    CHFSWAP_Fix_6M_OIS = "CHFSWAP FIX 6M OIS"
+    CHFSWAP_Libor = "CHFSWAP LIBOR"
+    DEMGOV = "DEMGOV"
+    DKKGOV = "DKKGOV"
+    DKKMTGNYK = "DKKMTGNYKSOFTBLT"
+    DKKSWAP = "DKKSWAP"
+    DKKSWAP_Disc_OIS = "DKKSWAP DISC OIS"
+    DKKSWAP_Fix_1D_OIS = "DKKSWAP FIX 1D OIS"
+    DKKSWAP_Fix_1M_OIS = "DKKSWAP FIX 1M OIS"
+    DKKSWAP_Fix_1Y_OIS = "DKKSWAP FIX 1Y OIS"
+    DKKSWAP_Fix_3M_OIS = "DKKSWAP FIX 3M OIS"
+    DKKSWAP_Fix_6M_OIS = "DKKSWAP FIX 6M OIS"
+    DKKSWAP_Libor = "DKKSWAP LIBOR"
+    DKKSWAP_Libor_3M = "DKKSWAP LIBOR 3M"
+    ESPGOV = "ESPGOV"
+    EURGOV = "EURGOV"
+    EURSWAP = "EURSWAP"
+    EURSWAP_Disc_ESTR = "EURSWAP DISC ESTR"
+    EURSWAP_Disc_OIS = "EURSWAP DISC OIS"
+    EURSWAP_Fix_1D_ESTR = "EURSWAP FIX 1D ESTR"
+    EURSWAP_Fix_1D_OIS = "EURSWAP FIX 1D OIS"
+    EURSWAP_Fix_1M_ESTR = "EURSWAP FIX 1M ESTR"
+    EURSWAP_Fix_1Y_ESTR = "EURSWAP FIX 1Y ESTR"
+    EURSWAP_Fix_3M_ESTR = "EURSWAP FIX 3M ESTR"
+    EURSWAP_Fix_6M_ESTR = "EURSWAP FIX 6M ESTR"
+    EURSWAP_Libor = "EURSWAP LIBOR"
+    FIMGOV = "FIMGOV"
+    FRFGOV = "FRFGOV"
+    GBPGOV = "GBPGOV"
+    GBPSWAP = "GBPSWAP"
+    GBPSWAP_Disc_OIS = "GBPSWAP DISC OIS"
+    GBPSWAP_Fix_1D_OIS = "GBPSWAP FIX 1D OIS"
+    GBPSWAP_Fix_3M_OIS = "GBPSWAP FIX 3M OIS"
+    GBPSWAP_Fix_6M_OIS = "GBPSWAP FIX 6M OIS"
+    GBPSWAP_Libor = "GBPSWAP LIBOR"
+    ITLGOV = "ITLGOV"
+    JPYGOV = "JPYGOV"
+    JPYSWAP = "JPYSWAP"
+    JPYSWAP_Disc_OIS = "JPYSWAP DISC OIS"
+    JPYSWAP_Fix_1D_OIS = "JPYSWAP FIX 1D OIS"
+    JPYSWAP_Fix_3M_OIS = "JPYSWAP FIX 3M OIS"
+    JPYSWAP_Fix_6M_OIS = "JPYSWAP FIX 6M OIS"
+    JPYSWAP_Libor = "JPYSWAP LIBOR"
+    NLGGOV = "NLGGOV"
+    NOKGOV = "NOKGOV"
+    NOKSWAP = "NOKSWAP"
+    NOKSWAP_Disc_OIS = "NOKSWAP DISC OIS"
+    NOKSWAP_Fix_1D_OIS = "NOKSWAP FIX 1D OIS"
+    NOKSWAP_Fix_1Y_OIS = "NOKSWAP FIX 1Y OIS"
+    NOKSWAP_Fix_3M_OIS = "NOKSWAP FIX 3M OIS"
+    NOKSWAP_Fix_6M_OIS = "NOKSWAP FIX 6M OIS"
+    NOKSWAP_Libor = "NOKSWAP LIBOR"
+    PLNGOV = "PLNGOV"
+    RUBSWAP = "RUBSWAP"
+    RUBSWAP_Disc_OIS = "RUBSWAP DISC OIS"
+    RUBSWAP_Fix_1D_OIS = "RUBSWAP FIX 1D OIS"
+    RUBSWAP_Fix_3M_OIS = "RUBSWAP FIX 3M OIS"
+    RUBSWAP_Fix_6M_OIS = "RUBSWAP FIX 6M OIS"
+    RUBSWAP_Libor = "RUBSWAP LIBOR"
+    SEKGOV = "SEKGOV"
+    SEKMTGBLEND = "SEKMTGBLEND"
+    SEKMTGNBH = "SEKMTGNBH"
+    SEKMTGSEB = "SEKMTGSEB"
+    SEKMTGSHYP = "SEKMTGSHYP"
+    SEKMTGSWED = "SEKMTGSWED"
+    SEKSWAP = "SEKSWAP"
+    SEKSWAP_Disc_OIS = "SEKSWAP DISC OIS"
+    SEKSWAP_Fix_1D_OIS = "SEKSWAP FIX 1D OIS"
+    SEKSWAP_Fix_1Y_OIS = "SEKSWAP FIX 1Y OIS"
+    SEKSWAP_Fix_3M_OIS = "SEKSWAP FIX 3M OIS"
+    SEKSWAP_Fix_6M_OIS = "SEKSWAP FIX 6M OIS"
+    SEKSWAP_Libor = "SEKSWAP LIBOR"
+    USDGOV = "USDGOV"
+    USDSWAP = "USDSWAP"
+    USDSWAP_Disc_OIS = "USDSWAP DISC OIS"
+    USDSWAP_Fix_1D_OIS = "USDSWAP FIX 1D OIS"
+    USDSWAP_Fix_3M_OIS = "USDSWAP FIX 3M OIS"
+    USDSWAP_Fix_6M_OIS = "USDSWAP FIX 6M OIS"
+    USDSWAP_Libor = "USDSWAP LIBOR"
+
+
+class CurveDefinitionName(Enum):
+    """Most common available curves definition. Availability not limit to this list."""
+
+    # Note that curve definition is limited to non-Infinity curves for externals.
+    ATSGOV = "ATSGOV"
+    BEFGOV = "BEFGOV"
+    CHFGOV = "CHFGOV"
+    DEMGOV = "DEMGOV"
+    DKKGOV = "DKKGOV"
+    DKKMTGNYK = "DKKMTGNYKSOFTBLT"
+    DKKSWAP = "DKKSWAP"
+    ESPGOV = "ESPGOV"
+    EURGOV = "EURGOV"
+    EURSWAP = "EURSWAP"
+    FIMGOV = "FIMGOV"
+    FRFGOV = "FRFGOV"
+    GBPGOV = "GBPGOV"
+    GBPSWAP = "GBPSWAP"
+    ITLGOV = "ITLGOV"
+    JPYGOV = "JPYGOV"
+    JPYSWAP = "JPYSWAP"
+    NLGGOV = "NLGGOV"
+    NOKGOV = "NOKGOV"
+    NOKSWAP = "NOKSWAP"
+    NOKSWAP_Libor = "NOKSWAP LIBOR"
+    PLNGOV = "PLNGOV"
+    RUBSWAP = "RUBSWAP"
+    SEKGOV = "SEKGOV"
+    SEKMTGBLEND = "SEKMTGBLEND"
+    SEKMTGNBH = "SEKMTGNBH"
+    SEKMTGSEB = "SEKMTGSEB"
+    SEKMTGSHYP = "SEKMTGSHYP"
+    SEKMTGSWED = "SEKMTGSWED"
+    SEKSWAP = "SEKSWAP"
+    USDGOV = "USDGOV"
+    USDSWAP = "USDSWAP"
+
+
+class CurveType(Enum):
+    """Curve types available in the service."""
+
+    Bootstrap = "bootstrap"
+    NelsonSiegel = "nelsonsiegel"
+    XNelsonSiegel = "xnelsonsiegel"
+    HybridXNS = "hybridxns"
+    HybridNS = "hybridns"
+    YTMCurve = "ytm curve"
+    ParCurve = "par curve"
+    DurationCurve = "duration curve"
+
+
+class SpotForward(Enum):
+    """Spot/forward available in the service."""
+
+    Spot = "Spot"
+    Forward = "Forward"
+    ImpliedForward = "ImpliedForward"
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/auth.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/auth.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""Script for various methods for auth nordea analytics library."""
-from urllib.parse import urljoin, urlparse
-
-import requests
-from requests import cookies
-from requests_kerberos import DISABLED, HTTPKerberosAuth  # type: ignore
-
-from nordea_analytics.nalib.util import get_config
-
-config = get_config()
-
-
-def authenticate() -> cookies.RequestsCookieJar:
-    """Function provide OAUTH2 authentication.
-
-    Returns:
-        Auth cookies if authentication succeed.
-        None if OAUTH2 authentication method is not supported.
-
-    """
-    if "auth" not in config["url_suffix"]:
-        return None
-
-    base_url = config["service_url"]
-    auth_url = urljoin(base_url, config["url_suffix"]["auth"])
-    base_domain = urlparse(base_url).netloc
-    kerberos_auth = HTTPKerberosAuth(
-        mutual_authentication=DISABLED, sanitize_mutual_error_response=False
-    )
-    with requests.session() as http_session:
-        response = http_session.get(auth_url, auth=kerberos_auth, allow_redirects=True)
-        response.raise_for_status()
-
-        # Clear cookies from different from base_domain domains
-        for domain in http_session.cookies.list_domains():
-            if domain != base_domain:
-                http_session.cookies.clear(domain)
-
-        return http_session.cookies
+"""Script for various methods for auth nordea analytics library."""
+from urllib.parse import urljoin, urlparse
+
+import requests
+from requests import cookies
+from requests_kerberos import DISABLED, HTTPKerberosAuth  # type: ignore
+
+from nordea_analytics.nalib.util import get_config
+
+config = get_config()
+
+
+def authenticate() -> cookies.RequestsCookieJar:
+    """Function provide OAUTH2 authentication.
+
+    Returns:
+        Auth cookies if authentication succeed.
+        None if OAUTH2 authentication method is not supported.
+
+    """
+    if "auth" not in config["url_suffix"]:
+        return None
+
+    base_url = config["service_url"]
+    auth_url = urljoin(base_url, config["url_suffix"]["auth"])
+    base_domain = urlparse(base_url).netloc
+    kerberos_auth = HTTPKerberosAuth(
+        mutual_authentication=DISABLED, sanitize_mutual_error_response=False
+    )
+    with requests.session() as http_session:
+        response = http_session.get(auth_url, auth=kerberos_auth, allow_redirects=True)
+        response.raise_for_status()
+
+        # Clear cookies from different from base_domain domains
+        for domain in http_session.cookies.list_domains():
+            if domain != base_domain:
+                http_session.cookies.clear(domain)
+
+        return http_session.cookies
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/config.yml` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 url_suffix:
   benchmark_definition: "benchmark-definition"
   bond_key_figures: "bonds/keyfigure"
   calculate: "bonds-calculation"
   calculate_advanced: "bonds-advanced-calculation"
   calculate_horizon: "bonds-horizoncalculation"
+  calculate_repo: "bonds-repo-calculation"
   bond_static_data: "bonds/static-data"
   curve: "curves"
   curve_definition: "curves/definition"
   curve_time_series: "curves/timeseries"
   date_sequence: "date-sequence"
   fx_forecast: "fx-forecasts"
   fx_quotes: "fx-quotes"
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/config_test.yml` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/config_test.yml`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/exceptions.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/exceptions.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-from typing import Any
-import warnings
-
-STACKLEVEL = 2
-
-
-class HttpClientImproperlyConfigured(Exception):
-    """The http service is somehow improperly configured."""
-
-    pass
-
-
-class ApiServerUnauthorized(Exception):
-    """The server can't authorize request."""
-
-    pass
-
-
-class ApiServerError(Exception):
-    """Basic exception for all server errors."""
-
-    def __init__(self, error_id: str, error_description: str) -> None:
-        """Common base class for all Analytics API Server exceptions."""
-        self.error_id = error_id
-        super(ApiServerError, self).__init__(error_description)
-
-    def __str__(self) -> str:
-        """Return str(self)."""
-        return f"Error code: {self.error_id} -> {super(ApiServerError, self).__str__()}"
-
-
-class BackgroundCalculationFailed(ApiServerError, Exception):
-    """The server can't process the background calculation request."""
-
-    pass
-
-
-class BackgroundCalculationTimeout(Exception):
-    """Throw when the time allotted for a background calculation has expired."""
-
-    pass
-
-
-class AnalyticsResponseError(Exception):
-    """Throw when response from Analytics API is not as expected."""
-
-    pass
-
-
-class AnalyticsInputError(Exception):
-    """Throw when input to Analytics API is not as expected."""
-
-    pass
-
-
-class AnalyticsWarning(Warning):
-    """Category which is used for Analytics warnings only."""
-
-    pass
-
-
-class CustomWarning(Warning):
-    """Throw custom instead of standard warning to indicate warning came from Analytics API."""
-
-    def __init__(self, message: str, category: Any) -> None:
-        """Create new instance of class.
-
-        Args:
-            message: warning message.
-            category: warning category.
-        """
-        self.message = message
-        warnings.warn(self.message, category=category, stacklevel=STACKLEVEL)
-
-
-class CustomWarningCheck:
-    """Class for containing custom warning messages."""
-
-    @staticmethod
-    def curve_not_retrieved_warning(response: dict, curve: str) -> None:
-        """Throw warning when curve time series does not return anything."""
-        if len(response["curve"]["curve"]["values"]) == 0:
-            message = curve + " could not be retrieved."
-            CustomWarning(message, AnalyticsWarning)
-
-    @staticmethod
-    def curve_time_series_not_retrieved_warning(response: dict, curve: str) -> None:
-        """Throw warning when curve time series does not return anything."""
-        if "timeseries" in response and len(response["timeseries"]) == 0:
-            message = curve + " could not be retrieved."
-            CustomWarning(message, AnalyticsWarning)
-
-    @staticmethod
-    def live_key_figure_access_restricted(response: dict) -> None:
-        """Throw warning when bond live key figures response includes bonds with no data available."""
-        if "access_restricted" in response and len(response["access_restricted"]) > 0:
-            message = f"Access restricted to the following bonds: {', '.join(response['access_restricted'])}"
-            CustomWarning(message, AnalyticsWarning)
-
-    @staticmethod
-    def live_key_figure_calculation_not_supported_warning(response: dict) -> None:
-        """Throw warning when bond live key figures response includes bonds that are not supported."""
-        if "not_supported" in response and len(response["not_supported"]) > 0:
-            message = f"The following bonds are not supported for live calculation: {', '.join(response['not_supported'])}"
-            CustomWarning(message, AnalyticsWarning)
-
-    @staticmethod
-    def live_key_figure_data_not_available_warning(response: dict) -> None:
-        """Throw warning when bond live key figures response includes bonds with no data available."""
-        if "data_not_available" in response and len(response["data_not_available"]) > 0:
-            message = f"No data available for the following bonds: {', '.join(response['data_not_available'])}"
-            CustomWarning(message, AnalyticsWarning)
-
-    @staticmethod
-    def live_key_figure_no_data_closing_down_warning() -> None:
-        """Throw warning when bond live key figures have no data for 10 minutes."""
-        message = "No data have been received for 10 minutes, closing down the service."
-        CustomWarning(message, AnalyticsWarning)
-
-    @staticmethod
-    def post_response_not_retrieved_warning(error: Exception, symbol: str) -> None:
-        """Throw warning when post response throws exception to ensure result from remaining bonds is returned."""
-        error_code = error.error_id if isinstance(error, ApiServerError) else ""
-        if len(error.args) > 0 and "Failed to retrieve bond.":
-            message = f"{symbol} could not be retrieved, {error.args[0]} Error code: {error_code}"
-            CustomWarning(message, AnalyticsWarning)
+from typing import Any
+import warnings
+
+STACKLEVEL = 2
+
+
+class HttpClientImproperlyConfigured(Exception):
+    """The http service is somehow improperly configured."""
+
+    pass
+
+
+class ApiServerUnauthorized(Exception):
+    """The server can't authorize request."""
+
+    pass
+
+
+class ApiServerError(Exception):
+    """Basic exception for all server errors."""
+
+    def __init__(self, error_id: str, error_description: str) -> None:
+        """Common base class for all Analytics API Server exceptions."""
+        self.error_id = error_id
+        super(ApiServerError, self).__init__(error_description)
+
+    def __str__(self) -> str:
+        """Return str(self)."""
+        return f"Error code: {self.error_id} -> {super(ApiServerError, self).__str__()}"
+
+
+class BackgroundCalculationFailed(ApiServerError, Exception):
+    """The server can't process the background calculation request."""
+
+    pass
+
+
+class BackgroundCalculationTimeout(Exception):
+    """Throw when the time allotted for a background calculation has expired."""
+
+    pass
+
+
+class AnalyticsResponseError(Exception):
+    """Throw when response from Analytics API is not as expected."""
+
+    pass
+
+
+class AnalyticsInputError(Exception):
+    """Throw when input to Analytics API is not as expected."""
+
+    pass
+
+
+class AnalyticsWarning(Warning):
+    """Category which is used for Analytics warnings only."""
+
+    pass
+
+
+class CustomWarning(Warning):
+    """Throw custom instead of standard warning to indicate warning came from Analytics API."""
+
+    def __init__(self, message: str, category: Any) -> None:
+        """Create new instance of class.
+
+        Args:
+            message: warning message.
+            category: warning category.
+        """
+        self.message = message
+        warnings.warn(self.message, category=category, stacklevel=STACKLEVEL)
+
+
+class CustomWarningCheck:
+    """Class for containing custom warning messages."""
+
+    @staticmethod
+    def curve_not_retrieved_warning(response: dict, curve: str) -> None:
+        """Throw warning when curve time series does not return anything."""
+        if len(response["curve"]["curve"]["values"]) == 0:
+            message = curve + " could not be retrieved."
+            CustomWarning(message, AnalyticsWarning)
+
+    @staticmethod
+    def curve_time_series_not_retrieved_warning(response: dict, curve: str) -> None:
+        """Throw warning when curve time series does not return anything."""
+        if "timeseries" in response and len(response["timeseries"]) == 0:
+            message = curve + " could not be retrieved."
+            CustomWarning(message, AnalyticsWarning)
+
+    @staticmethod
+    def live_key_figure_access_restricted(response: dict) -> None:
+        """Throw warning when bond live key figures response includes bonds with no data available."""
+        if "access_restricted" in response and len(response["access_restricted"]) > 0:
+            message = f"Access restricted to the following bonds: {', '.join(response['access_restricted'])}"
+            CustomWarning(message, AnalyticsWarning)
+
+    @staticmethod
+    def live_key_figure_calculation_not_supported_warning(response: dict) -> None:
+        """Throw warning when bond live key figures response includes bonds that are not supported."""
+        if "not_supported" in response and len(response["not_supported"]) > 0:
+            message = f"The following bonds are not supported for live calculation: {', '.join(response['not_supported'])}"
+            CustomWarning(message, AnalyticsWarning)
+
+    @staticmethod
+    def live_key_figure_data_not_available_warning(response: dict) -> None:
+        """Throw warning when bond live key figures response includes bonds with no data available."""
+        if "data_not_available" in response and len(response["data_not_available"]) > 0:
+            message = f"No data available for the following bonds: {', '.join(response['data_not_available'])}"
+            CustomWarning(message, AnalyticsWarning)
+
+    @staticmethod
+    def live_key_figure_no_data_closing_down_warning() -> None:
+        """Throw warning when bond live key figures have no data for 10 minutes."""
+        message = "No data have been received for 10 minutes, closing down the service."
+        CustomWarning(message, AnalyticsWarning)
+
+    @staticmethod
+    def post_response_not_retrieved_warning(error: Exception, symbol: str) -> None:
+        """Throw warning when post response throws exception to ensure result from remaining bonds is returned."""
+        error_code = error.error_id if isinstance(error, ApiServerError) else ""
+        if len(error.args) > 0 and "Failed to retrieve bond.":
+            message = f"{symbol} could not be retrieved, {error.args[0]} Error code: {error_code}"
+            CustomWarning(message, AnalyticsWarning)
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/live_keyfigures/open_banking.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/live_keyfigures/open_banking.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import datetime
-from threading import Event
-from typing import Any, Iterator, List
-import urllib.parse
-
-import requests
-
-from nordea_analytics.nalib.http.core import RestApiHttpClient
-from nordea_analytics.nalib.live_keyfigures.core import HttpStreamIterator
-
-URL_SUFFIX = "bonds/live-keyfigures"
-
-
-class OpenBankingHttpStreamIterator(HttpStreamIterator):
-    """Contain methods to create iterator for request/response live keyfigures streaming."""
-
-    def __init__(
-        self,
-        http_client: RestApiHttpClient,
-        interval_between_requests_sec: int = 5,
-        stream_suffix: str = URL_SUFFIX,
-    ) -> None:
-        """Constructs an :class:`OpenBankingHttpStreamIterator <OpenBankingHttpStreamIterator>`.
-
-        Args:
-            http_client: instance of RestApiHttpClient which will perform HTTP requests.
-            interval_between_requests_sec: minimal interval between requests.
-            stream_suffix: url where the HTTP stream is located.
-        """
-        self.http_client = http_client
-        self.interval_in_sec = interval_between_requests_sec
-        self.stream_suffix: str = stream_suffix
-        self._last_request = datetime.datetime.min
-
-    def __enter__(self) -> HttpStreamIterator:
-        """Entry to the body of the 'with' statement."""
-        return self
-
-    def __exit__(self, exc_type: None, exc_val: None, exc_tb: None) -> None:
-        """Exit from the body of the 'with' statement."""
-        pass
-
-    def stream(self, bonds: List) -> Iterator[Any]:
-        """Return Iterator for request/response HTTP streaming that request updates from a server within an interval.
-
-        Args:
-            bonds: List of Bonds to request updates for.
-
-        Raises:
-            StopIteration: when iterator failed to proceed response from server.
-
-        Yields:
-            Iterate over HTTP stream.
-        """
-        params = {"bonds": str.join(",", bonds)}
-        stream_url = f"{self.stream_suffix}?{urllib.parse.urlencode(params)}"
-        sleep_event = Event()
-        sleep_event.clear()
-
-        while True:
-            # Sleep if too many requests per second
-            interval_between_requests = datetime.datetime.utcnow() - self._last_request
-            if interval_between_requests.total_seconds() < self.interval_in_sec:
-                sleep_event.wait(
-                    self.interval_in_sec - interval_between_requests.total_seconds()
-                )
-            self._last_request = datetime.datetime.utcnow()
-
-            response = self.http_client.get(stream_url)
-            try:
-                response.raise_for_status()
-            except requests.models.HTTPError as e:
-                raise StopIteration("Failed to read from remote server") from e
-
-            yield response.text
+import datetime
+from threading import Event
+from typing import Any, Iterator, List
+import urllib.parse
+
+import requests
+
+from nordea_analytics.nalib.http.core import RestApiHttpClient
+from nordea_analytics.nalib.live_keyfigures.core import HttpStreamIterator
+
+URL_SUFFIX = "bonds/live-keyfigures"
+
+
+class OpenBankingHttpStreamIterator(HttpStreamIterator):
+    """Contain methods to create iterator for request/response live keyfigures streaming."""
+
+    def __init__(
+        self,
+        http_client: RestApiHttpClient,
+        interval_between_requests_sec: int = 5,
+        stream_suffix: str = URL_SUFFIX,
+    ) -> None:
+        """Constructs an :class:`OpenBankingHttpStreamIterator <OpenBankingHttpStreamIterator>`.
+
+        Args:
+            http_client: instance of RestApiHttpClient which will perform HTTP requests.
+            interval_between_requests_sec: minimal interval between requests.
+            stream_suffix: url where the HTTP stream is located.
+        """
+        self.http_client = http_client
+        self.interval_in_sec = interval_between_requests_sec
+        self.stream_suffix: str = stream_suffix
+        self._last_request = datetime.datetime.min
+
+    def __enter__(self) -> HttpStreamIterator:
+        """Entry to the body of the 'with' statement."""
+        return self
+
+    def __exit__(self, exc_type: None, exc_val: None, exc_tb: None) -> None:
+        """Exit from the body of the 'with' statement."""
+        pass
+
+    def stream(self, bonds: List) -> Iterator[Any]:
+        """Return Iterator for request/response HTTP streaming that request updates from a server within an interval.
+
+        Args:
+            bonds: List of Bonds to request updates for.
+
+        Raises:
+            StopIteration: when iterator failed to proceed response from server.
+
+        Yields:
+            Iterate over HTTP stream.
+        """
+        params = {"bonds": str.join(",", bonds)}
+        stream_url = f"{self.stream_suffix}?{urllib.parse.urlencode(params)}"
+        sleep_event = Event()
+        sleep_event.clear()
+
+        while True:
+            # Sleep if too many requests per second
+            interval_between_requests = datetime.datetime.utcnow() - self._last_request
+            if interval_between_requests.total_seconds() < self.interval_in_sec:
+                sleep_event.wait(
+                    self.interval_in_sec - interval_between_requests.total_seconds()
+                )
+            self._last_request = datetime.datetime.utcnow()
+
+            response = self.http_client.get(stream_url)
+            try:
+                response.raise_for_status()
+            except requests.models.HTTPError as e:
+                raise StopIteration("Failed to read from remote server") from e
+
+            yield response.text
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/proxy_finder.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/proxy_finder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,239 +1,242 @@
-import ast
-import ctypes.wintypes
-from pathlib import Path
-import platform
-from typing import Any, Dict, Union
-import urllib.parse
-import urllib.request
-
-
-class ProxyFinder:
-    """Retrieves proxy information when needed."""
-
-    def __init__(self, url: str, proxy_path: Path = None) -> None:
-        """Initialization of the class.
-
-        Args:
-            url: URL that needs a proxy.
-            proxy_path: Path where proxy information is saved.
-        """
-        self.proxy_path = (
-            Path(__file__).parent / ".proxy_info" if proxy_path is None else proxy_path
-        )
-        self.proxies: Union[Dict, str] = self.get_proxies(url)
-
-    def get_proxies(self, url: str) -> Union[Dict, str]:
-        """Find proxy information either from pre-saved place or searched for it.
-
-        Args:
-            url: URL that needs a proxy.
-
-        Returns:
-            Proxy information.
-
-        Raises:
-            LookupError: If proxy information need to be written in manually.
-        """
-        if self.proxy_path.exists():
-            proxy_info = self.proxy_path.read_text()
-            return ast.literal_eval(proxy_info)
-        else:
-            proxy_info = self.find_proxies(url)
-            if proxy_info == {} or "http://None" in proxy_info.values():  # type:ignore
-                self.proxy_path.write_text(
-                    str('{"http":"ENTER PROXY INFO HERE IN A STRING FORMAT"}')
-                )
-                raise LookupError(
-                    "We were not able to find your proxy information, "
-                    "please enter them manually in " + str(self.proxy_path)
-                )
-            else:
-                self.proxy_path.write_text(str(proxy_info))
-            return proxy_info
-
-    @staticmethod
-    def find_proxies(url: str) -> Any:
-        """Searches for proxy information.
-
-        Args:
-            url: URL that needs a proxy.
-
-        Returns:
-            Proxy information.
-        """
-        proxies = urllib.request.getproxies()
-        if platform.system() != "Windows":
-            return proxies
-
-        session_handle = None
-        try:
-            ctypes_struct = CtypesStructure(url)
-            if ctypes_struct.session_handle == 0 or ctypes_struct.session_handle == -1:
-                return {}
-
-            current_user_ie_proxy_config = ctypes_struct.current_user_ie_proxy_config
-
-            auto_proxy_settings = current_user_ie_proxy_config.lpszAutoConfigUrl
-            proxy_info = ctypes_struct.proxy_info
-            # parse protocol
-            if url is None:
-                return {}
-            parsed_url = urllib.parse.urlparse(url)
-            session_handle = ctypes_struct.session_handle
-            if "https" in auto_proxy_settings:
-                url_prefix = "https"
-            else:
-                url_prefix = "http"
-            return {
-                parsed_url.scheme: "{url}://{info}".format(
-                    url=url_prefix, info=proxy_info.lpszProxy
-                )
-            }
-        finally:
-            if session_handle:
-                ctypes.windll.winhttp.WinHttpCloseHandle.argtypes = (
-                    ctypes.wintypes.HANDLE,
-                )
-                ctypes.windll.winhttp.WinHttpCloseHandle(session_handle)
-
-
-class CtypesStructure:
-    """Find proxy information using the Web Proxy Auto-discovery Protocol."""
-
-    def __init__(self, url: str) -> None:
-        """nitialization of the class.
-
-        Args:
-            url: URL that needs a proxy.
-        """
-        # https://docs.microsoft.com/en-us/windows/win32/winhttp/winhttp-autoproxy-api
-        self.url = url
-        self.winhttp_access_type_no_proxy = 0x00000001
-        self.winhttp_no_proxy_name = 0
-        self.winhttp_no_proxy_bypass = 0
-        self.winhttp_autoproxy_auto_detect = 0x00000001
-        self.winhttp_autoproxy_config_url = 0x00000002
-        self.winhttp_auto_detect_type_dhcp = 0x00000001
-        self.winhttp_auto_detect_type_dns_a = 0x00000002
-        self.winHttp = ctypes.windll.winhttp
-        self.session_handle = self._get_session_handle()
-        self.current_user_ie_proxy_config = self._get_current_user_ie_proxy_config()
-        self.autoproxy_options = self._get_autoproxy_options()
-        self.proxy_info = self._get_proxy_info()
-
-    def _get_session_handle(self) -> int:
-        """Retrieves session handle.
-
-        Returns:
-            Session handle.
-
-        """
-        # https://docs.microsoft.com/en-gb/windows/win32/api/winhttp/
-        # nf-winhttp-winhttpopen
-        self.winHttp.WinHttpOpen.restype = ctypes.wintypes.HANDLE
-        session_handle = self.winHttp.WinHttpOpen(
-            "WinHTTP AutoProxy/1.0",
-            self.winhttp_access_type_no_proxy,
-            self.winhttp_no_proxy_name,
-            self.winhttp_no_proxy_bypass,
-            0,
-        )
-        return session_handle
-
-    def _get_current_user_ie_proxy_config(self) -> Any:
-        """Retrieves current user proxy config.
-
-        Returns:
-            Current user proxy config.
-        """
-        # https://docs.microsoft.com/en-us/windows/win32/api/winhttp/
-        # ns-winhttp-winhttp_current_user_ie_proxy_config
-        class WINHTTP_CURRENT_USER_IE_PROXY_CONFIG(ctypes.Structure):
-            _fields_ = [
-                ("fAutoDetect", ctypes.wintypes.BOOL),
-                ("lpszAutoConfigUrl", ctypes.wintypes.LPWSTR),
-                ("lpszProxy", ctypes.wintypes.LPWSTR),
-                ("lpszProxyBypass", ctypes.wintypes.LPWSTR),
-            ]
-
-        current_user_ie_proxy_config = WINHTTP_CURRENT_USER_IE_PROXY_CONFIG()
-        self.winHttp.WinHttpGetIEProxyConfigForCurrentUser(
-            ctypes.pointer(current_user_ie_proxy_config)
-        )
-        return current_user_ie_proxy_config
-
-    def _get_autoproxy_options(self) -> Any:
-        """Retrieves auto proxy options.
-
-        Returns:
-            Auto proxy options.
-        """
-        # https://docs.microsoft.com/en-us/windows/win32/api/winhttp/
-        # ns-winhttp-winhttp_autoproxy_options
-        class WINHTTP_AUTOPROXY_OPTIONS(ctypes.Structure):
-            _fields_ = [
-                ("dwFlags", ctypes.wintypes.DWORD),
-                ("dwAutoDetectFlags", ctypes.wintypes.DWORD),
-                ("lpszAutoConfigUrl", ctypes.wintypes.LPCWSTR),
-                ("lpvReserved", ctypes.wintypes.LPVOID),
-                ("dwReserved", ctypes.wintypes.DWORD),
-                ("fAutoLogonIfChallenged", ctypes.wintypes.BOOL),
-            ]
-
-        auto_config_url = self.current_user_ie_proxy_config.lpszAutoConfigUrl
-        auto_detect = self.current_user_ie_proxy_config.fAutoDetect == 1
-        autoproxy_options = WINHTTP_AUTOPROXY_OPTIONS()
-
-        autoproxy_options.dwFlags = (
-            self.winhttp_autoproxy_auto_detect if auto_detect else 0
-        ) | (self.winhttp_autoproxy_config_url if auto_config_url else 0)
-        autoproxy_options.dwAutoDetectFlags = (
-            self.winhttp_auto_detect_type_dhcp | self.winhttp_auto_detect_type_dns_a
-            if auto_detect
-            else 0
-        )
-        autoproxy_options.lpszAutoConfigUrl = auto_config_url
-        autoproxy_options.dwReserved = 0
-        autoproxy_options.fAutoLogonIfChallenged = 0
-        return autoproxy_options
-
-    def _get_proxy_info(self) -> Any:
-        """Retrieves proxy information.
-
-        Returns:
-            Proxy info.
-        """
-        # https://docs.microsoft.com/en-us/windows/win32/api/winhttp/
-        # ns-winhttp-winhttp_proxy_info
-        class WINHTTP_PROXY_INFO(ctypes.Structure):
-            _fields_ = [
-                ("dwAccessType", ctypes.wintypes.DWORD),
-                ("lpszProxy", ctypes.wintypes.LPWSTR),
-                ("lpszProxyBypass", ctypes.wintypes.LPWSTR),
-            ]
-
-        proxy_info = WINHTTP_PROXY_INFO()
-        self.winHttp.WinHttpGetProxyForUrl.argtypes = (
-            ctypes.wintypes.HANDLE,
-            ctypes.wintypes.LPCWSTR,
-            ctypes.POINTER(self.autoproxy_options.__class__),
-            ctypes.POINTER(WINHTTP_PROXY_INFO),
-        )
-        is_ok = self.winHttp.WinHttpGetProxyForUrl(
-            self.session_handle,
-            self.url,
-            ctypes.pointer(self.autoproxy_options),
-            ctypes.pointer(proxy_info),
-        )
-        # https://docs.microsoft.com/en-us/windows/win32/winhttp/error-messages
-        if not is_ok and ctypes.get_last_error() == 12015:
-            self.autoproxy_options.fAutoLogonIfChallenged = 1
-            is_ok = self.winHttp.WinHttpGetProxyForUrl(
-                self.session_handle,
-                self.url,
-                ctypes.pointer(self.autoproxy_options),
-                ctypes.pointer(proxy_info),
-            )
-            if not is_ok:
-                return {}
-        return proxy_info
+import ast
+import ctypes.wintypes
+from pathlib import Path
+import platform
+from typing import Any, Dict, Union
+import urllib.parse
+import urllib.request
+
+
+class ProxyFinder:
+    """Retrieves proxy information when needed."""
+
+    def __init__(self, url: str, proxy_path: Path = None) -> None:
+        """Initialization of the class.
+
+        Args:
+            url: URL that needs a proxy.
+            proxy_path: Path where proxy information is saved.
+        """
+        self.proxy_path = (
+            Path(__file__).parent / ".proxy_info" if proxy_path is None else proxy_path
+        )
+        self.proxies: Union[Dict, str] = self.get_proxies(url)
+
+    def get_proxies(self, url: str) -> Union[Dict, str]:
+        """Find proxy information either from pre-saved place or searched for it.
+
+        Args:
+            url: URL that needs a proxy.
+
+        Returns:
+            Proxy information.
+
+        Raises:
+            LookupError: If proxy information need to be written in manually.
+        """
+        if self.proxy_path.exists():
+            proxy_info = self.proxy_path.read_text()
+            return ast.literal_eval(proxy_info)
+        else:
+            proxy_info = self.find_proxies(url)
+            if proxy_info == {} or "http://None" in proxy_info.values():  # type:ignore
+                self.proxy_path.write_text(
+                    str('{"http":"ENTER PROXY INFO HERE IN A STRING FORMAT"}')
+                )
+                raise LookupError(
+                    "We were not able to find your proxy information, "
+                    "please enter them manually in " + str(self.proxy_path)
+                )
+            else:
+                self.proxy_path.write_text(str(proxy_info))
+            return proxy_info
+
+    @staticmethod
+    def find_proxies(url: str) -> Any:
+        """Searches for proxy information.
+
+        Args:
+            url: URL that needs a proxy.
+
+        Returns:
+            Proxy information.
+        """
+        proxies = urllib.request.getproxies()
+        if platform.system() != "Windows":
+            return proxies
+
+        session_handle = None
+        try:
+            ctypes_struct = CtypesStructure(url)
+            if ctypes_struct.session_handle == 0 or ctypes_struct.session_handle == -1:
+                return {}
+
+            current_user_ie_proxy_config = ctypes_struct.current_user_ie_proxy_config
+
+            auto_proxy_settings = current_user_ie_proxy_config.lpszAutoConfigUrl
+            proxy_info = ctypes_struct.proxy_info
+            # parse protocol
+            if url is None:
+                return {}
+            parsed_url = urllib.parse.urlparse(url)
+            session_handle = ctypes_struct.session_handle
+            if "https" in auto_proxy_settings:
+                url_prefix = "https"
+            else:
+                url_prefix = "http"
+            return {
+                parsed_url.scheme: "{url}://{info}".format(
+                    url=url_prefix, info=proxy_info.lpszProxy
+                )
+            }
+        finally:
+            if session_handle:
+                ctypes.windll.winhttp.WinHttpCloseHandle.argtypes = (
+                    ctypes.wintypes.HANDLE,
+                )
+                ctypes.windll.winhttp.WinHttpCloseHandle(session_handle)
+
+
+class CtypesStructure:
+    """Find proxy information using the Web Proxy Auto-discovery Protocol."""
+
+    def __init__(self, url: str) -> None:
+        """nitialization of the class.
+
+        Args:
+            url: URL that needs a proxy.
+        """
+        # https://docs.microsoft.com/en-us/windows/win32/winhttp/winhttp-autoproxy-api
+        self.url = url
+        self.winhttp_access_type_no_proxy = 0x00000001
+        self.winhttp_no_proxy_name = 0
+        self.winhttp_no_proxy_bypass = 0
+        self.winhttp_autoproxy_auto_detect = 0x00000001
+        self.winhttp_autoproxy_config_url = 0x00000002
+        self.winhttp_auto_detect_type_dhcp = 0x00000001
+        self.winhttp_auto_detect_type_dns_a = 0x00000002
+        self.winHttp = ctypes.windll.winhttp
+        self.session_handle = self._get_session_handle()
+        self.current_user_ie_proxy_config = self._get_current_user_ie_proxy_config()
+        self.autoproxy_options = self._get_autoproxy_options()
+        self.proxy_info = self._get_proxy_info()
+
+    def _get_session_handle(self) -> int:
+        """Retrieves session handle.
+
+        Returns:
+            Session handle.
+
+        """
+        # https://docs.microsoft.com/en-gb/windows/win32/api/winhttp/
+        # nf-winhttp-winhttpopen
+        self.winHttp.WinHttpOpen.restype = ctypes.wintypes.HANDLE
+        session_handle = self.winHttp.WinHttpOpen(
+            "WinHTTP AutoProxy/1.0",
+            self.winhttp_access_type_no_proxy,
+            self.winhttp_no_proxy_name,
+            self.winhttp_no_proxy_bypass,
+            0,
+        )
+        return session_handle
+
+    def _get_current_user_ie_proxy_config(self) -> Any:
+        """Retrieves current user proxy config.
+
+        Returns:
+            Current user proxy config.
+        """
+
+        # https://docs.microsoft.com/en-us/windows/win32/api/winhttp/
+        # ns-winhttp-winhttp_current_user_ie_proxy_config
+        class WINHTTP_CURRENT_USER_IE_PROXY_CONFIG(ctypes.Structure):
+            _fields_ = [
+                ("fAutoDetect", ctypes.wintypes.BOOL),
+                ("lpszAutoConfigUrl", ctypes.wintypes.LPWSTR),
+                ("lpszProxy", ctypes.wintypes.LPWSTR),
+                ("lpszProxyBypass", ctypes.wintypes.LPWSTR),
+            ]
+
+        current_user_ie_proxy_config = WINHTTP_CURRENT_USER_IE_PROXY_CONFIG()
+        self.winHttp.WinHttpGetIEProxyConfigForCurrentUser(
+            ctypes.pointer(current_user_ie_proxy_config)
+        )
+        return current_user_ie_proxy_config
+
+    def _get_autoproxy_options(self) -> Any:
+        """Retrieves auto proxy options.
+
+        Returns:
+            Auto proxy options.
+        """
+
+        # https://docs.microsoft.com/en-us/windows/win32/api/winhttp/
+        # ns-winhttp-winhttp_autoproxy_options
+        class WINHTTP_AUTOPROXY_OPTIONS(ctypes.Structure):
+            _fields_ = [
+                ("dwFlags", ctypes.wintypes.DWORD),
+                ("dwAutoDetectFlags", ctypes.wintypes.DWORD),
+                ("lpszAutoConfigUrl", ctypes.wintypes.LPCWSTR),
+                ("lpvReserved", ctypes.wintypes.LPVOID),
+                ("dwReserved", ctypes.wintypes.DWORD),
+                ("fAutoLogonIfChallenged", ctypes.wintypes.BOOL),
+            ]
+
+        auto_config_url = self.current_user_ie_proxy_config.lpszAutoConfigUrl
+        auto_detect = self.current_user_ie_proxy_config.fAutoDetect == 1
+        autoproxy_options = WINHTTP_AUTOPROXY_OPTIONS()
+
+        autoproxy_options.dwFlags = (
+            self.winhttp_autoproxy_auto_detect if auto_detect else 0
+        ) | (self.winhttp_autoproxy_config_url if auto_config_url else 0)
+        autoproxy_options.dwAutoDetectFlags = (
+            self.winhttp_auto_detect_type_dhcp | self.winhttp_auto_detect_type_dns_a
+            if auto_detect
+            else 0
+        )
+        autoproxy_options.lpszAutoConfigUrl = auto_config_url
+        autoproxy_options.dwReserved = 0
+        autoproxy_options.fAutoLogonIfChallenged = 0
+        return autoproxy_options
+
+    def _get_proxy_info(self) -> Any:
+        """Retrieves proxy information.
+
+        Returns:
+            Proxy info.
+        """
+
+        # https://docs.microsoft.com/en-us/windows/win32/api/winhttp/
+        # ns-winhttp-winhttp_proxy_info
+        class WINHTTP_PROXY_INFO(ctypes.Structure):
+            _fields_ = [
+                ("dwAccessType", ctypes.wintypes.DWORD),
+                ("lpszProxy", ctypes.wintypes.LPWSTR),
+                ("lpszProxyBypass", ctypes.wintypes.LPWSTR),
+            ]
+
+        proxy_info = WINHTTP_PROXY_INFO()
+        self.winHttp.WinHttpGetProxyForUrl.argtypes = (
+            ctypes.wintypes.HANDLE,
+            ctypes.wintypes.LPCWSTR,
+            ctypes.POINTER(self.autoproxy_options.__class__),
+            ctypes.POINTER(WINHTTP_PROXY_INFO),
+        )
+        is_ok = self.winHttp.WinHttpGetProxyForUrl(
+            self.session_handle,
+            self.url,
+            ctypes.pointer(self.autoproxy_options),
+            ctypes.pointer(proxy_info),
+        )
+        # https://docs.microsoft.com/en-us/windows/win32/winhttp/error-messages
+        if not is_ok and ctypes.get_last_error() == 12015:
+            self.autoproxy_options.fAutoLogonIfChallenged = 1
+            is_ok = self.winHttp.WinHttpGetProxyForUrl(
+                self.session_handle,
+                self.url,
+                ctypes.pointer(self.autoproxy_options),
+                ctypes.pointer(proxy_info),
+            )
+            if not is_ok:
+                return {}
+        return proxy_info
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/util.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,303 +1,306 @@
-"""Script for various methods for nordea analytics library."""
-from abc import ABC
-from enum import Enum
-import json
-from pathlib import Path
-from re import sub
-from typing import Callable, Dict, List, Mapping, Union
-
-import yaml
-
-from nordea_analytics import (
-    BenchmarkName,
-    BondIndexName,
-    BondKeyFigureName,
-    CalculatedBondKeyFigureName,
-    CashflowType,
-    CurveDefinitionName,
-    CurveName,
-    CurveType,
-    DateRollConvention,
-    DayCountConvention,
-    Exchange,
-    HorizonCalculatedBondKeyFigureName,
-    LiveBondKeyFigureName,
-    SpotForward,
-    TimeConvention,
-    TimeSeriesKeyFigureName,
-    YieldCountry,
-    YieldHorizon,
-    YieldType,
-)
-from nordea_analytics.nalib.exceptions import AnalyticsResponseError
-from nordea_analytics.search_bond_names import (
-    AmortisationType,
-    AssetType,
-    CapitalCentres,
-    CapitalCentreTypes,
-    InstrumentGroup,
-)
-
-
-def convert_to_float_if_float(string: str) -> Union[str, float]:
-    """Converts a given string to a float, if the string has a float format.
-
-    Args:
-        string: string that should maybe be converted.
-
-    Returns:
-         float value if possible, else the given string.
-    """
-    try:
-        return_value = float(string)
-        return return_value
-    except ValueError:
-        return string
-
-
-def convert_to_variable_string(
-    variable: Union[
-        str,
-        AmortisationType,
-        AssetType,
-        BenchmarkName,
-        BondIndexName,
-        BondKeyFigureName,
-        CalculatedBondKeyFigureName,
-        CapitalCentres,
-        CapitalCentreTypes,
-        CashflowType,
-        CurveDefinitionName,
-        CurveName,
-        CurveType,
-        DateRollConvention,
-        DayCountConvention,
-        Exchange,
-        HorizonCalculatedBondKeyFigureName,
-        InstrumentGroup,
-        LiveBondKeyFigureName,
-        SpotForward,
-        TimeConvention,
-        TimeSeriesKeyFigureName,
-        YieldCountry,
-        YieldType,
-        YieldHorizon,
-    ],
-    variable_type: Callable,
-) -> str:
-    """Convert of any variable name to string which is available in the service.
-
-    Args:
-        variable: variable which should be converted
-            and/or checked. Can be any of the variable
-            names or string.
-        variable_type: Called to check if string available in service.
-
-    Returns:
-        Variable name as a string that can be retrieved from the service.
-
-    Raises:
-        ValueError: If string value is not valid for service or variable
-            input not supported
-
-    """
-    if type(variable) in (
-        AmortisationType,
-        AssetType,
-        BenchmarkName,
-        BondIndexName,
-        BondKeyFigureName,
-        CalculatedBondKeyFigureName,
-        CapitalCentres,
-        CapitalCentreTypes,
-        CashflowType,
-        CurveDefinitionName,
-        CurveName,
-        CurveType,
-        DateRollConvention,
-        DayCountConvention,
-        Exchange,
-        HorizonCalculatedBondKeyFigureName,
-        InstrumentGroup,
-        LiveBondKeyFigureName,
-        TimeConvention,
-        TimeSeriesKeyFigureName,
-        SpotForward,
-        YieldCountry,
-        YieldType,
-        YieldHorizon,
-    ):
-        try:
-            variable_type(variable.value)  # type:ignore
-            return variable.value  # type:ignore
-        except ValueError as e:
-            raise e
-    elif type(variable) is str:
-        try:
-            if variable.lower() == "forward" or variable.lower() == "spot":
-                return variable.title()
-            elif variable.lower() == "impliedforward":
-                return "ImpliedForward"
-            elif (
-                # For enum types where string value is fully capitalised
-                variable_type == BenchmarkName
-                or variable_type == BondIndexName
-                or variable_type == CashflowType
-                or variable_type == CurveName
-                or variable_type == CurveDefinitionName
-                or variable_type == CapitalCentres
-                or variable_type == CapitalCentreTypes
-                or variable_type == Exchange
-                or variable_type == YieldCountry
-                or variable_type == YieldHorizon
-            ):
-                variable_type(variable.upper())
-                return variable.upper()
-            else:
-                # to cause ValueError when incorrect key figure is passed, e.g. "Quotes"
-                variable_type(variable.lower())
-                return variable.lower()
-        except ValueError as e:
-            raise e
-    else:
-        raise ValueError(str(type(variable)) + "as variable input not supported")
-
-
-def get_user(user_path: Path) -> str:
-    """Get user information from .user_info if available.
-
-    Args:
-        user_path: Path where .user_info should be saved.
-
-    Returns:
-        User info in form of string if available, else empty string.
-    """
-    if user_path.exists():
-        user_info = user_path.read_text()
-        return user_info
-    else:
-        return ""
-
-
-class ConfigContainer(ABC):
-    """Store config data."""
-
-    config: Dict = {}
-
-
-def get_config(config_path: str = None) -> Dict:
-    """Find and return the config file."""
-    if ConfigContainer.config and config_path is None:
-        return ConfigContainer.config
-
-    if not config_path:
-        config_path = str(Path(__file__).parent / "config.yml")
-    with open(config_path) as file:
-        ConfigContainer.config = yaml.safe_load(file)
-    return ConfigContainer.config
-
-
-def float_to_tenor_string(float_tenor: Union[str, float]) -> str:
-    """Convert float year fraction to tenor string."""
-    if float(float_tenor).is_integer():
-        return str(int(float(float_tenor))) + "Y"
-    else:
-        return str(float(float_tenor)) + "Y"
-
-
-def check_json_response(json_response: Union[List, Mapping]) -> bool:
-    """Check if json_response is empty and returns False, else True."""
-    if not json_response or (
-        type(json_response) == dict and all(not json_response[d] for d in json_response)
-    ):
-        return False
-    else:
-        return True
-
-
-def check_json_response_error(output_found: bool) -> None:
-    """Throws error if output in json_response isn't found."""
-    if not output_found:
-        raise AnalyticsResponseError(
-            "No data was retrieved! Please look if you have further "
-            "warning messages to identify the issue."
-        )
-
-
-def pretty_dict_string(d: Dict, indent: int = 4, sort_keys: bool = True) -> str:
-    """Print dict content as nice-formatted JSON string."""
-    return json.dumps(d, indent=indent, sort_keys=sort_keys) if d else "{}"
-
-
-def get_keyfigure_key(
-    key_figure: str,
-    key_figures_original: Union[
-        List[str],
-        List[CalculatedBondKeyFigureName],
-        List[Union[str, CalculatedBondKeyFigureName]],
-        List[HorizonCalculatedBondKeyFigureName],
-        List[Union[str, HorizonCalculatedBondKeyFigureName]],
-        List[LiveBondKeyFigureName],
-        List[Union[str, LiveBondKeyFigureName]],
-    ],
-    enum_type: str,
-) -> str:
-    """Get keyfigure key for dict."""
-    for kf_original in key_figures_original:
-        if key_figure == kf_original or (
-            type(key_figure) == str
-            and type(kf_original) == str
-            and key_figure.lower() == kf_original.lower()
-        ):
-            return str(kf_original)
-    try:
-        if enum_type == CalculatedBondKeyFigureName.__name__:
-            key_figure_key = CalculatedBondKeyFigureName(key_figure).name
-        elif enum_type == HorizonCalculatedBondKeyFigureName.__name__:
-            key_figure_key = HorizonCalculatedBondKeyFigureName(key_figure).name
-        elif enum_type == LiveBondKeyFigureName.__name__:
-            key_figure_key = LiveBondKeyFigureName(key_figure).name
-        else:
-            raise AnalyticsResponseError(
-                "Keyfigure enum type not handled explicitly, report this to package provider."
-            )
-    except Exception:
-        key_figure_key = key_figure
-
-    return key_figure_key
-
-
-def convert_to_original_format(
-    new: str,
-    originals: Union[List[Union[str, Enum]], List[str], List[Enum]],
-) -> str:
-    """Convert the output to be the same as the input."""
-    original = originals[
-        [
-            f.lower() if type(f) == str else f.value.lower()  # type:ignore
-            for f in originals
-        ].index(new.lower())
-    ]
-    if type(original) == str:
-        return original
-    else:
-        try:
-            return original.name  # type:ignore
-        except Exception:
-            AnalyticsResponseError(
-                "Conversion function not working properly, report this to package provider."
-            )
-            return new
-
-
-def pascal_case(s: str) -> str:
-    """Convert to PascalCase, only for formatting user output."""
-    s = sub(r"(_|-)+", " ", s).title().replace(" ", "")
-    return "".join([s[0].upper(), s[1:]])
-
-
-class RequestMethod(Enum):
-    """Enum for request methods."""
-
-    Get = 1
-    Post = 2
+"""Script for various methods for nordea analytics library."""
+from abc import ABC
+from enum import Enum
+import json
+from pathlib import Path
+from re import sub
+from typing import Callable, Dict, List, Mapping, Union
+
+import yaml
+
+from nordea_analytics import (
+    BenchmarkName,
+    BondIndexName,
+    BondKeyFigureName,
+    CalculatedBondKeyFigureName,
+    CashflowType,
+    CurveDefinitionName,
+    CurveName,
+    CurveType,
+    DateRollConvention,
+    DayCountConvention,
+    Exchange,
+    HorizonCalculatedBondKeyFigureName,
+    LiveBondKeyFigureName,
+    SpotForward,
+    TimeConvention,
+    TimeSeriesKeyFigureName,
+    YieldCountry,
+    YieldHorizon,
+    YieldType,
+)
+from nordea_analytics.key_figure_names import CalculatedRepoBondKeyFigureName
+from nordea_analytics.nalib.exceptions import AnalyticsResponseError
+from nordea_analytics.search_bond_names import (
+    AmortisationType,
+    AssetType,
+    CapitalCentres,
+    CapitalCentreTypes,
+    InstrumentGroup,
+)
+
+
+def convert_to_float_if_float(string: str) -> Union[str, float]:
+    """Converts a given string to a float, if the string has a float format.
+
+    Args:
+        string: string that should maybe be converted.
+
+    Returns:
+         float value if possible, else the given string.
+    """
+    try:
+        return_value = float(string)
+        return return_value
+    except ValueError:
+        return string
+
+
+def convert_to_variable_string(
+    variable: Union[
+        str,
+        AmortisationType,
+        AssetType,
+        BenchmarkName,
+        BondIndexName,
+        BondKeyFigureName,
+        CalculatedBondKeyFigureName,
+        CapitalCentres,
+        CapitalCentreTypes,
+        CashflowType,
+        CurveDefinitionName,
+        CurveName,
+        CurveType,
+        DateRollConvention,
+        DayCountConvention,
+        Exchange,
+        HorizonCalculatedBondKeyFigureName,
+        CalculatedRepoBondKeyFigureName,
+        InstrumentGroup,
+        LiveBondKeyFigureName,
+        SpotForward,
+        TimeConvention,
+        TimeSeriesKeyFigureName,
+        YieldCountry,
+        YieldType,
+        YieldHorizon,
+    ],
+    variable_type: Callable,
+) -> str:
+    """Convert of any variable name to string which is available in the service.
+
+    Args:
+        variable: variable which should be converted
+            and/or checked. Can be any of the variable
+            names or string.
+        variable_type: Called to check if string available in service.
+
+    Returns:
+        Variable name as a string that can be retrieved from the service.
+
+    Raises:
+        ValueError: If string value is not valid for service or variable
+            input not supported
+
+    """
+    if type(variable) in (
+        AmortisationType,
+        AssetType,
+        BenchmarkName,
+        BondIndexName,
+        BondKeyFigureName,
+        CalculatedBondKeyFigureName,
+        CapitalCentres,
+        CapitalCentreTypes,
+        CashflowType,
+        CurveDefinitionName,
+        CurveName,
+        CurveType,
+        DateRollConvention,
+        DayCountConvention,
+        Exchange,
+        HorizonCalculatedBondKeyFigureName,
+        CalculatedRepoBondKeyFigureName,
+        InstrumentGroup,
+        LiveBondKeyFigureName,
+        TimeConvention,
+        TimeSeriesKeyFigureName,
+        SpotForward,
+        YieldCountry,
+        YieldType,
+        YieldHorizon,
+    ):
+        try:
+            variable_type(variable.value)  # type:ignore
+            return variable.value  # type:ignore
+        except ValueError as e:
+            raise e
+    elif type(variable) is str:
+        try:
+            if variable.lower() == "forward" or variable.lower() == "spot":
+                return variable.title()
+            elif variable.lower() == "impliedforward":
+                return "ImpliedForward"
+            elif (
+                # For enum types where string value is fully capitalised
+                variable_type == BenchmarkName
+                or variable_type == BondIndexName
+                or variable_type == CashflowType
+                or variable_type == CurveName
+                or variable_type == CurveDefinitionName
+                or variable_type == CapitalCentres
+                or variable_type == CapitalCentreTypes
+                or variable_type == Exchange
+                or variable_type == YieldCountry
+                or variable_type == YieldHorizon
+            ):
+                variable_type(variable.upper())
+                return variable.upper()
+            else:
+                # to cause ValueError when incorrect key figure is passed, e.g. "Quotes"
+                variable_type(variable.lower())
+                return variable.lower()
+        except ValueError as e:
+            raise e
+    else:
+        raise ValueError(str(type(variable)) + "as variable input not supported")
+
+
+def get_user(user_path: Path) -> str:
+    """Get user information from .user_info if available.
+
+    Args:
+        user_path: Path where .user_info should be saved.
+
+    Returns:
+        User info in form of string if available, else empty string.
+    """
+    if user_path.exists():
+        user_info = user_path.read_text()
+        return user_info
+    else:
+        return ""
+
+
+class ConfigContainer(ABC):
+    """Store config data."""
+
+    config: Dict = {}
+
+
+def get_config(config_path: str = None) -> Dict:
+    """Find and return the config file."""
+    if ConfigContainer.config and config_path is None:
+        return ConfigContainer.config
+
+    if not config_path:
+        config_path = str(Path(__file__).parent / "config.yml")
+    with open(config_path) as file:
+        ConfigContainer.config = yaml.safe_load(file)
+    return ConfigContainer.config
+
+
+def float_to_tenor_string(float_tenor: Union[str, float]) -> str:
+    """Convert float year fraction to tenor string."""
+    if float(float_tenor).is_integer():
+        return str(int(float(float_tenor))) + "Y"
+    else:
+        return str(float(float_tenor)) + "Y"
+
+
+def check_json_response(json_response: Union[List, Mapping]) -> bool:
+    """Check if json_response is empty and returns False, else True."""
+    if not json_response or (
+        type(json_response) == dict and all(not json_response[d] for d in json_response)
+    ):
+        return False
+    else:
+        return True
+
+
+def check_json_response_error(output_found: bool) -> None:
+    """Throws error if output in json_response isn't found."""
+    if not output_found:
+        raise AnalyticsResponseError(
+            "No data was retrieved! Please look if you have further "
+            "warning messages to identify the issue."
+        )
+
+
+def pretty_dict_string(d: Dict, indent: int = 4, sort_keys: bool = True) -> str:
+    """Print dict content as nice-formatted JSON string."""
+    return json.dumps(d, indent=indent, sort_keys=sort_keys) if d else "{}"
+
+
+def get_keyfigure_key(
+    key_figure: str,
+    key_figures_original: Union[
+        List[str],
+        List[CalculatedBondKeyFigureName],
+        List[Union[str, CalculatedBondKeyFigureName]],
+        List[HorizonCalculatedBondKeyFigureName],
+        List[Union[str, HorizonCalculatedBondKeyFigureName]],
+        List[LiveBondKeyFigureName],
+        List[Union[str, LiveBondKeyFigureName]],
+    ],
+    enum_type: str,
+) -> str:
+    """Get keyfigure key for dict."""
+    for kf_original in key_figures_original:
+        if key_figure == kf_original or (
+            type(key_figure) == str
+            and type(kf_original) == str
+            and key_figure.lower() == kf_original.lower()
+        ):
+            return str(kf_original)
+    try:
+        if enum_type == CalculatedBondKeyFigureName.__name__:
+            key_figure_key = CalculatedBondKeyFigureName(key_figure).name
+        elif enum_type == HorizonCalculatedBondKeyFigureName.__name__:
+            key_figure_key = HorizonCalculatedBondKeyFigureName(key_figure).name
+        elif enum_type == LiveBondKeyFigureName.__name__:
+            key_figure_key = LiveBondKeyFigureName(key_figure).name
+        else:
+            raise AnalyticsResponseError(
+                "Keyfigure enum type not handled explicitly, report this to package provider."
+            )
+    except Exception:
+        key_figure_key = key_figure
+
+    return key_figure_key
+
+
+def convert_to_original_format(
+    new: str,
+    originals: Union[List[Union[str, Enum]], List[str], List[Enum]],
+) -> str:
+    """Convert the output to be the same as the input."""
+    original = originals[
+        [
+            f.lower() if type(f) == str else f.value.lower()  # type:ignore
+            for f in originals
+        ].index(new.lower())
+    ]
+    if type(original) == str:
+        return original
+    else:
+        try:
+            return original.name  # type:ignore
+        except Exception:
+            AnalyticsResponseError(
+                "Conversion function not working properly, report this to package provider."
+            )
+            return new
+
+
+def pascal_case(s: str) -> str:
+    """Convert to PascalCase, only for formatting user output."""
+    s = sub(r"(_|-)+", " ", s).title().replace(" ", "")
+    return "".join([s[0].upper(), s[1:]])
+
+
+class RequestMethod(Enum):
+    """Enum for request methods."""
+
+    Get = 1
+    Post = 2
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondFinder.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondFinder.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,38 @@
     Issuers,
 )
 
 config = get_config()
 
 
 class BondFinder(ValueRetriever):
-    """Retrieves and reformat bonds given a search criteria."""
+    """Retrieves and reformats bonds given search criteria.
+
+    Args:
+        client: The client used to retrieve data.
+        dmb: Defaults to False. True if only Danish Mortgage Bonds should be found.
+        country: Country of issue.
+        currency: Issue currency.
+        issuers: Name of issuers.
+        asset_types: Type of asset.
+        instrument_groups: Type of instrument.
+        lower_issue_date: Minimum (from) issue date.
+        upper_issue_date: Maximum (to) issue date.
+        lower_maturity: Minimum (from) maturity.
+        upper_maturity: Maximum (to) maturity.
+        lower_closing_date: Minimum(from) closing date - only applicable for DMB.
+        upper_closing_date: Maximum(to) closing date - only applicable for DMB.
+        lower_coupon: Minimum coupon.
+        upper_coupon: Maximum coupon.
+        amortisation_type: Amortisation type of bond.
+        capital_centres: Capital centres names - only applicable for DMB.
+        capital_centre_types: Capital centres types - only applicable for DMB.
+        lower_outstanding_amount: Minimum outstanding amount - only applicable for DMB.
+        upper_outstanding_amount: Maximum outstanding amount - only applicable for DMB.
+    """
 
     def __init__(
         self,
         client: DataRetrievalServiceClient,
         dmb: bool = False,
         country: Optional[str] = None,
         currency: Optional[str] = None,
@@ -78,40 +101,37 @@
                 List[str],
                 List[Union[CapitalCentreTypes, str]],
             ]
         ] = None,
         lower_outstanding_amount: Optional[float] = None,
         upper_outstanding_amount: Optional[float] = None,
     ) -> None:
-        """Initialization of class.
+        """Initialize the BondFinder class.
 
         Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            dmb: Default to False. True if only Danish Mortgage
-                Bonds should be found.
+            client: The client used to retrieve data.
+            dmb: True if only Danish Mortgage Bonds should be found, False otherwise.
             country: Country of issue.
             currency: Issue currency.
             issuers: Name of issuers.
             asset_types: Type of asset.
             instrument_groups: Type of instrument.
             lower_issue_date: Minimum (from) issue date.
             upper_issue_date: Maximum (to) issue date.
             lower_maturity: Minimum (from) maturity.
             upper_maturity: Maximum (to) maturity.
-            lower_closing_date: Minimum(from) closing date - only applicable for DMB.
-            upper_closing_date: Maximum(to) closing date - only applicable for DMB.
+            lower_closing_date: Minimum (from) closing date - only applicable for DMB.
+            upper_closing_date: Maximum (to) closing date - only applicable for DMB.
             lower_coupon: Minimum coupon.
             upper_coupon: Maximum coupon.
             amortisation_type: Amortisation type of bond.
             capital_centres: Capital centres names - only applicable for DMB.
             capital_centre_types: Capital centres types - only applicable for DMB.
             lower_outstanding_amount: Minimum outstanding amount - only applicable for DMB.
             upper_outstanding_amount: Maximum outstanding amount - only applicable for DMB.
-
         """
         super(BondFinder, self).__init__(client)
         self._client = client
         self.dmb = dmb
         self.country = country
         self.currency = currency
         self.issuers = issuers
@@ -216,38 +236,63 @@
         self.upper_outstanding_amount = upper_outstanding_amount
 
         self.check_inputs()
 
         self._data = self.get_search_bonds()
 
     def get_search_bonds(self) -> Mapping:
-        """Retrieves response given the search criteria."""
+        """Retrieves the response from the API based on the search criteria.
+
+        Returns:
+            The JSON response containing the search results.
+        """
+        # Get the JSON response from the API using the request dictionary
         _json_response = self.get_response(self.request)
+
+        # Extract the search results from the JSON response
         json_response = _json_response[config["results"]["search"]]
 
         return json_response
 
     @staticmethod
     def check_response(json_response: Mapping) -> None:
-        """Checks if json_reponse contains output, else throws error."""
+        """Checks if the JSON response contains output, else throws an error.
+
+        Args:
+            json_response: The JSON response to be checked.
+        """
+        # Call the check_json_response() function to check if output is found
         output_found = check_json_response(json_response)
 
+        # Call the check_json_response_error() function to raise an error if output is not found
         check_json_response_error(output_found)
 
     @property
     def url_suffix(self) -> str:
-        """Url suffix suffix for a given method."""
+        """URL suffix for a given method.
+
+        Returns:
+            The URL suffix based on the value of self.dmb.
+        """
         if self.dmb:
             return config["url_suffix"]["search_dmb_bonds"]
         else:
             return config["url_suffix"]["search_bonds"]
 
     @property
     def request(self) -> Dict:
-        """Request dictionary for searched bonds."""
+        """Request dictionary for searched bonds.
+
+        Returns:
+            The request dictionary containing the search criteria.
+
+        Raises:
+            ValueError: Containing description of error.
+        """
+        # Create the initial request dictionary with all search criteria
         initial_request = {
             "country": self.country,
             "currency": self.currency,
             "issuers": self.issuers,
             "asset-types": self.asset_types,
             "instrument-groups": self.instrument_groups,
             "lower-issue-date": self.lower_issue_date,
@@ -261,61 +306,83 @@
             "amortisation-type": self.amortisation_type,
             "capital-centres": self.capital_centres,
             "capital-centre-types": self.capital_centre_types,
             "lower-outstanding-amount": self.lower_outstanding_amount,
             "upper-outstanding-amount": self.upper_outstanding_amount,
         }
 
+        # Filter out None values from the initial request dictionary
         request = {
             key: initial_request[key]
             for key in initial_request.keys()
             if initial_request[key] is not None
         }
+
+        # Raise an error if no search criteria is provided
         if request == {}:
             raise ValueError("You need to input some search criteria")
         return request
 
     def check_inputs(self) -> None:
-        """Check if inputs are given that only apply to dmb."""
-        if self.capital_centres is not None:
-            if not self.dmb:
-                warnings.warn(
-                    "capital_centres is only relevant for DMB. "
-                    "This variable will be ignored.",
-                    stacklevel=2,
-                )
-        if self.capital_centre_types is not None:
-            if not self.dmb:
-                warnings.warn(
-                    "capital_centre_types is only relevant for DMB."
-                    " This variable will be ignored.",
-                    stacklevel=2,
-                )
-        if self.lower_outstanding_amount is not None:
-            if not self.dmb:
-                warnings.warn(
-                    "lower_outstanding_amount is only relevant for DMB. "
-                    "This variable will be ignored.",
-                    stacklevel=2,
-                )
-        if self.upper_outstanding_amount is not None:
-            if not self.dmb:
-                warnings.warn(
-                    "upper_outstanding_amount is only relevant for DMB. "
-                    "This variable will be ignored.",
-                    stacklevel=2,
-                )
+        """Check if inputs are given that only apply to DMB.
+
+        Raises:
+            If inputs that only apply to DMB are provided when `dmb` is False.
+        """
+        if self.capital_centres is not None and not self.dmb:
+            # Raise warning if capital_centres is provided but `dmb` is False
+            warnings.warn(
+                "capital_centres is only relevant for DMB. This variable will be ignored.",
+                stacklevel=2,
+                category=UserWarning,
+            )
+        if self.capital_centre_types is not None and not self.dmb:
+            # Raise warning if capital_centre_types is provided but `dmb` is False
+            warnings.warn(
+                "capital_centre_types is only relevant for DMB. This variable will be ignored.",
+                stacklevel=2,
+                category=UserWarning,
+            )
+        if self.lower_outstanding_amount is not None and not self.dmb:
+            # Raise warning if lower_outstanding_amount is provided but `dmb` is False
+            warnings.warn(
+                "lower_outstanding_amount is only relevant for DMB. This variable will be ignored.",
+                stacklevel=2,
+                category=UserWarning,
+            )
+        if self.upper_outstanding_amount is not None and not self.dmb:
+            # Raise warning if upper_outstanding_amount is provided but `dmb` is False
+            warnings.warn(
+                "upper_outstanding_amount is only relevant for DMB. This variable will be ignored.",
+                stacklevel=2,
+                category=UserWarning,
+            )
 
     def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
+        """Reformat the JSON response to a dictionary.
+
+        Returns:
+            A dictionary containing the reformatted JSON response.
+        """
         _dict: Dict[Any, Any] = {}
         for i, search_data in enumerate(self._data):
+            # Create dictionary entry for each search data
             _dict[i] = {}
-            _dict[i]["ISIN"] = search_data["isin"]
-            _dict[i]["Name"] = search_data["name"]
+            _dict[i]["ISIN"] = search_data[
+                "isin"
+            ]  # Extract 'isin' key from search data
+            _dict[i]["Name"] = search_data[
+                "name"
+            ]  # Extract 'name' key from search data
         return _dict
 
     def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        _dict = self.to_dict()
-        df = pd.DataFrame.from_dict(_dict).transpose()
+        """Reformat the JSON response to a pandas DataFrame.
+
+        Returns:
+            A pandas DataFrame containing the reformatted JSON response.
+        """
+        _dict = self.to_dict()  # Convert JSON response to dictionary
+        df = pd.DataFrame.from_dict(
+            _dict
+        ).transpose()  # Create DataFrame from dictionary and transpose it
         return df
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureAdvancedCalculator.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureHorizonCalculator.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,302 +5,342 @@
 import pandas as pd
 
 from nordea_analytics.convention_variable_names import CashflowType
 from nordea_analytics.curve_variable_names import (
     CurveName,
 )
 from nordea_analytics.key_figure_names import (
-    CalculatedBondKeyFigureName,
+    HorizonCalculatedBondKeyFigureName,
 )
 from nordea_analytics.nalib.data_retrieval_client import (
     DataRetrievalServiceClient,
 )
 from nordea_analytics.nalib.exceptions import CustomWarningCheck
 from nordea_analytics.nalib.util import (
     convert_to_float_if_float,
+    convert_to_original_format,
     convert_to_variable_string,
     get_config,
-    get_keyfigure_key,
 )
 from nordea_analytics.nalib.value_retriever import ValueRetriever
 
 config = get_config()
 
 
-class BondKeyFigureAdvancedCalculator(ValueRetriever):
-    """Retrieves and reformat calculated bond key figure."""
+class BondKeyFigureHorizonCalculator(ValueRetriever):
+    """Retrieves and reformat calculated future bond key figure."""
 
     def __init__(
         self,
         client: DataRetrievalServiceClient,
         symbols: Union[str, List[str]],
         keyfigures: Union[
             str,
-            CalculatedBondKeyFigureName,
+            HorizonCalculatedBondKeyFigureName,
             List[str],
-            List[CalculatedBondKeyFigureName],
-            List[Union[str, CalculatedBondKeyFigureName]],
+            List[HorizonCalculatedBondKeyFigureName],
+            List[Union[str, HorizonCalculatedBondKeyFigureName]],
         ],
         calc_date: datetime,
-        curves: Optional[Union[List[str], str, CurveName, List[CurveName]]] = None,
+        horizon_date: datetime,
+        curves: Optional[
+            Union[
+                str,
+                CurveName,
+                List[str],
+                List[CurveName],
+                List[Union[str, CurveName]],
+            ]
+        ] = None,
         shift_tenors: Optional[Union[List[float], float]] = None,
         shift_values: Optional[Union[List[float], float]] = None,
         pp_speed: Optional[float] = None,
         prices: Optional[Union[float, List[float]]] = None,
-        spread: Optional[float] = None,
-        spread_curve: Optional[Union[str, CurveName]] = None,
-        yield_input: Optional[float] = None,
-        asw_fix_frequency: Optional[str] = None,
-        ladder_definition: Optional[Union[float, List[float]]] = None,
         cashflow_type: Optional[Union[str, CashflowType]] = None,
-        fixed_principal_payment: Optional[Union[str, List[str]]] = None,
-        volatility_date: Optional[datetime] = None,
-        refinancing_curve_date: Optional[datetime] = None,
+        fixed_prepayments: Optional[float] = None,
+        reinvest_in_series: Optional[bool] = None,
+        reinvestment_rate: Optional[float] = None,
+        spread_change_horizon: Optional[float] = None,
+        align_to_forward_curve: Optional[bool] = None,
     ) -> None:
         """Initialization of class.
 
         Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
+            client: The client used to retrieve data.
             symbols: ISIN or name of bonds that should be valued.
             keyfigures: Bond key figure that should be valued.
-            calc_date: Date of calculation.
-            curves: Discount curves for calculation.
+            calc_date: date of calculation
+            horizon_date: future date of calculation
+            curves: discount curves for calculation
             shift_tenors: Tenors to shift curves expressed as float. For example [0.25, 0.5, 1, 3, 5].
             shift_values: Shift values in basispoints. For example [100, 100, 75, 100, 100].
             pp_speed: Prepayment speed. Default = 1.
             prices: fixed price per bond.
-            spread: fixed spread for bond. Mandatory to give
-                spread_curve also as an input.
-            spread_curve: spread curve to calculate the
-                key figures when a fixed spread is given.
-            yield_input: fixed yield for bond.
-            asw_fix_frequency: Fixing frequency of swap in ASW calculation.
-                Mandatory input in all ASW calculations.
-            ladder_definition: Tenors should be included in
-                BPV ladder calculation. For example [0.25, 0.5, 1, 3, 5].
             cashflow_type: Type of cashflow to calculate with.
-            fixed_principal_payment: Principal payment each cash flow date.
-            volatility_date: Date of volatility surface.
-            refinancing_curve_date: Date of refinancing curve.
+            fixed_prepayments: repayments between calc_cate and horizon date.
+                Value of 0.01 would mean that prepayments are set to 1%,
+                but model prepayments are still used after horizon date.
+                If noting entered, then model prepayments used.
+            reinvest_in_series: True if you want to reinvest in the series.
+                Default value is True
+            reinvestment_rate: Rate you want to reinvest if you don't
+                want to reinvest in series. Only relevant if
+                    reinvest_in_series is False, or horizon date is
+                    further out than maturity of the bond.
+            spread_change_horizon: Bump the spread between calc date
+                and horizon date. Value should be in bps.
+            align_to_forward_curve: True if you want the curve used for horizon
+                calculations to be the respective forward curve.
+                Default is False.
         """
-        super(BondKeyFigureAdvancedCalculator, self).__init__(client)
+        super(BondKeyFigureHorizonCalculator, self).__init__(client)
         self._client = client
-        _keyfigures: List = keyfigures if type(keyfigures) == list else [keyfigures]
+        self.key_figures_original: List = (
+            keyfigures if isinstance(keyfigures, list) else [keyfigures]
+        )
         self.keyfigures = [
-            convert_to_variable_string(keyfigure, CalculatedBondKeyFigureName)
-            for keyfigure in _keyfigures
+            convert_to_variable_string(kf, HorizonCalculatedBondKeyFigureName)
+            if isinstance(kf, HorizonCalculatedBondKeyFigureName)
+            else kf.lower()
+            for kf in self.key_figures_original
         ]
-        self.symbols = [symbols] if type(symbols) == str else symbols
+
+        self.symbols = symbols if isinstance(symbols, list) else [symbols]
         self.calc_date = calc_date
-        self.key_figures_original: Union[
-            List[str],
-            List[CalculatedBondKeyFigureName],
-            List[Union[str, CalculatedBondKeyFigureName]],
-        ] = (
-            keyfigures if isinstance(keyfigures, list) else [keyfigures]
+        self.horizon_date = horizon_date
+        self.curves_original: Union[List, None] = (
+            curves
+            if isinstance(curves, list)
+            else [curves]
+            if isinstance(curves, str) or isinstance(curves, CurveName)
+            else None
         )
-        _curves: Union[List[Union[str, ValueError]], None]
+
+        _curves: Union[List[str], None]
         if isinstance(curves, list):
-            _curves = [convert_to_variable_string(curve, CurveName) for curve in curves]
+            _curves = [
+                convert_to_variable_string(curve, CurveName)
+                if isinstance(curve, CurveName)
+                else str(curve)
+                for curve in curves
+            ]
         elif curves is not None:
             # mypy doesn't know that curves in this line is never a list
             _curves = [convert_to_variable_string(curves, CurveName)]  # type: ignore
         else:
             _curves = None
 
         self.curves = _curves
-        self.shifts_tenors = shift_tenors
-        self.shifts_values = shift_values
+        self.shift_tenors = shift_tenors
+        self.shift_values = shift_values
         self.pp_speed = pp_speed
 
         _prices: Union[List[float], None]
         if isinstance(prices, list):
             _prices = prices
         elif prices is not None:
             _prices = [prices]
         else:
             _prices = None
 
         self.prices = _prices
-        self.spread = spread
-        _spread_curve = (
-            convert_to_variable_string(spread_curve, CurveName)
-            if spread_curve
-            else None
-        )
-        self.spread_curve = _spread_curve
-        self.yield_input = yield_input
-        self.asw_fix_frequency = asw_fix_frequency
-        self.ladder_definition = (
-            ladder_definition
-            if isinstance(ladder_definition, list)
-            else [ladder_definition]
-            if isinstance(ladder_definition, float)
-            or isinstance(ladder_definition, int)
-            else None
-        )
         self.cashflow_type = (
             convert_to_variable_string(cashflow_type, CashflowType)
             if cashflow_type is not None
             else None
         )
-        self.fixed_principal_payment = fixed_principal_payment
-        self.volatility_date = volatility_date
-        self.refinancing_curve_date = refinancing_curve_date
-
-        self._data = self.calculate_bond_key_figure()
-
-    def calculate_bond_key_figure(self) -> Mapping:
-        """Retrieves response with calculated key figures."""
-        json_response = self.get_post_get_response()
+        self.fixed_prepayments = fixed_prepayments
+        self.reinvest_in_series = reinvest_in_series
+        self.reinvestment_rate = reinvestment_rate
+        self.spread_change_horizon = spread_change_horizon
+        self.align_to_forward_curve = align_to_forward_curve
+        self.fixed_keyfigures = [
+            "price",
+            "price_at_horizon",
+            "return_interest",
+            "return_interest_amount",
+            "return_principal",
+            "return_principal_amount",
+            "prepayments",
+        ]
+
+        self._data = self.calculate_horizon_bond_key_figure()
+
+    def calculate_horizon_bond_key_figure(self) -> Mapping:
+        """Retrieves response with calculated key figures for horizon bond key figure calculation.
 
+        Returns:
+            A dictionary containing the calculated key figures, with symbols as keys and responses as values.
+        """
+        json_response = (
+            self.get_post_get_response()
+        )  # Call helper method to get response
         return json_response
 
     def get_post_get_response(self) -> Dict:
-        """Retrieves response after posting the request."""
+        """Retrieves response after posting the request to the API.
+
+        Returns:
+            A dictionary containing the response for each symbol in the request, with symbols as keys and responses as values.
+        """
         json_response: Dict = {}
         for request_dict in self.request:
             try:
+                # Call asynchronous method to get response and store it in json_response dictionary
                 _json_response = self._client.get_response_asynchronous(
                     request_dict, self.url_suffix
                 )
                 json_response[request_dict["symbol"]] = _json_response
             except Exception as ex:
+                # Catch and handle exceptions for unsuccessful responses
                 CustomWarningCheck.post_response_not_retrieved_warning(
                     ex, request_dict["symbol"]
                 )
-
         return json_response
 
     @property
     def url_suffix(self) -> str:
-        """Url suffix suffix for a given method."""
-        return config["url_suffix"]["calculate_advanced"]
+        """URL suffix for horizon bond key figure calculation.
+
+        Returns:
+            The URL suffix for the horizon bond key figure calculation method.
+        """
+        return config["url_suffix"]["calculate_horizon"]
 
     @property
     def request(self) -> List[Dict]:
-        """Post request dictionary calculate bond key figure."""
+        """Property that generates the post request dictionary for calculating bond key figures.
+
+        Returns:
+            A list of dictionaries, each containing the request parameters for a specific bond symbol.
+        """
         request_dict = []
         keyfigures = copy.deepcopy(self.keyfigures)
-        keyfigures.remove("price") if "price" in self.keyfigures else keyfigures
-        if keyfigures == []:  # There has to be some key figure in request,
-            # but it will not be returned in final results
-            keyfigures = "bpv"  # type:ignore
+        for kf in self.fixed_keyfigures:
+            if kf in self.keyfigures:
+                keyfigures.remove(kf)
+
+        if not keyfigures:
+            # There has to be at least one key figure in request,
+            # but it will not be returned in the final results
+            keyfigures = ["yield"]  # type:ignore
+
         for x in range(len(self.symbols)):
             initial_request = {
                 "symbol": self.symbols[x],
                 "date": self.calc_date.strftime("%Y-%m-%d"),
+                "horizon_date": self.horizon_date.strftime("%Y-%m-%d"),
                 "keyfigures": keyfigures,
                 "curves": self.curves,
-                "shift_tenors": self.shifts_tenors,
-                "shift_values": self.shifts_values,
+                "shift_tenors": self.shift_tenors,
+                "shift_values": self.shift_values,
                 "pp_speed": self.pp_speed,
                 "price": self.prices[x]
-                if self.prices is not None and x < len(self.prices)
+                if self.prices and x < len(self.prices)
                 else None,
-                "spread": self.spread,
-                "spread_curve": self.spread_curve,
-                "yield": self.yield_input,
-                "asw_fix_frequency": self.asw_fix_frequency,
-                "ladder_definition": self.ladder_definition,
                 "cashflow_type": self.cashflow_type,
-                "fixed_principal_payment": self.fixed_principal_payment,
-                "volatility_date": self.volatility_date.strftime("%Y-%m-%d")
-                if self.volatility_date is not None
-                else None,
-                "refinancing_curve_date": self.refinancing_curve_date.strftime(
-                    "%Y-%m-%d"
-                )
-                if self.refinancing_curve_date is not None
-                else None,
+                "fixed_prepayments": self.fixed_prepayments,
+                "reinvest_in_series": self.reinvest_in_series,
+                "reinvestment_rate": self.reinvestment_rate,
+                "spread_change_horizon": self.spread_change_horizon,
+                "align_to_forward_curve": self.align_to_forward_curve,
             }
             request = {
                 key: initial_request[key]
                 for key in initial_request.keys()
                 if initial_request[key] is not None
             }
             request_dict.append(request)
-
         return request_dict
 
     def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
+        """Convert the json response to a dictionary.
+
+        Returns:
+            A dictionary containing the bond data, with bond symbols as keys and bond information as values.
+        """
         _dict: Dict[Any, Any] = {}
         for symbol in self._data:
             bond_data = self._data[symbol]
             _dict_bond = self.to_dict_bond(bond_data)
             _dict[symbol] = _dict_bond
+
         return _dict
 
     def to_dict_bond(self, bond_data: Dict) -> Dict:
-        """to_dict function too complicated."""
+        """Convert bond_data to a dictionary with curve data.
+
+        Args:
+            bond_data (Dict): Bond data in JSON format.
+
+        Returns:
+            Dictionary with curve data extracted from bond_data.
+        """
         _dict_bond: Dict[Any, Any] = {}
         for key_figure in bond_data:
-            if key_figure != "price" and key_figure in self.keyfigures:
-                for curve_data in bond_data[key_figure]["values"]:
-                    _data_dict = {}
-                    if key_figure == "bpvladder":
-                        ladder_dict = {
-                            convert_to_float_if_float(
-                                ladder["key"]
-                            ): convert_to_float_if_float(ladder["value"])
-                            for ladder in curve_data["ladder"]
-                        }
-                        _data_dict[
-                            CalculatedBondKeyFigureName(key_figure).name
-                        ] = ladder_dict
-                    elif key_figure == "expectedcashflow":
-                        cashflow_dict = {
-                            cashflows["key"]: convert_to_float_if_float(
-                                cashflows["value"]
-                            )
-                            for cashflows in curve_data["cashflows"]
-                        }
-                        _data_dict[
-                            CalculatedBondKeyFigureName(key_figure).name
-                        ] = cashflow_dict
-                    elif key_figure == "vegamatrix":
-                        vega_dict = {
-                            vega_list["key"]: vega_list["value"]
-                            for vega_list in curve_data["vega_points"]
-                        }
-                        _data_dict[
-                            get_keyfigure_key(
-                                key_figure,
-                                self.key_figures_original,
-                                CalculatedBondKeyFigureName.__name__,
-                            )
-                        ] = vega_dict
-                    else:
-                        _data_dict[
-                            CalculatedBondKeyFigureName(key_figure).name
-                        ] = convert_to_float_if_float(
-                            curve_data["value"]
-                        )  # type:ignore
-                    if curve_data["key"] in _dict_bond.keys():
-                        _dict_bond[curve_data["key"]].update(_data_dict)
+            if (
+                "price" != key_figure
+                and "prepayments" != key_figure
+                and key_figure in self.keyfigures
+            ):
+                data = (
+                    bond_data[key_figure]
+                    if key_figure in self.fixed_keyfigures
+                    else bond_data[key_figure]["values"]
+                )
+                for curve_data in data:
+                    _data_dict: Dict[Any, Any] = {}
+                    formatted_result = convert_to_float_if_float(curve_data["value"])
+                    _data_dict[
+                        convert_to_original_format(
+                            key_figure, self.key_figures_original
+                        )
+                    ] = formatted_result
+                    curve_key = (
+                        CurveName(curve_data["key"].upper()).name
+                        if self.curves_original is None
+                        else convert_to_original_format(
+                            curve_data["key"], self.curves_original  # type:ignore
+                        )
+                    )
+                    if curve_key in _dict_bond.keys():
+                        _dict_bond[curve_key].update(_data_dict)
                     else:
-                        _dict_bond[curve_data["key"]] = _data_dict
-        if (
-            _dict_bond == {}
-        ):  # This would be the case if only Price would be selected as key figure
-            for curve_data in bond_data["bpv"]["values"]:
-                _dict_bond[curve_data["key"]] = {}
+                        _dict_bond[curve_key] = _data_dict
+
+        # This would be the case if only Price would be selected as key figure
+        # If not, price has no curve to be inserted into
+        if _dict_bond == {}:
+            _dict_bond["No curve found"] = {}
 
         if "price" in bond_data and "price" in self.keyfigures:
             for curve in _dict_bond:
                 _dict_bond[curve][
-                    CalculatedBondKeyFigureName("price").name
+                    convert_to_original_format("price", self.key_figures_original)
                 ] = bond_data["price"]
 
+        if "prepayments" in self.keyfigures and "prepayments" in bond_data:
+            for curve in _dict_bond:
+                _dict_bond[curve][
+                    convert_to_original_format("prepayments", self.key_figures_original)
+                ] = {
+                    convert_to_float_if_float(pp["key"]): convert_to_float_if_float(
+                        pp["value"]
+                    )
+                    for pp in bond_data["prepayments"]["values"]
+                }
+
         return _dict_bond
 
     def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
+        """Convert bond data to a pandas DataFrame.
+
+        Returns:
+            Pandas DataFrame with bond data.
+        """
         _dict = self.to_dict()
         df = pd.DataFrame()
         for symbol in _dict:
             _df = pd.DataFrame.from_dict(_dict[symbol]).transpose()
             _df = _df.reset_index().rename(columns={"index": "Curve"})
             _df.index = [symbol] * len(_df)
             df = pd.concat([df, _df], axis=0)
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureCalculator.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureCalculator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,457 +1,524 @@
-import copy
-from datetime import datetime
-from typing import Any, Dict, List, Mapping, Optional, Union
-
-import pandas as pd
-
-from nordea_analytics.convention_variable_names import CashflowType
-from nordea_analytics.curve_variable_names import (
-    CurveName,
-)
-from nordea_analytics.key_figure_names import (
-    CalculatedBondKeyFigureName,
-)
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.exceptions import CustomWarningCheck
-from nordea_analytics.nalib.util import (
-    convert_to_float_if_float,
-    convert_to_original_format,
-    convert_to_variable_string,
-    get_config,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class BondKeyFigureCalculator(ValueRetriever):
-    """Retrieves and reformat calculated bond key figure."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        symbols: Union[str, List[str]],
-        keyfigures: Union[
-            str,
-            CalculatedBondKeyFigureName,
-            List[str],
-            List[CalculatedBondKeyFigureName],
-            List[Union[str, CalculatedBondKeyFigureName]],
-        ],
-        calc_date: datetime,
-        curves: Optional[
-            Union[
-                str,
-                CurveName,
-                List[str],
-                List[CurveName],
-                List[Union[str, CurveName]],
-            ]
-        ] = None,
-        shift_tenors: Union[
-            float, List[float], int, List[int], List[Union[float, int]]
-        ] = None,
-        shift_values: Union[
-            float, List[float], int, List[int], List[Union[float, int]]
-        ] = None,
-        pp_speed: Optional[float] = None,
-        prices: Optional[Union[float, List[float]]] = None,
-        spread: Optional[float] = None,
-        spread_curve: Optional[Union[str, CurveName]] = None,
-        yield_input: Optional[float] = None,
-        asw_fix_frequency: Optional[str] = None,
-        ladder_definition: Optional[Union[float, List[float]]] = None,
-        cashflow_type: Optional[Union[str, CashflowType]] = None,
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            symbols: ISIN or name of bonds that should be valued.
-            keyfigures: Bond key figure that should be valued.
-            calc_date: date of calculation.
-            curves: discount curves for calculation.
-            shift_tenors: Tenors to shift curves expressed as float. For example [0.25, 0.5, 1, 3, 5].
-            shift_values: Shift values in basispoints. For example [100, 100, 75, 100, 100].
-            pp_speed: Prepayment speed. Default = 1.
-            prices: fixed price per bond.
-            spread: fixed spread for bond. Mandatory to give
-                spread_curve also as an input.
-            spread_curve: spread curve to calculate the
-                key figures when a fixed spread is given.
-            yield_input: fixed yield for bond.
-            asw_fix_frequency: Fixing frequency of swap in ASW calculation.
-                Mandatory input in all ASW calculations.
-            ladder_definition: Optional. Tenors should be included in
-                BPV ladder calculation. For example [0.25, 0.5, 1, 3, 5].
-            cashflow_type: Type of cashflow to calculate with.
-        """
-        super(BondKeyFigureCalculator, self).__init__(client)
-        self._client = client
-
-        self.key_figures_original: List = (
-            keyfigures if isinstance(keyfigures, list) else [keyfigures]
-        )
-        self.keyfigures = [
-            convert_to_variable_string(keyfigure, CalculatedBondKeyFigureName)
-            if isinstance(keyfigure, CalculatedBondKeyFigureName)
-            else keyfigure.lower()
-            for keyfigure in self.key_figures_original
-        ]
-
-        self.symbols = symbols if isinstance(symbols, list) else [symbols]
-        self.calc_date = calc_date
-        self.curves_original: Union[List, None] = (
-            curves
-            if isinstance(curves, list)
-            else [curves]
-            if isinstance(curves, str) or isinstance(curves, CurveName)
-            else None
-        )
-
-        _curves: Union[List[str], None]
-        if isinstance(curves, list):
-            _curves = [
-                convert_to_variable_string(curve, CurveName)
-                if isinstance(curve, CurveName)
-                else curve
-                for curve in curves
-            ]
-        elif curves is not None:
-            # mypy doesn't know that curves in this line is never a list
-            _curves = [convert_to_variable_string(curves, CurveName)]  # type: ignore
-        else:
-            _curves = None
-
-        self.curves = _curves
-        self.shift_tenors = shift_tenors
-        self.shift_values = shift_values
-        self.pp_speed = pp_speed
-
-        _prices: Union[List[float], None]
-        if isinstance(prices, list):
-            _prices = prices
-        elif prices is not None:
-            _prices = [prices]
-        else:
-            _prices = None
-
-        self.prices = _prices
-        self.spread = spread
-        _spread_curve = (
-            convert_to_variable_string(spread_curve, CurveName)
-            if spread_curve
-            else None
-        )
-        self.spread_curve = _spread_curve
-        self.yield_input = yield_input
-        self.asw_fix_frequency = asw_fix_frequency
-        self.ladder_definition = (
-            ladder_definition
-            if isinstance(ladder_definition, list)
-            else [ladder_definition]
-            if isinstance(ladder_definition, float)
-            or isinstance(ladder_definition, int)
-            else None
-        )
-        self.cashflow_type = (
-            convert_to_variable_string(cashflow_type, CashflowType)
-            if cashflow_type is not None
-            else None
-        )
-        if not isinstance(self, BondKeyFigureAdvancedCalculator):
-            self._data = self.calculate_bond_key_figure()
-
-    def calculate_bond_key_figure(self) -> Mapping:
-        """Retrieves response with calculated key figures."""
-        json_response = self.get_post_get_response()
-
-        return json_response
-
-    def get_post_get_response(self) -> Dict:
-        """Retrieves response after posting the request."""
-        json_response: Dict = {}
-        for request_dict in self.request:
-            try:
-                _json_response = self._client.get_response_asynchronous(
-                    request_dict, self.url_suffix
-                )
-                json_response[request_dict["symbol"]] = _json_response
-            except Exception as ex:
-                CustomWarningCheck.post_response_not_retrieved_warning(
-                    ex, request_dict["symbol"]
-                )
-
-        return json_response
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix for a given method."""
-        return config["url_suffix"]["calculate"]
-
-    @property
-    def request(self) -> List[Dict]:
-        """Post request dictionary calculate bond key figure."""
-        request_dict = []
-        keyfigures = copy.deepcopy(self.keyfigures)
-        keyfigures.remove("price") if "price" in self.keyfigures else keyfigures
-        if keyfigures == []:  # There has to be some key figure in request,
-            # but it will not be returned in final results
-            keyfigures = "yield"  # type:ignore
-        for x in range(len(self.symbols)):
-            initial_request = {
-                "symbol": self.symbols[x],
-                "date": self.calc_date.strftime("%Y-%m-%d"),
-                "keyfigures": keyfigures,
-                "curves": self.curves,
-                "shift_tenors": self.shift_tenors,
-                "shift_values": self.shift_values,
-                "pp_speed": self.pp_speed,
-                "price": self.prices[x]
-                if self.prices is not None and x < len(self.prices)
-                else None,
-                "spread": self.spread,
-                "spread_curve": self.spread_curve,
-                "yield": self.yield_input,
-                "asw_fix_frequency": self.asw_fix_frequency,
-                "ladder_definition": self.ladder_definition,
-                "cashflow_type": self.cashflow_type,
-            }
-            request = {
-                key: initial_request[key]
-                for key in initial_request.keys()
-                if initial_request[key] is not None
-            }
-            request_dict.append(request)
-
-        return request_dict
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        _dict: Dict[Any, Any] = {}
-        for symbol in self._data:
-            bond_data = self._data[symbol]
-            _dict_bond = self.to_dict_bond(bond_data)
-            _dict[symbol] = _dict_bond
-        return _dict
-
-    def to_dict_bond(self, bond_data: Dict) -> Dict:
-        """to_dict function too complicated."""
-        _dict_bond: Dict[Any, Any] = {}
-        for key_figure in bond_data:
-            if key_figure != "price" and key_figure in self.keyfigures:
-                for curve_data in bond_data[key_figure]["values"]:
-                    _data_dict: Dict[Any, Any] = {}
-                    if key_figure == "bpvladder":
-                        ladder_dict = {
-                            convert_to_float_if_float(
-                                ladder["key"]
-                            ): convert_to_float_if_float(ladder["value"])
-                            for ladder in curve_data["ladder"]
-                        }
-                        formatted_result = ladder_dict
-                    elif key_figure == "expectedcashflow":
-                        cashflow_dict = {
-                            datetime.strptime(
-                                cashflow["payment_date"], "%Y-%m-%d"
-                            ).date(): {
-                                "interest": cashflow["interest"],
-                                "principal": cashflow["principal"],
-                            }
-                            for cashflow in curve_data["cashflows"]
-                        }
-                        formatted_result = cashflow_dict  # type:ignore
-                    elif key_figure == "vegamatrix":
-                        vega_dict = {
-                            vega_list["key"]: vega_list["value"]
-                            for vega_list in curve_data["vega_points"]
-                        }
-                        formatted_result = vega_dict
-                    else:
-                        formatted_result = convert_to_float_if_float(
-                            curve_data["value"]
-                        )  # type:ignore
-
-                    _data_dict[
-                        convert_to_original_format(
-                            key_figure, self.key_figures_original
-                        )
-                    ] = formatted_result
-
-                    curve_key = (
-                        CurveName(curve_data["key"].upper())
-                        if self.curves_original is None
-                        else convert_to_original_format(
-                            curve_data["key"], self.curves_original  # type:ignore
-                        )
-                    )
-                    if curve_key in _dict_bond.keys():
-                        _dict_bond[curve_key].update(_data_dict)
-                    else:
-                        _dict_bond[curve_key] = _data_dict
-
-        # This would be the case if only Price would be selected as key figure
-        # If not, price has no curve to be inserted into
-        if _dict_bond == {}:
-            _dict_bond["No curve found"] = {}
-
-        if "price" in bond_data and "price" in self.keyfigures:
-            for curve in _dict_bond:
-                _dict_bond[curve][
-                    convert_to_original_format("price", self.key_figures_original)
-                ] = bond_data["price"]
-
-        return _dict_bond
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        _dict = self.to_dict()
-        df = pd.DataFrame()
-        for symbol in _dict:
-            _df = pd.DataFrame.from_dict(_dict[symbol]).transpose()
-            _df = _df.reset_index().rename(columns={"index": "Curve"})
-            _df.index = [symbol] * len(_df)
-            df = pd.concat([df, _df], axis=0)
-        return df
-
-
-class BondKeyFigureAdvancedCalculator(BondKeyFigureCalculator):
-    """Retrieves and reformat calculated bond key figure."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        symbols: Union[str, List[str]],
-        keyfigures: Union[
-            str,
-            CalculatedBondKeyFigureName,
-            List[str],
-            List[CalculatedBondKeyFigureName],
-            List[Union[str, CalculatedBondKeyFigureName]],
-        ],
-        calc_date: datetime,
-        curves: Optional[Union[List[str], str, CurveName, List[CurveName]]] = None,
-        shift_tenors: Optional[Union[List[float], float]] = None,
-        shift_values: Optional[Union[List[float], float]] = None,
-        pp_speed: Optional[float] = None,
-        prices: Optional[Union[float, List[float]]] = None,
-        spread: Optional[float] = None,
-        spread_curve: Optional[Union[str, CurveName]] = None,
-        yield_input: Optional[float] = None,
-        asw_fix_frequency: Optional[str] = None,
-        ladder_definition: Optional[Union[float, List[float]]] = None,
-        cashflow_type: Optional[Union[str, CashflowType]] = None,
-        fixed_principal_payment: Optional[Union[str, List[str]]] = None,
-        volatility_date: Optional[datetime] = None,
-        refinancing_curve_date: Optional[datetime] = None,
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            symbols: ISIN or name of bonds that should be valued.
-            keyfigures: Bond key figure that should be valued.
-            calc_date: Date of calculation.
-            curves: Discount curves for calculation.
-            shift_tenors: Tenors to shift curves expressed as float. For example [0.25, 0.5, 1, 3, 5].
-            shift_values: Shift values in basispoints. For example [100, 100, 75, 100, 100].
-            pp_speed: Prepayment speed. Default = 1.
-            prices: fixed price per bond.
-            spread: fixed spread for bond. Mandatory to give
-                spread_curve also as an input.
-            spread_curve: spread curve to calculate the
-                key figures when a fixed spread is given.
-            yield_input: fixed yield for bond.
-            asw_fix_frequency: Fixing frequency of swap in ASW calculation.
-                Mandatory input in all ASW calculations.
-            ladder_definition: Tenors should be included in
-                BPV ladder calculation. For example [0.25, 0.5, 1, 3, 5].
-            cashflow_type: Type of cashflow to calculate with.
-            fixed_principal_payment: Principal payment each cash flow date.
-            volatility_date: Date of volatility surface.
-            refinancing_curve_date: Date of refinancing curve.
-        """
-        super(BondKeyFigureAdvancedCalculator, self).__init__(
-            client,
-            symbols,
-            keyfigures,
-            calc_date,
-            curves,
-            shift_tenors,
-            shift_values,
-            pp_speed,
-            prices,
-            spread,
-            spread_curve,
-            yield_input,
-            asw_fix_frequency,
-            ladder_definition,
-            cashflow_type,
-        )
-
-        self.fixed_principal_payment = fixed_principal_payment
-        self.volatility_date = volatility_date
-        self.refinancing_curve_date = refinancing_curve_date
-
-        self._data = self.calculate_bond_key_figure_advanced()
-
-    def calculate_bond_key_figure_advanced(self) -> Mapping:
-        """Retrieves response with calculated key figures."""
-        json_response = self.get_post_get_response()
-
-        return json_response
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix for a given method."""
-        return config["url_suffix"]["calculate_advanced"]
-
-    @property
-    def request(self) -> List[Dict]:
-        """Post request dictionary calculate bond key figure."""
-        request_dict = []
-        keyfigures = copy.deepcopy(self.keyfigures)
-        keyfigures.remove("price") if "price" in self.keyfigures else keyfigures
-        if keyfigures == []:  # There has to be some key figure in request,
-            # but it will not be returned in final results
-            keyfigures = "bpv"  # type:ignore
-        for x in range(len(self.symbols)):
-            initial_request = {
-                "symbol": self.symbols[x],
-                "date": self.calc_date.strftime("%Y-%m-%d"),
-                "keyfigures": keyfigures,
-                "curves": self.curves,
-                "shift_tenors": self.shift_tenors,
-                "shift_values": self.shift_values,
-                "pp_speed": self.pp_speed,
-                "price": self.prices[x]
-                if self.prices is not None and x < len(self.prices)
-                else None,
-                "spread": self.spread,
-                "spread_curve": self.spread_curve,
-                "yield": self.yield_input,
-                "asw_fix_frequency": self.asw_fix_frequency,
-                "ladder_definition": self.ladder_definition,
-                "cashflow_type": self.cashflow_type,
-                "fixed_principal_payment": self.fixed_principal_payment,
-                "volatility_date": self.volatility_date.strftime("%Y-%m-%d")
-                if self.volatility_date is not None
-                else None,
-                "refinancing_curve_date": self.refinancing_curve_date.strftime(
-                    "%Y-%m-%d"
-                )
-                if self.refinancing_curve_date is not None
-                else None,
-            }
-            request = {
-                key: initial_request[key]
-                for key in initial_request.keys()
-                if initial_request[key] is not None
-            }
-            request_dict.append(request)
-
-        return request_dict
+import copy
+from datetime import datetime
+from typing import Any, Dict, List, Mapping, Optional, Union
+
+import pandas as pd
+
+from nordea_analytics.convention_variable_names import CashflowType
+from nordea_analytics.curve_variable_names import (
+    CurveName,
+)
+from nordea_analytics.key_figure_names import (
+    CalculatedBondKeyFigureName,
+)
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.exceptions import CustomWarningCheck
+from nordea_analytics.nalib.util import (
+    convert_to_float_if_float,
+    convert_to_original_format,
+    convert_to_variable_string,
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class BondKeyFigureCalculator(ValueRetriever):
+    """Retrieves and reformats calculated bond key figures.
+
+    Args:
+        client: The client used to retrieve data.
+        symbols: ISIN or name of bonds that should be valued.
+        keyfigures: Bond key figures that should be valued.
+        calc_date: date of calculation.
+        curves: discount curves for calculation.
+        shift_tenors: Tenors to shift curves expressed as float.
+                      For example [0.25, 0.5, 1, 3, 5].
+        shift_values: Shift values in basis points.
+                      For example [100, 100, 75, 100, 100].
+        pp_speed: Prepayment speed. Default = 1.
+        prices: fixed price per bond.
+        spread: fixed spread for bond. Mandatory to give spread_curve also as an input.
+        spread_curve: spread curve to calculate the key figures when a fixed spread is given.
+        yield_input: fixed yield for bond.
+        asw_fix_frequency: Fixing frequency of swap in ASW calculation.
+                            Mandatory input in all ASW calculations.
+        ladder_definition: Optional. Tenors should be included in BPV ladder calculation.
+                            For example [0.25, 0.5, 1, 3, 5].
+        cashflow_type: Type of cashflow to calculate with.
+    """
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        symbols: Union[str, List[str]],
+        keyfigures: Union[
+            str,
+            CalculatedBondKeyFigureName,
+            List[str],
+            List[CalculatedBondKeyFigureName],
+            List[Union[str, CalculatedBondKeyFigureName]],
+        ],
+        calc_date: datetime,
+        curves: Optional[
+            Union[
+                str,
+                CurveName,
+                List[str],
+                List[CurveName],
+                List[Union[str, CurveName]],
+            ]
+        ] = None,
+        shift_tenors: Union[
+            float, List[float], int, List[int], List[Union[float, int]]
+        ] = None,
+        shift_values: Union[
+            float, List[float], int, List[int], List[Union[float, int]]
+        ] = None,
+        pp_speed: Optional[float] = None,
+        prices: Optional[Union[float, List[float]]] = None,
+        spread: Optional[float] = None,
+        spread_curve: Optional[Union[str, CurveName]] = None,
+        yield_input: Optional[float] = None,
+        asw_fix_frequency: Optional[str] = None,
+        ladder_definition: Optional[Union[float, List[float]]] = None,
+        cashflow_type: Optional[Union[str, CashflowType]] = None,
+    ) -> None:
+        """Initialization of class.
+
+        Args:
+            client: The client used to retrieve data.
+            symbols: ISIN or name of bonds that should be valued.
+            keyfigures: Bond key figure that should be valued.
+            calc_date: date of calculation.
+            curves: discount curves for calculation.
+            shift_tenors: Tenors to shift curves expressed as float. For example [0.25, 0.5, 1, 3, 5].
+            shift_values: Shift values in basispoints. For example [100, 100, 75, 100, 100].
+            pp_speed: Prepayment speed. Default = 1.
+            prices: fixed price per bond.
+            spread: fixed spread for bond. Mandatory to give
+                spread_curve also as an input.
+            spread_curve: spread curve to calculate the
+                key figures when a fixed spread is given.
+            yield_input: fixed yield for bond.
+            asw_fix_frequency: Fixing frequency of swap in ASW calculation.
+                Mandatory input in all ASW calculations.
+            ladder_definition: Tenors should be included in
+                BPV ladder calculation. For example [0.25, 0.5, 1, 3, 5].
+            cashflow_type: Type of cashflow to calculate with.
+        """
+        super(BondKeyFigureCalculator, self).__init__(client)
+        self._client = client
+
+        self.key_figures_original: List = (
+            keyfigures if isinstance(keyfigures, list) else [keyfigures]
+        )
+        self.keyfigures = [
+            convert_to_variable_string(keyfigure, CalculatedBondKeyFigureName)
+            if isinstance(keyfigure, CalculatedBondKeyFigureName)
+            else keyfigure.lower()
+            for keyfigure in self.key_figures_original
+        ]
+
+        self.symbols = symbols if isinstance(symbols, list) else [symbols]
+        self.calc_date = calc_date
+        self.curves_original: Union[List, None] = (
+            curves
+            if isinstance(curves, list)
+            else [curves]
+            if isinstance(curves, str) or isinstance(curves, CurveName)
+            else None
+        )
+
+        _curves: Union[List[str], None]
+        if isinstance(curves, list):
+            _curves = [
+                convert_to_variable_string(curve, CurveName)
+                if isinstance(curve, CurveName)
+                else curve
+                for curve in curves
+            ]
+        elif curves is not None:
+            # mypy doesn't know that curves in this line is never a list
+            _curves = [convert_to_variable_string(curves, CurveName)]  # type: ignore
+        else:
+            _curves = None
+
+        self.curves = _curves
+        self.shift_tenors = shift_tenors
+        self.shift_values = shift_values
+        self.pp_speed = pp_speed
+
+        _prices: Union[List[float], None]
+        if isinstance(prices, list):
+            _prices = prices
+        elif prices is not None:
+            _prices = [prices]
+        else:
+            _prices = None
+
+        self.prices = _prices
+        self.spread = spread
+        _spread_curve = (
+            convert_to_variable_string(spread_curve, CurveName)
+            if spread_curve
+            else None
+        )
+        self.spread_curve = _spread_curve
+        self.yield_input = yield_input
+        self.asw_fix_frequency = asw_fix_frequency
+        self.ladder_definition = (
+            ladder_definition
+            if isinstance(ladder_definition, list)
+            else [ladder_definition]
+            if isinstance(ladder_definition, float)
+            or isinstance(ladder_definition, int)
+            else None
+        )
+        self.cashflow_type = (
+            convert_to_variable_string(cashflow_type, CashflowType)
+            if cashflow_type is not None
+            else None
+        )
+        if not isinstance(self, BondKeyFigureAdvancedCalculator):
+            self._data = self.calculate_bond_key_figure()
+
+    def calculate_bond_key_figure(self) -> Mapping:
+        """Retrieves response with calculated key figures.
+
+        Returns:
+            The calculated key figures as a dictionary with bond symbols as keys.
+        """
+        json_response = (
+            self.get_post_get_response()
+        )  # Call internal method to get response
+        return json_response
+
+    def get_post_get_response(self) -> Dict:
+        """Retrieves response after posting the request.
+
+        Returns:
+            The response received after posting the request as a dictionary.
+        """
+        json_response: Dict = {}
+        for request_dict in self.request:  # Iterate over request dictionary
+            try:
+                _json_response = self._client.get_response_asynchronous(
+                    request_dict, self.url_suffix
+                )
+                json_response[request_dict["symbol"]] = _json_response
+            except Exception as ex:
+                CustomWarningCheck.post_response_not_retrieved_warning(
+                    ex, request_dict["symbol"]
+                )
+        return json_response
+
+    @property
+    def url_suffix(self) -> str:
+        """Url suffix for a given method.
+
+        Returns:
+            The URL suffix for the bond calculator method.
+        """
+        return config["url_suffix"]["calculate"]
+
+    @property
+    def request(self) -> List[Dict]:
+        """Post request dictionary to calculate bond key figures.
+
+        Returns:
+            The list of request dictionaries to calculate bond key figures.
+        """
+        request_dict = []
+        keyfigures = copy.deepcopy(self.keyfigures)
+        keyfigures.remove("price") if "price" in self.keyfigures else keyfigures
+        if keyfigures == []:
+            keyfigures = ["yield"]
+        for x in range(len(self.symbols)):
+            initial_request = {
+                "symbol": self.symbols[x],
+                "date": self.calc_date.strftime("%Y-%m-%d"),
+                "keyfigures": keyfigures,
+                "curves": self.curves,
+                "shift_tenors": self.shift_tenors,
+                "shift_values": self.shift_values,
+                "pp_speed": self.pp_speed,
+                "price": self.prices[x]
+                if self.prices is not None and x < len(self.prices)
+                else None,
+                "spread": self.spread,
+                "spread_curve": self.spread_curve,
+                "yield": self.yield_input,
+                "asw_fix_frequency": self.asw_fix_frequency,
+                "ladder_definition": self.ladder_definition,
+                "cashflow_type": self.cashflow_type,
+            }
+            request = {
+                key: initial_request[key]
+                for key in initial_request.keys()
+                if initial_request[key] is not None
+            }
+            request_dict.append(request)
+        return request_dict
+
+    def to_dict(self) -> Dict:
+        """Reformat the JSON response to a dictionary.
+
+        Returns:
+            A dictionary containing the reformatted JSON data.
+        """
+        _dict: Dict[Any, Any] = {}
+        for symbol in self._data:
+            bond_data = self._data[symbol]
+            _dict_bond = self.to_dict_bond(bond_data)
+            _dict[symbol] = _dict_bond
+        return _dict
+
+    def to_dict_bond(self, bond_data: Dict) -> Dict:
+        """Reformat the JSON bond data to a dictionary.
+
+        Args:
+            bond_data: The JSON data of a bond.
+
+        Returns:
+            A dictionary containing the reformatted bond data.
+        """
+        _dict_bond: Dict[Any, Any] = {}
+        for key_figure in bond_data:
+            if key_figure != "price" and key_figure in self.keyfigures:
+                for curve_data in bond_data[key_figure]["values"]:
+                    _data_dict: Dict[Any, Any] = {}
+                    if key_figure == "bpvladder":
+                        # Convert ladder data to dictionary
+                        ladder_dict = {
+                            convert_to_float_if_float(
+                                ladder["key"]
+                            ): convert_to_float_if_float(ladder["value"])
+                            for ladder in curve_data["ladder"]
+                        }
+                        formatted_result = ladder_dict  # type:ignore
+                    elif key_figure == "expectedcashflow":
+                        # Convert cashflow data to dictionary with datetime object as key
+                        cashflow_dict = {
+                            datetime.strptime(
+                                cashflow["payment_date"], "%Y-%m-%d"
+                            ).date(): {
+                                "interest": cashflow["interest"],
+                                "principal": cashflow["principal"],
+                            }
+                            for cashflow in curve_data["cashflows"]
+                        }
+                        formatted_result = cashflow_dict  # type:ignore
+                    elif key_figure == "vegamatrix":
+                        # Convert vega points data to dictionary
+                        vega_dict = {
+                            vega_list["key"]: vega_list["value"]
+                            for vega_list in curve_data["vega_points"]
+                        }
+                        formatted_result = vega_dict  # type:ignore
+                    else:
+                        formatted_result = convert_to_float_if_float(
+                            curve_data["value"]
+                        )  # type:ignore
+
+                    _data_dict[
+                        convert_to_original_format(
+                            key_figure, self.key_figures_original
+                        )
+                    ] = formatted_result
+
+                    curve_key = (
+                        CurveName(curve_data["key"].upper()).name
+                        if self.curves_original is None
+                        else convert_to_original_format(
+                            curve_data["key"], self.curves_original
+                        )
+                    )
+                    if curve_key in _dict_bond.keys():
+                        _dict_bond[curve_key].update(_data_dict)
+                    else:
+                        _dict_bond[curve_key] = _data_dict
+
+        # This would be the case if only Price would be selected as key figure
+        # If not, price has no curve to be inserted into
+        if _dict_bond == {}:
+            _dict_bond["No curve found"] = {}
+
+        if "price" in bond_data and "price" in self.keyfigures:
+            for curve in _dict_bond:
+                _dict_bond[curve][
+                    convert_to_original_format("price", self.key_figures_original)
+                ] = bond_data["price"]
+
+        return _dict_bond
+
+    def to_df(self) -> pd.DataFrame:
+        """Reformat the JSON response of bond data to a pandas DataFrame.
+
+        Returns:
+            A pandas DataFrame containing the reformatted bond data.
+        """
+        bond_data_dict = self.to_dict()
+        df = pd.DataFrame()
+
+        for symbol in bond_data_dict:
+            # Convert the data for the symbol to a DataFrame and transpose it
+            symbol_df = pd.DataFrame.from_dict(bond_data_dict[symbol]).transpose()
+            # Reset the index and rename the columns to "Curve"
+            symbol_df = symbol_df.reset_index().rename(columns={"index": "Curve"})
+            symbol_df.index = [symbol] * len(symbol_df)
+
+            # Concatenate the symbol DataFrame to the main DataFrame along the rows
+            df = pd.concat([df, symbol_df], axis=0)
+
+        return df
+
+
+class BondKeyFigureAdvancedCalculator(BondKeyFigureCalculator):
+    """Retrieves and reformat calculated bond key figure."""
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        symbols: Union[str, List[str]],
+        keyfigures: Union[
+            str,
+            CalculatedBondKeyFigureName,
+            List[str],
+            List[CalculatedBondKeyFigureName],
+            List[Union[str, CalculatedBondKeyFigureName]],
+        ],
+        calc_date: datetime,
+        curves: Optional[Union[List[str], str, CurveName, List[CurveName]]] = None,
+        shift_tenors: Optional[Union[List[float], float]] = None,
+        shift_values: Optional[Union[List[float], float]] = None,
+        pp_speed: Optional[float] = None,
+        prices: Optional[Union[float, List[float]]] = None,
+        spread: Optional[float] = None,
+        spread_curve: Optional[Union[str, CurveName]] = None,
+        yield_input: Optional[float] = None,
+        asw_fix_frequency: Optional[str] = None,
+        ladder_definition: Optional[Union[float, List[float]]] = None,
+        cashflow_type: Optional[Union[str, CashflowType]] = None,
+        fixed_principal_payment: Optional[Union[str, List[str]]] = None,
+        volatility_date: Optional[datetime] = None,
+        refinancing_curve_date: Optional[datetime] = None,
+    ) -> None:
+        """Initialization of the class.
+
+        Args:
+            client: The client used to retrieve data.
+            symbols: ISIN or name of bonds that should be valued.
+            keyfigures: Bond key figure that should be valued.
+            calc_date: Date of calculation.
+            curves: Discount curves for calculation.
+            shift_tenors: Tenors to shift curves expressed as float. For example [0.25, 0.5, 1, 3, 5].
+            shift_values: Shift values in basis points. For example [100, 100, 75, 100, 100].
+            pp_speed: Prepayment speed. Default = 1.
+            prices: Fixed price per bond.
+            spread: Fixed spread for bond. Mandatory to give spread_curve also as an input.
+            spread_curve: Spread curve to calculate the key figures when a fixed spread is given.
+            yield_input: Fixed yield for bond.
+            asw_fix_frequency: Fixing frequency of swap in ASW calculation.
+                Mandatory input in all ASW calculations.
+            ladder_definition: Tenors should be included in BPV ladder calculation. For example [0.25, 0.5, 1, 3, 5].
+            cashflow_type: Type of cashflow to calculate with.
+            fixed_principal_payment: Principal payment each cash flow date.
+            volatility_date: Date of the volatility surface.
+            refinancing_curve_date: Date of the refinancing curve.
+        """
+        super(BondKeyFigureAdvancedCalculator, self).__init__(
+            client,
+            symbols,
+            keyfigures,
+            calc_date,
+            curves,
+            shift_tenors,
+            shift_values,
+            pp_speed,
+            prices,
+            spread,
+            spread_curve,
+            yield_input,
+            asw_fix_frequency,
+            ladder_definition,
+            cashflow_type,
+        )
+
+        self.fixed_principal_payment = fixed_principal_payment
+        self.volatility_date = volatility_date
+        self.refinancing_curve_date = refinancing_curve_date
+
+        self._data = self.calculate_bond_key_figure_advanced()
+
+    def calculate_bond_key_figure_advanced(self) -> Mapping:
+        """Retrieves response with calculated key figures.
+
+        Returns:
+            The JSON response with calculated key figures.
+        """
+        json_response = self.get_post_get_response()
+
+        return json_response
+
+    @property
+    def url_suffix(self) -> str:
+        """Get the URL suffix for the given method.
+
+        Returns:
+            The URL suffix.
+        """
+        return config["url_suffix"]["calculate_advanced"]
+
+    @property
+    def request(self) -> List[Dict]:
+        """Get the post request dictionary for calculating bond key figure.
+
+        Returns:
+            The list of dictionaries representing the post request data.
+        """
+        request_dict = []
+        keyfigures = copy.deepcopy(self.keyfigures)
+        keyfigures.remove("price") if "price" in self.keyfigures else keyfigures
+        if keyfigures == []:  # There has to be some key figure in request,
+            # but it will not be returned in final results
+            keyfigures = "bpv"  # type:ignore
+        for x in range(len(self.symbols)):
+            initial_request = {
+                "symbol": self.symbols[x],
+                "date": self.calc_date.strftime("%Y-%m-%d"),
+                "keyfigures": keyfigures,
+                "curves": self.curves,
+                "shift_tenors": self.shift_tenors,
+                "shift_values": self.shift_values,
+                "pp_speed": self.pp_speed,
+                "price": self.prices[x]
+                if self.prices is not None and x < len(self.prices)
+                else None,
+                "spread": self.spread,
+                "spread_curve": self.spread_curve,
+                "yield": self.yield_input,
+                "asw_fix_frequency": self.asw_fix_frequency,
+                "ladder_definition": self.ladder_definition,
+                "cashflow_type": self.cashflow_type,
+                "fixed_principal_payment": self.fixed_principal_payment,
+                "volatility_date": self.volatility_date.strftime("%Y-%m-%d")
+                if self.volatility_date is not None
+                else None,
+                "refinancing_curve_date": self.refinancing_curve_date.strftime(
+                    "%Y-%m-%d"
+                )
+                if self.refinancing_curve_date is not None
+                else None,
+            }
+            request = {
+                key: initial_request[key]
+                for key in initial_request.keys()
+                if initial_request[key] is not None
+            }
+            request_dict.append(request)
+
+        return request_dict
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigures.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/BondKeyFigures.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,158 @@
-from datetime import datetime
-import math
-from typing import Any, Dict, List, Union
-
-import numpy as np
-import pandas as pd
-
-from nordea_analytics.key_figure_names import (
-    BondKeyFigureName,
-)
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.util import (
-    convert_to_float_if_float,
-    convert_to_original_format,
-    convert_to_variable_string,
-    get_config,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class BondKeyFigures(ValueRetriever):
-    """Retrieves and reformat given bond key figures for given bonds and calc date."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        symbols: Union[List[str], str],
-        keyfigures: Union[
-            str,
-            BondKeyFigureName,
-            List[str],
-            List[BondKeyFigureName],
-            List[Union[str, BondKeyFigureName]],
-        ],
-        calc_date: datetime,
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client:  DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing
-            symbols: ISIN or name of bonds for requests.
-            keyfigures: Bond key figure names for request.
-            calc_date: calculation date for request.
-        """
-        super(BondKeyFigures, self).__init__(client)
-
-        self.symbols: List = [symbols] if type(symbols) != list else symbols
-        self.keyfigures_original: List = (
-            keyfigures if type(keyfigures) == list else [keyfigures]
-        )
-        self.keyfigures = [
-            convert_to_variable_string(keyfigure, BondKeyFigureName)
-            if type(keyfigure) == BondKeyFigureName
-            else keyfigure
-            for keyfigure in self.keyfigures_original
-        ]
-        self.calc_date = calc_date
-        self._data = self.get_bond_key_figures()
-
-    def get_bond_key_figures(self) -> List:
-        """Calls the client and retrieves response with key figures from the service."""
-        json_response: List[Any] = []
-        for request_dict in self.request:
-            _json_response = self.get_response(request_dict)
-            json_map = _json_response[config["results"]["bond_key_figures"]]
-            json_response = list(json_map) + json_response
-
-        return json_response
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix for a given method."""
-        return config["url_suffix"]["bond_key_figures"]
-
-    @property
-    def request(self) -> List[Dict]:
-        """Request list of dictionaries for a given set of symbols, key figures and calc date."""
-        if len(self.symbols) > config["max_bonds"]:
-            split_symbols = np.array_split(
-                self.symbols, math.ceil(len(self.symbols) / config["max_bonds"])
-            )
-            request_dict = [
-                {
-                    "symbols": list(symbols),
-                    "keyfigures": self.keyfigures,
-                    "date": self.calc_date.strftime("%Y-%m-%d"),
-                }
-                for symbols in split_symbols
-            ]
-        else:
-            request_dict = [
-                {
-                    "symbols": self.symbols,
-                    "keyFigures": self.keyfigures,
-                    "date": self.calc_date.strftime("%Y-%m-%d"),
-                }
-            ]
-
-        return request_dict
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        _dict = {}
-        for bond_data in self._data:
-            _bond_dict = {}
-            for key_figure_data in bond_data["values"]:
-                key_figure_name = convert_to_original_format(
-                    key_figure_data["keyfigure"], self.keyfigures_original
-                )
-                _bond_dict[key_figure_name] = convert_to_float_if_float(
-                    key_figure_data["value"]
-                )
-
-            _dict[bond_data["symbol"]] = _bond_dict
-
-        return _dict
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        return pd.DataFrame.from_dict(self.to_dict(), orient="index")
+from datetime import datetime
+import math
+from typing import Any, Dict, List, Union
+
+import numpy as np
+import pandas as pd
+
+from nordea_analytics.key_figure_names import (
+    BondKeyFigureName,
+)
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.util import (
+    convert_to_float_if_float,
+    convert_to_original_format,
+    convert_to_variable_string,
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class BondKeyFigures(ValueRetriever):
+    """Retrieves and reformats given bond key figures for given bonds and calculation date.
+
+    Inherits from ValueRetriever class.
+    """
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        symbols: Union[List[str], str],
+        keyfigures: Union[
+            str,
+            BondKeyFigureName,
+            List[str],
+            List[BondKeyFigureName],
+            List[Union[str, BondKeyFigureName]],
+        ],
+        calc_date: datetime,
+    ) -> None:
+        """Initialize the BondKeyFigures class.
+
+        Args:
+            client: The client used to retrieve data.
+            symbols: ISIN or name of bonds for requests.
+                List of bond symbols or a single bond symbol.
+            keyfigures: Bond key figure names for request.
+                Can be a single key figure name or a list of key figure names.
+                Alternatively, can be a single BondKeyFigureName or a list of BondKeyFigureName enums,
+                or a list of strings or BondKeyFigureName enums.
+            calc_date: Calculation date for request.
+        """
+        super(BondKeyFigures, self).__init__(client)
+
+        # Convert symbols to a list if it's not already a list
+        self.symbols: List = [symbols] if not isinstance(symbols, list) else symbols
+
+        # Convert keyfigures to a list of strings
+        self.keyfigures_original: List = (
+            keyfigures if isinstance(keyfigures, list) else [keyfigures]
+        )
+
+        # Convert keyfigures to variable string format if it's a BondKeyFigureName enum
+        self.keyfigures = [
+            convert_to_variable_string(keyfigure, BondKeyFigureName)
+            if isinstance(keyfigure, BondKeyFigureName)
+            else keyfigure
+            for keyfigure in self.keyfigures_original
+        ]
+
+        self.calc_date = calc_date
+        self._data = self.get_bond_key_figures()
+
+    def get_bond_key_figures(self) -> List:
+        """Calls the client and retrieves response with key figures from the service.
+
+        Returns:
+            A list of key figures retrieved from the service.
+        """
+        json_response: List[Any] = []
+        for request_dict in self.request:
+            _json_response = self.get_response(request_dict)
+            json_map = _json_response[config["results"]["bond_key_figures"]]
+            json_response = list(json_map) + json_response
+
+        return json_response
+
+    @property
+    def url_suffix(self) -> str:
+        """Url suffix for a given method.
+
+        Returns:
+            The URL suffix for the method.
+        """
+        return config["url_suffix"]["bond_key_figures"]
+
+    @property
+    def request(self) -> List[Dict]:
+        """Request list of dictionaries for a given set of symbols, key figures and calc date.
+
+        Returns:
+            A list of dictionaries containing request parameters for each batch of symbols.
+        """
+        if len(self.symbols) > config["max_bonds"]:
+            # Split symbols into smaller lists if it exceeds the maximum number of bonds
+            split_symbols = np.array_split(
+                self.symbols, math.ceil(len(self.symbols) / config["max_bonds"])
+            )
+            request_dict = [
+                {
+                    "symbols": list(symbols),
+                    "keyfigures": self.keyfigures,
+                    "date": self.calc_date.strftime("%Y-%m-%d"),
+                }
+                for symbols in split_symbols
+            ]
+        else:
+            request_dict = [
+                {
+                    "symbols": self.symbols,
+                    "keyFigures": self.keyfigures,
+                    "date": self.calc_date.strftime("%Y-%m-%d"),
+                }
+            ]
+
+        return request_dict
+
+    def to_dict(self) -> Dict:
+        """Reformat the json response to a dictionary.
+
+        Returns:
+            A dictionary containing bond symbols as keys and their respective key figures as values.
+        """
+        _dict = {}
+        for bond_data in self._data:
+            _bond_dict = {}
+            for key_figure_data in bond_data["values"]:
+                key_figure_name = convert_to_original_format(
+                    key_figure_data["keyfigure"], self.keyfigures_original
+                )
+                _bond_dict[key_figure_name] = convert_to_float_if_float(
+                    key_figure_data["value"]
+                )
+
+            _dict[bond_data["symbol"]] = _bond_dict
+
+        return _dict
+
+    def to_df(self) -> pd.DataFrame:
+        """Reformat the json response to a pandas DataFrame.
+
+        Returns:
+            A pandas DataFrame containing bond symbols, key figures, and their values.
+        """
+        return pd.DataFrame.from_dict(self.to_dict(), orient="index")
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/BondStaticData.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/FXQuotes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,115 @@
-from datetime import datetime
-import math
-from typing import Any, Dict, List, Union
-
-import numpy as np
-import pandas as pd
-
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.util import (
-    get_config,
-    pascal_case,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class BondStaticData(ValueRetriever):
-    """Retrieves and reformat latest static data for given bonds."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        symbols: Union[List[str], str],
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client:  DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing
-            symbols: ISIN or name of bonds for requests.
-        """
-        super(BondStaticData, self).__init__(client)
-
-        self.symbols: List = [symbols] if type(symbols) != list else symbols
-        self._data = self.get_bond_static_data()
-
-    def get_bond_static_data(self) -> List:
-        """Calls the client and retrieves response with static data from the service."""
-        json_response: List[Any] = []
-        for request_dict in self.request:
-            _json_response = self.get_response(request_dict)
-            json_map = _json_response[config["results"]["bond_static_data"]]
-            json_response = list(json_map) + json_response
-
-        return json_response
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix suffix for a given method."""
-        return config["url_suffix"]["bond_static_data"]
-
-    @property
-    def request(self) -> List[Dict]:
-        """Request dictionary for a given set of symbols."""
-        if len(self.symbols) > config["max_bonds"]:
-            split_symbols = np.array_split(
-                self.symbols, math.ceil(len(self.symbols) / config["max_bonds"])
-            )
-            request_dict = [
-                {
-                    "symbols": list(symbols),
-                }
-                for symbols in split_symbols
-            ]
-        else:
-            request_dict = [
-                {
-                    "symbols": self.symbols,
-                }
-            ]
-
-        return request_dict
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        _dict = {}
-        for bond_data in self._data:
-            _symbol_dict = {}
-            _symbol_dict["Name"] = bond_data["name"]
-
-            for static_data_key in bond_data["static_data"]:
-                key_value_pair = bond_data["static_data"][static_data_key]
-
-                if (
-                    key_value_pair["key"] == "closing_date"
-                    or key_value_pair["key"] == "issue_date"
-                    or key_value_pair["key"] == "maturity"
-                    or key_value_pair["key"] == "retrieval_date"
-                ):
-                    _symbol_dict[
-                        pascal_case(key_value_pair["key"])
-                    ] = datetime.strptime(
-                        key_value_pair["value"], "%Y-%m-%dT%H:%M:%S.0000000"
-                    )
-                else:
-                    _symbol_dict[pascal_case(key_value_pair["key"])] = key_value_pair[
-                        "value"
-                    ]
-
-            _dict[bond_data["symbol"]] = _symbol_dict
-
-        return _dict
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        return pd.DataFrame.from_dict(self.to_dict(), orient="index")
+from datetime import datetime
+from typing import Any, Dict, List, Union
+
+import pandas as pd
+
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.exceptions import CustomWarningCheck
+from nordea_analytics.nalib.util import (
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class FXQuotes(ValueRetriever):
+    """Retrieves FX quotes."""
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        symbols: Union[List[str], str],
+        calc_date: datetime,
+    ) -> None:
+        """Initialize the FXQuotes class.
+
+        Args:
+            client: The client used to retrieve data.
+            symbols: Name of FX instruments for request.
+            calc_date: Calculation date for request.
+        """
+        super(FXQuotes, self).__init__(client)
+
+        self.symbols: List = [symbols] if type(symbols) != list else symbols
+        self.calc_date = calc_date
+        self._data = self.get_fx_quotes()
+
+    def get_fx_quotes(self) -> List:
+        """Call the client and retrieve response with FX quotes from the service.
+
+        Returns:
+            List of FX quotes retrieved from the service.
+        """
+        _json_response = self.get_post_get_response()
+        json_response: List[Any] = _json_response[config["results"]["fx_quotes"]]
+
+        return json_response
+
+    def get_post_get_response(self) -> Dict:
+        """Retrieve response after posting the request.
+
+        Returns:
+            JSON response retrieved from the service.
+        """
+        json_response: Dict = {}
+        try:
+            json_response = self._client.get_post_get_response(
+                self.request, self.url_suffix
+            )
+        except Exception as ex:
+            CustomWarningCheck.post_response_not_retrieved_warning(
+                ex, "One or more symbols "
+            )
+
+        return json_response
+
+    @property
+    def url_suffix(self) -> str:
+        """URL suffix for the FX quotes API.
+
+        Returns:
+            URL suffix for the FX quotes API.
+        """
+        return config["url_suffix"]["fx_quotes"]
+
+    @property
+    def request(self) -> Dict:
+        """Request dictionary for a given set of symbols and calculation date.
+
+        Returns:
+            Request dictionary with symbols and calculation date.
+        """
+        request_dict = {
+            "symbols": self.symbols,
+            "date": self.calc_date.strftime("%Y-%m-%d"),
+        }
+
+        return request_dict
+
+    def to_dict(self) -> Dict:
+        """Reformat the JSON response to a dictionary.
+
+        Returns:
+            Reformatted dictionary with FX quotes.
+        """
+        _dict = {}
+        for bond_data in self._data:
+            _bond_dict = {
+                "Bid": bond_data["price"]["bid"],
+                "Ask": bond_data["price"]["ask"],
+            }
+
+            _dict[bond_data["symbol"]] = _bond_dict
+
+        return _dict
+
+    def to_df(self) -> pd.DataFrame:
+        """Reformat the JSON response to a pandas DataFrame.
+
+        Returns:
+            Reformatted pandas DataFrame with FX quotes.
+        """
+        return pd.DataFrame.from_dict(self.to_dict(), orient="index")
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/CurveDefinition.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/CurveDefinition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,182 @@
-from datetime import datetime
-from typing import Any, Dict, List, Mapping, Union
-
-import numpy as np
-import pandas as pd
-
-from nordea_analytics.curve_variable_names import (
-    CurveDefinitionName,
-    CurveName,
-)
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.exceptions import AnalyticsWarning, CustomWarning
-from nordea_analytics.nalib.util import (
-    convert_to_float_if_float,
-    convert_to_variable_string,
-    get_config,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class CurveDefinition(ValueRetriever):
-    """Retrieves and reformat curve definition."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        curve: Union[str, CurveDefinitionName, CurveName],
-        calc_date: datetime,
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            curve: Name of curve that should be retrieved.
-            calc_date: calculation date for request.
-        """
-        super(CurveDefinition, self).__init__(client)
-        self._client = client
-        self.curve: str = (
-            convert_to_variable_string(curve, CurveName)
-            if type(curve) == CurveName
-            else convert_to_variable_string(curve, CurveDefinitionName)
-            if type(curve) == CurveDefinitionName
-            else str(curve)
-        )
-        self.curve_original = curve
-        self.calc_date = calc_date
-        self._data = self.get_curve_definition()
-
-    def get_curve_definition(self) -> Mapping:
-        """Retrieves response with curve definition."""
-        json_response = self.get_response(self.request)
-        json_response = json_response[config["results"]["curve_definition"]]
-
-        return json_response
-
-    def format_curve_names(
-        self,
-        data: List,
-        curve_name: Union[str, CurveName],
-    ) -> List:
-        """Formats curve names to be identical to curves input."""
-        curve_dict = {}
-        curve_name_string: Union[str, ValueError]
-        if type(curve_name) == CurveName:
-            curve_name_string = convert_to_variable_string(curve_name, CurveName)
-            if curve_name_string != ValueError:
-                curve_name_string = curve_name_string.upper()
-            else:
-                CustomWarning(
-                    "Conversion of {0} failed.".format(curve_name), AnalyticsWarning
-                )
-        elif type(curve_name) == str:
-            curve_name_string = curve_name.upper()
-        curve_dict[curve_name_string] = (
-            curve_name.name if type(curve_name) == CurveName else curve_name
-        )
-
-        for curve_result in data:
-            curve_result["curve"]["curve_specification"]["name"] = curve_dict[
-                curve_result["curve"]["curve_specification"]["name"].upper()
-            ]
-
-        return data
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix suffix for a given method."""
-        return config["url_suffix"]["curve_definition"]
-
-    @property
-    def request(self) -> Dict:
-        """Request dictionary curve time definition."""
-        request = {"date": self.calc_date.strftime("%Y-%m-%d"), "curve": self.curve}
-
-        return request
-
-    def get_curve_key(self, curve_name: str) -> str:
-        """Get curve key for dict."""
-        if curve_name == self.curve_original:  # True when curve is input as string
-            curve_key = curve_name
-        else:
-            try:
-                curve_key = CurveName(curve_name).name
-            except Exception:
-                curve_key = curve_name
-
-        return curve_key
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        _dict = {}
-        _curve_def_dict: Dict[Any, Any] = {}
-        for curve_def in self._data["values"]:
-            _curve_def_dict = {}
-            if "quote" in curve_def["asset"]:
-                _curve_def_dict["Quote"] = convert_to_float_if_float(
-                    curve_def["asset"]["quote"]
-                )
-            if "weight" in curve_def["asset"]:
-                _curve_def_dict["Weight"] = curve_def["asset"]["weight"]
-            if "maturity" in curve_def["asset"]:
-                _curve_def_dict["Maturity"] = datetime.strptime(
-                    curve_def["asset"]["maturity"], "%Y-%m-%dT%H:%M:%S.0000000"
-                )
-            curve_key = self.get_curve_key(self.curve)
-            _dict[curve_def["name"]] = _curve_def_dict
-        return {curve_key: _dict}
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        _dict = self.to_dict()
-
-        curve_key = (
-            self.curve_original.name
-            if type(self.curve_original) == CurveName
-            or type(self.curve_original) == CurveDefinitionName
-            else self.curve_original
-        )
-
-        df = pd.DataFrame.from_dict(_dict[curve_key]).transpose()
-        df = df.astype(object).mask(df.isna(), np.nan)
-        df = df.reset_index().rename(columns={"index": "Name"})
-        df.index = [curve_key] * len(df)
-        return df
+from datetime import datetime
+from typing import Any, Dict, List, Mapping, Union
+
+import numpy as np
+import pandas as pd
+
+from nordea_analytics.curve_variable_names import (
+    CurveDefinitionName,
+    CurveName,
+)
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.exceptions import AnalyticsWarning, CustomWarning
+from nordea_analytics.nalib.util import (
+    convert_to_float_if_float,
+    convert_to_variable_string,
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class CurveDefinition(ValueRetriever):
+    """Retrieves and reformats curve definition.
+
+    Inherits from ValueRetriever class.
+    """
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        curve: Union[str, CurveDefinitionName, CurveName],
+        calc_date: datetime,
+    ) -> None:
+        """Initialize the CurveDefinition class.
+
+        Args:
+            client: The client used to retrieve data.
+            curve: Name of curve that should be retrieved.
+                Can be a string, CurveDefinitionName enum, or CurveName enum.
+            calc_date: Calculation date for request.
+        """
+        super(CurveDefinition, self).__init__(client)
+
+        # Convert curve to variable string format based on its type
+
+        _curve: str
+        if isinstance(curve, CurveName):
+            _curve = convert_to_variable_string(curve, CurveName)
+        elif isinstance(curve, CurveDefinitionName):
+            _curve = convert_to_variable_string(curve, CurveDefinitionName)
+        else:
+            _curve = str(curve)
+        self.curve = _curve
+
+        self.curve_original = curve
+        self.calc_date = calc_date
+        self._data = self.get_curve_definition()
+
+    def get_curve_definition(self) -> Mapping:
+        """Retrieve response with curve definition.
+
+        Returns:
+            The curve definition data as a dictionary.
+        """
+        json_response = self.get_response(self.request)
+        json_response = json_response[config["results"]["curve_definition"]]
+        return json_response
+
+    def format_curve_names(
+        self,
+        data: List,
+        curve_name: Union[str, CurveName],
+    ) -> List:
+        """Format curve names to be identical to the curves input.
+
+        Args:
+            data: List of curve data.
+            curve_name: Name of the curve to be formatted.
+
+        Returns:
+            List of curve data with formatted curve names.
+        """
+        curve_dict = {}
+        curve_name_string: Union[str, ValueError]
+
+        if isinstance(curve_name, CurveName):
+            curve_name_string = convert_to_variable_string(curve_name, CurveName)
+            if curve_name_string != ValueError:
+                curve_name_string = curve_name_string.upper()
+            else:
+                CustomWarning(
+                    "Conversion of {0} failed.".format(curve_name), AnalyticsWarning
+                )
+        elif isinstance(curve_name, str):
+            curve_name_string = curve_name.upper()
+
+        curve_dict[curve_name_string] = (
+            curve_name.name if isinstance(curve_name, CurveName) else curve_name
+        )
+
+        for curve_result in data:
+            curve_result["curve"]["curve_specification"]["name"] = curve_dict[
+                curve_result["curve"]["curve_specification"]["name"].upper()
+            ]
+
+        return data
+
+    @property
+    def url_suffix(self) -> str:
+        """Get the URL suffix for a given method.
+
+        Returns:
+            The URL suffix for the curve definition method.
+        """
+        return config["url_suffix"]["curve_definition"]
+
+    @property
+    def request(self) -> Dict:
+        """Request dictionary curve time definition."""
+        request = {"date": self.calc_date.strftime("%Y-%m-%d"), "curve": self.curve}
+
+        return request
+
+    def get_curve_key(self, curve_name: str) -> str:
+        """Get curve key for dict."""
+        if curve_name == self.curve_original:  # True when curve is input as string
+            curve_key = curve_name
+        else:
+            try:
+                curve_key = CurveName(curve_name).name
+            except Exception:
+                curve_key = curve_name
+
+        return curve_key
+
+    def to_dict(self) -> Dict:
+        """Converts the JSON response to a dictionary.
+
+        Returns:
+            A dictionary representing the reformatted JSON response.
+        """
+        _dict = {}
+        _curve_def_dict: Dict[Any, Any] = {}
+        for curve_def in self._data["values"]:
+            _curve_def_dict = {}
+            if "quote" in curve_def["asset"]:
+                _curve_def_dict["Quote"] = convert_to_float_if_float(
+                    curve_def["asset"]["quote"]
+                )
+            if "weight" in curve_def["asset"]:
+                _curve_def_dict["Weight"] = curve_def["asset"]["weight"]
+            if "maturity" in curve_def["asset"]:
+                _curve_def_dict["Maturity"] = datetime.strptime(
+                    curve_def["asset"]["maturity"], "%Y-%m-%dT%H:%M:%S.0000000"
+                )
+            curve_key = self.get_curve_key(self.curve)
+            _dict[curve_def["name"]] = _curve_def_dict
+        return {curve_key: _dict}
+
+    def to_df(self) -> pd.DataFrame:
+        """Converts the JSON response to a pandas DataFrame.
+
+        Returns:
+            A pandas DataFrame representing the reformatted JSON response.
+        """
+        _dict = self.to_dict()
+
+        curve_key = (
+            self.curve_original.name
+            if type(self.curve_original) == CurveName
+            or type(self.curve_original) == CurveDefinitionName
+            else self.curve_original
+        )
+
+        df = pd.DataFrame.from_dict(_dict[curve_key]).transpose()
+        df = df.astype(object).mask(df.isna(), np.nan)
+        df = df.reset_index().rename(columns={"index": "Name"})
+        df.index = [curve_key] * len(df)
+        return df
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/FXForecast.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/FXForecast.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,120 @@
-from datetime import datetime
-from typing import Any, Dict, Mapping
-
-import pandas as pd
-
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.util import (
-    get_config,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class FXForecast(ValueRetriever):
-    """Retrieves and reformat FX forecast."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        currency_pair: str,
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            currency_pair: Currency cross for which to retrieve forecasts.
-        """
-        super(FXForecast, self).__init__(client)
-        self._client = client
-        self.currency_pair = currency_pair
-        self._data = self.get_fx_forecast()
-
-    def get_fx_forecast(self) -> Mapping:
-        """Retrieves response with FX forecast."""
-        json_response = self.get_response(self.request)
-        json_response = json_response[config["results"]["fx_forecast"]]
-
-        return json_response
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix for a given method."""
-        return config["url_suffix"]["fx_forecast"]
-
-    @property
-    def request(self) -> Dict:
-        """Request dictionary FX forecast."""
-        currency_pair = self.currency_pair
-
-        request_dict = {
-            "currency-pair": currency_pair,
-        }
-
-        return request_dict
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        _dict: Dict[Any, Any] = {}
-
-        forecast_data = {}
-
-        for fx_type_data in self._data["forecasts"]:
-            fx_type_forecast_data = {}
-            type = fx_type_data["type"]
-
-            for data in fx_type_data["forecast"]:
-                values = {}
-
-                values["Updated_at"] = datetime.strptime(
-                    fx_type_data["updated_at"].split("T")[0], "%Y-%m-%d"
-                )
-
-                values["Value"] = data["value"]
-                fx_type_forecast_data[data["horizon"]] = values
-
-            forecast_data[type] = fx_type_forecast_data
-
-        _dict[self._data["symbol"]] = forecast_data
-
-        return _dict
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        _dict = self.to_dict()
-
-        df = pd.DataFrame.from_dict(
-            {
-                (i, j, k): _dict[i][j][k]
-                for i in _dict.keys()
-                for j in _dict[i].keys()
-                for k in _dict[i][j].keys()
-            },
-            orient="index",
-        )
-        df = df.reset_index().rename(
-            columns={"level_0": "Symbol", "level_1": "FX_type", "level_2": "Horizon"}
-        )
-
-        return df
+from datetime import datetime
+from typing import Any, Dict, Mapping
+
+import pandas as pd
+
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.util import (
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class FXForecast(ValueRetriever):
+    """A class for retrieving and reformatting FX forecasts."""
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        currency_pair: str,
+    ) -> None:
+        """Initialize the FXForecast object.
+
+        Args:
+            client: The client used to retrieve data.
+            currency_pair: The currency cross for which to retrieve forecasts.
+        """
+        super(FXForecast, self).__init__(client)
+        self._client = client
+        self._currency_pair = currency_pair
+        self._data = self.get_fx_forecast()
+
+    def get_fx_forecast(self) -> Mapping:
+        """Retrieve response with FX forecast.
+
+        Returns:
+            A dictionary containing the FX forecast data.
+        """
+        json_response = self.get_response(self.request)
+        json_response = json_response[config["results"]["fx_forecast"]]
+        return json_response
+
+    @property
+    def url_suffix(self) -> str:
+        """Get URL suffix for the given method.
+
+        Returns:
+            The URL suffix for the FX forecast method.
+        """
+        return config["url_suffix"]["fx_forecast"]
+
+    @property
+    def request(self) -> Dict:
+        """Get request dictionary for FX forecast.
+
+        Returns:
+            The request dictionary for the FX forecast.
+        """
+        currency_pair = self._currency_pair
+
+        request_dict = {
+            "currency-pair": currency_pair,
+        }
+
+        return request_dict
+
+    def to_dict(self) -> Dict:
+        """Reformat the JSON response to a dictionary.
+
+        Returns:
+            The reformatted dictionary from the JSON response.
+        """
+        forecast_dict: Dict[Any, Any] = {}
+        forecast_data = {}
+
+        for fx_type_data in self._data["forecasts"]:
+            fx_type_forecast_data = {}
+            fx_type = fx_type_data["type"]
+
+            for data in fx_type_data["forecast"]:
+                values = {}
+
+                values["Updated_at"] = datetime.strptime(
+                    fx_type_data["updated_at"].split("T")[0], "%Y-%m-%d"
+                )
+
+                values["Value"] = data["value"]
+                fx_type_forecast_data[data["horizon"]] = values
+
+            forecast_data[fx_type] = fx_type_forecast_data
+
+        forecast_dict[self._data["symbol"]] = forecast_data
+
+        return forecast_dict
+
+    def to_df(self) -> pd.DataFrame:
+        """Reformat the JSON response to a pandas DataFrame.
+
+        Returns:
+            The reformatted DataFrame from the JSON response.
+        """
+        forecast_dict = self.to_dict()
+
+        df = pd.DataFrame.from_dict(
+            {
+                (i, j, k): forecast_dict[i][j][k]
+                for i in forecast_dict.keys()
+                for j in forecast_dict[i].keys()
+                for k in forecast_dict[i][j].keys()
+            },
+            orient="index",
+        )
+        df = df.reset_index().rename(
+            columns={"level_0": "Symbol", "level_1": "FX_type", "level_2": "Horizon"}
+        )
+
+        return df
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/IndexComposition.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/IndexComposition.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,101 @@
 from datetime import datetime
 from typing import Dict, List, Mapping, Union
 
 import pandas as pd
 
+from nordea_analytics.instrument_variable_names import BondIndexName
 from nordea_analytics.nalib.data_retrieval_client import (
     DataRetrievalServiceClient,
 )
 from nordea_analytics.nalib.util import (
     convert_to_float_if_float,
+    convert_to_original_format,
+    convert_to_variable_string,
     get_config,
 )
 from nordea_analytics.nalib.value_retriever import ValueRetriever
 
 config = get_config()
 
 
 class IndexComposition(ValueRetriever):
-    """Retrieves and reformat index composition for a given indices and calc date."""
+    """Retrieves and reformats index composition for a given set of indices and calculation date."""
 
     def __init__(
         self,
         client: DataRetrievalServiceClient,
         indices: Union[List[str], str],
         calc_date: datetime,
     ) -> None:
-        """Initialization of class.
+        """Initialize the class.
 
         Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            indices: Indices for request.
-            calc_date: calculation date for request.
+            client: The client used to retrieve data.
+            indices:
+                List of indices or a single index for which to retrieve the composition.
+            calc_date: Calculation date for the index composition.
         """
         super(IndexComposition, self).__init__(client)
         self._client = client
-        self.indices = indices
+
+        self.indices_original: List = (
+            indices if isinstance(indices, list) else [indices]
+        )
+
+        # Convert index names to variable strings
+        _indices: List = []
+        for index in self.indices_original:
+            if isinstance(index, BondIndexName):
+                _indices.append(convert_to_variable_string(index, BondIndexName))
+            else:
+                _indices.append(index)
+        self.indices = _indices
+
         self.calc_date = calc_date
         self._data = self.get_index_composition()
 
     def get_index_composition(self) -> Mapping:
-        """Calls the client and retrieves response with index comp. from service."""
+        """Calls the client and retrieves response with index composition from the service.
+
+        Returns:
+            Dictionary containing the index composition data.
+        """
         json_response = self.get_response(self.request)
         json_response = json_response[config["results"]["index_composition"]]
 
         return json_response
 
     @property
     def url_suffix(self) -> str:
-        """Url suffix suffix for a given method."""
+        """URL suffix for the index composition endpoint.
+
+        Returns:
+            String containing the URL suffix for the index composition endpoint.
+        """
         return config["url_suffix"]["index_composition"]
 
     @property
     def request(self) -> Dict:
-        """Request dictionary for a given set of indices and calc date."""
+        """Request dictionary for a given set of indices and calculation date.
+
+        Returns:
+            Dictionary containing the request parameters for retrieving index composition.
+        """
         return {
             "symbols": self.indices,
             "date": self.calc_date.strftime("%Y-%m-%d"),
         }
 
     def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
+        """Reformat the JSON response to a dictionary.
+
+        Returns:
+            Dictionary containing the reformatted index composition data.
+        """
         _dict = {}
         for index_data in self._data:
             _index_dict = {}
             _index_dict["ISIN"] = [x["symbol"] for x in index_data["underlyings"]]
             _index_dict["Name"] = [x["name"] for x in index_data["underlyings"]]
             _index_dict["Nominal_Amount"] = [
                 convert_to_float_if_float(x["nominal"])
@@ -80,24 +112,31 @@
             ]
 
             if not _index_dict["Market_Amount"].__contains__(None):
                 sum_market = sum(_index_dict["Market_Amount"])
                 _index_dict["Market_Weight"] = [
                     x / sum_market for x in _index_dict["Market_Amount"]
                 ]
-            _dict[index_data["index_name"]["name"]] = _index_dict
+            index_original = convert_to_original_format(
+                index_data["index_name"]["name"], self.indices_original
+            )
+            _dict[index_original] = _index_dict
 
         return _dict
 
     def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
+        """Reformat the JSON response to a pandas DataFrame.
+
+        Returns:
+            Pandas DataFrame containing the reformatted index composition data.
+        """
         df = pd.DataFrame()
         _dict = self.to_dict()
         for index in _dict:
             _df = pd.DataFrame.from_dict(_dict[index])
             _df.insert(0, "Index", [index] * len(_df))
 
-            if df is pd.DataFrame.empty:
+            if df.empty:
                 df = _df
             else:
                 df = pd.concat([df, _df], axis=0)
         return df
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/LiveBondKeyFigures.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/LiveBondKeyFigures.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,132 +1,164 @@
-import json
-import math
-from typing import Any, Dict, Iterator, List, Union
-
-import numpy as np
-import pandas as pd
-
-from nordea_analytics.key_figure_names import (
-    LiveBondKeyFigureName,
-)
-from nordea_analytics.nalib.data_retrieval_client import DataRetrievalServiceClient
-from nordea_analytics.nalib.exceptions import CustomWarningCheck
-from nordea_analytics.nalib.live_keyfigures.parsing import (
-    filter_keyfigures,
-    parse_live_keyfigures_json,
-    to_data_frame,
-)
-from nordea_analytics.nalib.util import (
-    convert_to_variable_string,
-    get_config,
-    RequestMethod,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class LiveBondKeyFigures(ValueRetriever):
-    """Retrieves and reformats calculated live bond key figure."""
-
-    def __init__(
-        self,
-        symbols: Union[str, List[str]],
-        client: DataRetrievalServiceClient,
-        keyfigures: Union[
-            LiveBondKeyFigureName,
-            str,
-            List[LiveBondKeyFigureName],
-            List[str],
-            List[Union[LiveBondKeyFigureName, str]],
-        ],
-        as_df: bool,
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            symbols: ISIN or name of bonds that should be retrieved live
-            client: LiveDataRetrivalServiceClient
-            keyfigures: List of bond key figures which should be streamed.
-                Can be a list of LiveBondKeyFigureNames or string.
-            as_df: if True, the results are represented
-                as pd.DataFrame, else as dictionary
-        """
-        super(LiveBondKeyFigures, self).__init__(client)
-        self.symbols: List = [symbols] if isinstance(symbols, str) else symbols
-        _keyfigures: List = keyfigures if isinstance(keyfigures, list) else [keyfigures]
-        self.keyfigures: List = [
-            convert_to_variable_string(keyfigure, LiveBondKeyFigureName)
-            if type(keyfigure) == LiveBondKeyFigureName
-            else keyfigure.lower()
-            for keyfigure in _keyfigures
-        ]
-
-        self.keyfigures_original = _keyfigures
-        self._as_df = as_df
-        self._stream_iterator = Iterator[Any]
-        self._data = self.get_live_key_figure_response
-
-    @property
-    def get_live_key_figure_response(self) -> List[Dict]:
-        """Returns the latest available live key figures from cache."""
-        json_response: List[Any] = []
-        for request_dict in self.request:
-            response = self._client.get_response(
-                request_dict, self.url_suffix, RequestMethod.Get
-            )
-            json_response += response["keyfigure_values"]
-            CustomWarningCheck.live_key_figure_calculation_not_supported_warning(
-                response
-            )
-            CustomWarningCheck.live_key_figure_data_not_available_warning(response)
-            CustomWarningCheck.live_key_figure_access_restricted(response)
-
-        return json_response
-
-    @property
-    def stream_keyfigures(self) -> Iterator[Any]:
-        """Returns the stream listener which controls the live stream."""
-        for stream_chunk in self._client.get_live_streamer().stream(self.symbols):
-            json_payload = json.loads(stream_chunk)
-            yield self._response_decorator(json_payload)
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix suffix for a given method."""
-        return config["url_suffix"]["live_bond_key_figures"]
-
-    @property
-    def request(self) -> List[Dict]:
-        """Request list of dictionaries for a given set of bonds, key figures and calc date."""
-        if len(self.symbols) > config["max_bonds"]:
-            split_symbols = np.array_split(
-                self.symbols, math.ceil(len(self.symbols) / config["max_bonds"])
-            )
-            request_dict = [{"bonds": list(symbols)} for symbols in split_symbols]
-        else:
-            request_dict = [{"bonds": self.symbols}]
-
-        return request_dict
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        results: Dict = {}
-        for values in self._data:
-            results = results | filter_keyfigures(
-                values, self.keyfigures, self.keyfigures_original
-            )
-
-        return results
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        return to_data_frame(self.to_dict())
-
-    def _response_decorator(self, json_payload: dict) -> Any:
-        json_payload = parse_live_keyfigures_json(
-            json_payload, self.keyfigures, self.keyfigures_original
-        )
-        if self._as_df:
-            return to_data_frame(json_payload)
-
-        return json_payload
+import json
+import math
+from typing import Any, Dict, Iterator, List, Union
+
+import numpy as np
+import pandas as pd
+
+from nordea_analytics.key_figure_names import (
+    LiveBondKeyFigureName,
+)
+from nordea_analytics.nalib.data_retrieval_client import DataRetrievalServiceClient
+from nordea_analytics.nalib.exceptions import CustomWarningCheck
+from nordea_analytics.nalib.live_keyfigures.parsing import (
+    filter_keyfigures,
+    parse_live_keyfigures_json,
+    to_data_frame,
+)
+from nordea_analytics.nalib.util import (
+    convert_to_variable_string,
+    get_config,
+    RequestMethod,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class LiveBondKeyFigures(ValueRetriever):
+    """Retrieves and reformats calculated live bond key figures.
+
+    Args:
+        symbols: ISIN or name of bonds that should be retrieved live.
+        client: The client used to retrieve data.
+        keyfigures: List of bond key figures
+                        which should be streamed. Can be a list of LiveBondKeyFigureNames or string.
+        as_df: If True, the results are represented as pd.DataFrame, else as dictionary.
+    """
+
+    def __init__(
+        self,
+        symbols: Union[str, List[str]],
+        client: DataRetrievalServiceClient,
+        keyfigures: Union[
+            LiveBondKeyFigureName,
+            str,
+            List[LiveBondKeyFigureName],
+            List[str],
+            List[Union[LiveBondKeyFigureName, str]],
+        ],
+        as_df: bool,
+    ) -> None:
+        """Initialize the LiveBondKeyFigures class."""
+        super(LiveBondKeyFigures, self).__init__(client)
+        self.symbols: List = [symbols] if isinstance(symbols, str) else symbols
+        _keyfigures: List = keyfigures if isinstance(keyfigures, list) else [keyfigures]
+        self.keyfigures: List = [
+            convert_to_variable_string(keyfigure, LiveBondKeyFigureName)
+            if type(keyfigure) == LiveBondKeyFigureName
+            else keyfigure.lower()
+            for keyfigure in _keyfigures
+        ]
+
+        self.keyfigures_original = _keyfigures
+        self._as_df = as_df
+        self._stream_iterator = Iterator[Any]
+        self._data = self.get_live_key_figure_response
+
+    @property
+    def get_live_key_figure_response(self) -> List[Dict]:
+        """Returns the latest available live key figures from cache.
+
+        Returns:
+            A list of dictionaries containing the live key figure values.
+        """
+        json_response: List[Any] = []
+        for request_dict in self.request:
+            response = self._client.get_response(
+                request_dict, self.url_suffix, RequestMethod.Get
+            )
+            json_response += response["keyfigure_values"]
+            CustomWarningCheck.live_key_figure_calculation_not_supported_warning(
+                response
+            )
+            CustomWarningCheck.live_key_figure_data_not_available_warning(response)
+            CustomWarningCheck.live_key_figure_access_restricted(response)
+
+        return json_response
+
+    @property
+    def stream_keyfigures(self) -> Iterator[Any]:
+        """Returns the stream listener which controls the live stream.
+
+        Yields:
+            Stream chunks containing live key figure values.
+        """
+        for stream_chunk in self._client.get_live_streamer().stream(self.symbols):
+            json_payload = json.loads(stream_chunk)
+            yield self._response_decorator(json_payload)
+
+    @property
+    def url_suffix(self) -> str:
+        """URL suffix for the given method.
+
+        Returns:
+            URL suffix for live bond key figures.
+        """
+        return config["url_suffix"]["live_bond_key_figures"]
+
+    @property
+    def request(self) -> List[Dict]:
+        """Request list of dictionaries for a given set of bonds, key figures and calc date.
+
+        Returns:
+            A list of request dictionaries.
+        """
+        if len(self.symbols) > config["max_bonds"]:
+            split_symbols = np.array_split(
+                self.symbols, math.ceil(len(self.symbols) / config["max_bonds"])
+            )
+            request_dict = [{"bonds": list(symbols)} for symbols in split_symbols]
+        else:
+            request_dict = [{"bonds": self.symbols}]
+
+        return request_dict
+
+    def to_dict(self) -> Dict:
+        """Reformat the JSON response to a dictionary.
+
+        Returns:
+            A dictionary containing the reformatted live key figure values.
+        """
+        results: Dict = {}
+
+        for values in self._data:
+            results = results | filter_keyfigures(
+                values, self.keyfigures, self.keyfigures_original
+            )
+
+        return results
+
+    def to_df(self) -> pd.DataFrame:
+        """Reformat the JSON response to a pandas DataFrame.
+
+        Returns:
+            A pandas DataFrame containing the reformatted live key figure values.
+        """
+        return to_data_frame(self.to_dict())
+
+    def _response_decorator(self, json_payload: dict) -> Any:
+        """Decorator to process the payload and return appropriate response.
+
+        Args:
+            json_payload: Payload containing live key figure values.
+
+        Returns:
+            Either a pandas DataFrame or a dictionary containing the reformatted live key figure values.
+        """
+        json_payload = parse_live_keyfigures_json(
+            json_payload, self.keyfigures, self.keyfigures_original
+        )
+        if self._as_df:
+            return to_data_frame(json_payload)
+
+        return json_payload
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/Quotes.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/Quotes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,115 @@
-from datetime import datetime
-from typing import Any, Dict, List, Union
-
-import pandas as pd
-
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.exceptions import CustomWarningCheck
-from nordea_analytics.nalib.util import (
-    get_config,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class Quotes(ValueRetriever):
-    """Retrieves FX quotes ."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        symbols: Union[List[str], str],
-        calc_date: datetime,
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing
-            symbols: Name of instruments for request.
-            calc_date: calculation date for request.
-        """
-        super(Quotes, self).__init__(client)
-
-        self.symbols: List = [symbols] if type(symbols) != list else symbols
-        self.calc_date = calc_date
-        self._data = self.get_fx_quotes()
-
-    def get_fx_quotes(self) -> List:
-        """Calls the client and retrieves response with key figures from the service."""
-        _json_response = self.get_post_get_response()
-        json_response: List[Any] = _json_response[config["results"]["quotes"]]
-
-        return json_response
-
-    def get_post_get_response(self) -> Dict:
-        """Retrieves response after posting the request."""
-        json_response: Dict = {}
-        try:
-            json_response = self._client.get_post_get_response(
-                self.request, self.url_suffix
-            )
-        except Exception as ex:
-            CustomWarningCheck.post_response_not_retrieved_warning(
-                ex, "One or more symbols "
-            )
-
-        return json_response
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix suffix for a given method."""
-        return config["url_suffix"]["quotes"]
-
-    @property
-    def request(self) -> Dict:
-        """Request list of dictionaries for a given set of symbols, key figures and calc date."""
-        request_dict = {
-            "symbols": self.symbols,
-            "date": self.calc_date.strftime("%Y-%m-%d"),
-        }
-
-        return request_dict
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        _dict = {}
-        for bond_data in self._data:
-            _dict[bond_data["symbol"]] = bond_data["quote"]
-
-        return _dict
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        return pd.DataFrame.from_dict(self.to_dict(), orient="index", columns=["Quote"])
+from datetime import datetime
+from typing import Any, Dict, List, Union
+
+import pandas as pd
+
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.exceptions import CustomWarningCheck
+from nordea_analytics.nalib.util import (
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class Quotes(ValueRetriever):
+    """Retrieves FX quotes.
+
+    This class inherits from ValueRetriever and provides methods to retrieve and reformat FX quote data
+    from a DataRetrievalServiceClient instance.
+    """
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        symbols: Union[List[str], str],
+        calc_date: datetime,
+    ) -> None:
+        """Initializes the Quotes instance.
+
+        Args:
+            client: The client used to retrieve data.
+            symbols: Name of instruments for request.
+            calc_date: Calculation date for request.
+        """
+        super(Quotes, self).__init__(client)
+
+        # Convert symbols to list if it's not already a list
+        self.symbols: List = [symbols] if type(symbols) != list else symbols
+        self.calc_date = calc_date
+        self._data = self.get_fx_quotes()
+
+    def get_fx_quotes(self) -> List:
+        """Calls the client and retrieves response with FX quote data from the service.
+
+        Returns:
+            A list of dictionaries containing FX quote data.
+        """
+        _json_response = self.get_post_get_response()
+        json_response: List[Any] = _json_response[config["results"]["quotes"]]
+
+        return json_response
+
+    def get_post_get_response(self) -> Dict:
+        """Retrieves response after posting the request.
+
+        Returns:
+            A dictionary containing the response data.
+        """
+        json_response: Dict = {}
+        try:
+            json_response = self._client.get_post_get_response(
+                self.request, self.url_suffix
+            )
+        except Exception as ex:
+            CustomWarningCheck.post_response_not_retrieved_warning(
+                ex, "One or more symbols "
+            )
+
+        return json_response
+
+    @property
+    def url_suffix(self) -> str:
+        """Returns the URL suffix for FX quotes.
+
+        Returns:
+            The URL suffix for FX quotes.
+        """
+        return config["url_suffix"]["quotes"]
+
+    @property
+    def request(self) -> Dict:
+        """Returns a request dictionary for a given set of symbols and calculation date.
+
+        Returns:
+            A dictionary representing the request data.
+        """
+        request_dict = {
+            "symbols": self.symbols,
+            "date": self.calc_date.strftime("%Y-%m-%d"),
+        }
+
+        return request_dict
+
+    def to_dict(self) -> Dict:
+        """Reformats the JSON response to a dictionary.
+
+        Returns:
+            A dictionary containing the reformatted data from the JSON response.
+        """
+        _dict = {}
+        for quote_data in self._data:
+            _dict[quote_data["symbol"]] = quote_data["quote"]
+
+        return _dict
+
+    def to_df(self) -> pd.DataFrame:
+        """Reformats the JSON response to a pandas DataFrame.
+
+        Returns:
+            A pandas DataFrame containing the reformatted data from the JSON response.
+        """
+        return pd.DataFrame.from_dict(self.to_dict(), orient="index", columns=["Quote"])
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/ShiftDays.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/ShiftDays.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,136 @@
-from datetime import datetime
-import typing
-from typing import Dict, Union
-
-import pandas as pd
-
-from nordea_analytics.convention_variable_names import (
-    DateRollConvention,
-    DayCountConvention,
-    Exchange,
-)
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.util import (
-    convert_to_variable_string,
-    get_config,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class ShiftDays(ValueRetriever):
-    """Shifts a datetime by a given number of days."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        date: datetime,
-        days: int,
-        exchange: Union[str, Exchange] = None,
-        day_count_convention: Union[str, DayCountConvention] = None,
-        date_roll_convention: Union[str, DateRollConvention] = None,
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            date: The date that will be shifted.
-            days: The number of days to shift 'date' with.
-                Negative values move date back in time.
-            exchange: The exchange's holiday calendar will be used.
-            day_count_convention: The convention to use for counting days.
-            date_roll_convention: The convention to use for rolling
-                when a holiday is encountered.
-        """
-        super(ShiftDays, self).__init__(client)
-        self._client = client
-        self.date = date
-        self.days = days
-        self.exchange = (
-            convert_to_variable_string(exchange, Exchange)
-            if type(exchange) == Exchange
-            else exchange
-        )
-        self.day_count_convention = (
-            convert_to_variable_string(day_count_convention, DayCountConvention)
-            if type(day_count_convention) == DayCountConvention
-            else day_count_convention
-        )
-        self.date_roll_convention = (
-            convert_to_variable_string(date_roll_convention, DateRollConvention)
-            if type(date_roll_convention) == DateRollConvention
-            else date_roll_convention
-        )
-        self._data = self.shift_days()
-
-    def shift_days(self) -> Dict:
-        """Retrieves response with shifted date."""
-        json_response = self.get_response(self.request)
-
-        return json_response[config["results"]["shift_days"]]
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix for a given method."""
-        return config["url_suffix"]["shift_days"]
-
-    @property
-    def request(self) -> dict:
-        """Request shifted date."""
-        date = self.date.strftime("%Y-%m-%d")
-        days = self.days
-        exchange = self.exchange
-        day_count_convention = self.day_count_convention
-        date_roll_convention = self.date_roll_convention
-
-        request_dict = {
-            "date": date,
-            "days": days,
-            "exchange": exchange,
-            "day-count-convention": day_count_convention,
-            "date-roll-convention": date_roll_convention,
-        }
-
-        return request_dict
-
-    def to_datetime(self) -> datetime:
-        """Reformat the json response to a datetime."""
-        shifted_date_string = typing.cast(str, self._data["date"])
-
-        shifted_date = datetime.strptime(shifted_date_string, "%Y-%m-%d")
-        return shifted_date
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        pass
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        pass
+from datetime import datetime
+import typing
+from typing import Dict, Union
+
+import pandas as pd
+
+from nordea_analytics.convention_variable_names import (
+    DateRollConvention,
+    DayCountConvention,
+    Exchange,
+)
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.util import (
+    convert_to_variable_string,
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class ShiftDays(ValueRetriever):
+    """Shifts a datetime by a given number of days."""
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        date: datetime,
+        days: int,
+        exchange: Union[str, Exchange] = None,
+        day_count_convention: Union[str, DayCountConvention] = None,
+        date_roll_convention: Union[str, DateRollConvention] = None,
+    ) -> None:
+        """Initialization of class.
+
+        Args:
+            client: The client used to retrieve data.
+            date: The date that will be shifted.
+            days: The number of days to shift 'date' with.
+                Negative values move date back in time.
+            exchange: The exchange's holiday calendar to be used.
+            day_count_convention: The convention to use for counting days.
+            date_roll_convention: The convention to use for rolling
+                when a holiday is encountered.
+        """
+        super(ShiftDays, self).__init__(client)
+        self._client = client
+        self.date = date
+        self.days = days
+        self.exchange = (
+            convert_to_variable_string(exchange, Exchange)
+            if type(exchange) == Exchange
+            else exchange
+        )
+        self.day_count_convention = (
+            convert_to_variable_string(day_count_convention, DayCountConvention)
+            if type(day_count_convention) == DayCountConvention
+            else day_count_convention
+        )
+        self.date_roll_convention = (
+            convert_to_variable_string(date_roll_convention, DateRollConvention)
+            if type(date_roll_convention) == DateRollConvention
+            else date_roll_convention
+        )
+        self._data = self.shift_days()
+
+    def shift_days(self) -> Dict:
+        """Shifts the date by the specified number of days and retrieves the response with the shifted date.
+
+        Returns:
+            The JSON response with the shifted date.
+        """
+        json_response = self.get_response(self.request)
+
+        return json_response[config["results"]["shift_days"]]
+
+    @property
+    def url_suffix(self) -> str:
+        """Get the URL suffix for the API endpoint.
+
+        Returns:
+            The URL suffix for the API endpoint.
+        """
+        return config["url_suffix"]["shift_days"]
+
+    @property
+    def request(self) -> dict:
+        """Construct the request dictionary for the API call.
+
+        Returns:
+            The request dictionary for the API call.
+        """
+        date = self.date.strftime("%Y-%m-%d")
+        days = self.days
+        exchange = self.exchange
+        day_count_convention = self.day_count_convention
+        date_roll_convention = self.date_roll_convention
+
+        request_dict = {
+            "date": date,
+            "days": days,
+            "exchange": exchange,
+            "day-count-convention": day_count_convention,
+            "date-roll-convention": date_roll_convention,
+        }
+
+        return request_dict
+
+    def to_datetime(self) -> datetime:
+        """Convert the JSON response to a datetime object.
+
+        Returns:
+            The datetime object representing the shifted date.
+        """
+        shifted_date_string = typing.cast(str, self._data["date"])
+
+        shifted_date = datetime.strptime(shifted_date_string, "%Y-%m-%d")
+        return shifted_date
+
+    def to_dict(self) -> Dict:
+        """Convert the JSON response to a dictionary.
+
+        Returns:
+            The dictionary representing the JSON response.
+        """
+        pass
+
+    def to_df(self) -> pd.DataFrame:
+        """Convert the JSON response to a pandas DataFrame.
+
+        Returns:
+            The pandas DataFrame representing the JSON response.
+        """
+        pass
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/TimeSeries.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/TimeSeries.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,210 +1,239 @@
-from datetime import datetime, timedelta
-import math
-from typing import Any, Dict, List, Union
-
-import numpy as np
-import pandas as pd
-
-from nordea_analytics.instrument_variable_names import BenchmarkName, BondIndexName
-from nordea_analytics.key_figure_names import (
-    TimeSeriesKeyFigureName,
-)
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.util import (
-    convert_to_float_if_float,
-    convert_to_original_format,
-    convert_to_variable_string,
-    get_config,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class TimeSeries(ValueRetriever):
-    """Retrieves and reformat time series."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        symbols: Union[
-            str,
-            BondIndexName,
-            BenchmarkName,
-            List[str],
-            List[BenchmarkName],
-            List[BondIndexName],
-            List[Union[str, BenchmarkName, BondIndexName]],
-        ],
-        keyfigures: Union[
-            TimeSeriesKeyFigureName,
-            str,
-            List[str],
-            List[TimeSeriesKeyFigureName],
-            List[Union[str, TimeSeriesKeyFigureName]],
-        ],
-        from_date: datetime,
-        to_date: datetime,
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            symbols: Bonds, swaps, FX, FX swap point.
-            keyfigures: Key figure names for request. If symbol is
-                something else than a bonds, quote should be chosen.
-            from_date: From date for calc date interval.
-            to_date: To date for calc date interval.
-        """
-        super(TimeSeries, self).__init__(client)
-        self._client = client
-        self.symbols_original: List = (
-            symbols if isinstance(symbols, list) else [symbols]
-        )
-
-        _symbols: List = []
-        for symbol in self.symbols_original:
-            if isinstance(symbol, BenchmarkName):
-                _symbols.append(convert_to_variable_string(symbol, BenchmarkName))
-            elif isinstance(symbol, BondIndexName):
-                _symbols.append(convert_to_variable_string(symbol, BondIndexName))
-            else:
-                _symbols.append(symbol)
-        self.symbols = _symbols
-
-        self.keyfigures_original: List = (
-            keyfigures if isinstance(keyfigures, list) else [keyfigures]
-        )
-        self.keyfigures = [
-            convert_to_variable_string(keyfigure, TimeSeriesKeyFigureName)
-            if type(keyfigure) == TimeSeriesKeyFigureName
-            else keyfigure
-            for keyfigure in self.keyfigures_original
-        ]
-        self.from_date = from_date
-        self.to_date = to_date
-
-        self._data = self.get_time_series()
-
-    def get_time_series(self) -> List:
-        """Retrieves response with key figures time series."""
-        json_response: List[Any] = []
-        for request_dict in self.request:
-            _json_response = self.get_response(request_dict)
-            json_map = _json_response[config["results"]["time_series"]]
-            json_response = list(json_map) + json_response
-
-        return json_response
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix for a given method."""
-        return config["url_suffix"]["time_series"]
-
-    @property
-    def request(self) -> List[Dict]:
-        """Request dictionary time series key figures."""
-        intv = config["max_years_timeseries"] * 365
-        date_interv = []
-        new_from_date = self.from_date
-        while (self.to_date - new_from_date).days > intv:
-            new_to_date = new_from_date + timedelta(days=intv)
-            date_interv.append({"from": new_from_date, "to": new_to_date})
-            new_from_date = new_from_date + timedelta(days=intv + 1)
-            if new_from_date > self.to_date:
-                new_from_date = self.to_date
-
-        date_interv.append({"from": new_from_date, "to": self.to_date})
-
-        split_symbol = np.array_split(
-            self.symbols, math.ceil(len(self.symbols) / config["max_symbol_timeseries"])
-        )
-
-        request_dict = [
-            {
-                "symbols": list(symbol),
-                "keyfigure": keyfigure,
-                "from": dates["from"].strftime("%Y-%m-%d"),
-                "to": dates["to"].strftime("%Y-%m-%d"),
-            }
-            for dates in date_interv
-            for symbol in split_symbol
-            for keyfigure in self.keyfigures
-        ]
-
-        return request_dict
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        _dict: Dict[Any, Any] = {}
-        for symbol_data in self._data:
-            _timeseries_dict: Dict[Any, Any] = {}
-            symbol_original = convert_to_original_format(
-                symbol_data["symbol"], self.symbols_original
-            )
-            for timeseries in symbol_data["timeseries"]:
-                key_figure_original = convert_to_original_format(
-                    timeseries["keyfigure"], self.keyfigures_original
-                )
-                _timeseries_dict[key_figure_original] = {}
-                _timeseries_dict[key_figure_original]["Date"] = [
-                    datetime.strptime(x["key"], "%Y-%m-%d")
-                    for x in timeseries["values"]
-                ]
-                _timeseries_dict[key_figure_original]["Value"] = [
-                    convert_to_float_if_float(x["value"]) for x in timeseries["values"]
-                ]
-
-                if symbol_data["symbol"] in _dict.keys():
-                    if key_figure_original in _dict[symbol_data["symbol"]].keys():
-                        if (
-                            _dict[symbol_original][key_figure_original]["Date"][-1]
-                            > _timeseries_dict[key_figure_original]["Date"][0]
-                        ):
-                            _dict[symbol_original][key_figure_original][
-                                "Date"
-                            ] += _timeseries_dict[key_figure_original]["Date"]
-                            _dict[symbol_original][key_figure_original][
-                                "Value"
-                            ] += _timeseries_dict[key_figure_original]["Value"]
-                        else:
-                            _dict[symbol_original][key_figure_original]["Date"] = (
-                                _timeseries_dict[key_figure_original]["Date"]
-                                + _dict[symbol_original][key_figure_original]["Date"]
-                            )
-                            _dict[symbol_original][key_figure_original]["Value"] = (
-                                _timeseries_dict[key_figure_original]["Value"]
-                                + _dict[symbol_original][key_figure_original]["Value"]
-                            )
-                    else:
-                        _dict[symbol_original].update(_timeseries_dict)
-                else:
-                    _dict[symbol_original] = _timeseries_dict
-
-        return _dict
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        df = pd.DataFrame()
-        _dict = self.to_dict()
-        for symbol in _dict:
-            _df = pd.DataFrame.empty
-            for keyfigure in _dict[symbol]:
-                _df_keyfigure = pd.DataFrame.from_dict(_dict[symbol][keyfigure])
-                _df_keyfigure = _df_keyfigure[["Date", "Value"]]
-                _df_keyfigure.columns = ["Date", keyfigure]
-                if _df is pd.DataFrame.empty:
-                    _df = _df_keyfigure
-                else:
-                    _df = _df.merge(_df_keyfigure, on="Date", how="outer")
-            _df = _df.sort_values(by="Date")
-            _df.insert(0, "Symbol", [symbol] * len(_df))
-
-            if df.empty:
-                df = _df
-            else:
-                df = pd.concat([df, _df], axis=0)
-        return df.reset_index(drop=True)
+from datetime import datetime, timedelta
+import math
+from typing import Any, Dict, List, Union
+
+import numpy as np
+import pandas as pd
+
+from nordea_analytics.instrument_variable_names import BenchmarkName, BondIndexName
+from nordea_analytics.key_figure_names import (
+    TimeSeriesKeyFigureName,
+)
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.util import (
+    convert_to_float_if_float,
+    convert_to_original_format,
+    convert_to_variable_string,
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class TimeSeries(ValueRetriever):
+    """Retrieves and reformats time series data."""
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        symbols: Union[
+            str,
+            BondIndexName,
+            BenchmarkName,
+            List[str],
+            List[BenchmarkName],
+            List[BondIndexName],
+            List[Union[str, BenchmarkName, BondIndexName]],
+        ],
+        keyfigures: Union[
+            TimeSeriesKeyFigureName,
+            str,
+            List[str],
+            List[TimeSeriesKeyFigureName],
+            List[Union[str, TimeSeriesKeyFigureName]],
+        ],
+        from_date: datetime,
+        to_date: datetime,
+    ) -> None:
+        """Initialization of the TimeSeries class.
+
+        Args:
+            client: The client used to retrieve data.
+            symbols: Bonds, swaps, FX, FX swap point.
+            keyfigures: Key figure names for request.
+                 If symbol is something else than a bond, quote should be chosen.
+            from_date: From date for calculating date interval.
+            to_date: To date for calculating date interval.
+        """
+        super(TimeSeries, self).__init__(client)
+        self._client = client
+        self.symbols_original: List = (
+            symbols if isinstance(symbols, list) else [symbols]
+        )
+
+        # Convert symbol names to variable strings
+        _symbols: List = []
+        for symbol in self.symbols_original:
+            if isinstance(symbol, BenchmarkName):
+                _symbols.append(convert_to_variable_string(symbol, BenchmarkName))
+            elif isinstance(symbol, BondIndexName):
+                _symbols.append(convert_to_variable_string(symbol, BondIndexName))
+            else:
+                _symbols.append(symbol)
+        self.symbols = _symbols
+
+        self.keyfigures_original: List = (
+            keyfigures if isinstance(keyfigures, list) else [keyfigures]
+        )
+
+        # Convert key figure names to variable strings
+        self.keyfigures = [
+            convert_to_variable_string(keyfigure, TimeSeriesKeyFigureName)
+            if isinstance(keyfigure, TimeSeriesKeyFigureName)
+            else keyfigure
+            for keyfigure in self.keyfigures_original
+        ]
+
+        self.from_date = from_date
+        self.to_date = to_date
+
+        self._data = self.get_time_series()
+
+    def get_time_series(self) -> List:
+        """Retrieves response with key figures time series.
+
+        Returns:
+            List of JSON response with key figures time series.
+        """
+        json_response: List[Any] = []
+
+        # Loop through each request dictionary and get the response
+        for request_dict in self.request:
+            _json_response = self.get_response(request_dict)
+            json_map = _json_response[config["results"]["time_series"]]
+            json_response = list(json_map) + json_response
+
+        return json_response
+
+    @property
+    def url_suffix(self) -> str:
+        """Url suffix for a given method.
+
+        Returns:
+            Url suffix for a given method.
+        """
+        return config["url_suffix"]["time_series"]
+
+    @property
+    def request(self) -> List[Dict]:
+        """Request dictionary time series key figures.
+
+        Returns:
+            List of request dictionaries for time series key figures.
+        """
+        intv = config["max_years_timeseries"] * 365
+        date_interv = []
+        new_from_date = self.from_date
+
+        # Calculate date intervals for the given from_date and to_date
+        while (self.to_date - new_from_date).days > intv:
+            new_to_date = new_from_date + timedelta(days=intv)
+            date_interv.append({"from": new_from_date, "to": new_to_date})
+            new_from_date = new_from_date + timedelta(days=intv + 1)
+            if new_from_date > self.to_date:
+                new_from_date = self.to_date
+
+        date_interv.append({"from": new_from_date, "to": self.to_date})
+
+        # Split symbols into smaller chunks to avoid exceeding maximum symbol limit
+        split_symbol = np.array_split(
+            self.symbols, math.ceil(len(self.symbols) / config["max_symbol_timeseries"])
+        )
+
+        # Generate request dictionaries for each date interval, symbol, and key figure
+        request_dict = [
+            {
+                "symbols": list(symbol),
+                "keyfigure": keyfigure,
+                "from": dates["from"].strftime("%Y-%m-%d"),
+                "to": dates["to"].strftime("%Y-%m-%d"),
+            }
+            for dates in date_interv
+            for symbol in split_symbol
+            for keyfigure in self.keyfigures
+        ]
+
+        return request_dict
+
+    def to_dict(self) -> Dict:
+        """Reformat the JSON response to a dictionary.
+
+        Returns:
+            A dictionary containing the reformatted data.
+        """
+        _dict: Dict[Any, Any] = {}
+        for symbol_data in self._data:
+            _timeseries_dict: Dict[Any, Any] = {}
+            symbol_original = convert_to_original_format(
+                symbol_data["symbol"], self.symbols_original
+            )
+            for timeseries in symbol_data["timeseries"]:
+                key_figure_original = convert_to_original_format(
+                    timeseries["keyfigure"], self.keyfigures_original
+                )
+                _timeseries_dict[key_figure_original] = {}
+                _timeseries_dict[key_figure_original]["Date"] = [
+                    datetime.strptime(x["key"], "%Y-%m-%d")
+                    for x in timeseries["values"]
+                ]
+                _timeseries_dict[key_figure_original]["Value"] = [
+                    convert_to_float_if_float(x["value"]) for x in timeseries["values"]
+                ]
+
+                if symbol_data["symbol"] in _dict.keys():
+                    if key_figure_original in _dict[symbol_data["symbol"]].keys():
+                        if (
+                            _dict[symbol_original][key_figure_original]["Date"][-1]
+                            > _timeseries_dict[key_figure_original]["Date"][0]
+                        ):
+                            _dict[symbol_original][key_figure_original][
+                                "Date"
+                            ] += _timeseries_dict[key_figure_original]["Date"]
+                            _dict[symbol_original][key_figure_original][
+                                "Value"
+                            ] += _timeseries_dict[key_figure_original]["Value"]
+                        else:
+                            _dict[symbol_original][key_figure_original]["Date"] = (
+                                _timeseries_dict[key_figure_original]["Date"]
+                                + _dict[symbol_original][key_figure_original]["Date"]
+                            )
+                            _dict[symbol_original][key_figure_original]["Value"] = (
+                                _timeseries_dict[key_figure_original]["Value"]
+                                + _dict[symbol_original][key_figure_original]["Value"]
+                            )
+                    else:
+                        _dict[symbol_original].update(_timeseries_dict)
+                else:
+                    _dict[symbol_original] = _timeseries_dict
+
+        return _dict
+
+    def to_df(self) -> pd.DataFrame:
+        """Reformat the JSON response to a pandas DataFrame.
+
+        Returns:
+            A pandas DataFrame containing the reformatted data.
+        """
+        df = pd.DataFrame()
+        _dict = self.to_dict()
+        for symbol in _dict:
+            _df = pd.DataFrame.empty
+            for keyfigure in _dict[symbol]:
+                _df_keyfigure = pd.DataFrame.from_dict(_dict[symbol][keyfigure])
+                _df_keyfigure = _df_keyfigure[["Date", "Value"]]
+                _df_keyfigure.columns = ["Date", keyfigure]
+                if _df is pd.DataFrame.empty:
+                    _df = _df_keyfigure
+                else:
+                    _df = _df.merge(_df_keyfigure, on="Date", how="outer")
+            _df = _df.sort_values(by="Date")
+            _df.insert(0, "Symbol", [symbol] * len(_df))
+
+            if df.empty:
+                df = _df
+            else:
+                df = pd.concat([df, _df], axis=0)
+        return df.reset_index(drop=True)
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/YearFraction.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/YearFraction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,113 @@
-from datetime import datetime
-from typing import Dict, Union
-
-import pandas as pd
-
-from nordea_analytics import TimeConvention
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.util import (
-    convert_to_variable_string,
-    get_config,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class YearFraction(ValueRetriever):
-    """Calculate the time between two dates in terms of years."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        from_date: datetime,
-        to_date: datetime,
-        time_convention: Union[str, TimeConvention],
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            from_date: The start date of the time calculation.
-            to_date: The end date of the time calculation.
-            time_convention: The convention to use for counting time.
-        """
-        super(YearFraction, self).__init__(client)
-        self._client = client
-        self.from_date = from_date
-        self.to_date = to_date
-        self.time_convention = (
-            convert_to_variable_string(time_convention, TimeConvention)
-            if type(time_convention) == TimeConvention
-            else time_convention
-        )
-        self._data = self.year_fraction()
-
-    def year_fraction(self) -> Dict:
-        """Retrieves response with year fraction."""
-        json_response = self.get_response(self.request)
-
-        return json_response[config["results"]["year_fraction"]]
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix for a given method."""
-        return config["url_suffix"]["year_fraction"]
-
-    @property
-    def request(self) -> dict:
-        """Request year fraction."""
-        from_date = self.from_date.strftime("%Y-%m-%d")
-        to_date = self.to_date.strftime("%Y-%m-%d")
-        time_convention = self.time_convention
-
-        request_dict = {
-            "from": from_date,
-            "to": to_date,
-            "time-convention": time_convention,
-        }
-
-        return request_dict
-
-    def to_float(self) -> float:
-        """Reformat the json response to a float."""
-        year_fraction = self._data["year_fraction"]
-
-        return year_fraction
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        pass
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        pass
+from datetime import datetime
+from typing import Dict, Union
+
+import pandas as pd
+
+from nordea_analytics import TimeConvention
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.util import (
+    convert_to_variable_string,
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class YearFraction(ValueRetriever):
+    """Calculate the time between two dates in terms of years.
+
+    Inherits from ValueRetriever class.
+    """
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        from_date: datetime,
+        to_date: datetime,
+        time_convention: Union[str, TimeConvention],
+    ) -> None:
+        """Initialization of class.
+
+        Args:
+            client: The client used to retrieve data.
+            from_date: The start date of the time calculation.
+            to_date: The end date of the time calculation.
+            time_convention: The convention to use for counting time.
+        """
+        super(YearFraction, self).__init__(client)
+        self._client = client
+        self.from_date = from_date
+        self.to_date = to_date
+        self.time_convention = (
+            convert_to_variable_string(time_convention, TimeConvention)
+            if type(time_convention) == TimeConvention
+            else time_convention
+        )
+        self._data = self.year_fraction()
+
+    def year_fraction(self) -> Dict:
+        """Retrieve response with year fraction.
+
+        Returns:
+            JSON response with year fraction.
+        """
+        json_response = self.get_response(self.request)
+
+        return json_response[config["results"]["year_fraction"]]
+
+    @property
+    def url_suffix(self) -> str:
+        """URL suffix for the year_fraction method.
+
+        Returns:
+            URL suffix for year_fraction.
+        """
+        return config["url_suffix"]["year_fraction"]
+
+    @property
+    def request(self) -> dict:
+        """Generate request for year fraction.
+
+        Returns:
+            Request dictionary for year fraction.
+        """
+        from_date = self.from_date.strftime("%Y-%m-%d")
+        to_date = self.to_date.strftime("%Y-%m-%d")
+        time_convention = self.time_convention
+
+        request_dict = {
+            "from": from_date,
+            "to": to_date,
+            "time-convention": time_convention,
+        }
+
+        return request_dict
+
+    def to_float(self) -> float:
+        """Reformat the JSON response to a float.
+
+        Returns:
+            Year fraction as a float.
+        """
+        year_fraction = self._data["year_fraction"]
+
+        return year_fraction
+
+    def to_dict(self) -> Dict:
+        """Reformat the JSON response to a dictionary.
+
+        Returns:
+            Year fraction as a dictionary.
+        """
+        pass
+
+    def to_df(self) -> pd.DataFrame:
+        """Reformat the JSON response to a pandas DataFrame.
+
+        Returns:
+            Year fraction as a DataFrame.
+        """
+        pass
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nalib/value_retrievers/YieldForecast.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nalib/value_retrievers/YieldForecast.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,134 @@
-from datetime import datetime
-from typing import Any, Dict, Mapping, Union
-
-import pandas as pd
-
-from nordea_analytics.forecast_names import YieldCountry, YieldHorizon, YieldType
-from nordea_analytics.nalib.data_retrieval_client import (
-    DataRetrievalServiceClient,
-)
-from nordea_analytics.nalib.util import (
-    convert_to_variable_string,
-    get_config,
-)
-from nordea_analytics.nalib.value_retriever import ValueRetriever
-
-config = get_config()
-
-
-class YieldForecast(ValueRetriever):
-    """Retrieves and reformat Yield forecast."""
-
-    def __init__(
-        self,
-        client: DataRetrievalServiceClient,
-        country: Union[str, YieldCountry],
-        yield_type: Union[str, YieldType],
-        yield_horizon: Union[str, YieldHorizon],
-    ) -> None:
-        """Initialization of class.
-
-        Args:
-            client: DataRetrievalServiceClient
-                or DataRetrievalServiceClientTest for testing.
-            country: Country of the yield for which to retrieve forecasts.
-            yield_type: Type of yield for which to retrieve forecasts.
-            yield_horizon: Horizon for which to retrieve forecasts.
-        """
-        super(YieldForecast, self).__init__(client)
-        self._client = client
-        self.country = convert_to_variable_string(country, YieldCountry)
-        self.yield_type = convert_to_variable_string(yield_type, YieldType)
-        self.yield_horizon = convert_to_variable_string(yield_horizon, YieldHorizon)
-        self._data = self.get_yield_forecast()
-
-    def get_yield_forecast(self) -> Mapping:
-        """Retrieves response with yield forecast."""
-        json_response = self.get_response(self.request)
-        json_response = json_response[config["results"]["yield_forecast"]]
-
-        return json_response
-
-    @property
-    def url_suffix(self) -> str:
-        """Url suffix for a given method."""
-        return config["url_suffix"]["yield_forecast"]
-
-    @property
-    def request(self) -> Dict:
-        """Request dictionary yield forecast."""
-        country = self.country
-        yield_type = self.yield_type
-        yield_horizon = self.yield_horizon
-
-        request_dict = {
-            "country": country,
-            "yield-type": yield_type,
-            "yield-horizon": yield_horizon,
-        }
-
-        return request_dict
-
-    def to_dict(self) -> Dict:
-        """Reformat the json response to a dictionary."""
-        _dict: Dict[Any, Any] = {}
-
-        forecast_data = {}
-
-        for yield_type_data in self._data["forecasts"]:
-            yield_type_forecast_data = {}
-            type = yield_type_data["type"]
-
-            for data in yield_type_data["forecast"]:
-                values = {}
-
-                values["Updated_at"] = datetime.strptime(
-                    yield_type_data["updated_at"].split("T")[0], "%Y-%m-%d"
-                )
-
-                values["Value"] = data["value"]
-                yield_type_forecast_data[data["horizon"]] = values
-
-            forecast_data[type] = yield_type_forecast_data
-
-        _dict[self._data["symbol"]] = forecast_data
-
-        return _dict
-
-    def to_df(self) -> pd.DataFrame:
-        """Reformat the json response to a pandas DataFrame."""
-        _dict = self.to_dict()
-
-        df = pd.DataFrame.from_dict(
-            {
-                (i, j, k): _dict[i][j][k]
-                for i in _dict.keys()
-                for j in _dict[i].keys()
-                for k in _dict[i][j].keys()
-            },
-            orient="index",
-        )
-        df = df.reset_index().rename(
-            columns={"level_0": "Symbol", "level_1": "Yield_type", "level_2": "Horizon"}
-        )
-
-        return df
+from datetime import datetime
+from typing import Any, Dict, Mapping, Union
+
+import pandas as pd
+
+from nordea_analytics.forecast_names import YieldCountry, YieldHorizon, YieldType
+from nordea_analytics.nalib.data_retrieval_client import (
+    DataRetrievalServiceClient,
+)
+from nordea_analytics.nalib.util import (
+    convert_to_variable_string,
+    get_config,
+)
+from nordea_analytics.nalib.value_retriever import ValueRetriever
+
+config = get_config()
+
+
+class YieldForecast(ValueRetriever):
+    """Retrieves and reformats yield forecast."""
+
+    def __init__(
+        self,
+        client: DataRetrievalServiceClient,
+        country: Union[str, YieldCountry],
+        yield_type: Union[str, YieldType],
+        yield_horizon: Union[str, YieldHorizon],
+    ) -> None:
+        """Initializes the YieldForecast class.
+
+        Args:
+            client: The client used to retrieve data.
+            country : Country of the yield for which to retrieve forecasts.
+            yield_type: Type of yield for which to retrieve forecasts.
+            yield_horizon: Horizon for which to retrieve forecasts.
+        """
+        super(YieldForecast, self).__init__(client)
+        self._client = client
+        self.country = convert_to_variable_string(country, YieldCountry)
+        self.yield_type = convert_to_variable_string(yield_type, YieldType)
+        self.yield_horizon = convert_to_variable_string(yield_horizon, YieldHorizon)
+        self._data = self.get_yield_forecast()
+
+    def get_yield_forecast(self) -> Mapping:
+        """Retrieves response with yield forecast.
+
+        Returns:
+            JSON response containing the yield forecast.
+        """
+        json_response = self.get_response(self.request)
+        json_response = json_response[config["results"]["yield_forecast"]]
+
+        return json_response
+
+    @property
+    def url_suffix(self) -> str:
+        """Returns the URL suffix for the yield forecast API endpoint.
+
+        Returns:
+            URL suffix for the yield forecast API endpoint.
+        """
+        return config["url_suffix"]["yield_forecast"]
+
+    @property
+    def request(self) -> Dict:
+        """Returns the request dictionary for the yield forecast API call.
+
+        Returns:
+            Request dictionary for the yield forecast API call.
+        """
+        country = self.country
+        yield_type = self.yield_type
+        yield_horizon = self.yield_horizon
+
+        request_dict = {
+            "country": country,
+            "yield-type": yield_type,
+            "yield-horizon": yield_horizon,
+        }
+
+        return request_dict
+
+    def to_dict(self) -> Dict:
+        """Reformat the JSON response to a dictionary.
+
+        Returns:
+            Reformatted dictionary containing yield forecast data.
+        """
+        _dict: Dict[Any, Any] = {}
+
+        forecast_data = {}
+
+        for yield_type_data in self._data["forecasts"]:
+            yield_type_forecast_data = {}
+            yield_type = yield_type_data["type"]
+
+            for data in yield_type_data["forecast"]:
+                values = {}
+
+                values["Updated_at"] = datetime.strptime(
+                    yield_type_data["updated_at"].split("T")[0], "%Y-%m-%d"
+                )
+
+                values["Value"] = data["value"]
+                yield_type_forecast_data[data["horizon"]] = values
+
+            forecast_data[yield_type] = yield_type_forecast_data
+
+        _dict[self._data["symbol"]] = forecast_data
+
+        return _dict
+
+    def to_df(self) -> pd.DataFrame:
+        """Reformat the JSON response to a pandas DataFrame.
+
+        Returns:
+            Reformatted pandas DataFrame containing yield forecast data.
+        """
+        _dict = self.to_dict()
+
+        df = pd.DataFrame.from_dict(
+            {
+                (i, j, k): _dict[i][j][k]
+                for i in _dict.keys()
+                for j in _dict[i].keys()
+                for k in _dict[i][j].keys()
+            },
+            orient="index",
+        )
+        df = df.reset_index().rename(
+            columns={"level_0": "Symbol", "level_1": "Yield_type", "level_2": "Horizon"}
+        )
+
+        return df
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/nordea_analytics_service/core.py` & `nordea-analytics-1.9.0/src/nordea_analytics/nordea_analytics_service/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     SpotForward,
 )
 from nordea_analytics.forecast_names import YieldCountry, YieldHorizon, YieldType
 from nordea_analytics.instrument_variable_names import BenchmarkName, BondIndexName
 from nordea_analytics.key_figure_names import (
     BondKeyFigureName,
     CalculatedBondKeyFigureName,
+    CalculatedRepoBondKeyFigureName,
     HorizonCalculatedBondKeyFigureName,
     LiveBondKeyFigureName,
     TimeSeriesKeyFigureName,
 )
 from nordea_analytics.nalib.data_retrieval_client import DataRetrievalServiceClient
 from nordea_analytics.nalib.util import pretty_dict_string
 from nordea_analytics.nalib.value_retriever import ValueRetriever
@@ -31,14 +32,17 @@
 from nordea_analytics.nalib.value_retrievers.BondKeyFigureCalculator import (
     BondKeyFigureCalculator,
 )
 from nordea_analytics.nalib.value_retrievers.BondKeyFigureHorizonCalculator import (
     BondKeyFigureHorizonCalculator,
 )
 from nordea_analytics.nalib.value_retrievers.BondKeyFigures import BondKeyFigures
+from nordea_analytics.nalib.value_retrievers.BondRepoCalculator import (
+    BondRepoCalculator,
+)
 from nordea_analytics.nalib.value_retrievers.Curve import Curve
 from nordea_analytics.nalib.value_retrievers.CurveDefinition import CurveDefinition
 from nordea_analytics.nalib.value_retrievers.CurveTimeSeries import CurveTimeSeries
 from nordea_analytics.nalib.value_retrievers.DateSequence import DateSequence
 from nordea_analytics.nalib.value_retrievers.FXForecast import FXForecast
 from nordea_analytics.nalib.value_retrievers.IndexComposition import IndexComposition
 from nordea_analytics.nalib.value_retrievers.LiveBondKeyFigures import (
@@ -545,14 +549,63 @@
                 reinvestment_rate,
                 spread_change_horizon,
                 align_to_forward_curve,
             ),
             as_df,
         )
 
+    def calculate_repo_bond_key_figure(
+        self,
+        symbols: Union[str, List[str]],
+        keyfigures: Union[
+            str,
+            CalculatedRepoBondKeyFigureName,
+            List[str],
+            List[CalculatedRepoBondKeyFigureName],
+            List[Union[str, CalculatedRepoBondKeyFigureName]],
+        ],
+        calc_date: datetime,
+        forward_date: datetime,
+        prices: Union[float, List[float]] = None,
+        forward_prices: Union[float, List[float]] = None,
+        repo_rates: Union[float, List[float]] = None,
+        as_df: bool = False,
+    ) -> Any:
+        """Calculate repo rate, price or forward price for given bonds.
+
+        Args:
+            symbols: ISIN or name of bonds that should be valued.
+            keyfigures: Repo bond key figure that should be valued.
+            calc_date: date of calculation.
+            forward_date: future date of calculation.
+            prices: current price of bond.
+            forward_prices: future price of bond.
+            repo_rates: Repo rate of bond.
+            as_df: Default False. If True, the results are represented
+                as pandas DataFrame, else as dictionary
+
+
+        Returns:
+            Dictionary containing requested data. if as_df is True,
+                the data is in form of a DataFrame.
+        """
+        return self._retrieve_value(
+            BondRepoCalculator(
+                self._client,
+                symbols,
+                keyfigures,
+                calc_date,
+                forward_date,
+                prices,
+                forward_prices,
+                repo_rates,
+            ),
+            as_df,
+        )
+
     def get_fx_forecasts(
         self,
         currency_pair: str,
         as_df: bool = False,
     ) -> Any:
         """Retrieves Nordea's latest FX forecasts.
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/search_bond_names.py` & `nordea-analytics-1.9.0/src/nordea_analytics/search_bond_names.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,501 +1,501 @@
-from enum import Enum
-
-
-class AmortisationType(Enum):
-    """Amortisation Type available when searching for bonds."""
-
-    Annuity = "annuity"
-    Bullet = "bullet"
-    Irregular = "irregular"
-    Serial = "serial"
-
-
-class AssetType(Enum):
-    """Asset Types available when searching for bonds."""
-
-    BenchmarkBond = "Benchmark Bond"
-    DanishCappedFloaters = "Danish Capped Floater"
-    CreditBond = "credit bond"
-    DanishIndexBond = "Danish index bond"
-    DanishMortgageBond = "Danish mortgage bond"
-    FixToFloatBond = "Fix To Float Bond"
-    FRN = "FRN"
-    IndexLinkedBond = "Index Linked Bond"
-    NonCallableBond = "Non-callable Bond"
-
-
-class InstrumentGroup(Enum):
-    """Instrument Groups available when searching for bonds."""
-
-    CreditBonds = "Credit Bonds"
-    FloatingRateNotes = "FRNs"
-    GovernmentBonds = "Government Bonds"
-    DanishCallableMortgageBonds = "Danish Callable Mortgage Bonds"
-    DanishNonCallableMortgageBonds = "Danish Non-callable Mortgage Bonds"
-    FixedRateBonds = "Fixed Rate Bonds"
-    DanishIndexBonds = "Danish Index Bonds"
-
-
-class CapitalCentres(Enum):
-    """Capital centres available when searching for bonds."""
-
-    BRF_B = "B (BRF)"
-    BRF_E = "E (BRF)"
-    BRF_General = "GENERAL (BRF)"
-    DLR_B = "B (DLR)"
-    DLR_General = "GENERAL (DLR)"
-    NDA_1 = "1 (NDA)"
-    NDA_2 = "2 (NDA)"
-    NYK_C = "C (NYK)"
-    NYK_D = "D (NYK)"
-    NYK_E = "E (NYK)"
-    NYK_G = "G (NYK)"
-    NYK_General = "GENERAL (NYK)"
-    NYK_H = "H (NYK)"
-    NYK_I = "I (NYK)"
-    RD_General = "GENERAL (RD)"
-    RD_S = "S (RD)"
-    RD_T = "T (RD)"
-    TOT_C = "C (TOT)"
-
-
-class CapitalCentreTypes(Enum):
-    """Capital centre types available when searching for bonds."""
-
-    JCB = "JCB"
-    RO = "RO"
-    SDO = "SDO"
-    SDRO = "SDRO"
-
-
-class Issuers:
-    """Most common available issuers. Availability not limited to this list."""
-
-    Aareal_Bank_AG = "Aareal Bank AG"
-    Aareal_Beteiligungen_AG = "Aareal Beteiligungen AG"
-    Aareal_Hyp_AG = "Aareal Hyp AG"
-    ABB_International_Finance_Ltd = "ABB International Finance Ltd"
-    Abbey_National_Treasury_Services_London_Plc = (
-        "Abbey National Treasury Services (London) Plc"
-    )
-    Accor_SA = "Accor SA"
-    Achmea_Bank_NV = "Achmea Bank NV"
-    Adecco_Financial_Service_Ltd = "Adecco Financial Service Ltd"
-    Agbar_International_BV = "Agbar International BV"
-    ageas_Fin_NV = "ageas Fin NV"
-    Ahold_Finance_USA_LLC = "Ahold Finance USA LLC"
-    Air_Products_and_Chemicals_Inc = "Air Products and Chemicals Inc"
-    Akzo_Nobel_NV = "Akzo Nobel NV"
-    Alcatel_Lucent_SA = "Alcatel Lucent SA"
-    Allianz_SE = "Allianz SE"
-    Allied_Domecq_Financial_Services_Ltd = "Allied Domecq Financial Services Ltd"
-    Ally_Financial_Inc = "Ally Financial Inc"
-    Altria_Finance_Cayman_Islands_Ltd = "Altria Finance Cayman Islands Ltd"
-    Anglian_Water_Services_Financing_Plc = "Anglian Water Services Financing Plc"
-    ArcelorMittal_Finance = "ArcelorMittal Finance"
-    Asian_Development_Bank = "Asian Development Bank"
-    Assa_Abloy_AB = "Assa Abloy AB"
-    Assicurazioni_Generali_SpA = "Assicurazioni Generali SpA"
-    ATT_Corp = "AT&T Corp"
-    Australia = "Australia"
-    Australia_and_New_Zealand_Banking_Group_Ltd = (
-        "Australia and New Zealand Banking Group Ltd"
-    )
-    Austria = "Austria"
-    Autoliv_Inc_OLD = "Autoliv Inc (OLD)"
-    AXA_SA = "AXA SA"
-    Banco_Bilbao_Vizcaya_Argentaria_SA = "Banco Bilbao Vizcaya Argentaria SA"
-    Banco_Espanol_de_Credito_SA_Banesto = "Banco Español de Crédito SA (Banesto)"
-    Bank_1_Oslo_Akershus_AS = "Bank 1 Oslo Akershus AS"
-    Bank_fur_Arbeit_und_Wirtschaft_AG = "Bank für Arbeit und Wirtschaft AG"
-    Bank_Nederlandse_Gemeenten_NV = "Bank Nederlandse Gemeenten NV"
-    Bank_of_America_Corp = "Bank of America Corp"
-    Bank_of_Scotland_Plc = "Bank of Scotland Plc"
-    Bankinter_SA = "Bankinter SA"
-    Barclays_Bank_Plc = "Barclays Bank Plc"
-    BASF_SE = "BASF SE"
-    BAT_International_Finance_Plc = "BAT International Finance Plc"
-    Baxter_International_Inc = "Baxter International Inc"
-    Bayer_AG = "Bayer AG"
-    Bayerische_Landesbank = "Bayerische Landesbank"
-    Belgium = "Belgium"
-    Berlin_Hannover_Hypothekenbank_AG = "Berlin-Hannover Hypothekenbank AG"
-    Bezeq_Israeli_Telecommunication_Corp_Ltd = (
-        "Bezeq Israeli Telecommunication Corp Ltd"
-    )
-    BMW_Finance_NV = "BMW Finance NV"
-    BN_Bank_ASA = "BN Bank ASA"
-    Bolig_og_Naeringskreditt_AS = "Bolig og Næringskreditt AS"
-    Bombardier_Inc = "Bombardier Inc"
-    Bouygues_SA = "Bouygues SA"
-    BPB_Ltd = "BPB Ltd"
-    BPCE = "BPCE"
-    Bradford_and_Bingley_Plc = "Bradford & Bingley Plc"
-    Brazil = "Brazil"
-    Brisa_Finance_BV = "Brisa Finance BV"
-    British_Telecommunications_Plc = "British Telecommunications Plc"
-    Burmah_Castrol_Plc = "Burmah Castrol Plc"
-    Caisse_Centrale_du_Credit_Immobilier_de_France_SA = (
-        "Caisse Centrale du Credit Immobilier de France SA"
-    )
-    Caisse_dAmortissement_de_la_Dette_Sociale = (
-        "Caisse d'Amortissement de la Dette Sociale"
-    )
-    Caisse_Nationale_des_Autoroutes = "Caisse Nationale des Autoroutes"
-    Caixa_d_Estalvis_Catalunya_Tarragona_i_Manresa = (
-        "Caixa d Estalvis Catalunya Tarragona i Manresa"
-    )
-    Caja_de_Ahorros_y_Monte_de_Piedad_de_Madrid = (
-        "Caja de Ahorros y Monte de Piedad de Madrid"
-    )
-    Caja_de_Ahorros_y_Pensiones_de_Barcelona = (
-        "Caja de Ahorros y Pensiones de Barcelona"
-    )
-    Canada = "Canada"
-    Carrefour_SA = "Carrefour SA"
-    Casino_Guichard_Perrachon_SA = "Casino Guichard Perrachon SA"
-    Cie_Financiere_et_Industrielle_des_Autoroutes_SA = (
-        "Cie Financiere et Industrielle des Autoroutes SA"
-    )
-    CIF_Euromortgage_SA = "CIF Euromortgage SA"
-    CIFG_Assurn_North_America_Inc = "CIFG Assurn North America Inc"
-    CIT_Group_Inc = "CIT Group Inc"
-    Citigroup_Inc = "Citigroup Inc"
-    Clear_Channel_Communications_Inc = "Clear Channel Communications Inc"
-    CocaCola_HBC_Finance_BV = "Coca-Cola HBC Finance BV"
-    CocaCola_Refreshments_USA_Inc = "CocaCola Refreshments USA Inc"
-    Commerzbank_AG = "Commerzbank AG"
-    Compagnie_de_Financement_Foncier_SA = "Compagnie de Financement Foncier SA"
-    Compass_Group_Plc = "Compass Group Plc"
-    Continental_Rubber_of_America = "Continental Rubber of America"
-    Cooper_Industries_Finance_BV = "Cooper Industries Finance BV"
-    Corning_Inc = "Corning Inc"
-    Corus_Finance_Plc = "Corus Finance Plc"
-    Costa_Finance_SA = "Costa Finance SA"
-    Croatia = "Croatia"
-    Czech_Republic = "Czech Republic"
-    Danaher_Corp = "Danaher Corp"
-    Danmarks_Skibskreditfond = "Danmarks Skibskreditfond"
-    Danone_Finance_SA = "Danone Finance SA"
-    Dansk_Landbrugs_Realkreditfond_Kredit_AS = (
-        "Dansk Landbrugs Realkreditfond Kredit A/S"
-    )
-    Danske_Bank_AS = "Danske Bank A/S"
-    Danske_Hypotek_AB_Publ = "Danske Hypotek AB (Publ)"
-    Danske_Kredit_Realkreditaktieselskab = "Danske Kredit Realkreditaktieselskab"
-    DekaBank_Deutsche_Girozentrale = "DekaBank Deutsche Girozentrale"
-    Denmark = "Denmark"
-    Dentsply_International_Inc = "Dentsply International Inc"
-    Deutsche_Bahn_Finance_GmbH = "Deutsche Bahn Finance GmbH"
-    Deutsche_Bank_AG = "Deutsche Bank AG"
-    Deutsche_Genossenschafts_Hypothekenbank_AG = (
-        "Deutsche Genossenschafts-Hypothekenbank AG"
-    )
-    Deutsche_Hypothekenbank_AG = "Deutsche Hypothekenbank AG"
-    Deutsche_Pfandbriefbank_AG = "Deutsche Pfandbriefbank AG"
-    Deutsche_Postbank_AG = "Deutsche Postbank AG"
-    Deutsche_Telekom_International_Finance_BV = (
-        "Deutsche Telekom International Finance BV"
-    )
-    Development_Bank_of_Japan = "Development Bank of Japan"
-    Dexia_Credit_Local_SA = "Dexia Credit Local SA"
-    Dexia_Kommunalbank_Deutschland_AG = "Dexia Kommunalbank Deutschland AG"
-    Dexia_Municipal_Agency = "Dexia Municipal Agency"
-    Dow_Chemical_Co = "Dow Chemical Co"
-    Dresdner_Finance_BV = "Dresdner Finance BV"
-    Dusseldorfer_Hypothekenbank_AG = "Düsseldorfer Hypothekenbank AG"
-    EON_International_Finance_BV = "E.ON International Finance BV"
-    EON_UK_Plc = "E.ON UK Plc"
-    Ecolab_Inc = "Ecolab Inc"
-    Edison_SpA = "Edison SpA"
-    EDP_Energias_de_Portugal_SA = "EDP Energias de Portugal SA"
-    Eika_Boligkreditt_AS = "Eika Boligkreditt AS"
-    El_Paso_Corp = "El Paso Corp"
-    Electricite_de_France_SA = "Electricite de France SA"
-    Electrolux_AB = "Electrolux AB"
-    Elisa_Oyj = "Elisa Oyj"
-    EnBW_International_Finance_BV = "EnBW International Finance BV"
-    Endesa_SA = "Endesa SA"
-    Enel_SpA = "Enel SpA"
-    ENI_SpA = "ENI SpA"
-    Estonia = "Estonia"
-    Euro_Zone = "Euro Zone"
-    Eurohypo_AG = "Eurohypo AG"
-    Europaische_Hypothekenbank_SA_Luxembourg = (
-        "Europäische Hypothekenbank SA Luxembourg"
-    )
-    European_Investment_Bank = "European Investment Bank"
-    EVN_AG = "EVN AG"
-    Experian_Finance_Plc = "Experian Finance Plc"
-    Fannie_Mae_Federal_National_Mortgage_Association = (
-        "Fannie Mae (Federal National Mortgage Association)"
-    )
-    Faroe_Islands = "Faroe Islands"
-    Fiat_Chrysler_Finance_Europe_SA = "Fiat Chrysler Finance Europe SA"
-    FIH_Erhvervsbank = "FIH Erhvervsbank"
-    FIL_Ltd = "FIL Ltd"
-    Finland = "Finland"
-    FKI_Ltd = "FKI Ltd"
-    Fonterra_Cooperative_Group_Ltd = "Fonterra Cooperative Group Ltd"
-    Ford_Motor_Credit_Company_LLC = "Ford Motor Credit Company LLC"
-    France = "France"
-    France_Telecom_SA = "France Telecom SA"
-    Freddie_Mac_Federal_Home_Loan_Mortgage_Corp = (
-        "Freddie Mac (Federal Home Loan Mortgage Corp)"
-    )
-    Gallaher_Group_Ltd = "Gallaher Group Ltd"
-    Gas_Natural_Finance_BV = "Gas Natural Finance BV"
-    General_Electric_Capital_Corp = "General Electric Capital Corp"
-    Germany = "Germany"
-    GIE_PSA_Tresorerie = "GIE PSA Tresorerie"
-    Gillette_Co = "Gillette Co"
-    Goodyear_Tire_and_Rubber_Co = "Goodyear Tire & Rubber Co"
-    Greece = "Greece"
-    Halifax_Group_Euro_Finance_LP = "Halifax Group Euro Finance LP"
-    Hammerson_Plc = "Hammerson Plc"
-    HeidelbergCement_Finance_BV = "HeidelbergCement Finance BV"
-    Helaba_International_Finance_Plc = "Helaba International Finance Plc"
-    Helgeland_Boligkreditt_AS = "Helgeland Boligkreditt AS"
-    Hewlett_Packard_Enterprise_Co = "Hewlett Packard Enterprise Co"
-    HJ_Heinz_Co = "HJ Heinz Co"
-    HSBC_Finance_Corp = "HSBC Finance Corp"
-    HSH_N_Finance_Guernsey_Ltd = "HSH N Finance Guernsey Ltd"
-    Hungary = "Hungary"
-    Hutchison_Whampoa_Finance_CI_Ltd = "Hutchison Whampoa Finance (CI) Ltd"
-    Hypo_Alpe_Adria_Bank_International_AG = "Hypo Alpe-Adria-Bank International AG"
-    Hypo_Pfandbrief_Bank_International_SA = "Hypo Pfandbrief Bank International SA"
-    Hypo_Real_Estate_Bank_AG_Nurnberger_Hypothekenbank = (
-        "Hypo Real Estate Bank AG (Nürnberger Hypothekenbank)"
-    )
-    Hypo_Real_Estate_Bank_International_AG = "Hypo Real Estate Bank International AG"
-    Hypo_Tirol_Bank_AG = "Hypo Tirol Bank AG"
-    Iberdrola_International_BV = "Iberdrola International BV"
-    Imerys_SA = "Imerys SA"
-    Imperial_Brands_Finance_Plc = "Imperial Brands Finance Plc"
-    ING_Bank_NV = "ING Bank NV"
-    ING_Groep_NV = "ING Groep NV"
-    Innogy_Finance_BV = "Innogy Finance BV"
-    Innogy_Plc = "Innogy Plc"
-    Instituto_de_Credito_Oficial = "Instituto de Credito Oficial"
-    Inter_American_Development_Bank = "Inter-American Development Bank"
-    International_Bank_for_Reconstruction_and_Development = (
-        "International Bank for Reconstruction and Development"
-    )
-    International_Business_Machines_Corp = "International Business Machines Corp"
-    International_Lease_Finance_Corp = "International Lease Finance Corp"
-    Invensys_Plc = "Invensys Plc"
-    Investor_AB = "Investor AB"
-    Ireland = "Ireland"
-    Italy = "Italy"
-    J_Sainsbury_Plc = "J Sainsbury Plc"
-    Japan = "Japan"
-    JP_Morgan_Chase_and_Co = "JP Morgan Chase & Co"
-    Jyske_Realkredit_AS = "Jyske Realkredit A/S"
-    KBC_Internationale_Financieringsmaatschappij_NV = (
-        "KBC Internationale Financieringsmaatschappij NV"
-    )
-    Kelda_Group_Ltd = "Kelda Group Ltd"
-    Klepierre = "Klepierre"
-    Kommunalbanken_AS = "Kommunalbanken AS"
-    Kommunekredit_AS = "Kommunekredit AS"
-    Kongeriget_Danmarks_Fiskeribank = "Kongeriget Danmarks Fiskeribank"
-    Koninklijke_DSM_NV = "Koninklijke DSM NV"
-    Koninklijke_KPN_NV = "Koninklijke KPN NV"
-    Koninklijke_Philips_NV = "Koninklijke Philips NV"
-    Kreditanstalt_fur_Wiederaufbau = "Kreditanstalt für Wiederaufbau"
-    Ladbrokes_Group_Finance_Plc = "Ladbrokes Group Finance Plc"
-    Lafarge_SA = "Lafarge SA"
-    Landesbank_Baden_Wuerttemberg = "Landesbank Baden Wuerttemberg"
-    Landesbank_Berlin_AG = "Landesbank Berlin AG"
-    Landesbank_Schleswig_Holstein_Girozentrale = (
-        "Landesbank Schleswig-Holstein Girozentrale"
-    )
-    Landmark_Mortgages_Ltd = "Landmark Mortgages Ltd"
-    Landshypotek_Bank_AB_publ = "Landshypotek Bank AB (publ)"
-    Landwirtschaftliche_Rentenbank = "Landwirtschaftliche Rentenbank"
-    Lansforsakringar_Hypotek_AB_publ = "Lansforsakringar Hypotek AB (publ)"
-    Latvia = "Latvia"
-    Lehman_Brothers_Holdings_Inc = "Lehman Brothers Holdings Inc"
-    Linde_Finance_BV = "Linde Finance BV"
-    Lithuania = "Lithuania"
-    Liz_Claiborne_Inc = "Liz Claiborne Inc"
-    LR_Realkredit_Landsbankernes_Reallanefond_AS = (
-        "LR Realkredit (Landsbankernes Reallånefond) A/S"
-    )
-    Marks_and_Spencer_Plc = "Marks & Spencer Plc"
-    MBNA_Europe_Funding_Plc = "MBNA Europe Funding Plc"
-    McDonalds_Corp = "McDonald's Corp"
-    Merrill_Lynch__Inc = "Merrill Lynch  Inc"
-    Metallgesellschaft_Finance = "Metallgesellschaft Finance"
-    Metro_AG = "Metro AG"
-    Metsa_Board_Oyj = "Metsa Board Oyj"
-    Metso_Oyj = "Metso Oyj"
-    Mexico = "Mexico"
-    Michelin_Luxembourg_SCS = "Michelin Luxembourg SCS"
-    mmO2_Plc = "mmO2 Plc"
-    Morgan_Guaranty_Trust_Co_of_New_York = "Morgan Guaranty Trust Co of New York"
-    Morgan_Stanley = "Morgan Stanley"
-    Munchener_Hypothekenbank_eG = "Münchener Hypothekenbank eG"
-    National_Grid_Gas_Plc = "National Grid Gas Plc"
-    National_Rural_Utilities_Cooperative_Finance_Corp = (
-        "National Rural Utilities Cooperative Finance Corp"
-    )
-    Nederlandse_Waterschapsbank_NV = "Nederlandse Waterschapsbank NV"
-    Nestle_SA = "Nestle SA"
-    Netherlands = "Netherlands"
-    New_Zealand = "New Zealand"
-    Nippon_Telegraph_and_Telephone_Corp = "Nippon Telegraph & Telephone Corp"
-    Norddeutsche_Landesbank_Girozentrale = "Norddeutsche Landesbank Girozentrale"
-    Nordea_Nordbanken_Hypotek_AB = "Nordea (Nordbanken) Hypotek AB"
-    Nordea_Bank_Abp = "Nordea Bank Abp"
-    Nordea_Bank_Danmark_AS = "Nordea Bank Danmark A/S"
-    Nordea_Bank_Finland_ABP = "Nordea Bank Finland ABP"
-    Nordea_Bank_Norge_ASA = "Nordea Bank Norge ASA"
-    Nordea_Bank_Sweden_AB = "Nordea Bank Sweden AB"
-    Nordea_Eiendomskreditt_AS = "Nordea Eiendomskreditt AS"
-    Nordea_Funds_Oy = "Nordea Funds Oy"
-    Nordea_Hypotek_AB = "Nordea Hypotek AB"
-    Nordea_Hypoteksbank_Abp = "Nordea Hypoteksbank Abp"
-    Nordea_Kredit_Realkreditaktieselskab = "Nordea Kredit Realkreditaktieselskab"
-    Nordea_Mortgage_Bank_Plc = "Nordea Mortgage Bank Plc"
-    Norsk_Hydro_ASA = "Norsk Hydro ASA"
-    Norway = "Norway"
-    Novartis_Securities_Investment_Ltd = "Novartis Securities Investment Ltd"
-    Nykredit_Realkredit_AS = "Nykredit Realkredit A/S"
-    Oesterreichische_Kontrollbank_AG = "Oesterreichische Kontrollbank AG"
-    OP_Mortgage_Bank = "OP Mortgage Bank"
-    OTE_Plc = "OTE Plc"
-    Parker_Hannifin_Corp = "Parker Hannifin Corp"
-    Pearson_Funding_Five_Plc = "Pearson Funding Five Plc"
-    Pemex_Project_Funding_Master_Trust = "Pemex Project Funding Master Trust"
-    Petronas_Capital_Ltd = "Petronas Capital Ltd"
-    Pfandbriefstelle_der_Oesterreichischen_Landes_Hypothekenbanken = (
-        "Pfandbriefstelle der Oesterreichischen Landes-Hypothekenbanken"
-    )
-    Pilkington_Group_Ltd = "Pilkington Group Ltd"
-    Pirelli_SpA = "Pirelli SpA"
-    Poland = "Poland"
-    Portugal = "Portugal"
-    Portugal_Telecom_International_Finance_BV = (
-        "Portugal Telecom International Finance BV"
-    )
-    PostNL_NV = "PostNL NV"
-    Procter_and_Gamble_Co = "Procter & Gamble Co"
-    Promodes_SA = "Promodes SA"
-    ProSieben_SAT_1_Media_AG = "ProSieben SAT.1 Media AG"
-    Public_Power_Corp_SA = "Public Power Corp SA"
-    Publishing_and_Broadcasting_Finance_Ltd = "Publishing and Broadcasting Finance Ltd"
-    Quebec_Province_of = "Quebec (Province of)"
-    Rabobank_Nederland_NV = "Rabobank Nederland NV"
-    Realkredit_Danmark_AS = "Realkredit Danmark A/S"
-    Reed_Elsevier_Capital_Inc = "Reed Elsevier Capital Inc"
-    Renault_SA = "Renault SA"
-    Rentokil_Initial_1927_Plc = "Rentokil Initial 1927 Plc"
-    Repsol_International_Finance_BV = "Repsol International Finance BV"
-    Reseau_Ferre_de_France = "Reseau Ferre de France"
-    Residential_Capital_LLC = "Residential Capital LLC"
-    Rexam_Plc = "Rexam Plc"
-    Rheinland_Pfalz_Bank = "Rheinland-Pfalz Bank"
-    Rheinmetall_AG = "Rheinmetall AG"
-    Rhodia_SA = "Rhodia SA"
-    Rio_Tinto_Finance_Plc = "Rio Tinto Finance Plc"
-    Rohm_og_Haas_Denmark_AS = "Rohm & Haas Denmark A/S"
-    Rolls_Royce_Plc = "Rolls-Royce Plc"
-    Royal_Bank_of_Scotland_NV = "Royal Bank of Scotland NV"
-    Russia = "Russia"
-    Sachsen_Bank = "Sachsen Bank"
-    Saint_Gobain_Nederland_BV = "Saint Gobain Nederland BV"
-    Sampo_Housing_Loan_Bank_Plc = "Sampo Housing Loan Bank Plc"
-    SANOFI = "SANOFI"
-    Santander_UK_Plc = "Santander UK Plc"
-    Sara_Lee_Corp = "Sara Lee Corp"
-    Scandinavian_Airlines_System_AB = "Scandinavian Airlines System AB"
-    Scania_AB = "Scania AB"
-    Schlumberger_SA = "Schlumberger SA"
-    Schneider_Electric_SE = "Schneider Electric SE"
-    SEB_AG = "SEB AG"
-    Securitas_AB = "Securitas AB"
-    Siemens_Financieringsmaatschappij_NV = "Siemens Financieringsmaatschappij NV"
-    Singapore_Telecommunications_Ltd = "Singapore Telecommunications Ltd"
-    SingTel_Optus_Finance_Pty_Ltd = "SingTel Optus Finance Pty Ltd"
-    Skandinaviska_Enskilda_Banken_BoLan_AB = "Skandinaviska Enskilda Banken BoLån AB"
-    Slovakia = "Slovakia"
-    Slovenia = "Slovenia"
-    SNCF_Mobilites_EPIC = "SNCF Mobilites EPIC"
-    SNS_Bank_NV = "SNS Bank NV"
-    SODEXO = "SODEXO"
-    Sol_Melia_Europe_BV = "Sol Melia Europe BV"
-    Solvay_SA = "Solvay SA"
-    South_Africa = "South Africa"
-    Spain = "Spain"
-    Sparebanken_Sor = "Sparebanken Sør"
-    Sparebanken_Vest_Boligkreditt_AS = "Sparebanken Vest Boligkreditt AS"
-    Sparebankenes_Kredittselskap_AS = "Sparebankenes Kredittselskap A/S"
-    Sparkasse_KoelnBonn = "Sparkasse KoelnBonn"
-    Stadshypotek_AB = "Stadshypotek AB"
-    Stagecoach_Group_Plc = "Stagecoach Group Plc"
-    State_of_Saxony_Anhalt = "State of Saxony-Anhalt"
-    Statkraft_AS = "Statkraft AS"
-    Statoil_ASA = "Statoil ASA"
-    Stora_Enso_Oyj = "Stora Enso Oyj"
-    Sudzucker_International_Finance_BV = "Südzucker International Finance BV"
-    Sveriges_Bostadsfinansieringsaktiebolag = "Sveriges Bostadsfinansieringsaktiebolag"
-    Swedbank_Hypotek_AB = "Swedbank Hypotek AB"
-    Sweden = "Sweden"
-    Swedish_Covered_Bond_Corp = "Swedish Covered Bond Corp"
-    Swedish_Match_AB = "Swedish Match AB"
-    Switzerland = "Switzerland"
-    Syngenta_Luxembourg_Finance_SA = "Syngenta Luxembourg Finance SA"
-    TCNZ = "TCNZ"
-    TDC_AS = "TDC A/S"
-    Technicolor = "Technicolor"
-    Telecom_Italia_Finance_Sogerim_SA = "Telecom Italia Finance (Sogerim) SA"
-    Telecom_Italia_Finance_SA = "Telecom Italia Finance SA"
-    Telefonaktiebolaget_LM_Ericsson = "Telefonaktiebolaget LM Ericsson"
-    Telefonica_SA = "Telefonica SA"
-    Telenor_ASA = "Telenor ASA"
-    Telia_Company_AB = "Telia Company AB"
-    TeliaSonera_Finland_Oyj = "TeliaSonera Finland Oyj"
-    Telstra_Corporation_Ltd = "Telstra Corporation Ltd"
-    Tesco_Plc = "Tesco Plc"
-    Textron_Inc = "Textron Inc"
-    The_Nielsen_Co = "The Nielsen Co"
-    ThyssenKrupp_Finance_Nederland_BV = "ThyssenKrupp Finance Nederland BV"
-    TI_Group_Ltd = "TI Group Ltd"
-    Tokyo_Electric_Power_Co_Inc = "Tokyo Electric Power Co Inc"
-    Total_SA = "Total SA"
-    Totalkredit_AS = "Totalkredit A/S"
-    Toyota_Motor_Credit_Corp = "Toyota Motor Credit Corp"
-    Toys_R_Us_Inc = "Toys R Us Inc"
-    TPSA_Eurofinance_BV = "TPSA Eurofinance BV"
-    Turkey = "Turkey"
-    Tyco_International_Group_SA = "Tyco International Group SA"
-    Unibail = "Unibail"
-    UniCredit_Bank_AG = "UniCredit Bank AG"
-    UniCredit_Bank_Austria_AG = "UniCredit Bank Austria AG"
-    Unilever_NV = "Unilever NV"
-    United_Kingdom = "United Kingdom"
-    United_States = "United States"
-    United_Utilities_Water_Plc = "United Utilities Water Plc"
-    UPM_Kymmene_Oyj = "UPM-Kymmene Oyj"
-    Valeo_SA = "Valeo SA"
-    Vattenfall_Treasury_AB = "Vattenfall Treasury AB"
-    Vauban_Mobilisation_Garanties_SA = "Vauban Mobilisation Garanties SA"
-    Veolia_Environnement = "Veolia Environnement"
-    Vodafone_Finance_BV = "Vodafone Finance BV"
-    Voith_GmbH = "Voith GmbH"
-    Volvo_Treasury_AB = "Volvo Treasury AB"
-    Vorarlberger_Landes_und_Hypothekenbank_AG = (
-        "Vorarlberger Landes- und Hypothekenbank AG"
-    )
-    VW_Financial_Services_AG = "VW Financial Services AG"
-    Westfaelische_Landschaft_Bodenkreditbank_AG = (
-        "Westfaelische Landschaft Bodenkreditbank AG"
-    )
-    WestLB_AG = "WestLB AG"
-    Whirlpool_Corp = "Whirlpool Corp"
-    Wolters_Kluwer_NV = "Wolters Kluwer NV"
-    WPP_Plc = "WPP Plc"
-    Wurth_Finance_International_BV = "Würth Finance International BV"
-    Xerox_Corp = "Xerox Corp"
-    Yorkshire_Building_Society = "Yorkshire Building Society"
+from enum import Enum
+
+
+class AmortisationType(Enum):
+    """Amortisation Type available when searching for bonds."""
+
+    Annuity = "annuity"
+    Bullet = "bullet"
+    Irregular = "irregular"
+    Serial = "serial"
+
+
+class AssetType(Enum):
+    """Asset Types available when searching for bonds."""
+
+    BenchmarkBond = "Benchmark Bond"
+    DanishCappedFloaters = "Danish Capped Floater"
+    CreditBond = "credit bond"
+    DanishIndexBond = "Danish index bond"
+    DanishMortgageBond = "Danish mortgage bond"
+    FixToFloatBond = "Fix To Float Bond"
+    FRN = "FRN"
+    IndexLinkedBond = "Index Linked Bond"
+    NonCallableBond = "Non-callable Bond"
+
+
+class InstrumentGroup(Enum):
+    """Instrument Groups available when searching for bonds."""
+
+    CreditBonds = "Credit Bonds"
+    FloatingRateNotes = "FRNs"
+    GovernmentBonds = "Government Bonds"
+    DanishCallableMortgageBonds = "Danish Callable Mortgage Bonds"
+    DanishNonCallableMortgageBonds = "Danish Non-callable Mortgage Bonds"
+    FixedRateBonds = "Fixed Rate Bonds"
+    DanishIndexBonds = "Danish Index Bonds"
+
+
+class CapitalCentres(Enum):
+    """Capital centres available when searching for bonds."""
+
+    BRF_B = "B (BRF)"
+    BRF_E = "E (BRF)"
+    BRF_General = "GENERAL (BRF)"
+    DLR_B = "B (DLR)"
+    DLR_General = "GENERAL (DLR)"
+    NDA_1 = "1 (NDA)"
+    NDA_2 = "2 (NDA)"
+    NYK_C = "C (NYK)"
+    NYK_D = "D (NYK)"
+    NYK_E = "E (NYK)"
+    NYK_G = "G (NYK)"
+    NYK_General = "GENERAL (NYK)"
+    NYK_H = "H (NYK)"
+    NYK_I = "I (NYK)"
+    RD_General = "GENERAL (RD)"
+    RD_S = "S (RD)"
+    RD_T = "T (RD)"
+    TOT_C = "C (TOT)"
+
+
+class CapitalCentreTypes(Enum):
+    """Capital centre types available when searching for bonds."""
+
+    JCB = "JCB"
+    RO = "RO"
+    SDO = "SDO"
+    SDRO = "SDRO"
+
+
+class Issuers:
+    """Most common available issuers. Availability not limited to this list."""
+
+    Aareal_Bank_AG = "Aareal Bank AG"
+    Aareal_Beteiligungen_AG = "Aareal Beteiligungen AG"
+    Aareal_Hyp_AG = "Aareal Hyp AG"
+    ABB_International_Finance_Ltd = "ABB International Finance Ltd"
+    Abbey_National_Treasury_Services_London_Plc = (
+        "Abbey National Treasury Services (London) Plc"
+    )
+    Accor_SA = "Accor SA"
+    Achmea_Bank_NV = "Achmea Bank NV"
+    Adecco_Financial_Service_Ltd = "Adecco Financial Service Ltd"
+    Agbar_International_BV = "Agbar International BV"
+    ageas_Fin_NV = "ageas Fin NV"
+    Ahold_Finance_USA_LLC = "Ahold Finance USA LLC"
+    Air_Products_and_Chemicals_Inc = "Air Products and Chemicals Inc"
+    Akzo_Nobel_NV = "Akzo Nobel NV"
+    Alcatel_Lucent_SA = "Alcatel Lucent SA"
+    Allianz_SE = "Allianz SE"
+    Allied_Domecq_Financial_Services_Ltd = "Allied Domecq Financial Services Ltd"
+    Ally_Financial_Inc = "Ally Financial Inc"
+    Altria_Finance_Cayman_Islands_Ltd = "Altria Finance Cayman Islands Ltd"
+    Anglian_Water_Services_Financing_Plc = "Anglian Water Services Financing Plc"
+    ArcelorMittal_Finance = "ArcelorMittal Finance"
+    Asian_Development_Bank = "Asian Development Bank"
+    Assa_Abloy_AB = "Assa Abloy AB"
+    Assicurazioni_Generali_SpA = "Assicurazioni Generali SpA"
+    ATT_Corp = "AT&T Corp"
+    Australia = "Australia"
+    Australia_and_New_Zealand_Banking_Group_Ltd = (
+        "Australia and New Zealand Banking Group Ltd"
+    )
+    Austria = "Austria"
+    Autoliv_Inc_OLD = "Autoliv Inc (OLD)"
+    AXA_SA = "AXA SA"
+    Banco_Bilbao_Vizcaya_Argentaria_SA = "Banco Bilbao Vizcaya Argentaria SA"
+    Banco_Espanol_de_Credito_SA_Banesto = "Banco Español de Crédito SA (Banesto)"
+    Bank_1_Oslo_Akershus_AS = "Bank 1 Oslo Akershus AS"
+    Bank_fur_Arbeit_und_Wirtschaft_AG = "Bank für Arbeit und Wirtschaft AG"
+    Bank_Nederlandse_Gemeenten_NV = "Bank Nederlandse Gemeenten NV"
+    Bank_of_America_Corp = "Bank of America Corp"
+    Bank_of_Scotland_Plc = "Bank of Scotland Plc"
+    Bankinter_SA = "Bankinter SA"
+    Barclays_Bank_Plc = "Barclays Bank Plc"
+    BASF_SE = "BASF SE"
+    BAT_International_Finance_Plc = "BAT International Finance Plc"
+    Baxter_International_Inc = "Baxter International Inc"
+    Bayer_AG = "Bayer AG"
+    Bayerische_Landesbank = "Bayerische Landesbank"
+    Belgium = "Belgium"
+    Berlin_Hannover_Hypothekenbank_AG = "Berlin-Hannover Hypothekenbank AG"
+    Bezeq_Israeli_Telecommunication_Corp_Ltd = (
+        "Bezeq Israeli Telecommunication Corp Ltd"
+    )
+    BMW_Finance_NV = "BMW Finance NV"
+    BN_Bank_ASA = "BN Bank ASA"
+    Bolig_og_Naeringskreditt_AS = "Bolig og Næringskreditt AS"
+    Bombardier_Inc = "Bombardier Inc"
+    Bouygues_SA = "Bouygues SA"
+    BPB_Ltd = "BPB Ltd"
+    BPCE = "BPCE"
+    Bradford_and_Bingley_Plc = "Bradford & Bingley Plc"
+    Brazil = "Brazil"
+    Brisa_Finance_BV = "Brisa Finance BV"
+    British_Telecommunications_Plc = "British Telecommunications Plc"
+    Burmah_Castrol_Plc = "Burmah Castrol Plc"
+    Caisse_Centrale_du_Credit_Immobilier_de_France_SA = (
+        "Caisse Centrale du Credit Immobilier de France SA"
+    )
+    Caisse_dAmortissement_de_la_Dette_Sociale = (
+        "Caisse d'Amortissement de la Dette Sociale"
+    )
+    Caisse_Nationale_des_Autoroutes = "Caisse Nationale des Autoroutes"
+    Caixa_d_Estalvis_Catalunya_Tarragona_i_Manresa = (
+        "Caixa d Estalvis Catalunya Tarragona i Manresa"
+    )
+    Caja_de_Ahorros_y_Monte_de_Piedad_de_Madrid = (
+        "Caja de Ahorros y Monte de Piedad de Madrid"
+    )
+    Caja_de_Ahorros_y_Pensiones_de_Barcelona = (
+        "Caja de Ahorros y Pensiones de Barcelona"
+    )
+    Canada = "Canada"
+    Carrefour_SA = "Carrefour SA"
+    Casino_Guichard_Perrachon_SA = "Casino Guichard Perrachon SA"
+    Cie_Financiere_et_Industrielle_des_Autoroutes_SA = (
+        "Cie Financiere et Industrielle des Autoroutes SA"
+    )
+    CIF_Euromortgage_SA = "CIF Euromortgage SA"
+    CIFG_Assurn_North_America_Inc = "CIFG Assurn North America Inc"
+    CIT_Group_Inc = "CIT Group Inc"
+    Citigroup_Inc = "Citigroup Inc"
+    Clear_Channel_Communications_Inc = "Clear Channel Communications Inc"
+    CocaCola_HBC_Finance_BV = "Coca-Cola HBC Finance BV"
+    CocaCola_Refreshments_USA_Inc = "CocaCola Refreshments USA Inc"
+    Commerzbank_AG = "Commerzbank AG"
+    Compagnie_de_Financement_Foncier_SA = "Compagnie de Financement Foncier SA"
+    Compass_Group_Plc = "Compass Group Plc"
+    Continental_Rubber_of_America = "Continental Rubber of America"
+    Cooper_Industries_Finance_BV = "Cooper Industries Finance BV"
+    Corning_Inc = "Corning Inc"
+    Corus_Finance_Plc = "Corus Finance Plc"
+    Costa_Finance_SA = "Costa Finance SA"
+    Croatia = "Croatia"
+    Czech_Republic = "Czech Republic"
+    Danaher_Corp = "Danaher Corp"
+    Danmarks_Skibskreditfond = "Danmarks Skibskreditfond"
+    Danone_Finance_SA = "Danone Finance SA"
+    Dansk_Landbrugs_Realkreditfond_Kredit_AS = (
+        "Dansk Landbrugs Realkreditfond Kredit A/S"
+    )
+    Danske_Bank_AS = "Danske Bank A/S"
+    Danske_Hypotek_AB_Publ = "Danske Hypotek AB (Publ)"
+    Danske_Kredit_Realkreditaktieselskab = "Danske Kredit Realkreditaktieselskab"
+    DekaBank_Deutsche_Girozentrale = "DekaBank Deutsche Girozentrale"
+    Denmark = "Denmark"
+    Dentsply_International_Inc = "Dentsply International Inc"
+    Deutsche_Bahn_Finance_GmbH = "Deutsche Bahn Finance GmbH"
+    Deutsche_Bank_AG = "Deutsche Bank AG"
+    Deutsche_Genossenschafts_Hypothekenbank_AG = (
+        "Deutsche Genossenschafts-Hypothekenbank AG"
+    )
+    Deutsche_Hypothekenbank_AG = "Deutsche Hypothekenbank AG"
+    Deutsche_Pfandbriefbank_AG = "Deutsche Pfandbriefbank AG"
+    Deutsche_Postbank_AG = "Deutsche Postbank AG"
+    Deutsche_Telekom_International_Finance_BV = (
+        "Deutsche Telekom International Finance BV"
+    )
+    Development_Bank_of_Japan = "Development Bank of Japan"
+    Dexia_Credit_Local_SA = "Dexia Credit Local SA"
+    Dexia_Kommunalbank_Deutschland_AG = "Dexia Kommunalbank Deutschland AG"
+    Dexia_Municipal_Agency = "Dexia Municipal Agency"
+    Dow_Chemical_Co = "Dow Chemical Co"
+    Dresdner_Finance_BV = "Dresdner Finance BV"
+    Dusseldorfer_Hypothekenbank_AG = "Düsseldorfer Hypothekenbank AG"
+    EON_International_Finance_BV = "E.ON International Finance BV"
+    EON_UK_Plc = "E.ON UK Plc"
+    Ecolab_Inc = "Ecolab Inc"
+    Edison_SpA = "Edison SpA"
+    EDP_Energias_de_Portugal_SA = "EDP Energias de Portugal SA"
+    Eika_Boligkreditt_AS = "Eika Boligkreditt AS"
+    El_Paso_Corp = "El Paso Corp"
+    Electricite_de_France_SA = "Electricite de France SA"
+    Electrolux_AB = "Electrolux AB"
+    Elisa_Oyj = "Elisa Oyj"
+    EnBW_International_Finance_BV = "EnBW International Finance BV"
+    Endesa_SA = "Endesa SA"
+    Enel_SpA = "Enel SpA"
+    ENI_SpA = "ENI SpA"
+    Estonia = "Estonia"
+    Euro_Zone = "Euro Zone"
+    Eurohypo_AG = "Eurohypo AG"
+    Europaische_Hypothekenbank_SA_Luxembourg = (
+        "Europäische Hypothekenbank SA Luxembourg"
+    )
+    European_Investment_Bank = "European Investment Bank"
+    EVN_AG = "EVN AG"
+    Experian_Finance_Plc = "Experian Finance Plc"
+    Fannie_Mae_Federal_National_Mortgage_Association = (
+        "Fannie Mae (Federal National Mortgage Association)"
+    )
+    Faroe_Islands = "Faroe Islands"
+    Fiat_Chrysler_Finance_Europe_SA = "Fiat Chrysler Finance Europe SA"
+    FIH_Erhvervsbank = "FIH Erhvervsbank"
+    FIL_Ltd = "FIL Ltd"
+    Finland = "Finland"
+    FKI_Ltd = "FKI Ltd"
+    Fonterra_Cooperative_Group_Ltd = "Fonterra Cooperative Group Ltd"
+    Ford_Motor_Credit_Company_LLC = "Ford Motor Credit Company LLC"
+    France = "France"
+    France_Telecom_SA = "France Telecom SA"
+    Freddie_Mac_Federal_Home_Loan_Mortgage_Corp = (
+        "Freddie Mac (Federal Home Loan Mortgage Corp)"
+    )
+    Gallaher_Group_Ltd = "Gallaher Group Ltd"
+    Gas_Natural_Finance_BV = "Gas Natural Finance BV"
+    General_Electric_Capital_Corp = "General Electric Capital Corp"
+    Germany = "Germany"
+    GIE_PSA_Tresorerie = "GIE PSA Tresorerie"
+    Gillette_Co = "Gillette Co"
+    Goodyear_Tire_and_Rubber_Co = "Goodyear Tire & Rubber Co"
+    Greece = "Greece"
+    Halifax_Group_Euro_Finance_LP = "Halifax Group Euro Finance LP"
+    Hammerson_Plc = "Hammerson Plc"
+    HeidelbergCement_Finance_BV = "HeidelbergCement Finance BV"
+    Helaba_International_Finance_Plc = "Helaba International Finance Plc"
+    Helgeland_Boligkreditt_AS = "Helgeland Boligkreditt AS"
+    Hewlett_Packard_Enterprise_Co = "Hewlett Packard Enterprise Co"
+    HJ_Heinz_Co = "HJ Heinz Co"
+    HSBC_Finance_Corp = "HSBC Finance Corp"
+    HSH_N_Finance_Guernsey_Ltd = "HSH N Finance Guernsey Ltd"
+    Hungary = "Hungary"
+    Hutchison_Whampoa_Finance_CI_Ltd = "Hutchison Whampoa Finance (CI) Ltd"
+    Hypo_Alpe_Adria_Bank_International_AG = "Hypo Alpe-Adria-Bank International AG"
+    Hypo_Pfandbrief_Bank_International_SA = "Hypo Pfandbrief Bank International SA"
+    Hypo_Real_Estate_Bank_AG_Nurnberger_Hypothekenbank = (
+        "Hypo Real Estate Bank AG (Nürnberger Hypothekenbank)"
+    )
+    Hypo_Real_Estate_Bank_International_AG = "Hypo Real Estate Bank International AG"
+    Hypo_Tirol_Bank_AG = "Hypo Tirol Bank AG"
+    Iberdrola_International_BV = "Iberdrola International BV"
+    Imerys_SA = "Imerys SA"
+    Imperial_Brands_Finance_Plc = "Imperial Brands Finance Plc"
+    ING_Bank_NV = "ING Bank NV"
+    ING_Groep_NV = "ING Groep NV"
+    Innogy_Finance_BV = "Innogy Finance BV"
+    Innogy_Plc = "Innogy Plc"
+    Instituto_de_Credito_Oficial = "Instituto de Credito Oficial"
+    Inter_American_Development_Bank = "Inter-American Development Bank"
+    International_Bank_for_Reconstruction_and_Development = (
+        "International Bank for Reconstruction and Development"
+    )
+    International_Business_Machines_Corp = "International Business Machines Corp"
+    International_Lease_Finance_Corp = "International Lease Finance Corp"
+    Invensys_Plc = "Invensys Plc"
+    Investor_AB = "Investor AB"
+    Ireland = "Ireland"
+    Italy = "Italy"
+    J_Sainsbury_Plc = "J Sainsbury Plc"
+    Japan = "Japan"
+    JP_Morgan_Chase_and_Co = "JP Morgan Chase & Co"
+    Jyske_Realkredit_AS = "Jyske Realkredit A/S"
+    KBC_Internationale_Financieringsmaatschappij_NV = (
+        "KBC Internationale Financieringsmaatschappij NV"
+    )
+    Kelda_Group_Ltd = "Kelda Group Ltd"
+    Klepierre = "Klepierre"
+    Kommunalbanken_AS = "Kommunalbanken AS"
+    Kommunekredit_AS = "Kommunekredit AS"
+    Kongeriget_Danmarks_Fiskeribank = "Kongeriget Danmarks Fiskeribank"
+    Koninklijke_DSM_NV = "Koninklijke DSM NV"
+    Koninklijke_KPN_NV = "Koninklijke KPN NV"
+    Koninklijke_Philips_NV = "Koninklijke Philips NV"
+    Kreditanstalt_fur_Wiederaufbau = "Kreditanstalt für Wiederaufbau"
+    Ladbrokes_Group_Finance_Plc = "Ladbrokes Group Finance Plc"
+    Lafarge_SA = "Lafarge SA"
+    Landesbank_Baden_Wuerttemberg = "Landesbank Baden Wuerttemberg"
+    Landesbank_Berlin_AG = "Landesbank Berlin AG"
+    Landesbank_Schleswig_Holstein_Girozentrale = (
+        "Landesbank Schleswig-Holstein Girozentrale"
+    )
+    Landmark_Mortgages_Ltd = "Landmark Mortgages Ltd"
+    Landshypotek_Bank_AB_publ = "Landshypotek Bank AB (publ)"
+    Landwirtschaftliche_Rentenbank = "Landwirtschaftliche Rentenbank"
+    Lansforsakringar_Hypotek_AB_publ = "Lansforsakringar Hypotek AB (publ)"
+    Latvia = "Latvia"
+    Lehman_Brothers_Holdings_Inc = "Lehman Brothers Holdings Inc"
+    Linde_Finance_BV = "Linde Finance BV"
+    Lithuania = "Lithuania"
+    Liz_Claiborne_Inc = "Liz Claiborne Inc"
+    LR_Realkredit_Landsbankernes_Reallanefond_AS = (
+        "LR Realkredit (Landsbankernes Reallånefond) A/S"
+    )
+    Marks_and_Spencer_Plc = "Marks & Spencer Plc"
+    MBNA_Europe_Funding_Plc = "MBNA Europe Funding Plc"
+    McDonalds_Corp = "McDonald's Corp"
+    Merrill_Lynch__Inc = "Merrill Lynch  Inc"
+    Metallgesellschaft_Finance = "Metallgesellschaft Finance"
+    Metro_AG = "Metro AG"
+    Metsa_Board_Oyj = "Metsa Board Oyj"
+    Metso_Oyj = "Metso Oyj"
+    Mexico = "Mexico"
+    Michelin_Luxembourg_SCS = "Michelin Luxembourg SCS"
+    mmO2_Plc = "mmO2 Plc"
+    Morgan_Guaranty_Trust_Co_of_New_York = "Morgan Guaranty Trust Co of New York"
+    Morgan_Stanley = "Morgan Stanley"
+    Munchener_Hypothekenbank_eG = "Münchener Hypothekenbank eG"
+    National_Grid_Gas_Plc = "National Grid Gas Plc"
+    National_Rural_Utilities_Cooperative_Finance_Corp = (
+        "National Rural Utilities Cooperative Finance Corp"
+    )
+    Nederlandse_Waterschapsbank_NV = "Nederlandse Waterschapsbank NV"
+    Nestle_SA = "Nestle SA"
+    Netherlands = "Netherlands"
+    New_Zealand = "New Zealand"
+    Nippon_Telegraph_and_Telephone_Corp = "Nippon Telegraph & Telephone Corp"
+    Norddeutsche_Landesbank_Girozentrale = "Norddeutsche Landesbank Girozentrale"
+    Nordea_Nordbanken_Hypotek_AB = "Nordea (Nordbanken) Hypotek AB"
+    Nordea_Bank_Abp = "Nordea Bank Abp"
+    Nordea_Bank_Danmark_AS = "Nordea Bank Danmark A/S"
+    Nordea_Bank_Finland_ABP = "Nordea Bank Finland ABP"
+    Nordea_Bank_Norge_ASA = "Nordea Bank Norge ASA"
+    Nordea_Bank_Sweden_AB = "Nordea Bank Sweden AB"
+    Nordea_Eiendomskreditt_AS = "Nordea Eiendomskreditt AS"
+    Nordea_Funds_Oy = "Nordea Funds Oy"
+    Nordea_Hypotek_AB = "Nordea Hypotek AB"
+    Nordea_Hypoteksbank_Abp = "Nordea Hypoteksbank Abp"
+    Nordea_Kredit_Realkreditaktieselskab = "Nordea Kredit Realkreditaktieselskab"
+    Nordea_Mortgage_Bank_Plc = "Nordea Mortgage Bank Plc"
+    Norsk_Hydro_ASA = "Norsk Hydro ASA"
+    Norway = "Norway"
+    Novartis_Securities_Investment_Ltd = "Novartis Securities Investment Ltd"
+    Nykredit_Realkredit_AS = "Nykredit Realkredit A/S"
+    Oesterreichische_Kontrollbank_AG = "Oesterreichische Kontrollbank AG"
+    OP_Mortgage_Bank = "OP Mortgage Bank"
+    OTE_Plc = "OTE Plc"
+    Parker_Hannifin_Corp = "Parker Hannifin Corp"
+    Pearson_Funding_Five_Plc = "Pearson Funding Five Plc"
+    Pemex_Project_Funding_Master_Trust = "Pemex Project Funding Master Trust"
+    Petronas_Capital_Ltd = "Petronas Capital Ltd"
+    Pfandbriefstelle_der_Oesterreichischen_Landes_Hypothekenbanken = (
+        "Pfandbriefstelle der Oesterreichischen Landes-Hypothekenbanken"
+    )
+    Pilkington_Group_Ltd = "Pilkington Group Ltd"
+    Pirelli_SpA = "Pirelli SpA"
+    Poland = "Poland"
+    Portugal = "Portugal"
+    Portugal_Telecom_International_Finance_BV = (
+        "Portugal Telecom International Finance BV"
+    )
+    PostNL_NV = "PostNL NV"
+    Procter_and_Gamble_Co = "Procter & Gamble Co"
+    Promodes_SA = "Promodes SA"
+    ProSieben_SAT_1_Media_AG = "ProSieben SAT.1 Media AG"
+    Public_Power_Corp_SA = "Public Power Corp SA"
+    Publishing_and_Broadcasting_Finance_Ltd = "Publishing and Broadcasting Finance Ltd"
+    Quebec_Province_of = "Quebec (Province of)"
+    Rabobank_Nederland_NV = "Rabobank Nederland NV"
+    Realkredit_Danmark_AS = "Realkredit Danmark A/S"
+    Reed_Elsevier_Capital_Inc = "Reed Elsevier Capital Inc"
+    Renault_SA = "Renault SA"
+    Rentokil_Initial_1927_Plc = "Rentokil Initial 1927 Plc"
+    Repsol_International_Finance_BV = "Repsol International Finance BV"
+    Reseau_Ferre_de_France = "Reseau Ferre de France"
+    Residential_Capital_LLC = "Residential Capital LLC"
+    Rexam_Plc = "Rexam Plc"
+    Rheinland_Pfalz_Bank = "Rheinland-Pfalz Bank"
+    Rheinmetall_AG = "Rheinmetall AG"
+    Rhodia_SA = "Rhodia SA"
+    Rio_Tinto_Finance_Plc = "Rio Tinto Finance Plc"
+    Rohm_og_Haas_Denmark_AS = "Rohm & Haas Denmark A/S"
+    Rolls_Royce_Plc = "Rolls-Royce Plc"
+    Royal_Bank_of_Scotland_NV = "Royal Bank of Scotland NV"
+    Russia = "Russia"
+    Sachsen_Bank = "Sachsen Bank"
+    Saint_Gobain_Nederland_BV = "Saint Gobain Nederland BV"
+    Sampo_Housing_Loan_Bank_Plc = "Sampo Housing Loan Bank Plc"
+    SANOFI = "SANOFI"
+    Santander_UK_Plc = "Santander UK Plc"
+    Sara_Lee_Corp = "Sara Lee Corp"
+    Scandinavian_Airlines_System_AB = "Scandinavian Airlines System AB"
+    Scania_AB = "Scania AB"
+    Schlumberger_SA = "Schlumberger SA"
+    Schneider_Electric_SE = "Schneider Electric SE"
+    SEB_AG = "SEB AG"
+    Securitas_AB = "Securitas AB"
+    Siemens_Financieringsmaatschappij_NV = "Siemens Financieringsmaatschappij NV"
+    Singapore_Telecommunications_Ltd = "Singapore Telecommunications Ltd"
+    SingTel_Optus_Finance_Pty_Ltd = "SingTel Optus Finance Pty Ltd"
+    Skandinaviska_Enskilda_Banken_BoLan_AB = "Skandinaviska Enskilda Banken BoLån AB"
+    Slovakia = "Slovakia"
+    Slovenia = "Slovenia"
+    SNCF_Mobilites_EPIC = "SNCF Mobilites EPIC"
+    SNS_Bank_NV = "SNS Bank NV"
+    SODEXO = "SODEXO"
+    Sol_Melia_Europe_BV = "Sol Melia Europe BV"
+    Solvay_SA = "Solvay SA"
+    South_Africa = "South Africa"
+    Spain = "Spain"
+    Sparebanken_Sor = "Sparebanken Sør"
+    Sparebanken_Vest_Boligkreditt_AS = "Sparebanken Vest Boligkreditt AS"
+    Sparebankenes_Kredittselskap_AS = "Sparebankenes Kredittselskap A/S"
+    Sparkasse_KoelnBonn = "Sparkasse KoelnBonn"
+    Stadshypotek_AB = "Stadshypotek AB"
+    Stagecoach_Group_Plc = "Stagecoach Group Plc"
+    State_of_Saxony_Anhalt = "State of Saxony-Anhalt"
+    Statkraft_AS = "Statkraft AS"
+    Statoil_ASA = "Statoil ASA"
+    Stora_Enso_Oyj = "Stora Enso Oyj"
+    Sudzucker_International_Finance_BV = "Südzucker International Finance BV"
+    Sveriges_Bostadsfinansieringsaktiebolag = "Sveriges Bostadsfinansieringsaktiebolag"
+    Swedbank_Hypotek_AB = "Swedbank Hypotek AB"
+    Sweden = "Sweden"
+    Swedish_Covered_Bond_Corp = "Swedish Covered Bond Corp"
+    Swedish_Match_AB = "Swedish Match AB"
+    Switzerland = "Switzerland"
+    Syngenta_Luxembourg_Finance_SA = "Syngenta Luxembourg Finance SA"
+    TCNZ = "TCNZ"
+    TDC_AS = "TDC A/S"
+    Technicolor = "Technicolor"
+    Telecom_Italia_Finance_Sogerim_SA = "Telecom Italia Finance (Sogerim) SA"
+    Telecom_Italia_Finance_SA = "Telecom Italia Finance SA"
+    Telefonaktiebolaget_LM_Ericsson = "Telefonaktiebolaget LM Ericsson"
+    Telefonica_SA = "Telefonica SA"
+    Telenor_ASA = "Telenor ASA"
+    Telia_Company_AB = "Telia Company AB"
+    TeliaSonera_Finland_Oyj = "TeliaSonera Finland Oyj"
+    Telstra_Corporation_Ltd = "Telstra Corporation Ltd"
+    Tesco_Plc = "Tesco Plc"
+    Textron_Inc = "Textron Inc"
+    The_Nielsen_Co = "The Nielsen Co"
+    ThyssenKrupp_Finance_Nederland_BV = "ThyssenKrupp Finance Nederland BV"
+    TI_Group_Ltd = "TI Group Ltd"
+    Tokyo_Electric_Power_Co_Inc = "Tokyo Electric Power Co Inc"
+    Total_SA = "Total SA"
+    Totalkredit_AS = "Totalkredit A/S"
+    Toyota_Motor_Credit_Corp = "Toyota Motor Credit Corp"
+    Toys_R_Us_Inc = "Toys R Us Inc"
+    TPSA_Eurofinance_BV = "TPSA Eurofinance BV"
+    Turkey = "Turkey"
+    Tyco_International_Group_SA = "Tyco International Group SA"
+    Unibail = "Unibail"
+    UniCredit_Bank_AG = "UniCredit Bank AG"
+    UniCredit_Bank_Austria_AG = "UniCredit Bank Austria AG"
+    Unilever_NV = "Unilever NV"
+    United_Kingdom = "United Kingdom"
+    United_States = "United States"
+    United_Utilities_Water_Plc = "United Utilities Water Plc"
+    UPM_Kymmene_Oyj = "UPM-Kymmene Oyj"
+    Valeo_SA = "Valeo SA"
+    Vattenfall_Treasury_AB = "Vattenfall Treasury AB"
+    Vauban_Mobilisation_Garanties_SA = "Vauban Mobilisation Garanties SA"
+    Veolia_Environnement = "Veolia Environnement"
+    Vodafone_Finance_BV = "Vodafone Finance BV"
+    Voith_GmbH = "Voith GmbH"
+    Volvo_Treasury_AB = "Volvo Treasury AB"
+    Vorarlberger_Landes_und_Hypothekenbank_AG = (
+        "Vorarlberger Landes- und Hypothekenbank AG"
+    )
+    VW_Financial_Services_AG = "VW Financial Services AG"
+    Westfaelische_Landschaft_Bodenkreditbank_AG = (
+        "Westfaelische Landschaft Bodenkreditbank AG"
+    )
+    WestLB_AG = "WestLB AG"
+    Whirlpool_Corp = "Whirlpool Corp"
+    Wolters_Kluwer_NV = "Wolters Kluwer NV"
+    WPP_Plc = "WPP Plc"
+    Wurth_Finance_International_BV = "Würth Finance International BV"
+    Xerox_Corp = "Xerox Corp"
+    Yorkshire_Building_Society = "Yorkshire Building Society"
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics/shortcuts/open_banking.py` & `nordea-analytics-1.9.0/src/nordea_analytics/shortcuts/open_banking.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics.egg-info/PKG-INFO` & `nordea-analytics-1.9.0/src/nordea_analytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordea-analytics
-Version: 1.8.1
+Version: 1.9.0
 Summary: Nordea Analytics Python library
 Home-page: https://github.com/NordeaOSS/nordea-analytics
 Author: Nordea Desk Quants and Markets Advisory Tools
 Author-email: E-advisorySupport@nordea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nordea-analytics-1.8.1/src/nordea_analytics.egg-info/SOURCES.txt` & `nordea-analytics-1.9.0/src/nordea_analytics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 src/nordea_analytics/nalib/http/open_banking.py
 src/nordea_analytics/nalib/live_keyfigures/__init__.py
 src/nordea_analytics/nalib/live_keyfigures/core.py
 src/nordea_analytics/nalib/live_keyfigures/open_banking.py
 src/nordea_analytics/nalib/live_keyfigures/parsing.py
 src/nordea_analytics/nalib/value_retrievers/BenchmarkDefinition.py
 src/nordea_analytics/nalib/value_retrievers/BondFinder.py
-src/nordea_analytics/nalib/value_retrievers/BondKeyFigureAdvancedCalculator.py
 src/nordea_analytics/nalib/value_retrievers/BondKeyFigureCalculator.py
 src/nordea_analytics/nalib/value_retrievers/BondKeyFigureHorizonCalculator.py
 src/nordea_analytics/nalib/value_retrievers/BondKeyFigures.py
+src/nordea_analytics/nalib/value_retrievers/BondRepoCalculator.py
 src/nordea_analytics/nalib/value_retrievers/BondStaticData.py
 src/nordea_analytics/nalib/value_retrievers/Curve.py
 src/nordea_analytics/nalib/value_retrievers/CurveDefinition.py
 src/nordea_analytics/nalib/value_retrievers/CurveTimeSeries.py
 src/nordea_analytics/nalib/value_retrievers/DateSequence.py
 src/nordea_analytics/nalib/value_retrievers/FXForecast.py
 src/nordea_analytics/nalib/value_retrievers/FXQuotes.py
```

### Comparing `nordea-analytics-1.8.1/tests/test_proxy_finder.py` & `nordea-analytics-1.9.0/tests/test_proxy_finder.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.8.1/tests/test_util.py` & `nordea-analytics-1.9.0/tests/test_util.py`

 * *Files identical despite different names*

