# Comparing `tmp/brownian-stock-0.0.8.tar.gz` & `tmp/brownian-stock-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brownian-stock-0.0.8.tar", last modified: Fri Mar 31 15:51:15 2023, max compression
+gzip compressed data, was "brownian-stock-0.0.9.tar", last modified: Fri Mar 31 16:23:25 2023, max compression
```

## Comparing `brownian-stock-0.0.8.tar` & `brownian-stock-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 15:51:15.067845 brownian-stock-0.0.8/
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1074 2023-03-29 05:15:29.000000 brownian-stock-0.0.8/LICENSE.txt
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)       33 2023-03-30 09:55:26.000000 brownian-stock-0.0.8/MANIFEST.in
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      159 2023-03-31 15:51:15.067845 brownian-stock-0.0.8/PKG-INFO
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1597 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/README.md
-drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 15:51:15.063845 brownian-stock-0.0.8/brownian/
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      984 2023-03-31 15:51:07.000000 brownian-stock-0.0.8/brownian/__init__.py
-drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 15:51:15.063845 brownian-stock-0.0.8/brownian/commands/
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        0 2023-03-30 15:50:15.000000 brownian-stock-0.0.8/brownian/commands/__init__.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)    11751 2023-03-31 07:11:14.000000 brownian-stock-0.0.8/brownian/commands/download.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     7421 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/commands/generate.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2618 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/const.py
-drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 15:51:15.063845 brownian-stock-0.0.8/brownian/data/
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)    15232 2023-03-31 06:51:42.000000 brownian-stock-0.0.8/brownian/data/calendar.json
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)    42887 2023-01-03 12:53:37.000000 brownian-stock-0.0.8/brownian/data/topix_universe.csv
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     6469 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/evaluation.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2556 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/main.py
-drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 15:51:15.067845 brownian-stock-0.0.8/brownian/models/
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        0 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/models/__init__.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     9907 2023-03-30 16:24:18.000000 brownian-stock-0.0.8/brownian/models/abstract_model.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4456 2023-03-31 15:27:51.000000 brownian-stock-0.0.8/brownian/models/abstract_series.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5333 2023-03-30 16:22:55.000000 brownian-stock-0.0.8/brownian/models/account.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      602 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/models/brand.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4442 2023-03-30 16:21:22.000000 brownian-stock-0.0.8/brownian/models/calendar.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2335 2023-03-31 07:08:03.000000 brownian-stock-0.0.8/brownian/models/index_series.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      933 2023-03-30 16:22:30.000000 brownian-stock-0.0.8/brownian/models/joined_index_series.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1280 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/models/order.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1452 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/models/pct_change_series.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5084 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/models/return_map.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     3049 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/models/sector_code.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5677 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/models/statements.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     9908 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/models/statements_report.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5929 2023-03-31 15:36:25.000000 brownian-stock-0.0.8/brownian/models/stock_series.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     7191 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/models/stock_set.py
-drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 15:51:15.067845 brownian-stock-0.0.8/brownian/repository/
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      906 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/__init__.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1151 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/brand_repository.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1506 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/index_csv_repository.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2914 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/raw_brand_repository.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5709 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/raw_statements_repository.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4302 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/raw_stock_repository.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     3086 2023-03-31 07:00:15.000000 brownian-stock-0.0.8/brownian/repository/repository_path.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2062 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/statements_csv_repository.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1703 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/statements_sql_repository.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1380 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/stock_csv_repository.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1162 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/stock_set_repository.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4001 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/repository/stock_sql_repository.py
-drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 15:51:15.067845 brownian-stock-0.0.8/brownian/services/
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        0 2023-02-01 14:09:51.000000 brownian-stock-0.0.8/brownian/services/__init__.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      840 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/services/date.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      632 2023-03-31 06:50:35.000000 brownian-stock-0.0.8/brownian/services/dot_file.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1072 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/services/download_comodity.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2132 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/services/index.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5228 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/services/jquants.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2600 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/services/neutralize.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     7035 2023-03-29 05:29:25.000000 brownian-stock-0.0.8/brownian/services/trading.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4509 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/brownian/services/universe.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1017 2023-03-31 07:08:54.000000 brownian-stock-0.0.8/brownian/services/yahoo.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5459 2023-03-31 14:43:51.000000 brownian-stock-0.0.8/brownian/simulator.py
-drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 15:51:15.067845 brownian-stock-0.0.8/brownian_stock.egg-info/
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      159 2023-03-31 15:51:15.000000 brownian-stock-0.0.8/brownian_stock.egg-info/PKG-INFO
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1979 2023-03-31 15:51:15.000000 brownian-stock-0.0.8/brownian_stock.egg-info/SOURCES.txt
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        1 2023-03-31 15:51:15.000000 brownian-stock-0.0.8/brownian_stock.egg-info/dependency_links.txt
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)       48 2023-03-31 15:51:15.000000 brownian-stock-0.0.8/brownian_stock.egg-info/entry_points.txt
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      100 2023-03-31 15:51:15.000000 brownian-stock-0.0.8/brownian_stock.egg-info/requires.txt
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)       15 2023-03-31 15:51:15.000000 brownian-stock-0.0.8/brownian_stock.egg-info/top_level.txt
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      382 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/pyproject.toml
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      123 2023-03-31 15:51:15.067845 brownian-stock-0.0.8/setup.cfg
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      652 2023-03-31 15:50:56.000000 brownian-stock-0.0.8/setup.py
-drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 15:51:15.067845 brownian-stock-0.0.8/tests/
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        0 2022-12-25 14:55:52.000000 brownian-stock-0.0.8/tests/__init__.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      532 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/tests/test_evaluation.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4400 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/tests/test_simulator.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     3902 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/tests/test_stock.py
--rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2739 2023-03-29 05:15:11.000000 brownian-stock-0.0.8/tests/test_universe.py
+drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 16:23:25.299916 brownian-stock-0.0.9/
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1074 2023-03-29 05:15:29.000000 brownian-stock-0.0.9/LICENSE.txt
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)       33 2023-03-30 09:55:26.000000 brownian-stock-0.0.9/MANIFEST.in
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      159 2023-03-31 16:23:25.299916 brownian-stock-0.0.9/PKG-INFO
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1597 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/README.md
+drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 16:23:25.291916 brownian-stock-0.0.9/brownian/
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      984 2023-03-31 16:23:10.000000 brownian-stock-0.0.9/brownian/__init__.py
+drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 16:23:25.291916 brownian-stock-0.0.9/brownian/commands/
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        0 2023-03-30 15:50:15.000000 brownian-stock-0.0.9/brownian/commands/__init__.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)    11751 2023-03-31 07:11:14.000000 brownian-stock-0.0.9/brownian/commands/download.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     7421 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/commands/generate.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2618 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/const.py
+drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 16:23:25.291916 brownian-stock-0.0.9/brownian/data/
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)    15232 2023-03-31 06:51:42.000000 brownian-stock-0.0.9/brownian/data/calendar.json
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)    42887 2023-01-03 12:53:37.000000 brownian-stock-0.0.9/brownian/data/topix_universe.csv
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     6469 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/evaluation.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2556 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/main.py
+drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 16:23:25.295916 brownian-stock-0.0.9/brownian/models/
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        0 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/models/__init__.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     9907 2023-03-30 16:24:18.000000 brownian-stock-0.0.9/brownian/models/abstract_model.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4689 2023-03-31 16:19:23.000000 brownian-stock-0.0.9/brownian/models/abstract_series.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5333 2023-03-30 16:22:55.000000 brownian-stock-0.0.9/brownian/models/account.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      602 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/models/brand.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4442 2023-03-30 16:21:22.000000 brownian-stock-0.0.9/brownian/models/calendar.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2335 2023-03-31 07:08:03.000000 brownian-stock-0.0.9/brownian/models/index_series.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      933 2023-03-30 16:22:30.000000 brownian-stock-0.0.9/brownian/models/joined_index_series.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1280 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/models/order.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1452 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/models/pct_change_series.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5084 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/models/return_map.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     3049 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/models/sector_code.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5677 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/models/statements.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     9908 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/models/statements_report.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5929 2023-03-31 15:36:25.000000 brownian-stock-0.0.9/brownian/models/stock_series.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     7191 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/models/stock_set.py
+drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 16:23:25.295916 brownian-stock-0.0.9/brownian/repository/
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      906 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/__init__.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1151 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/brand_repository.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1506 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/index_csv_repository.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2914 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/raw_brand_repository.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5709 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/raw_statements_repository.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4302 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/raw_stock_repository.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     3086 2023-03-31 07:00:15.000000 brownian-stock-0.0.9/brownian/repository/repository_path.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2062 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/statements_csv_repository.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1703 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/statements_sql_repository.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1380 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/stock_csv_repository.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1162 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/stock_set_repository.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4001 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/repository/stock_sql_repository.py
+drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 16:23:25.295916 brownian-stock-0.0.9/brownian/services/
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        0 2023-02-01 14:09:51.000000 brownian-stock-0.0.9/brownian/services/__init__.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      840 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/services/date.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      632 2023-03-31 06:50:35.000000 brownian-stock-0.0.9/brownian/services/dot_file.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1072 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/services/download_comodity.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2132 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/services/index.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5228 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/services/jquants.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2600 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/services/neutralize.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     7035 2023-03-29 05:29:25.000000 brownian-stock-0.0.9/brownian/services/trading.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4509 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/brownian/services/universe.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1017 2023-03-31 07:08:54.000000 brownian-stock-0.0.9/brownian/services/yahoo.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     5459 2023-03-31 14:43:51.000000 brownian-stock-0.0.9/brownian/simulator.py
+drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 16:23:25.299916 brownian-stock-0.0.9/brownian_stock.egg-info/
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      159 2023-03-31 16:23:25.000000 brownian-stock-0.0.9/brownian_stock.egg-info/PKG-INFO
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     1979 2023-03-31 16:23:25.000000 brownian-stock-0.0.9/brownian_stock.egg-info/SOURCES.txt
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        1 2023-03-31 16:23:25.000000 brownian-stock-0.0.9/brownian_stock.egg-info/dependency_links.txt
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)       48 2023-03-31 16:23:25.000000 brownian-stock-0.0.9/brownian_stock.egg-info/entry_points.txt
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      100 2023-03-31 16:23:25.000000 brownian-stock-0.0.9/brownian_stock.egg-info/requires.txt
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)       15 2023-03-31 16:23:25.000000 brownian-stock-0.0.9/brownian_stock.egg-info/top_level.txt
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      382 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/pyproject.toml
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      123 2023-03-31 16:23:25.299916 brownian-stock-0.0.9/setup.cfg
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      652 2023-03-31 16:23:16.000000 brownian-stock-0.0.9/setup.py
+drwxrwxr-x   0 keisuke   (1000) keisuke   (1000)        0 2023-03-31 16:23:25.299916 brownian-stock-0.0.9/tests/
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)        0 2022-12-25 14:55:52.000000 brownian-stock-0.0.9/tests/__init__.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)      532 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/tests/test_evaluation.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     4400 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/tests/test_simulator.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     3902 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/tests/test_stock.py
+-rw-rw-r--   0 keisuke   (1000) keisuke   (1000)     2739 2023-03-29 05:15:11.000000 brownian-stock-0.0.9/tests/test_universe.py
```

### Comparing `brownian-stock-0.0.8/LICENSE.txt` & `brownian-stock-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/README.md` & `brownian-stock-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/__init__.py` & `brownian-stock-0.0.9/brownian/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 from .models.statements_report import StatementsReport  # NOQA
 from .models.stock_series import StockSeries, load_stock_series  # NOQA
 from .models.stock_set import StockSet, load_stock_set  # NOQA
 from .services import date, index, neutralize, trading, universe  # NOQA
 from .services.index import average_index  # NOQA
 from .simulator import AbstractModel, Simulator  # NOQA
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

