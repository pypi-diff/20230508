# Comparing `tmp/dsxquant-2.0.0.tar.gz` & `tmp/dsxquant-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsxquant-2.0.0.tar", last modified: Fri Apr 28 07:54:39 2023, max compression
+gzip compressed data, was "dsxquant-2.1.0.tar", last modified: Mon May  8 02:46:28 2023, max compression
```

## Comparing `dsxquant-2.0.0.tar` & `dsxquant-2.1.0.tar`

### file list

```diff
@@ -1,80 +1,83 @@
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.493602 dsxquant-2.0.0/
--rw-r--r--   0 fengming   (501) staff       (20)     1087 2023-03-14 11:47:02.000000 dsxquant-2.0.0/LICENSE
--rw-rw-rw-   0 fengming   (501) staff       (20)       37 2023-01-13 17:11:01.000000 dsxquant-2.0.0/MANIFEST.in
--rw-r--r--   0 fengming   (501) staff       (20)    18143 2023-04-28 07:54:39.493795 dsxquant-2.0.0/PKG-INFO
--rw-r--r--   0 fengming   (501) staff       (20)    17417 2023-04-27 12:01:18.000000 dsxquant-2.0.0/README.md
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.451839 dsxquant-2.0.0/dsxquant.egg-info/
--rw-r--r--   0 fengming   (501) staff       (20)    18143 2023-04-28 07:54:38.000000 dsxquant-2.0.0/dsxquant.egg-info/PKG-INFO
--rw-r--r--   0 fengming   (501) staff       (20)     2118 2023-04-28 07:54:39.000000 dsxquant-2.0.0/dsxquant.egg-info/SOURCES.txt
--rw-r--r--   0 fengming   (501) staff       (20)        1 2023-04-28 07:54:38.000000 dsxquant-2.0.0/dsxquant.egg-info/dependency_links.txt
--rw-r--r--   0 fengming   (501) staff       (20)        1 2023-01-13 17:17:35.000000 dsxquant-2.0.0/dsxquant.egg-info/not-zip-safe
--rw-r--r--   0 fengming   (501) staff       (20)        9 2023-04-28 07:54:38.000000 dsxquant-2.0.0/dsxquant.egg-info/top_level.txt
--rw-r--r--   0 fengming   (501) staff       (20)      590 2023-04-27 11:43:13.000000 dsxquant-2.0.0/pyproject.toml
--rw-rw-rw-   0 fengming   (501) staff       (20)       82 2023-04-28 07:54:39.494717 dsxquant-2.0.0/setup.cfg
--rw-r--r--   0 fengming   (501) staff       (20)     1008 2023-04-27 11:44:27.000000 dsxquant-2.0.0/setup.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.443703 dsxquant-2.0.0/src/
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.452635 dsxquant-2.0.0/src/dsxquant/
--rw-r--r--   0 fengming   (501) staff       (20)     3791 2023-04-11 06:26:26.000000 dsxquant-2.0.0/src/dsxquant/__init__.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.453020 dsxquant-2.0.0/src/dsxquant/backtest/
--rw-r--r--   0 fengming   (501) staff       (20)    14523 2023-04-27 11:58:10.000000 dsxquant-2.0.0/src/dsxquant/backtest/back_test.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.461242 dsxquant-2.0.0/src/dsxquant/common/
--rw-r--r--   0 fengming   (501) staff       (20)    14302 2023-04-13 11:36:50.000000 dsxquant-2.0.0/src/dsxquant/common/cache.py
--rw-r--r--   0 fengming   (501) staff       (20)      115 2023-01-13 14:06:03.000000 dsxquant-2.0.0/src/dsxquant/common/fn.py
--rw-r--r--   0 fengming   (501) staff       (20)     1041 2023-02-08 13:44:10.000000 dsxquant-2.0.0/src/dsxquant/common/json2model.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.461721 dsxquant-2.0.0/src/dsxquant/config/
--rw-r--r--   0 fengming   (501) staff       (20)        0 2023-01-13 04:46:01.000000 dsxquant-2.0.0/src/dsxquant/config/__init__.py
--rw-r--r--   0 fengming   (501) staff       (20)     2931 2023-04-03 15:50:28.000000 dsxquant-2.0.0/src/dsxquant/config/config.py
--rw-r--r--   0 fengming   (501) staff       (20)      726 2023-02-28 10:01:42.000000 dsxquant-2.0.0/src/dsxquant/config/logconfig.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.462503 dsxquant-2.0.0/src/dsxquant/dataser/
--rw-r--r--   0 fengming   (501) staff       (20)        0 2023-01-13 04:45:54.000000 dsxquant-2.0.0/src/dsxquant/dataser/__init__.py
--rw-r--r--   0 fengming   (501) staff       (20)    20357 2023-04-11 06:26:36.000000 dsxquant-2.0.0/src/dsxquant/dataser/dsx_dataser.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.465671 dsxquant-2.0.0/src/dsxquant/dataser/models/
--rw-r--r--   0 fengming   (501) staff       (20)     1218 2023-02-20 16:10:27.000000 dsxquant-2.0.0/src/dsxquant/dataser/models/quotes.py
--rw-r--r--   0 fengming   (501) staff       (20)     1040 2023-04-09 15:11:20.000000 dsxquant-2.0.0/src/dsxquant/dataser/models/result.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.476785 dsxquant-2.0.0/src/dsxquant/dataser/parser/
--rw-r--r--   0 fengming   (501) staff       (20)     9247 2023-04-11 06:12:30.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/base.py
--rw-r--r--   0 fengming   (501) staff       (20)      679 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_category.py
--rw-r--r--   0 fengming   (501) staff       (20)      708 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_factors.py
--rw-r--r--   0 fengming   (501) staff       (20)     2449 2023-04-06 05:38:06.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_finance.py
--rw-r--r--   0 fengming   (501) staff       (20)     1948 2023-04-10 13:50:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_kline.py
--rw-r--r--   0 fengming   (501) staff       (20)      767 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_quotes.py
--rw-r--r--   0 fengming   (501) staff       (20)     2011 2023-04-06 05:30:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_sharebonus.py
--rw-r--r--   0 fengming   (501) staff       (20)     1198 2023-04-11 06:26:52.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_stocks.py
--rw-r--r--   0 fengming   (501) staff       (20)     1992 2023-04-06 05:30:40.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_structure.py
--rw-r--r--   0 fengming   (501) staff       (20)     1520 2023-04-11 01:02:42.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_timesharing.py
--rw-r--r--   0 fengming   (501) staff       (20)     1599 2023-04-11 01:02:27.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_translist.py
--rw-r--r--   0 fengming   (501) staff       (20)      570 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/heart.py
--rw-r--r--   0 fengming   (501) staff       (20)      838 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/login.py
--rw-r--r--   0 fengming   (501) staff       (20)      594 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/register.py
--rw-r--r--   0 fengming   (501) staff       (20)      559 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/sub_all_quotes.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.479647 dsxquant-2.0.0/src/dsxquant/emulation/
--rw-r--r--   0 fengming   (501) staff       (20)      637 2023-03-20 10:20:35.000000 dsxquant-2.0.0/src/dsxquant/emulation/base.py
--rw-r--r--   0 fengming   (501) staff       (20)      569 2023-03-20 10:20:52.000000 dsxquant-2.0.0/src/dsxquant/emulation/buy.py
--rw-r--r--   0 fengming   (501) staff       (20)      360 2023-03-18 13:46:31.000000 dsxquant-2.0.0/src/dsxquant/emulation/cancel.py
--rw-r--r--   0 fengming   (501) staff       (20)      568 2023-03-20 10:21:00.000000 dsxquant-2.0.0/src/dsxquant/emulation/sell.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.483816 dsxquant-2.0.0/src/dsxquant/engins/
--rw-r--r--   0 fengming   (501) staff       (20)     2127 2023-04-04 01:51:04.000000 dsxquant-2.0.0/src/dsxquant/engins/base.py
--rw-r--r--   0 fengming   (501) staff       (20)     1199 2023-04-03 13:32:57.000000 dsxquant-2.0.0/src/dsxquant/engins/cache_space.py
--rw-r--r--   0 fengming   (501) staff       (20)     6634 2023-04-11 13:47:37.000000 dsxquant-2.0.0/src/dsxquant/engins/data_feed.py
--rw-r--r--   0 fengming   (501) staff       (20)     2022 2023-04-04 01:49:38.000000 dsxquant-2.0.0/src/dsxquant/engins/emultion_engin.py
--rw-r--r--   0 fengming   (501) staff       (20)     2055 2023-04-26 01:51:50.000000 dsxquant-2.0.0/src/dsxquant/engins/engin.py
--rw-r--r--   0 fengming   (501) staff       (20)     3914 2023-04-26 01:52:48.000000 dsxquant-2.0.0/src/dsxquant/engins/event_bus.py
--rw-r--r--   0 fengming   (501) staff       (20)      983 2023-03-20 09:56:55.000000 dsxquant-2.0.0/src/dsxquant/engins/event_model.py
--rw-r--r--   0 fengming   (501) staff       (20)     3503 2023-04-23 15:08:44.000000 dsxquant-2.0.0/src/dsxquant/engins/strategy_engin.py
--rw-r--r--   0 fengming   (501) staff       (20)     2176 2023-03-15 15:09:55.000000 dsxquant-2.0.0/src/dsxquant/engins/trade_engin.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.483988 dsxquant-2.0.0/src/dsxquant/orders/
--rw-r--r--   0 fengming   (501) staff       (20)    14031 2023-04-27 11:39:06.000000 dsxquant-2.0.0/src/dsxquant/orders/orders.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.490837 dsxquant-2.0.0/src/dsxquant/strategy/
--rw-r--r--   0 fengming   (501) staff       (20)     4905 2023-04-11 14:48:36.000000 dsxquant-2.0.0/src/dsxquant/strategy/base.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.492163 dsxquant-2.0.0/src/dsxquant/strategy/common/
--rw-r--r--   0 fengming   (501) staff       (20)     1495 2023-04-26 01:36:49.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/macross_strategy.py
--rw-r--r--   0 fengming   (501) staff       (20)     1396 2023-03-17 11:08:35.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/myself_strategy.py
--rw-r--r--   0 fengming   (501) staff       (20)     1089 2023-03-17 13:58:55.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/t_strategy.py
--rw-r--r--   0 fengming   (501) staff       (20)     2212 2023-04-13 14:11:22.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/抛物线策略.py
--rw-r--r--   0 fengming   (501) staff       (20)     2268 2023-04-13 14:44:39.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/放量突破策略.py
--rw-r--r--   0 fengming   (501) staff       (20)     1535 2023-04-23 15:29:19.000000 dsxquant-2.0.0/src/dsxquant/strategy/data_model.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.493430 dsxquant-2.0.0/src/dsxquant/trade/
--rw-r--r--   0 fengming   (501) staff       (20)      441 2023-03-14 07:06:27.000000 dsxquant-2.0.0/src/dsxquant/trade/base.py
--rw-r--r--   0 fengming   (501) staff       (20)      321 2023-03-14 07:11:49.000000 dsxquant-2.0.0/src/dsxquant/trade/buy.py
--rw-r--r--   0 fengming   (501) staff       (20)      326 2023-03-14 07:11:58.000000 dsxquant-2.0.0/src/dsxquant/trade/cancel.py
--rw-r--r--   0 fengming   (501) staff       (20)      322 2023-03-14 07:12:02.000000 dsxquant-2.0.0/src/dsxquant/trade/sell.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.970299 dsxquant-2.1.0/
+-rw-r--r--   0 fengming   (501) staff       (20)     1087 2023-03-14 11:47:02.000000 dsxquant-2.1.0/LICENSE
+-rw-rw-rw-   0 fengming   (501) staff       (20)       37 2023-01-13 17:11:01.000000 dsxquant-2.1.0/MANIFEST.in
+-rw-r--r--   0 fengming   (501) staff       (20)    18560 2023-05-08 02:46:28.970521 dsxquant-2.1.0/PKG-INFO
+-rw-r--r--   0 fengming   (501) staff       (20)    17833 2023-05-08 02:27:08.000000 dsxquant-2.1.0/README.md
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.937932 dsxquant-2.1.0/dsxquant.egg-info/
+-rw-r--r--   0 fengming   (501) staff       (20)    18560 2023-05-08 02:46:27.000000 dsxquant-2.1.0/dsxquant.egg-info/PKG-INFO
+-rw-r--r--   0 fengming   (501) staff       (20)     2179 2023-05-08 02:46:28.000000 dsxquant-2.1.0/dsxquant.egg-info/SOURCES.txt
+-rw-r--r--   0 fengming   (501) staff       (20)        1 2023-05-08 02:46:27.000000 dsxquant-2.1.0/dsxquant.egg-info/dependency_links.txt
+-rw-r--r--   0 fengming   (501) staff       (20)        1 2023-01-13 17:17:35.000000 dsxquant-2.1.0/dsxquant.egg-info/not-zip-safe
+-rw-r--r--   0 fengming   (501) staff       (20)        9 2023-05-08 02:46:27.000000 dsxquant-2.1.0/dsxquant.egg-info/top_level.txt
+-rw-r--r--   0 fengming   (501) staff       (20)      590 2023-05-06 05:15:30.000000 dsxquant-2.1.0/pyproject.toml
+-rw-rw-rw-   0 fengming   (501) staff       (20)       82 2023-05-08 02:46:28.971103 dsxquant-2.1.0/setup.cfg
+-rw-r--r--   0 fengming   (501) staff       (20)     1008 2023-05-06 05:15:17.000000 dsxquant-2.1.0/setup.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.933631 dsxquant-2.1.0/src/
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.938249 dsxquant-2.1.0/src/dsxquant/
+-rw-r--r--   0 fengming   (501) staff       (20)     4208 2023-05-08 00:17:42.000000 dsxquant-2.1.0/src/dsxquant/__init__.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.938612 dsxquant-2.1.0/src/dsxquant/backtest/
+-rw-r--r--   0 fengming   (501) staff       (20)    14579 2023-05-06 05:19:29.000000 dsxquant-2.1.0/src/dsxquant/backtest/back_test.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.940094 dsxquant-2.1.0/src/dsxquant/common/
+-rw-r--r--   0 fengming   (501) staff       (20)    15808 2023-05-07 23:34:23.000000 dsxquant-2.1.0/src/dsxquant/common/cache.py
+-rw-r--r--   0 fengming   (501) staff       (20)      115 2023-01-13 14:06:03.000000 dsxquant-2.1.0/src/dsxquant/common/fn.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1041 2023-02-08 13:44:10.000000 dsxquant-2.1.0/src/dsxquant/common/json2model.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.940579 dsxquant-2.1.0/src/dsxquant/config/
+-rw-r--r--   0 fengming   (501) staff       (20)        0 2023-01-13 04:46:01.000000 dsxquant-2.1.0/src/dsxquant/config/__init__.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2931 2023-04-03 15:50:28.000000 dsxquant-2.1.0/src/dsxquant/config/config.py
+-rw-r--r--   0 fengming   (501) staff       (20)      726 2023-02-28 10:01:42.000000 dsxquant-2.1.0/src/dsxquant/config/logconfig.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.940924 dsxquant-2.1.0/src/dsxquant/dataser/
+-rw-r--r--   0 fengming   (501) staff       (20)        0 2023-01-13 04:45:54.000000 dsxquant-2.1.0/src/dsxquant/dataser/__init__.py
+-rw-r--r--   0 fengming   (501) staff       (20)    21399 2023-05-08 02:21:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/dsx_dataser.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.946650 dsxquant-2.1.0/src/dsxquant/dataser/models/
+-rw-r--r--   0 fengming   (501) staff       (20)     1218 2023-02-20 16:10:27.000000 dsxquant-2.1.0/src/dsxquant/dataser/models/quotes.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1040 2023-04-09 15:11:20.000000 dsxquant-2.1.0/src/dsxquant/dataser/models/result.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.954813 dsxquant-2.1.0/src/dsxquant/dataser/parser/
+-rw-r--r--   0 fengming   (501) staff       (20)     9247 2023-04-11 06:12:30.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/base.py
+-rw-r--r--   0 fengming   (501) staff       (20)      679 2023-03-01 04:18:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_category.py
+-rw-r--r--   0 fengming   (501) staff       (20)      708 2023-03-01 04:18:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_factors.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2449 2023-04-06 05:38:06.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_finance.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1948 2023-04-10 13:50:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_kline.py
+-rw-r--r--   0 fengming   (501) staff       (20)      767 2023-03-01 04:18:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_quotes.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2011 2023-04-06 05:30:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_sharebonus.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1198 2023-04-11 06:26:52.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_stocks.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1992 2023-04-06 05:30:40.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_structure.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1520 2023-04-11 01:02:42.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_timesharing.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1684 2023-05-07 10:11:02.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/get_translist.py
+-rw-r--r--   0 fengming   (501) staff       (20)      570 2023-03-01 04:18:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/heart.py
+-rw-r--r--   0 fengming   (501) staff       (20)      838 2023-03-01 04:18:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/login.py
+-rw-r--r--   0 fengming   (501) staff       (20)      594 2023-03-01 04:18:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/register.py
+-rw-r--r--   0 fengming   (501) staff       (20)      559 2023-03-01 04:18:32.000000 dsxquant-2.1.0/src/dsxquant/dataser/parser/sub_all_quotes.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.956219 dsxquant-2.1.0/src/dsxquant/emulation/
+-rw-r--r--   0 fengming   (501) staff       (20)      637 2023-03-20 10:20:35.000000 dsxquant-2.1.0/src/dsxquant/emulation/base.py
+-rw-r--r--   0 fengming   (501) staff       (20)      569 2023-03-20 10:20:52.000000 dsxquant-2.1.0/src/dsxquant/emulation/buy.py
+-rw-r--r--   0 fengming   (501) staff       (20)      360 2023-03-18 13:46:31.000000 dsxquant-2.1.0/src/dsxquant/emulation/cancel.py
+-rw-r--r--   0 fengming   (501) staff       (20)      568 2023-03-20 10:21:00.000000 dsxquant-2.1.0/src/dsxquant/emulation/sell.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.961380 dsxquant-2.1.0/src/dsxquant/engins/
+-rw-r--r--   0 fengming   (501) staff       (20)     2127 2023-04-04 01:51:04.000000 dsxquant-2.1.0/src/dsxquant/engins/base.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1199 2023-04-03 13:32:57.000000 dsxquant-2.1.0/src/dsxquant/engins/cache_space.py
+-rw-r--r--   0 fengming   (501) staff       (20)     6634 2023-04-11 13:47:37.000000 dsxquant-2.1.0/src/dsxquant/engins/data_feed.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2022 2023-04-04 01:49:38.000000 dsxquant-2.1.0/src/dsxquant/engins/emultion_engin.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2055 2023-04-26 01:51:50.000000 dsxquant-2.1.0/src/dsxquant/engins/engin.py
+-rw-r--r--   0 fengming   (501) staff       (20)     3914 2023-04-26 01:52:48.000000 dsxquant-2.1.0/src/dsxquant/engins/event_bus.py
+-rw-r--r--   0 fengming   (501) staff       (20)      983 2023-03-20 09:56:55.000000 dsxquant-2.1.0/src/dsxquant/engins/event_model.py
+-rw-r--r--   0 fengming   (501) staff       (20)     3503 2023-04-23 15:08:44.000000 dsxquant-2.1.0/src/dsxquant/engins/strategy_engin.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2176 2023-03-15 15:09:55.000000 dsxquant-2.1.0/src/dsxquant/engins/trade_engin.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.961606 dsxquant-2.1.0/src/dsxquant/orders/
+-rw-r--r--   0 fengming   (501) staff       (20)    14031 2023-04-27 11:39:06.000000 dsxquant-2.1.0/src/dsxquant/orders/orders.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.961951 dsxquant-2.1.0/src/dsxquant/restful/
+-rw-r--r--   0 fengming   (501) staff       (20)        0 2023-05-06 04:37:59.000000 dsxquant-2.1.0/src/dsxquant/restful/__init__.py
+-rw-r--r--   0 fengming   (501) staff       (20)     6736 2023-05-08 01:27:12.000000 dsxquant-2.1.0/src/dsxquant/restful/app.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.965073 dsxquant-2.1.0/src/dsxquant/strategy/
+-rw-r--r--   0 fengming   (501) staff       (20)     4905 2023-04-11 14:48:36.000000 dsxquant-2.1.0/src/dsxquant/strategy/base.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.969481 dsxquant-2.1.0/src/dsxquant/strategy/common/
+-rw-r--r--   0 fengming   (501) staff       (20)     1495 2023-04-26 01:36:49.000000 dsxquant-2.1.0/src/dsxquant/strategy/common/macross_strategy.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1396 2023-03-17 11:08:35.000000 dsxquant-2.1.0/src/dsxquant/strategy/common/myself_strategy.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1089 2023-03-17 13:58:55.000000 dsxquant-2.1.0/src/dsxquant/strategy/common/t_strategy.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2212 2023-04-13 14:11:22.000000 dsxquant-2.1.0/src/dsxquant/strategy/common/抛物线策略.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2267 2023-05-05 10:24:10.000000 dsxquant-2.1.0/src/dsxquant/strategy/common/放量突破策略.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1535 2023-04-23 15:29:19.000000 dsxquant-2.1.0/src/dsxquant/strategy/data_model.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 02:46:28.970165 dsxquant-2.1.0/src/dsxquant/trade/
+-rw-r--r--   0 fengming   (501) staff       (20)      441 2023-03-14 07:06:27.000000 dsxquant-2.1.0/src/dsxquant/trade/base.py
+-rw-r--r--   0 fengming   (501) staff       (20)      321 2023-03-14 07:11:49.000000 dsxquant-2.1.0/src/dsxquant/trade/buy.py
+-rw-r--r--   0 fengming   (501) staff       (20)      326 2023-03-14 07:11:58.000000 dsxquant-2.1.0/src/dsxquant/trade/cancel.py
+-rw-r--r--   0 fengming   (501) staff       (20)      322 2023-03-14 07:12:02.000000 dsxquant-2.1.0/src/dsxquant/trade/sell.py
```

### Comparing `dsxquant-2.0.0/LICENSE` & `dsxquant-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/PKG-INFO` & `dsxquant-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsxquant
-Version: 2.0.0
+Version: 2.1.0
 Summary: Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
 Home-page: https://github.com/dsxkline/dsx_quant_python
 Author: fangyunsm
 Author-email: fangyunsm <934476300@qq.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/dsxkline/dsxquant
 Project-URL: Bug Tracker, https://github.com/dsxkline/dsxquant/issues
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dsxquant 开源量化工具箱
 
 Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
 
