# Comparing `tmp/dsxindexer-1.0.0.tar.gz` & `tmp/dsxindexer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsxindexer-1.0.0.tar", last modified: Thu Mar 30 15:03:28 2023, max compression
+gzip compressed data, was "dsxindexer-1.1.0.tar", last modified: Mon May  8 08:39:17 2023, max compression
```

## Comparing `dsxindexer-1.0.0.tar` & `dsxindexer-1.1.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.727669 dsxindexer-1.0.0/
--rw-r--r--   0 fengming   (501) staff       (20)     1077 2023-03-01 09:49:49.000000 dsxindexer-1.0.0/LICENSE
--rw-rw-rw-   0 fengming   (501) staff       (20)       39 2023-03-12 13:57:03.000000 dsxindexer-1.0.0/MANIFEST.in
--rw-r--r--   0 fengming   (501) staff       (20)     3681 2023-03-30 15:03:28.728128 dsxindexer-1.0.0/PKG-INFO
--rw-r--r--   0 fengming   (501) staff       (20)     2954 2023-03-24 01:38:12.000000 dsxindexer-1.0.0/README.md
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.679250 dsxindexer-1.0.0/dsxindexer.egg-info/
--rw-r--r--   0 fengming   (501) staff       (20)     3681 2023-03-30 15:03:28.000000 dsxindexer-1.0.0/dsxindexer.egg-info/PKG-INFO
--rw-r--r--   0 fengming   (501) staff       (20)     2412 2023-03-30 15:03:28.000000 dsxindexer-1.0.0/dsxindexer.egg-info/SOURCES.txt
--rw-r--r--   0 fengming   (501) staff       (20)        1 2023-03-30 15:03:28.000000 dsxindexer-1.0.0/dsxindexer.egg-info/dependency_links.txt
--rw-r--r--   0 fengming   (501) staff       (20)        1 2023-03-12 13:57:49.000000 dsxindexer-1.0.0/dsxindexer.egg-info/not-zip-safe
--rw-r--r--   0 fengming   (501) staff       (20)       11 2023-03-30 15:03:28.000000 dsxindexer-1.0.0/dsxindexer.egg-info/top_level.txt
--rw-r--r--   0 fengming   (501) staff       (20)      565 2023-03-12 14:00:17.000000 dsxindexer-1.0.0/pyproject.toml
--rw-rw-rw-   0 fengming   (501) staff       (20)      181 2023-03-30 15:03:28.729683 dsxindexer-1.0.0/setup.cfg
--rw-r--r--   0 fengming   (501) staff       (20)     1011 2023-03-12 13:57:41.000000 dsxindexer-1.0.0/setup.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.674435 dsxindexer-1.0.0/src/
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.685916 dsxindexer-1.0.0/src/dsxindexer/
--rw-r--r--   0 fengming   (501) staff       (20)      630 2023-03-14 07:02:11.000000 dsxindexer-1.0.0/src/dsxindexer/__init__.py
--rw-r--r--   0 fengming   (501) staff       (20)     2589 2023-03-21 07:31:41.000000 dsxindexer-1.0.0/src/dsxindexer/configer.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.692782 dsxindexer-1.0.0/src/dsxindexer/factors/
--rw-r--r--   0 fengming   (501) staff       (20)      377 2023-03-06 15:18:11.000000 dsxindexer-1.0.0/src/dsxindexer/factors/base_factor.py
--rw-r--r--   0 fengming   (501) staff       (20)      366 2023-03-14 02:11:39.000000 dsxindexer-1.0.0/src/dsxindexer/factors/float_factor.py
--rw-r--r--   0 fengming   (501) staff       (20)     6667 2023-03-13 14:02:09.000000 dsxindexer-1.0.0/src/dsxindexer/factors/function_factor.py
--rw-r--r--   0 fengming   (501) staff       (20)      367 2023-03-06 12:06:36.000000 dsxindexer-1.0.0/src/dsxindexer/factors/int_factor.py
--rw-r--r--   0 fengming   (501) staff       (20)     1348 2023-03-09 01:59:24.000000 dsxindexer-1.0.0/src/dsxindexer/factors/lparen_factor.py
--rw-r--r--   0 fengming   (501) staff       (20)      406 2023-03-21 08:33:20.000000 dsxindexer-1.0.0/src/dsxindexer/factors/minus_factor.py
--rw-r--r--   0 fengming   (501) staff       (20)      457 2023-03-06 12:06:39.000000 dsxindexer-1.0.0/src/dsxindexer/factors/newline_factor.py
--rw-r--r--   0 fengming   (501) staff       (20)     1123 2023-03-13 11:05:59.000000 dsxindexer-1.0.0/src/dsxindexer/factors/string_factor.py
--rw-r--r--   0 fengming   (501) staff       (20)     1888 2023-03-09 15:52:16.000000 dsxindexer-1.0.0/src/dsxindexer/factors/variable_factor.py
--rw-r--r--   0 fengming   (501) staff       (20)     3508 2023-03-11 10:26:06.000000 dsxindexer-1.0.0/src/dsxindexer/functioner.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.704443 dsxindexer-1.0.0/src/dsxindexer/operators/
--rw-r--r--   0 fengming   (501) staff       (20)     1123 2023-03-21 07:49:41.000000 dsxindexer-1.0.0/src/dsxindexer/operators/andor_operator.py
--rw-r--r--   0 fengming   (501) staff       (20)     1589 2023-03-21 08:28:53.000000 dsxindexer-1.0.0/src/dsxindexer/operators/assign_operator.py
--rw-r--r--   0 fengming   (501) staff       (20)      430 2023-03-06 15:17:57.000000 dsxindexer-1.0.0/src/dsxindexer/operators/base_operator.py
--rw-r--r--   0 fengming   (501) staff       (20)      736 2023-03-21 08:28:46.000000 dsxindexer-1.0.0/src/dsxindexer/operators/equal_operator.py
--rw-r--r--   0 fengming   (501) staff       (20)     1627 2023-03-21 08:31:42.000000 dsxindexer-1.0.0/src/dsxindexer/operators/grealess_operator.py
--rw-r--r--   0 fengming   (501) staff       (20)      859 2023-03-06 12:07:14.000000 dsxindexer-1.0.0/src/dsxindexer/operators/greaterthen_operator.py
--rw-r--r--   0 fengming   (501) staff       (20)      651 2023-03-21 08:29:10.000000 dsxindexer-1.0.0/src/dsxindexer/operators/minus_operator.py
--rw-r--r--   0 fengming   (501) staff       (20)     1613 2023-03-21 08:29:14.000000 dsxindexer-1.0.0/src/dsxindexer/operators/muldiv_operator.py
--rw-r--r--   0 fengming   (501) staff       (20)     2061 2023-03-21 08:29:19.000000 dsxindexer-1.0.0/src/dsxindexer/operators/plusminus_operator.py
--rw-r--r--   0 fengming   (501) staff       (20)     3952 2023-03-21 08:30:41.000000 dsxindexer-1.0.0/src/dsxindexer/parser.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.706000 dsxindexer-1.0.0/src/dsxindexer/processors/
--rw-r--r--   0 fengming   (501) staff       (20)     2740 2023-03-14 06:41:27.000000 dsxindexer-1.0.0/src/dsxindexer/processors/base_processor.py
--rw-r--r--   0 fengming   (501) staff       (20)     1223 2023-03-21 08:33:35.000000 dsxindexer-1.0.0/src/dsxindexer/processors/factor_processor.py
--rw-r--r--   0 fengming   (501) staff       (20)     1396 2023-03-21 08:29:57.000000 dsxindexer-1.0.0/src/dsxindexer/processors/operator_processor.py
--rw-r--r--   0 fengming   (501) staff       (20)     4342 2023-03-20 02:23:26.000000 dsxindexer-1.0.0/src/dsxindexer/processors/sindexer_processor.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.722883 dsxindexer-1.0.0/src/dsxindexer/sindexer/
--rw-r--r--   0 fengming   (501) staff       (20)     1406 2023-03-09 13:13:56.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/BOLL.py
--rw-r--r--   0 fengming   (501) staff       (20)     1487 2023-03-11 08:39:03.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/BRAR.py
--rw-r--r--   0 fengming   (501) staff       (20)     1078 2023-03-09 08:43:51.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/CCI.py
--rw-r--r--   0 fengming   (501) staff       (20)      673 2023-03-13 06:15:13.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/CDP.py
--rw-r--r--   0 fengming   (501) staff       (20)     1005 2023-03-14 02:20:52.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/CR.py
--rw-r--r--   0 fengming   (501) staff       (20)      927 2023-03-13 09:54:40.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/DMA.py
--rw-r--r--   0 fengming   (501) staff       (20)     1625 2023-03-13 06:15:36.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/DMI.py
--rw-r--r--   0 fengming   (501) staff       (20)      934 2023-03-14 02:54:37.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/EMV.py
--rw-r--r--   0 fengming   (501) staff       (20)      827 2023-03-14 04:00:30.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/EXPMA.py
--rw-r--r--   0 fengming   (501) staff       (20)      670 2023-03-13 06:15:46.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/KDJ.py
--rw-r--r--   0 fengming   (501) staff       (20)      498 2023-03-13 06:15:55.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/MACD.py
--rw-r--r--   0 fengming   (501) staff       (20)      933 2023-03-14 03:30:27.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/MIKE.py
--rw-r--r--   0 fengming   (501) staff       (20)     1283 2023-03-11 08:20:43.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/OBV.py
--rw-r--r--   0 fengming   (501) staff       (20)      626 2023-03-11 08:30:35.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/PSY.py
--rw-r--r--   0 fengming   (501) staff       (20)      983 2023-03-13 06:16:06.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/ROC.py
--rw-r--r--   0 fengming   (501) staff       (20)      962 2023-03-13 06:16:11.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/RSI.py
--rw-r--r--   0 fengming   (501) staff       (20)      833 2023-03-11 05:42:01.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/TRIX.py
--rw-r--r--   0 fengming   (501) staff       (20)      670 2023-03-14 04:08:19.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/VR.py
--rw-r--r--   0 fengming   (501) staff       (20)      612 2023-03-13 06:17:16.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/WR.py
--rw-r--r--   0 fengming   (501) staff       (20)      571 2023-03-14 04:11:15.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/WVAD.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.726023 dsxindexer-1.0.0/src/dsxindexer/sindexer/base/
--rw-r--r--   0 fengming   (501) staff       (20)     2416 2023-03-10 14:42:50.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/base/cons_funcs.py
--rw-r--r--   0 fengming   (501) staff       (20)    11909 2023-03-27 01:51:30.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/base/index_funcs.py
--rw-r--r--   0 fengming   (501) staff       (20)     1228 2023-03-10 14:42:42.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/base/large_funcs.py
--rw-r--r--   0 fengming   (501) staff       (20)     3797 2023-03-13 15:03:59.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/base/logical_funcs.py
--rw-r--r--   0 fengming   (501) staff       (20)    10484 2023-03-11 08:35:45.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/base/math_funcs.py
--rw-r--r--   0 fengming   (501) staff       (20)     2989 2023-03-13 05:59:38.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/base/price_funcs.py
--rw-r--r--   0 fengming   (501) staff       (20)     4908 2023-03-11 08:46:49.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/base/refer_funcs.py
--rw-r--r--   0 fengming   (501) staff       (20)     9992 2023-03-14 06:40:43.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/base_sindexer.py
--rw-r--r--   0 fengming   (501) staff       (20)     5703 2023-03-14 04:54:07.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/fomulas.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-30 15:03:28.726633 dsxindexer-1.0.0/src/dsxindexer/sindexer/models/
--rw-r--r--   0 fengming   (501) staff       (20)      377 2023-03-05 10:42:53.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/models/kline_model.py
--rw-r--r--   0 fengming   (501) staff       (20)      518 2023-03-14 06:41:06.000000 dsxindexer-1.0.0/src/dsxindexer/sindexer/sindexer_factory.py
--rw-r--r--   0 fengming   (501) staff       (20)    14277 2023-03-21 08:08:51.000000 dsxindexer-1.0.0/src/dsxindexer/tokenizer.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.373848 dsxindexer-1.1.0/
+-rw-r--r--   0 fengming   (501) staff       (20)     1077 2023-03-01 09:49:49.000000 dsxindexer-1.1.0/LICENSE
+-rw-rw-rw-   0 fengming   (501) staff       (20)       39 2023-03-12 13:57:03.000000 dsxindexer-1.1.0/MANIFEST.in
+-rw-r--r--   0 fengming   (501) staff       (20)     3699 2023-05-08 08:39:17.373987 dsxindexer-1.1.0/PKG-INFO
+-rw-r--r--   0 fengming   (501) staff       (20)     2972 2023-05-08 08:30:21.000000 dsxindexer-1.1.0/README.md
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.288717 dsxindexer-1.1.0/dsxindexer.egg-info/
+-rw-r--r--   0 fengming   (501) staff       (20)     3699 2023-05-08 08:39:17.000000 dsxindexer-1.1.0/dsxindexer.egg-info/PKG-INFO
+-rw-r--r--   0 fengming   (501) staff       (20)     2445 2023-05-08 08:39:17.000000 dsxindexer-1.1.0/dsxindexer.egg-info/SOURCES.txt
+-rw-r--r--   0 fengming   (501) staff       (20)        1 2023-05-08 08:39:17.000000 dsxindexer-1.1.0/dsxindexer.egg-info/dependency_links.txt
+-rw-r--r--   0 fengming   (501) staff       (20)        1 2023-03-12 13:57:49.000000 dsxindexer-1.1.0/dsxindexer.egg-info/not-zip-safe
+-rw-r--r--   0 fengming   (501) staff       (20)       49 2023-05-08 08:39:17.000000 dsxindexer-1.1.0/dsxindexer.egg-info/requires.txt
+-rw-r--r--   0 fengming   (501) staff       (20)       11 2023-05-08 08:39:17.000000 dsxindexer-1.1.0/dsxindexer.egg-info/top_level.txt
+-rw-r--r--   0 fengming   (501) staff       (20)      565 2023-05-08 08:30:30.000000 dsxindexer-1.1.0/pyproject.toml
+-rw-rw-rw-   0 fengming   (501) staff       (20)      199 2023-05-08 08:39:17.375205 dsxindexer-1.1.0/setup.cfg
+-rw-r--r--   0 fengming   (501) staff       (20)     1102 2023-05-08 08:38:55.000000 dsxindexer-1.1.0/setup.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.283738 dsxindexer-1.1.0/src/
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.294609 dsxindexer-1.1.0/src/dsxindexer/
+-rw-r--r--   0 fengming   (501) staff       (20)      630 2023-03-14 07:02:11.000000 dsxindexer-1.1.0/src/dsxindexer/__init__.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2698 2023-04-10 08:50:26.000000 dsxindexer-1.1.0/src/dsxindexer/configer.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.312180 dsxindexer-1.1.0/src/dsxindexer/factors/
+-rw-r--r--   0 fengming   (501) staff       (20)      377 2023-03-06 15:18:11.000000 dsxindexer-1.1.0/src/dsxindexer/factors/base_factor.py
+-rw-r--r--   0 fengming   (501) staff       (20)      366 2023-03-14 02:11:39.000000 dsxindexer-1.1.0/src/dsxindexer/factors/float_factor.py
+-rw-r--r--   0 fengming   (501) staff       (20)     9446 2023-05-05 04:36:08.000000 dsxindexer-1.1.0/src/dsxindexer/factors/function_factor.py
+-rw-r--r--   0 fengming   (501) staff       (20)      367 2023-03-06 12:06:36.000000 dsxindexer-1.1.0/src/dsxindexer/factors/int_factor.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1348 2023-03-09 01:59:24.000000 dsxindexer-1.1.0/src/dsxindexer/factors/lparen_factor.py
+-rw-r--r--   0 fengming   (501) staff       (20)      406 2023-03-21 08:33:20.000000 dsxindexer-1.1.0/src/dsxindexer/factors/minus_factor.py
+-rw-r--r--   0 fengming   (501) staff       (20)      457 2023-03-06 12:06:39.000000 dsxindexer-1.1.0/src/dsxindexer/factors/newline_factor.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1123 2023-03-13 11:05:59.000000 dsxindexer-1.1.0/src/dsxindexer/factors/string_factor.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1888 2023-03-09 15:52:16.000000 dsxindexer-1.1.0/src/dsxindexer/factors/variable_factor.py
+-rw-r--r--   0 fengming   (501) staff       (20)     3885 2023-04-10 10:33:03.000000 dsxindexer-1.1.0/src/dsxindexer/functioner.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.336147 dsxindexer-1.1.0/src/dsxindexer/operators/
+-rw-r--r--   0 fengming   (501) staff       (20)     1123 2023-03-21 07:49:41.000000 dsxindexer-1.1.0/src/dsxindexer/operators/andor_operator.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1648 2023-05-05 04:51:19.000000 dsxindexer-1.1.0/src/dsxindexer/operators/assign_operator.py
+-rw-r--r--   0 fengming   (501) staff       (20)      430 2023-03-06 15:17:57.000000 dsxindexer-1.1.0/src/dsxindexer/operators/base_operator.py
+-rw-r--r--   0 fengming   (501) staff       (20)      736 2023-03-21 08:28:46.000000 dsxindexer-1.1.0/src/dsxindexer/operators/equal_operator.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1627 2023-03-21 08:31:42.000000 dsxindexer-1.1.0/src/dsxindexer/operators/grealess_operator.py
+-rw-r--r--   0 fengming   (501) staff       (20)      859 2023-03-06 12:07:14.000000 dsxindexer-1.1.0/src/dsxindexer/operators/greaterthen_operator.py
+-rw-r--r--   0 fengming   (501) staff       (20)      651 2023-03-21 08:29:10.000000 dsxindexer-1.1.0/src/dsxindexer/operators/minus_operator.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1613 2023-03-21 08:29:14.000000 dsxindexer-1.1.0/src/dsxindexer/operators/muldiv_operator.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2061 2023-03-21 08:29:19.000000 dsxindexer-1.1.0/src/dsxindexer/operators/plusminus_operator.py
+-rw-r--r--   0 fengming   (501) staff       (20)     3952 2023-03-21 08:30:41.000000 dsxindexer-1.1.0/src/dsxindexer/parser.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.341940 dsxindexer-1.1.0/src/dsxindexer/processors/
+-rw-r--r--   0 fengming   (501) staff       (20)     2740 2023-03-14 06:41:27.000000 dsxindexer-1.1.0/src/dsxindexer/processors/base_processor.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1223 2023-03-21 08:33:35.000000 dsxindexer-1.1.0/src/dsxindexer/processors/factor_processor.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1396 2023-03-21 08:29:57.000000 dsxindexer-1.1.0/src/dsxindexer/processors/operator_processor.py
+-rw-r--r--   0 fengming   (501) staff       (20)     4893 2023-04-10 10:32:14.000000 dsxindexer-1.1.0/src/dsxindexer/processors/sindexer_processor.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.369164 dsxindexer-1.1.0/src/dsxindexer/sindexer/
+-rw-r--r--   0 fengming   (501) staff       (20)     1406 2023-03-09 13:13:56.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/BOLL.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1487 2023-03-11 08:39:03.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/BRAR.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1078 2023-03-09 08:43:51.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/CCI.py
+-rw-r--r--   0 fengming   (501) staff       (20)      673 2023-03-13 06:15:13.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/CDP.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1005 2023-03-14 02:20:52.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/CR.py
+-rw-r--r--   0 fengming   (501) staff       (20)      927 2023-03-13 09:54:40.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/DMA.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1625 2023-03-13 06:15:36.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/DMI.py
+-rw-r--r--   0 fengming   (501) staff       (20)      934 2023-03-14 02:54:37.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/EMV.py
+-rw-r--r--   0 fengming   (501) staff       (20)      827 2023-03-14 04:00:30.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/EXPMA.py
+-rw-r--r--   0 fengming   (501) staff       (20)      670 2023-03-13 06:15:46.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/KDJ.py
+-rw-r--r--   0 fengming   (501) staff       (20)      498 2023-03-13 06:15:55.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/MACD.py
+-rw-r--r--   0 fengming   (501) staff       (20)      933 2023-03-14 03:30:27.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/MIKE.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1283 2023-03-11 08:20:43.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/OBV.py
+-rw-r--r--   0 fengming   (501) staff       (20)      626 2023-03-11 08:30:35.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/PSY.py
+-rw-r--r--   0 fengming   (501) staff       (20)      983 2023-03-13 06:16:06.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/ROC.py
+-rw-r--r--   0 fengming   (501) staff       (20)      962 2023-03-13 06:16:11.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/RSI.py
+-rw-r--r--   0 fengming   (501) staff       (20)      833 2023-03-11 05:42:01.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/TRIX.py
+-rw-r--r--   0 fengming   (501) staff       (20)      670 2023-03-14 04:08:19.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/VR.py
+-rw-r--r--   0 fengming   (501) staff       (20)      612 2023-03-13 06:17:16.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/WR.py
+-rw-r--r--   0 fengming   (501) staff       (20)      571 2023-03-14 04:11:15.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/WVAD.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.372947 dsxindexer-1.1.0/src/dsxindexer/sindexer/base/
+-rw-r--r--   0 fengming   (501) staff       (20)     2416 2023-03-10 14:42:50.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/base/cons_funcs.py
+-rw-r--r--   0 fengming   (501) staff       (20)    15410 2023-05-06 04:06:20.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/base/index_funcs.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1228 2023-03-10 14:42:42.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/base/large_funcs.py
+-rw-r--r--   0 fengming   (501) staff       (20)     3797 2023-03-13 15:03:59.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/base/logical_funcs.py
+-rw-r--r--   0 fengming   (501) staff       (20)    10484 2023-03-11 08:35:45.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/base/math_funcs.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2989 2023-03-13 05:59:38.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/base/price_funcs.py
+-rw-r--r--   0 fengming   (501) staff       (20)     4908 2023-03-11 08:46:49.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/base/refer_funcs.py
+-rw-r--r--   0 fengming   (501) staff       (20)     9992 2023-03-14 06:40:43.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/base_sindexer.py
+-rw-r--r--   0 fengming   (501) staff       (20)     5703 2023-03-14 04:54:07.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/fomulas.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-05-08 08:39:17.373478 dsxindexer-1.1.0/src/dsxindexer/sindexer/models/
+-rw-r--r--   0 fengming   (501) staff       (20)      449 2023-04-05 04:59:33.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/models/kline_model.py
+-rw-r--r--   0 fengming   (501) staff       (20)      518 2023-03-14 06:41:06.000000 dsxindexer-1.1.0/src/dsxindexer/sindexer/sindexer_factory.py
+-rw-r--r--   0 fengming   (501) staff       (20)    14277 2023-03-21 08:08:51.000000 dsxindexer-1.1.0/src/dsxindexer/tokenizer.py
```

### Comparing `dsxindexer-1.0.0/LICENSE` & `dsxindexer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/PKG-INFO` & `dsxindexer-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsxindexer
-Version: 1.0.0
+Version: 1.1.0
 Summary: dsxindexer 是一个指标生成器，支持常用指标，自定义扩展指标算法，公式编辑功能
 Home-page: https://github.com/dsxkline/dsxindexer
 Author: fangyunsm
 Author-email: fangyunsm <934476300@qq.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/dsxkline/dsxindexer
 Project-URL: Bug Tracker, https://github.com/dsxkline/dsxindexer/issues
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dsxindexer
- 量化指标公式编辑器框架,目前支持部分通达信公式，因为公式太多，所以慢慢完善中，有兴趣的朋友可以自己实现哦。
+ 基于麦语言的量化指标公式编辑器框架,目前支持部分通达信公式，因为公式太多，所以慢慢完善中，有兴趣的朋友可以自己实现哦。
 
 ## 安装
 
 ```
 pip install dsxindexer
 ```
