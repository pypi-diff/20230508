# Comparing `tmp/adata-0.0.8b0.tar.gz` & `tmp/adata-0.0.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata-0.0.8b0.tar", last modified: Fri May  5 15:18:33 2023, max compression
+gzip compressed data, was "adata-0.0.9b0.tar", last modified: Sat May  6 10:41:11 2023, max compression
```

## Comparing `adata-0.0.8b0.tar` & `adata-0.0.9b0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.368432 adata-0.0.8b0/
--rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.8b0/HISTORY.md
--rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.8b0/LICENSE
--rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.8b0/MANIFEST.in
--rw-rw-rw-   0        0        0     7151 2023-05-05 15:18:33.368432 adata-0.0.8b0/PKG-INFO
--rw-rw-rw-   0        0        0     6512 2023-04-25 16:01:44.000000 adata-0.0.8b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.288433 adata-0.0.8b0/adata/
--rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.8b0/adata/__init__.py
--rw-rw-rw-   0        0        0      756 2023-05-05 15:18:30.000000 adata-0.0.8b0/adata/__version__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.298432 adata-0.0.8b0/adata/bond/
--rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.8b0/adata/bond/__init__.py
--rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.8b0/adata/bond/bond_market.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.308432 adata-0.0.8b0/adata/common/
--rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.8b0/adata/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.308432 adata-0.0.8b0/adata/common/headers/
--rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.8b0/adata/common/headers/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.8b0/adata/common/headers/baidu_headers.py
--rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.8b0/adata/common/headers/sina_headers.py
--rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.8b0/adata/common/headers/ths_headers.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.318432 adata-0.0.8b0/adata/common/js/
--rw-rw-rw-   0        0        0       99 2023-05-05 13:46:05.000000 adata-0.0.8b0/adata/common/js/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.328435 adata-0.0.8b0/adata/common/utils/
--rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.8b0/adata/common/utils/__init__.py
--rw-rw-rw-   0        0        0      753 2023-05-05 13:46:05.000000 adata-0.0.8b0/adata/common/utils/cookie.py
--rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.8b0/adata/common/utils/snowflake.py
--rw-rw-rw-   0        0        0      979 2023-04-24 16:42:55.000000 adata-0.0.8b0/adata/common/utils/sunrequests.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.328435 adata-0.0.8b0/adata/etf/
--rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.8b0/adata/etf/__init__.py
--rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.8b0/adata/etf/etf_market.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.338432 adata-0.0.8b0/adata/message/
--rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.8b0/adata/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.338432 adata-0.0.8b0/adata/stock/
--rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.8b0/adata/stock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.338432 adata-0.0.8b0/adata/stock/index/
--rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.8b0/adata/stock/index/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.348432 adata-0.0.8b0/adata/stock/info/
--rw-rw-rw-   0        0        0      380 2023-05-05 13:46:05.000000 adata-0.0.8b0/adata/stock/info/__init__.py
--rw-rw-rw-   0        0        0     2550 2023-04-25 15:29:33.000000 adata-0.0.8b0/adata/stock/info/stock_code.py
--rw-rw-rw-   0        0        0     6720 2023-05-05 15:18:22.000000 adata-0.0.8b0/adata/stock/info/stock_concept.py
--rw-rw-rw-   0        0        0     2027 2023-05-05 14:11:27.000000 adata-0.0.8b0/adata/stock/info/trade_calendar.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.358432 adata-0.0.8b0/adata/stock/market/
--rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.8b0/adata/stock/market/__init__.py
--rw-rw-rw-   0        0        0     2941 2023-04-20 13:03:47.000000 adata-0.0.8b0/adata/stock/market/stock_dividend.py
--rw-rw-rw-   0        0        0    10485 2023-04-25 15:43:53.000000 adata-0.0.8b0/adata/stock/market/stock_market.py
--rw-rw-rw-   0        0        0     8363 2023-04-25 15:49:26.000000 adata-0.0.8b0/adata/stock/market/stock_market_concept.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.358432 adata-0.0.8b0/adata/stock/sentiment/
--rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.8b0/adata/stock/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:18:33.298432 adata-0.0.8b0/adata.egg-info/
--rw-rw-rw-   0        0        0     7151 2023-05-05 15:18:33.000000 adata-0.0.8b0/adata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2023-05-05 15:18:33.000000 adata-0.0.8b0/adata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 15:18:33.000000 adata-0.0.8b0/adata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-05 15:18:33.000000 adata-0.0.8b0/adata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 15:18:33.000000 adata-0.0.8b0/adata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-05-05 13:46:05.000000 adata-0.0.8b0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 15:18:33.368432 adata-0.0.8b0/setup.cfg
--rw-rw-rw-   0        0        0     1819 2023-05-05 15:09:50.000000 adata-0.0.8b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:11.023979 adata-0.0.9b0/
+-rw-rw-rw-   0        0        0      186 2023-04-07 05:48:39.000000 adata-0.0.9b0/HISTORY.md
+-rw-rw-rw-   0        0        0    11558 2023-04-07 05:48:39.000000 adata-0.0.9b0/LICENSE
+-rw-rw-rw-   0        0        0       41 2023-05-06 10:39:00.000000 adata-0.0.9b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7274 2023-05-06 10:41:11.022979 adata-0.0.9b0/PKG-INFO
+-rw-rw-rw-   0        0        0     6635 2023-05-06 06:40:35.000000 adata-0.0.9b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:10.974976 adata-0.0.9b0/adata/
+-rw-rw-rw-   0        0        0      545 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/__init__.py
+-rw-rw-rw-   0        0        0      756 2023-05-06 10:39:46.000000 adata-0.0.9b0/adata/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:10.985980 adata-0.0.9b0/adata/bond/
+-rw-rw-rw-   0        0        0      122 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/bond/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/bond/bond_market.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:10.986979 adata-0.0.9b0/adata/common/
+-rw-rw-rw-   0        0        0      150 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:10.989979 adata-0.0.9b0/adata/common/headers/
+-rw-rw-rw-   0        0        0      104 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/common/headers/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/common/headers/baidu_headers.py
+-rw-rw-rw-   0        0        0      602 2023-04-18 11:18:06.000000 adata-0.0.9b0/adata/common/headers/sina_headers.py
+-rw-rw-rw-   0        0        0     2999 2023-05-05 10:41:12.000000 adata-0.0.9b0/adata/common/headers/ths_headers.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:10.990980 adata-0.0.9b0/adata/common/js/
+-rw-rw-rw-   0        0        0       99 2023-05-05 10:05:38.000000 adata-0.0.9b0/adata/common/js/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:11.003978 adata-0.0.9b0/adata/common/utils/
+-rw-rw-rw-   0        0        0      205 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/common/utils/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-05-05 10:49:50.000000 adata-0.0.9b0/adata/common/utils/cookie.py
+-rw-rw-rw-   0        0        0     3046 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/common/utils/snowflake.py
+-rw-rw-rw-   0        0        0      979 2023-05-05 03:38:48.000000 adata-0.0.9b0/adata/common/utils/sunrequests.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:11.009981 adata-0.0.9b0/adata/etf/
+-rw-rw-rw-   0        0        0      118 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/etf/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/etf/etf_market.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:11.010976 adata-0.0.9b0/adata/message/
+-rw-rw-rw-   0        0        0      103 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:11.012979 adata-0.0.9b0/adata/stock/
+-rw-rw-rw-   0        0        0      333 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/stock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:11.012979 adata-0.0.9b0/adata/stock/index/
+-rw-rw-rw-   0        0        0      105 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/stock/index/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:11.016976 adata-0.0.9b0/adata/stock/info/
+-rw-rw-rw-   0        0        0      380 2023-05-05 08:46:59.000000 adata-0.0.9b0/adata/stock/info/__init__.py
+-rw-rw-rw-   0        0        0     2550 2023-05-05 03:38:48.000000 adata-0.0.9b0/adata/stock/info/stock_code.py
+-rw-rw-rw-   0        0        0     6908 2023-05-06 08:50:25.000000 adata-0.0.9b0/adata/stock/info/stock_concept.py
+-rw-rw-rw-   0        0        0     2027 2023-05-06 06:40:35.000000 adata-0.0.9b0/adata/stock/info/trade_calendar.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:11.020981 adata-0.0.9b0/adata/stock/market/
+-rw-rw-rw-   0        0        0      408 2023-04-18 01:39:18.000000 adata-0.0.9b0/adata/stock/market/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-04-23 03:30:14.000000 adata-0.0.9b0/adata/stock/market/stock_dividend.py
+-rw-rw-rw-   0        0        0    10485 2023-05-05 03:38:48.000000 adata-0.0.9b0/adata/stock/market/stock_market.py
+-rw-rw-rw-   0        0        0     8363 2023-05-05 03:38:48.000000 adata-0.0.9b0/adata/stock/market/stock_market_concept.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:11.021977 adata-0.0.9b0/adata/stock/sentiment/
+-rw-rw-rw-   0        0        0      115 2023-04-07 05:48:39.000000 adata-0.0.9b0/adata/stock/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:41:10.983978 adata-0.0.9b0/adata.egg-info/
+-rw-rw-rw-   0        0        0     7274 2023-05-06 10:41:10.000000 adata-0.0.9b0/adata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2023-05-06 10:41:10.000000 adata-0.0.9b0/adata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 10:41:10.000000 adata-0.0.9b0/adata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-06 10:41:10.000000 adata-0.0.9b0/adata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 10:41:10.000000 adata-0.0.9b0/adata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-05-05 10:31:46.000000 adata-0.0.9b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 10:41:11.023979 adata-0.0.9b0/setup.cfg
+-rw-rw-rw-   0        0        0     1819 2023-05-06 06:40:35.000000 adata-0.0.9b0/setup.py
```

### Comparing `adata-0.0.8b0/LICENSE` & `adata-0.0.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/PKG-INFO` & `adata-0.0.9b0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: adata
-Version: 0.0.8b0
-Summary: A Data,A Stock,ETF,Bond,Quant
-Home-page: https://gitee.com/inchaos/adata
-Author: 1nchaos
-Author-email: 9527@1nchaos.com
-License: Apache License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # A Data
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/master/LICENSE)
 
 
 ## 0、介绍
 免费开源A股数据库，专注量化，向阳而生。