-<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dsxquant"> <img alt="PyPI" src="https://img.shields.io/pypi/v/dsxquant?label=dsxquant"> <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dsxkline/dsxquant"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/dsxquant"> <img alt="Libraries.io dependency status for GitHub repo" src="https://img.shields.io/librariesio/github/dsxkline/dsxquant"> <img alt="GitHub" src="https://img.shields.io/github/license/dsxkline/dsxquant"> <img alt="GitHub search hit counter" src="https://img.shields.io/github/search/dsxkline/dsxquant/dsxquant"> <img alt="Website" src="https://img.shields.io/website?label=dsxquant%20website&up_message=online&url=https%3A%2F%2Fwww.dsxquant.com">
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dsxquant"> <img alt="PyPI" src="https://img.shields.io/pypi/v/dsxquant?label=dsxquant"> <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dsxkline/dsxquant"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/dsxquant"> <img alt="Libraries.io dependency status for GitHub repo" src="https://img.shields.io/librariesio/github/dsxkline/dsxquant"> <img alt="GitHub" src="https://img.shields.io/github/license/dsxkline/dsxquant"> <img alt="GitHub search hit counter" src="https://img.shields.io/github/search/dsxkline/dsxquant/dsxquant"> <img alt="Website" src="https://img.shields.io/website?label=dsxquant%20website&up_message=online&url=https%3A%2F%2Fwww.dsxquant.com"> <img alt="Lines of code" src="https://img.shields.io/tokei/lines/github/dsxkline/dsxquant">
 
 ## 一、简介
 Dsxquant 采用模块化设计思想，框架集成了数据、回测、策略、因子、仿真、资管、交易等模块。
 
 技术架构
 
 <img src="https://www.dsxquant.com/wp-content/uploads/2023/03/Dsxquant-Main-Engine-2-1024x985.png" width="300" />