```

### Comparing `dsxindexer-1.0.0/README.md` & `dsxindexer-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # dsxindexer
- 量化指标公式编辑器框架,目前支持部分通达信公式，因为公式太多，所以慢慢完善中，有兴趣的朋友可以自己实现哦。
+ 基于麦语言的量化指标公式编辑器框架,目前支持部分通达信公式，因为公式太多，所以慢慢完善中，有兴趣的朋友可以自己实现哦。
 
 ## 安装
 
 ```
 pip install dsxindexer
 ```
```

### Comparing `dsxindexer-1.0.0/dsxindexer.egg-info/PKG-INFO` & `dsxindexer-1.1.0/dsxindexer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsxindexer
-Version: 1.0.0
+Version: 1.1.0
 Summary: dsxindexer 是一个指标生成器，支持常用指标，自定义扩展指标算法，公式编辑功能
 Home-page: https://github.com/dsxkline/dsxindexer
 Author: fangyunsm
 Author-email: fangyunsm <934476300@qq.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/dsxkline/dsxindexer
 Project-URL: Bug Tracker, https://github.com/dsxkline/dsxindexer/issues
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dsxindexer
- 量化指标公式编辑器框架,目前支持部分通达信公式，因为公式太多，所以慢慢完善中，有兴趣的朋友可以自己实现哦。
+ 基于麦语言的量化指标公式编辑器框架,目前支持部分通达信公式，因为公式太多，所以慢慢完善中，有兴趣的朋友可以自己实现哦。
 
 ## 安装
 
 ```
 pip install dsxindexer
 ```