@@ -82,19 +64,20 @@
 
 整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
 
 ### （1）股票-Stock
 
 #### 	1. 基本信息
 
-| 数据         | API                                  | 说明                             | 备注                 |
-| ------------ | ------------------------------------ | -------------------------------- | -------------------- |
-| A股代码      | stock.info.all_code()                | 所有A股代码信息                  |                      |
-| 概念代码     | stock.info.all_concept_code_ths()    | 所有A股概念代码信息（同花顺）app | 来源：同花顺公开数据 |
-| 概念成分列表 | stock.info.concept_constituent_ths() | 获取概念的成分股                 |                      |
+| 数据         | API                                  | 说明                          | 备注                 |
+| ------------ | ------------------------------------ | ----------------------------- | -------------------- |
+| A股代码      | stock.info.all_code()                | 所有A股代码信息               |                      |
+| 概念代码     | stock.info.all_concept_code_ths()    | 所有A股概念代码信息（同花顺） | 来源：同花顺公开数据 |
+| 概念成分列表 | stock.info.concept_constituent_ths() | 获取同花顺概念指数的成分股    |                      |
+| 股票交易日历 | stock.info.trade_calendar()          | 获取股票交易日信息            | 来源：深交所         |
 
 #### 	2. 行情信息
 
 | 数据     | API                                         | 说明                                  | 备注                   |
 | -------- | ------------------------------------------- | ------------------------------------- | ---------------------- |
 | 分红信息 | stock.maket.get_dividend()                  | 获取单只股票的分红信息                |                        |
 | 股票行情 | stock.market.get_market()                   | 获取单只股票的行情信息-日、周、月 k线 |                        |