@@ -58,15 +58,16 @@
 
 安装后直接导入包即可使用
 
 ``` python
 import dsxquant
 # dsxquant 默认维护了一个连接
 # 可直接读取实时行情
-result = dsxquant.get_quotes("sh000001,sh600000").series()
+# result = dsxquant.get_quotes("sh000001,sh600000").series()
+result = dsxquant.get_price("sh000001,sh600000").series()
 print(result)
 ```
 
 ## 五、连接
 
 连接方式：
 同步连接 （默认）connect()
@@ -101,15 +102,15 @@
 if dd_async:
     # 异步请求实时行情接口，服务器会主动推送实时行情
     def quotes_callback(response:dsxquant.parser):
         # logger.debug(response.get("msg"))
         result = response.dataframe()
         logger.debug(result)
         pass
-
+    
     result = dd_async.sub_quotes("sh000001,sh600000,sz000001,bj430047,bj430090",quotes_callback)
     logger.debug(result)
 ```
 
 ## 六、订阅
 
 Dsxquant 提供实时行情订阅功能，可批量订阅，也可以全量订阅。订阅功能需要启用异步连接 asyncconnect()，批量订阅最多支持50个股票代码，全量订阅默认全市场变动数据推送。
@@ -630,7 +631,18 @@
 backtest = BackTest(MACrossStrategy,"sz000001",start="20200412",end="20230427",data=EventType.DAYLINE)
 engin.install(backtest)
 # 等待回测完成并显示回测结果  
 backtest.show()
 engin.shutdown()
 
 ```