### Comparing `brownian-stock-0.0.8/brownian/commands/download.py` & `brownian-stock-0.0.9/brownian/commands/download.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/commands/generate.py` & `brownian-stock-0.0.9/brownian/commands/generate.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/const.py` & `brownian-stock-0.0.9/brownian/const.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/data/calendar.json` & `brownian-stock-0.0.9/brownian/data/calendar.json`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/data/topix_universe.csv` & `brownian-stock-0.0.9/brownian/data/topix_universe.csv`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/evaluation.py` & `brownian-stock-0.0.9/brownian/evaluation.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/main.py` & `brownian-stock-0.0.9/brownian/main.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/abstract_model.py` & `brownian-stock-0.0.9/brownian/models/abstract_model.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/abstract_series.py` & `brownian-stock-0.0.9/brownian/models/abstract_series.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,28 +92,33 @@
     def dataframe(self, as_polars :bool = False) -> Union[pl.DataFrame, pd.DataFrame]:
         if as_polars:
             return self._df
         return self._df.to_pandas()
 
     def get_value(self, target_date: datetime.date, col: str) -> Any:
         try:
-            df = self._df.filter(pl.col(const.COL_DATE) == target_date)
-            value = df[0, col]
+            idx = self._binary_search_left(target_date)
+            if self._df[idx, const.COL_DATE] != target_date:
+                return None
+            value = self._df[idx, col]
             if math.isnan(value):
                 value = None
             return value
         except Exception:
             return None
 
     def latest_value(self, col_name: str, at: Optional[datetime.date] = None) -> Any:
-        """ 最新の情報を取得する
+        """ Get latest value. If `at` is given, return latest value where d <= `at`.
         """
         if at is not None:
-            df = self._df.filter(pl.col(const.COL_DATE) <= at)
-            return df[-1, col_name]
+            next_date = at + datetime.timedelta(days=1)
+            idx = self._binary_search_left(next_date) - 1
+            if idx < 0:
+                return None
+            return self._df[idx, col_name]
         return self._df[-1, col_name]
 
     def oldest_value(self, col_name: str) -> Any:
         """ 一番古い情報を取得する
         """
         return self._df[0, col_name]
```

### Comparing `brownian-stock-0.0.8/brownian/models/account.py` & `brownian-stock-0.0.9/brownian/models/account.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/brand.py` & `brownian-stock-0.0.9/brownian/models/brand.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/calendar.py` & `brownian-stock-0.0.9/brownian/models/calendar.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/index_series.py` & `brownian-stock-0.0.9/brownian/models/index_series.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/joined_index_series.py` & `brownian-stock-0.0.9/brownian/models/joined_index_series.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/order.py` & `brownian-stock-0.0.9/brownian/models/order.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/pct_change_series.py` & `brownian-stock-0.0.9/brownian/models/pct_change_series.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/return_map.py` & `brownian-stock-0.0.9/brownian/models/return_map.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/sector_code.py` & `brownian-stock-0.0.9/brownian/models/sector_code.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/statements.py` & `brownian-stock-0.0.9/brownian/models/statements.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/statements_report.py` & `brownian-stock-0.0.9/brownian/models/statements_report.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/stock_series.py` & `brownian-stock-0.0.9/brownian/models/stock_series.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/models/stock_set.py` & `brownian-stock-0.0.9/brownian/models/stock_set.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/__init__.py` & `brownian-stock-0.0.9/brownian/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/brand_repository.py` & `brownian-stock-0.0.9/brownian/repository/brand_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/index_csv_repository.py` & `brownian-stock-0.0.9/brownian/repository/index_csv_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/raw_brand_repository.py` & `brownian-stock-0.0.9/brownian/repository/raw_brand_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/raw_statements_repository.py` & `brownian-stock-0.0.9/brownian/repository/raw_statements_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/raw_stock_repository.py` & `brownian-stock-0.0.9/brownian/repository/raw_stock_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/repository_path.py` & `brownian-stock-0.0.9/brownian/repository/repository_path.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/statements_csv_repository.py` & `brownian-stock-0.0.9/brownian/repository/statements_csv_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/statements_sql_repository.py` & `brownian-stock-0.0.9/brownian/repository/statements_sql_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/stock_csv_repository.py` & `brownian-stock-0.0.9/brownian/repository/stock_csv_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/stock_set_repository.py` & `brownian-stock-0.0.9/brownian/repository/stock_set_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/repository/stock_sql_repository.py` & `brownian-stock-0.0.9/brownian/repository/stock_sql_repository.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/services/date.py` & `brownian-stock-0.0.9/brownian/services/date.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/services/dot_file.py` & `brownian-stock-0.0.9/brownian/services/dot_file.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/services/download_comodity.py` & `brownian-stock-0.0.9/brownian/services/download_comodity.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/services/index.py` & `brownian-stock-0.0.9/brownian/services/index.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/services/jquants.py` & `brownian-stock-0.0.9/brownian/services/jquants.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/services/neutralize.py` & `brownian-stock-0.0.9/brownian/services/neutralize.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/services/trading.py` & `brownian-stock-0.0.9/brownian/services/trading.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/services/universe.py` & `brownian-stock-0.0.9/brownian/services/universe.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/services/yahoo.py` & `brownian-stock-0.0.9/brownian/services/yahoo.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian/simulator.py` & `brownian-stock-0.0.9/brownian/simulator.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/brownian_stock.egg-info/SOURCES.txt` & `brownian-stock-0.0.9/brownian_stock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/setup.py` & `brownian-stock-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="brownian-stock",
-    version="0.0.8",
+    version="0.0.9",
     long_description="Support tools for assisting analysis and verification of Japanese stocks.",
     install_requires=[
         "pandas",
         "polars",
         "numpy",
         "tqdm",
         "requests",
```

### Comparing `brownian-stock-0.0.8/tests/test_evaluation.py` & `brownian-stock-0.0.9/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/tests/test_simulator.py` & `brownian-stock-0.0.9/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/tests/test_stock.py` & `brownian-stock-0.0.9/tests/test_stock.py`

 * *Files identical despite different names*

### Comparing `brownian-stock-0.0.8/tests/test_universe.py` & `brownian-stock-0.0.9/tests/test_universe.py`

 * *Files identical despite different names*