```

### Comparing `adata-0.0.8b0/README.md` & `adata-0.0.9b0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: adata
+Version: 0.0.9b0
+Summary: A Data,A Stock,ETF,Bond,Quant
+Home-page: https://gitee.com/inchaos/adata
+Author: 1nchaos
+Author-email: 9527@1nchaos.com
+License: Apache License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # A Data
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/master/LICENSE)
 
 
 ## 0、介绍
 免费开源A股数据库，专注量化，向阳而生。
@@ -64,19 +82,20 @@
 
 整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
 
 ### （1）股票-Stock
 
 #### 	1. 基本信息
 
-| 数据         | API                                  | 说明                             | 备注                 |
-| ------------ | ------------------------------------ | -------------------------------- | -------------------- |
-| A股代码      | stock.info.all_code()                | 所有A股代码信息                  |                      |
-| 概念代码     | stock.info.all_concept_code_ths()    | 所有A股概念代码信息（同花顺）app | 来源：同花顺公开数据 |
-| 概念成分列表 | stock.info.concept_constituent_ths() | 获取概念的成分股                 |                      |
+| 数据         | API                                  | 说明                          | 备注                 |
+| ------------ | ------------------------------------ | ----------------------------- | -------------------- |
+| A股代码      | stock.info.all_code()                | 所有A股代码信息               |                      |
+| 概念代码     | stock.info.all_concept_code_ths()    | 所有A股概念代码信息（同花顺） | 来源：同花顺公开数据 |
+| 概念成分列表 | stock.info.concept_constituent_ths() | 获取同花顺概念指数的成分股    |                      |
+| 股票交易日历 | stock.info.trade_calendar()          | 获取股票交易日信息            | 来源：深交所         |
 
 #### 	2. 行情信息
 
 | 数据     | API                                         | 说明                                  | 备注                   |
 | -------- | ------------------------------------------- | ------------------------------------- | ---------------------- |
 | 分红信息 | stock.maket.get_dividend()                  | 获取单只股票的分红信息                |                        |
 | 股票行情 | stock.market.get_market()                   | 获取单只股票的行情信息-日、周、月 k线 |                        |