+
+## RESTful Api 接口
+采用Flask框架设计了一套RESTful API，支持一键启动，支持Nginx部署等
+
+```python
+import dsxquant
+dsxquant.restfulapi.run()
+
+```
+
+启动后通过浏览器进行访问 http://127.0.0.1:5000/price?symbols=sh000001,sz000001
```

### Comparing `dsxquant-2.0.0/README.md` & `dsxquant-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Dsxquant 开源量化工具箱
 
 Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
 
-<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dsxquant"> <img alt="PyPI" src="https://img.shields.io/pypi/v/dsxquant?label=dsxquant"> <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dsxkline/dsxquant"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/dsxquant"> <img alt="Libraries.io dependency status for GitHub repo" src="https://img.shields.io/librariesio/github/dsxkline/dsxquant"> <img alt="GitHub" src="https://img.shields.io/github/license/dsxkline/dsxquant"> <img alt="GitHub search hit counter" src="https://img.shields.io/github/search/dsxkline/dsxquant/dsxquant"> <img alt="Website" src="https://img.shields.io/website?label=dsxquant%20website&up_message=online&url=https%3A%2F%2Fwww.dsxquant.com">
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dsxquant"> <img alt="PyPI" src="https://img.shields.io/pypi/v/dsxquant?label=dsxquant"> <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dsxkline/dsxquant"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/dsxquant"> <img alt="Libraries.io dependency status for GitHub repo" src="https://img.shields.io/librariesio/github/dsxkline/dsxquant"> <img alt="GitHub" src="https://img.shields.io/github/license/dsxkline/dsxquant"> <img alt="GitHub search hit counter" src="https://img.shields.io/github/search/dsxkline/dsxquant/dsxquant"> <img alt="Website" src="https://img.shields.io/website?label=dsxquant%20website&up_message=online&url=https%3A%2F%2Fwww.dsxquant.com"> <img alt="Lines of code" src="https://img.shields.io/tokei/lines/github/dsxkline/dsxquant">
 
 ## 一、简介
 Dsxquant 采用模块化设计思想，框架集成了数据、回测、策略、因子、仿真、资管、交易等模块。
 
 技术架构
 
 <img src="https://www.dsxquant.com/wp-content/uploads/2023/03/Dsxquant-Main-Engine-2-1024x985.png" width="300" />