```

### Comparing `dsxindexer-1.0.0/dsxindexer.egg-info/SOURCES.txt` & `dsxindexer-1.1.0/dsxindexer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 dsxindexer.egg-info/PKG-INFO
 dsxindexer.egg-info/SOURCES.txt
 dsxindexer.egg-info/dependency_links.txt
 dsxindexer.egg-info/not-zip-safe
+dsxindexer.egg-info/requires.txt
 dsxindexer.egg-info/top_level.txt
 src/dsxindexer/__init__.py
 src/dsxindexer/configer.py
 src/dsxindexer/functioner.py
 src/dsxindexer/parser.py
 src/dsxindexer/tokenizer.py
 src/dsxindexer/factors/base_factor.py
```

### Comparing `dsxindexer-1.0.0/pyproject.toml` & `dsxindexer-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dsxindexer"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="fangyunsm", email="934476300@qq.com" },
 ]
 description = "dsxindexer 是一个指标生成器，支持常用指标，自定义扩展指标算法，公式编辑功能"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dsxindexer-1.0.0/setup.py` & `dsxindexer-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,28 @@
     with open('README.md', encoding='utf-8') as f:
         content = f.read()
     return content
 
 
 setup(
     name="dsxindexer",  # 包名称
-    version="1.0.0",  # 版本号
+    version="1.1.0",  # 版本号
     author="fangyunsm",  # 作者
     author_email="934476300@qq.com",  # 作者邮箱
-    description="dsxindexer 是一个指标生成器，支持常用指标，自定义扩展指标算法，公式编辑功能",  # 描述
+    description="dsxindexer 是一个基于麦语言的指标生成器，支持常用指标，自定义扩展指标算法，公式编辑功能",  # 描述
     long_description=readme(),  # 长文描述
     keywords="通达信指标,公式编辑器,量化指标",  # 项目关键词
     url="https://github.com/dsxkline/dsxindexer",  # 项目主页
     license="MIT License",  # 许可证
     # packages=find_namespace_packages('pydsxkline'),
     zip_safe=False,
     packages=['dsxindexer'],
     package_dir={"dsxindexer": "src/dsxindexer"},
     include_package_data=True,
     # package_data={"": ['*.py', '*.js', '*.html']},
-    # install_requires=['pywebview'],
+    install_requires=[
+        "dsxquant>=2.1.0",
+        "numba==0.56.4",
+        "progressbar33==2.4"
+    ],
     python_requires='>=3.6,<4'
 )