```

### Comparing `adata-0.0.8b0/adata/__init__.py` & `adata-0.0.9b0/adata/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/__version__.py` & `adata-0.0.9b0/adata/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-VERSION = (0, 0, 8)
+VERSION = (0, 0, 9)
 # PRERELEASE = None  # alpha, beta or rc
 PRERELEASE = 'beta'  # alpha, beta or rc
 REVISION = None
 
 
 def generate_version(version, prerelease=None, revision=None):
     version_parts = [".".join(map(str, version))]
```

### Comparing `adata-0.0.8b0/adata/common/headers/baidu_headers.py` & `adata-0.0.9b0/adata/common/headers/baidu_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/common/headers/sina_headers.py` & `adata-0.0.9b0/adata/common/headers/sina_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/common/headers/ths_headers.py` & `adata-0.0.9b0/adata/common/headers/ths_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/common/utils/cookie.py` & `adata-0.0.9b0/adata/common/utils/cookie.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/common/utils/snowflake.py` & `adata-0.0.9b0/adata/common/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/common/utils/sunrequests.py` & `adata-0.0.9b0/adata/common/utils/sunrequests.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/stock/info/stock_code.py` & `adata-0.0.9b0/adata/stock/info/stock_code.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/stock/info/stock_concept.py` & `adata-0.0.9b0/adata/stock/info/stock_concept.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,15 @@
                                                                                             ignore_index=True)
         return data_df
 
     def concept_constituent_ths(self, concept_code=None):
         """
         同花顺概念成分股
         web_url :http://q.10jqka.com.cn/gn/detail/field/199112/order/desc/page/1/ajax/1/code/301539
+        TODO:http://www.iwencai.com/gateway/urp/v7/landing/getDataList?query=chatgpt%20%E6%A6%82%E5%BF%B5%E6%88%90%E5%88%86&page=1&perpage=100&query_type=stock&comp_id=6734520&uuid=24087
         :param concept_code: 概念代码： 301539
         :return:['concept_code', 'stock_code', 'short_name']
         """
         # 1. url，拼接月份
         data = []
         for i in tqdm(range(258)):
             api_url = f"http://q.10jqka.com.cn/gn/detail/field/199112/order/desc/page/{i + 1}/ajax/1/code/{concept_code}"
```

### Comparing `adata-0.0.8b0/adata/stock/info/trade_calendar.py` & `adata-0.0.9b0/adata/stock/info/trade_calendar.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/stock/market/stock_dividend.py` & `adata-0.0.9b0/adata/stock/market/stock_dividend.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/stock/market/stock_market.py` & `adata-0.0.9b0/adata/stock/market/stock_market.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata/stock/market/stock_market_concept.py` & `adata-0.0.9b0/adata/stock/market/stock_market_concept.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/adata.egg-info/PKG-INFO` & `adata-0.0.9b0/adata.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 0.0.8b0
+Version: 0.0.9b0
 Summary: A Data,A Stock,ETF,Bond,Quant
 Home-page: https://gitee.com/inchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -82,19 +82,20 @@
 
 整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
 
 ### （1）股票-Stock
 
 #### 	1. 基本信息
 
-| 数据         | API                                  | 说明                             | 备注                 |
-| ------------ | ------------------------------------ | -------------------------------- | -------------------- |
-| A股代码      | stock.info.all_code()                | 所有A股代码信息                  |                      |
-| 概念代码     | stock.info.all_concept_code_ths()    | 所有A股概念代码信息（同花顺）app | 来源：同花顺公开数据 |
-| 概念成分列表 | stock.info.concept_constituent_ths() | 获取概念的成分股                 |                      |
+| 数据         | API                                  | 说明                          | 备注                 |
+| ------------ | ------------------------------------ | ----------------------------- | -------------------- |
+| A股代码      | stock.info.all_code()                | 所有A股代码信息               |                      |
+| 概念代码     | stock.info.all_concept_code_ths()    | 所有A股概念代码信息（同花顺） | 来源：同花顺公开数据 |
+| 概念成分列表 | stock.info.concept_constituent_ths() | 获取同花顺概念指数的成分股    |                      |
+| 股票交易日历 | stock.info.trade_calendar()          | 获取股票交易日信息            | 来源：深交所         |
 
 #### 	2. 行情信息
 
 | 数据     | API                                         | 说明                                  | 备注                   |
 | -------- | ------------------------------------------- | ------------------------------------- | ---------------------- |
 | 分红信息 | stock.maket.get_dividend()                  | 获取单只股票的分红信息                |                        |
 | 股票行情 | stock.market.get_market()                   | 获取单只股票的行情信息-日、周、月 k线 |                        |
```

### Comparing `adata-0.0.8b0/adata.egg-info/SOURCES.txt` & `adata-0.0.9b0/adata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adata-0.0.8b0/setup.py` & `adata-0.0.9b0/setup.py`

 * *Files identical despite different names*

