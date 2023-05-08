# Comparing `tmp/zillionare_backtest-0.4.18.tar.gz` & `tmp/zillionare_backtest-0.4.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare_backtest-0.4.18.tar", max compression
+gzip compressed data, was "zillionare_backtest-0.4.19.tar", max compression
```

## Comparing `zillionare_backtest-0.4.18.tar` & `zillionare_backtest-0.4.19.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1068 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/LICENSE
--rw-r--r--   0        0        0     7504 2023-04-30 02:28:40.884883 zillionare_backtest-0.4.18/README.md
--rw-r--r--   0        0        0      114 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/__init__.py
--rw-r--r--   0        0        0     2160 2023-02-14 02:11:34.858631 zillionare_backtest-0.4.18/backtest/app.py
--rw-r--r--   0        0        0     2924 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/cli.py
--rw-r--r--   0        0        0        0 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/common/__init__.py
--rw-r--r--   0        0        0     2180 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/common/errors.py
--rw-r--r--   0        0        0     6281 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/common/helper.py
--rw-r--r--   0        0        0     1077 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/config/__init__.py
--rw-r--r--   0        0        0     1109 2023-05-01 07:03:53.365967 zillionare_backtest-0.4.18/backtest/config/defaults.yaml
--rw-r--r--   0        0        0      862 2023-05-01 08:43:15.780342 zillionare_backtest-0.4.18/backtest/config/dev.yaml
--rw-r--r--   0        0        0     1165 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/config/schema.py
--rw-r--r--   0        0        0      501 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/feed/__init__.py
--rw-r--r--   0        0        0     3423 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/feed/basefeed.py
--rw-r--r--   0        0        0     5422 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/feed/zillionarefeed.py
--rw-r--r--   0        0        0       62 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.18/backtest/trade/__init__.py
--rw-r--r--   0        0        0    48445 2023-05-01 09:23:29.569986 zillionare_backtest-0.4.18/backtest/trade/broker.py
--rw-r--r--   0        0        0     2989 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.18/backtest/trade/datatypes.py
--rw-r--r--   0        0        0     3999 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.18/backtest/trade/trade.py
--rw-r--r--   0        0        0     1100 2023-04-29 08:15:19.279077 zillionare_backtest-0.4.18/backtest/trade/transaction.py
--rw-r--r--   0        0        0       50 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.18/backtest/web/__init__.py
--rw-r--r--   0        0        0     4115 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.18/backtest/web/accounts.py
--rw-r--r--   0        0        0    13822 2023-04-30 02:15:22.554201 zillionare_backtest-0.4.18/backtest/web/interfaces.py
--rw-r--r--   0        0        0     3027 2023-05-01 09:42:52.723800 zillionare_backtest-0.4.18/pyproject.toml
--rw-r--r--   0        0        0     8067 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.18/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.18/tests/common/__init__.py
--rw-r--r--   0        0        0     1844 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.18/tests/common/test_helper.py
--rw-r--r--   0        0        0     3289 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.18/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   613076 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.18/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0      700 2023-04-29 14:40:00.305575 zillionare_backtest-0.4.18/tests/data/hljh_1d.csv
--rw-r--r--   0        0        0   163810 2023-04-29 14:37:20.922040 zillionare_backtest-0.4.18/tests/data/hljh_1m.csv
--rw-r--r--   0        0        0     1073 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.18/tests/data/limits.csv
--rw-r--r--   0        0        0      438 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.18/tests/data/readme.md
--rw-r--r--   0        0        0      665 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.18/tests/data/tyst_1d.csv
--rw-r--r--   0        0        0   156635 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/data/tyst_1m.csv
--rw-r--r--   0        0        0    11225 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/data/validation.xlsx
--rw-r--r--   0        0        0        0 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/feed/__init__.py
--rw-r--r--   0        0        0     8414 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/feed/test_zillionarefeed.py
--rw-r--r--   0        0        0      840 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/test_app.py
--rw-r--r--   0        0        0      650 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/test_cli.py
--rw-r--r--   0        0        0        0 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.18/tests/trade/__init__.py
--rw-r--r--   0        0        0    39691 2023-05-01 09:07:39.605377 zillionare_backtest-0.4.18/tests/trade/test_broker.py
--rw-r--r--   0        0        0        0 2023-02-06 14:55:38.172353 zillionare_backtest-0.4.18/tests/web/__init__.py
--rw-r--r--   0        0        0    19344 2023-05-01 09:28:17.262527 zillionare_backtest-0.4.18/tests/web/test_interfaces.py
--rw-r--r--   0        0        0    10047 1970-01-01 00:00:00.000000 zillionare_backtest-0.4.18/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/LICENSE
+-rw-r--r--   0        0        0     7504 2023-04-30 02:28:40.884883 zillionare_backtest-0.4.19/README.md
+-rw-r--r--   0        0        0      114 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/__init__.py
+-rw-r--r--   0        0        0     2160 2023-02-14 02:11:34.858631 zillionare_backtest-0.4.19/backtest/app.py
+-rw-r--r--   0        0        0     2924 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/cli.py
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/common/__init__.py
+-rw-r--r--   0        0        0     2180 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/common/errors.py
+-rw-r--r--   0        0        0     6281 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/common/helper.py
+-rw-r--r--   0        0        0     1077 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/config/__init__.py
+-rw-r--r--   0        0        0     1109 2023-05-01 07:03:53.365967 zillionare_backtest-0.4.19/backtest/config/defaults.yaml
+-rw-r--r--   0        0        0      862 2023-05-01 08:43:15.780342 zillionare_backtest-0.4.19/backtest/config/dev.yaml
+-rw-r--r--   0        0        0     1165 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/config/schema.py
+-rw-r--r--   0        0        0      501 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/feed/__init__.py
+-rw-r--r--   0        0        0     3423 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/feed/basefeed.py
+-rw-r--r--   0        0        0     5422 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/feed/zillionarefeed.py
+-rw-r--r--   0        0        0       62 2023-02-06 14:55:37.972351 zillionare_backtest-0.4.19/backtest/trade/__init__.py
+-rw-r--r--   0        0        0    48529 2023-05-08 07:31:21.226366 zillionare_backtest-0.4.19/backtest/trade/broker.py
+-rw-r--r--   0        0        0     2989 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.19/backtest/trade/datatypes.py
+-rw-r--r--   0        0        0     3999 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.19/backtest/trade/trade.py
+-rw-r--r--   0        0        0     1100 2023-04-29 08:15:19.279077 zillionare_backtest-0.4.19/backtest/trade/transaction.py
+-rw-r--r--   0        0        0       50 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.19/backtest/web/__init__.py
+-rw-r--r--   0        0        0     4115 2023-02-06 14:55:37.976351 zillionare_backtest-0.4.19/backtest/web/accounts.py
+-rw-r--r--   0        0        0    13822 2023-04-30 02:15:22.554201 zillionare_backtest-0.4.19/backtest/web/interfaces.py
+-rw-r--r--   0        0        0     3027 2023-05-08 07:32:22.678008 zillionare_backtest-0.4.19/pyproject.toml
+-rw-r--r--   0        0        0     8067 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.19/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.19/tests/common/__init__.py
+-rw-r--r--   0        0        0     1844 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.19/tests/common/test_helper.py
+-rw-r--r--   0        0        0     3289 2023-02-06 14:55:38.156353 zillionare_backtest-0.4.19/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   613076 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.19/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0      700 2023-04-29 14:40:00.305575 zillionare_backtest-0.4.19/tests/data/hljh_1d.csv
+-rw-r--r--   0        0        0   163810 2023-04-29 14:37:20.922040 zillionare_backtest-0.4.19/tests/data/hljh_1m.csv
+-rw-r--r--   0        0        0     1073 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.19/tests/data/limits.csv
+-rw-r--r--   0        0        0      438 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.19/tests/data/readme.md
+-rw-r--r--   0        0        0      665 2023-02-06 14:55:38.164353 zillionare_backtest-0.4.19/tests/data/tyst_1d.csv
+-rw-r--r--   0        0        0   156635 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.19/tests/data/tyst_1m.csv
+-rw-r--r--   0        0        0    11225 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.19/tests/data/validation.xlsx
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.19/tests/feed/__init__.py
+-rw-r--r--   0        0        0     8414 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.19/tests/feed/test_zillionarefeed.py
+-rw-r--r--   0        0        0      840 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.19/tests/test_app.py
+-rw-r--r--   0        0        0      650 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.19/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:38.168353 zillionare_backtest-0.4.19/tests/trade/__init__.py
+-rw-r--r--   0        0        0    39743 2023-05-08 07:42:14.242455 zillionare_backtest-0.4.19/tests/trade/test_broker.py
+-rw-r--r--   0        0        0        0 2023-02-06 14:55:38.172353 zillionare_backtest-0.4.19/tests/web/__init__.py
+-rw-r--r--   0        0        0    19405 2023-05-08 07:37:25.125550 zillionare_backtest-0.4.19/tests/web/test_interfaces.py
+-rw-r--r--   0        0        0    10047 1970-01-01 00:00:00.000000 zillionare_backtest-0.4.19/PKG-INFO
```

### Comparing `zillionare_backtest-0.4.18/LICENSE` & `zillionare_backtest-0.4.19/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/README.md` & `zillionare_backtest-0.4.19/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/app.py` & `zillionare_backtest-0.4.19/backtest/app.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/cli.py` & `zillionare_backtest-0.4.19/backtest/cli.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/common/errors.py` & `zillionare_backtest-0.4.19/backtest/common/errors.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/common/helper.py` & `zillionare_backtest-0.4.19/backtest/common/helper.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/config/__init__.py` & `zillionare_backtest-0.4.19/backtest/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/config/defaults.yaml` & `zillionare_backtest-0.4.19/backtest/config/defaults.yaml`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/config/dev.yaml` & `zillionare_backtest-0.4.19/backtest/config/dev.yaml`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/config/schema.py` & `zillionare_backtest-0.4.19/backtest/config/schema.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/feed/basefeed.py` & `zillionare_backtest-0.4.19/backtest/feed/basefeed.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/feed/zillionarefeed.py` & `zillionare_backtest-0.4.19/backtest/feed/zillionarefeed.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/trade/broker.py` & `zillionare_backtest-0.4.19/backtest/trade/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1273,15 +1273,15 @@
         """冻结账户，停止接收新的委托"""
         self._bt_stopped = True
 
     async def metrics(
         self,
         start: Optional[datetime.date] = None,
         end: Optional[datetime.date] = None,
-        baseline: Optional[str] = None,
+        baseline: Optional[str] = "399300.XSHE",
     ) -> Dict:
         """获取指定时间段的账户指标
 
         Args:
             start: 开始时间
             end: 结束时间
             baseline: 参考标的
@@ -1389,21 +1389,22 @@
 
             if ref_bars.size < 2:
                 ref_results = None
             else:
                 returns = ref_bars["close"][1:] / ref_bars["close"][:-1] - 1
 
                 ref_results = {
-                    "code": baseline,
+                    "total_profit_rate": cum_returns_final(returns),
                     "win_rate": np.count_nonzero(returns > 0) / len(returns),
+                    "mean_return": np.mean(returns).item(),
                     "sharpe": sharpe_ratio(returns, rf),
-                    "max_drawdown": max_drawdown(returns),
                     "sortino": sortino_ratio(returns, rf),
+                    "calmar": calmar_ratio(returns),
+                    "max_drawdown": max_drawdown(returns),
                     "annual_return": annual_return(returns),
-                    "total_profit_rate": cum_returns_final(returns),
                     "volatility": annual_volatility(returns),
                 }
         else:
             ref_results = None
 
         return {
             "start": start,
```

### Comparing `zillionare_backtest-0.4.18/backtest/trade/datatypes.py` & `zillionare_backtest-0.4.19/backtest/trade/datatypes.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/trade/trade.py` & `zillionare_backtest-0.4.19/backtest/trade/trade.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/trade/transaction.py` & `zillionare_backtest-0.4.19/backtest/trade/transaction.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/web/accounts.py` & `zillionare_backtest-0.4.19/backtest/web/accounts.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/backtest/web/interfaces.py` & `zillionare_backtest-0.4.19/backtest/web/interfaces.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/pyproject.toml` & `zillionare_backtest-0.4.19/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "zillionare-backtest"
-version = "0.4.18"
+version = "0.4.19"
 homepage = "https://github.com/zillionare/backtest"
 description = "zillionare backtest framework."
 authors = ["Aaron Yang <aaron_yang@jieyu.ai>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `zillionare_backtest-0.4.18/tests/__init__.py` & `zillionare_backtest-0.4.19/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/common/test_helper.py` & `zillionare_backtest-0.4.19/tests/common/test_helper.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/data/bars_1d.pkl` & `zillionare_backtest-0.4.19/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/data/bars_1m.pkl` & `zillionare_backtest-0.4.19/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/data/hljh_1d.csv` & `zillionare_backtest-0.4.19/tests/data/hljh_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/data/hljh_1m.csv` & `zillionare_backtest-0.4.19/tests/data/hljh_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/data/limits.csv` & `zillionare_backtest-0.4.19/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/data/tyst_1d.csv` & `zillionare_backtest-0.4.19/tests/data/tyst_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/data/tyst_1m.csv` & `zillionare_backtest-0.4.19/tests/data/tyst_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/data/validation.xlsx` & `zillionare_backtest-0.4.19/tests/data/validation.xlsx`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/feed/test_zillionarefeed.py` & `zillionare_backtest-0.4.19/tests/feed/test_zillionarefeed.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/test_app.py` & `zillionare_backtest-0.4.19/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/test_cli.py` & `zillionare_backtest-0.4.19/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `zillionare_backtest-0.4.18/tests/trade/test_broker.py` & `zillionare_backtest-0.4.19/tests/trade/test_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,21 +531,22 @@
             "sharpe": -1.396890251070207,
             "sortino": -2.0486727998320817,
             "calmar": -2.422741706100782,
             "max_drawdown": -0.0041827334569883405,
             "annual_return": -0.010133682791748755,
             "volatility": 0.02850594795764624,
             "baseline": {
-                "code": "002537.XSHE",
+                "total_profit_rate": 0.006315946578979492,
                 "win_rate": 0.5555555555555556,
+                "mean_return": 0.0028306511,
                 "sharpe": 0.6190437353475076,
-                "max_drawdown": -0.17059373779725692,
                 "sortino": 1.0015572769806516,
+                "calmar": 1.1300787322194514,
+                "max_drawdown": -0.17059373779725692,
                 "annual_return": 0.19278435493450163,
-                "total_profit_rate": 0.006315946578979492,
                 "volatility": 1.1038380776228978,
             },
         }
 
         assert_deep_almost_equal(self, actual, exp, places=4)
 
     async def test_assets(self):
```

### Comparing `zillionare_backtest-0.4.18/tests/web/test_interfaces.py` & `zillionare_backtest-0.4.19/tests/web/test_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,21 +344,22 @@
             "sharpe": -1.396890251070207,
             "sortino": -2.0486727998320817,
             "calmar": -2.422741706100782,
             "max_drawdown": -0.0041827334569883405,
             "annual_return": -0.010133682791748755,
             "volatility": 0.02850594795764624,
             "baseline": {
-                "code": "002537.XSHE",
+                "total_profit_rate": 0.006315946578979492,
                 "win_rate": 0.5555555555555556,
+                "mean_return": 0.0028306511230766773,
                 "sharpe": 0.6190437353475076,
-                "max_drawdown": -0.17059373779725692,
                 "sortino": 1.0015572769806516,
+                "calmar": 1.1300787322194514,
+                "max_drawdown": -0.17059373779725692,
                 "annual_return": 0.19278435493450163,
-                "total_profit_rate": 0.006315946578979492,
                 "volatility": 1.1038380776228978,
             },
         }
         assert_deep_almost_equal(self, exp, actual, places=2)
 
         assets = await get("assets", self.token)
         self.assertEqual(assets["date"][0], datetime.date(2022, 3, 1))
```

### Comparing `zillionare_backtest-0.4.18/PKG-INFO` & `zillionare_backtest-0.4.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-backtest
-Version: 0.4.18
+Version: 0.4.19
 Summary: zillionare backtest framework.
 Home-page: https://github.com/zillionare/backtest
 License: MIT
 Author: Aaron Yang
 Author-email: aaron_yang@jieyu.ai
 Requires-Python: >=3.8,<3.9
 Classifier: Development Status :: 2 - Pre-Alpha
```