```

### Comparing `dsxindexer-1.0.0/src/dsxindexer/__init__.py` & `dsxindexer-1.1.0/src/dsxindexer/__init__.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/configer.py` & `dsxindexer-1.1.0/src/dsxindexer/configer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging,logging.config
+import os
 DEBUG = False
 if DEBUG:
     LOGLEVEL = logging.DEBUG
 else:
     LOGLEVEL = logging.INFO
 logger = logging.getLogger("dsxindexer")  # 生成一个log实例
 handle = logging.StreamHandler()
@@ -94,15 +95,18 @@
 class ExpreItemDirection:
     DEFAULT = 0
     LEFT = 1
     RIGHT = 2
 
 class Cursor:
     index:int = 0
+    count:int = 0
     
 # 表达式结束符
 EXPR_END_CHART = ";"
 # 赋值符号
 ASSIGN_CHART = ":="
 # 注释符 开始和结束标签
 ANNOTATION_CHART = ("#","\n")
 ANNOTATION_CHART_OTHER = ("{","}")
+# 缓存地址
+CACHE_PATH = os.path.dirname(os.path.abspath(__file__))+"/caches"
```

### Comparing `dsxindexer-1.0.0/src/dsxindexer/factors/lparen_factor.py` & `dsxindexer-1.1.0/src/dsxindexer/factors/lparen_factor.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/factors/string_factor.py` & `dsxindexer-1.1.0/src/dsxindexer/factors/string_factor.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/factors/variable_factor.py` & `dsxindexer-1.1.0/src/dsxindexer/factors/variable_factor.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/functioner.py` & `dsxindexer-1.1.0/src/dsxindexer/functioner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import hashlib
 import re
 import threading
