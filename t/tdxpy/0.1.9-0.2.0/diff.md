# Comparing `tmp/tdxpy-0.1.9.tar.gz` & `tmp/tdxpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdxpy-0.1.9.tar", last modified: Mon Nov 28 12:32:39 2022, max compression
+gzip compressed data, was "tdxpy-0.2.0.tar", max compression
```

## Comparing `tdxpy-0.1.9.tar` & `tdxpy-0.2.0.tar`

### file list

```diff
@@ -1,73 +1,56 @@
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:32:39.092617 tdxpy-0.1.9/
--rw-r--r--   0 bopo       (501) staff       (20)     1064 2022-11-28 11:30:43.000000 tdxpy-0.1.9/LICENSE
--rw-r--r--   0 bopo       (501) staff       (20)      249 2022-11-28 11:30:43.000000 tdxpy-0.1.9/MANIFEST.in
--rw-r--r--   0 bopo       (501) staff       (20)     1592 2022-11-28 12:32:39.092687 tdxpy-0.1.9/PKG-INFO
--rw-r--r--   0 bopo       (501) staff       (20)     1291 2022-11-28 11:30:43.000000 tdxpy-0.1.9/README.md
--rw-r--r--   0 bopo       (501) staff       (20)      517 2022-11-28 12:32:35.000000 tdxpy-0.1.9/pyproject.toml
--rw-r--r--   0 bopo       (501) staff       (20)      243 2022-11-28 11:30:43.000000 tdxpy-0.1.9/requirements.txt
--rw-r--r--   0 bopo       (501) staff       (20)      756 2022-11-28 12:32:39.092972 tdxpy-0.1.9/setup.cfg
--rw-r--r--   0 bopo       (501) staff       (20)     1366 2022-11-28 12:32:35.000000 tdxpy-0.1.9/setup.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:32:39.086402 tdxpy-0.1.9/tdxpy/
--rw-r--r--   0 bopo       (501) staff       (20)       63 2022-11-28 12:32:35.000000 tdxpy-0.1.9/tdxpy/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     9373 2022-11-28 12:28:33.000000 tdxpy-0.1.9/tdxpy/base_socket_client.py
--rw-r--r--   0 bopo       (501) staff       (20)     6552 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/constants.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:32:39.087385 tdxpy-0.1.9/tdxpy/crawler/
--rw-r--r--   0 bopo       (501) staff       (20)       48 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/crawler/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     3488 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/crawler/base_crawler.py
--rw-r--r--   0 bopo       (501) staff       (20)     5976 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/crawler/history_financial_crawler.py
--rw-r--r--   0 bopo       (501) staff       (20)      441 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/exceptions.py
--rw-r--r--   0 bopo       (501) staff       (20)     4911 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/exhq.py
--rw-r--r--   0 bopo       (501) staff       (20)     1392 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/heartbeat.py
--rw-r--r--   0 bopo       (501) staff       (20)     4496 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/helper.py
--rw-r--r--   0 bopo       (501) staff       (20)    10528 2022-11-28 11:42:14.000000 tdxpy-0.1.9/tdxpy/hq.py
--rw-r--r--   0 bopo       (501) staff       (20)      321 2022-11-28 12:27:50.000000 tdxpy-0.1.9/tdxpy/logger.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:32:39.087854 tdxpy-0.1.9/tdxpy/parser/
--rw-r--r--   0 bopo       (501) staff       (20)        0 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     4754 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/base.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:32:39.089360 tdxpy-0.1.9/tdxpy/parser/ext/
--rw-r--r--   0 bopo       (501) staff       (20)        0 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     2604 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py
--rw-r--r--   0 bopo       (501) staff       (20)     1222 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_history_minute_time_data.py
--rw-r--r--   0 bopo       (501) staff       (20)     4171 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_history_transaction_data.py
--rw-r--r--   0 bopo       (501) staff       (20)     2125 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_instrument_bars.py
--rw-r--r--   0 bopo       (501) staff       (20)      343 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_instrument_count.py
--rw-r--r--   0 bopo       (501) staff       (20)     1351 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_instrument_info.py
--rw-r--r--   0 bopo       (501) staff       (20)     2853 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_instrument_quote.py
--rw-r--r--   0 bopo       (501) staff       (20)     6321 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_instrument_quote_list.py
--rw-r--r--   0 bopo       (501) staff       (20)     1253 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_markets.py
--rw-r--r--   0 bopo       (501) staff       (20)     1331 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_minute_time_data.py
--rw-r--r--   0 bopo       (501) staff       (20)     4078 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/ext/ex_get_transaction_data.py
--rw-r--r--   0 bopo       (501) staff       (20)      417 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/raw_parser.py
--rw-r--r--   0 bopo       (501) staff       (20)     1317 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/setup_commands.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:32:39.091488 tdxpy-0.1.9/tdxpy/parser/std/
--rw-r--r--   0 bopo       (501) staff       (20)        0 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     2325 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_block_info.py
--rw-r--r--   0 bopo       (501) staff       (20)     1507 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_company_info_category.py
--rw-r--r--   0 bopo       (501) staff       (20)     1119 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_company_info_content.py
--rw-r--r--   0 bopo       (501) staff       (20)     3999 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_finance_info.py
--rw-r--r--   0 bopo       (501) staff       (20)     1437 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_history_minute_time_data.py
--rw-r--r--   0 bopo       (501) staff       (20)     1735 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_history_transaction_data.py
--rw-r--r--   0 bopo       (501) staff       (20)     3056 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_index_bars.py
--rw-r--r--   0 bopo       (501) staff       (20)     1083 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_minute_time_data.py
--rw-r--r--   0 bopo       (501) staff       (20)     1015 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_report_file.py
--rw-r--r--   0 bopo       (501) staff       (20)     2838 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_security_bars.py
--rw-r--r--   0 bopo       (501) staff       (20)      569 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_security_count.py
--rw-r--r--   0 bopo       (501) staff       (20)     1412 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_security_list.py
--rw-r--r--   0 bopo       (501) staff       (20)     7770 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_security_quotes.py
--rw-r--r--   0 bopo       (501) staff       (20)     1688 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_transaction_data.py
--rw-r--r--   0 bopo       (501) staff       (20)     3868 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/parser/std/get_xdxr_info.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:32:39.092497 tdxpy-0.1.9/tdxpy/reader/
--rw-r--r--   0 bopo       (501) staff       (20)      744 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/reader/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     1365 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/reader/base_reader.py
--rw-r--r--   0 bopo       (501) staff       (20)     4386 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/reader/block_reader.py
--rw-r--r--   0 bopo       (501) staff       (20)     5612 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/reader/daily_bar_reader.py
--rw-r--r--   0 bopo       (501) staff       (20)     1712 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/reader/exhq_daily_bar_reader.py
--rw-r--r--   0 bopo       (501) staff       (20)      938 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/reader/history_financial_reader.py
--rw-r--r--   0 bopo       (501) staff       (20)     2588 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/reader/lc_min_bar_reader.py
--rw-r--r--   0 bopo       (501) staff       (20)     3053 2022-11-28 11:30:43.000000 tdxpy-0.1.9/tdxpy/reader/min_bar_reader.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:32:39.087025 tdxpy-0.1.9/tdxpy.egg-info/
--rw-r--r--   0 bopo       (501) staff       (20)     1592 2022-11-28 12:32:39.000000 tdxpy-0.1.9/tdxpy.egg-info/PKG-INFO
--rw-r--r--   0 bopo       (501) staff       (20)     2016 2022-11-28 12:32:39.000000 tdxpy-0.1.9/tdxpy.egg-info/SOURCES.txt
--rw-r--r--   0 bopo       (501) staff       (20)        1 2022-11-28 12:32:39.000000 tdxpy-0.1.9/tdxpy.egg-info/dependency_links.txt
--rw-r--r--   0 bopo       (501) staff       (20)       35 2022-11-28 12:32:39.000000 tdxpy-0.1.9/tdxpy.egg-info/requires.txt
--rw-r--r--   0 bopo       (501) staff       (20)       12 2022-11-28 12:32:39.000000 tdxpy-0.1.9/tdxpy.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1064 2023-05-08 05:02:45.303090 tdxpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1289 2023-05-08 05:02:56.770731 tdxpy-0.2.0/README.md
+-rw-r--r--   0        0        0      960 2023-05-08 05:02:56.774731 tdxpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-05-08 05:02:56.786730 tdxpy-0.2.0/tdxpy/__init__.py
+-rw-r--r--   0        0        0     9372 2023-05-08 05:02:56.786730 tdxpy-0.2.0/tdxpy/base_socket_client.py
+-rw-r--r--   0        0        0     6405 2023-05-08 05:02:56.790730 tdxpy-0.2.0/tdxpy/constants.py
+-rw-r--r--   0        0        0       48 2023-05-08 05:02:45.307090 tdxpy-0.2.0/tdxpy/crawler/__init__.py
+-rw-r--r--   0        0        0     3487 2023-05-08 05:02:56.790730 tdxpy-0.2.0/tdxpy/crawler/base_crawler.py
+-rw-r--r--   0        0        0     5975 2023-05-08 05:02:56.790730 tdxpy-0.2.0/tdxpy/crawler/history_financial_crawler.py
+-rw-r--r--   0        0        0      419 2023-05-08 05:02:56.790730 tdxpy-0.2.0/tdxpy/exceptions.py
+-rw-r--r--   0        0        0     4910 2023-05-08 05:02:56.794730 tdxpy-0.2.0/tdxpy/exhq.py
+-rw-r--r--   0        0        0     1391 2023-05-08 05:02:56.794730 tdxpy-0.2.0/tdxpy/heartbeat.py
+-rw-r--r--   0        0        0     4495 2023-05-08 05:02:56.794730 tdxpy-0.2.0/tdxpy/helper.py
+-rw-r--r--   0        0        0    11429 2023-05-08 05:02:56.794730 tdxpy-0.2.0/tdxpy/hq.py
+-rw-r--r--   0        0        0      320 2023-05-08 05:02:56.798730 tdxpy-0.2.0/tdxpy/logger.py
+-rw-r--r--   0        0        0        0 2023-05-08 05:02:45.311090 tdxpy-0.2.0/tdxpy/parser/__init__.py
+-rw-r--r--   0        0        0     4753 2023-05-08 05:02:56.798730 tdxpy-0.2.0/tdxpy/parser/base.py
+-rw-r--r--   0        0        0        0 2023-05-08 05:02:45.311090 tdxpy-0.2.0/tdxpy/parser/ext/__init__.py
+-rw-r--r--   0        0        0     2603 2023-05-08 05:02:56.798730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py
+-rw-r--r--   0        0        0     1221 2023-05-08 05:02:56.802730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_minute_time_data.py
+-rw-r--r--   0        0        0     4170 2023-05-08 05:02:56.802730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_transaction_data.py
+-rw-r--r--   0        0        0     2124 2023-05-08 05:02:56.802730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_bars.py
+-rw-r--r--   0        0        0      342 2023-05-08 05:02:56.802730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_count.py
+-rw-r--r--   0        0        0     1350 2023-05-08 05:02:56.806730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_info.py
+-rw-r--r--   0        0        0     2852 2023-05-08 05:02:56.806730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_quote.py
+-rw-r--r--   0        0        0     6320 2023-05-08 05:02:56.806730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_quote_list.py
+-rw-r--r--   0        0        0     1252 2023-05-08 05:02:56.810730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_markets.py
+-rw-r--r--   0        0        0     1330 2023-05-08 05:02:56.810730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_minute_time_data.py
+-rw-r--r--   0        0        0     4077 2023-05-08 05:02:56.810730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_transaction_data.py
+-rw-r--r--   0        0        0      396 2023-05-08 05:02:56.810730 tdxpy-0.2.0/tdxpy/parser/raw_parser.py
+-rw-r--r--   0        0        0     1316 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/setup_commands.py
+-rw-r--r--   0        0        0        0 2023-05-08 05:02:45.315090 tdxpy-0.2.0/tdxpy/parser/std/__init__.py
+-rw-r--r--   0        0        0     2324 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_block_info.py
+-rw-r--r--   0        0        0     1506 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_company_info_category.py
+-rw-r--r--   0        0        0     1071 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_company_info_content.py
+-rw-r--r--   0        0        0     3998 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_finance_info.py
+-rw-r--r--   0        0        0     1436 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_history_minute_time_data.py
+-rw-r--r--   0        0        0     1734 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_history_transaction_data.py
+-rw-r--r--   0        0        0     3055 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_index_bars.py
+-rw-r--r--   0        0        0     1082 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_minute_time_data.py
+-rw-r--r--   0        0        0      975 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_report_file.py
+-rw-r--r--   0        0        0     2837 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_security_bars.py
+-rw-r--r--   0        0        0      568 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_security_count.py
+-rw-r--r--   0        0        0     1411 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_security_list.py
+-rw-r--r--   0        0        0     7836 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_security_quotes.py
+-rw-r--r--   0        0        0     1687 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_transaction_data.py
+-rw-r--r--   0        0        0     3867 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_xdxr_info.py
+-rw-r--r--   0        0        0      744 2023-05-08 05:02:45.315090 tdxpy-0.2.0/tdxpy/reader/__init__.py
+-rw-r--r--   0        0        0     1301 2023-05-08 05:02:56.818729 tdxpy-0.2.0/tdxpy/reader/base_reader.py
+-rw-r--r--   0        0        0     4385 2023-05-08 05:02:56.818729 tdxpy-0.2.0/tdxpy/reader/block_reader.py
+-rw-r--r--   0        0        0     5611 2023-05-08 05:02:56.818729 tdxpy-0.2.0/tdxpy/reader/daily_bar_reader.py
+-rw-r--r--   0        0        0     1711 2023-05-08 05:02:56.818729 tdxpy-0.2.0/tdxpy/reader/exhq_daily_bar_reader.py
+-rw-r--r--   0        0        0      937 2023-05-08 05:02:56.822729 tdxpy-0.2.0/tdxpy/reader/history_financial_reader.py
+-rw-r--r--   0        0        0     2587 2023-05-08 05:02:56.822729 tdxpy-0.2.0/tdxpy/reader/lc_min_bar_reader.py
+-rw-r--r--   0        0        0     3052 2023-05-08 05:02:56.822729 tdxpy-0.2.0/tdxpy/reader/min_bar_reader.py
+-rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 tdxpy-0.2.0/PKG-INFO
```

### Comparing `tdxpy-0.1.9/LICENSE` & `tdxpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdxpy-0.1.9/PKG-INFO` & `tdxpy-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,40 @@
-Metadata-Version: 2.1
-Name: tdxpy
-Version: 0.1.9
-Summary: TdxPy - Python TDX 数据接口
-Home-page: https://github.com/mootdx/tdxpy
-Maintainer: BoPo
-Maintainer-email: ibopo@126.com
-License-File: LICENSE
+# TdxPy - Python TDX 数据接口
 