@@ -40,15 +40,16 @@
 
 安装后直接导入包即可使用
 
 ``` python
 import dsxquant
 # dsxquant 默认维护了一个连接
 # 可直接读取实时行情
-result = dsxquant.get_quotes("sh000001,sh600000").series()
+# result = dsxquant.get_quotes("sh000001,sh600000").series()
+result = dsxquant.get_price("sh000001,sh600000").series()
 print(result)
 ```
 
 ## 五、连接
 
 连接方式：
 同步连接 （默认）connect()
@@ -83,15 +84,15 @@
 if dd_async:
     # 异步请求实时行情接口，服务器会主动推送实时行情
     def quotes_callback(response:dsxquant.parser):
         # logger.debug(response.get("msg"))
         result = response.dataframe()
         logger.debug(result)
         pass
-
+    
     result = dd_async.sub_quotes("sh000001,sh600000,sz000001,bj430047,bj430090",quotes_callback)
     logger.debug(result)
 ```
 
 ## 六、订阅
 
 Dsxquant 提供实时行情订阅功能，可批量订阅，也可以全量订阅。订阅功能需要启用异步连接 asyncconnect()，批量订阅最多支持50个股票代码，全量订阅默认全市场变动数据推送。
@@ -612,7 +613,18 @@
 backtest = BackTest(MACrossStrategy,"sz000001",start="20200412",end="20230427",data=EventType.DAYLINE)
 engin.install(backtest)
 # 等待回测完成并显示回测结果  
 backtest.show()
 engin.shutdown()
 
 ```
+
+## RESTful Api 接口
+采用Flask框架设计了一套RESTful API，支持一键启动，支持Nginx部署等
+
+```python
+import dsxquant
+dsxquant.restfulapi.run()
+
+```
+
+启动后通过浏览器进行访问 http://127.0.0.1:5000/price?symbols=sh000001,sz000001
```

### Comparing `dsxquant-2.0.0/dsxquant.egg-info/PKG-INFO` & `dsxquant-2.1.0/dsxquant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsxquant
-Version: 2.0.0
+Version: 2.1.0
 Summary: Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
 Home-page: https://github.com/dsxkline/dsx_quant_python
 Author: fangyunsm
 Author-email: fangyunsm <934476300@qq.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/dsxkline/dsxquant
 Project-URL: Bug Tracker, https://github.com/dsxkline/dsxquant/issues
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dsxquant 开源量化工具箱
 
 Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
 
-<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dsxquant"> <img alt="PyPI" src="https://img.shields.io/pypi/v/dsxquant?label=dsxquant"> <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dsxkline/dsxquant"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/dsxquant"> <img alt="Libraries.io dependency status for GitHub repo" src="https://img.shields.io/librariesio/github/dsxkline/dsxquant"> <img alt="GitHub" src="https://img.shields.io/github/license/dsxkline/dsxquant"> <img alt="GitHub search hit counter" src="https://img.shields.io/github/search/dsxkline/dsxquant/dsxquant"> <img alt="Website" src="https://img.shields.io/website?label=dsxquant%20website&up_message=online&url=https%3A%2F%2Fwww.dsxquant.com">
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dsxquant"> <img alt="PyPI" src="https://img.shields.io/pypi/v/dsxquant?label=dsxquant"> <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dsxkline/dsxquant"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/dsxquant"> <img alt="Libraries.io dependency status for GitHub repo" src="https://img.shields.io/librariesio/github/dsxkline/dsxquant"> <img alt="GitHub" src="https://img.shields.io/github/license/dsxkline/dsxquant"> <img alt="GitHub search hit counter" src="https://img.shields.io/github/search/dsxkline/dsxquant/dsxquant"> <img alt="Website" src="https://img.shields.io/website?label=dsxquant%20website&up_message=online&url=https%3A%2F%2Fwww.dsxquant.com"> <img alt="Lines of code" src="https://img.shields.io/tokei/lines/github/dsxkline/dsxquant">
 
 ## 一、简介
 Dsxquant 采用模块化设计思想，框架集成了数据、回测、策略、因子、仿真、资管、交易等模块。
 
 技术架构
 
 <img src="https://www.dsxquant.com/wp-content/uploads/2023/03/Dsxquant-Main-Engine-2-1024x985.png" width="300" />
@@ -58,15 +58,16 @@
 
 安装后直接导入包即可使用
 
 ``` python
 import dsxquant
 # dsxquant 默认维护了一个连接
 # 可直接读取实时行情
-result = dsxquant.get_quotes("sh000001,sh600000").series()
+# result = dsxquant.get_quotes("sh000001,sh600000").series()
+result = dsxquant.get_price("sh000001,sh600000").series()
 print(result)
 ```
 
 ## 五、连接
 
 连接方式：
 同步连接 （默认）connect()
@@ -101,15 +102,15 @@
 if dd_async:
     # 异步请求实时行情接口，服务器会主动推送实时行情
     def quotes_callback(response:dsxquant.parser):
         # logger.debug(response.get("msg"))
         result = response.dataframe()
         logger.debug(result)
         pass
-
+    
     result = dd_async.sub_quotes("sh000001,sh600000,sz000001,bj430047,bj430090",quotes_callback)
     logger.debug(result)
 ```
 
 ## 六、订阅
 
 Dsxquant 提供实时行情订阅功能，可批量订阅，也可以全量订阅。订阅功能需要启用异步连接 asyncconnect()，批量订阅最多支持50个股票代码，全量订阅默认全市场变动数据推送。
@@ -630,7 +631,18 @@
 backtest = BackTest(MACrossStrategy,"sz000001",start="20200412",end="20230427",data=EventType.DAYLINE)
 engin.install(backtest)
 # 等待回测完成并显示回测结果  
 backtest.show()
 engin.shutdown()
 
 ```
+
+## RESTful Api 接口
+采用Flask框架设计了一套RESTful API，支持一键启动，支持Nginx部署等
+
+```python
+import dsxquant
+dsxquant.restfulapi.run()
+
+```
+
+启动后通过浏览器进行访问 http://127.0.0.1:5000/price?symbols=sh000001,sz000001
```

### Comparing `dsxquant-2.0.0/dsxquant.egg-info/SOURCES.txt` & `dsxquant-2.1.0/dsxquant.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 src/dsxquant/engins/emultion_engin.py
 src/dsxquant/engins/engin.py
 src/dsxquant/engins/event_bus.py
 src/dsxquant/engins/event_model.py
 src/dsxquant/engins/strategy_engin.py
 src/dsxquant/engins/trade_engin.py
 src/dsxquant/orders/orders.py
+src/dsxquant/restful/__init__.py
+src/dsxquant/restful/app.py
 src/dsxquant/strategy/base.py
 src/dsxquant/strategy/data_model.py
 src/dsxquant/strategy/common/macross_strategy.py
 src/dsxquant/strategy/common/myself_strategy.py
 src/dsxquant/strategy/common/t_strategy.py
 src/dsxquant/strategy/common/抛物线策略.py
 src/dsxquant/strategy/common/放量突破策略.py