-from dsxindexer.configer import logger
+from dsxindexer.configer import Cursor, logger
 
 # def singleton(cls):
 #     instances = {}
 #     def get_instance(*args, **kwargs):
 #         if cls not in instances:
 #             instances[cls] = cls(*args, **kwargs)
 #         return instances[cls]
@@ -17,15 +18,20 @@
         with func.__lock__:
             return func(*args, **kwargs)
 
     return wrapper
 
 # @singleton
 class Functioner:
-    def __init__(self) -> None:
+    def __init__(self,klines:list=None,symbol:str=None,market:int=None,cursor:Cursor=None,enable_cache:bool=True) -> None:
+        self.klines = klines
+        self.symbol = symbol
+        self.market = market
+        self.cursor = cursor
+        self.enable_cache = enable_cache
         self.function_exs = []
         self.variables = {}
         pass
     
     def register(self,cls):
         if cls not in self.function_exs:
             self.function_exs.append(cls)
@@ -52,14 +58,18 @@
 
     def MIN(self,a,b):
         return min(a,b)
     
     def ABS(self,a):
         return abs(a)
     
+    def MD5(self,s:str):
+        md5 = hashlib.md5(s.encode('utf-8')).hexdigest()
+        return md5
+    
 
     @synchronized
     def set_value(self,namespace:str,name:str,value:any,func_name:str=None):
         """保存变量值
 
         Args:
             namespace (str): 命名空间
```

### Comparing `dsxindexer-1.0.0/src/dsxindexer/operators/andor_operator.py` & `dsxindexer-1.1.0/src/dsxindexer/operators/andor_operator.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/operators/assign_operator.py` & `dsxindexer-1.1.0/src/dsxindexer/operators/assign_operator.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,28 +13,29 @@
             token = self.token
             if self.token.export:
                 self.parser.export.append(self.parser.last_avariable)
             variable = self.parser.last_avariable
             expre = self.token.value
             self.parser.eat(self.token.type)
             # 开始处理右边表达式的值
-            result = self.parser_equal(expre)
+            result = self.parser_equal(expre,variable)
             logger.debug("正则赋值 %s=%s" % (variable,result))
             # 给变量赋值
             self.parser.funcer.set_value(self.parser.namespace,variable,result,self.parser.func_name)
             # 继续下一个项
             rs = self.parser.term()
             if rs!=None:
                 result = rs
         return result
     
-    def parser_equal(self,expre):
+    def parser_equal(self,expre,variable):
         """解析等号右边表达式"""
         from dsxindexer.tokenizer import Lexer
         from dsxindexer.parser import Parser
         # 词法分析器
         lexer = Lexer(expre,ExpreItemDirection.RIGHT,self.token.location[0])
         # 语法解析器
         parser = Parser(lexer,self.parser.funcer,self.parser.namespace,func_name=self.parser.func_name)
+        parser.last_avariable = variable
         # 解析并返回结果
         ps = parser.parse()
         return ps.result
```

### Comparing `dsxindexer-1.0.0/src/dsxindexer/operators/equal_operator.py` & `dsxindexer-1.1.0/src/dsxindexer/operators/equal_operator.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/operators/grealess_operator.py` & `dsxindexer-1.1.0/src/dsxindexer/operators/grealess_operator.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/operators/greaterthen_operator.py` & `dsxindexer-1.1.0/src/dsxindexer/operators/greaterthen_operator.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/operators/minus_operator.py` & `dsxindexer-1.1.0/src/dsxindexer/operators/minus_operator.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/operators/muldiv_operator.py` & `dsxindexer-1.1.0/src/dsxindexer/operators/muldiv_operator.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/operators/plusminus_operator.py` & `dsxindexer-1.1.0/src/dsxindexer/operators/plusminus_operator.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/parser.py` & `dsxindexer-1.1.0/src/dsxindexer/parser.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/processors/base_processor.py` & `dsxindexer-1.1.0/src/dsxindexer/processors/base_processor.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/processors/factor_processor.py` & `dsxindexer-1.1.0/src/dsxindexer/processors/factor_processor.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/processors/operator_processor.py` & `dsxindexer-1.1.0/src/dsxindexer/processors/operator_processor.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/processors/sindexer_processor.py` & `dsxindexer-1.1.0/src/dsxindexer/processors/sindexer_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from concurrent.futures import ThreadPoolExecutor,wait,as_completed
 import datetime
 import time
 import types
-
 from dsxindexer.configer import Cursor,logger
 from dsxindexer.sindexer.fomulas import Formulas
 from dsxindexer.sindexer.models.kline_model import KlineModel
 from dsxindexer.parser import Parser
 from dsxindexer.tokenizer import Lexer
 from dsxindexer.functioner import Functioner
 from dsxindexer.processors.base_processor import BaseProcessor
 from dsxindexer.sindexer.base_sindexer import BaseSindexer
 from typing import List
 from progressbar import ProgressBar
+from numba import njit
+
 class SindexerProcessor(BaseProcessor):
 
     # 内置一些底层函数，如果是通过指标记录编写的可以在这里初始化注册
     __processors:List[BaseProcessor]=[
     ]
    
 
-    def __init__(self,klines:list=None) -> None:
+    def __init__(self,klines:list=None,symbol:str=None,market:int=None,enable_cache:bool=True) -> None:
          # 自定义注册指标函数
         self.processors:List[BaseSindexer] = [
             
         ]
         # k线数据
         self.klines:List[KlineModel] = self.cover_to_model(klines)
         # 当前游标
         self.cursor = Cursor()
+        self.cursor.count = self.klines.__len__()
+        self.symbol = symbol
+        self.market = market
         # 初始化一个函数库，集成了函数和内存空间
-        self.functioner = Functioner()
-        pass
+        self.functioner = Functioner(self.klines,self.symbol,self.market,self.cursor,enable_cache)
+        
     
     def cover_to_model(self,klines:list):
         newklines = []
         if klines:
             for item in klines:
                 d,o,h,l,c,v,a = type(item)==list and item or item.split(",")
                 date = self.get_date(d)
@@ -64,24 +68,35 @@
             return datetime.datetime.strptime(date+" 15:00:00","%Y%m%d %H:%M:%S")
         # 分钟线时间格式 
         if len(date)==12:
             return datetime.datetime.strptime(date,"%Y%m%d%H%M")
     
     def next(self):
         self.cursor.index += 1
+        self.cursor.count = self.klines.__len__()
     
     def execute(self):
         t = time.time()
         # 把指标公式都注册进解析器函数库
         self.regs()
         # executor = ThreadPoolExecutor(max_workers=self.processors.__len__())
-        pbar = ProgressBar(self.klines.__len__())
+        
+        self.execute_action(self.klines,self.processors)
+        # executor.shutdown()
+        t = time.time() - t
+        logger.info("编译用时:%s s" % t)
+        return self.klines
+    
+    # @njit
+    def execute_action(self,klines,processors):
+        # i = 0
+        pbar:ProgressBar = ProgressBar(self.klines.__len__())
         pbar.start()
-        i = 0
-        for item in self.klines:
+        for i in range(self.klines.__len__()):
+            item = self.klines[i]
             # 计算所有注册指标
             # futures = []
             # for sindexer in self.processors:
             #     # 得到指标的值
             #     future = executor.submit(sindexer.execute)
             #     setattr(future,"__typename__",sindexer.__typename__)
             #     futures.append(future)
@@ -91,22 +106,19 @@
             #     if result:
             #         setattr(item,future.__typename__,result)
             
             for sindexer in self.processors:
                 # 得到指标的值
                 result = sindexer.execute()
                 if result!=None:
+                    # item.setvalue(sindexer.__typename__,result)
                     setattr(item,sindexer.__typename__,result)
             self.next()
             pbar.update(i)
-            i += 1
-        # executor.shutdown()
-        t = time.time() - t
-        # logger.info("编译用时:%s s" % t)
-        return self.klines
+            # i += 1
 
     def regs(self):
         # 给自定义指标注册基础函数
         for cls in self.__processors:
             obj:BaseSindexer = cls(self.klines,self.cursor)
             obj.set_functioner(self.functioner)
             # self.functioner.register(obj)
```

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/BOLL.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/BOLL.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/BRAR.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/BRAR.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/CCI.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/CCI.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/CDP.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/CDP.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/CR.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/CR.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/DMA.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/DMA.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/DMI.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/DMI.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/EMV.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/EMV.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/EXPMA.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/EXPMA.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/KDJ.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/KDJ.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/MIKE.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/MIKE.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/OBV.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/OBV.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/PSY.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/PSY.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/ROC.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/ROC.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/RSI.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/RSI.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/TRIX.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/TRIX.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/VR.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/VR.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/WR.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/WR.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/WVAD.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/WVAD.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/base/cons_funcs.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/base/cons_funcs.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/base/index_funcs.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/base/index_funcs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """指标函数(PEAK、SAR、COSET、WINNER、ZIG等)
 """
 
+import math
 from dsxindexer.configer import DSX_FIELD_STR
 from dsxindexer.sindexer.base_sindexer import BaseSindexer
 
 def MA(self:BaseSindexer,X:DSX_FIELD_STR="CLOSE",N=5):
     """MA指标是英文(Moving average)的简写，叫移动平均线指标。
     1.N日MA=N日收市价的总和/N(即算术平均数)
     