-TdxPy - Python TDX 数据接口
-===========================
-
-|Build Status|
+[![Build Status](https://travis-ci.org/rainx/pytdx.svg?branch=master)](https://travis-ci.org/bopo/tdxpy)
 
 如果喜欢本项目可以在右上角给颗⭐！你的支持是我最大的动力😎！
 
--  开源协议: MIT license
--  在线文档: https://tdxpy.readthedocs.io
--  国内镜像: https://gitee.com/ibopo/tdxpy
--  项目仓库: https://github.com/mootdx/tdxpy
+- 开源协议: MIT license
+- 在线文档: https://tdxpy.readthedocs.io
+- 国内镜像: https://gitee.com/ibopo/tdxpy
+- 项目仓库: https://github.com/mootdx/tdxpy
 
 项目概述
---------
-
-本项目是 pytdx 衍生项目, 原作者因不再维护了,
-以至于很多问题不能得到修复。
+---------
+本项目是 pytdx 衍生项目, 原作者因不再维护了, 以至于很多问题不能得到修复。
 
 项目特点
---------
+------
 
--  纯 python 实现，无须引入动态连接库\ ``.dll / .so``\ 文件
--  支持全平台\ ``Windows / MacOS / Linux``
--  移除\ ``python2``\ 的支持
--  去除命令行功能
--  修复若干 bug
--  重新整理项目结构
--  修复基金价格问题
+* 纯 python 实现，无须引入动态连接库`.dll / .so`文件
+* 支持全平台`Windows / MacOS / Linux`
+* 移除`python2`的支持
+* 去除命令行功能
+* 修复若干 bug
+* 重新整理项目结构
+* 修复基金价格问题
 
 快速安装
 --------
 
-.. code:: shell
-
-   pip install tdxpy
+```shell
+pip install tdxpy
+```
 
 郑重声明
---------
-
+-------
 本项目只作学习交流, 不得用于任何商业目的.
 
-此代码用于个人对网络协议的研究和习作，不对外提供服务，任何人使用本代码遇到问题请自行解决，也可以在
-github 提 issue 给我，但是我不保证能即时处理。
+此代码用于个人对网络协议的研究和习作，不对外提供服务，任何人使用本代码遇到问题请自行解决，也可以在 github 提 issue 给我，但是我不保证能即时处理。
 
 由于我们连接的是既有的行情软件兼容行情服务器，机构请不要使用此代码，对此造成的任何问题本人概不负责。
-
-.. |Build Status| image:: https://travis-ci.org/rainx/pytdx.svg?branch=master
-   :target: https://travis-ci.org/bopo/tdxpy
```

### Comparing `tdxpy-0.1.9/tdxpy/base_socket_client.py` & `tdxpy-0.2.0/tdxpy/base_socket_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import datetime
 import functools
 import socket
 import threading
 import time
 
 import pandas as pd
```

### Comparing `tdxpy-0.1.9/tdxpy/constants.py` & `tdxpy-0.2.0/tdxpy/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,175 +1,176 @@
-# cython: language_level=3
-
-class TDXParams:
-    # 市场
-
-    MARKET_SZ = 0  # 深圳
-    MARKET_SH = 1  # 上海
-
-    # K线种类
-    # K 线种类
-    # 0 -   5 分钟K 线
-    # 1 -   15 分钟K 线
-    # 2 -   30 分钟K 线
-    # 3 -   1 小时K 线
-    # 4 -   日K 线
-    # 5 -   周K 线
-    # 6 -   月K 线
-    # 7 -   1 分钟
-    # 8 -   1 分钟K 线
-    # 9 -   日K 线
-    # 10 -  季K 线
-    # 11 -  年K 线
-
-    KLINE_TYPE_5MIN = 0
-    KLINE_TYPE_15MIN = 1
-    KLINE_TYPE_30MIN = 2
-    KLINE_TYPE_1HOUR = 3
-    KLINE_TYPE_DAILY = 4
-    KLINE_TYPE_WEEKLY = 5
-    KLINE_TYPE_MONTHLY = 6
-    KLINE_TYPE_EXHQ_1MIN = 7
-    KLINE_TYPE_1MIN = 8
-    KLINE_TYPE_RI_K = 9
-    KLINE_TYPE_3MONTH = 10
-    KLINE_TYPE_YEARLY = 11
-
-    # ref : https://github.com/rainx/tdxpy/issues/7
-    # 分笔行情最多2000条
-    MAX_TRANSACTION_COUNT = 2000
-    # k先数据最多800条
-    MAX_KLINE_COUNT = 800
-
-    # 板块相关参数
-    BLOCK_SZ = "block_zs.dat"
-    BLOCK_FG = "block_fg.dat"
-    BLOCK_GN = "block_gn.dat"
-    BLOCK_DEFAULT = "block.dat"
-
-
-hq_hosts = [
-    ("长城国瑞电信1", "218.85.139.19", 7709),
-    ("长城国瑞电信2", "218.85.139.20", 7709),
-    ("长城国瑞网通", "58.23.131.163", 7709),
-    ("上证云成都电信一", "218.6.170.47", 7709),
-    ("上证云北京联通一", "123.125.108.14", 7709),
-    ("上海电信主站Z1", "180.153.18.170", 7709),
-    ("上海电信主站Z2", "180.153.18.171", 7709),
-    ("上海电信主站Z80", "180.153.18.172", 80),
-    ("北京联通主站Z1", "202.108.253.130", 7709),
-    ("北京联通主站Z2", "202.108.253.131", 7709),
-    ("北京联通主站Z80", "202.108.253.139", 80),
-    ("杭州电信主站J1", "60.191.117.167", 7709),
-    ("杭州电信主站J2", "115.238.56.198", 7709),
-    ("杭州电信主站J3", "218.75.126.9", 7709),
-    ("杭州电信主站J4", "115.238.90.165", 7709),
-    ("杭州联通主站J1", "124.160.88.183", 7709),
-    ("杭州联通主站J2", "60.12.136.250", 7709),
-    ("杭州华数主站J1", "218.108.98.244", 7709),
-    ("杭州华数主站J2", "218.108.47.69", 7709),
-    ("义乌移动主站J1", "223.94.89.115", 7709),
-    ("青岛联通主站W1", "218.57.11.101", 7709),
-    ("青岛电信主站W1", "58.58.33.123", 7709),
-    ("深圳电信主站Z1", "14.17.75.71", 7709),
-    ("云行情上海电信Z1", "114.80.63.12", 7709),
-    ("云行情上海电信Z2", "114.80.63.35", 7709),
-    ("上海电信主站Z3", "180.153.39.51", 7709),
-    ("招商证券深圳行情", "119.147.212.81", 7709),
-    ("华泰证券(南京电信)", "221.231.141.60", 7709),
-    ("华泰证券(上海电信)", "101.227.73.20", 7709),
-    ("华泰证券(上海电信二)", "101.227.77.254", 7709),
-    ("华泰证券(深圳电信)", "14.215.128.18", 7709),
-    ("华泰证券(武汉电信)", "59.173.18.140", 7709),
-    ("华泰证券(天津联通)", "60.28.23.80", 7709),
-    ("华泰证券(沈阳联通)", "218.60.29.136", 7709),
-    ("华泰证券(南京联通)", "122.192.35.44", 7709),
-    ("华泰证券(南京联通)", "122.192.35.44", 7709),
-    ("安信", "112.95.140.74", 7709),
-    ("安信", "112.95.140.92", 7709),
-    ("安信", "112.95.140.93", 7709),
-    ("安信", "114.80.149.19", 7709),
-    ("安信", "114.80.149.21", 7709),
-    ("安信", "114.80.149.22", 7709),
-    ("安信", "114.80.149.91", 7709),
-    ("安信", "114.80.149.92", 7709),
-    ("安信", "121.14.104.60", 7709),
-    ("安信", "121.14.104.66", 7709),
-    ("安信", "123.126.133.13", 7709),
-    ("安信", "123.126.133.14", 7709),
-    ("安信", "123.126.133.21", 7709),
-    ("安信", "211.139.150.61", 7709),
-    ("安信", "59.36.5.11", 7709),
-    ("广发", "119.29.19.242", 7709),
-    ("广发", "123.138.29.107", 7709),
-    ("广发", "123.138.29.108", 7709),
-    ("广发", "124.232.142.29", 7709),
-    ("广发", "183.57.72.11", 7709),
-    ("广发", "183.57.72.12", 7709),
-    ("广发", "183.57.72.13", 7709),
-    ("广发", "183.57.72.15", 7709),
-    ("广发", "183.57.72.21", 7709),
-    ("广发", "183.57.72.22", 7709),
-    ("广发", "183.57.72.23", 7709),
-    ("广发", "183.57.72.24", 7709),
-    ("广发", "183.60.224.177", 7709),
-    ("广发", "183.60.224.178", 7709),
-    ("国泰君安", "113.105.92.100", 7709),
-    ("国泰君安", "113.105.92.101", 7709),
-    ("国泰君安", "113.105.92.102", 7709),
-    ("国泰君安", "113.105.92.103", 7709),
-    ("国泰君安", "113.105.92.104", 7709),
-    ("国泰君安", "113.105.92.99", 7709),
-    ("国泰君安", "117.34.114.13", 7709),
-    ("国泰君安", "117.34.114.14", 7709),
-    ("国泰君安", "117.34.114.15", 7709),
-    ("国泰君安", "117.34.114.16", 7709),
-    ("国泰君安", "117.34.114.17", 7709),
-    ("国泰君安", "117.34.114.18", 7709),
-    ("国泰君安", "117.34.114.20", 7709),
-    ("国泰君安", "117.34.114.27", 7709),
-    ("国泰君安", "117.34.114.30", 7709),
-    ("国泰君安", "117.34.114.31", 7709),
-    ("国信", "182.131.3.252", 7709),
-    ("国信", "183.60.224.11", 7709),
-    ("国信", "58.210.106.91", 7709),
-    ("国信", "58.63.254.216", 7709),
-    ("国信", "58.63.254.219", 7709),
-    ("国信", "58.63.254.247", 7709),
-    ("海通", "123.125.108.90", 7709),
-    ("海通", "175.6.5.153", 7709),
-    ("海通", "182.118.47.151", 7709),
-    ("海通", "182.131.3.245", 7709),
-    ("海通", "202.100.166.27", 7709),
-    ("海通", "222.161.249.156", 7709),
-    ("海通", "42.123.69.62", 7709),
-    ("海通", "58.63.254.191", 7709),
-    ("海通", "58.63.254.217", 7709),
-    ("华林", "120.55.172.97", 7709),
-    ("华林", "139.217.20.27", 7709),
-    ("华林", "202.100.166.21", 7709),
-    ("华林", "202.96.138.90", 7709),
-    ("华林", "218.106.92.182", 7709),
-    ("华林", "218.106.92.183", 7709),
-    ("华林", "220.178.55.71", 7709),
-    ("华林", "220.178.55.86", 7709),
-]
-
-# 交易所
-SECURITY_EXCHANGE = ["sz", "sh"]
-
-# 股票类型
-SECURITY_TYPE = ["SH_A_STOCK", "SH_B_STOCK", "SH_INDEX", "SH_FUND", "SH_BOND", "SZ_A_STOCK", "SZ_B_STOCK", "SZ_INDEX", "SZ_FUND", "SZ_BOND"]
-
-# todo 股票系数
-SECURITY_COEFFICIENT = {
-    "SH_A_STOCK": [0.01, 0.01],
-    "SH_B_STOCK": [0.001, 0.01],
-    "SH_INDEX": [0.01, 1.0],
-    "SH_FUND": [0.001, 1.0],
-    "SH_BOND": [0.0001, 1.0],
-    "SZ_A_STOCK": [0.01, 0.01],
-    "SZ_B_STOCK": [0.01, 0.01],
-    "SZ_INDEX": [0.01, 1.0],
-    "SZ_FUND": [0.001, 0.01],
-    "SZ_BOND": [0.0001, 0.01],
-}
+# cython: language_level=3
+
+class TDXParams:
+    # 市场
+
+    MARKET_SZ = 0  # 深圳
+    MARKET_SH = 1  # 上海
+    MARKET_BJ = 2  # 北京
+
+    # K线种类
+    # K 线种类
+    # 0 -   5 分钟K 线
+    # 1 -   15 分钟K 线
+    # 2 -   30 分钟K 线
+    # 3 -   1 小时K 线
+    # 4 -   日K 线
+    # 5 -   周K 线
+    # 6 -   月K 线
+    # 7 -   1 分钟
+    # 8 -   1 分钟K 线
+    # 9 -   日K 线
+    # 10 -  季K 线
+    # 11 -  年K 线
+
+    KLINE_TYPE_5MIN = 0
+    KLINE_TYPE_15MIN = 1
+    KLINE_TYPE_30MIN = 2
+    KLINE_TYPE_1HOUR = 3
+    KLINE_TYPE_DAILY = 4
+    KLINE_TYPE_WEEKLY = 5
+    KLINE_TYPE_MONTHLY = 6
+    KLINE_TYPE_EXHQ_1MIN = 7
+    KLINE_TYPE_1MIN = 8
+    KLINE_TYPE_RI_K = 9
+    KLINE_TYPE_3MONTH = 10
+    KLINE_TYPE_YEARLY = 11
+
+    # ref : https://github.com/rainx/tdxpy/issues/7
+    # 分笔行情最多2000条
+    MAX_TRANSACTION_COUNT = 2000
+    # k先数据最多800条
+    MAX_KLINE_COUNT = 800
+
+    # 板块相关参数
+    BLOCK_SZ = "block_zs.dat"
+    BLOCK_FG = "block_fg.dat"
+    BLOCK_GN = "block_gn.dat"
+    BLOCK_DEFAULT = "block.dat"
+
+
+hq_hosts = [
+    ("长城国瑞电信1", "218.85.139.19", 7709),
+    ("长城国瑞电信2", "218.85.139.20", 7709),
+    ("长城国瑞网通", "58.23.131.163", 7709),
+    ("上证云成都电信一", "218.6.170.47", 7709),
+    ("上证云北京联通一", "123.125.108.14", 7709),
+    ("上海电信主站Z1", "180.153.18.170", 7709),
+    ("上海电信主站Z2", "180.153.18.171", 7709),
+    ("上海电信主站Z80", "180.153.18.172", 80),
+    ("北京联通主站Z1", "202.108.253.130", 7709),
+    ("北京联通主站Z2", "202.108.253.131", 7709),
+    ("北京联通主站Z80", "202.108.253.139", 80),
+    ("杭州电信主站J1", "60.191.117.167", 7709),
+    ("杭州电信主站J2", "115.238.56.198", 7709),
+    ("杭州电信主站J3", "218.75.126.9", 7709),
+    ("杭州电信主站J4", "115.238.90.165", 7709),
+    ("杭州联通主站J1", "124.160.88.183", 7709),
+    ("杭州联通主站J2", "60.12.136.250", 7709),
+    ("杭州华数主站J1", "218.108.98.244", 7709),
+    ("杭州华数主站J2", "218.108.47.69", 7709),
+    ("义乌移动主站J1", "223.94.89.115", 7709),
+    ("青岛联通主站W1", "218.57.11.101", 7709),
+    ("青岛电信主站W1", "58.58.33.123", 7709),
+    ("深圳电信主站Z1", "14.17.75.71", 7709),
+    ("云行情上海电信Z1", "114.80.63.12", 7709),
+    ("云行情上海电信Z2", "114.80.63.35", 7709),
+    ("上海电信主站Z3", "180.153.39.51", 7709),
+    ("招商证券深圳行情", "119.147.212.81", 7709),
+    ("华泰证券(南京电信)", "221.231.141.60", 7709),
+    ("华泰证券(上海电信)", "101.227.73.20", 7709),
+    ("华泰证券(上海电信二)", "101.227.77.254", 7709),
+    ("华泰证券(深圳电信)", "14.215.128.18", 7709),
+    ("华泰证券(武汉电信)", "59.173.18.140", 7709),
+    ("华泰证券(天津联通)", "60.28.23.80", 7709),
+    ("华泰证券(沈阳联通)", "218.60.29.136", 7709),
+    ("华泰证券(南京联通)", "122.192.35.44", 7709),
+    ("华泰证券(南京联通)", "122.192.35.44", 7709),
+    ("安信", "112.95.140.74", 7709),
+    ("安信", "112.95.140.92", 7709),
+    ("安信", "112.95.140.93", 7709),
+    ("安信", "114.80.149.19", 7709),
+    ("安信", "114.80.149.21", 7709),
+    ("安信", "114.80.149.22", 7709),
+    ("安信", "114.80.149.91", 7709),
+    ("安信", "114.80.149.92", 7709),
+    ("安信", "121.14.104.60", 7709),
+    ("安信", "121.14.104.66", 7709),
+    ("安信", "123.126.133.13", 7709),
+    ("安信", "123.126.133.14", 7709),
+    ("安信", "123.126.133.21", 7709),
+    ("安信", "211.139.150.61", 7709),
+    ("安信", "59.36.5.11", 7709),
+    ("广发", "119.29.19.242", 7709),
+    ("广发", "123.138.29.107", 7709),
+    ("广发", "123.138.29.108", 7709),
+    ("广发", "124.232.142.29", 7709),
+    ("广发", "183.57.72.11", 7709),
+    ("广发", "183.57.72.12", 7709),
+    ("广发", "183.57.72.13", 7709),
+    ("广发", "183.57.72.15", 7709),
+    ("广发", "183.57.72.21", 7709),
+    ("广发", "183.57.72.22", 7709),
+    ("广发", "183.57.72.23", 7709),
+    ("广发", "183.57.72.24", 7709),
+    ("广发", "183.60.224.177", 7709),
+    ("广发", "183.60.224.178", 7709),
+    ("国泰君安", "113.105.92.100", 7709),
+    ("国泰君安", "113.105.92.101", 7709),
+    ("国泰君安", "113.105.92.102", 7709),
+    ("国泰君安", "113.105.92.103", 7709),
+    ("国泰君安", "113.105.92.104", 7709),
+    ("国泰君安", "113.105.92.99", 7709),
+    ("国泰君安", "117.34.114.13", 7709),
+    ("国泰君安", "117.34.114.14", 7709),
+    ("国泰君安", "117.34.114.15", 7709),
+    ("国泰君安", "117.34.114.16", 7709),
+    ("国泰君安", "117.34.114.17", 7709),
+    ("国泰君安", "117.34.114.18", 7709),
+    ("国泰君安", "117.34.114.20", 7709),
+    ("国泰君安", "117.34.114.27", 7709),
+    ("国泰君安", "117.34.114.30", 7709),
+    ("国泰君安", "117.34.114.31", 7709),
+    ("国信", "182.131.3.252", 7709),
+    ("国信", "183.60.224.11", 7709),
+    ("国信", "58.210.106.91", 7709),
+    ("国信", "58.63.254.216", 7709),
+    ("国信", "58.63.254.219", 7709),
+    ("国信", "58.63.254.247", 7709),
+    ("海通", "123.125.108.90", 7709),
+    ("海通", "175.6.5.153", 7709),
+    ("海通", "182.118.47.151", 7709),
+    ("海通", "182.131.3.245", 7709),
+    ("海通", "202.100.166.27", 7709),
+    ("海通", "222.161.249.156", 7709),
+    ("海通", "42.123.69.62", 7709),
+    ("海通", "58.63.254.191", 7709),
+    ("海通", "58.63.254.217", 7709),
+    ("华林", "120.55.172.97", 7709),
+    ("华林", "139.217.20.27", 7709),
+    ("华林", "202.100.166.21", 7709),
+    ("华林", "202.96.138.90", 7709),
+    ("华林", "218.106.92.182", 7709),
+    ("华林", "218.106.92.183", 7709),
+    ("华林", "220.178.55.71", 7709),
+    ("华林", "220.178.55.86", 7709),
+]
+
+# 交易所
+SECURITY_EXCHANGE = ["sz", "sh"]
+
+# 股票类型
+SECURITY_TYPE = ["SH_A_STOCK", "SH_B_STOCK", "SH_INDEX", "SH_FUND", "SH_BOND", "SZ_A_STOCK", "SZ_B_STOCK", "SZ_INDEX", "SZ_FUND", "SZ_BOND"]
+
+# todo 股票系数
+SECURITY_COEFFICIENT = {
+    "SH_A_STOCK": [0.01, 0.01],
+    "SH_B_STOCK": [0.001, 0.01],
+    "SH_INDEX": [0.01, 1.0],
+    "SH_FUND": [0.001, 1.0],
+    "SH_BOND": [0.0001, 1.0],
+    "SZ_A_STOCK": [0.01, 0.01],
+    "SZ_B_STOCK": [0.01, 0.01],
+    "SZ_INDEX": [0.01, 1.0],
+    "SZ_FUND": [0.001, 0.01],
+    "SZ_BOND": [0.0001, 0.01],
+}
```

### Comparing `tdxpy-0.1.9/tdxpy/crawler/base_crawler.py` & `tdxpy-0.2.0/tdxpy/crawler/base_crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import abc
 import tempfile
 from urllib.request import Request
 from urllib.request import urlopen
 
 from tdxpy.logger import logger
```

### Comparing `tdxpy-0.1.9/tdxpy/crawler/history_financial_crawler.py` & `tdxpy-0.2.0/tdxpy/crawler/history_financial_crawler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # cython: language_level=3
-
 import secrets
 import shutil
 import tempfile
 from pathlib import Path
 from struct import calcsize
 from struct import unpack
 
 import pandas as pd
 
-from .base_crawler import BaseCrawler
 from ..exceptions import ValidationException
+from .base_crawler import BaseCrawler
 
 VALUE = "<6s1c1L"
 
 
 class HistoryFinancialListCrawler(BaseCrawler):
     """
     获取历史财务数据的接口，参考上面issue里面 @datochan 的方案和代码
```

### Comparing `tdxpy-0.1.9/tdxpy/exhq.py` & `tdxpy-0.2.0/tdxpy/exhq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 from tdxpy.base_socket_client import BaseSocketClient
 from tdxpy.base_socket_client import last_ack_time
 from tdxpy.parser.ext.ex_get_history_instrument_bars_range import GetHistoryInstrumentBarsRange
 from tdxpy.parser.ext.ex_get_history_minute_time_data import GetHistoryMinuteTimeData
 from tdxpy.parser.ext.ex_get_history_transaction_data import GetHistoryTransactionData
 from tdxpy.parser.ext.ex_get_instrument_bars import GetInstrumentBars
 from tdxpy.parser.ext.ex_get_instrument_count import GetInstrumentCount
```

### Comparing `tdxpy-0.1.9/tdxpy/heartbeat.py` & `tdxpy-0.2.0/tdxpy/heartbeat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import time
 from threading import Thread
 
 from tdxpy.logger import logger
 
 # 10秒一个heartbeat
 DEFAULT_HEARTBEAT_INTERVAL = 10.0
```

### Comparing `tdxpy-0.1.9/tdxpy/helper.py` & `tdxpy-0.2.0/tdxpy/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from pathlib import Path
 
 from tdxpy.constants import SECURITY_COEFFICIENT
 from tdxpy.logger import logger
```

### Comparing `tdxpy-0.1.9/tdxpy/hq.py` & `tdxpy-0.2.0/tdxpy/hq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # cython: language_level=3
-
 import secrets
+import warnings
 
 import pandas as pd
 
 from tdxpy.base_socket_client import BaseSocketClient
 from tdxpy.base_socket_client import last_ack_time
+from tdxpy.constants import TDXParams
 from tdxpy.parser.setup_commands import SetupCmd1
 from tdxpy.parser.setup_commands import SetupCmd2
 from tdxpy.parser.setup_commands import SetupCmd3
+from tdxpy.parser.std.get_block_info import get_and_parse_block_info
 from tdxpy.parser.std.get_block_info import GetBlockInfo
 from tdxpy.parser.std.get_block_info import GetBlockInfoMeta
-from tdxpy.parser.std.get_block_info import get_and_parse_block_info
 from tdxpy.parser.std.get_company_info_category import GetCompanyInfoCategory
 from tdxpy.parser.std.get_company_info_content import GetCompanyInfoContent
 from tdxpy.parser.std.get_finance_info import GetFinanceInfo
 from tdxpy.parser.std.get_history_minute_time_data import GetHistoryMinuteTimeData
 from tdxpy.parser.std.get_history_transaction_data import GetHistoryTransactionData
 from tdxpy.parser.std.get_index_bars import GetIndexBarsCmd
 from tdxpy.parser.std.get_minute_time_data import GetMinuteTimeData
@@ -79,17 +80,26 @@
         :param code{optional} code to query
         :return:
         """
 
         # if not all_stock:
         #     raise ValidationException('参数错误')
 
+        if isinstance(all_stock, list) and TDXParams.MARKET_BJ in [x[0] for x in all_stock]:
+            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            return None
+
+        if all_stock == TDXParams.MARKET_BJ:
+            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            return None
+
         if code:
             all_stock = [(all_stock, code)]
-        elif (isinstance(all_stock, list) or isinstance(all_stock, tuple)) and len(all_stock) == 2 and type(all_stock[0]) is int:
+        elif (isinstance(all_stock, list) or isinstance(all_stock, tuple)) and len(all_stock) == 2 and type(
+            all_stock[0]) is int:
             all_stock = [all_stock]
 
         cmd = GetSecurityQuotesCmd(self.client, lock=self.lock)
         cmd.setParams(all_stock)
 
         return cmd.call_api()
 
@@ -109,14 +119,18 @@
     def get_security_list(self, market, start):
         """
         获取证券列表
         :param market:
         :param start:
         :return:
         """
+        if market == TDXParams.MARKET_BJ:
+            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            return None
+
         cmd = GetSecurityList(self.client, lock=self.lock)
         cmd.setParams(market, start)
 
         return cmd.call_api()
 
     @last_ack_time
     def get_minute_time_data(self, market, code):
@@ -180,14 +194,18 @@
     def get_company_info_category(self, market, code):
         """
         公司信息类别
         :param market:
         :param code:
         :return:
         """
+        if market == TDXParams.MARKET_BJ:
+            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            return None
+
         cmd = GetCompanyInfoCategory(self.client, lock=self.lock)
         cmd.setParams(market, code)
 
         return cmd.call_api()
 
     @last_ack_time
     def get_company_info_content(self, market, code, filename, start, length):
@@ -196,14 +214,18 @@
         :param market:
         :param code:
         :param filename:
         :param start:
         :param length:
         :return:
         """
+        if market == TDXParams.MARKET_BJ:
+            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            return None
+
         cmd = GetCompanyInfoContent(self.client, lock=self.lock)
         cmd.setParams(market, code, filename, start, length)
 
         return cmd.call_api()
 
     @last_ack_time
     def get_xdxr_info(self, market, code):
@@ -329,15 +351,17 @@
 
         # 新版一劳永逸偷懒写法zzz
         # market_code = 1 if str(code)[0] == '6' else 0
 
         # https://github.com/rainx/pytdx/issues/33
         # 0 - 深圳， 1 - 上海
 
-        result = pd.concat([self.to_df(self.get_security_bars(9, __select_market_code(code), code, (9 - i) * 800, 800)) for i in range(10)], axis=0)
+        result = pd.concat(
+            [self.to_df(self.get_security_bars(9, __select_market_code(code), code, (9 - i) * 800, 800)) for i in
+             range(10)], axis=0)
         result = (
             result.assign(date=result["datetime"].apply(lambda x: str(x)[0:10]))
             .assign(code=str(code))
             .set_index("date", drop=False, inplace=False)
             .drop(["year", "month", "day", "hour", "minute", "datetime"], axis=1)[start_date:end_date]
         )
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/base.py` & `tdxpy-0.2.0/tdxpy/parser/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # cython: language_level=3
 import abc
 import datetime
 import struct
-
 import zlib
 
 from tdxpy.logger import logger
 
 try:
     import cython  # noqa
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
 
 
 class GetHistoryInstrumentBarsRange(BaseParser):
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_history_minute_time_data.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_minute_time_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
 
 
 class GetHistoryMinuteTimeData(BaseParser):
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_history_transaction_data.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_transaction_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import datetime
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_instrument_bars.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_bars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_datetime
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_instrument_info.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
 
 
 class GetInstrumentInfo(BaseParser):
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_instrument_quote.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
 
 
 class GetInstrumentQuote(BaseParser):
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_instrument_quote_list.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_quote_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.logger import logger
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_markets.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_markets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
 
 
 class GetMarkets(BaseParser):
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_minute_time_data.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_minute_time_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
 
 
 class GetMinuteTimeData(BaseParser):
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/ext/ex_get_transaction_data.py` & `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_transaction_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import datetime
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/setup_commands.py` & `tdxpy-0.2.0/tdxpy/parser/setup_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 from tdxpy.parser.base import BaseParser
 
 
 class BaseSetup(BaseParser):
     def parseResponse(self, body_buf):
         """
         解析返回结果
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_block_info.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_block_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 
 from tdxpy import logger
 from tdxpy.parser.base import BaseParser
 from tdxpy.reader.block_reader import BlockReader
 from tdxpy.reader.block_reader import BlockReader_TYPE_FLAT
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_company_info_category.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_company_info_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.logger import logger
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_finance_info.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_finance_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
 
 
 class GetFinanceInfo(BaseParser):
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_history_minute_time_data.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_history_minute_time_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_price
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_history_transaction_data.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_history_transaction_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_price
 from tdxpy.helper import get_time
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_index_bars.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_index_bars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_datetime
 from tdxpy.helper import get_price
 from tdxpy.helper import get_volume
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_minute_time_data.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_minute_time_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_price
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_security_bars.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_security_bars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_datetime
 from tdxpy.helper import get_price
 from tdxpy.helper import get_volume
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_security_count.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_security_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 
 from tdxpy.parser.base import BaseParser
 
 
 class GetSecurityCountCmd(BaseParser):
     def setParams(self, market):
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_security_list.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_security_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_volume
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_security_quotes.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_security_quotes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_price
 from tdxpy.helper import get_security_coefficient
 from tdxpy.helper import get_volume
 from tdxpy.parser.base import BaseParser
@@ -192,15 +191,18 @@
     def _format_time(time_stamp):
         """
         format time from reversed_bytes0
         by using method from https://github.com/rainx/pytdx/issues/187
         :param time_stamp:
         :return:
         """
-        time = time_stamp[:-6] + ":"
+        if not int(time_stamp):
+            return time_stamp
+
+        time = time_stamp[:8][:-6] + ":"
 
         if int(time_stamp[-6:-4]) < 60:
             time += "%s:" % time_stamp[-6:-4]
             time += "%06.3f" % (int(time_stamp[-4:]) * 60 / 10000.0)
         else:
             time += "%02d:" % (int(time_stamp[-6:]) * 60 / 1000000)
             time += "%06.3f" % ((int(time_stamp[-6:]) * 60 % 1000000) * 60 / 1000000.0)
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_transaction_data.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_transaction_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_price
 from tdxpy.helper import get_time
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/parser/std/get_xdxr_info.py` & `tdxpy-0.2.0/tdxpy/parser/std/get_xdxr_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_datetime
 from tdxpy.helper import get_volume
 from tdxpy.parser.base import BaseParser
```

### Comparing `tdxpy-0.1.9/tdxpy/reader/__init__.py` & `tdxpy-0.2.0/tdxpy/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.1.9/tdxpy/reader/block_reader.py` & `tdxpy-0.2.0/tdxpy/reader/block_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from collections import OrderedDict
 from pathlib import Path
 
 import pandas as pd
 
 from tdxpy.reader.base_reader import BaseReader
```

### Comparing `tdxpy-0.1.9/tdxpy/reader/daily_bar_reader.py` & `tdxpy-0.2.0/tdxpy/reader/daily_bar_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 from pathlib import Path
 
 import pandas as pd
 
 from tdxpy.logger import logger
 from tdxpy.reader.base_reader import BaseReader
 from tdxpy.reader.base_reader import TdxFileNotFoundException
```

### Comparing `tdxpy-0.1.9/tdxpy/reader/exhq_daily_bar_reader.py` & `tdxpy-0.2.0/tdxpy/reader/exhq_daily_bar_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 import struct
 from pathlib import Path
 
 import pandas as pd
 
 from tdxpy.reader.base_reader import BaseReader
 from tdxpy.reader.base_reader import TdxFileNotFoundException
```

### Comparing `tdxpy-0.1.9/tdxpy/reader/history_financial_reader.py` & `tdxpy-0.2.0/tdxpy/reader/history_financial_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 from tdxpy.crawler.history_financial_crawler import HistoryFinancialCrawler
 from tdxpy.reader.base_reader import BaseReader
 
 
 class HistoryFinancialReader(BaseReader):
     """
     使用 history_financial_cralwer 里面的HistoryFinancialCrawler完成此功能，这个reader仅对其做简单的封装
```

### Comparing `tdxpy-0.1.9/tdxpy/reader/lc_min_bar_reader.py` & `tdxpy-0.2.0/tdxpy/reader/lc_min_bar_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 from collections import OrderedDict
 from pathlib import Path
 
 import pandas as pd
 
 from tdxpy.reader.base_reader import BaseReader
 from tdxpy.reader.base_reader import TdxFileNotFoundException
```

### Comparing `tdxpy-0.1.9/tdxpy/reader/min_bar_reader.py` & `tdxpy-0.2.0/tdxpy/reader/min_bar_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # cython: language_level=3
-
 from collections import OrderedDict
 from pathlib import Path
 
 import pandas as pd
 
 from tdxpy.reader.base_reader import BaseReader
 from tdxpy.reader.base_reader import TdxFileNotFoundException
```

### Comparing `tdxpy-0.1.9/tdxpy.egg-info/PKG-INFO` & `tdxpy-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: tdxpy
-Version: 0.1.9
-Summary: TdxPy - Python TDX 数据接口
-Home-page: https://github.com/mootdx/tdxpy
-Maintainer: BoPo
-Maintainer-email: ibopo@126.com
-License-File: LICENSE
+Version: 0.2.0
+Summary: 
+Author: bopo
+Author-email: ibopo@126.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cryptography (>=38.0.3,<39.0.0)
+Requires-Dist: pandas (>=1.5.1,<2.0.0)
+Description-Content-Type: text/markdown
 
-TdxPy - Python TDX 数据接口
-===========================
+# TdxPy - Python TDX 数据接口
 
-|Build Status|
+[![Build Status](https://travis-ci.org/rainx/pytdx.svg?branch=master)](https://travis-ci.org/bopo/tdxpy)
 
 如果喜欢本项目可以在右上角给颗⭐！你的支持是我最大的动力😎！
 
--  开源协议: MIT license
--  在线文档: https://tdxpy.readthedocs.io
--  国内镜像: https://gitee.com/ibopo/tdxpy
--  项目仓库: https://github.com/mootdx/tdxpy
+- 开源协议: MIT license
+- 在线文档: https://tdxpy.readthedocs.io
+- 国内镜像: https://gitee.com/ibopo/tdxpy
+- 项目仓库: https://github.com/mootdx/tdxpy
 
 项目概述
---------
-
-本项目是 pytdx 衍生项目, 原作者因不再维护了,
-以至于很多问题不能得到修复。
+---------
+本项目是 pytdx 衍生项目, 原作者因不再维护了, 以至于很多问题不能得到修复。
 
 项目特点
---------
+------
 
--  纯 python 实现，无须引入动态连接库\ ``.dll / .so``\ 文件
--  支持全平台\ ``Windows / MacOS / Linux``
--  移除\ ``python2``\ 的支持
--  去除命令行功能
--  修复若干 bug
--  重新整理项目结构
--  修复基金价格问题
+* 纯 python 实现，无须引入动态连接库`.dll / .so`文件
+* 支持全平台`Windows / MacOS / Linux`
+* 移除`python2`的支持
+* 去除命令行功能
+* 修复若干 bug
+* 重新整理项目结构
+* 修复基金价格问题
 
 快速安装
 --------
 
-.. code:: shell
-
-   pip install tdxpy
+```shell
+pip install tdxpy
+```
 
 郑重声明
---------
-
+-------
 本项目只作学习交流, 不得用于任何商业目的.
 
-此代码用于个人对网络协议的研究和习作，不对外提供服务，任何人使用本代码遇到问题请自行解决，也可以在
-github 提 issue 给我，但是我不保证能即时处理。
+此代码用于个人对网络协议的研究和习作，不对外提供服务，任何人使用本代码遇到问题请自行解决，也可以在 github 提 issue 给我，但是我不保证能即时处理。
 
 由于我们连接的是既有的行情软件兼容行情服务器，机构请不要使用此代码，对此造成的任何问题本人概不负责。
 
-.. |Build Status| image:: https://travis-ci.org/rainx/pytdx.svg?branch=master
-   :target: https://travis-ci.org/bopo/tdxpy
```