```

### Comparing `dsxquant-2.0.0/pyproject.toml` & `dsxquant-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dsxquant"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
   { name="fangyunsm", email="934476300@qq.com" },
 ]
 description = "Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dsxquant-2.0.0/setup.py` & `dsxquant-2.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', encoding='utf-8') as f:
         content = f.read()
     return content
 
 
 setup(
     name="dsxquant",  # 包名称
-    version="2.0.0",  # 版本号
+    version="2.1.0",  # 版本号
     author="fangyunsm",  # 作者
     author_email="934476300@qq.com",  # 作者邮箱
     description="Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。",  # 描述
     long_description=readme(),  # 长文描述
     keywords="quant 量化",  # 项目关键词
     url="https://github.com/dsxkline/dsx_quant_python",  # 项目主页
     license="MIT License",  # 许可证
```

### Comparing `dsxquant-2.0.0/src/dsxquant/__init__.py` & `dsxquant-2.1.0/src/dsxquant/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Union
+from deprecated import deprecated
 from dsxquant.config import config
 # 默认服务器
 config.DEFAULT_SERVER_IP = "129.211.209.104"
 config.DEFAULT_PORT = 8085
 from dsxquant.config.config import MARKET,EventType,PositionStatus,BaseSymbol,FQ,MARKET_VAL
 from dsxquant.dataser.dsx_dataser import DsxDataser
 from dsxquant.dataser.parser.base import BaseParser
@@ -16,14 +17,15 @@
 from dsxquant.engins.strategy_engin import StrategyEngin
 from dsxquant.backtest.back_test import BackTest
 from dsxquant.engins.data_feed import DataFeed
 from dsxquant.orders.orders import Orders
 from dsxindexer.processors.sindexer_processor import SindexerProcessor as sindexer
 from dsxindexer.sindexer.models.kline_model import KlineModel
 from dsxquant.strategy.base import BaseStrategy
+from dsxquant.restful import app as restfulapi
 # 市场编号
 market = MARKET
 # 周期
 cycle = config.CYCLE
 # 复权
 Fq = config.FQ
 # 报表类型
@@ -54,27 +56,33 @@
 
 def get_stocks(market:int=None,symbol:str=None,hangye:str=None,gainian:str=None,diyu:str=None,listing_date:str=None,category:int=0) -> Union[BaseParser,None]:
     if connect():  return conn.get_stocks(market,symbol,hangye,gainian,diyu,listing_date,category)
 
 def get_quotes(symbols:Union[list,str,tuple]) -> Union[BaseParser,None]:
     if connect():  return conn.get_quotes(symbols)
 
+def get_price(symbols:Union[list,str,tuple]) -> Union[BaseParser,None]:
+    if connect():  return conn.get_quotes(symbols)
+
 def get_klines(symbol:str,market:int,page:int=1,page_size:int=320,fq:str=config.FQ.DEFAULT,cycle:config.CYCLE=config.CYCLE.DAY,start:str=None,end:str=None,enable_cache:bool=True) -> Union[BaseParser,None]:
     if connect():  return conn.get_klines(symbol,market,page,page_size,fq,cycle,start,end,enable_cache)
 
 def get_finance(symbol,market:int,report_type:config.REPORT_TYPE=config.REPORT_TYPE.DEFAULT,report_date="",start:str=None,end:str=None,enable_cache:bool=True) -> Union[BaseParser,None]:
     if connect():  return conn.get_finance(symbol,market,report_type,report_date,start,end,enable_cache)
 
 def get_sharebonus(symbol:str,market:int,start:str=None,end:str=None,enable_cache:bool=True) -> Union[BaseParser,None]:
     if connect():  return conn.get_sharebonus(symbol,market,start,end,enable_cache)
 
 def get_structure(symbol:str,market:int,start:str=None,end:str=None,enable_cache:bool=True) -> Union[BaseParser,None]:
     if connect():  return conn.get_structure(symbol,market,start,end,enable_cache)
 
 def get_factors(symbol:str,market:int) -> Union[BaseParser,None]:
     if connect():  return conn.get_factors(symbol,market)
-
+@deprecated
 def get_timeshring(symbol:str,market:int,trade_date:str="",enable_cache:bool=True) -> Union[BaseParser,None]:
     if connect():  return conn.get_timeshring(symbol,market,trade_date,enable_cache)
 
+def get_timesharing(symbol:str,market:int,trade_date:str="",enable_cache:bool=True) -> Union[BaseParser,None]:
+    if connect():  return conn.get_timesharing(symbol,market,trade_date,enable_cache)
+
 def get_translist(symbol:str,market:int,trade_date:str="",page:int=1,page_size:int=10,enable_cache:bool=True) -> Union[BaseParser,None]:
-    if connect():  return conn.get_quotes(symbol,market,trade_date,page,page_size,enable_cache)
+    if connect():  return conn.get_translist(symbol,market,trade_date,page,page_size,enable_cache)
```

### Comparing `dsxquant-2.0.0/src/dsxquant/backtest/back_test.py` & `dsxquant-2.1.0/src/dsxquant/backtest/back_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class BackTest:
     last_backtest = []
     def __init__(self,strategy,symbol:str,market:MARKET=MARKET.SH,start:str=None,end:str=None,funds=100000,base_symbol:BaseSymbol=BaseSymbol.HS300,data:EventType=EventType.DAYLINE,fq:FQ=FQ.QFQ,norisk=2.5,export_path=None):
         """回测
 
         Args:
+            strategy (BaseStrategy): 自定义策略类
             symbol (str): 股票代码
             market (MARKET): 市场
             start (str): 开始日期
             end (str): 结束日期
             funds (int, optional): 初始资金. Defaults to 100000.
             base_symbol (BaseSymbol, optional): 基准指数. Defaults to BaseSymbol.HS300.
             data (EventType, optional): _description_. 数据 to EventType.DAYLINE.
```

### Comparing `dsxquant-2.0.0/src/dsxquant/common/cache.py` & `dsxquant-2.1.0/src/dsxquant/common/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,21 +155,25 @@
                 pass
             dir2 = date.replace("-","")
             if report_type:
                 dir2 = report_type+"/"+date.replace("-","")
             filename = CacheHelper.get_db_filename(symbol,market,symbol,dir2,db)
             with open(filename,mode="w",encoding=CacheHelper.encoding) as f:
                 f.write(json.dumps(datas))
+            CacheHelper.save_cache_date(CacheHelper.get_db_path(symbol,report_type,db))
     
     @staticmethod
     def get_finance(symbol:str,market:int,report_type:config.REPORT_TYPE=config.REPORT_TYPE.DEFAULT,report_date="",start:str=None,end:str=None):
         db = "finance"
         path = CacheHelper.get_db_path(symbol,report_type,db)
+        # 如果今天没有缓存过，就不使用缓存
+        if not report_date and not CacheHelper.today_is_cache_date(path):return
         dir_list:list = os.listdir(path)
         if not dir_list: return []
+        if "last_date.txt" in dir_list: dir_list.remove("last_date.txt")
         dir_list.sort()
         if report_date=="":report_date = dir_list[-1]
         if not report_date : return []
         report_date = report_date.replace("-","")
         dir2 = report_date
         if report_type:
             dir2 = report_type+"/"+report_date
@@ -202,21 +206,25 @@
     def save_structure(symbol:str,market:MARKET,date:str,datas:any):
         if datas:
             db = "structure"
             dir2 = date.replace("-","")
             filename = CacheHelper.get_db_filename(symbol,market,symbol,dir2,db)
             with open(filename,mode="w",encoding=CacheHelper.encoding) as f:
                 f.write(json.dumps(datas))
+            CacheHelper.save_cache_date(CacheHelper.get_db_path(symbol,None,db))
     
     @staticmethod
     def get_structure(symbol:str,market:int,start:str=None,end:str=None):
         db = "structure"
         path = CacheHelper.get_db_path(symbol,None,db)
+        # 如果今天没有缓存过，就不使用缓存
+        if not end and not CacheHelper.today_is_cache_date(path):return
         dir_list:list = os.listdir(path)
         if not dir_list: return []
+        if "last_date.txt" in dir_list: dir_list.remove("last_date.txt")
         dir_list.sort()
         date = ""
         if date=="":date = dir_list[-1]
         if not date : return []
         date = date.replace("-","")
         dir2 = date
         if not start and not end:
@@ -248,21 +256,26 @@
     def save_sharebonus(symbol:str,market:MARKET,date:str,datas:any):
         if datas:
             db = "sharebonus"
             dir2 = date.replace("-","")
             filename = CacheHelper.get_db_filename(symbol,market,symbol,dir2,db)
             with open(filename,mode="w",encoding=CacheHelper.encoding) as f:
                 f.write(json.dumps(datas))
+            CacheHelper.save_cache_date(CacheHelper.get_db_path(symbol,None,db))
     
     @staticmethod
     def get_sharebonus(symbol:str,market:int,start:str=None,end:str=None):
         db = "sharebonus"
         path = CacheHelper.get_db_path(symbol,None,db)
+        # 如果今天没有缓存过，就不使用缓存
+        if not date and not CacheHelper.today_is_cache_date(path):return
+
         dir_list:list = os.listdir(path)
         if not dir_list: return []
+        if "last_date.txt" in dir_list: dir_list.remove("last_date.txt")
         dir_list.sort()
         date = ""
         if date=="":date = dir_list[-1]
         if not date : return []
         date = date.replace("-","")
         dir2 = date
         if not start and not end:
@@ -294,58 +307,69 @@
     def save_timesharing(symbol:str,market:MARKET,date:str,datas:any):
         if datas:
             db = "timesharing"
             dir2 = date.replace("-","")
             filename = CacheHelper.get_db_filename(symbol,market,symbol,dir2,db)
             with open(filename,mode="w",encoding=CacheHelper.encoding) as f:
                 f.write(json.dumps(datas))
+            CacheHelper.save_cache_date(CacheHelper.get_db_path(symbol,None,db))
     
     @staticmethod
     def get_timesharing(symbol:str,market:int,date:str=None):
         db = "timesharing"
         path = CacheHelper.get_db_path(symbol,None,db)
+        # 如果今天没有缓存过，就不使用缓存
+        if not date and not CacheHelper.today_is_cache_date(path):return
+
         dir_list:list = os.listdir(path)
         if not dir_list: return []
+        if "last_date.txt" in dir_list: dir_list.remove("last_date.txt")
         dir_list.sort()
         if not date:date = dir_list[-1]
         if not date : return []
         date = date.replace("-","")
         dir2 = date
         filename = CacheHelper.get_db_filename(symbol,market,symbol,dir2,db)
         if not os.path.exists(filename): return
         with open(filename,mode="r",encoding=CacheHelper.encoding) as f:
             content = f.read()
             if content:
                 content = json.loads(content)
                 return content
     
     @staticmethod
-    def save_translist(symbol:str,market:MARKET,date:str,datas:any):
+    def save_translist(symbol:str,market:MARKET,date:str,datas:any,page:int=1,page_size:int=10):
         if datas:
             db = "translist"
             dir2 = date.replace("-","")
+            dir2 += "/%s-%s" % (page,page_size)
             filename = CacheHelper.get_db_filename(symbol,market,symbol,dir2,db)
             with open(filename,mode="w",encoding=CacheHelper.encoding) as f:
                 f.write(json.dumps(datas))
+            CacheHelper.save_cache_date(os.path.dirname(filename))
     
     @staticmethod
     def get_translist(symbol:str,market:int,date:str=None,page:int=1,page_size:int=10):
         db = "translist"
         path = CacheHelper.get_db_path(symbol,None,db)
         dir_list:list = os.listdir(path)
         if not dir_list: return []
         dir_list.sort()
         if not date:date = dir_list[-1]
         if not date : return []
         date = date.replace("-","")
         dir2 = date
+        dir2 += "/%s-%s" % (page,page_size)
         filename = CacheHelper.get_db_filename(symbol,market,symbol,dir2,db)
+        # 如果今天没有缓存过，就不使用缓存
+        if not date and not CacheHelper.today_is_cache_date(os.path.dirname(filename)):return
+
         if not os.path.exists(filename): return
         with open(filename,mode="r",encoding=CacheHelper.encoding) as f:
             content = f.read()
             if content:
                 datas:list = json.loads(content)
                 # datas.reverse()
-                start = (page-1) * page_size
-                end = page * page_size
-                datas = datas[start:end]
+                # start = (page-1) * page_size
+                # end = page * page_size
+                # datas = datas[start:end]
                 return datas
```

### Comparing `dsxquant-2.0.0/src/dsxquant/common/json2model.py` & `dsxquant-2.1.0/src/dsxquant/common/json2model.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/config/config.py` & `dsxquant-2.1.0/src/dsxquant/config/config.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/config/logconfig.py` & `dsxquant-2.1.0/src/dsxquant/config/logconfig.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/dsx_dataser.py` & `dsxquant-2.1.0/src/dsxquant/dataser/dsx_dataser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import json
 import socket
 import struct
 import threading
 import time
 import traceback
 from typing import Union
+
+from deprecated import deprecated
 from dsxquant.config import config
 from dsxquant.config.logconfig import logger
 from dsxquant.dataser.parser.base import BaseParser
 from dsxquant.dataser.parser.get_quotes import GetQuotesParser
 from dsxquant.dataser.parser.register import RegisterParser
 from dsxquant.dataser.parser.get_kline import GetKlinesParser
 from dsxquant.dataser.parser.login import LoginParser
@@ -397,38 +399,51 @@
             symbol (str): 证券代码
         """
         if not self.connected:return
         r =  GetQuotesParser(self.client,self.sync,None)
         r.setParams(symbols)
         if(not self.sync): self.__save_api(r)
         return r.call_api()
+    
+    def get_price(self,symbols:Union[list,str,tuple]):
+        """请求实时行情
+
+        Args:
+            symbol (str): 证券代码
+        """
+        return self.get_quotes(symbols)
 
     def sub_quotes(self,symbols:Union[list,str,tuple],callback):
         """订阅实时行情
         订阅后系统会持续推行情过来，需要用户自己实现回调函数
 
         Args:
             symbol (str): 证券代码
         """
         if not self.connected:return
         r =  GetQuotesParser(self.client,self.sync,callback)
         r.setParams(symbols)
         if(not self.sync): self.__save_api(r)
         return r.call_api()
     
+    def sub_price(self,symbols:Union[list,str,tuple],callback):
+        return self.sub_quotes(symbols,callback)
+    
     def sub_all_quotes(self,callback):
         """订阅全市场实时行情
 
         """
         if not self.connected:return
         r =  SubAllQuotesParser(self.client,self.sync,callback)
         r.setParams()
         if(not self.sync): self.__save_api(r)
         return r.call_api()
         
+    def sub_all_price(self,callback):
+        return self.sub_all_quotes(callback)
 
     def get_klines(self,symbol:str,market:int,page:int=1,page_size:int=320,fq:str=config.FQ.DEFAULT,cycle:config.CYCLE=config.CYCLE.DAY,start:str=None,end:str=None,enable_cache:bool=True):
         """请求历史K线图
 
         Args:
             symbol (str): 证券代码
             market (int): 市场代码
@@ -512,22 +527,40 @@
             market (str): 市场代码
         """
         if not self.connected:return
         r =  GetFactorsParser(self.client)
         r.setParams(symbol,market)
         return r.call_api()
     
+    @deprecated
     def get_timeshring(self,symbol:str,market:int,trade_date:str="",enable_cache:bool=True):
         """请求分时线
 
         Args:
             symbol (str): 证券代码
             market (int): 市场编号
             trade_date (str, optional): 交易日期 %Y-%m-%d. Defaults to "".
 
+        Returns:
+            _type_: _description_
+        """
+        if not self.connected:return
+        r =  GetTimeSharingParser(self.client,self.sync,None)
+        r.setParams(symbol,market,trade_date,enable_cache)
+        if(not self.sync): self.__save_api(r)
+        return r.call_api()
+    
+    def get_timesharing(self,symbol:str,market:int,trade_date:str="",enable_cache:bool=True):
+        """请求分时线
+
+        Args:
+            symbol (str): 证券代码
+            market (int): 市场编号
+            trade_date (str, optional): 交易日期 %Y-%m-%d. Defaults to "".
+
         Returns:
             _type_: _description_
         """
         if not self.connected:return
         r =  GetTimeSharingParser(self.client,self.sync,None)
         r.setParams(symbol,market,trade_date,enable_cache)
         if(not self.sync): self.__save_api(r)
```

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/models/quotes.py` & `dsxquant-2.1.0/src/dsxquant/dataser/models/quotes.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/models/result.py` & `dsxquant-2.1.0/src/dsxquant/dataser/models/result.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/base.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/base.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_category.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_category.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_factors.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_factors.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_finance.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_finance.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_kline.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_kline.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_quotes.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_quotes.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_sharebonus.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_sharebonus.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_stocks.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_stocks.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_structure.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_structure.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_timesharing.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_timesharing.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_translist.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/get_translist.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
             market (int): 市场代码
             trade_date (str): 交易日期 Y-m-d
         """
         self.enable_cache = enable_cache
         self.symbol = symbol
         self.market = market
         self.trade_date = trade_date
+        self.page = page
+        self.page_size = page_size
         datas = self.transdata({
             "symbol":symbol,
             "market":market,
             "trade_date":trade_date,
             "page":page,
             "page_size":page_size
         })
@@ -38,13 +40,13 @@
         # logger.debug("parseResponse  "+__name__+" ")
         # 保存缓存数据
         if datas and self.enable_cache:
             if datas["success"]:
                 data = datas["data"]
                 if data:
                     if not self.trade_date:self.trade_date = datetime.datetime.now().strftime("%Y%m%d")
-                    CacheHelper.save_translist(self.symbol,self.market,self.trade_date,data)
+                    CacheHelper.save_translist(self.symbol,self.market,self.trade_date,data,self.page,self.page_size)
 
         return datas
```

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/heart.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/heart.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/login.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/login.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/register.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/register.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/dataser/parser/sub_all_quotes.py` & `dsxquant-2.1.0/src/dsxquant/dataser/parser/sub_all_quotes.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/emulation/base.py` & `dsxquant-2.1.0/src/dsxquant/emulation/base.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/emulation/buy.py` & `dsxquant-2.1.0/src/dsxquant/emulation/buy.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/emulation/sell.py` & `dsxquant-2.1.0/src/dsxquant/emulation/sell.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/engins/base.py` & `dsxquant-2.1.0/src/dsxquant/engins/base.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/engins/cache_space.py` & `dsxquant-2.1.0/src/dsxquant/engins/cache_space.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/engins/data_feed.py` & `dsxquant-2.1.0/src/dsxquant/engins/data_feed.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/engins/emultion_engin.py` & `dsxquant-2.1.0/src/dsxquant/engins/emultion_engin.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/engins/engin.py` & `dsxquant-2.1.0/src/dsxquant/engins/engin.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/engins/event_bus.py` & `dsxquant-2.1.0/src/dsxquant/engins/event_bus.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/engins/event_model.py` & `dsxquant-2.1.0/src/dsxquant/engins/event_model.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/engins/strategy_engin.py` & `dsxquant-2.1.0/src/dsxquant/engins/strategy_engin.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/engins/trade_engin.py` & `dsxquant-2.1.0/src/dsxquant/engins/trade_engin.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/orders/orders.py` & `dsxquant-2.1.0/src/dsxquant/orders/orders.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/strategy/base.py` & `dsxquant-2.1.0/src/dsxquant/strategy/base.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/strategy/common/macross_strategy.py` & `dsxquant-2.1.0/src/dsxquant/strategy/common/macross_strategy.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/strategy/common/myself_strategy.py` & `dsxquant-2.1.0/src/dsxquant/strategy/common/myself_strategy.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/strategy/common/t_strategy.py` & `dsxquant-2.1.0/src/dsxquant/strategy/common/t_strategy.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/strategy/common/抛物线策略.py` & `dsxquant-2.1.0/src/dsxquant/strategy/common/抛物线策略.py`

 * *Files identical despite different names*

### Comparing `dsxquant-2.0.0/src/dsxquant/strategy/common/放量突破策略.py` & `dsxquant-2.1.0/src/dsxquant/strategy/common/放量突破策略.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dsxquant.strategy.base import BaseStrategy
 from dsxquant import EventType,MARKET
 
 class 放量突破策略(BaseStrategy):
-
     __title__ = "放量突破策略"
     __desc__ = """
     主力放量后，第二天上涨买入
     止盈：5% 收益
     止损：-3% 止损
     """
     __type__ = (EventType.DAYBAR,EventType.MINBAR)
```

### Comparing `dsxquant-2.0.0/src/dsxquant/strategy/data_model.py` & `dsxquant-2.1.0/src/dsxquant/strategy/data_model.py`

 * *Files identical despite different names*