@@ -276,20 +277,122 @@
     """
 
 def ZIG(self:BaseSindexer,K:int,N:float):
     """之字转向 属于未来函数
     ZIG(K,N),当价格变化量超过N%时转向,K表示0:开盘价,1:最高价,2:最低价,3:收盘价
     ZIG(3,5)表示收盘价的5%的ZIG转向
     """
+    zig = None
+    # 计算过程缓存
+    key = "zig_%s_%s_" % (K,N)
+    CLOSE = "CLOSE"
+    if K==0: CLOSE = "OPEN"
+    if K==1: CLOSE = "HIGH"
+    if K==2: CLOSE = "LOW"
+    if K==3: CLOSE = "CLOSE"
+    # 当前值
+    value = self.GET(CLOSE)
+    # 上一个低点
+    zig_low = self.REF(key+"low")
+    if not zig_low:zig_low = value
+    # 上一个高点
+    zig_high = self.REF(key+"high")
+    if not zig_high:zig_high = value
+    # 上一个低点位置
+    zig_low_day = self.REF(key+"low_day")
+    if zig_low_day==None:zig_low_day = self.cursor.index
+    # 上一个高点位置
+    zig_high_day = self.REF(key+"high_day")
+    if zig_high_day==None:zig_high_day = self.cursor.index
+    # 默认继承
+    self.save_temp(key+"low",zig_low)
+    self.save_temp(key+"high",zig_high)
+    self.save_temp(key+"high_day",zig_high_day)
+    self.save_temp(key+"low_day",zig_low_day)
+    
+    # 极点阀值，计算跟上一个低点的阀值
+    fz = 100 * (value - zig_low) / zig_low
+    # 如果极点阀值大于N，这个是高点
+    if fz>=N:
+        zig_max = self.HHV(CLOSE, self.cursor.index-zig_low_day);
+        if value>=zig_max:
+            # 更新中间的zig值
+            self.__ZIG(CLOSE,zig_low_day,1)
+            # 更新极点
+            zig = value
+            self.save_temp(key+"high",value)
+            self.save_temp(key+"high_day",self.cursor.index)
+        
+    # 低点阀值
+    fz = 100 * (value - zig_high) / zig_high
+    if fz<=-N:
+        zig_min = self.LLV(CLOSE, self.cursor.index-zig_high_day)
+        if value<=zig_min:
+            # 更新中间的zig值
+            self.__ZIG(CLOSE,zig_high_day,0)
+            # 更新极点
+            zig = value
+            self.save_temp(key+"low",value)
+            self.save_temp(key+"low_day",self.cursor.index)
+
+    # 最新一个k线值
+    if(self.cursor.index==self.cursor.count-1):
+        # 高点延续
+        if zig_high_day>zig_low_day:
+            # 更新中间的zig值
+            self.__ZIG(CLOSE,zig_high_day,0)
+            # 更新极点
+            zig = value
+            self.save_temp(key+"low",value)
+            self.save_temp(key+"low_day",self.cursor.index)
+        else:
+            # 更新中间的zig值
+            self.__ZIG(CLOSE,zig_low_day,1)
+            # 更新极点
+            zig = value
+            self.save_temp(key+"high",value)
+            self.save_temp(key+"high_day",self.cursor.index)
+    
+    return zig
+       
+    
+def __ZIG(self:BaseSindexer,CLOSE,day,type=0):
+    # 计算斜边长度
+    first_value = self.GET(CLOSE,day)
+    a = self.cursor.index - day
+    b = first_value - self.GET(CLOSE)
+    if(type>0):
+        # 低到高
+        b = self.GET(CLOSE) - first_value
+    c = math.sqrt(a*a + b*b)
+    # 计算b边长对向的角度,后面根据角度即可计算斜线c
+    thetb = math.acos(a / c) * 180 / math.pi
+    # 之前的低点位置全部为空
+    for i in range(self.cursor.index-1,day,-1):
+        a = i - day
+        c = a / math.cos(thetb * math.pi / 180)
+        b = first_value - math.sqrt(c ** 2 - a ** 2)
+        if(type>0):
+            b = first_value + math.sqrt(c ** 2 - a ** 2)
+        # 更新之前的ZIG指标值
+        subitem = self.klines[i]
+        if hasattr(subitem,self.namespace):
+            namespace = getattr(subitem,self.namespace)
+            if namespace and self.variable_name:
+                if hasattr(namespace,self.variable_name):
+                    setattr(namespace,self.variable_name,b)
+        
+
+
 def ZIGA(self:BaseSindexer,K:int,N:float):
     """反向之字转向 属于未来函数
     用法:
     ZIGA(K,X),当价格变化超过X时转向,K表示0:开盘价,1:最高价,2:最低价,3:收盘价,其余:数组信息
     例如:
-    ZIGA(3,1.5)表示收盘价变化1.5元的ZIGA转向
+    ZIGA(3,1.5)表示收盘价变化1.5%的ZIGA转向
     """
 
 def COSTEX(self:BaseSindexer,A:DSX_FIELD_STR,B:DSX_FIELD_STR):
     """区间成本
     COSTEX(A,B),表示两日收盘价格间筹码的成本
     COSTEX(CLOSE,REF(CLOSE)),表示近两日收盘价格间筹码的成本.返回10表示区间成本为10元.
     """
```

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/base/large_funcs.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/base/large_funcs.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/base/logical_funcs.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/base/logical_funcs.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/base/math_funcs.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/base/math_funcs.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/base/price_funcs.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/base/price_funcs.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/base/refer_funcs.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/base/refer_funcs.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/base_sindexer.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/base_sindexer.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/fomulas.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/fomulas.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/sindexer/sindexer_factory.py` & `dsxindexer-1.1.0/src/dsxindexer/sindexer/sindexer_factory.py`

 * *Files identical despite different names*

### Comparing `dsxindexer-1.0.0/src/dsxindexer/tokenizer.py` & `dsxindexer-1.1.0/src/dsxindexer/tokenizer.py`

 * *Files identical despite different names*

